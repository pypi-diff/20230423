# Comparing `tmp/ovinc_client-0.0.1.tar.gz` & `tmp/ovinc_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovinc_client-0.0.1.tar", last modified: Fri Apr 21 11:06:00 2023, max compression
+gzip compressed data, was "ovinc_client-0.0.2.tar", last modified: Sun Apr 23 15:49:34 2023, max compression
```

## Comparing `ovinc_client-0.0.1.tar` & `ovinc_client-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 11:06:00.216057 ovinc_client-0.0.1/
--rw-r--r--   0 orenzhang   (501) staff       (20)     1065 2023-04-21 10:04:38.000000 ovinc_client-0.0.1/LICENSE
--rw-r--r--   0 orenzhang   (501) staff       (20)      361 2023-04-21 11:06:00.215948 ovinc_client-0.0.1/PKG-INFO
--rw-r--r--   0 orenzhang   (501) staff       (20)      128 2023-04-21 11:03:45.000000 ovinc_client-0.0.1/README.md
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 11:06:00.214700 ovinc_client-0.0.1/ovinc_client/
--rw-r--r--   0 orenzhang   (501) staff       (20)       71 2023-04-21 10:03:03.000000 ovinc_client-0.0.1/ovinc_client/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2198 2023-04-21 11:01:25.000000 ovinc_client-0.0.1/ovinc_client/client.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 11:06:00.215787 ovinc_client-0.0.1/ovinc_client/components/
--rw-r--r--   0 orenzhang   (501) staff       (20)       72 2023-04-21 10:38:52.000000 ovinc_client-0.0.1/ovinc_client/components/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      722 2023-04-21 11:05:37.000000 ovinc_client-0.0.1/ovinc_client/components/base.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      769 2023-04-21 11:05:37.000000 ovinc_client-0.0.1/ovinc_client/components/notice.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      485 2023-04-21 11:02:37.000000 ovinc_client-0.0.1/ovinc_client/constants.py
--rw-r--r--   0 orenzhang   (501) staff       (20)       50 2023-04-21 10:25:11.000000 ovinc_client-0.0.1/ovinc_client/logger.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 11:06:00.215422 ovinc_client-0.0.1/ovinc_client.egg-info/
--rw-r--r--   0 orenzhang   (501) staff       (20)      361 2023-04-21 11:06:00.000000 ovinc_client-0.0.1/ovinc_client.egg-info/PKG-INFO
--rw-r--r--   0 orenzhang   (501) staff       (20)      404 2023-04-21 11:06:00.000000 ovinc_client-0.0.1/ovinc_client.egg-info/SOURCES.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)        1 2023-04-21 11:06:00.000000 ovinc_client-0.0.1/ovinc_client.egg-info/dependency_links.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)       17 2023-04-21 11:06:00.000000 ovinc_client-0.0.1/ovinc_client.egg-info/requires.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)       13 2023-04-21 11:06:00.000000 ovinc_client-0.0.1/ovinc_client.egg-info/top_level.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)       38 2023-04-21 11:06:00.216099 ovinc_client-0.0.1/setup.cfg
--rw-r--r--   0 orenzhang   (501) staff       (20)      532 2023-04-21 11:01:47.000000 ovinc_client-0.0.1/setup.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-23 15:49:34.098806 ovinc_client-0.0.2/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1065 2023-04-21 10:04:38.000000 ovinc_client-0.0.2/LICENSE
+-rw-r--r--   0 orenzhang   (501) staff       (20)      361 2023-04-23 15:49:34.098680 ovinc_client-0.0.2/PKG-INFO
+-rw-r--r--   0 orenzhang   (501) staff       (20)      128 2023-04-21 11:03:45.000000 ovinc_client-0.0.2/README.md
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-23 15:49:34.097509 ovinc_client-0.0.2/ovinc_client/
+-rw-r--r--   0 orenzhang   (501) staff       (20)       71 2023-04-21 10:03:03.000000 ovinc_client-0.0.2/ovinc_client/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2204 2023-04-23 15:47:55.000000 ovinc_client-0.0.2/ovinc_client/client.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-23 15:49:34.098489 ovinc_client-0.0.2/ovinc_client/components/
+-rw-r--r--   0 orenzhang   (501) staff       (20)       72 2023-04-21 10:38:52.000000 ovinc_client-0.0.2/ovinc_client/components/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      722 2023-04-21 11:05:37.000000 ovinc_client-0.0.2/ovinc_client/components/base.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      769 2023-04-21 11:05:37.000000 ovinc_client-0.0.2/ovinc_client/components/notice.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      485 2023-04-21 11:02:37.000000 ovinc_client-0.0.2/ovinc_client/constants.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)       50 2023-04-21 10:25:11.000000 ovinc_client-0.0.2/ovinc_client/logger.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-23 15:49:34.098126 ovinc_client-0.0.2/ovinc_client.egg-info/
+-rw-r--r--   0 orenzhang   (501) staff       (20)      361 2023-04-23 15:49:34.000000 ovinc_client-0.0.2/ovinc_client.egg-info/PKG-INFO
+-rw-r--r--   0 orenzhang   (501) staff       (20)      404 2023-04-23 15:49:34.000000 ovinc_client-0.0.2/ovinc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)        1 2023-04-23 15:49:34.000000 ovinc_client-0.0.2/ovinc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)       17 2023-04-23 15:49:34.000000 ovinc_client-0.0.2/ovinc_client.egg-info/requires.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)       13 2023-04-23 15:49:34.000000 ovinc_client-0.0.2/ovinc_client.egg-info/top_level.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)       38 2023-04-23 15:49:34.098855 ovinc_client-0.0.2/setup.cfg
+-rw-r--r--   0 orenzhang   (501) staff       (20)      532 2023-04-23 15:49:28.000000 ovinc_client-0.0.2/setup.py
```

### Comparing `ovinc_client-0.0.1/LICENSE` & `ovinc_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.0.1/ovinc_client/client.py` & `ovinc_client-0.0.2/ovinc_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def call_api(self, method: str, url: str, params: dict) -> ResponseData:
         """
         call union api
         """
 
         # init kwargs
-        kwargs = {"headers": self._build_headers(), "verify": strtobool(os.getenv("OVINC_API_VERIFY", "True"))}
+        kwargs = {"headers": self._build_headers(), "verify": bool(strtobool(os.getenv("OVINC_API_VERIFY", "True")))}
         if method == RequestMethodEnum.GET.value:
             kwargs["params"] = params
         else:
             kwargs["json"] = params
 
         # request
         response = requests.request(method=method, url=url, **kwargs)
```

### Comparing `ovinc_client-0.0.1/ovinc_client/components/base.py` & `ovinc_client-0.0.2/ovinc_client/components/base.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.0.1/ovinc_client/components/notice.py` & `ovinc_client-0.0.2/ovinc_client/components/notice.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.0.1/setup.py` & `ovinc_client-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ovinc_client",
-    version="0.0.1",
+    version="0.0.2",
     author="OVINC",
     url="https://www.ovinc.cn/",
     author_email="contact@ovinc.cn",
     description="A Tool for OVINC Union API",
     packages=["ovinc_client", "ovinc_client.components"],
     install_requires=[
-        "requests==2.27.1",
+        "requests>=2.27.1",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

