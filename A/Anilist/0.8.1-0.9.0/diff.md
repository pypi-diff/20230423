# Comparing `tmp/Anilist-0.8.1.tar.gz` & `tmp/Anilist-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.8.1.tar", last modified: Sat Apr 22 06:53:18 2023, max compression
+gzip compressed data, was "Anilist-0.9.0.tar", last modified: Sun Apr 23 02:43:09 2023, max compression
```

## Comparing `Anilist-0.8.1.tar` & `Anilist-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.385189 Anilist-0.8.1/
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.296584 Anilist-0.8.1/Anilist/
--rw-rw-rw-   0        0        0      164 2023-04-21 07:31:24.000000 Anilist-0.8.1/Anilist/__init__.py
--rw-rw-rw-   0        0        0     1072 2023-04-22 06:25:28.000000 Anilist-0.8.1/Anilist/anilist_types.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.344873 Anilist-0.8.1/Anilist/auth/
--rw-rw-rw-   0        0        0       22 2023-04-21 03:25:44.000000 Anilist-0.8.1/Anilist/auth/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.8.1/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0     1007 2023-04-22 06:50:55.000000 Anilist-0.8.1/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.8.1/Anilist/auth/token.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.352488 Anilist-0.8.1/Anilist/client/
--rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.8.1/Anilist/client/__init__.py
--rw-rw-rw-   0        0        0     2573 2023-04-22 06:07:42.000000 Anilist-0.8.1/Anilist/client/client.py
--rw-rw-rw-   0        0        0      477 2023-04-21 20:55:21.000000 Anilist-0.8.1/Anilist/client/mutation.py
--rw-rw-rw-   0        0        0      923 2023-04-22 03:59:01.000000 Anilist-0.8.1/Anilist/client/query.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.355485 Anilist-0.8.1/Anilist/errors/
--rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.8.1/Anilist/errors/__init__.py
--rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.8.1/Anilist/errors/request.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.360483 Anilist-0.8.1/Anilist/mutation/
--rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.8.1/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-22 06:24:47.000000 Anilist-0.8.1/Anilist/mutation/media_list.py
--rw-rw-rw-   0        0        0      393 2023-04-22 06:22:20.000000 Anilist-0.8.1/Anilist/mutation/mutable.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.367198 Anilist-0.8.1/Anilist/query/
--rw-rw-rw-   0        0        0       80 2023-04-22 01:33:28.000000 Anilist-0.8.1/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0      583 2023-04-22 06:50:02.000000 Anilist-0.8.1/Anilist/query/media_entry.py
--rw-rw-rw-   0        0        0      637 2023-04-22 06:49:55.000000 Anilist-0.8.1/Anilist/query/media_list.py
--rw-rw-rw-   0        0        0     3293 2023-04-22 06:49:45.000000 Anilist-0.8.1/Anilist/query/query.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.372195 Anilist-0.8.1/Anilist/scheme/
--rw-rw-rw-   0        0        0      112 2023-04-22 01:40:50.000000 Anilist-0.8.1/Anilist/scheme/__init__.py
--rw-rw-rw-   0        0        0      662 2023-04-22 01:52:21.000000 Anilist-0.8.1/Anilist/scheme/media_scheme.py
--rw-rw-rw-   0        0        0     2234 2023-04-21 20:53:49.000000 Anilist-0.8.1/Anilist/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.378193 Anilist-0.8.1/Anilist/utils/
--rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.8.1/Anilist/utils/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.8.1/Anilist/utils/consts.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.8.1/Anilist/utils/logging.py
--rw-rw-rw-   0        0        0      652 2023-04-21 20:02:38.000000 Anilist-0.8.1/Anilist/utils/object.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.380190 Anilist-0.8.1/Anilist/vars/
--rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.8.1/Anilist/vars/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-04-22 06:23:55.000000 Anilist-0.8.1/Anilist/vars/vars.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.338875 Anilist-0.8.1/Anilist.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-22 06:53:18.000000 Anilist-0.8.1/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      887 2023-04-22 06:53:18.000000 Anilist-0.8.1/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:53:18.000000 Anilist-0.8.1/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 06:53:18.000000 Anilist-0.8.1/Anilist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.8.1/LICENSE
--rw-rw-rw-   0        0        0      563 2023-04-22 06:53:18.384200 Anilist-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.8.1/README.md
--rw-rw-rw-   0        0        0      601 2023-04-22 06:52:15.000000 Anilist-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 06:53:18.386186 Anilist-0.8.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 06:53:18.383190 Anilist-0.8.1/tests/
--rw-rw-rw-   0        0        0     1454 2023-04-22 06:51:13.000000 Anilist-0.8.1/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.225318 Anilist-0.9.0/
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.061417 Anilist-0.9.0/Anilist/
+-rw-rw-rw-   0        0        0      188 2023-04-22 21:40:55.000000 Anilist-0.9.0/Anilist/__init__.py
+-rw-rw-rw-   0        0        0     1072 2023-04-22 06:25:28.000000 Anilist-0.9.0/Anilist/anilist_types.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.125378 Anilist-0.9.0/Anilist/auth/
+-rw-rw-rw-   0        0        0      749 2023-04-23 02:39:40.000000 Anilist-0.9.0/Anilist/auth/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-23 01:27:00.000000 Anilist-0.9.0/Anilist/auth/auth.py
+-rw-rw-rw-   0        0        0      993 2023-04-22 22:01:35.000000 Anilist-0.9.0/Anilist/auth/code.py
+-rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.9.0/Anilist/auth/token.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.140368 Anilist-0.9.0/Anilist/client/
+-rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.9.0/Anilist/client/__init__.py
+-rw-rw-rw-   0        0        0     2573 2023-04-22 22:13:50.000000 Anilist-0.9.0/Anilist/client/client.py
+-rw-rw-rw-   0        0        0      477 2023-04-21 20:55:21.000000 Anilist-0.9.0/Anilist/client/mutation.py
+-rw-rw-rw-   0        0        0     1072 2023-04-23 02:38:44.000000 Anilist-0.9.0/Anilist/client/query.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.143366 Anilist-0.9.0/Anilist/errors/
+-rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.9.0/Anilist/errors/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.9.0/Anilist/errors/request.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.167360 Anilist-0.9.0/Anilist/mutation/
+-rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.9.0/Anilist/mutation/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-22 06:24:47.000000 Anilist-0.9.0/Anilist/mutation/media_list.py
+-rw-rw-rw-   0        0        0      393 2023-04-22 06:22:20.000000 Anilist-0.9.0/Anilist/mutation/mutable.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.175346 Anilist-0.9.0/Anilist/query/
+-rw-rw-rw-   0        0        0      132 2023-04-22 21:50:16.000000 Anilist-0.9.0/Anilist/query/__init__.py
+-rw-rw-rw-   0        0        0      721 2023-04-23 02:37:43.000000 Anilist-0.9.0/Anilist/query/media_entry.py
+-rw-rw-rw-   0        0        0      769 2023-04-23 02:37:57.000000 Anilist-0.9.0/Anilist/query/media_list.py
+-rw-rw-rw-   0        0        0     6825 2023-04-23 02:36:40.000000 Anilist-0.9.0/Anilist/query/query.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.179345 Anilist-0.9.0/Anilist/scheme/
+-rw-rw-rw-   0        0        0      139 2023-04-22 22:02:36.000000 Anilist-0.9.0/Anilist/scheme/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-04-22 01:52:21.000000 Anilist-0.9.0/Anilist/scheme/media_scheme.py
+-rw-rw-rw-   0        0        0     4017 2023-04-23 02:11:42.000000 Anilist-0.9.0/Anilist/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.190338 Anilist-0.9.0/Anilist/utils/
+-rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.9.0/Anilist/utils/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.9.0/Anilist/utils/consts.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.9.0/Anilist/utils/logging.py
+-rw-rw-rw-   0        0        0     2933 2023-04-23 02:02:48.000000 Anilist-0.9.0/Anilist/utils/object.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.193336 Anilist-0.9.0/Anilist/vars/
+-rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.9.0/Anilist/vars/__init__.py
+-rw-rw-rw-   0        0        0     2070 2023-04-23 01:31:18.000000 Anilist-0.9.0/Anilist/vars/vars.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.094398 Anilist-0.9.0/Anilist.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 02:43:08.000000 Anilist-0.9.0/Anilist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-04-23 02:43:09.224318 Anilist-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.9.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-23 02:41:38.000000 Anilist-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 02:43:09.226316 Anilist-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 02:43:09.221320 Anilist-0.9.0/tests/
+-rw-rw-rw-   0        0        0     1334 2023-04-22 21:40:22.000000 Anilist-0.9.0/tests/test_externals.py
+-rw-rw-rw-   0        0        0      223 2023-04-22 21:39:23.000000 Anilist-0.9.0/tests/test_internals.py
```

### Comparing `Anilist-0.8.1/Anilist/anilist_types.py` & `Anilist-0.9.0/Anilist/anilist_types.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/Anilist/auth/code.py` & `Anilist-0.9.0/Anilist/auth/code.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 import webbrowser
 
 pat = re.compile(r'\?code=(.*?)(\&|\r| |\n)')
 
 def get_code(client_id):
     webbrowser.open(f"https://anilist.co/api/v2/oauth/authorize?client_id={client_id}&redirect_uri=http://127.0.0.1:8000/&response_type=code", autoraise=True)
     
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    s.bind(("127.0.0.1", 8000))
-    s.listen()
-    conn, addr = s.accept()
-    while True:
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        s.bind(("127.0.0.1", 8000))
+        s.listen()
+        conn, _ = s.accept()
+        code = None
         data = conn.recv(1024)
         if not data:
