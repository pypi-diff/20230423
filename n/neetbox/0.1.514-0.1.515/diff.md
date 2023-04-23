# Comparing `tmp/neetbox-0.1.514.tar.gz` & `tmp/neetbox-0.1.515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.514.tar", max compression
+gzip compressed data, was "neetbox-0.1.515.tar", max compression
```

## Comparing `neetbox-0.1.514.tar` & `neetbox-0.1.515.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0     1067 2023-04-19 04:05:41.060662 neetbox-0.1.514/LICENSE
--rw-r--r--   0        0        0      397 2023-04-19 04:05:41.060662 neetbox-0.1.514/README.md
--rw-r--r--   0        0        0     2827 2023-04-19 04:05:41.064662 neetbox-0.1.514/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 04:05:41.064662 neetbox-0.1.514/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1390 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/config/_config.py
--rw-r--r--   0        0        0       66 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/core/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/core/registry.py
--rw-r--r--   0        0        0     2984 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      872 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     2161 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     3086 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0     3226 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_win_service.py
--rw-r--r--   0        0        0      337 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     3924 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/environment/hardware.py
--rw-r--r--   0        0        0     1748 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/environment/platform.py
--rw-r--r--   0        0        0     8870 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/__init__.py
--rw-r--r--   0        0        0    12181 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     2526 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18871 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/logger.py
--rw-r--r--   0        0        0      241 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      299 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/_pipe.py
--rw-r--r--   0        0        0     5167 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/_signal_and_slot.py
--rw-r--r--   0        0        0        0 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      108 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5636 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6703 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2400 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2699 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4702 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/profile.py
--rw-r--r--   0        0        0       78 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/_package.py
--rw-r--r--   0        0        0     1019 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/format.py
--rw-r--r--   0        0        0     2303 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/framing.py
--rw-r--r--   0        0        0     1238 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/mvc.py
--rw-r--r--   0        0        0     1239 2023-04-19 04:05:41.068662 neetbox-0.1.514/pyproject.toml
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 neetbox-0.1.514/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-23 10:28:51.984400 neetbox-0.1.515/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-23 10:28:51.984400 neetbox-0.1.515/README.md
+-rw-r--r--   0        0        0     3022 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1390 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/config/_config.py
+-rw-r--r--   0        0        0       66 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/core/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/core/registry.py
+-rw-r--r--   0        0        0     2498 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     2161 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     3736 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0      828 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_daemon_launcher.py
+-rw-r--r--   0        0        0      250 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_local_http_client.py
+-rw-r--r--   0        0        0     3226 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/_win_service.py
+-rw-r--r--   0        0        0     3039 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/daemon/daemonable_process.py
+-rw-r--r--   0        0        0      337 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     3924 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/integrations/environment/hardware.py
+-rw-r--r--   0        0        0     1748 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/integrations/environment/platform.py
+-rw-r--r--   0        0        0     8870 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0    12181 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-23 10:28:51.988400 neetbox-0.1.515/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     2526 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18871 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/logging/logger.py
+-rw-r--r--   0        0        0      241 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/pipeline/_pipe.py
+-rw-r--r--   0        0        0     5167 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/pipeline/_signal_and_slot.py
+-rw-r--r--   0        0        0        0 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      108 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5636 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6703 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2400 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2699 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4702 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/torch/profile.py
+-rw-r--r--   0        0        0       78 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/utils/_package.py
+-rw-r--r--   0        0        0     1019 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/utils/format.py
+-rw-r--r--   0        0        0     2303 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     1238 2023-04-23 10:28:51.992400 neetbox-0.1.515/neetbox/utils/mvc.py
+-rw-r--r--   0        0        0     1236 2023-04-23 10:28:51.992400 neetbox-0.1.515/pyproject.toml
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 neetbox-0.1.515/PKG-INFO
```

### Comparing `neetbox-0.1.514/LICENSE` & `neetbox-0.1.515/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/__init__.py` & `neetbox-0.1.515/neetbox/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -66,10 +66,12 @@
     except Exception as e:
         from neetbox.logging.logger import Logger
 
         logger = Logger("NEETBOX")  # builtin standalone logger
         logger.err(f"Failed to load config from {config_file_path}: {e}")
         return False
 
-
-if os.path.isfile(config_file_name):  # if in a workspace
+is_in_daemon_process = 'NEETBOX_DAEMON_PROCESS' in os.environ and os.environ['NEETBOX_DAEMON_PROCESS'] == '1'
+print('prevent_daemon_loading =', is_in_daemon_process)
+if os.path.isfile(config_file_name) and not is_in_daemon_process:  # if in a workspace
     init(load=True)
+
```

### Comparing `neetbox-0.1.514/neetbox/cli/parse.py` & `neetbox-0.1.515/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/config/__init__.py` & `neetbox-0.1.515/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/config/_config.py` & `neetbox-0.1.515/neetbox/config/_config.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/core/registry.py` & `neetbox-0.1.515/neetbox/core/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/daemon/__init__.py` & `neetbox-0.1.515/neetbox/daemon/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
 from neetbox.daemon._daemon_client import connect_daemon
+from neetbox.daemon.daemonable_process import DaemonableProcess
 from neetbox.logging import logger
 from neetbox.utils import pkg
+from neetbox.pipeline import watch, listen
 import platform
 import time
 import os
