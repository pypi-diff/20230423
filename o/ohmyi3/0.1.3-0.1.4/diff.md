# Comparing `tmp/ohmyi3-0.1.3.tar.gz` & `tmp/ohmyi3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmyi3-0.1.3.tar", max compression
+gzip compressed data, was "ohmyi3-0.1.4.tar", max compression
```

## Comparing `ohmyi3-0.1.3.tar` & `ohmyi3-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.3/LICENSE
--rw-r--r--   0        0        0    22565 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/README.md
--rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.3/ohmyi3/commands/entrypoint.py
--rw-r--r--   0        0        0     3208 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/commands/generate.py
--rw-r--r--   0        0        0      432 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/commands/info.py
--rw-r--r--   0        0        0     1529 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/commands/init.py
--rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.3/ohmyi3/config/app.py
--rw-r--r--   0        0        0     2238 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/config/package.py
--rw-r--r--   0        0        0      446 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/i3ctl.py
--rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.3/ohmyi3/services/bootstrap.py
--rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.3/ohmyi3/services/ohmyi3.py
--rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.3/ohmyi3/stubs/README.md
--rw-r--r--   0        0        0      810 2023-04-22 16:38:39.408913 ohmyi3-0.1.3/ohmyi3/stubs/config.d/00-header.conf
--rw-r--r--   0        0        0     1985 2023-04-22 16:38:39.408913 ohmyi3-0.1.3/ohmyi3/stubs/config.d/05-system.conf
--rw-r--r--   0        0        0     3035 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/10-autostart.conf
--rw-r--r--   0        0        0      775 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/15-borders.conf
--rw-r--r--   0        0        0     6434 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/20-navigation.conf
--rw-r--r--   0        0        0     3212 2023-04-22 16:38:39.412246 ohmyi3-0.1.3/ohmyi3/stubs/config.d/80-applications.conf
--rw-r--r--   0        0        0     6720 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/85-windows.conf
--rw-r--r--   0        0        0     3195 2023-04-22 16:38:39.412246 ohmyi3-0.1.3/ohmyi3/stubs/config.d/90-gaps.conf
--rw-r--r--   0        0        0    12738 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.py
--rw-r--r--   0        0        0       33 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/__init__.py
--rw-r--r--   0        0        0      893 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/alacritty.py
--rw-r--r--   0        0        0       29 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/__init__.py
--rw-r--r--   0        0        0      958 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/archey3.py
--rw-r--r--   0        0        0       31 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
--rw-r--r--   0        0        0       29 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/__init__.py
--rw-r--r--   0        0        0     2188 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/polybar.py
--rw-r--r--   0        0        0   385109 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/background.jpg
--rw-r--r--   0        0        0     1874 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/theme.conf
--rw-r--r--   0        0        0   198158 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/background.jpg
--rw-r--r--   0        0        0     1915 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/theme.conf
--rw-r--r--   0        0        0     1869 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/i3status.conf
--rw-r--r--   0        0        0   108928 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/background.jpg
--rw-r--r--   0        0        0     1935 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/theme.conf
--rw-r--r--   0        0        0   514555 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/background.jpg
--rw-r--r--   0        0        0     2422 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/theme.conf
--rw-r--r--   0        0        0     5683 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/util.py
--rw-r--r--   0        0        0      703 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    23384 1970-01-01 00:00:00.000000 ohmyi3-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.4/LICENSE
+-rw-r--r--   0        0        0    22565 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/README.md
+-rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.4/ohmyi3/commands/entrypoint.py
+-rw-r--r--   0        0        0     3208 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/commands/generate.py
+-rw-r--r--   0        0        0      432 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/commands/info.py
+-rw-r--r--   0        0        0     1529 2023-04-20 23:03:25.268975 ohmyi3-0.1.4/ohmyi3/commands/init.py
+-rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.4/ohmyi3/config/app.py
+-rw-r--r--   0        0        0     2238 2023-04-20 23:03:25.268975 ohmyi3-0.1.4/ohmyi3/config/package.py
+-rw-r--r--   0        0        0      446 2023-04-20 23:03:25.268975 ohmyi3-0.1.4/ohmyi3/i3ctl.py
+-rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.4/ohmyi3/services/bootstrap.py
+-rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.4/ohmyi3/services/ohmyi3.py
+-rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.4/ohmyi3/stubs/README.md
+-rw-r--r--   0        0        0      810 2023-04-22 16:38:39.408913 ohmyi3-0.1.4/ohmyi3/stubs/config.d/00-header.conf
+-rw-r--r--   0        0        0     1985 2023-04-22 16:38:39.408913 ohmyi3-0.1.4/ohmyi3/stubs/config.d/05-system.conf
+-rw-r--r--   0        0        0     3035 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/stubs/config.d/10-autostart.conf
+-rw-r--r--   0        0        0      775 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/stubs/config.d/15-borders.conf
+-rw-r--r--   0        0        0     6434 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/stubs/config.d/20-navigation.conf
+-rw-r--r--   0        0        0     3212 2023-04-22 16:38:39.412246 ohmyi3-0.1.4/ohmyi3/stubs/config.d/80-applications.conf
+-rw-r--r--   0        0        0     6720 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/stubs/config.d/85-windows.conf
+-rw-r--r--   0        0        0     3195 2023-04-22 16:38:39.412246 ohmyi3-0.1.4/ohmyi3/stubs/config.d/90-gaps.conf
+-rw-r--r--   0        0        0    12738 2023-04-22 16:39:52.219550 ohmyi3-0.1.4/ohmyi3/stubs/config.py
+-rw-r--r--   0        0        0       33 2023-04-22 16:38:50.699004 ohmyi3-0.1.4/ohmyi3/stubs/plugins/alacritty/__init__.py
+-rw-r--r--   0        0        0      893 2023-04-22 16:38:50.699004 ohmyi3-0.1.4/ohmyi3/stubs/plugins/alacritty/alacritty.py
+-rw-r--r--   0        0        0       29 2023-04-22 16:38:50.699004 ohmyi3-0.1.4/ohmyi3/stubs/plugins/archey3/__init__.py
+-rw-r--r--   0        0        0      958 2023-04-22 16:38:50.699004 ohmyi3-0.1.4/ohmyi3/stubs/plugins/archey3/archey3.py
+-rw-r--r--   0        0        0       31 2023-04-22 16:38:50.702337 ohmyi3-0.1.4/ohmyi3/stubs/plugins/nitrogen/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-22 16:38:50.702337 ohmyi3-0.1.4/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
+-rw-r--r--   0        0        0       29 2023-04-22 16:38:50.702337 ohmyi3-0.1.4/ohmyi3/stubs/plugins/polybar/__init__.py
+-rw-r--r--   0        0        0     2188 2023-04-22 16:38:50.702337 ohmyi3-0.1.4/ohmyi3/stubs/plugins/polybar/polybar.py
+-rw-r--r--   0        0        0   385109 2023-04-22 16:39:04.589120 ohmyi3-0.1.4/ohmyi3/stubs/themes/amber/background.jpg
+-rw-r--r--   0        0        0     1874 2023-04-22 16:39:04.589120 ohmyi3-0.1.4/ohmyi3/stubs/themes/amber/theme.conf
+-rw-r--r--   0        0        0   198158 2023-04-22 16:39:04.589120 ohmyi3-0.1.4/ohmyi3/stubs/themes/archlinux/background.jpg
+-rw-r--r--   0        0        0     1915 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/archlinux/theme.conf
+-rw-r--r--   0        0        0     1869 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/i3status.conf
+-rw-r--r--   0        0        0   108928 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/manjaro/background.jpg
+-rw-r--r--   0        0        0     1935 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/manjaro/theme.conf
+-rw-r--r--   0        0        0   514555 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/pink/background.jpg
+-rw-r--r--   0        0        0     2422 2023-04-22 16:39:04.592453 ohmyi3-0.1.4/ohmyi3/stubs/themes/pink/theme.conf
+-rw-r--r--   0        0        0     5800 2023-04-23 15:39:17.356053 ohmyi3-0.1.4/ohmyi3/util.py
+-rw-r--r--   0        0        0      703 2023-04-23 15:39:17.359387 ohmyi3-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    23384 1970-01-01 00:00:00.000000 ohmyi3-0.1.4/PKG-INFO
```

### Comparing `ohmyi3-0.1.3/LICENSE` & `ohmyi3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/README.md` & `ohmyi3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/commands/entrypoint.py` & `ohmyi3-0.1.4/ohmyi3/commands/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/commands/generate.py` & `ohmyi3-0.1.4/ohmyi3/commands/generate.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/commands/init.py` & `ohmyi3-0.1.4/ohmyi3/commands/init.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/config/app.py` & `ohmyi3-0.1.4/ohmyi3/config/app.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/config/package.py` & `ohmyi3-0.1.4/ohmyi3/config/package.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/services/bootstrap.py` & `ohmyi3-0.1.4/ohmyi3/services/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/services/ohmyi3.py` & `ohmyi3-0.1.4/ohmyi3/services/ohmyi3.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/00-header.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/00-header.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/05-system.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/05-system.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/10-autostart.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/10-autostart.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/15-borders.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/15-borders.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/20-navigation.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/20-navigation.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/80-applications.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/80-applications.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/85-windows.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/85-windows.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.d/90-gaps.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/config.d/90-gaps.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/config.py` & `ohmyi3-0.1.4/ohmyi3/stubs/config.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/alacritty.py` & `ohmyi3-0.1.4/ohmyi3/stubs/plugins/alacritty/alacritty.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/archey3.py` & `ohmyi3-0.1.4/ohmyi3/stubs/plugins/archey3/archey3.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/nitrogen.py` & `ohmyi3-0.1.4/ohmyi3/stubs/plugins/nitrogen/nitrogen.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/polybar.py` & `ohmyi3-0.1.4/ohmyi3/stubs/plugins/polybar/polybar.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/background.jpg` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/amber/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/theme.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/amber/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/background.jpg` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/archlinux/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/theme.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/archlinux/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/i3status.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/i3status.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/background.jpg` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/manjaro/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/theme.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/manjaro/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/background.jpg` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/pink/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/theme.conf` & `ohmyi3-0.1.4/ohmyi3/stubs/themes/pink/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.3/ohmyi3/util.py` & `ohmyi3-0.1.4/ohmyi3/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import platform
+import subprocess
 from uvicore.typing import Dict
 from datetime import datetime
 from uvicore.support.module import load
 from jinja2 import Environment as JinjaEnv
 from uvicore.support.dumper import dump, dd
 from jinja2 import FileSystemLoader as JinjaLoader
 
