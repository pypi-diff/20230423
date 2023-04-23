# Comparing `tmp/lightning-habana-0.1.0rc0.tar.gz` & `tmp/lightning-habana-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-habana-0.1.0rc0.tar", last modified: Tue Mar 14 18:25:37 2023, max compression
+gzip compressed data, was "lightning-habana-0.2.0.dev0.tar", last modified: Sun Apr 23 12:30:09 2023, max compression
```

## Comparing `lightning-habana-0.1.0rc0.tar` & `lightning-habana-0.2.0.dev0.tar`

### file list

```diff
@@ -1,29 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.543195 lightning-habana-0.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:30:09.543195 lightning-habana-0.2.0.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.535195 lightning-habana-0.2.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/profiler/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-23 12:29:53.000000 lightning-habana-0.2.0.dev0/src/lightning_habana/utils/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:09.539195 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 12:30:09.000000 lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/top_level.txt
```

### Comparing `lightning-habana-0.1.0rc0/LICENSE` & `lightning-habana-0.2.0.dev0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -195,7 +195,21 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+
+   Copyright (c) 2023 Habana Labs, Ltd. an Intel Company
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lightning-habana-0.1.0rc0/MANIFEST.in` & `lightning-habana-0.2.0.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0rc0/setup.py` & `lightning-habana-0.2.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/accelerator.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/accelerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from lightning_fabric.utilities.types import _DEVICE
     from pytorch_lightning.accelerators.accelerator import Accelerator
     from pytorch_lightning.utilities.exceptions import MisconfigurationException
     from pytorch_lightning.utilities.rank_zero import rank_zero_debug
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HPU_AVAILABLE
 
 if _HPU_AVAILABLE:
     import habana_frameworks.torch.hpu as torch_hpu
 
 
 class HPUAccelerator(Accelerator):
     """Accelerator for HPU devices."""
```

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/__init__.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from lightning_habana.plugins.io_plugin import HPUCheckpointIO
-from lightning_habana.plugins.precision import HPUPrecisionPlugin
+from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
+from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 
 __all__ = ["HPUPrecisionPlugin", "HPUCheckpointIO"]
```

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/io_plugin.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/precision.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/plugins/precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 if module_available("lightning"):
     from lightning.pytorch.plugins.precision.precision_plugin import PrecisionPlugin
 elif module_available("pytorch_lightning"):
     from pytorch_lightning.plugins.precision.precision_plugin import PrecisionPlugin
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HPU_AVAILABLE
 
 if _HPU_AVAILABLE:
     from habana_frameworks.torch.hpex import hmp
 
