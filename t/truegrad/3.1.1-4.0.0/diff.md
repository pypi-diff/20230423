# Comparing `tmp/truegrad-3.1.1.tar.gz` & `tmp/truegrad-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truegrad-3.1.1.tar", last modified: Sat Mar 18 16:47:15 2023, max compression
+gzip compressed data, was "truegrad-4.0.0.tar", last modified: Sun Apr 23 06:02:52 2023, max compression
```

## Comparing `truegrad-3.1.1.tar` & `truegrad-4.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-18 16:47:15.260648 truegrad-3.1.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-3.1.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-03-18 16:47:15.260648 truegrad-3.1.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-3.1.1/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-03-18 16:47:15.260648 truegrad-3.1.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1092 2023-03-18 16:46:59.000000 truegrad-3.1.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-18 16:47:15.260648 truegrad-3.1.1/truegrad/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-3.1.1/truegrad/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-3.1.1/truegrad/functional.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-18 16:47:15.260648 truegrad-3.1.1/truegrad/nn/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-3.1.1/truegrad/nn/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-3.1.1/truegrad/nn/functional.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    17924 2023-03-18 16:46:59.000000 truegrad-3.1.1/truegrad/optim.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     5568 2023-03-18 16:42:50.000000 truegrad-3.1.1/truegrad/test.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-3.1.1/truegrad/utils.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-18 16:47:15.260648 truegrad-3.1.1/truegrad.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-03-18 16:47:15.000000 truegrad-3.1.1/truegrad.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-03-18 16:47:15.000000 truegrad-3.1.1/truegrad.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-03-18 16:47:15.000000 truegrad-3.1.1/truegrad.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-03-18 16:47:15.000000 truegrad-3.1.1/truegrad.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:02:52.042276 truegrad-4.0.0/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-4.0.0/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:02:52.042276 truegrad-4.0.0/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-4.0.0/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-04-23 06:02:52.042276 truegrad-4.0.0/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1092 2023-04-22 16:48:57.000000 truegrad-4.0.0/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:02:52.042276 truegrad-4.0.0/truegrad/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-4.0.0/truegrad/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-4.0.0/truegrad/functional.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:02:52.042276 truegrad-4.0.0/truegrad/nn/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-4.0.0/truegrad/nn/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-4.0.0/truegrad/nn/functional.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    19699 2023-04-22 17:22:16.000000 truegrad-4.0.0/truegrad/optim.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7199 2023-04-22 19:54:25.000000 truegrad-4.0.0/truegrad/test.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-4.0.0/truegrad/utils.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:02:52.042276 truegrad-4.0.0/truegrad.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:02:52.000000 truegrad-4.0.0/truegrad.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-04-23 06:02:52.000000 truegrad-4.0.0/truegrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-23 06:02:52.000000 truegrad-4.0.0/truegrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-04-23 06:02:52.000000 truegrad-4.0.0/truegrad.egg-info/top_level.txt
```

### Comparing `truegrad-3.1.1/LICENSE` & `truegrad-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/PKG-INFO` & `truegrad-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 3.1.1
+Version: 4.0.0
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truegrad-3.1.1/README.md` & `truegrad-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/setup.py` & `truegrad-4.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.truegrad@nestler.sh",
     name='truegrad',
     license='BSD',
     description='PyTorch interface for TrueGrad-AdamW',
-    version='3.1.1',
+    version='4.0.0',
     long_description=README,
     url='https://github.com/clashluke/truegrad',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

### Comparing `truegrad-3.1.1/truegrad/functional.py` & `truegrad-4.0.0/truegrad/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/truegrad/nn/__init__.py` & `truegrad-4.0.0/truegrad/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/truegrad/nn/functional.py` & `truegrad-4.0.0/truegrad/nn/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/truegrad/optim.py` & `truegrad-4.0.0/truegrad/optim.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,104 @@
+import functools
 import warnings
 from typing import Tuple, Union, List, Dict, Any, Optional
 
 import torch
 from torch import Tensor
 from torch.nn import Parameter
 
 
