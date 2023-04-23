# Comparing `tmp/cfscanner-1.3.13.tar.gz` & `tmp/cfscanner-1.3.14.tar.gz`

## Comparing `cfscanner-1.3.13.tar` & `cfscanner-1.3.14.tar`

### file list

```diff
@@ -1,36 +1,44 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.13/.vscode/settings.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/__main__.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/args/__init__.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/args/parser.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/args/testconfig.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/report/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/report/colors.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/report/print.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/report/result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/__init__.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/conduct.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/download.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/fronting.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/tools.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/speedtest/upload.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/subnets/__init__.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/subnets/cidr.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/subnets/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/decorators.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/exceptions.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/os.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/requests.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/utils/socket.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/xray/__init__.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/xray/binary.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/xray/config.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/xray/service.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.13/cfscanner/xray/templates.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.13/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.13/LICENSE
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 cfscanner-1.3.13/README.md
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 cfscanner-1.3.13/pyproject.toml
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 cfscanner-1.3.13/PKG-INFO
+-rw-r--r--   0        0        0    15834 2020-02-02 00:00:00.000000 cfscanner-1.3.14/temp.ipynb
+-rwxr-xr-x   0        0        0 25346048 2020-02-02 00:00:00.000000 cfscanner-1.3.14/xray-linux-64
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.14/.vscode/settings.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/__main__.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/__init__.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/parser.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/testconfig.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/colors.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/print.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/__init__.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/conduct.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/download.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/fronting.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/tools.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/upload.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/__init__.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/cidr.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/decorators.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/exceptions.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/os.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/requests.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/socket.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/__init__.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/binary.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/config.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/service.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172219.log
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172314.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172527.log
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172219_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172314_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172527_result.csv
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.14/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.14/LICENSE
+-rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 cfscanner-1.3.14/README.md
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 cfscanner-1.3.14/pyproject.toml
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 cfscanner-1.3.14/PKG-INFO
```

### Comparing `cfscanner-1.3.13/cfscanner/main.py` & `cfscanner-1.3.14/cfscanner/main.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/args/parser.py` & `cfscanner-1.3.14/cfscanner/args/parser.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/args/testconfig.py` & `cfscanner-1.3.14/cfscanner/args/testconfig.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/report/print.py` & `cfscanner-1.3.14/cfscanner/report/print.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/report/result.py` & `cfscanner-1.3.14/cfscanner/report/result.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/speedtest/conduct.py` & `cfscanner-1.3.14/cfscanner/speedtest/conduct.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/speedtest/download.py` & `cfscanner-1.3.14/cfscanner/speedtest/download.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/speedtest/fronting.py` & `cfscanner-1.3.14/cfscanner/speedtest/fronting.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/speedtest/upload.py` & `cfscanner-1.3.14/cfscanner/speedtest/upload.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/subnets/cidr.py` & `cfscanner-1.3.14/cfscanner/subnets/cidr.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         list: The list of cidrs associated with ``asn_list``
     """
     try:
         r = requests.get(url, timeout=timeout)
         if r.status_code != 200:
             raise SubnetsReadError(
                 f"Could not read cidrs from url - status code: {r.status_code}", url)
-        cidr_regex = r"(?:[0-9]{1,3}\.){3}[0-9]{1,3}\/[\d]+"
+        cidr_regex = r"(?:[0-9]{1,3}\.){3}[0-9]{1,3}(?:\/[\d]+)?"
         cidrs = re.findall(cidr_regex, r.text)
         if len(cidrs) == 0:
             raise SubnetsReadError(
                 f"Could not find any cidr in url {url}"
             )
     except Exception as e:
         raise SubnetsReadError(f"Could not read cidrs from url \"{url}\"")
```

### Comparing `cfscanner-1.3.13/cfscanner/utils/decorators.py` & `cfscanner-1.3.14/cfscanner/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/utils/exceptions.py` & `cfscanner-1.3.14/cfscanner/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/utils/os.py` & `cfscanner-1.3.14/cfscanner/utils/os.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/utils/requests.py` & `cfscanner-1.3.14/cfscanner/utils/requests.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/utils/socket.py` & `cfscanner-1.3.14/cfscanner/utils/socket.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/xray/__init__.py` & `cfscanner-1.3.14/cfscanner/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/xray/binary.py` & `cfscanner-1.3.14/cfscanner/xray/binary.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/xray/config.py` & `cfscanner-1.3.14/cfscanner/xray/config.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/xray/service.py` & `cfscanner-1.3.14/cfscanner/xray/service.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/cfscanner/xray/templates.py` & `cfscanner-1.3.14/cfscanner/xray/templates.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/.gitignore` & `cfscanner-1.3.14/.gitignore`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/LICENSE` & `cfscanner-1.3.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.13/README.md` & `cfscanner-1.3.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -222,10 +222,12 @@
 * 1.3.11
   * fixed multiple printing bug
 * 1.3.12
   * added setuptools to the dependencies
 * 1.3.13
   * added removal of duplicate subnets (issue [#490])
   * reduced the file size used for fronting test
+* 1.3.14
+  * Fixed a bug in reading ips from url. The regex now supports single ips as well
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.13-blue
```

### Comparing `cfscanner-1.3.13/pyproject.toml` & `cfscanner-1.3.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfscanner"
-version = "1.3.13"
+version = "1.3.14"
 authors = [
   { name="tempookian", email="tempookian@gmail.com" },
   { name="Morteza Bashsiz", email="morteza.bashsiz@gmail.com"}
 ]
 description = "Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `cfscanner-1.3.13/PKG-INFO` & `cfscanner-1.3.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.3.13
+Version: 1.3.14
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -240,10 +240,12 @@
 * 1.3.11
   * fixed multiple printing bug
 * 1.3.12
   * added setuptools to the dependencies
 * 1.3.13
   * added removal of duplicate subnets (issue [#490])
   * reduced the file size used for fronting test
+* 1.3.14
+  * Fixed a bug in reading ips from url. The regex now supports single ips as well
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.13-blue
```

