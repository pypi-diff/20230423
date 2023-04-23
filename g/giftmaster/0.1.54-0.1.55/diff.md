# Comparing `tmp/giftmaster-0.1.54.tar.gz` & `tmp/giftmaster-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giftmaster-0.1.54.tar", last modified: Sun Apr 23 15:14:44 2023, max compression
+gzip compressed data, was "giftmaster-0.1.55.tar", last modified: Sun Apr 23 15:34:44 2023, max compression
```

## Comparing `giftmaster-0.1.54.tar` & `giftmaster-0.1.55.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.199430 giftmaster-0.1.54/
--rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.54/.cirrus.yml
--rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.54/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.54/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.54/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.54/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:14:44.199681 giftmaster-0.1.54/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.54/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.186027 giftmaster-0.1.54/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.187393 giftmaster-0.1.54/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.54/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 15:14:44.201179 giftmaster-0.1.54/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.54/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.168588 giftmaster-0.1.54/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.192505 giftmaster-0.1.54/src/giftmaster/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.54/src/giftmaster/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.54/src/giftmaster/args.py
--rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.54/src/giftmaster/logger.py
--rw-r--r--   0 mtm        (501) staff       (20)     4718 2023-04-23 15:13:57.000000 giftmaster-0.1.54/src/giftmaster/signtool.py
--rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.54/src/giftmaster/skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.54/src/giftmaster/timestamp.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.197567 giftmaster-0.1.54/src/giftmaster.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.54/src/giftmaster.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.198900 giftmaster-0.1.54/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.54/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.54/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.54/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.531568 giftmaster-0.1.55/
+-rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.55/.cirrus.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.55/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.55/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.55/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.55/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.55/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.55/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.55/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.55/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.55/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:34:44.531837 giftmaster-0.1.55/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.55/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.520388 giftmaster-0.1.55/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.521239 giftmaster-0.1.55/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.55/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.55/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 15:34:44.533518 giftmaster-0.1.55/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.55/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.503976 giftmaster-0.1.55/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.525354 giftmaster-0.1.55/src/giftmaster/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.55/src/giftmaster/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.55/src/giftmaster/args.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.55/src/giftmaster/logger.py
+-rw-r--r--   0 mtm        (501) staff       (20)     5041 2023-04-23 15:32:18.000000 giftmaster-0.1.55/src/giftmaster/signtool.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.55/src/giftmaster/skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.55/src/giftmaster/timestamp.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.529446 giftmaster-0.1.55/src/giftmaster.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.55/src/giftmaster.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 15:34:44.000000 giftmaster-0.1.55/src/giftmaster.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:34:44.530826 giftmaster-0.1.55/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.55/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.55/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.55/tox.ini
```

### Comparing `giftmaster-0.1.54/.cirrus.yml` & `giftmaster-0.1.55/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/.coveragerc` & `giftmaster-0.1.55/.coveragerc`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/.gitignore` & `giftmaster-0.1.55/.gitignore`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/.pre-commit-config.yaml` & `giftmaster-0.1.55/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/CONTRIBUTING.rst` & `giftmaster-0.1.55/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/LICENSE.txt` & `giftmaster-0.1.55/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/PKG-INFO` & `giftmaster-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.54
+Version: 0.1.55
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.54/README.rst` & `giftmaster-0.1.55/README.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/docs/Makefile` & `giftmaster-0.1.55/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/docs/conf.py` & `giftmaster-0.1.55/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/docs/index.rst` & `giftmaster-0.1.55/docs/index.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/setup.cfg` & `giftmaster-0.1.55/setup.cfg`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/setup.py` & `giftmaster-0.1.55/setup.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/src/giftmaster/__init__.py` & `giftmaster-0.1.55/src/giftmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/src/giftmaster/args.py` & `giftmaster-0.1.55/src/giftmaster/args.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/src/giftmaster/logger.py` & `giftmaster-0.1.55/src/giftmaster/logger.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/src/giftmaster/signtool.py` & `giftmaster-0.1.55/src/giftmaster/signtool.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 from typing import List
 
 from foodsale import pathfromglob
 
 from giftmaster import timestamp
 
 
+class SigntoolPrivatekeyException(Exception):
+    def __init__(self, message="signtool couldn't get a private key"):
+        self.message = message
+        super().__init__(self.message)
+
+
 def unsign_cmd(*paths, signtool="signtool"):
     cmd = [
         signtool,  # fixme
         "remove",
         "/v",
         "/s",
     ]
@@ -99,14 +105,16 @@
         err_path = pathlib.Path(f"signtool-{epoch}.err")
         stdout, stderr = process.communicate()
         err_path.write_text(stderr.decode())
         log_path.write_text(stdout.decode())
 
         if err := stderr.decode():
             logging.warning(err)
+            if "No private key is available" in err:
+                raise SigntoolPrivatekeyException("No private key is available")
 
         logging.debug(f"singtool.exe's returncode: {process.returncode}")
         return process.returncode
 
     def verify_cmd(self, *paths: List[str]):
         """
         signtool.exe verify /debug /v /pa C:\dxLib.dll
```

### Comparing `giftmaster-0.1.54/src/giftmaster/skeleton.py` & `giftmaster-0.1.55/src/giftmaster/skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/src/giftmaster.egg-info/PKG-INFO` & `giftmaster-0.1.55/src/giftmaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.54
+Version: 0.1.55
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.54/src/giftmaster.egg-info/SOURCES.txt` & `giftmaster-0.1.55/src/giftmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/tests/test_skeleton.py` & `giftmaster-0.1.55/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.54/tox.ini` & `giftmaster-0.1.55/tox.ini`

 * *Files identical despite different names*