+class WeightDecayBase:
+    def __init__(self):
+        pass
+
+    def __call__(self, mod: torch.optim.Optimizer, p: torch.Tensor, idx: int):
+        return p
+
+
+class WeightDecayChain:
+    def __init__(self, *operands: WeightDecayBase):
+        self.operands = operands
+
+    def __call__(self, mod: torch.optim.Optimizer):
+        idx = 0
+        for group in mod.param_groups:
+            for p in group["params"]:
+                p.data.add_(functools.reduce(lambda x, f: f(mod, x, idx), self.operands, p),
+                            alpha=-group["lr"] * group["weight_decay"])
+                idx += 1
+
+
+class LpWeightDecay(WeightDecayBase):
+    def __init__(self, power: float):
+        self.power = power
+
+    def __call__(self, mod: torch.optim.Optimizer, p: Tensor, idx: int):
+        return p.abs().pow(self.power) * p.sign()
+
+
+class L1WeightDecay(LpWeightDecay):
+    def __init__(self):
+        super().__init__(0)
+
+
+class L2WeightDecay(LpWeightDecay):
+    def __init__(self):
+        super().__init__(1)
+
+
+def _param_iterator(mod: torch.optim.Optimizer):
+    yield from (p.detach().clone() for group in mod.param_groups for p in group["params"])
+
+
+class WeightDecayToValue(WeightDecayBase):
+    def __init__(self):
+        self.target_values: List[Tensor] = ...
+        self.global_step = 0
+
+    def _on_step_start(self, mod: torch.optim.Optimizer):
+        pass
+
+    def _on_global_start(self, mod: torch.optim.Optimizer):
+        pass
+
+    def _preprocess(self, target: Tensor):
+        return target
+
+    def __call__(self, mod: torch.optim.Optimizer, p: Tensor, idx: int):
+        if idx == 0:
+            if self.global_step == 0:
+                self._on_global_start(mod)
+            self._on_step_start(mod)
+            self.global_step += 1
+        return p - self._preprocess(self.target_values[idx])
+
+
+class WeightDecayToInit(WeightDecayToValue):
+    def _on_global_start(self, mod: torch.optim.Optimizer):
+        self.target_values = list(_param_iterator(mod))
+
+
+class WeightDecayToEMA(WeightDecayToInit):
+    def __init__(self, beta: float = 0.999):
+        super().__init__()
+        self.beta = beta
+
+    def _on_global_start(self, mod: torch.optim.Optimizer):
+        self.target_values = [torch.zeros_like(x) for x in _param_iterator(mod)]
+
+    def _on_step_start(self, mod: torch.optim.Optimizer):
+        self.global_step += 1
+        for v, p in zip(self.target_values, _param_iterator(mod)):
+            v.mul_(self.beta).add_(p, alpha=1 - self.beta)
+
+    def _preprocess(self, target: Tensor):
+        return target / (1 - self.beta ** self.global_step)
+
+
 def ema_(base: Tensor, update: Tensor, beta: float, step: Optional[int] = None):
     base.mul_(beta).add_(update, alpha=1 - beta)
     if step is None:
         return base
     return base / (1 - beta ** step)
 
 
@@ -27,36 +116,44 @@
             state["param_at_init"] = torch.clone(param.detach())
         else:
             param.add_(state["param_at_init"] - param, alpha=group["weight_decay"] * group["lr"])
     else:
         param.mul_(1 - group["weight_decay"] * group["lr"])
 
 
+def _default_decay(weight_decay_cls: Optional[WeightDecayChain]) -> WeightDecayChain:
+    if weight_decay_cls is None:
+        return WeightDecayChain(L2WeightDecay())
+    return weight_decay_cls
+
+
 class OptimizerOptimizer(torch.optim.Optimizer):
     def __init__(self, params, inner_optimizer: torch.optim.Optimizer, learning_rate_learning_rate: float = 1,
-                 weight_decay: float = 0, decay_to_init: bool = False):
-        self.learning_rate_learning_rate = learning_rate_learning_rate
-
+                 weight_decay: float = 0, weight_decay_cls: Optional[WeightDecayChain] = None):
         self.inner_optimizer = inner_optimizer
+        self.learning_rate_learning_rate = learning_rate_learning_rate
+        self.weight_decay_cls = _default_decay(weight_decay_cls)
         param_groups = self.inner_optimizer.param_groups
         self.inner_optimizer.param_groups = []
         for group in param_groups:
             for param in group["params"]:
                 group = {k: v for k, v in group.items() if k != "params"}
                 group["params"] = [param]
                 self.inner_optimizer.param_groups.append(group)
 
-        super(OptimizerOptimizer, self).__init__(params, {"weight_decay": weight_decay, "decay_to_init": decay_to_init})
+        super(OptimizerOptimizer, self).__init__(params, {"weight_decay": weight_decay})
 
     @torch.no_grad()
     def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
 
