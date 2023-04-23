# Comparing `tmp/giftmaster-0.1.59.tar.gz` & `tmp/giftmaster-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giftmaster-0.1.59.tar", last modified: Sun Apr 23 16:49:01 2023, max compression
+gzip compressed data, was "giftmaster-0.1.60.tar", last modified: Sun Apr 23 17:05:46 2023, max compression
```

## Comparing `giftmaster-0.1.59.tar` & `giftmaster-0.1.60.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.028118 giftmaster-0.1.59/
--rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.59/.cirrus.yml
--rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.59/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.59/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.59/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.59/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.59/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.59/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.59/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.59/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.59/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:49:01.028303 giftmaster-0.1.59/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.59/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.017865 giftmaster-0.1.59/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.018632 giftmaster-0.1.59/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.59/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.59/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 16:49:01.029266 giftmaster-0.1.59/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.59/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.001299 giftmaster-0.1.59/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.022451 giftmaster-0.1.59/src/giftmaster/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.59/src/giftmaster/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.59/src/giftmaster/args.py
--rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.59/src/giftmaster/logger.py
--rw-r--r--   0 mtm        (501) staff       (20)     5325 2023-04-23 16:46:46.000000 giftmaster-0.1.59/src/giftmaster/signtool.py
--rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.59/src/giftmaster/skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.59/src/giftmaster/timestamp.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.026338 giftmaster-0.1.59/src/giftmaster.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.59/src/giftmaster.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 16:49:00.000000 giftmaster-0.1.59/src/giftmaster.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:49:01.027651 giftmaster-0.1.59/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.59/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.59/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.59/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.939041 giftmaster-0.1.60/
+-rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.60/.cirrus.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.60/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.60/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.60/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.60/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.60/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.60/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.60/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.60/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.60/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 17:05:46.939206 giftmaster-0.1.60/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.60/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.927765 giftmaster-0.1.60/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.929303 giftmaster-0.1.60/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.60/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.60/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 17:05:46.940086 giftmaster-0.1.60/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.60/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.887686 giftmaster-0.1.60/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.935432 giftmaster-0.1.60/src/giftmaster/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.60/src/giftmaster/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.60/src/giftmaster/args.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.60/src/giftmaster/logger.py
+-rw-r--r--   0 mtm        (501) staff       (20)     5015 2023-04-23 17:04:07.000000 giftmaster-0.1.60/src/giftmaster/signtool.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.60/src/giftmaster/skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.60/src/giftmaster/timestamp.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.938073 giftmaster-0.1.60/src/giftmaster.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.60/src/giftmaster.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 17:05:46.000000 giftmaster-0.1.60/src/giftmaster.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 17:05:46.938680 giftmaster-0.1.60/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.60/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.60/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.60/tox.ini
```

### Comparing `giftmaster-0.1.59/.cirrus.yml` & `giftmaster-0.1.60/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/.coveragerc` & `giftmaster-0.1.60/.coveragerc`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/.gitignore` & `giftmaster-0.1.60/.gitignore`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/.pre-commit-config.yaml` & `giftmaster-0.1.60/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/CONTRIBUTING.rst` & `giftmaster-0.1.60/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/LICENSE.txt` & `giftmaster-0.1.60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/PKG-INFO` & `giftmaster-0.1.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.59
+Version: 0.1.60
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.59/README.rst` & `giftmaster-0.1.60/README.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/docs/Makefile` & `giftmaster-0.1.60/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/docs/conf.py` & `giftmaster-0.1.60/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/docs/index.rst` & `giftmaster-0.1.60/docs/index.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/setup.cfg` & `giftmaster-0.1.60/setup.cfg`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/setup.py` & `giftmaster-0.1.60/setup.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/src/giftmaster/__init__.py` & `giftmaster-0.1.60/src/giftmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/src/giftmaster/args.py` & `giftmaster-0.1.60/src/giftmaster/args.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/src/giftmaster/logger.py` & `giftmaster-0.1.60/src/giftmaster/logger.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/src/giftmaster/signtool.py` & `giftmaster-0.1.60/src/giftmaster/signtool.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 
 class SigntoolPrivatekeyException(Exception):
     def __init__(self, message="signtool couldn't get a private key"):
         self.message = message
         super().__init__(self.message)
 
 
-class SigntoolFileNotSignedException(Exception):
-    def __init__(self, message="file is not signed"):
-        self.message = message
-        super().__init__(self.message)
-
-
 def unsign_cmd(*paths, signtool="signtool"):
     cmd = [
         signtool,  # fixme
         "remove",
         "/v",
         "/s",
     ]
@@ -110,19 +104,16 @@
         log_path = pathlib.Path(f"signtool-{epoch}.log")
         err_path = pathlib.Path(f"signtool-{epoch}.err")
         stdout, stderr = process.communicate()
         err_path.write_text(stderr.decode())
         log_path.write_text(stdout.decode())
 
         if err := stderr.decode():
-            if "No private key is available".lower() in err.lower():
+            if "No private key is available" in err:
                 raise SigntoolPrivatekeyException(err)
-            if "No signature found".lower() in err.lower():
-                raise SigntoolFileNotSignedException(err)
-
             logging.warning(err)
 
         logging.debug(f"singtool.exe's returncode: {process.returncode}")
         return process.returncode
 
     def verify_cmd(self, *paths: List[str]):
         """
```

### Comparing `giftmaster-0.1.59/src/giftmaster/skeleton.py` & `giftmaster-0.1.60/src/giftmaster/skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/src/giftmaster.egg-info/PKG-INFO` & `giftmaster-0.1.60/src/giftmaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.59
+Version: 0.1.60
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.59/src/giftmaster.egg-info/SOURCES.txt` & `giftmaster-0.1.60/src/giftmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/tests/test_skeleton.py` & `giftmaster-0.1.60/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.59/tox.ini` & `giftmaster-0.1.60/tox.ini`

 * *Files identical despite different names*

