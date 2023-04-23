# Comparing `tmp/giftmaster-0.1.57.tar.gz` & `tmp/giftmaster-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giftmaster-0.1.57.tar", last modified: Sun Apr 23 16:04:19 2023, max compression
+gzip compressed data, was "giftmaster-0.1.58.tar", last modified: Sun Apr 23 16:41:01 2023, max compression
```

## Comparing `giftmaster-0.1.57.tar` & `giftmaster-0.1.58.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.438742 giftmaster-0.1.57/
--rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.57/.cirrus.yml
--rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.57/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.57/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.57/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.57/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.57/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.57/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.57/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.57/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.57/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:04:19.439063 giftmaster-0.1.57/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.57/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.426950 giftmaster-0.1.57/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.427545 giftmaster-0.1.57/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.57/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.57/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 16:04:19.440649 giftmaster-0.1.57/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.57/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.411194 giftmaster-0.1.57/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.432442 giftmaster-0.1.57/src/giftmaster/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.57/src/giftmaster/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.57/src/giftmaster/args.py
--rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.57/src/giftmaster/logger.py
--rw-r--r--   0 mtm        (501) staff       (20)     5016 2023-04-23 16:03:32.000000 giftmaster-0.1.57/src/giftmaster/signtool.py
--rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.57/src/giftmaster/skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.57/src/giftmaster/timestamp.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.436776 giftmaster-0.1.57/src/giftmaster.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.57/src/giftmaster.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 16:04:19.000000 giftmaster-0.1.57/src/giftmaster.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:04:19.438102 giftmaster-0.1.57/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.57/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.57/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.57/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.037140 giftmaster-0.1.58/
+-rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.58/.cirrus.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.58/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.58/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.58/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.58/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.58/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.58/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.58/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.58/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.58/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:41:01.037557 giftmaster-0.1.58/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.58/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.021779 giftmaster-0.1.58/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.022531 giftmaster-0.1.58/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.58/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.58/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 16:41:01.039027 giftmaster-0.1.58/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.58/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.007217 giftmaster-0.1.58/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.029480 giftmaster-0.1.58/src/giftmaster/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.58/src/giftmaster/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.58/src/giftmaster/args.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.58/src/giftmaster/logger.py
+-rw-r--r--   0 mtm        (501) staff       (20)     5015 2023-04-23 16:37:07.000000 giftmaster-0.1.58/src/giftmaster/signtool.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.58/src/giftmaster/skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.58/src/giftmaster/timestamp.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.034775 giftmaster-0.1.58/src/giftmaster.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 16:41:00.000000 giftmaster-0.1.58/src/giftmaster.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 16:41:01.000000 giftmaster-0.1.58/src/giftmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 16:41:00.000000 giftmaster-0.1.58/src/giftmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 16:41:00.000000 giftmaster-0.1.58/src/giftmaster.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.58/src/giftmaster.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 16:41:00.000000 giftmaster-0.1.58/src/giftmaster.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 16:41:00.000000 giftmaster-0.1.58/src/giftmaster.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 16:41:01.036291 giftmaster-0.1.58/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.58/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.58/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.58/tox.ini
```

### Comparing `giftmaster-0.1.57/.cirrus.yml` & `giftmaster-0.1.58/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/.coveragerc` & `giftmaster-0.1.58/.coveragerc`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/.gitignore` & `giftmaster-0.1.58/.gitignore`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/.pre-commit-config.yaml` & `giftmaster-0.1.58/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/CONTRIBUTING.rst` & `giftmaster-0.1.58/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/LICENSE.txt` & `giftmaster-0.1.58/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/PKG-INFO` & `giftmaster-0.1.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.57
+Version: 0.1.58
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.57/README.rst` & `giftmaster-0.1.58/README.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/docs/Makefile` & `giftmaster-0.1.58/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/docs/conf.py` & `giftmaster-0.1.58/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/docs/index.rst` & `giftmaster-0.1.58/docs/index.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/setup.cfg` & `giftmaster-0.1.58/setup.cfg`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/setup.py` & `giftmaster-0.1.58/setup.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/src/giftmaster/__init__.py` & `giftmaster-0.1.58/src/giftmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/src/giftmaster/args.py` & `giftmaster-0.1.58/src/giftmaster/args.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/src/giftmaster/logger.py` & `giftmaster-0.1.58/src/giftmaster/logger.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/src/giftmaster/signtool.py` & `giftmaster-0.1.58/src/giftmaster/signtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         log_path = pathlib.Path(f"signtool-{epoch}.log")
         err_path = pathlib.Path(f"signtool-{epoch}.err")
         stdout, stderr = process.communicate()
         err_path.write_text(stderr.decode())
         log_path.write_text(stdout.decode())
 
         if err := stderr.decode():
-            logging.critical(err)
             if "No private key is available" in err:
                 raise SigntoolPrivatekeyException(err)
+            logging.warning(err)
 
         logging.debug(f"singtool.exe's returncode: {process.returncode}")
         return process.returncode
 
     def verify_cmd(self, *paths: List[str]):
         """
         signtool.exe verify /debug /v /pa C:\dxLib.dll
```

### Comparing `giftmaster-0.1.57/src/giftmaster/skeleton.py` & `giftmaster-0.1.58/src/giftmaster/skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/src/giftmaster.egg-info/PKG-INFO` & `giftmaster-0.1.58/src/giftmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.1.57
+Version: 0.1.58
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `giftmaster-0.1.57/src/giftmaster.egg-info/SOURCES.txt` & `giftmaster-0.1.58/src/giftmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/tests/test_skeleton.py` & `giftmaster-0.1.58/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.1.57/tox.ini` & `giftmaster-0.1.58/tox.ini`

 * *Files identical despite different names*