+import json
 
 
 def __attach_daemon(daemon_config):
     if not daemon_config["allowIpython"]:
         try:
             eval("__IPYTHON__")
         except NameError:
@@ -21,58 +24,51 @@
         else:
             logger.log(
                 "NEETBOX DAEMON won't start when debugging in ipython console. If you want to allow daemon run in "
                 "ipython, try to set 'allowIpython' to True."
             )
             return False  # ignore if debugging in ipython
     _online_status = connect_daemon(daemon_config)  # try to connect daemon
+    logger.log('daemon connection status: ' + str(_online_status))
     if not _online_status:  # if no daemon online
         logger.log(
             f"No daemon running at {daemon_config['server']}:{daemon_config['port']}, trying to create daemon..."
         )
-        if platform.system() == "Windows":  # running on windows
-            try:
-                assert pkg.is_installed(
-                    "win32api", try_install_if_not="pywin32"
-                ), "Please install 'pywin32' before using NEETBOX daemon"
-                assert pkg.is_installed(
-                    "win32serviceutil", try_install_if_not="pypiwin32"
-                ), "Please install 'pywin32' before using NEETBOX daemon"
-                from neetbox.daemon._win_service import installService
-
-                installService(cfg=daemon_config)
-            except Exception as e:
-                logger.err(f"Could not install Windows service because {e}.")
-                return False
-        else:  # not on windows
-            pid = os.fork()
-            if pid == 0:  # child process
-                pkg.is_installed("daemon", try_install_if_not="python-daemon")
-                import daemon
-                from neetbox.daemon._daemon import daemon_process
-
-                with daemon.DaemonContext():
-                    daemon_process(daemon_config)  # create daemon
-            elif pid < 0:
-                logger.err(
-                    "Faild to spawn daemon process using os.fork. NEETBOX daemon will not start."
-                )
-                return False
+
+        popen = DaemonableProcess(
+            target='neetbox.daemon._daemon_launcher',
+            args=['--config', json.dumps(daemon_config)],
+            mode='detached',
+            redirect_stdout=None,
+            env_append={'NEETBOX_DAEMON_PROCESS': '1'},
+        ).start()
+
         time.sleep(1)
-        _retry = 3
-        while not connect_daemon(daemon_config):  # try connect daemon
-            logger.warn(f"Could not connect to the daemon. {_retry} retries remaining.")
-            time.sleep(1)
-            _retry -= 1
-            if not _retry:
-                logger.err(
-                    "Connect daemon faild after 3 retries, daemon connector won't start."
-                )
-                return False
-        return True
+        
+        _retry_timeout = 10
+        _time_begin = time.perf_counter()
+
+        logger.log('Created daemon process, trying to connect to daemon...')
+        while time.perf_counter() - _time_begin < 10:  # try connect daemon
+            if connect_daemon(daemon_config):
+                return True
+            else:
+                exit_code = popen.poll()
+                if exit_code is not None:
+                    logger.err(
+                        f"Daemon process exited unexpectedly with exit code {exit_code}."
+                    )
+                    return False
+            
+                time.sleep(0.5)
+
+        logger.err(
+            f"Failed to connect to daemon after {_retry_timeout}s, daemon connector won't start."
+        )
+        return False
 
 
 def _try_attach_daemon():
     from neetbox.config import get_module_level_config
 
     _cfg = get_module_level_config()
     if _cfg["enable"]:
```

### Comparing `neetbox-0.1.514/neetbox/daemon/_daemon.py` & `neetbox-0.1.515/neetbox/daemon/_daemon.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/daemon/_win_service.py` & `neetbox-0.1.515/neetbox/daemon/_win_service.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/integrations/engine.py` & `neetbox-0.1.515/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/integrations/environment/hardware.py` & `neetbox-0.1.515/neetbox/integrations/environment/hardware.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/integrations/environment/platform.py` & `neetbox-0.1.515/neetbox/integrations/environment/platform.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/integrations/resource.py` & `neetbox-0.1.515/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.515/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.515/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.515/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.515/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.515/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/formatting.py` & `neetbox-0.1.515/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/logging/logger.py` & `neetbox-0.1.515/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/pipeline/_signal_and_slot.py` & `neetbox-0.1.515/neetbox/pipeline/_signal_and_slot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/plotting/plot.py` & `neetbox-0.1.515/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/arch/canny.py` & `neetbox-0.1.515/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/arch/cnn.py` & `neetbox-0.1.515/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/arch/kernels.py` & `neetbox-0.1.515/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.515/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/nlp.py` & `neetbox-0.1.515/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/torch/profile.py` & `neetbox-0.1.515/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/utils/_package.py` & `neetbox-0.1.515/neetbox/utils/_package.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/utils/format.py` & `neetbox-0.1.515/neetbox/utils/format.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/utils/framing.py` & `neetbox-0.1.515/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/neetbox/utils/mvc.py` & `neetbox-0.1.515/neetbox/utils/mvc.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.514/pyproject.toml` & `neetbox-0.1.515/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.514"
+version = "0.1.515"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
@@ -36,15 +36,15 @@
 toml = ">0.10"
 injector = ">=0.20"
 setproctitle = "^1.3.2"
 rich = "^13.3.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0.0"
-requests = "^2.28.2"
+httpx = "^0.24.0"
 flask = "^2.2.3"
 
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `neetbox-0.1.514/PKG-INFO` & `neetbox-0.1.515/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.514
+Version: 0.1.515
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

