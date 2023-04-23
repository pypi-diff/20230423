# Comparing `tmp/pyhOn-0.8.2.tar.gz` & `tmp/pyhOn-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.2.tar", last modified: Sun Apr 23 01:37:59 2023, max compression
+gzip compressed data, was "pyhOn-0.8.3.tar", last modified: Sun Apr 23 12:42:51 2023, max compression
```

## Comparing `pyhOn-0.8.2.tar` & `pyhOn-0.8.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.109723 pyhOn-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 01:37:48.000000 pyhOn-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 01:37:59.109723 pyhOn-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 01:37:48.000000 pyhOn-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.101723 pyhOn-0.8.2/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 01:37:59.000000 pyhOn-0.8.2/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.101723 pyhOn-0.8.2/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.105723 pyhOn-0.8.2/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/hon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:59.109723 pyhOn-0.8.2/pyhon/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 01:37:48.000000 pyhOn-0.8.2/pyhon/parameter/range.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 01:37:59.109723 pyhOn-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 01:37:48.000000 pyhOn-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.159371 pyhOn-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 12:42:34.000000 pyhOn-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 12:42:51.159371 pyhOn-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 12:42:34.000000 pyhOn-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.151371 pyhOn-0.8.3/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 12:42:51.000000 pyhOn-0.8.3/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.155371 pyhOn-0.8.3/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.155371 pyhOn-0.8.3/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.155371 pyhOn-0.8.3/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.159371 pyhOn-0.8.3/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:51.159371 pyhOn-0.8.3/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 12:42:34.000000 pyhOn-0.8.3/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:42:51.159371 pyhOn-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 12:42:34.000000 pyhOn-0.8.3/setup.py
```

### Comparing `pyhOn-0.8.2/LICENSE` & `pyhOn-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/PKG-INFO` & `pyhOn-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.2
+Version: 0.8.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.2/README.md` & `pyhOn-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.3/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.2
+Version: 0.8.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.2/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.3/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/__main__.py` & `pyhOn-0.8.3/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/appliance.py` & `pyhOn-0.8.3/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/appliances/ov.py` & `pyhOn-0.8.3/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/appliances/td.py` & `pyhOn-0.8.3/pyhon/appliances/td.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/commands.py` & `pyhOn-0.8.3/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/api.py` & `pyhOn-0.8.3/pyhon/connection/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,22 @@
             return await resp.json()
 
     async def load_commands(self, appliance: HonAppliance) -> Dict:
         params: Dict = {
             "applianceType": appliance.appliance_type,
             "code": appliance.info["code"],
             "applianceModelId": appliance.appliance_model_id,
-            "firmwareId": appliance.info["eepromId"],
             "macAddress": appliance.mac_address,
             "fwVersion": appliance.info["fwVersion"],
             "os": const.OS,
             "appVersion": const.APP_VERSION,
             "series": appliance.info["series"],
         }
+        if firmware_id := appliance.info.get("eepromId"):
+            params["firmwareId"] = firmware_id
         url: str = f"{const.API_URL}/commands/v1/retrieve"
         async with self._hon.get(url, params=params) as response:
             result: Dict = (await response.json()).get("payload", {})
             if not result or result.pop("resultCode") != "0":
                 return {}
             return result
```

### Comparing `pyhOn-0.8.2/pyhon/connection/auth.py` & `pyhOn-0.8.3/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/device.py` & `pyhOn-0.8.3/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.3/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/handler/auth.py` & `pyhOn-0.8.3/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/handler/base.py` & `pyhOn-0.8.3/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/connection/handler/hon.py` & `pyhOn-0.8.3/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/helper.py` & `pyhOn-0.8.3/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/hon.py` & `pyhOn-0.8.3/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/parameter/base.py` & `pyhOn-0.8.3/pyhon/parameter/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/parameter/enum.py` & `pyhOn-0.8.3/pyhon/parameter/enum.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/parameter/fixed.py` & `pyhOn-0.8.3/pyhon/parameter/fixed.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/parameter/program.py` & `pyhOn-0.8.3/pyhon/parameter/program.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/pyhon/parameter/range.py` & `pyhOn-0.8.3/pyhon/parameter/range.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.2/setup.py` & `pyhOn-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.2",
+    version="0.8.3",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

