# Comparing `tmp/flexypy-0.0.6.tar.gz` & `tmp/flexypy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.6.tar", last modified: Sat Apr 22 20:39:49 2023, max compression
+gzip compressed data, was "flexypy-0.0.7.tar", last modified: Sun Apr 23 10:16:07 2023, max compression
```

## Comparing `flexypy-0.0.6.tar` & `flexypy-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.597180 flexypy-0.0.6/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-22 20:39:49.597180 flexypy-0.0.6/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.393177 flexypy-0.0.6/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.6/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.6/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.473178 flexypy-0.0.6/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.6/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.6/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.6/flexypy/exceptions/extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.6/flexypy/exceptions/render.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.6/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.6/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.481178 flexypy-0.0.6/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.6/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.6/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.6/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.501178 flexypy-0.0.6/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.6/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.6/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.521179 flexypy-0.0.6/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.6/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.545179 flexypy-0.0.6/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.6/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.6/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.6/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      197 2023-04-19 17:14:31.000000 flexypy-0.0.6/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.557179 flexypy-0.0.6/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.6/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.0.6/flexypy/http/cookie.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2401 2023-04-22 20:23:47.000000 flexypy-0.0.6/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.6/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     9611 2023-04-22 20:34:05.000000 flexypy-0.0.6/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.557179 flexypy-0.0.6/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.6/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.577180 flexypy-0.0.6/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.6/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.6/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.6/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.6/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.589180 flexypy-0.0.6/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.6/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.6/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 20:39:49.421177 flexypy-0.0.6/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-22 20:39:49.000000 flexypy-0.0.6/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-04-22 20:39:49.000000 flexypy-0.0.6/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-22 20:39:49.000000 flexypy-0.0.6/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-22 20:39:49.000000 flexypy-0.0.6/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-22 20:39:49.000000 flexypy-0.0.6/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-22 20:39:33.000000 flexypy-0.0.6/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-22 20:39:49.597180 flexypy-0.0.6/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.284161 flexypy-0.0.7/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-23 10:16:07.284161 flexypy-0.0.7/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.096160 flexypy-0.0.7/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.7/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.7/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.184160 flexypy-0.0.7/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.7/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.7/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.7/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.7/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.7/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.7/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.188160 flexypy-0.0.7/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.7/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.7/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.7/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.208160 flexypy-0.0.7/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.7/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.7/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.220161 flexypy-0.0.7/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.7/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.220161 flexypy-0.0.7/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.0.7/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.244161 flexypy-0.0.7/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.7/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.0.7/flexypy/http/cookie.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2431 2023-04-23 10:12:45.000000 flexypy-0.0.7/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.7/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     9611 2023-04-22 20:34:05.000000 flexypy-0.0.7/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.248161 flexypy-0.0.7/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.7/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.264161 flexypy-0.0.7/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.7/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.7/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.7/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.7/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.272161 flexypy-0.0.7/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.7/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.7/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.132160 flexypy-0.0.7/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-04-23 10:15:55.000000 flexypy-0.0.7/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-23 10:16:07.284161 flexypy-0.0.7/setup.cfg
```

### Comparing `flexypy-0.0.6/flexypy/exceptions/web/server.py` & `flexypy-0.0.7/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/generate_templates/generator.py` & `flexypy-0.0.7/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/cookie.py` & `flexypy-0.0.7/flexypy/http/cookie.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/request.py` & `flexypy-0.0.7/flexypy/http/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     @classmethod
     def set_cookie(cls, name, value, expires=None):
         c = cookies.SimpleCookie()
         c[name] = Cookie.encrypt_cookie(value).decode()
         c[name]['expires'] = (datetime.datetime.now() + datetime.timedelta(days=365)). \
             strftime('%a, %d-%b-%Y %H:%M:%S GMT')
         c[name]['secure'] = True
+        c[name]['path'] = '/'
         if expires:
             c[name]['expires'] = expires
         cls._set_cookie.update(c)
 
     @classmethod
     def set_server_cookie(cls, cookie):
         c = cookies.SimpleCookie()
```

### Comparing `flexypy-0.0.6/flexypy/http/routing.py` & `flexypy-0.0.7/flexypy/http/routing.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/server.py` & `flexypy-0.0.7/flexypy/http/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.0.7/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/template/extensions/template_ext.py` & `flexypy-0.0.7/flexypy/http/template/extensions/template_ext.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy/http/template/render.py` & `flexypy-0.0.7/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.6/flexypy.egg-info/SOURCES.txt` & `flexypy-0.0.7/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

