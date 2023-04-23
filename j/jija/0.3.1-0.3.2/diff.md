# Comparing `tmp/jija-0.3.1.tar.gz` & `tmp/jija-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jija-0.3.1.tar", last modified: Sat Apr 22 11:43:09 2023, max compression
+gzip compressed data, was "jija-0.3.2.tar", last modified: Sun Apr 23 18:07:39 2023, max compression
```

## Comparing `jija-0.3.1.tar` & `jija-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-22 11:43:09.187370 jija-0.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/
--rwxr-xr-x   0 root         (0) root         (0)      308 2023-04-20 16:55:27.000000 jija-0.3.1/jija/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6316 2023-04-22 10:21:56.000000 jija-0.3.1/jija/app.py
--rwxr-xr-x   0 root         (0) root         (0)     4247 2023-04-20 22:18:05.000000 jija-0.3.1/jija/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/base_app/
--rwxr-xr-x   0 root         (0) root         (0)      198 2023-04-20 21:51:13.000000 jija-0.3.1/jija/base_app/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/base_app/commands/
--rwxr-xr-x   0 root         (0) root         (0)      165 2023-04-20 15:29:36.000000 jija-0.3.1/jija/base_app/commands/migrate.py
--rwxr-xr-x   0 root         (0) root         (0)     1366 2023-04-18 13:14:24.000000 jija-0.3.1/jija/base_app/commands/run.py
--rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.3.1/jija/base_app/commands/runprocess.py
--rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:30:36.000000 jija-0.3.1/jija/base_app/commands/update.py
--rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.3.1/jija/base_app/middlewares.py
--rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-20 22:16:18.000000 jija-0.3.1/jija/collector.py
--rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.3.1/jija/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/config/
--rwxr-xr-x   0 root         (0) root         (0)      136 2023-04-20 15:42:10.000000 jija-0.3.1/jija/config/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.3.1/jija/config/base.py
--rwxr-xr-x   0 root         (0) root         (0)      685 2023-04-20 10:04:29.000000 jija-0.3.1/jija/config/dev.py
--rwxr-xr-x   0 root         (0) root         (0)      928 2023-04-20 15:19:31.000000 jija-0.3.1/jija/config/drivers.py
--rwxr-xr-x   0 root         (0) root         (0)      290 2023-04-20 13:46:57.000000 jija-0.3.1/jija/config/network.py
--rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-20 13:50:19.000000 jija-0.3.1/jija/config/structute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/auth/
--rwxr-xr-x   0 root         (0) root         (0)      488 2023-04-20 13:48:49.000000 jija-0.3.1/jija/contrib/auth/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/jija_orm/
--rwxr-xr-x   0 root         (0) root         (0)     2238 2023-04-22 11:38:34.000000 jija-0.3.1/jija/contrib/jija_orm/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/swagger/
--rwxr-xr-x   0 root         (0) root         (0)     1481 2023-04-20 14:28:01.000000 jija-0.3.1/jija/contrib/swagger/driver.py
--rwxr-xr-x   0 root         (0) root         (0)     4723 2023-04-20 14:10:00.000000 jija-0.3.1/jija/contrib/swagger/processor.py
--rwxr-xr-x   0 root         (0) root         (0)      234 2023-04-20 14:05:10.000000 jija-0.3.1/jija/contrib/swagger/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/drivers/
--rwxr-xr-x   0 root         (0) root         (0)       90 2023-04-20 14:55:05.000000 jija-0.3.1/jija/drivers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:18:55.000000 jija-0.3.1/jija/drivers/base.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-04-20 15:29:36.000000 jija-0.3.1/jija/drivers/database.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2023-04-20 14:28:01.000000 jija-0.3.1/jija/drivers/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.3.1/jija/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.3.1/jija/middleware.py
--rwxr-xr-x   0 root         (0) root         (0)     1829 2023-04-20 10:04:29.000000 jija-0.3.1/jija/reloader.py
--rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.3.1/jija/response.py
--rwxr-xr-x   0 root         (0) root         (0)     2281 2023-04-20 21:45:15.000000 jija-0.3.1/jija/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/serializers/
--rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.3.1/jija/serializers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.3.1/jija/serializers/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)     3305 2023-04-20 13:50:19.000000 jija-0.3.1/jija/serializers/fields.py
--rwxr-xr-x   0 root         (0) root         (0)     1283 2023-04-20 11:10:56.000000 jija-0.3.1/jija/serializers/serializer.py
--rwxr-xr-x   0 root         (0) root         (0)     3220 2023-04-20 13:50:19.000000 jija-0.3.1/jija/serializers/validators.py
--rwxr-xr-x   0 root         (0) root         (0)     6044 2023-04-20 14:13:13.000000 jija-0.3.1/jija/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 11:43:09.187370 jija-0.3.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      718 2023-04-22 11:43:07.000000 jija-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-23 18:07:39.012263 jija-0.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/
+-rwxr-xr-x   0 root         (0) root         (0)      308 2023-04-20 16:55:27.000000 jija-0.3.2/jija/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6316 2023-04-22 10:21:56.000000 jija-0.3.2/jija/app.py
+-rwxr-xr-x   0 root         (0) root         (0)     4247 2023-04-20 22:18:05.000000 jija-0.3.2/jija/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/base_app/
+-rwxr-xr-x   0 root         (0) root         (0)      198 2023-04-20 21:51:13.000000 jija-0.3.2/jija/base_app/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/base_app/commands/
+-rwxr-xr-x   0 root         (0) root         (0)      165 2023-04-20 15:29:36.000000 jija-0.3.2/jija/base_app/commands/migrate.py
+-rwxr-xr-x   0 root         (0) root         (0)     1366 2023-04-18 13:14:24.000000 jija-0.3.2/jija/base_app/commands/run.py
+-rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.3.2/jija/base_app/commands/runprocess.py
+-rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:30:36.000000 jija-0.3.2/jija/base_app/commands/update.py
+-rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.3.2/jija/base_app/middlewares.py
+-rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-20 22:16:18.000000 jija-0.3.2/jija/collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.3.2/jija/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/config/
+-rwxr-xr-x   0 root         (0) root         (0)      136 2023-04-20 15:42:10.000000 jija-0.3.2/jija/config/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.3.2/jija/config/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      685 2023-04-20 10:04:29.000000 jija-0.3.2/jija/config/dev.py
+-rwxr-xr-x   0 root         (0) root         (0)      928 2023-04-23 10:06:57.000000 jija-0.3.2/jija/config/drivers.py
+-rwxr-xr-x   0 root         (0) root         (0)      290 2023-04-20 13:46:57.000000 jija-0.3.2/jija/config/network.py
+-rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-20 13:50:19.000000 jija-0.3.2/jija/config/structute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/contrib/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      592 2023-04-23 18:05:18.000000 jija-0.3.2/jija/contrib/auth/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/contrib/jija_orm/
+-rwxr-xr-x   0 root         (0) root         (0)     2238 2023-04-22 11:38:34.000000 jija-0.3.2/jija/contrib/jija_orm/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/contrib/swagger/
+-rwxr-xr-x   0 root         (0) root         (0)     1481 2023-04-20 14:28:01.000000 jija-0.3.2/jija/contrib/swagger/driver.py
+-rwxr-xr-x   0 root         (0) root         (0)     4723 2023-04-20 14:10:00.000000 jija-0.3.2/jija/contrib/swagger/processor.py
+-rwxr-xr-x   0 root         (0) root         (0)      234 2023-04-20 14:05:10.000000 jija-0.3.2/jija/contrib/swagger/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/drivers/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-04-20 14:55:05.000000 jija-0.3.2/jija/drivers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:18:55.000000 jija-0.3.2/jija/drivers/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-04-20 15:29:36.000000 jija-0.3.2/jija/drivers/database.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2023-04-20 14:28:01.000000 jija-0.3.2/jija/drivers/docs.py
+-rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.3.2/jija/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.3.2/jija/middleware.py
+-rwxr-xr-x   0 root         (0) root         (0)     1829 2023-04-20 10:04:29.000000 jija-0.3.2/jija/reloader.py
+-rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.3.2/jija/response.py
+-rwxr-xr-x   0 root         (0) root         (0)     2281 2023-04-20 21:45:15.000000 jija-0.3.2/jija/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija/serializers/
+-rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.3.2/jija/serializers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.3.2/jija/serializers/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     3305 2023-04-20 13:50:19.000000 jija-0.3.2/jija/serializers/fields.py
+-rwxr-xr-x   0 root         (0) root         (0)     1470 2023-04-23 18:05:18.000000 jija-0.3.2/jija/serializers/serializer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3220 2023-04-20 13:50:19.000000 jija-0.3.2/jija/serializers/validators.py
+-rwxr-xr-x   0 root         (0) root         (0)     6044 2023-04-20 14:13:13.000000 jija-0.3.2/jija/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:07:39.012263 jija-0.3.2/jija.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-23 18:07:39.000000 jija-0.3.2/jija.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 18:07:39.012263 jija-0.3.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      718 2023-04-23 18:05:44.000000 jija-0.3.2/setup.py
```

### Comparing `jija-0.3.1/jija/app.py` & `jija-0.3.2/jija/app.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/apps.py` & `jija-0.3.2/jija/apps.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/base_app/commands/run.py` & `jija-0.3.2/jija/base_app/commands/run.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/base_app/middlewares.py` & `jija-0.3.2/jija/base_app/middlewares.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/collector.py` & `jija-0.3.2/jija/collector.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/config/base.py` & `jija-0.3.2/jija/config/base.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/config/dev.py` & `jija-0.3.2/jija/config/dev.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/config/drivers.py` & `jija-0.3.2/jija/config/drivers.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/config/structute.py` & `jija-0.3.2/jija/config/structute.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/contrib/jija_orm/driver.py` & `jija-0.3.2/jija/contrib/jija_orm/driver.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/contrib/swagger/driver.py` & `jija-0.3.2/jija/contrib/swagger/driver.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/contrib/swagger/processor.py` & `jija-0.3.2/jija/contrib/swagger/processor.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/reloader.py` & `jija-0.3.2/jija/reloader.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/response.py` & `jija-0.3.2/jija/response.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/router.py` & `jija-0.3.2/jija/router.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/serializers/fields.py` & `jija-0.3.2/jija/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/serializers/serializer.py` & `jija-0.3.2/jija/serializers/serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,22 @@
             try:
                 self.data[name] = await field.validate(self.data.get(name))
 
             except ValidationError as exception:
                 self.errors[name] = exception.error
                 self.data[name] = exception.value
 
-        if inspect.iscoroutinefunction(self.clean):
-            await self.clean()
-        else:
-            self.clean()
+        try:
+            if inspect.iscoroutinefunction(self.clean):
+                # noinspection PyUnresolvedReferences
+                await self.clean()
+            else:
+                self.clean()
+        except ValidationError as exception:
+            self.errors[exception.error] = exception.value
 
         self.__valid = len(self.errors) == 0
         if not self.__valid:
             print(self.errors)
 
         return self.__valid
```

### Comparing `jija-0.3.1/jija/serializers/validators.py` & `jija-0.3.2/jija/serializers/validators.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija/views.py` & `jija-0.3.2/jija/views.py`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/jija.egg-info/SOURCES.txt` & `jija-0.3.2/jija.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jija-0.3.1/setup.py` & `jija-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jija',
-    version='0.3.1',
+    version='0.3.2',
     description='Async framework for web development with graceful collector',
     url='https://gitlab.com/by_dezz/jija/',
 
     packages=[
         'jija',
         'jija.base_app',
         'jija.base_app.commands',
```

