# Comparing `tmp/nekograd-0.1.0.tar.gz` & `tmp/nekograd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nekograd-0.1.0.tar", last modified: Sat Apr 15 09:08:18 2023, max compression
+gzip compressed data, was "nekograd-0.1.1.tar", last modified: Sun Apr 23 12:27:41 2023, max compression
```

## Comparing `nekograd-0.1.0.tar` & `nekograd-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 09:08:08.000000 nekograd-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 09:08:08.000000 nekograd-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-15 09:08:18.100280 nekograd-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-15 09:08:08.000000 nekograd-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/data/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/nekograd/model/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/nekograd/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 09:08:08.000000 nekograd-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 09:08:18.100280 nekograd-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-15 09:08:08.000000 nekograd-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 12:27:31.000000 nekograd-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 12:27:31.000000 nekograd-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-23 12:27:41.879311 nekograd-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-23 12:27:31.000000 nekograd-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/data/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 12:27:31.000000 nekograd-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:27:41.879311 nekograd-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-23 12:27:31.000000 nekograd-0.1.1/setup.py
```

### Comparing `nekograd-0.1.0/LICENSE` & `nekograd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.0/nekograd/metrics/binary.py` & `nekograd-0.1.1/nekograd/metrics/binary.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.0/nekograd/metrics/utils.py` & `nekograd-0.1.1/nekograd/metrics/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import wraps
 from typing import Callable, Sequence, Union
 
 import numpy as np
 from torch import Tensor
 
-from ..torch.utils import to_np, np2tensor
+from ..torch.utils import np2tensor, to_np
 
 ArrayLike = Union[np.ndarray, Tensor]
 
 
 def ravel(metric):
     @wraps(metric)
     def wrapper(t: np.ndarray, p: np.ndarray, *args, **kwargs):
@@ -74,15 +74,15 @@
     return wrapper
 
 
 def batched(aggregate: Callable = np.mean):
     def decorator(metric):
         @wraps(metric)
         def wrapper(
-                ts: Sequence[np.ndarray], ps: Sequence[np.ndarray], *args, **kwargs
+            ts: Sequence[np.ndarray], ps: Sequence[np.ndarray], *args, **kwargs
         ):
             return aggregate([metric(t, p, *args, **kwargs) for t, p in zip(ts, ps)])
 
         return wrapper
 
     return decorator
```

### Comparing `nekograd-0.1.0/nekograd/model/base.py` & `nekograd-0.1.1/nekograd/model/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta
-from typing import List, Dict, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 
 from ..torch.utils import np2tensor, to_np
 
@@ -17,45 +17,45 @@
     def __init__(self):
         super().__init__()
         self.training_step_outputs = []
         self.validation_step_outputs = []
         self.test_step_outputs = []
 
     def on_before_batch_transfer(
-            self, batch: Tuple[np.ndarray, ...], dataloader_idx: int
+        self, batch: Tuple[np.ndarray, ...], dataloader_idx: int
     ) -> Tuple[torch.Tensor, ...]:
         return tuple(map(np2tensor, batch))
 
     def on_train_epoch_start(self) -> None:
         self.training_step_outputs.clear()
 
     def on_validation_epoch_start(self) -> None:
         self.validation_step_outputs.clear()
 
     def on_test_epoch_start(self) -> None:
         self.test_step_outputs.clear()
 
     def on_train_batch_end(
-            self,
-            outputs: TRAIN_STEP_OUTPUT,
-            batch: Tuple[torch.Tensor, ...],
-            batch_idx: int,
+        self,
+        outputs: TRAIN_STEP_OUTPUT,
+        batch: Tuple[torch.Tensor, ...],
+        batch_idx: int,
     ) -> None:
         self.training_step_outputs.append(to_np(outputs))
 
     def on_validation_batch_end(
-            self,
-            outputs: VAL_STEP_OUTPUT,
-            batch: Tuple[torch.Tensor, ...],
-            batch_idx: int,
-            dataloader_idx: int = 0,
+        self,
+        outputs: VAL_STEP_OUTPUT,
+        batch: Tuple[torch.Tensor, ...],
+        batch_idx: int,
+        dataloader_idx: int = 0,
     ) -> None:
         self.validation_step_outputs.append(outputs)
 
     def on_test_batch_end(
-            self,
-            outputs: TEST_STEP_OUTPUT,
-            batch: Tuple[torch.Tensor, ...],
-            batch_idx: int,
-            dataloader_idx: int = 0,
+        self,
+        outputs: TEST_STEP_OUTPUT,
+        batch: Tuple[torch.Tensor, ...],
+        batch_idx: int,
+        dataloader_idx: int = 0,
     ) -> None:
         self.test_step_outputs.append(outputs)
