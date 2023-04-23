# Comparing `tmp/truegrad-4.0.1.tar.gz` & `tmp/truegrad-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truegrad-4.0.1.tar", last modified: Sun Apr 23 06:13:58 2023, max compression
+gzip compressed data, was "truegrad-4.0.2.tar", last modified: Sun Apr 23 06:16:43 2023, max compression
```

## Comparing `truegrad-4.0.1.tar` & `truegrad-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:13:58.283375 truegrad-4.0.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-4.0.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:13:58.283375 truegrad-4.0.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-4.0.1/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-04-23 06:13:58.283375 truegrad-4.0.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1092 2023-04-23 06:12:22.000000 truegrad-4.0.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:13:58.283375 truegrad-4.0.1/truegrad/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-4.0.1/truegrad/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-4.0.1/truegrad/functional.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:13:58.283375 truegrad-4.0.1/truegrad/nn/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-4.0.1/truegrad/nn/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-4.0.1/truegrad/nn/functional.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    19866 2023-04-23 06:12:22.000000 truegrad-4.0.1/truegrad/optim.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7199 2023-04-22 19:54:25.000000 truegrad-4.0.1/truegrad/test.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-4.0.1/truegrad/utils.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:13:58.283375 truegrad-4.0.1/truegrad.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:13:58.000000 truegrad-4.0.1/truegrad.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-04-23 06:13:58.000000 truegrad-4.0.1/truegrad.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-23 06:13:58.000000 truegrad-4.0.1/truegrad.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-04-23 06:13:58.000000 truegrad-4.0.1/truegrad.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-4.0.2/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:16:43.011005 truegrad-4.0.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-4.0.2/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-04-23 06:16:43.011005 truegrad-4.0.2/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1092 2023-04-23 06:16:40.000000 truegrad-4.0.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/functional.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad/nn/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/nn/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/nn/functional.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    19262 2023-04-23 06:16:01.000000 truegrad-4.0.2/truegrad/optim.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7199 2023-04-22 19:54:25.000000 truegrad-4.0.2/truegrad/test.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/utils.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/top_level.txt
```

### Comparing `truegrad-4.0.1/LICENSE` & `truegrad-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/PKG-INFO` & `truegrad-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 4.0.1
+Version: 4.0.2
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truegrad-4.0.1/README.md` & `truegrad-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/setup.py` & `truegrad-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.truegrad@nestler.sh",
     name='truegrad',
     license='BSD',
     description='PyTorch interface for TrueGrad-AdamW',
-    version='4.0.1',
+    version='4.0.2',
     long_description=README,
     url='https://github.com/clashluke/truegrad',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

### Comparing `truegrad-4.0.1/truegrad/functional.py` & `truegrad-4.0.2/truegrad/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/truegrad/nn/__init__.py` & `truegrad-4.0.2/truegrad/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/truegrad/nn/functional.py` & `truegrad-4.0.2/truegrad/nn/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/truegrad/optim.py` & `truegrad-4.0.2/truegrad/optim.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,24 +111,14 @@
     return base.sqrt().clamp(min=eps)
 
 
 def div_ema(base: Tensor, eps: float, base_sq: Tensor, update_sq: Tensor, beta_sq: float, step: Optional[int] = None):
     return base / stable_sqrt(ema_(base_sq, update_sq, beta_sq, step), eps)
 
 
-def decay_weight_(state: Dict[str, Any], param: torch.nn.Parameter, group: Dict[str, Any]):
-    if group["decay_to_init"]:
-        if "param_at_init" not in state:
-            state["param_at_init"] = torch.clone(param.detach())
-        else:
-            param.add_(state["param_at_init"] - param, alpha=group["weight_decay"] * group["lr"])
-    else:
-        param.mul_(1 - group["weight_decay"] * group["lr"])
-
-
 def _default_decay(weight_decay_cls: Optional[WeightDecayChain]) -> WeightDecayChain:
     if weight_decay_cls is None:
         return WeightDecayChain(L2WeightDecay())
     return weight_decay_cls
 
 
 class OptimizerOptimizer(torch.optim.Optimizer):
@@ -149,24 +139,23 @@
 
     @torch.no_grad()
     def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
 
-        self.weight_decay_cls(self)
-
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
                 if "lr" in state:
                     group["lr"] = state["lr"]
-                    decay_weight_(state, p, group)
                 state["param"] = torch.clone(p.detach())
 
+        self.weight_decay_cls(self)
+
         self.inner_optimizer.step()
 
         for group in self.inner_optimizer.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
                 state = self.state[p]
@@ -326,16 +315,14 @@
                         state[s] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     if not do_base:
                         for s in self.true_statistics:
                             state[s] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     if do_base or group["graft"]:
                         for s in self.base_statistics:
                             state[s] = torch.zeros_like(p, memory_format=torch.preserve_format)
-                    if group["decay_to_init"]:
-                        state["init"] = torch.clone(p.detach())
 
                 step_t = state['step']
                 step_t += 1
 
                 self.weight_decay_cls(self)
 
                 step = step_t.item()
@@ -389,15 +376,15 @@
 
 class TGLaProp(TrueGrad):
     true_statistics: List[str] = ["exp_avg_true", "exp_avg_true_sq"]
     base_statistics: List[str] = ["exp_avg", "exp_avg_sq"]
 
     def __init__(self, params, lr: float = 1e-3,
                  betas: Union[Tuple[float, float], Tuple[float, float, float, float]] = (0.9, 0.99), eps: float = 1e-12,
-                 weight_decay: float = 1e-2, graft: bool = True, decay_to_init: bool = False,
+                 weight_decay: float = 1e-2, graft: bool = True,
                  default_to_baseline: bool = False, enforce_baseline: bool = False,
                  weight_decay_cls: Optional[WeightDecayChain] = None):
         super().__init__(params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, graft=graft,
                          default_to_baseline=default_to_baseline, enforce_baseline=enforce_baseline,
                          weight_decay_cls=weight_decay_cls)
 
     def _inner(self, step: int, p: Parameter, group: Dict[str, Any], exp_avg: Optional[Tensor] = None,
```

### Comparing `truegrad-4.0.1/truegrad/test.py` & `truegrad-4.0.2/truegrad/test.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/truegrad/utils.py` & `truegrad-4.0.2/truegrad/utils.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.1/truegrad.egg-info/PKG-INFO` & `truegrad-4.0.2/truegrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 4.0.1
+Version: 4.0.2
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