+        self.weight_decay_cls(self)
+
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
                 if "lr" in state:
                     group["lr"] = state["lr"]
                     decay_weight_(state, p, group)
                 state["param"] = torch.clone(p.detach())
@@ -76,36 +173,31 @@
                 state["old_update"] = torch.clone(update.to(torch.bfloat16).detach())
                 state["param"] = None
 
         return loss
 
 
 class Sign(torch.optim.Optimizer):
-    def __init__(self, params, base: torch.optim.Optimizer, lr: float = 1, weight_decay: float = 0,
-                 decay_to_init: bool = False, eps: float = 1e-12, graft_to_self: bool = True):
-        super().__init__(params, {"weight_decay": weight_decay, "decay_to_init": decay_to_init, "lr": lr, "eps": eps,
-                                  "graft_to_self": graft_to_self})
+    def __init__(self, params, base: torch.optim.Optimizer, lr: float = 1, weight_decay: float = 0, eps: float = 1e-12,
+                 graft_to_self: bool = True, weight_decay_cls: Optional[WeightDecayChain] = None):
+        self.weight_decay_cls = _default_decay(weight_decay_cls)
+
+        super().__init__(params, {"weight_decay": weight_decay, "lr": lr, "eps": eps, "graft_to_self": graft_to_self})
         self.base = base
 
     @torch.no_grad()
     def step(self, closure=None):
         if closure is None:
             loss = None
         else:
             with torch.enable_grad():
                 loss = closure()
 
-        params_flat = []
-        for group in self.param_groups:
-            for p in group["params"]:
-                params_flat.append(p)
-                decay_weight_(self.state[p], p, group)
-
-        params_flat = [torch.clone(p.detach()) for p in params_flat]
-
+        self.weight_decay_cls(self)
+        params_flat = list(_param_iterator(self))
         self.base.step()
 
         for group in self.param_groups:
             for p in group["params"]:
                 o = params_flat.pop(0)
                 update = p.double() - o.double()
                 p.set_(o)