-_PRECISION_INPUT = Literal["32-true", "16-mixed", "bf16-mixed"]
+_PRECISION_INPUT = Literal["32", "32-true", "bf16", "bf16-mixed"]
 
 
 class HPUPrecisionPlugin(PrecisionPlugin):
     """Plugin that enables bfloat/half support on HPUs.
 
     Args:
         precision: The precision to use.
```

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/strategies/__init__.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/fabric/strategies/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright The Lightning AI team.
+# Copyright (c) 2023 Habana Labs, Ltd. an Intel Company
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from lightning_habana.strategies.parallel import HPUParallelStrategy
-from lightning_habana.strategies.single import SingleHPUStrategy
+
+from lightning_habana.fabric.strategies.parallel import HPUParallelStrategy
+from lightning_habana.fabric.strategies.single import SingleHPUStrategy
 
 __all__ = ["HPUParallelStrategy", "SingleHPUStrategy"]
```

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana/strategies/parallel.py` & `lightning-habana-0.2.0.dev0/src/lightning_habana/pytorch/strategies/single.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,84 +7,66 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import logging
-import os
-from typing import Any, Callable, Dict, List, Optional, Union
 
-import torch.distributed
+from typing import Any, Callable, Dict, Optional, Union
+
 from lightning_utilities import module_available
 
 if module_available("lightning"):
-    from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
-    from lightning.fabric.utilities.distributed import group as _group
-    from lightning.pytorch import LightningModule
+    from lightning.fabric.plugins import CheckpointIO
+    from lightning.fabric.utilities.types import _DEVICE
+    from lightning.pytorch import LightningModule, Trainer
     from lightning.pytorch.accelerators import Accelerator
+    from lightning.pytorch.plugins.io.hpu_plugin import HPUCheckpointIO
     from lightning.pytorch.plugins.io.wrapper import _WrappingCheckpointIO
     from lightning.pytorch.plugins.precision import PrecisionPlugin
-    from lightning.pytorch.strategies.ddp import DDPStrategy
+    from lightning.pytorch.strategies.single_device import SingleDeviceStrategy
 elif module_available("pytorch_lightning"):
-    from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
-    from lightning_fabric.utilities.distributed import group as _group
-    from pytorch_lightning import LightningModule
+    from lightning_fabric.plugins import CheckpointIO
+    from lightning_fabric.utilities.types import _DEVICE
+    from pytorch_lightning import LightningModule, Trainer
     from pytorch_lightning.accelerators import Accelerator
-    from pytorch_lightning.overrides.torch_distributed import broadcast_object_list
     from pytorch_lightning.plugins.io.hpu_plugin import HPUCheckpointIO
     from pytorch_lightning.plugins.io.wrapper import _WrappingCheckpointIO
     from pytorch_lightning.plugins.precision import PrecisionPlugin
-    from pytorch_lightning.strategies.ddp import DDPStrategy
+    from pytorch_lightning.strategies.single_device import SingleDeviceStrategy
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
+
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 
-from lightning_habana import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HPU_AVAILABLE
 
 if _HPU_AVAILABLE:
     import habana_frameworks.torch.core as htcore
-    import habana_frameworks.torch.distributed.hccl  # noqa: F401
 
-log = logging.getLogger(__name__)
 
+class SingleHPUStrategy(SingleDeviceStrategy):
+    """Strategy for training on single HPU device."""
 
-class HPUParallelStrategy(DDPStrategy):
-    """Strategy for distributed training on multiple HPU devices."""
-
-    strategy_name = "hpu_parallel"
+    strategy_name = "hpu_single"
 
     def __init__(
         self,
+        device: _DEVICE = "hpu",
         accelerator: Optional[Accelerator] = None,
-        parallel_devices: Optional[List[torch.device]] = None,
-        cluster_environment: Optional[ClusterEnvironment] = None,
         checkpoint_io: Optional[CheckpointIO] = None,
         precision_plugin: Optional[PrecisionPlugin] = None,
-        ddp_comm_state: Optional[object] = None,
-        ddp_comm_hook: Optional[Callable] = None,
-        ddp_comm_wrapper: Optional[Callable] = None,
-        model_averaging_period: Optional[int] = None,
-        process_group_backend: Optional[str] = "hccl",
-        **kwargs: Any,
-    ) -> None:
+    ):
         super().__init__(
             accelerator=accelerator,
-            parallel_devices=parallel_devices,
-            cluster_environment=cluster_environment,
+            device=device,
             checkpoint_io=checkpoint_io,
             precision_plugin=precision_plugin,
-            ddp_comm_state=ddp_comm_state,
-            ddp_comm_hook=ddp_comm_hook,
-            ddp_comm_wrapper=ddp_comm_wrapper,
-            model_averaging_period=model_averaging_period,
-            process_group_backend=process_group_backend,
-            **kwargs,
         )
 
     @property
     def checkpoint_io(self) -> CheckpointIO:
         if self._checkpoint_io is None:  # type: ignore[has-type]
             self._checkpoint_io = HPUCheckpointIO()
         elif isinstance(self._checkpoint_io, _WrappingCheckpointIO):
@@ -92,31 +74,27 @@
 
         return self._checkpoint_io
 
     @checkpoint_io.setter
     def checkpoint_io(self, io: Optional[CheckpointIO]) -> None:
         self._checkpoint_io = io
 
-    def setup_environment(self) -> None:
-        os.environ["ID"] = str(self.local_rank)
-        if self._process_group_backend == "hccl":
-            # this env is used in overrides to check the backend initiated
-            os.environ["HCCL_DISTRIBUTED_BACKEND"] = str(1)
-        super().setup_environment()
-
-    def determine_ddp_device_ids(self) -> None:
-        return None
-
-    def broadcast(self, obj: object, src: int = 0) -> object:
-        obj = [obj]
-        if self.global_rank != src:
-            obj = [None]
+    @property
+    def is_distributed(self) -> bool:
+        return False
+
+    def setup(self, trainer: Trainer) -> None:
+        self.model_to_device()
+        super().setup(trainer)
 
-        broadcast_object_list(obj, src, group=_group.WORLD)
-        return obj[0]
+    def setup_optimizers(self, trainer: Trainer) -> None:
+        super().setup_optimizers(trainer)
+
+    def model_to_device(self) -> None:
+        self.model.to(self.root_device)
 
     def on_after_backward(self) -> None:
         # Break lazy accumulation of graph after fwd+bwd
         htcore.mark_step()
 
     def optimizer_step(
         self,
@@ -133,13 +111,7 @@
     @classmethod
     def register_strategies(cls, strategy_registry: Dict) -> None:
         strategy_registry.register(
             cls.strategy_name,
             cls,
             description=f"{cls.__class__.__name__}",
         )
-
-    def teardown(self) -> None:
-        super().teardown()
-        # Was set to local rank
-        os.environ.pop("ID", None)
-        os.environ.pop("HCCL_DISTRIBUTED_BACKEND", None)
```

### Comparing `lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/SOURCES.txt` & `lightning-habana-0.2.0.dev0/src/lightning_habana.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,33 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/lightning_habana/__about__.py
 src/lightning_habana/__init__.py
-src/lightning_habana/accelerator.py
 src/lightning_habana.egg-info/PKG-INFO
 src/lightning_habana.egg-info/SOURCES.txt
 src/lightning_habana.egg-info/dependency_links.txt
 src/lightning_habana.egg-info/not-zip-safe
 src/lightning_habana.egg-info/requires.txt
 src/lightning_habana.egg-info/top_level.txt
-src/lightning_habana/plugins/__init__.py
-src/lightning_habana/plugins/io_plugin.py
-src/lightning_habana/plugins/precision.py
-src/lightning_habana/strategies/__init__.py
-src/lightning_habana/strategies/parallel.py
-src/lightning_habana/strategies/single.py
+src/lightning_habana/fabric/__init__.py
+src/lightning_habana/fabric/accelerator.py
+src/lightning_habana/fabric/plugins/__init__.py
+src/lightning_habana/fabric/plugins/io_plugin.py
+src/lightning_habana/fabric/plugins/precision.py
+src/lightning_habana/fabric/strategies/__init__.py
+src/lightning_habana/fabric/strategies/parallel.py
+src/lightning_habana/fabric/strategies/single.py
+src/lightning_habana/pytorch/__init__.py
+src/lightning_habana/pytorch/accelerator.py
+src/lightning_habana/pytorch/plugins/__init__.py
+src/lightning_habana/pytorch/plugins/io_plugin.py
+src/lightning_habana/pytorch/plugins/precision.py
+src/lightning_habana/pytorch/profiler/__init__.py
+src/lightning_habana/pytorch/profiler/profiler.py
+src/lightning_habana/pytorch/strategies/__init__.py
+src/lightning_habana/pytorch/strategies/parallel.py
+src/lightning_habana/pytorch/strategies/single.py
+src/lightning_habana/utils/__init__.py
+src/lightning_habana/utils/imports.py
```

