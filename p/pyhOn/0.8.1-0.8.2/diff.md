# Comparing `tmp/pyhOn-0.8.1.tar.gz` & `tmp/pyhOn-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.1.tar", last modified: Wed Apr 19 18:20:09 2023, max compression
+gzip compressed data, was "pyhOn-0.8.2.tar", last modified: Sun Apr 23 01:37:59 2023, max compression
```

## Comparing `pyhOn-0.8.1.tar` & `pyhOn-0.8.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.926450 pyhOn-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 18:19:56.000000 pyhOn-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 18:20:09.926450 pyhOn-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-19 18:19:56.000000 pyhOn-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.922450 pyhOn-0.8.1/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 18:20:09.000000 pyhOn-0.8.1/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.922450 pyhOn-0.8.1/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.922450 pyhOn-0.8.1/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.922450 pyhOn-0.8.1/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.922450 pyhOn-0.8.1/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/hon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:20:09.926450 pyhOn-0.8.1/pyhon/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-19 18:19:56.000000 pyhOn-0.8.1/pyhon/parameter/range.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:20:09.926450 pyhOn-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-19 18:19:56.000000 pyhOn-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.109723 pyhOn-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 01:37:48.000000 pyhOn-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 01:37:59.109723 pyhOn-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 01:37:48.000000 pyhOn-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.101723 pyhOn-0.8.2/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.101723 pyhOn-0.8.2/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.109723 pyhOn-0.8.2/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 01:37:59.109723 pyhOn-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 01:37:48.000000 pyhOn-0.8.2/setup.py
```

### Comparing `pyhOn-0.8.1/LICENSE` & `pyhOn-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/PKG-INFO` & `pyhOn-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.1
+Version: 0.8.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.1/README.md` & `pyhOn-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.2/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.1
+Version: 0.8.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.1/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.2/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/__main__.py` & `pyhOn-0.8.2/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/appliance.py` & `pyhOn-0.8.2/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/appliances/ov.py` & `pyhOn-0.8.2/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/commands.py` & `pyhOn-0.8.2/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/api.py` & `pyhOn-0.8.2/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/auth.py` & `pyhOn-0.8.2/pyhon/connection/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,18 @@
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
         ) as response:
             try:
                 json_data = await response.json()
             except json.JSONDecodeError:
                 await self._error_logger(response)
                 return False
-            self._cognito_token = json_data["cognitoUser"]["Token"]
+            self._cognito_token = json_data.get("cognitoUser", {}).get("Token", "")
+            if not self._cognito_token:
+                _LOGGER.error(json_data)
+                raise exceptions.HonAuthenticationError()
         return True
 
     async def authenticate(self) -> None:
         self.clear()
         try:
             if not await self._load_login():
                 raise exceptions.HonAuthenticationError("Can't open login page")
```

### Comparing `pyhOn-0.8.1/pyhon/connection/device.py` & `pyhOn-0.8.2/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.2/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/handler/auth.py` & `pyhOn-0.8.2/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/handler/base.py` & `pyhOn-0.8.2/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/connection/handler/hon.py` & `pyhOn-0.8.2/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/helper.py` & `pyhOn-0.8.2/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/hon.py` & `pyhOn-0.8.2/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/parameter/base.py` & `pyhOn-0.8.2/pyhon/parameter/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/parameter/enum.py` & `pyhOn-0.8.2/pyhon/parameter/enum.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/parameter/program.py` & `pyhOn-0.8.2/pyhon/parameter/program.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.1/pyhon/parameter/range.py` & `pyhOn-0.8.2/pyhon/parameter/range.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any
+from typing import Dict, Any, List
 
 from pyhon.parameter.base import HonParameter
 
 
 def str_to_float(string: str | float) -> float:
     try:
         return int(string)
@@ -43,7 +43,11 @@
         value = str_to_float(value)
         if self._min <= value <= self._max and not value % self._step:
             self._value = value
         else:
             raise ValueError(
                 f"Allowed: min {self._min} max {self._max} step {self._step}"
             )
+
+    @property
+    def values(self) -> List[str]:
+        return [str(i) for i in range(int(self.min), int(self.max) + 1, int(self.step))]
```

### Comparing `pyhOn-0.8.1/setup.py` & `pyhOn-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.1",
+    version="0.8.2",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

