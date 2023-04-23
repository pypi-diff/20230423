# Comparing `tmp/accurating-0.4.3.tar.gz` & `tmp/accurating-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.3.tar", max compression
+gzip compressed data, was "accurating-0.4.4.tar", max compression
```

## Comparing `accurating-0.4.3.tar` & `accurating-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.3/LICENSE
--rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.3/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.3/accurating/__init__.py
--rw-r--r--   0        0        0     8407 2023-04-17 05:13:50.431970 accurating-0.4.3/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.3/accurating/tests/__init__.py
--rw-r--r--   0        0        0     2471 2023-04-17 05:14:30.265058 accurating-0.4.3/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-17 05:29:08.737759 accurating-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 accurating-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6186 2023-04-23 17:18:31.113038 accurating-0.4.4/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.4/accurating/__init__.py
+-rw-r--r--   0        0        0     8429 2023-04-23 19:11:22.260259 accurating-0.4.4/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.4/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     2491 2023-04-17 06:02:22.018441 accurating-0.4.4/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-23 19:14:15.668960 accurating-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 accurating-0.4.4/PKG-INFO
```

### Comparing `accurating-0.4.3/LICENSE` & `accurating-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.3/README.md` & `accurating-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AccuRating
 
 Library computing accurate ratings based on match results.
 