```

### Comparing `nekograd-0.1.0/nekograd/model/commands.py` & `nekograd-0.1.1/nekograd/model/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from functools import wraps
 from pathlib import Path
-from typing import Callable, Dict, Union, Sequence
+from typing import Callable, Dict, Sequence, Union
 
 import numpy as np
-from functools import wraps
 import pytorch_lightning as pl
 from more_itertools import zip_equal
 
 PathLike = Union[Path, str]
 
 
 def convert_to_aggregated(metric: Callable, aggregate_fn: Callable = np.mean):
```

### Comparing `nekograd-0.1.0/nekograd/model/model.py` & `nekograd-0.1.1/nekograd/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from functools import partial
-from itertools import chain
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 from cytoolz import compose, keymap
-from more_itertools import unzip, collapse
+from more_itertools import collapse, unzip
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
-from .base import BaseModel, STEP_OUTPUT, EPOCH_OUTPUT
+from ..torch.utils import to_np
+from .base import EPOCH_OUTPUT, STEP_OUTPUT, BaseModel
 from .commands import compute_metrics
 from .utils import criterion_wrapper
-from ..torch.utils import to_np
 
 
 class CoreModel(BaseModel):
     def __init__(
-            self,
-            architecture: nn.Module,
-            criterion: Callable,
-            metrics: Dict[str, Callable],
-            activation: Callable = nn.Identity(),
-            optimizer: Union[Optimizer, None] = None,
-            lr_scheduler: Union[_LRScheduler, None] = None,
-            n_targets: int = 1,
+        self,
+        architecture: nn.Module,
+        criterion: Callable,
+        metrics: Dict[str, Callable],
+        activation: Callable = nn.Identity(),
+        optimizer: Union[Optimizer, None] = None,
+        lr_scheduler: Union[_LRScheduler, None] = None,
+        n_targets: int = 1,
     ):
         super().__init__()
         self.architecture = architecture
         self.metrics = metrics
         self.criterion = criterion
         self.activation = activation
         self.optimizer = optimizer
@@ -53,30 +52,30 @@
         }
         return [self.optimizer], [self.lr_scheduler]
 
     def forward(self, *xs: torch.Tensor) -> torch.Tensor:
         return self.architecture(*xs)
 
     def training_step(
-            self, batch: Tuple[torch.Tensor, ...], batch_idx: int
+        self, batch: Tuple[torch.Tensor, ...], batch_idx: int
     ) -> Dict[str, torch.Tensor]:
-        x, y = batch[: -self._nt], batch[-self._nt:]
+        x, y = batch[: -self._nt], batch[-self._nt :]
         return self.wrapped_criterion(self(*x), *y)
 
     def validation_step(
-            self, batch: Tuple[torch.Tensor, ...], batch_idx: int
+        self, batch: Tuple[torch.Tensor, ...], batch_idx: int
     ) -> STEP_OUTPUT:
         return self.inference_step(batch[0]), to_np(batch[1])
 
     def test_step(self, batch: Tuple[torch.Tensor, ...], batch_idx: int) -> STEP_OUTPUT:
         return self.inference_step(batch[0]), to_np(batch[1])
 
     # TODO
     def predict_step(
-            self, batch: Tuple[torch.Tensor, ...], batch_idx: int, **kwargs
+        self, batch: Tuple[torch.Tensor, ...], batch_idx: int, **kwargs
     ) -> STEP_OUTPUT:
         raise NotImplementedError("Currently in development")
 
     def inference_step(self, x: torch.Tensor) -> np.ndarray:
         return to_np(self.activation(self(x)))
 
     def on_train_epoch_end(self) -> None:
