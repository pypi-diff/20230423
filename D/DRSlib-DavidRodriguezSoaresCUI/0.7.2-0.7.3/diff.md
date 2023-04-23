# Comparing `tmp/DRSlib-DavidRodriguezSoaresCUI-0.7.2.tar.gz` & `tmp/DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.7.2.tar", last modified: Sun Apr 23 14:13:17 2023, max compression
+gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar", last modified: Sun Apr 23 16:04:45 2023, max compression
```

## Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2.tar` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 14:13:17.439693 DRSlib-DavidRodriguezSoaresCUI-0.7.2/
--rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     3503 2023-04-23 14:13:17.439693 DRSlib-DavidRodriguezSoaresCUI-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/README.md
--rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0     1102 2023-04-23 14:13:17.440694 DRSlib-DavidRodriguezSoaresCUI-0.7.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 14:13:17.409664 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 14:13:17.424677 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/
--rw-rw-rw-   0        0        0      697 2023-04-22 15:27:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/__init__.py
--rw-rw-rw-   0        0        0     5046 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/banner.py
--rw-rw-rw-   0        0        0     9820 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/cli_ui.py
--rw-rw-rw-   0        0        0     6182 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/debug.py
--rw-rw-rw-   0        0        0     9731 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/decorators.py
--rw-rw-rw-   0        0        0     3413 2023-04-23 13:58:36.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/dict_utils.py
--rw-rw-rw-   0        0        0     1370 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/execute.py
--rw-rw-rw-   0        0        0    13598 2023-04-22 15:31:18.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/fsdb.py
--rw-rw-rw-   0        0        0     4219 2023-04-23 12:12:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/hash.py
--rw-rw-rw-   0        0        0     3410 2023-04-22 08:30:58.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/interval.py
--rw-rw-rw-   0        0        0      444 2023-04-23 12:01:10.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/list_utils.py
--rw-rw-rw-   0        0        0    15553 2023-04-23 12:11:23.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/mediainfo.py
--rw-rw-rw-   0        0        0     1329 2023-04-23 14:11:24.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/multiprocessing.py
--rw-rw-rw-   0        0        0     1568 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/os_detect.py
--rw-rw-rw-   0        0        0    13957 2023-04-22 15:33:39.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/path_tools.py
--rw-rw-rw-   0        0        0     2266 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/spinner.py
--rw-rw-rw-   0        0        0     4188 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/str_utils.py
--rw-rw-rw-   0        0        0     4040 2023-04-23 12:10:40.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 14:13:17.438692 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     3503 2023-04-23 14:13:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-04-23 14:13:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 14:13:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-23 14:13:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 14:13:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/
+-rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     3503 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/README.md
+-rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1102 2023-04-23 16:04:45.074573 DRSlib-DavidRodriguezSoaresCUI-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.045775 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.060789 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/
+-rw-rw-rw-   0        0        0      697 2023-04-22 15:27:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/__init__.py
+-rw-rw-rw-   0        0        0     5046 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/banner.py
+-rw-rw-rw-   0        0        0     9799 2023-04-23 16:02:46.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/cli_ui.py
+-rw-rw-rw-   0        0        0     6182 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/debug.py
+-rw-rw-rw-   0        0        0     9731 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/decorators.py
+-rw-rw-rw-   0        0        0     3413 2023-04-23 13:58:36.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/dict_utils.py
+-rw-rw-rw-   0        0        0     1370 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/execute.py
+-rw-rw-rw-   0        0        0    13598 2023-04-22 15:31:18.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/fsdb.py
+-rw-rw-rw-   0        0        0     4219 2023-04-23 12:12:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/hash.py
+-rw-rw-rw-   0        0        0     3410 2023-04-22 08:30:58.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/interval.py
+-rw-rw-rw-   0        0        0      444 2023-04-23 12:01:10.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/list_utils.py
+-rw-rw-rw-   0        0        0    15553 2023-04-23 12:11:23.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/mediainfo.py
+-rw-rw-rw-   0        0        0     1329 2023-04-23 14:11:24.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/multiprocessing.py
+-rw-rw-rw-   0        0        0     1568 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/os_detect.py
+-rw-rw-rw-   0        0        0    13957 2023-04-22 15:33:39.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/path_tools.py
+-rw-rw-rw-   0        0        0     2266 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/spinner.py
+-rw-rw-rw-   0        0        0     4188 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/str_utils.py
+-rw-rw-rw-   0        0        0     4040 2023-04-23 12:10:40.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     3503 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/LICENSE` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.7.2
+Version: 0.7.3
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/README.md` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/setup.cfg` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 5253 6c69 622d 4461 7669 6452   = DRSlib-DavidR
 00000020: 6f64 7269 6775 657a 536f 6172 6573 4355  odriguezSoaresCU
 00000030: 490d 0a76 6572 7369 6f6e 203d 2030 2e37  I..version = 0.7
-00000040: 2e32 0d0a 6175 7468 6f72 203d 2044 6176  .2..author = Dav
+00000040: 2e33 0d0a 6175 7468 6f72 203d 2044 6176  .3..author = Dav
 00000050: 6964 526f 6472 6967 7565 7a53 6f61 7265  idRodriguezSoare
 00000060: 7343 5549 0d0a 6175 7468 6f72 5f65 6d61  sCUI..author_ema
 00000070: 696c 203d 2066 6972 6562 6c61 7a65 3930  il = fireblaze90
 00000080: 342b 4452 536c 6962 4067 6d61 696c 2e63  4+DRSlib@gmail.c
 00000090: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 000000a0: 3d20 4452 536c 6962 202d 2061 2073 6574  = DRSlib - a set
 000000b0: 206f 6620 7574 696c 6974 6965 7320 6279   of utilities by
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/__init__.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/__init__.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/banner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/banner.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/cli_ui.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/cli_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,33 +122,32 @@
         if acceptable_UI(_user_input):
             return _user_input
 
         # case: processed user input is accepted
         variations = ["int(_user_input)", "float(_user_input)", "_user_input.lower()"]
         for variation in variations:
             try:
-                __user_input = ast.literal_eval(variation)
+                __user_input = eval(variation)
                 if acceptable_UI(__user_input):
                     return __user_input
             except (ValueError, AttributeError):
                 pass
 
         # case: user input is not accepted AND there is a default
         if default is not None:
             return default
 
         # case: user input is not accepted AND there is no default => notify user, ask again
         print(
-            "Input '%s' is not a valid input. %s",
-            _user_input,
-            (f"Please choose one of : {accepted}" if not callable(accepted) else ""),
+            f"Input '{_user_input}' is not a valid input.",
+            (f" Please choose one of : {accepted}" if not callable(accepted) else ""),
         )
 
 
-def choose_from_list(choices: list, default: Optional[int]) -> Any:
+def choose_from_list(choices: list, default: Optional[int] = None) -> Any:
     """Prints then asks the user to choose an item from a list
     `default`
     """
     # Print choices
     print(
         "Choices:\n  "
         + "\n  ".join([f"[{idx}] {choice}" for idx, choice in enumerate(choices)])
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/debug.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/debug.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/decorators.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/decorators.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/dict_utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/dict_utils.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/execute.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/execute.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/fsdb.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/fsdb.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/hash.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/hash.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/interval.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/interval.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/mediainfo.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/mediainfo.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/multiprocessing.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/os_detect.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/os_detect.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/path_tools.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/path_tools.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/spinner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/spinner.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/str_utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/str_utils.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib/utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/utils.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.7.2
+Version: 0.7.3
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.2/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