-            break
+            return code
         
         conn.send("HTTP/1.1 200 OK\n".encode())
         conn.send("Content-Type: text/html\n\n".encode())
         conn.send("\n".encode())
         conn.send("""
             <html>
                 <body>
                     <h1>Auth completed</h1>
                 </body>
             </html>
         """.encode())
         conn.close()
 
-        try:
-            code = pat.findall(data.decode('utf-8'))[0][0]
-            return code
-        except:
-            break
+        code = pat.findall(data.decode('utf-8'))[0][0]
+        
+    return code
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 import socket import re import webbrowser pat = re.compile(r'\?code=(.*?)
 (\&|\r| |\n)') def get_code(client_id): webbrowser.open(f"https://anilist.co/
 api/v2/oauth/authorize?client_id={client_id}&redirect_uri=http://127.0.0.1:
-8000/&response_type=code", autoraise=True) s = socket.socket(socket.AF_INET,
-socket.SOCK_STREAM) s.bind(("127.0.0.1", 8000)) s.listen() conn, addr =
-s.accept() while True: data = conn.recv(1024) if not data: break conn.send
-("HTTP/1.1 200 OK\n".encode()) conn.send("Content-Type: text/html\n\n".encode
-()) conn.send("\n".encode()) conn.send("""
+8000/&response_type=code", autoraise=True) with socket.socket(socket.AF_INET,
+socket.SOCK_STREAM) as s: s.bind(("127.0.0.1", 8000)) s.listen() conn, _ =
+s.accept() code = None data = conn.recv(1024) if not data: return code
+conn.send("HTTP/1.1 200 OK\n".encode()) conn.send("Content-Type: text/
+html\n\n".encode()) conn.send("\n".encode()) conn.send("""
 ****** Auth completed ******
-""".encode()) conn.close() try: code = pat.findall(data.decode('utf-8'))[0][0]
-return code except: break
+""".encode()) conn.close() code = pat.findall(data.decode('utf-8'))[0][0]
+return code
```

### Comparing `Anilist-0.8.1/Anilist/client/client.py` & `Anilist-0.9.0/Anilist/client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 break
 
             pg += 1
             vars.update("page", pg)
 
         return temp
 