@@ -85,29 +84,31 @@
     def on_validation_epoch_end(self) -> None:
         self.log_metrics_on_epoch_end(self.validation_step_outputs, "val")
 
     def on_test_epoch_end(self) -> None:
         self.log_metrics_on_epoch_end(self.test_step_outputs, "test")
 
     def log_metrics_on_epoch_end(
-            self, outputs: EPOCH_OUTPUT, prefix: str = ""
+        self, outputs: EPOCH_OUTPUT, prefix: str = ""
     ) -> Dict[str, Union[np.ndarray, float]]:
         if prefix:
             prefix += "/"
 
         if isinstance(outputs[0], dict):
             logs = {}
             for k in filter(lambda s: not s.startswith("_"), outputs[0].keys()):
                 logs[k] = np.mean(list(collapse(o[k] for o in outputs)))
         elif isinstance(outputs[0], (list, tuple)):
             x, y = map(compose(list, partial(collapse, levels=1)), unzip(outputs))
             logs = compute_metrics(y, x, self.metrics)
         else:
-            raise TypeError(f"Unknown type of outputs: {type(outputs[0])}, "
-                            "expected Union[dict, list, tuple]")
+            raise TypeError(
+                f"Unknown type of outputs: {type(outputs[0])}, "
+                "expected Union[dict, list, tuple]"
+            )
 
         logs = keymap(lambda k: prefix + k, logs)
         self.log_dict(logs, prog_bar=True, on_epoch=True)
         return logs
 
     def _wrap_criterion(self) -> None:
         self.wrapped_criterion = criterion_wrapper("loss")(self.criterion)
```

### Comparing `nekograd-0.1.0/nekograd/model/policy.py` & `nekograd-0.1.1/nekograd/model/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Dict, Callable
+from typing import Callable, Dict
 
 
 class Policy(ABC):
     def __call__(self, epoch: int):
         return self.epoch2value(epoch)
 
     @abstractmethod
@@ -37,14 +37,15 @@
     """
     Useful with torch.optim.lr_scheduler.LambdaLR
     lr_policy = Switch(lr_init, lambda i: np.cos(i / np.pi))
     optimizer = Adam(model.parameters(), lr=lr_init)
     scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer, lr_lambda=lr_policy)
     On i-th epoch lr_i = cos(i / np.pi)
     """
+
     def __init__(self, epoch2lr: Callable[[int], float], lr_init: float):
         super().__init__()
         if lr_init == 0:
             raise ValueError(f"lr_init must not be equal to 0")
         self.lr_init = lr_init
         self.epoch2lr = epoch2lr
```

### Comparing `nekograd-0.1.0/nekograd/model/utils.py` & `nekograd-0.1.1/nekograd/model/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     def decorator(criterion: Callable):
         @wraps(criterion)
         def wrapper(*args, **kwargs) -> Dict[str, torch.Tensor]:
             loss = criterion(*args, **kwargs)
             if isinstance(loss, torch.Tensor):
                 return {loss_key: loss}
             elif isinstance(loss, dict):
-                return loss if loss_key in loss else {loss_key: sum(loss.values()), **loss}
+                return (
+                    loss if loss_key in loss else {loss_key: sum(loss.values()), **loss}
+                )
             else:
-                raise ValueError(f"Expected `loss` to be dict or tensor, got {type(loss)}")
+                raise ValueError(
+                    f"Expected `loss` to be dict or tensor, got {type(loss)}"
+                )
 
         return wrapper
 
     return decorator
```

### Comparing `nekograd-0.1.0/nekograd/torch/criterion.py` & `nekograd-0.1.1/nekograd/torch/criterion.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.0/nekograd/torch/utils.py` & `nekograd-0.1.1/nekograd/torch/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Dict, Sequence, Any, List, Union
+from typing import Any, Dict, List, Sequence, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 
 def switch_grad(*models: nn.Module, mode: bool = False) -> None:
```

### Comparing `nekograd-0.1.0/nekograd.egg-info/SOURCES.txt` & `nekograd-0.1.1/nekograd.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 nekograd/__init__.py
 nekograd/__version__.py
+nekograd/utils.py
 nekograd.egg-info/PKG-INFO
 nekograd.egg-info/SOURCES.txt
 nekograd.egg-info/dependency_links.txt
 nekograd.egg-info/requires.txt
 nekograd.egg-info/top_level.txt
 nekograd/data/__init__.py
-nekograd/data/module.py
 nekograd/data/split.py
-nekograd/data/transforms.py
-nekograd/data/utils.py
 nekograd/metrics/__init__.py
 nekograd/metrics/binary.py
 nekograd/metrics/checks.py
 nekograd/metrics/utils.py
 nekograd/model/__init__.py
 nekograd/model/base.py
 nekograd/model/commands.py
```

### Comparing `nekograd-0.1.0/setup.py` & `nekograd-0.1.1/setup.py`

 * *Files identical despite different names*

