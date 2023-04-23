# Comparing `tmp/mitmproxy2swagger-0.8.2.tar.gz` & `tmp/mitmproxy2swagger-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitmproxy2swagger-0.8.2.tar", max compression
+gzip compressed data, was "mitmproxy2swagger-0.9.0.tar", max compression
```

## Comparing `mitmproxy2swagger-0.8.2.tar` & `mitmproxy2swagger-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     4616 2023-03-13 11:57:44.051414 mitmproxy2swagger-0.8.2/README.md
--rw-r--r--   0        0        0        0 2022-05-18 06:16:11.120503 mitmproxy2swagger-0.8.2/mitmproxy2swagger/__init__.py
--rw-r--r--   0        0        0     2136 2023-02-18 18:40:23.527597 mitmproxy2swagger-0.8.2/mitmproxy2swagger/console_util.py
--rw-r--r--   0        0        0     3426 2023-02-18 18:40:23.542334 mitmproxy2swagger-0.8.2/mitmproxy2swagger/har_capture_reader.py
--rwxr-xr-x   0        0        0    13687 2023-03-13 12:02:08.288130 mitmproxy2swagger-0.8.2/mitmproxy2swagger/mitmproxy2swagger.py
--rw-r--r--   0        0        0     2983 2023-02-18 18:40:23.541566 mitmproxy2swagger-0.8.2/mitmproxy2swagger/mitmproxy_capture_reader.py
--rw-r--r--   0        0        0     4070 2023-02-18 18:40:23.555728 mitmproxy2swagger-0.8.2/mitmproxy2swagger/swagger_util.py
--rw-r--r--   0        0        0      476 2023-03-13 12:04:07.294608 mitmproxy2swagger-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     5199 1970-01-01 00:00:00.000000 mitmproxy2swagger-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     5318 2023-04-22 17:35:43.219999 mitmproxy2swagger-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2022-05-18 06:16:11.120503 mitmproxy2swagger-0.9.0/mitmproxy2swagger/__init__.py
+-rw-r--r--   0        0        0     2160 2023-04-22 17:35:43.223831 mitmproxy2swagger-0.9.0/mitmproxy2swagger/console_util.py
+-rw-r--r--   0        0        0     3840 2023-04-22 17:35:43.223949 mitmproxy2swagger-0.9.0/mitmproxy2swagger/har_capture_reader.py
+-rw-r--r--   0        0        0    15534 2023-04-22 17:35:43.224222 mitmproxy2swagger-0.9.0/mitmproxy2swagger/mitmproxy2swagger.py
+-rw-r--r--   0        0        0     4263 2023-04-22 17:35:43.224338 mitmproxy2swagger-0.9.0/mitmproxy2swagger/mitmproxy_capture_reader.py
+-rw-r--r--   0        0        0     5003 2023-04-22 17:35:43.224446 mitmproxy2swagger-0.9.0/mitmproxy2swagger/swagger_util.py
+-rw-r--r--   0        0        0     1902 2023-04-22 17:35:43.224519 mitmproxy2swagger-0.9.0/mitmproxy2swagger/test_mitmproxy2swagger.py
+-rw-r--r--   0        0        0     1430 2023-04-22 17:35:43.224575 mitmproxy2swagger-0.9.0/mitmproxy2swagger/test_openapi_compliance.py
+-rw-r--r--   0        0        0     1759 2023-04-22 17:35:43.224626 mitmproxy2swagger-0.9.0/mitmproxy2swagger/testing_util.py
+-rw-r--r--   0        0        0     1029 2023-04-23 11:57:23.631338 mitmproxy2swagger-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5901 1970-01-01 00:00:00.000000 mitmproxy2swagger-0.9.0/PKG-INFO
```

### Comparing `mitmproxy2swagger-0.8.2/README.md` & `mitmproxy2swagger-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,130 @@
 # mitmproxy2swagger
 
