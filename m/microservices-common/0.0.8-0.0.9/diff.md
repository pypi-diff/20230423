# Comparing `tmp/microservices_common-0.0.8.tar.gz` & `tmp/microservices_common-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservices_common-0.0.8.tar", last modified: Mon May 16 11:50:59 2022, max compression
+gzip compressed data, was "microservices_common-0.0.9.tar", last modified: Mon May 16 11:55:14 2022, max compression
```

## Comparing `microservices_common-0.0.8.tar` & `microservices_common-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.047216 microservices_common-0.0.8/
--rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:50:59.046830 microservices_common-0.0.8/PKG-INFO
--rw-r--r--   0 alizaidi   (501) staff       (20)       38 2022-05-16 11:50:59.047365 microservices_common-0.0.8/setup.cfg
--rw-r--r--   0 alizaidi   (501) staff       (20)      657 2022-05-16 11:50:54.000000 microservices_common-0.0.8/setup.py
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.031646 microservices_common-0.0.8/src/
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.033131 microservices_common-0.0.8/src/microservices_common/
--rw-r--r--   0 alizaidi   (501) staff       (20)      134 2022-05-16 11:49:38.000000 microservices_common-0.0.8/src/microservices_common/__init__.py
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.040505 microservices_common-0.0.8/src/microservices_common/exceptions/
--rw-r--r--   0 alizaidi   (501) staff       (20)      425 2022-05-16 11:49:52.000000 microservices_common-0.0.8/src/microservices_common/exceptions/__init__.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      333 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/authentication_exception.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      361 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/custom_exception.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      366 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      448 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/invalid_input_exception.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      358 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/not_found_exception.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      333 2022-05-16 09:57:25.000000 microservices_common-0.0.8/src/microservices_common/exceptions/owner_not_found_exception.py
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.043522 microservices_common-0.0.8/src/microservices_common/middlewares/
--rw-r--r--   0 alizaidi   (501) staff       (20)      302 2022-05-16 11:50:11.000000 microservices_common-0.0.8/src/microservices_common/middlewares/__init__.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      327 2022-05-16 11:50:38.000000 microservices_common-0.0.8/src/microservices_common/middlewares/admin.py
--rw-r--r--   0 alizaidi   (501) staff       (20)     2246 2022-05-16 10:24:20.000000 microservices_common-0.0.8/src/microservices_common/middlewares/authorized.py
--rw-r--r--   0 alizaidi   (501) staff       (20)      879 2022-05-16 10:24:22.000000 microservices_common-0.0.8/src/microservices_common/middlewares/exception_handler.py
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.045345 microservices_common-0.0.8/src/microservices_common/util/
--rw-r--r--   0 alizaidi   (501) staff       (20)       45 2022-05-16 11:50:21.000000 microservices_common-0.0.8/src/microservices_common/util/__init__.py
--rw-r--r--   0 alizaidi   (501) staff       (20)    33353 2022-05-16 11:30:44.000000 microservices_common-0.0.8/src/microservices_common/util/util.py
-drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:50:59.036051 microservices_common-0.0.8/src/microservices_common.egg-info/
--rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:50:58.000000 microservices_common-0.0.8/src/microservices_common.egg-info/PKG-INFO
--rw-r--r--   0 alizaidi   (501) staff       (20)      999 2022-05-16 11:50:58.000000 microservices_common-0.0.8/src/microservices_common.egg-info/SOURCES.txt
--rw-r--r--   0 alizaidi   (501) staff       (20)        1 2022-05-16 11:50:58.000000 microservices_common-0.0.8/src/microservices_common.egg-info/dependency_links.txt
--rw-r--r--   0 alizaidi   (501) staff       (20)       78 2022-05-16 11:50:58.000000 microservices_common-0.0.8/src/microservices_common.egg-info/requires.txt
--rw-r--r--   0 alizaidi   (501) staff       (20)       21 2022-05-16 11:50:58.000000 microservices_common-0.0.8/src/microservices_common.egg-info/top_level.txt
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.114914 microservices_common-0.0.9/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:55:14.114564 microservices_common-0.0.9/PKG-INFO
+-rw-r--r--   0 alizaidi   (501) staff       (20)       38 2022-05-16 11:55:14.115047 microservices_common-0.0.9/setup.cfg
+-rw-r--r--   0 alizaidi   (501) staff       (20)      657 2022-05-16 11:55:09.000000 microservices_common-0.0.9/setup.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.105630 microservices_common-0.0.9/src/
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.106900 microservices_common-0.0.9/src/microservices_common/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      134 2022-05-16 11:55:01.000000 microservices_common-0.0.9/src/microservices_common/__init__.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.111537 microservices_common-0.0.9/src/microservices_common/exceptions/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      425 2022-05-16 11:49:52.000000 microservices_common-0.0.9/src/microservices_common/exceptions/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      354 2022-05-16 11:53:58.000000 microservices_common-0.0.9/src/microservices_common/exceptions/authentication_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      361 2022-05-16 09:57:25.000000 microservices_common-0.0.9/src/microservices_common/exceptions/custom_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      387 2022-05-16 11:54:04.000000 microservices_common-0.0.9/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      469 2022-05-16 11:54:08.000000 microservices_common-0.0.9/src/microservices_common/exceptions/invalid_input_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      379 2022-05-16 11:54:12.000000 microservices_common-0.0.9/src/microservices_common/exceptions/not_found_exception.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      354 2022-05-16 11:54:15.000000 microservices_common-0.0.9/src/microservices_common/exceptions/owner_not_found_exception.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.113222 microservices_common-0.0.9/src/microservices_common/middlewares/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      302 2022-05-16 11:50:11.000000 microservices_common-0.0.9/src/microservices_common/middlewares/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      348 2022-05-16 11:54:23.000000 microservices_common-0.0.9/src/microservices_common/middlewares/admin.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)     2246 2022-05-16 10:24:20.000000 microservices_common-0.0.9/src/microservices_common/middlewares/authorized.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)      921 2022-05-16 11:54:36.000000 microservices_common-0.0.9/src/microservices_common/middlewares/exception_handler.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.113977 microservices_common-0.0.9/src/microservices_common/util/
+-rw-r--r--   0 alizaidi   (501) staff       (20)       45 2022-05-16 11:50:21.000000 microservices_common-0.0.9/src/microservices_common/util/__init__.py
+-rw-r--r--   0 alizaidi   (501) staff       (20)    33374 2022-05-16 11:54:50.000000 microservices_common-0.0.9/src/microservices_common/util/util.py
+drwxr-xr-x   0 alizaidi   (501) staff       (20)        0 2022-05-16 11:55:14.108924 microservices_common-0.0.9/src/microservices_common.egg-info/
+-rw-r--r--   0 alizaidi   (501) staff       (20)      392 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/PKG-INFO
+-rw-r--r--   0 alizaidi   (501) staff       (20)      999 2022-05-16 11:55:14.000000 microservices_common-0.0.9/src/microservices_common.egg-info/SOURCES.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)        1 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/dependency_links.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)       78 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/requires.txt
+-rw-r--r--   0 alizaidi   (501) staff       (20)       21 2022-05-16 11:55:13.000000 microservices_common-0.0.9/src/microservices_common.egg-info/top_level.txt
```

### Comparing `microservices_common-0.0.8/setup.py` & `microservices_common-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="microservices_common",
-    version="0.0.8",
+    version="0.0.9",
     author="Ali Zaidi",
     author_email="support@arrivy.com",
     description="",
     long_description="",
     url="https://github.com/arrivy-dev/microservices-python-common",
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `microservices_common-0.0.8/src/microservices_common/middlewares/authorized.py` & `microservices_common-0.0.9/src/microservices_common/middlewares/authorized.py`

 * *Files identical despite different names*

### Comparing `microservices_common-0.0.8/src/microservices_common/middlewares/exception_handler.py` & `microservices_common-0.0.9/src/microservices_common/middlewares/exception_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from exceptions import CustomException
-from util.util import Util
+from microservices_common.exceptions import CustomException
+from microservices_common.util.util import Util
 from werkzeug.exceptions import HTTPException
 
 
 def handle_exception(e):
     print('in handle_exception')
     print(e)
     if isinstance(e, CustomException):
```

### Comparing `microservices_common-0.0.8/src/microservices_common/util/util.py` & `microservices_common-0.0.9/src/microservices_common/util/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,15 +700,15 @@
 
     @classmethod
     def log(cls, msg):
         print('{} {}'.format(datetime.now(), msg))
 
     @classmethod
     def get_owner_from_auth(cls, auth_info):
-        from exceptions import OwnerNotFound
+        from microservices_common.exceptions import OwnerNotFound
 
         owner = auth_info.get('user', dict()).get('company_id', None)
         if not owner:
             raise OwnerNotFound()
         return owner
 
     @classmethod
```

### Comparing `microservices_common-0.0.8/src/microservices_common.egg-info/SOURCES.txt` & `microservices_common-0.0.9/src/microservices_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