-    def _request(self, query, vars: Vars):
+    def _request(self, query: str, vars: Vars):
 
         log = AnilistLogger()
         log.info(f"Sending request to URI {self.URI} with headers {self.headers}")
         log.debug(f"The query is {query}\n The variables are {vars}")
         
         req = requests.post(self.URI, json={
             "query": query,
@@ -51,16 +51,16 @@
 
         if "errors" in resp and resp["errors"] != []:
             raise RequestError.from_json(resp["errors"][0])
         
         obj = AnilistObject(resp["data"])
         return obj
         
-    def _create_query(self, vars, *schs, head_sch=None):
-        schs = list(schs) if head_sch is None else [Scheme._combine(head_sch, sch) for sch in schs]
+    def _create_query(self, vars, *schs: Scheme, head_sch: Scheme=None):
+        schs = list(schs) if head_sch is None else head_sch.sub_schemes(*schs)
         if vars._names == "":
             return """
             {} {{
                 {}
             }}
             """.format(self._query_type(), Scheme._construct(*schs))
         return """
```

### Comparing `Anilist-0.8.1/Anilist/errors/request.py` & `Anilist-0.9.0/Anilist/errors/request.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/Anilist/mutation/media_list.py` & `Anilist-0.9.0/Anilist/mutation/media_list.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/Anilist/scheme/media_scheme.py` & `Anilist-0.9.0/Anilist/scheme/media_scheme.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/Anilist/utils/logging.py` & `Anilist-0.9.0/Anilist/utils/logging.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/Anilist.egg-info/PKG-INFO` & `Anilist-0.9.0/Anilist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.8.1
+Version: 0.9.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.8.1/Anilist.egg-info/SOURCES.txt` & `Anilist-0.9.0/Anilist.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 Anilist/scheme/scheme.py
 Anilist/utils/__init__.py
 Anilist/utils/consts.py
 Anilist/utils/logging.py
 Anilist/utils/object.py
 Anilist/vars/__init__.py
 Anilist/vars/vars.py
-tests/test_base.py
+tests/test_externals.py
+tests/test_internals.py
```

### Comparing `Anilist-0.8.1/LICENSE` & `Anilist-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Anilist-0.8.1/PKG-INFO` & `Anilist-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.8.1
+Version: 0.9.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.8.1/pyproject.toml` & `Anilist-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Anilist"
-version = "0.8.1"
+version = "0.9.0"
 authors = [
   { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
 ]
 description = "Anilist API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

