# Comparing `tmp/swagroutes-0.0.6.tar.gz` & `tmp/swagroutes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagroutes-0.0.6.tar", last modified: Tue Apr 18 20:48:16 2023, max compression
+gzip compressed data, was "swagroutes-1.0.2.tar", last modified: Sun Apr 23 19:41:38 2023, max compression
```

## Comparing `swagroutes-0.0.6.tar` & `swagroutes-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:16.914215 swagroutes-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 20:48:05.000000 swagroutes-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-18 20:48:16.910215 swagroutes-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-18 20:48:05.000000 swagroutes-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:48:16.914215 swagroutes-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 20:48:05.000000 swagroutes-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:16.910215 swagroutes-0.0.6/swagroutes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:48:05.000000 swagroutes-0.0.6/swagroutes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 20:48:05.000000 swagroutes-0.0.6/swagroutes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 20:48:05.000000 swagroutes-0.0.6/swagroutes/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 20:48:05.000000 swagroutes-0.0.6/swagroutes/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:16.910215 swagroutes-0.0.6/swagroutes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 20:48:16.000000 swagroutes-0.0.6/swagroutes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:16.910215 swagroutes-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:48:05.000000 swagroutes-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 20:48:05.000000 swagroutes-0.0.6/tests/test_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 19:41:38.112159 swagroutes-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 19:41:24.000000 swagroutes-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-23 19:41:38.112159 swagroutes-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-23 19:41:24.000000 swagroutes-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 19:41:38.112159 swagroutes-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-23 19:41:24.000000 swagroutes-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 19:41:38.108159 swagroutes-1.0.2/swagroutes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 19:41:24.000000 swagroutes-1.0.2/swagroutes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 19:41:24.000000 swagroutes-1.0.2/swagroutes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-23 19:41:24.000000 swagroutes-1.0.2/swagroutes/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-23 19:41:24.000000 swagroutes-1.0.2/swagroutes/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 19:41:38.108159 swagroutes-1.0.2/swagroutes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 19:41:38.000000 swagroutes-1.0.2/swagroutes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 19:41:38.112159 swagroutes-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 19:41:24.000000 swagroutes-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-23 19:41:24.000000 swagroutes-1.0.2/tests/test_extractor.py
```

### Comparing `swagroutes-0.0.6/LICENSE` & `swagroutes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.6/PKG-INFO` & `swagroutes-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-Metadata-Version: 2.1
-Name: swagroutes
-Version: 0.0.6
-Summary: Command-line tool that extracts and lists API routes from Swagger files in YAML or JSON format.
-Home-page: https://github.com/amalmurali47/swagroutes
-Author: Amal Murali
-Author-email: amalmurali47@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # swagroutes
 
 swagroutes is a command-line tool that extracts and lists API routes from Swagger files in YAML or JSON format. It simplifies the process of fetching the routes provided by an API and supports processing multiple files or directories at once.
 
