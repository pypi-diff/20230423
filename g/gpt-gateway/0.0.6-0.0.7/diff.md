# Comparing `tmp/gpt_gateway-0.0.6.tar.gz` & `tmp/gpt_gateway-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_gateway-0.0.6.tar", last modified: Sat Apr 22 01:45:14 2023, max compression
+gzip compressed data, was "gpt_gateway-0.0.7.tar", last modified: Sat Apr 22 23:40:50 2023, max compression
```

## Comparing `gpt_gateway-0.0.6.tar` & `gpt_gateway-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 01:45:14.016191 gpt_gateway-0.0.6/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 gpt_gateway-0.0.6/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-22 01:45:14.015936 gpt_gateway-0.0.6/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 01:45:14.010753 gpt_gateway-0.0.6/gpt_gateway/
--rw-r--r--   0 wsk        (501) staff       (20)       31 2023-04-10 15:45:11.000000 gpt_gateway-0.0.6/gpt_gateway/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1755 2023-04-10 20:46:51.000000 gpt_gateway-0.0.6/gpt_gateway/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     4208 2023-04-10 16:15:23.000000 gpt_gateway-0.0.6/gpt_gateway/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 gpt_gateway-0.0.6/gpt_gateway/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4424 2023-04-10 20:54:56.000000 gpt_gateway-0.0.6/gpt_gateway/gptg_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 gpt_gateway-0.0.6/gpt_gateway/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 01:45:14.015349 gpt_gateway-0.0.6/gpt_gateway/models/
--rw-r--r--   0 wsk        (501) staff       (20)      202 2023-04-10 15:26:57.000000 gpt_gateway-0.0.6/gpt_gateway/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 gpt_gateway-0.0.6/gpt_gateway/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)      129 2023-04-10 04:46:49.000000 gpt_gateway-0.0.6/gpt_gateway/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 gpt_gateway-0.0.6/gpt_gateway/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 gpt_gateway-0.0.6/gpt_gateway/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      385 2023-04-10 04:51:43.000000 gpt_gateway-0.0.6/gpt_gateway/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 gpt_gateway-0.0.6/gpt_gateway/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)    12396 2023-04-22 01:27:18.000000 gpt_gateway-0.0.6/gpt_gateway/models/models.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 gpt_gateway-0.0.6/gpt_gateway/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 gpt_gateway-0.0.6/gpt_gateway/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     1170 2023-04-22 01:44:51.000000 gpt_gateway-0.0.6/gpt_gateway/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 gpt_gateway-0.0.6/gpt_gateway/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 gpt_gateway-0.0.6/gpt_gateway/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     2415 2023-04-10 20:55:35.000000 gpt_gateway-0.0.6/gpt_gateway/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 01:45:14.012002 gpt_gateway-0.0.6/gpt_gateway.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-22 01:45:14.000000 gpt_gateway-0.0.6/gpt_gateway.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      757 2023-04-22 01:45:14.000000 gpt_gateway-0.0.6/gpt_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-22 01:45:14.000000 gpt_gateway-0.0.6/gpt_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-22 01:45:14.000000 gpt_gateway-0.0.6/gpt_gateway.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       12 2023-04-22 01:45:14.000000 gpt_gateway-0.0.6/gpt_gateway.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      691 2023-04-22 01:44:57.000000 gpt_gateway-0.0.6/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-22 01:45:14.016269 gpt_gateway-0.0.6/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 01:45:14.015615 gpt_gateway-0.0.6/test/
--rw-r--r--   0 wsk        (501) staff       (20)      795 2023-04-10 16:22:01.000000 gpt_gateway-0.0.6/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 23:40:50.246313 gpt_gateway-0.0.7/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 gpt_gateway-0.0.7/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-22 23:40:50.245876 gpt_gateway-0.0.7/PKG-INFO
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 23:40:50.238994 gpt_gateway-0.0.7/gpt_gateway/
+-rw-r--r--   0 wsk        (501) staff       (20)       31 2023-04-10 15:45:11.000000 gpt_gateway-0.0.7/gpt_gateway/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1755 2023-04-10 20:46:51.000000 gpt_gateway-0.0.7/gpt_gateway/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4208 2023-04-10 16:15:23.000000 gpt_gateway-0.0.7/gpt_gateway/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 gpt_gateway-0.0.7/gpt_gateway/config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4424 2023-04-10 20:54:56.000000 gpt_gateway-0.0.7/gpt_gateway/gptg_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 gpt_gateway-0.0.7/gpt_gateway/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 23:40:50.244850 gpt_gateway-0.0.7/gpt_gateway/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      202 2023-04-10 15:26:57.000000 gpt_gateway-0.0.7/gpt_gateway/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 gpt_gateway-0.0.7/gpt_gateway/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)      129 2023-04-10 04:46:49.000000 gpt_gateway-0.0.7/gpt_gateway/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 gpt_gateway-0.0.7/gpt_gateway/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 gpt_gateway-0.0.7/gpt_gateway/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      385 2023-04-10 04:51:43.000000 gpt_gateway-0.0.7/gpt_gateway/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 gpt_gateway-0.0.7/gpt_gateway/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12396 2023-04-22 01:27:18.000000 gpt_gateway-0.0.7/gpt_gateway/models/models.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 gpt_gateway-0.0.7/gpt_gateway/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 gpt_gateway-0.0.7/gpt_gateway/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:36:38.000000 gpt_gateway-0.0.7/gpt_gateway/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 gpt_gateway-0.0.7/gpt_gateway/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 gpt_gateway-0.0.7/gpt_gateway/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2415 2023-04-10 20:55:35.000000 gpt_gateway-0.0.7/gpt_gateway/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 23:40:50.240368 gpt_gateway-0.0.7/gpt_gateway.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-22 23:40:50.000000 gpt_gateway-0.0.7/gpt_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      757 2023-04-22 23:40:50.000000 gpt_gateway-0.0.7/gpt_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-22 23:40:50.000000 gpt_gateway-0.0.7/gpt_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-22 23:40:50.000000 gpt_gateway-0.0.7/gpt_gateway.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       12 2023-04-22 23:40:50.000000 gpt_gateway-0.0.7/gpt_gateway.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      691 2023-04-22 23:39:34.000000 gpt_gateway-0.0.7/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-22 23:40:50.246417 gpt_gateway-0.0.7/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-22 23:40:50.245251 gpt_gateway-0.0.7/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      795 2023-04-10 16:22:01.000000 gpt_gateway-0.0.7/test/test.py
```

### Comparing `gpt_gateway-0.0.6/LICENSE` & `gpt_gateway-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/PKG-INFO` & `gpt_gateway-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_gateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client for GPT-Gateway.com including ChatGPT Retreiver Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/gpt-gateway-client
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/gpt-gateway-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt_gateway-0.0.6/gpt_gateway/client.py` & `gpt_gateway-0.0.7/gpt_gateway/client.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/collection.py` & `gpt_gateway-0.0.7/gpt_gateway/collection.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/config.py` & `gpt_gateway-0.0.7/gpt_gateway/config.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/gptg_session.py` & `gpt_gateway-0.0.7/gpt_gateway/gptg_session.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/login.py` & `gpt_gateway-0.0.7/gpt_gateway/login.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/auth.py` & `gpt_gateway-0.0.7/gpt_gateway/models/auth.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/chunk.py` & `gpt_gateway-0.0.7/gpt_gateway/models/chunk.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/collection.py` & `gpt_gateway-0.0.7/gpt_gateway/models/collection.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/metadata.py` & `gpt_gateway-0.0.7/gpt_gateway/models/metadata.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/models.py` & `gpt_gateway-0.0.7/gpt_gateway/models/models.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/org.py` & `gpt_gateway-0.0.7/gpt_gateway/models/org.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/plugin.py` & `gpt_gateway-0.0.7/gpt_gateway/models/plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/providers.py` & `gpt_gateway-0.0.7/gpt_gateway/models/providers.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/models/user.py` & `gpt_gateway-0.0.7/gpt_gateway/models/user.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway/org.py` & `gpt_gateway-0.0.7/gpt_gateway/org.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/gpt_gateway.egg-info/PKG-INFO` & `gpt_gateway-0.0.7/gpt_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-gateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client for GPT-Gateway.com including ChatGPT Retreiver Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/gpt-gateway-client
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/gpt-gateway-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt_gateway-0.0.6/gpt_gateway.egg-info/SOURCES.txt` & `gpt_gateway-0.0.7/gpt_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.6/pyproject.toml` & `gpt_gateway-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt_gateway"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
 description = "Client for GPT-Gateway.com including ChatGPT Retreiver Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `gpt_gateway-0.0.6/test/test.py` & `gpt_gateway-0.0.7/test/test.py`

 * *Files identical despite different names*