@@ -146,34 +238,31 @@
     >>> opt = Graft(model.parameters(), magnitude_from, direction_from, weight_decay=0.1)
     >>> model(torch.randn((16, 10))).mean().backward()  # get some random gradients
     >>> opt.step()  # apply as usual
     >>> opt.zero_grad()
     """
 
     def __init__(self, params, magnitude: torch.optim.Optimizer, direction: torch.optim.Optimizer,
-                 weight_decay: float = 0, decay_to_init: bool = False, eps: float = 1e-12, lr: float = 1):
-        super().__init__(params, {"weight_decay": weight_decay, "decay_to_init": decay_to_init, "lr": lr, "eps": eps})
+                 weight_decay: float = 0, eps: float = 1e-12, lr: float = 1,
+                 weight_decay_cls: Optional[WeightDecayChain] = None):
+        super().__init__(params, {"weight_decay": weight_decay, "lr": lr, "eps": eps})
         self.magnitude = magnitude
         self.direction = direction
+        self.weight_decay_cls = _default_decay(weight_decay_cls)
 
     @torch.no_grad()
     def step(self, closure=None):
         if closure is None:
             loss = None
         else:
             with torch.enable_grad():
                 loss = closure()
 
-        params_flat = []
-        for group in self.param_groups:
-            for p in group["params"]:
-                params_flat.append(p)
-                decay_weight_(self.state[p], p, group)
-
-        original_params = [torch.clone(p.detach()) for p in params_flat]
+        self.weight_decay_cls(self)
+        original_params = list(_param_iterator(self))
 
         self.magnitude.step()
         magnitudes_flat = []
         for o, p in zip(original_params, params_flat):
             magnitudes_flat.append(torch.norm(o.double() - p.double()))
             p.copy_(o.data)
 
@@ -190,29 +279,24 @@
 
 
 class TrueGrad(torch.optim.Optimizer):
     true_statistics: List[str] = []
     base_statistics: List[str] = []
     shared_statistics: List[str] = []
 
-    def __init__(self, params, lr: float = 1e-3,
-                 betas: List[float] = (),
-                 eps: float = 1e-12,
-                 weight_decay: float = 1e-2,
-                 graft: bool = True,
-                 decay_to_init: bool = False,
-                 default_to_baseline: bool = False,
-                 enforce_baseline: bool = False):
+    def __init__(self, params, lr: float = 1e-3, betas: List[float] = (), eps: float = 1e-12,
+                 weight_decay: float = 1e-2, graft: bool = True, default_to_baseline: bool = False,
+                 enforce_baseline: bool = False, weight_decay_cls: Optional[WeightDecayChain] = None):
         defaults = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, graft=graft,
-                        decay_to_init=decay_to_init, default_to_baseline=default_to_baseline,
-                        enforce_baseline=enforce_baseline)
+                        default_to_baseline=default_to_baseline, enforce_baseline=enforce_baseline)
         super(TrueGrad, self).__init__(params, defaults)
+        self.weight_decay_cls = _default_decay(weight_decay_cls)
 
-    def _inner(self, step: int, p: Parameter, group: Dict[str, Any], **kwargs: Tensor
-               ) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
+    def _inner(self, step: int, p: Parameter, group: Dict[str, Any], **kwargs: Tensor) -> Tuple[
+        Optional[Tensor], Optional[Tensor], float]:
         raise NotImplementedError
 
     @torch.no_grad()
     def step(self, closure=None):
         if closure is None:
             loss = None
         else:
@@ -241,20 +325,15 @@
                             state[s] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     if group["decay_to_init"]:
                         state["init"] = torch.clone(p.detach())
 
                 step_t = state['step']
                 step_t += 1
 
-                # Perform stepweight decay
-                decay = group['lr'] * group['weight_decay']
-                if group["decay_to_init"]:
-                    p.add_(state["init"] - p, alpha=decay)
-                else:
-                    p.mul_(1 - decay)
+                self.weight_decay_cls(self)
 
                 step = step_t.item()
 
                 base_update, update, alpha = self._inner(step, p, group,
                                                          **{k: state.get(k) for k in self.shared_statistics},
                                                          **{k: state.get(k) for k in self.base_statistics},
                                                          **{k: state.get(k) for k in self.true_statistics})
@@ -271,36 +350,25 @@
 class TGAdamW(TrueGrad):
     true_statistics: List[str] = ["exp_avg_true_sq"]
     base_statistics: List[str] = ["exp_avg_sq"]
     shared_statistics: List[str] = ["exp_avg"]
 
     def __init__(self, params, lr: float = 1e-3,
                  betas: Union[Tuple[float, float], Tuple[float, float, float]] = (0.9, 0.999, 0.999),
-                 eps: float = 1e-12,
-                 weight_decay: float = 1e-2,
-                 graft: bool = True,
-                 decay_to_init: bool = False,
-                 default_to_adam: bool = None,
-                 default_to_baseline: bool = None,
-                 enforce_baseline: bool = False):
-        if default_to_baseline is None:
-            default_to_baseline = default_to_adam
-        elif default_to_adam is not None:
-            raise ValueError("Can't set both default_to_baseline and default_to_adam, as both map to the same argument")
-        if default_to_adam is not None:
-            warnings.warn("default_to_adam is deprecated and will be replaced by default_to_baseline in April 2023")
+                 eps: float = 1e-12, weight_decay: float = 1e-2, graft: bool = True, default_to_baseline: bool = None,
+                 enforce_baseline: bool = False, weight_decay_cls: Optional[WeightDecayChain] = None):
         if default_to_baseline is None:
             default_to_baseline = False
         super().__init__(params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, graft=graft,
-                         decay_to_init=decay_to_init, default_to_baseline=default_to_baseline,
-                         enforce_baseline=enforce_baseline)
+                         default_to_baseline=default_to_baseline, enforce_baseline=enforce_baseline,
+                         weight_decay_cls=weight_decay_cls)
 
     def _inner(self, step: int, p: Parameter, group: Dict[str, Any], exp_avg: Tensor,
-               exp_avg_sq: Optional[Tensor] = None, exp_avg_true_sq: Optional[Tensor] = None
-               ) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
+               exp_avg_sq: Optional[Tensor] = None, exp_avg_true_sq: Optional[Tensor] = None) -> Tuple[
+        Optional[Tensor], Optional[Tensor], float]:
         if len(group["betas"]) == 2:
             (beta1, beta2), (_, beta3) = group["betas"], group["betas"]
         else:
             beta1, beta2, beta3 = group['betas']
 
         update, base_update, eps = None, None, group["eps"]
         ema_(exp_avg, p.grad, beta1)
@@ -313,29 +381,25 @@
 
 
 class TGLaProp(TrueGrad):
     true_statistics: List[str] = ["exp_avg_true", "exp_avg_true_sq"]
     base_statistics: List[str] = ["exp_avg", "exp_avg_sq"]
 
     def __init__(self, params, lr: float = 1e-3,
-                 betas: Union[Tuple[float, float], Tuple[float, float, float, float]] = (0.9, 0.99),
-                 eps: float = 1e-12,
-                 weight_decay: float = 1e-2,
-                 graft: bool = True,
-                 decay_to_init: bool = False,
-                 default_to_baseline: bool = False,
-                 enforce_baseline: bool = False):
+                 betas: Union[Tuple[float, float], Tuple[float, float, float, float]] = (0.9, 0.99), eps: float = 1e-12,
+                 weight_decay: float = 1e-2, graft: bool = True, decay_to_init: bool = False,
+                 default_to_baseline: bool = False, enforce_baseline: bool = False,
+                 weight_decay_cls: Optional[WeightDecayChain] = None):
         super().__init__(params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, graft=graft,
-                         decay_to_init=decay_to_init, default_to_baseline=default_to_baseline,
-                         enforce_baseline=enforce_baseline)
+                         default_to_baseline=default_to_baseline, enforce_baseline=enforce_baseline,
+                         weight_decay_cls=weight_decay_cls)
 
-    def _inner(self, step: int, p: Parameter, group: Dict[str, Any],
-               exp_avg: Optional[Tensor] = None, exp_avg_sq: Optional[Tensor] = None,
-               exp_avg_true: Optional[Tensor] = None, exp_avg_true_sq: Optional[Tensor] = None
-               ) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
+    def _inner(self, step: int, p: Parameter, group: Dict[str, Any], exp_avg: Optional[Tensor] = None,
+               exp_avg_sq: Optional[Tensor] = None, exp_avg_true: Optional[Tensor] = None,
+               exp_avg_true_sq: Optional[Tensor] = None) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
         if len(group["betas"]) == 2:
             (beta1, beta2), (beta3, beta4) = group["betas"], group["betas"]
         else:
             beta1, beta2, beta3, beta4 = group['betas']
 
         update, base_update, alpha, eps = None, None, 1, group["eps"]
         if exp_avg_true_sq is not None:
@@ -358,29 +422,23 @@
     where correction = 1 / (1 - 0.9 ** step)
 
     It's fundamentally the same as TGLaProp() with beta1 and beta3 = 0
     """
     true_statistics: List[str] = ["exp_avg_true_sq"]
     base_statistics: List[str] = ["exp_avg_sq"]
 