@@ -39,15 +40,16 @@
 def now(dateformat='%Y-%m-%d_%H-%M-%S'):
     """Get now() date time in specified format (defaults 2021-01-24_19-24-58)"""
     return datetime.now().strftime(dateformat)
 
 
 def shell(cmd):
     """Execute a shell command"""
-    return os.system(cmd)
+    #return os.system(cmd)
+    return subprocess.run(cmd, shell=True, stdout=subprocess.PIPE).stdout.decode('utf-8').split()
 
 
 def template(file, *, base=None, output=None, values=None) -> str:
     """Render a single file through the Jinja2 templating system, return or write output"""
     if not base: base = os.path.dirname(file)
     base = path(base)
     filename = os.path.basename(file)
```

### Comparing `ohmyi3-0.1.3/pyproject.toml` & `ohmyi3-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ohmyi3"
-version = "0.1.3"
+version = "0.1.4"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "Dynamic i3 Configuration Manager "
 homepage = "https://github.com/ohmyi3/ohmyi3"
 documentation = "https://github.com/ohmyi3/ohmyi3"
 repository = "https://github.com/ohmyi3/ohmyi3"
 readme = "README.md"
```

### Comparing `ohmyi3-0.1.3/PKG-INFO` & `ohmyi3-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmyi3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dynamic i3 Configuration Manager 
 Home-page: https://github.com/ohmyi3/ohmyi3
 License: MIT
 Author: Matthew Reschke
 Author-email: mail@mreschke.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

