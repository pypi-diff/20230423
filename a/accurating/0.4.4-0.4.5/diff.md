# Comparing `tmp/accurating-0.4.4.tar.gz` & `tmp/accurating-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.4.tar", max compression
+gzip compressed data, was "accurating-0.4.5.tar", max compression
```

## Comparing `accurating-0.4.4.tar` & `accurating-0.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.4/LICENSE
--rw-r--r--   0        0        0     6186 2023-04-23 17:18:31.113038 accurating-0.4.4/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.4/accurating/__init__.py
--rw-r--r--   0        0        0     8429 2023-04-23 19:11:22.260259 accurating-0.4.4/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.4/accurating/tests/__init__.py
--rw-r--r--   0        0        0     2491 2023-04-17 06:02:22.018441 accurating-0.4.4/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-23 19:14:15.668960 accurating-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 accurating-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.5/LICENSE
+-rw-r--r--   0        0        0     6245 2023-04-23 19:14:57.625128 accurating-0.4.5/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.5/accurating/__init__.py
+-rw-r--r--   0        0        0     8408 2023-04-23 21:36:25.105635 accurating-0.4.5/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.5/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     2491 2023-04-23 19:19:28.850193 accurating-0.4.5/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-23 21:50:03.229146 accurating-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     6853 1970-01-01 00:00:00.000000 accurating-0.4.5/PKG-INFO
```

### Comparing `accurating-0.4.4/LICENSE` & `accurating-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.4/README.md` & `accurating-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -124,8 +124,11 @@
 
 ## Development
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
+# edit stuff; increase version
+poetry build
+poetry publish
 ```
```

### Comparing `accurating-0.4.4/accurating/model.py` & `accurating-0.4.5/accurating/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,21 +90,16 @@
     """It is automatically adjusted, but sometimes it is too large and blows up."""
 
 
 @dataclasses.dataclass
 class Model:
     """Trained model."""
 
-    rating: np.ndarray
-    """Currently the seasons have to be small integers.
-    rating contains players' rating at each timestam
-    rating has a shape (player_count, max(season)-1)."""
-
-    player_name: list[str] | None
-    """Indexed with player id (length player_count). Not used in the training."""
+    rating: dict[tuple[str, int], float]
+    """Player rating, indexed by name and season"""
 
 
 def fit(
     data: MatchResultArrays,
     config: Config,
 ) -> Model:
     """Fits the model to data according to config.
@@ -150,37 +145,29 @@
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
         # return jnp.mean(winner_win_prob_log) - 0.005*jnp.mean(cons ** 2)
 
     # Optimize for these params:
     rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
-    params = dataclasses.asdict(Model(rating=rating, player_name=None))
+    params = dataclasses.asdict(Model(rating=rating))
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
-    lr = config.initial_lr
+    lr = float(config.initial_lr)
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
     last_eval = -2  # eval of initial data is -1
     last_grad = tree_map(jnp.zeros_like, params)
     last_reset_step = 0
 
     for i in range(config.max_steps):
         (eval, model_fit), grad = jax.value_and_grad(model, has_aux=True)(params)
 
-        ratings = grad['rating']
-        q = jnp.sum(params['rating'] == last_params['rating']
-                    ) / params['rating'].size
-        if config.do_log:
-            print(
-                f'Step {i:4}: eval: {jnp.exp2(eval):0.12f} lr={lr:4.4f} grad={jnp.linalg.norm(ratings):2.4f} q={q:0.3f}')
-        if i > 1 and q > 0.99:
-            break
         if False:
             # Standard batch gradient descent algorithm works too. Just use good LR.
             params = tree_map(lambda p, g: p + lr * g, params, grad)
         else:
             if eval < last_eval:
                 if config.do_log:
                     print(f'reset to {jnp.exp2(last_eval)}')
@@ -188,20 +175,41 @@
                 if last_reset_step == i-1:
                     lr /= 4
                 last_reset_step = i
                 momentum = tree_map(jnp.zeros_like, params)
                 # momentum /= 2.
                 params, eval, grad = last_params, last_eval, last_grad
             else:
-                if (i - last_reset_step) % 12 == 0:
-                    lr *= 1.5
                 last_params, last_eval, last_grad = params, eval, grad
             momentum = tree_map(lambda m, g: m_lr * m + g, momentum, grad)
             params = tree_map(lambda p, m: p + lr * m, params, momentum)
-    return Model(rating=params['rating'], player_name=data.player_name)
+
+        max_d_rating = jnp.max(
+            jnp.abs(params['rating'] - last_params['rating']))
+
+        if config.do_log:
+            g = jnp.linalg.norm(grad['rating'])
+            print(
+                f'Step {i:4}: eval: {jnp.exp2(eval):0.12f} lr={lr: 4.4f} grad={g:2.4f} delta={max_d_rating}')
+
+        if max_d_rating < 1e-15:
+            break
+
+        lr *= 1.5 ** (1.0 / 12)
+
+    def postprocess():
+        rating = {}
+        for id, name in enumerate(data.player_name):
+            rating[name] = {}
+            for season in range(season_count):
+                rating[name][season] = float(params['rating'][id, season])
+        ret = Model(rating=rating)
+        return ret
+
+    return postprocess()
 
 
 def data_from_dicts(matches) -> MatchResultArrays:
     player_set = set()
 
     for match in matches:
         player_set.add(match['p1'])
```

### Comparing `accurating-0.4.4/accurating/tests/model_test.py` & `accurating-0.4.5/accurating/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.4/pyproject.toml` & `accurating-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.4"
+version = "0.4.5"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.4.4/PKG-INFO` & `accurating-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.4
+Version: 0.4.5
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -140,9 +140,12 @@
 
 ## Development
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
+# edit stuff; increase version
+poetry build
+poetry publish
 ```
```

