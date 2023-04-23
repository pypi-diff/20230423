# Comparing `tmp/legion-cli-0.2.7.tar.gz` & `tmp/legion-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-cli-0.2.7.tar", last modified: Tue Apr 18 03:17:33 2023, max compression
+gzip compressed data, was "legion-cli-0.3.0.tar", last modified: Sun Apr 23 03:35:44 2023, max compression
```

## Comparing `legion-cli-0.2.7.tar` & `legion-cli-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:53.005895 legion-cli-0.2.7/LICENSE
--rw-r--r--   0        0        0     2780 2023-04-16 21:05:35.342704 legion-cli-0.2.7/README.md
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/__init__.py
--rw-r--r--   0        0        0     4459 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/alerts_manager.py
--rw-r--r--   0        0        0     6797 2023-04-18 01:29:44.807755 legion-cli-0.2.7/legion_cli/cli.py
--rw-r--r--   0        0        0      214 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/config.py
--rw-r--r--   0        0        0     1451 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/log.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/tui/__init__.py
--rw-r--r--   0        0        0     8529 2023-04-10 23:51:04.144876 legion-cli-0.2.7/legion_cli/tui/alerts_monitor.py
--rw-r--r--   0        0        0     8791 2023-04-10 23:58:30.245037 legion-cli-0.2.7/legion_cli/tui/detail_list.py
--rw-r--r--   0        0        0      897 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/tui/keyboard.py
--rw-r--r--   0        0        0     1115 2023-04-18 03:10:43.017132 legion-cli-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/integration/__init__.py
--rw-r--r--   0        0        0     1507 2023-04-16 20:19:34.157064 legion-cli-0.2.7/tests/integration/test_watch.py
--rw-r--r--   0        0        0      521 2023-04-16 20:04:09.231827 legion-cli-0.2.7/tests/integration/utils.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/__init__.py
--rw-r--r--   0        0        0     8670 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_alerts_manager.py
--rw-r--r--   0        0        0      863 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_config.py
--rw-r--r--   0        0        0    11550 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_detail_list.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_keyboard.py
--rw-r--r--   0        0        0     3063 1970-01-01 00:00:00.000000 legion-cli-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:53.005895 legion-cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2780 2023-04-16 21:05:35.342704 legion-cli-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.3.0/legion_cli/__init__.py
+-rw-r--r--   0        0        0     4459 2022-11-16 02:41:53.005895 legion-cli-0.3.0/legion_cli/alerts_manager.py
+-rw-r--r--   0        0        0     7046 2023-04-23 03:30:47.582919 legion-cli-0.3.0/legion_cli/cli.py
+-rw-r--r--   0        0        0      214 2022-11-16 02:41:53.005895 legion-cli-0.3.0/legion_cli/config.py
+-rw-r--r--   0        0        0      301 2023-04-23 03:30:47.582919 legion-cli-0.3.0/legion_cli/log.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.3.0/legion_cli/tui/__init__.py
+-rw-r--r--   0        0        0     8529 2023-04-10 23:51:04.144876 legion-cli-0.3.0/legion_cli/tui/alerts_monitor.py
+-rw-r--r--   0        0        0     8791 2023-04-10 23:58:30.245037 legion-cli-0.3.0/legion_cli/tui/detail_list.py
+-rw-r--r--   0        0        0      897 2022-11-16 02:41:53.005895 legion-cli-0.3.0/legion_cli/tui/keyboard.py
+-rw-r--r--   0        0        0     1114 2023-04-23 03:30:47.582919 legion-cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1507 2023-04-16 20:19:34.157064 legion-cli-0.3.0/tests/integration/test_watch.py
+-rw-r--r--   0        0        0      521 2023-04-16 20:04:09.231827 legion-cli-0.3.0/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     8670 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/unit/test_alerts_manager.py
+-rw-r--r--   0        0        0      863 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/unit/test_config.py
+-rw-r--r--   0        0        0    11550 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/unit/test_detail_list.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.3.0/tests/unit/test_keyboard.py
+-rw-r--r--   0        0        0     3063 1970-01-01 00:00:00.000000 legion-cli-0.3.0/PKG-INFO
```

### Comparing `legion-cli-0.2.7/LICENSE` & `legion-cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/README.md` & `legion-cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/legion_cli/alerts_manager.py` & `legion-cli-0.3.0/legion_cli/alerts_manager.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/legion_cli/cli.py` & `legion-cli-0.3.0/legion_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import click
 from legion_utils import Priority
 from robotnikmq import RobotnikConfig, Subscriber, Message
 from termcolor import colored
 from typeguard import typechecked
 
 from legion_cli.tui.alerts_monitor import run_alerts_monitor_with_keyboard_input
-from legion_cli.log import log_to_file
+from legion_cli.log import log
 
 
 DEFAULT_CONFIG = Path.cwd() / "config.yaml"
 DEFAULT_LOGFILE = Path.home() / ".local" / "share" / "legion" / "legion.log"
 
 
 @contextmanager
@@ -195,10 +195,20 @@
     "alert_exchanges",
     type=str,
     multiple=True,
     required=True,
     help="Monitor an exchange for all alerts (warning,error,critical). Equivalent to `-r <EXCHANGE> #.warning -r <EXCHANGE> #.error -r <EXCHANGE> #.critical`",
 )
 def monitor(alert_exchanges: Iterable[str]):
-    """Given a series of exchanges, this command will display a TUI for monitoring alerts on those exchanges"""
-    log_to_file(DEFAULT_LOGFILE)
+    """Given a series of exchanges, this command will display a TUI for monitoring
+       alerts on those exchanges
+    """
+    config = {
+        "handlers": [
+            {"sink": DEFAULT_LOGFILE, "level": "INFO",
+            "format": "{time} | {level} | [{extra[rmq_server]}] {message}"}
+        ],
+        "extra": {"rmq_server": ""}
+    }
+    log.configure(**config)
+    log.enable("robotnikmq")
     run_alerts_monitor_with_keyboard_input(list(alert_exchanges))
```

### Comparing `legion-cli-0.2.7/legion_cli/tui/alerts_monitor.py` & `legion-cli-0.3.0/legion_cli/tui/alerts_monitor.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/legion_cli/tui/detail_list.py` & `legion-cli-0.3.0/legion_cli/tui/detail_list.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/legion_cli/tui/keyboard.py` & `legion-cli-0.3.0/legion_cli/tui/keyboard.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/pyproject.toml` & `legion-cli-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "legion-cli"
-version = "0.2.7"
+version = "0.3.0"
 description = "Commandline Utilities for the Legion Alerting and Monitoring System"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "click>=8.0",
-    "legion-utils>=0.2.14",
+    "legion-utils>=0.3.0",
     "rich>=10.8.0",
     "termcolor>=1.1",
 ]
 requires-python = ">=3.8.3,<4.0"
 readme = "README.md"
 
 [project.license]
```

### Comparing `legion-cli-0.2.7/tests/integration/test_watch.py` & `legion-cli-0.3.0/tests/integration/test_watch.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/tests/integration/utils.py` & `legion-cli-0.3.0/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/tests/unit/test_alerts_manager.py` & `legion-cli-0.3.0/tests/unit/test_alerts_manager.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/tests/unit/test_config.py` & `legion-cli-0.3.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/tests/unit/test_detail_list.py` & `legion-cli-0.3.0/tests/unit/test_detail_list.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.7/PKG-INFO` & `legion-cli-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legion-cli
-Version: 0.2.7
+Version: 0.3.0
 Summary: Commandline Utilities for the Legion Alerting and Monitoring System
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Legion CLI
```