-## Usage
-
-Take a look at the unit test.
+- [Documentation](https://lukaszlew.github.io/accurating/accurating.html)
+- [Package](https://pypi.org/project/accurating/)
+- [Usage example](https://github.com/lukaszlew/accurating/blob/main/accurating/tests/model_test.py#L50)
 
 ## Is AccuRating accurate?
 
 Yes. With the same data, AccuRating will return much more accurate ratings than chess ELO or EGD.
 For instance if a player Leon manages to win against player Caesar, Leon will "get" some X points for that victory.
 If later Caesar will win against strong players Alusia and EmCee, his rating will increase, but that would not affect Leon's rating in chess or EGD.
 If we want to use data efficienty Leon's rating should be adjusted because Caesar clearly demonstrated his power and it was not long ago that poor Leon lucked out a victory against Caesar.
@@ -37,15 +37,15 @@
 - 240.824 chess ELO difference for 1:5 win odds (20% vs 80%)
 - 361.236 chess ELO difference for 1:10 win odds (10% vs 90%)
 
 The Chess ELO formula is $P(win) = 1 / (1 + 10^{d / 400})$
 
 ### Compared to EGD
 
-In EGD, winning odds for 100 points of rating is not fixed.
+[In EGD, winning odds for 100 points of rating is not fixed.](http://goratings.eu/Home/About)
 This is beacuse: 1 dan/kyu difference = 100 EGD = 1 handicap.
 The nature of Go is that 1 handicap (i.e. 100 EGD) means more on a dan level than on a kyu level.
 
 On the dan level:
 
 - 90 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 180 EGD point difference is approximately 1:5 win odds (20% vs 80%)
```

### Comparing `accurating-0.4.3/accurating/model.py` & `accurating-0.4.4/accurating/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,38 +150,37 @@
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
         # return jnp.mean(winner_win_prob_log) - 0.005*jnp.mean(cons ** 2)
 
     # Optimize for these params:
     rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
-    params = dataclasses.asdict(
-        Model(rating=rating, player_name=None))
+    params = dataclasses.asdict(Model(rating=rating, player_name=None))
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
     lr = config.initial_lr
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
-    last_eval = -1
+    last_eval = -2  # eval of initial data is -1
     last_grad = tree_map(jnp.zeros_like, params)
     last_reset_step = 0
 
     for i in range(config.max_steps):
         (eval, model_fit), grad = jax.value_and_grad(model, has_aux=True)(params)
 
+        ratings = grad['rating']
+        q = jnp.sum(params['rating'] == last_params['rating']
+                    ) / params['rating'].size
         if config.do_log:
-            ratings = grad['rating']
-            q = jnp.sum(params['rating'] ==
-                        last_params['rating']) / params['rating'].size
-            if i > 100 and q > 0.9:
-                break
             print(
-                f'Step {i:4}: eval: {jnp.exp2(eval)} lr={lr:7} grad={jnp.linalg.norm(ratings)} {q}')
+                f'Step {i:4}: eval: {jnp.exp2(eval):0.12f} lr={lr:4.4f} grad={jnp.linalg.norm(ratings):2.4f} q={q:0.3f}')
+        if i > 1 and q > 0.99:
+            break
         if False:
             # Standard batch gradient descent algorithm works too. Just use good LR.
             params = tree_map(lambda p, g: p + lr * g, params, grad)
         else:
             if eval < last_eval:
                 if config.do_log:
                     print(f'reset to {jnp.exp2(last_eval)}')
```

### Comparing `accurating-0.4.3/accurating/tests/model_test.py` & `accurating-0.4.4/accurating/tests/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
 def test_fit():
     true_elos = jnp.array([[8.0, 4.0], [2.0, 3.0], [0.0, 0.0],])
     test_data = get_test_data(true_elos)
     config = accurating.Config(
         season_rating_stability=0.0,
         smoothing=0.0,
-        max_steps=100,
+        max_steps=300,
         do_log=True,
     )
     model = accurating.fit(test_data, config)
     elos = model.rating
     elos = elos - jnp.min(elos, axis=0, keepdims=True)
     err = jnp.linalg.norm(elos - jnp.array(true_elos))
-    assert err < 0.0001, f'FAIL err={err}; results={model}'
+    assert err < 0.000001, f'FAIL err={err}; results={model}'
 
 
 def test_data_from_dicts():
     json_str = """
     [
       {
         "p1": "Leon",
@@ -81,11 +81,16 @@
 
     assert data.player_name == player_name
     assert_array_equal(data.p1, p1)
     assert_array_equal(data.p2, p2)
     assert_array_equal(data.p1_win_prob, p1_win_prob)
     assert_array_equal(data.season, season)
 
-    cfg = accurating.Config(season_rating_stability=0.5,
-                            smoothing=0.1, max_steps=5, do_log=True, initial_lr=1.0,)
+    cfg = accurating.Config(
+        season_rating_stability=0.5,
+        smoothing=0.1,
+        max_steps=5,
+        do_log=True,
+        initial_lr=1.0,
+    )
     model = accurating.fit(data, cfg)
     del model
```

### Comparing `accurating-0.4.3/pyproject.toml` & `accurating-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.3"
+version = "0.4.4"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.4.3/PKG-INFO` & `accurating-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.3
+Version: 0.4.4
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -14,17 +14,17 @@
 Project-URL: Documentation, https://lukaszlew.github.io/accurating/
 Description-Content-Type: text/markdown
 
 # AccuRating
 
 Library computing accurate ratings based on match results.
 
-## Usage
-
-Take a look at the unit test.
+- [Documentation](https://lukaszlew.github.io/accurating/accurating.html)
+- [Package](https://pypi.org/project/accurating/)
+- [Usage example](https://github.com/lukaszlew/accurating/blob/main/accurating/tests/model_test.py#L50)
 
 ## Is AccuRating accurate?
 
 Yes. With the same data, AccuRating will return much more accurate ratings than chess ELO or EGD.
 For instance if a player Leon manages to win against player Caesar, Leon will "get" some X points for that victory.
 If later Caesar will win against strong players Alusia and EmCee, his rating will increase, but that would not affect Leon's rating in chess or EGD.
 If we want to use data efficienty Leon's rating should be adjusted because Caesar clearly demonstrated his power and it was not long ago that poor Leon lucked out a victory against Caesar.
@@ -53,15 +53,15 @@
 - 240.824 chess ELO difference for 1:5 win odds (20% vs 80%)
 - 361.236 chess ELO difference for 1:10 win odds (10% vs 90%)
 
 The Chess ELO formula is $P(win) = 1 / (1 + 10^{d / 400})$
 
 ### Compared to EGD
 
-In EGD, winning odds for 100 points of rating is not fixed.
+[In EGD, winning odds for 100 points of rating is not fixed.](http://goratings.eu/Home/About)
 This is beacuse: 1 dan/kyu difference = 100 EGD = 1 handicap.
 The nature of Go is that 1 handicap (i.e. 100 EGD) means more on a dan level than on a kyu level.
 
 On the dan level:
 
 - 90 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 180 EGD point difference is approximately 1:5 win odds (20% vs 80%)
```