-    def __init__(self, params, lr: float = 1e-3,
-                 betas: Union[float, Tuple[float], Tuple[float, float]] = (0.9,),
-                 eps: float = 1e-12,
-                 weight_decay: float = 1e-2,
-                 graft: bool = True,
-                 decay_to_init: bool = False,
-                 default_to_baseline: bool = False,
-                 enforce_baseline: bool = False):
+    def __init__(self, params, lr: float = 1e-3, betas: Union[float, Tuple[float], Tuple[float, float]] = (0.9,),
+                 eps: float = 1e-12, weight_decay: float = 1e-2, graft: bool = True, default_to_baseline: bool = False,
+                 enforce_baseline: bool = False, weight_decay_cls: Optional[WeightDecayChain] = None):
         super().__init__(params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, graft=graft,
-                         decay_to_init=decay_to_init, default_to_baseline=default_to_baseline,
-                         enforce_baseline=enforce_baseline)
+                         default_to_baseline=default_to_baseline, enforce_baseline=enforce_baseline,
+                         weight_decay_cls=weight_decay_cls)
 
-    def _inner(self, step: int, p: Parameter, group: Dict[str, Any],
-               exp_avg_sq: Optional[Tensor] = None, exp_avg_true_sq: Optional[Tensor] = None
-               ) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
+    def _inner(self, step: int, p: Parameter, group: Dict[str, Any], exp_avg_sq: Optional[Tensor] = None,
+               exp_avg_true_sq: Optional[Tensor] = None) -> Tuple[Optional[Tensor], Optional[Tensor], float]:
         if isinstance(group["betas"], float):
             beta1 = beta2 = group["betas"]
         elif len(group["betas"]) == 1:
             (beta1,), (beta2,) = group["betas"], group["betas"]
         else:
             beta1, beta2 = group['betas']
```

### Comparing `truegrad-3.1.1/truegrad/utils.py` & `truegrad-4.0.0/truegrad/utils.py`

 * *Files identical despite different names*

### Comparing `truegrad-3.1.1/truegrad.egg-info/PKG-INFO` & `truegrad-4.0.0/truegrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 3.1.1
+Version: 4.0.0
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