-
 [![PyPI version](https://badge.fury.io/py/mitmproxy2swagger.svg)](https://badge.fury.io/py/mitmproxy2swagger)
 [![Arch Linux repository](https://img.shields.io/badge/archlinux-mitmproxy2swagger-blue)](https://archlinux.org/packages/community/any/mitmproxy2swagger/)
 
-
-https://user-images.githubusercontent.com/5400940/168086818-c48f60ab-3f95-42eb-b435-c8b1a6326b81.mp4
-
-
+<https://user-images.githubusercontent.com/5400940/168086818-c48f60ab-3f95-42eb-b435-c8b1a6326b81.mp4>
 
 A tool for automatically converting [mitmproxy](https://mitmproxy.org/) captures to [OpenAPI 3.0](https://swagger.io/specification/) specifications. This means that you can automatically reverse-engineer REST APIs by just running the apps and capturing the traffic.
 
 ---
+
 **🆕 NEW!**
 
 Added support for processing HAR exported from the browser DevTools. See [Usage - HAR](#har) for more details.
 
 ---
 
 ## Installation
 
 First you will need python3 and pip3.
 
 ```bash
-$ pip install mitmproxy2swagger 
+$ pip install mitmproxy2swagger
 # ... or ...
 $ pip3 install mitmproxy2swagger
+# ... or ...
+$ git clone git@github.com:alufers/mitmproxy2swagger.git
+$ cd mitmproxy2swagger
+$ docker build -t mitmproxy2swagger .
 ```
 
 Then clone the repo and run `mitmproxy2swagger` as per examples below.
 
 ## Usage
 
 ### Mitmproxy
 
 To create a specification by inspecting HTTP traffic you will need to:
 
 1. Capture the traffic by using the mitmproxy tool. I personally recommend using mitmweb, which is a web interface built-in to mitmproxy.
 
-    ```bash
-    $ mitmweb
-    Web server listening at http://127.0.0.1:8081/
-    Proxy server listening at http://*:9999
-    ...
-    ```
-    **IMPORTANT**
+   ```bash
+   $ mitmweb
+   Web server listening at http://127.0.0.1:8081/
+   Proxy server listening at http://*:9999
+   ...
+   ```
 
-    To configure your client to use the proxy exposed by mitm proxy, please consult the [mitmproxy documentation](https://docs.mitmproxy.org/stable/) for more information.
+   **IMPORTANT**
+
+   To configure your client to use the proxy exposed by mitm proxy, please consult the [mitmproxy documentation](https://docs.mitmproxy.org/stable/) for more information.
 
 2. Save the traffic to a flow file.
 
-    In mitmweb you can do this by using the "File" menu and selecting "Save":
-    
-    ![](./docs/mitmweb_save.png)
+   In mitmweb you can do this by using the "File" menu and selecting "Save":
+
+   ![A screenshot showing the location of the "Save" option in the "File" menu](./docs/mitmweb_save.png)
 
 3. Run the first pass of mitmproxy2swagger:
 
-    ```bash
-    $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
-    ```
+   ```bash
+   $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
+   # ... or ...
+   $ docker run -it -v $PWD:/app mitmproxy2swagger mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
+   ```
 
-    Please note that you can use an existing schema, in which case the existing schema will be extended with the new data. You can also run it a few times with different flow captures, the captured data will be safely merged.
+   Please note that you can use an existing schema, in which case the existing schema will be extended with the new data. You can also run it a few times with different flow captures, the captured data will be safely merged.
 
-    `<api_prefix>` is the base url of the API you wish to reverse-engineer. You will need to obtain it by observing the requests being made in mitmproxy.
+   `<api_prefix>` is the base url of the API you wish to reverse-engineer. You will need to obtain it by observing the requests being made in mitmproxy.
 
-    For example if an app has made requests like these:
+   For example if an app has made requests like these:
 
-    ```
-    https://api.example.com/v1/login
-    https://api.example.com/v1/users/2
-    https://api.example.com/v1/users/2/profile
-    ```
+   ```http
+   https://api.example.com/v1/login
+   https://api.example.com/v1/users/2
+   https://api.example.com/v1/users/2/profile
+   ```
 
-    The likely prefix is `https://api.example.com/v1`.
+   The likely prefix is `https://api.example.com/v1`.
 
 4. Running the first pass should have created a section in the schema file like this:
 
-    ```yaml
-    x-path-templates:
-    # Remove the ignore: prefix to generate an endpoint with its URL
-    # Lines that are closer to the top take precedence, the matching is greedy
-    - ignore:/addresses
-    - ignore:/basket
-    - ignore:/basket/add
-    - ignore:/basket/checkouts
-    - ignore:/basket/coupons/attach/{id}
-    - ignore:/basket/coupons/attach/104754
-    ```
+   ```yaml
+   x-path-templates:
+     # Remove the ignore: prefix to generate an endpoint with its URL
+     # Lines that are closer to the top take precedence, the matching is greedy
+     - ignore:/addresses
+     - ignore:/basket
+     - ignore:/basket/add
+     - ignore:/basket/checkouts
+     - ignore:/basket/coupons/attach/{id}
+     - ignore:/basket/coupons/attach/104754
+   ```
 
-    You should edit the schema file with a text editor and remove the `ignore:` prefix from the paths you wish to be generated. You can also adjust the parameters appearing in the paths.
+   You should edit the schema file with a text editor and remove the `ignore:` prefix from the paths you wish to be generated. You can also adjust the parameters appearing in the paths.
 
 5. Run the second pass of mitmproxy2swagger:
 
-    ```bash
-    $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
-    ```
+   ```bash
+   $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
+   # ... or ...
+   $ docker run -it -v $PWD:/app mitmproxy2swagger mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
+   ```
 
-    Run the command a second time (with the same schema file). It will pick up the edited lines and generate endpoint descriptions. 
+   Run the command a second time (with the same schema file). It will pick up the edited lines and generate endpoint descriptions.
 
-    Please note that mitmproxy2swagger will not overwrite existing endpoint descriptions, if you want to overwrite them, you can delete them before running the second pass.
+   Please note that mitmproxy2swagger will not overwrite existing endpoint descriptions, if you want to overwrite them, you can delete them before running the second pass.
 
-    Passing `--examples` will add example data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
+   Passing `--examples` will add example data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
+   Passing `--headers` will add headers data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
 
 ### HAR
 
 1. Capture and export the traffic from the browser DevTools.
 
-    In the browser DevTools, go to the Network tab and click the "Export HAR" button.
+   In the browser DevTools, go to the Network tab and click the "Export HAR" button.
+
+   ![A screenshot showing where the export har button is located](./docs/export_har_button.png)
 
-    ![A screenshot showing where the export har button is located](./docs/export_har_button.png)
 2. Continue the same way you would do with the mitmproxy dump. `mitmproxy2swagger` will automatically detect the HAR file and process it.
 
 ## Example output
 
 See the [examples](./example_outputs/). You will find a generated schema there and an html file with the generated documentation (via [redoc-cli](https://www.npmjs.com/package/redoc-cli)).
 
 See the generated html file [here](https://raw.githack.com/alufers/mitmproxy2swagger/master/example_outputs/lisek-static.html).
 
 ## License
-MIT
 
+MIT
```

### Comparing `mitmproxy2swagger-0.8.2/mitmproxy2swagger/console_util.py` & `mitmproxy2swagger-0.9.0/mitmproxy2swagger/console_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import sys
 
 ANSI_RGB = "\033[38;2;{};{};{}m"
 ANSI_RGB_BG = "\033[48;2;{};{};{}m"
 ANSI_RED = "\033[31m"
 ANSI_RESET = "\033[0m"
```

### Comparing `mitmproxy2swagger-0.8.2/mitmproxy2swagger/har_capture_reader.py` & `mitmproxy2swagger-0.9.0/mitmproxy2swagger/har_capture_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# -*- coding: utf-8 -*-
 import os
-import json_stream
 from base64 import b64decode
-from typing import Iterator
+from typing import Iterator, Union
+
+import json_stream
 
 
-# a heuristic to determine if a fileis a har archive
+# a heuristic to determine if a file is a har archive
 def har_archive_heuristic(file_path: str) -> int:
     val = 0
     # if has the har extension
     if file_path.endswith(".har"):
         val += 15
     # read the first 2048 bytes
     with open(file_path, "rb") as f:
@@ -34,14 +36,21 @@
 class HarFlowWrapper:
     def __init__(self, flow: dict):
         self.flow = flow
 
     def get_url(self):
         return self.flow["request"]["url"]
 
+    def get_matching_url(self, prefix) -> Union[str, None]:
+        """Get the requests URL if the prefix matches the URL, None
+        otherwise."""
+        if self.flow["request"]["url"].startswith(prefix):
+            return self.flow["request"]["url"]
+        return None
+
     def get_method(self):
         return self.flow["request"]["method"]
 
     def get_request_headers(self):
         headers = {}
         for kv in self.flow["request"]["headers"]:
             k = kv["name"]
@@ -77,19 +86,22 @@
 
     def get_response_body(self):
         if (
             "response" in self.flow
             and "content" in self.flow["response"]
             and "text" in self.flow["response"]["content"]
         ):
-            if (
-                "encoding" in self.flow["response"]["content"]
-                and self.flow["response"]["content"]["encoding"] == "base64"
-            ):
-                return b64decode(self.flow["response"]["content"]["text"]).decode()
+            try:
+                if (
+                    "encoding" in self.flow["response"]["content"]
+                    and self.flow["response"]["content"]["encoding"] == "base64"
+                ):
+                    return b64decode(self.flow["response"]["content"]["text"]).decode()
+            except UnicodeDecodeError:
+                return None
             return self.flow["response"]["content"]["text"]
         return None
 
 
 class HarCaptureReader:
     def __init__(self, file_path: str, progress_callback=None):
         self.file_path = file_path
```

### Comparing `mitmproxy2swagger-0.8.2/mitmproxy2swagger/mitmproxy2swagger.py` & `mitmproxy2swagger-0.9.0/mitmproxy2swagger/mitmproxy2swagger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
-"""
-Converts a mitmproxy dump file to a swagger schema.
-"""
+# -*- coding: utf-8 -*-
+"""Converts a mitmproxy dump file to a swagger schema."""
+import argparse
+import json
 import os
+import re
 import sys
 import traceback
-from mitmproxy.exceptions import FlowReadException
-import json
-import argparse
+import urllib
+from typing import Any, Sequence
+
 import ruamel.yaml
-import re
-from . import swagger_util
-from .har_capture_reader import HarCaptureReader, har_archive_heuristic
-from .mitmproxy_capture_reader import (
+from mitmproxy.exceptions import FlowReadException
+
+from mitmproxy2swagger import console_util, swagger_util
+from mitmproxy2swagger.har_capture_reader import HarCaptureReader, har_archive_heuristic
+from mitmproxy2swagger.mitmproxy_capture_reader import (
     MitmproxyCaptureReader,
     mitmproxy_dump_file_huristic,
 )
-from . import console_util
-import urllib
 
 
 def path_to_regex(path):
     # replace the path template with a regex
     path = path.replace("\\", "\\\\")
     path = path.replace("{", "(?P<")
     path = path.replace("}", ">[^/]+)")
@@ -58,15 +59,15 @@
         print("har score: " + str(har_score))
         print("mitmproxy score: " + str(mitmproxy_score))
     if har_score > mitmproxy_score:
         return HarCaptureReader(file_path, progress_callback)
     return MitmproxyCaptureReader(file_path, progress_callback)
 
 
-def main():
+def main(override_args: Sequence[str] | None = None):
     parser = argparse.ArgumentParser(
         description="Converts a mitmproxy dump file or HAR to a swagger schema."
     )
     parser.add_argument(
         "-i",
         "--input",
         help="The input mitmproxy dump file or HAR dump file (from DevTools)",
@@ -82,40 +83,48 @@
     parser.add_argument(
         "-e",
         "--examples",
         action="store_true",
         help="Include examples in the schema. This might expose sensitive information.",
     )
     parser.add_argument(
+        "-hd",
+        "--headers",
+        action="store_true",
+        help="Include headers in the schema. This might expose sensitive information.",
+    )
+    parser.add_argument(
         "-f",
         "--format",
         choices=["flow", "har"],
         help="Override the input file format auto-detection.",
     )
-    args = parser.parse_args()
+    args = parser.parse_args(override_args)
 
     yaml = ruamel.yaml.YAML()
 
-    capture_reader = None
+    capture_reader: MitmproxyCaptureReader | HarCaptureReader
     if args.format == "flow" or args.format == "mitmproxy":
         capture_reader = MitmproxyCaptureReader(args.input, progress_callback)
     elif args.format == "har":
         capture_reader = HarCaptureReader(args.input, progress_callback)
     else:
         capture_reader = detect_input_format(args.input)
 
     swagger = None
 
     # try loading the existing swagger file
     try:
-        with open(args.output, "r") as f:
+        base_dir = os.getcwd()
+        relative_path = args.output
+        abs_path = os.path.join(base_dir, relative_path)
+        with open(abs_path, "r") as f:
             swagger = yaml.load(f)
     except FileNotFoundError:
         print("No existing swagger file found. Creating new one.")
-        pass
     if swagger is None:
         swagger = ruamel.yaml.comments.CommentedMap(
             {
                 "openapi": "3.0.0",
                 "info": {
                     "title": args.input + " Mitmproxy2Swagger",
                     "version": "1.0.0",
@@ -152,22 +161,23 @@
     # new endpoints will be added here so that they can be added as comments in the swagger file
     new_path_templates = []
     for path in path_templates:
         re.compile(path_to_regex(path))
     path_template_regexes = [re.compile(path_to_regex(path)) for path in path_templates]
 
     try:
-        for f in capture_reader.captured_requests():
+        for req in capture_reader.captured_requests():
             # strip the api prefix from the url
-            url = f.get_url()
-            if not url.startswith(args.api_prefix):
+            url = req.get_matching_url(args.api_prefix)
+
+            if url is None:
                 continue
-            method = f.get_method().lower()
+            method = req.get_method().lower()
             path = strip_query_string(url).removeprefix(args.api_prefix)
-            status = f.get_response_status_code()
+            status = req.get_response_status_code()
 
             # check if the path matches any of the path templates, and save the index
             path_template_index = None
             for i, path_template_regex in enumerate(path_template_regexes):
                 if path_template_regex.match(path):
                     path_template_index = i
                     break
@@ -188,37 +198,46 @@
                         method, path_template_to_set
                     ),
                     "responses": {},
                 },
             )
 
             params = swagger_util.url_to_params(url, path_template_to_set)
-
+            if args.headers:
+                headers_request = swagger_util.request_to_headers(
+                    req.get_request_headers()
+                )
+                if headers_request is not None and len(headers_request) > 0:
+                    set_key_if_not_exists(
+                        swagger["paths"][path_template_to_set][method],
+                        "parameters",
+                        headers_request,
+                    )
             if params is not None and len(params) > 0:
                 set_key_if_not_exists(
                     swagger["paths"][path_template_to_set][method], "parameters", params
                 )
 
             if method not in ["get", "head"]:
-                body = f.get_request_body()
+                body = req.get_request_body()
                 if body is not None:
                     body_val = None
                     content_type = None
                     # try to parse the body as json
                     try:
-                        body_val = json.loads(f.get_request_body())
+                        body_val = json.loads(req.get_request_body())
                         content_type = "application/json"
                     except UnicodeDecodeError:
                         pass
                     except json.decoder.JSONDecodeError:
                         pass
                     if content_type is None:
                         # try to parse the body as form data
                         try:
-                            body_val_bytes = dict(
+                            body_val_bytes: Any = dict(
                                 urllib.parse.parse_qsl(
                                     body, encoding="utf-8", keep_blank_values=True
                                 )
                             )
                             body_val = {}
                             did_find_anything = False
                             for key, value in body_val_bytes.items():
@@ -246,40 +265,60 @@
                         set_key_if_not_exists(
                             swagger["paths"][path_template_to_set][method],
                             "requestBody",
                             content_to_set,
                         )
 
             # try parsing the response as json
-            response_body = f.get_response_body()
+            response_body = req.get_response_body()
             if response_body is not None:
                 try:
                     response_json = json.loads(response_body)
                 except UnicodeDecodeError:
                     response_json = None
                 except json.decoder.JSONDecodeError:
                     response_json = None
                 if response_json is not None:
                     resp_data_to_set = {
-                        "description": f.get_response_reason(),
+                        "description": req.get_response_reason(),
                         "content": {
                             "application/json": {
                                 "schema": swagger_util.value_to_schema(response_json)
                             }
                         },
                     }
                     if args.examples:
                         resp_data_to_set["content"]["application/json"][
                             "example"
                         ] = swagger_util.limit_example_size(response_json)
+                    if args.headers:
+                        resp_data_to_set["headers"] = swagger_util.response_to_headers(
+                            req.get_response_headers()
+                        )
+
                     set_key_if_not_exists(
                         swagger["paths"][path_template_to_set][method]["responses"],
                         str(status),
                         resp_data_to_set,
                     )
+            if (
+                "responses" in swagger["paths"][path_template_to_set][method]
+                and len(swagger["paths"][path_template_to_set][method]["responses"])
+                == 0
+            ):
+                # add a default response if there were no responses detected,
+                # this is for compliance with the OpenAPI spec
+                content_type = (
+                    req.get_response_headers().get("content-type") or "text/plain"
+                )
+
+                swagger["paths"][path_template_to_set][method]["responses"]["200"] = {
+                    "description": "OK",
+                    "content": {content_type: {}},
+                }
 
     except FlowReadException as e:
         print(f"Flow file corrupted: {e}")
         traceback.print_exception(*sys.exc_info())
         print(
             f"{console_util.ANSI_RED}Failed to parse the input file as '{capture_reader.name()}'. "
         )
```

### Comparing `mitmproxy2swagger-0.8.2/mitmproxy2swagger/swagger_util.py` & `mitmproxy2swagger-0.9.0/mitmproxy2swagger/swagger_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+# -*- coding: utf-8 -*-
 import urllib
+from typing import Any, List
 
 VERBS = [
     "add",
     "create",
     "delete",
     "get",
     "attach",
@@ -74,14 +76,43 @@
                         "type": "number" if query_params[key][0].isdigit() else "string"
                     },
                 }
             )
     return params
 
 
+def request_to_headers(headers: dict[str, List[Any]], add_example: bool = False):
+    """When given an url and its path template, generates the parameters
+    section of the request."""
+    params = []
+    if headers:
+        for key in headers:
+            h = {
+                "name": key,
+                "in": "header",
+                "required": False,
+                "schema": {"type": "number" if headers[key][0].isdigit() else "string"},
+            }
+            if add_example:
+                h["example"] = headers[key][0]
+            params.append(h)
+    return params
+
+
+def response_to_headers(headers):
+    header = {}
+    if headers:
+        for key in headers:
+            header[key] = {
+                "description": headers[key][0],
+                "schema": {"type": "number" if headers[key][0].isdigit() else "string"},
+            }
+    return header
+
+
 def value_to_schema(value):
     # check if value is a number
     if type(value) == int or type(value) == float:
         return {"type": "number"}
     # check if value is a boolean
     elif type(value) == bool:
         return {"type": "boolean"}
```

### Comparing `mitmproxy2swagger-0.8.2/PKG-INFO` & `mitmproxy2swagger-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitmproxy2swagger
-Version: 0.8.2
+Version: 0.9.0
 Summary: 
 License: MIT
 Author: alufers
 Author-email: alufers@wp.pl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,128 +14,136 @@
 Requires-Dist: json-stream (>=2.2.0,<3.0.0)
 Requires-Dist: mitmproxy (>=9.0.1,<10.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Description-Content-Type: text/markdown
 
 # mitmproxy2swagger
 
-
 [![PyPI version](https://badge.fury.io/py/mitmproxy2swagger.svg)](https://badge.fury.io/py/mitmproxy2swagger)
 [![Arch Linux repository](https://img.shields.io/badge/archlinux-mitmproxy2swagger-blue)](https://archlinux.org/packages/community/any/mitmproxy2swagger/)
 
-
-https://user-images.githubusercontent.com/5400940/168086818-c48f60ab-3f95-42eb-b435-c8b1a6326b81.mp4
-
-
+<https://user-images.githubusercontent.com/5400940/168086818-c48f60ab-3f95-42eb-b435-c8b1a6326b81.mp4>
 
 A tool for automatically converting [mitmproxy](https://mitmproxy.org/) captures to [OpenAPI 3.0](https://swagger.io/specification/) specifications. This means that you can automatically reverse-engineer REST APIs by just running the apps and capturing the traffic.
 
 ---
+
 **🆕 NEW!**
 
 Added support for processing HAR exported from the browser DevTools. See [Usage - HAR](#har) for more details.
 
 ---
 
 ## Installation
 
 First you will need python3 and pip3.
 
 ```bash
-$ pip install mitmproxy2swagger 
+$ pip install mitmproxy2swagger
 # ... or ...
 $ pip3 install mitmproxy2swagger
+# ... or ...
+$ git clone git@github.com:alufers/mitmproxy2swagger.git
+$ cd mitmproxy2swagger
+$ docker build -t mitmproxy2swagger .
 ```
 
 Then clone the repo and run `mitmproxy2swagger` as per examples below.
 
 ## Usage
 
 ### Mitmproxy
 
 To create a specification by inspecting HTTP traffic you will need to:
 
 1. Capture the traffic by using the mitmproxy tool. I personally recommend using mitmweb, which is a web interface built-in to mitmproxy.
 
-    ```bash
-    $ mitmweb
-    Web server listening at http://127.0.0.1:8081/
-    Proxy server listening at http://*:9999
-    ...
-    ```
-    **IMPORTANT**
+   ```bash
+   $ mitmweb
+   Web server listening at http://127.0.0.1:8081/
+   Proxy server listening at http://*:9999
+   ...
+   ```
 
-    To configure your client to use the proxy exposed by mitm proxy, please consult the [mitmproxy documentation](https://docs.mitmproxy.org/stable/) for more information.
+   **IMPORTANT**
+
+   To configure your client to use the proxy exposed by mitm proxy, please consult the [mitmproxy documentation](https://docs.mitmproxy.org/stable/) for more information.
 
 2. Save the traffic to a flow file.
 
-    In mitmweb you can do this by using the "File" menu and selecting "Save":
-    
-    ![](./docs/mitmweb_save.png)
+   In mitmweb you can do this by using the "File" menu and selecting "Save":
+
+   ![A screenshot showing the location of the "Save" option in the "File" menu](./docs/mitmweb_save.png)
 
 3. Run the first pass of mitmproxy2swagger:
 
-    ```bash
-    $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
-    ```
+   ```bash
+   $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
+   # ... or ...
+   $ docker run -it -v $PWD:/app mitmproxy2swagger mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix>
+   ```
 
-    Please note that you can use an existing schema, in which case the existing schema will be extended with the new data. You can also run it a few times with different flow captures, the captured data will be safely merged.
+   Please note that you can use an existing schema, in which case the existing schema will be extended with the new data. You can also run it a few times with different flow captures, the captured data will be safely merged.
 
-    `<api_prefix>` is the base url of the API you wish to reverse-engineer. You will need to obtain it by observing the requests being made in mitmproxy.
+   `<api_prefix>` is the base url of the API you wish to reverse-engineer. You will need to obtain it by observing the requests being made in mitmproxy.
 
-    For example if an app has made requests like these:
+   For example if an app has made requests like these:
 
-    ```
-    https://api.example.com/v1/login
-    https://api.example.com/v1/users/2
-    https://api.example.com/v1/users/2/profile
-    ```
+   ```http
+   https://api.example.com/v1/login
+   https://api.example.com/v1/users/2
+   https://api.example.com/v1/users/2/profile
+   ```
 
-    The likely prefix is `https://api.example.com/v1`.
+   The likely prefix is `https://api.example.com/v1`.
 
 4. Running the first pass should have created a section in the schema file like this:
 
-    ```yaml
-    x-path-templates:
-    # Remove the ignore: prefix to generate an endpoint with its URL
-    # Lines that are closer to the top take precedence, the matching is greedy
-    - ignore:/addresses
-    - ignore:/basket
-    - ignore:/basket/add
-    - ignore:/basket/checkouts
-    - ignore:/basket/coupons/attach/{id}
-    - ignore:/basket/coupons/attach/104754
-    ```
+   ```yaml
+   x-path-templates:
+     # Remove the ignore: prefix to generate an endpoint with its URL
+     # Lines that are closer to the top take precedence, the matching is greedy
+     - ignore:/addresses
+     - ignore:/basket
+     - ignore:/basket/add
+     - ignore:/basket/checkouts
+     - ignore:/basket/coupons/attach/{id}
+     - ignore:/basket/coupons/attach/104754
+   ```
 
-    You should edit the schema file with a text editor and remove the `ignore:` prefix from the paths you wish to be generated. You can also adjust the parameters appearing in the paths.
+   You should edit the schema file with a text editor and remove the `ignore:` prefix from the paths you wish to be generated. You can also adjust the parameters appearing in the paths.
 
 5. Run the second pass of mitmproxy2swagger:
 
-    ```bash
-    $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
-    ```
+   ```bash
+   $ mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
+   # ... or ...
+   $ docker run -it -v $PWD:/app mitmproxy2swagger mitmproxy2swagger -i <path_to_mitmptoxy_flow> -o <path_to_output_schema> -p <api_prefix> [--examples]
+   ```
 
-    Run the command a second time (with the same schema file). It will pick up the edited lines and generate endpoint descriptions. 
+   Run the command a second time (with the same schema file). It will pick up the edited lines and generate endpoint descriptions.
 
-    Please note that mitmproxy2swagger will not overwrite existing endpoint descriptions, if you want to overwrite them, you can delete them before running the second pass.
+   Please note that mitmproxy2swagger will not overwrite existing endpoint descriptions, if you want to overwrite them, you can delete them before running the second pass.
 
-    Passing `--examples` will add example data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
+   Passing `--examples` will add example data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
+   Passing `--headers` will add headers data to requests and responses. Take caution when using this option, as it may add sensitive data (tokens, passwords, personal information etc.) to the schema.
 
 ### HAR
 
 1. Capture and export the traffic from the browser DevTools.
 
-    In the browser DevTools, go to the Network tab and click the "Export HAR" button.
+   In the browser DevTools, go to the Network tab and click the "Export HAR" button.
+
+   ![A screenshot showing where the export har button is located](./docs/export_har_button.png)
 
-    ![A screenshot showing where the export har button is located](./docs/export_har_button.png)
 2. Continue the same way you would do with the mitmproxy dump. `mitmproxy2swagger` will automatically detect the HAR file and process it.
 
 ## Example output
 
 See the [examples](./example_outputs/). You will find a generated schema there and an html file with the generated documentation (via [redoc-cli](https://www.npmjs.com/package/redoc-cli)).
 
 See the generated html file [here](https://raw.githack.com/alufers/mitmproxy2swagger/master/example_outputs/lisek-static.html).
 
 ## License
-MIT
 
+MIT
```

