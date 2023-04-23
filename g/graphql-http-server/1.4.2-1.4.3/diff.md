# Comparing `tmp/graphql_http_server-1.4.2.tar.gz` & `tmp/graphql_http_server-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.2.tar", last modified: Sun Apr 23 07:46:43 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.3.tar", last modified: Sun Apr 23 08:31:36 2023, max compression
```

## Comparing `graphql_http_server-1.4.2.tar` & `graphql_http_server-1.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:46:43.147969 graphql_http_server-1.4.2/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 07:46:43.147969 graphql_http_server-1.4.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-23 07:46:42.000000 graphql_http_server-1.4.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:46:43.145222 graphql_http_server-1.4.2/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:46:43.146138 graphql_http_server-1.4.2/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9135 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:46:43.146138 graphql_http_server-1.4.2/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 07:46:43.000000 graphql_http_server-1.4.2/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-23 07:46:43.000000 graphql_http_server-1.4.2/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 07:46:43.000000 graphql_http_server-1.4.2/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-23 07:46:43.000000 graphql_http_server-1.4.2/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-23 07:46:43.000000 graphql_http_server-1.4.2/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-23 07:46:43.149801 graphql_http_server-1.4.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:46:43.147969 graphql_http_server-1.4.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     1984 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-23 07:46:33.000000 graphql_http_server-1.4.2/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-23 08:31:35.000000 graphql_http_server-1.4.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.556429 graphql_http_server-1.4.3/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.558430 graphql_http_server-1.4.3/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9295 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.557429 graphql_http_server-1.4.3/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-23 08:31:36.560430 graphql_http_server-1.4.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2246 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.2/LICENSE` & `graphql_http_server-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/PKG-INFO` & `graphql_http_server-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.4.2
+Version: 1.4.3
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.2.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.3.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.2/graphql_http_server/error.py` & `graphql_http_server-1.4.3/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.3/graphql_http_server/graphiql/index.html`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/graphql_http_server/helpers.py` & `graphql_http_server-1.4.3/graphql_http_server/helpers.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/graphql_http_server/server.py` & `graphql_http_server-1.4.3/graphql_http_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,19 @@
 
         elif content_type in (
                 'application/x-www-form-urlencoded',
                 'multipart/form-data'
         ):
             return request.form
 
+        if request.data:
+            try:
+                return load_json_body(request.data.decode('utf8'))
+            except Exception:
+                pass
         return {}
 
     def should_serve_graphiql(self, request):
         if not self.serve_graphiql or 'raw' in request.args:
             return False
 
         return self.request_wants_html(request=request)
```

### Comparing `graphql_http_server-1.4.2/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.3/graphql_http_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.4.2
+Version: 1.4.3
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.2.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.3.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.2/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.3/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/setup.py` & `graphql_http_server-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.2/tests/test_app.py` & `graphql_http_server-1.4.3/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,21 @@
     def test_app(self, schema):
         server = GraphQLHTTPServer(schema=schema)
         response = server.client().get('/?query={hello}')
 
         assert response.status_code == 200
         assert response.data == b'{"data":{"hello":"world"}}'
 
+    def test_app_post(self, schema):
+        server = GraphQLHTTPServer(schema=schema)
+        response = server.client().post(data='{"query":"{hello}"}')
+
+        assert response.status_code == 200
+        assert response.data == b'{"data":{"hello":"world"}}'
+
     def test_health_endpoint(self, schema):
         server = GraphQLHTTPServer(schema=schema, health_path="/health")
         response = server.client().get('/health')
 
         assert response.status_code == 200
         assert response.data == b'OK'
```

### Comparing `graphql_http_server-1.4.2/tests/test_graphql_api.py` & `graphql_http_server-1.4.3/tests/test_graphql_api.py`

 * *Files identical despite different names*