-![](https://user-images.githubusercontent.com/3582096/232892882-7755d610-a85a-4c21-8a35-543d24204d23.png)
+![](https://user-images.githubusercontent.com/3582096/233068257-29adfadd-8cd3-45fd-9d1d-f22a9772d139.png)
 
 ## Install
 
 ```bash
 pip install swagroutes
 ```
 
 ## Upgrade
 ```bash
 pip install -U swagroutes
 ```
 
+## Help
+```
+usage: swagroutes [-h] [-o OUTPUT] [-p] input [input ...]
+
+Extract routes from Swagger files.
+
+positional arguments:
+  input                 Input file(s) or directory containing Swagger files.
+
+options:
+  -h, --help            show this help message and exit
+  -o OUTPUT, --output OUTPUT
+                        Output file to store the results.
+  -p, --include-params  Include query parameters in the extracted routes.
+```
+
 ## Usage
 To use swagroutes, simply provide input files or directories containing Swagger files as arguments. The tool will process the files and print the extracted routes.
 
 #### Single YAML or JSON file
 ```bash
 swagroutes file.yaml
 ```
@@ -53,35 +55,69 @@
 ```
 
 #### Mix of files and directories
 ```bash
 swagroutes file1.yaml directory1/ file2.json directory2/
 ```
 
+#### Extract parameters
+```bash
+swagroutes file1.yaml --include-params
+```
+
 #### Output to a file
 Save the extracted routes to an output file using the `-o` or `--output` option:
 
 ```bash
 swagroutes file.yaml -o output.txt 
 ```
 
 
 ## Examples
-Given a Swagger file with the following content:
 
+**Input:**
 ```yaml
 basePath: /api
 paths:
   /users:
     get: {}
     post: {}
   /profile/{profile_id}:
     put: {}
 ```
 
-swagroutes will output:
+**Output:**
 
 ```
 GET /api/users
 POST /api/users
 PUT /api/profile/{profile_id}
 ```
+
+---
+
+**Input:**
+```yaml
+basePath: /api/v1
+paths:
+  /users:
+    get:
+      parameters:
+        - name: limit
+          in: query
+        - name: offset
+          in: query
+
+  /users/{userId}:
+    get:
+      parameters:
+        - name: userId
+          in: path
+          required: true
+          type: string
+```
+
+**Output:**
+```
+GET /api/v1/users/{userId}
+GET /api/v1/users?limit&offset
+```
```

### Comparing `swagroutes-0.0.6/setup.py` & `swagroutes-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.6/swagroutes/extractor.py` & `swagroutes-1.0.2/swagroutes/extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,39 +9,44 @@
 
 
 def load_json_file(file_path):
     with open(file_path, 'r') as file:
         return json.load(file)
 
 
-def extract_routes(swagger_data):
+def extract_routes(swagger_data, include_params=False):
     routes = set()
     base_path = swagger_data.get('basePath', '')
     paths = swagger_data.get('paths', {})
 
     http_methods = {'get', 'put', 'post', 'delete', 'options', 'head', 'patch', 'trace'}
 
     for path, methods in paths.items():
-        for method in methods.keys():
+        for method, details in methods.items():
             if method.lower() in http_methods:
                 route = f'{method.upper()} {base_path}{path}'
+                if include_params:
+                    parameters = details.get('parameters', [])
+                    query_params = [param['name'] for param in parameters if param['in'] == 'query']
+                    if query_params:
+                        route += '?' + '&'.join(query_params)
                 routes.add(route)
 
     return routes
 
 
-def process_swagger_files(files):
+def process_swagger_files(files, include_params=False):
     all_routes = set()
 
     for file in files:
         file_extension = file.suffix.lower()
         if file_extension == '.yaml':
             swagger_data = load_yaml_file(file)
         elif file_extension == '.json':
             swagger_data = load_json_file(file)
         else:
             continue
-        routes = extract_routes(swagger_data)
+        routes = extract_routes(swagger_data, include_params)
         all_routes.update(routes)
 
     return all_routes
```

### Comparing `swagroutes-0.0.6/swagroutes.egg-info/PKG-INFO` & `swagroutes-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagroutes
-Version: 0.0.6
+Version: 1.0.2
 Summary: Command-line tool that extracts and lists API routes from Swagger files in YAML or JSON format.
 Home-page: https://github.com/amalmurali47/swagroutes
 Author: Amal Murali
 Author-email: amalmurali47@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,27 +12,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # swagroutes
 
 swagroutes is a command-line tool that extracts and lists API routes from Swagger files in YAML or JSON format. It simplifies the process of fetching the routes provided by an API and supports processing multiple files or directories at once.
 
-![](https://user-images.githubusercontent.com/3582096/232892882-7755d610-a85a-4c21-8a35-543d24204d23.png)
+![](https://user-images.githubusercontent.com/3582096/233068257-29adfadd-8cd3-45fd-9d1d-f22a9772d139.png)
 
 ## Install
 
 ```bash
 pip install swagroutes
 ```
 
 ## Upgrade
 ```bash
 pip install -U swagroutes
 ```
 
+## Help
+```
+usage: swagroutes [-h] [-o OUTPUT] [-p] input [input ...]
+
+Extract routes from Swagger files.
+
+positional arguments:
+  input                 Input file(s) or directory containing Swagger files.
+
+options:
+  -h, --help            show this help message and exit
+  -o OUTPUT, --output OUTPUT
+                        Output file to store the results.
+  -p, --include-params  Include query parameters in the extracted routes.
+```
+
 ## Usage
 To use swagroutes, simply provide input files or directories containing Swagger files as arguments. The tool will process the files and print the extracted routes.
 
 #### Single YAML or JSON file
 ```bash
 swagroutes file.yaml
 ```
@@ -53,35 +69,69 @@
 ```
 
 #### Mix of files and directories
 ```bash
 swagroutes file1.yaml directory1/ file2.json directory2/
 ```
 
+#### Extract parameters
+```bash
+swagroutes file1.yaml --include-params
+```
+
 #### Output to a file
 Save the extracted routes to an output file using the `-o` or `--output` option:
 
 ```bash
 swagroutes file.yaml -o output.txt 
 ```
 
 
 ## Examples
-Given a Swagger file with the following content:
 
+**Input:**
 ```yaml
 basePath: /api
 paths:
   /users:
     get: {}
     post: {}
   /profile/{profile_id}:
     put: {}
 ```
 
-swagroutes will output:
+**Output:**
 
 ```
 GET /api/users
 POST /api/users
 PUT /api/profile/{profile_id}
 ```
+
+---
+
+**Input:**
+```yaml
+basePath: /api/v1
+paths:
+  /users:
+    get:
+      parameters:
+        - name: limit
+          in: query
+        - name: offset
+          in: query
+
+  /users/{userId}:
+    get:
+      parameters:
+        - name: userId
+          in: path
+          required: true
+          type: string
+```
+
+**Output:**
+```
+GET /api/v1/users/{userId}
+GET /api/v1/users?limit&offset
+```
```

