# Comparing `tmp/fortigate-exporter-discovery-0.3.2.tar.gz` & `tmp/fortigate-exporter-discovery-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate-exporter-discovery-0.3.2.tar", last modified: Sun Apr 23 11:01:35 2023, max compression
+gzip compressed data, was "fortigate-exporter-discovery-0.3.3.tar", last modified: Sun Apr 23 11:45:32 2023, max compression
```

## Comparing `fortigate-exporter-discovery-0.3.2.tar` & `fortigate-exporter-discovery-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.099308 fortigate-exporter-discovery-0.3.2/fmg_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fmg_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/http_service_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/fmg_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fmg_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/http_service_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.3.2/LICENSE` & `fortigate-exporter-discovery-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/PKG-INFO` & `fortigate-exporter-discovery-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.2/README.md` & `fortigate-exporter-discovery-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/__init__.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/__main__.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/environments.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/file_service_discovery.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/file_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/fmg_api.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/fmg_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,18 +82,19 @@
         # Loop for each adom
         all_adom_devices = {}
         for adom in self.fmg_configuration['fmg']['adoms']:
             all_devices = []
             devices = self._get_fw_devices(adom['name'])
             for device in devices:
                 fw = Fortigate(name=device['name'], ip=device['ip'])
-                fw.labels['adom'] = adom['name']
-                fw.labels['latitude'] = device['latitude']
-                fw.labels['longitude'] = device['longitude']
-                fw.labels['platform'] = device['platform_str']
+                fw.labels['adom'] = adom['name'].strip()
+                fw.labels['latitude'] = device['latitude'].strip()
+                fw.labels['longitude'] = device['longitude'].strip()
+                fw.labels['platform'] = device['platform_str'].strip()
+                #fw.labels['name'] = device['name']
 
                 if 'labels' in adom:
                     fw.labels.update(adom['labels'])
                 if 'token' in adom['fortigate']:
                     fw.token = adom['fortigate']['token']
                 if 'port' in adom['fortigate']:
                     fw.port = adom['fortigate']['port']
```

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/fmglogging.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/fw.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/fw.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 from typing import Dict, Any, Tuple
 import ipaddress
 
 
 class Fortigate:
     def __init__(self, name: str, ip: str):
-        self.name: str = name
-        self.ip: str = ip
+        self.name: str = name.strip()
+        self.ip: str = ip.strip()
         self.token: str = ''
-        self.port: int = 8443
-        self.labels: Dict[str, str] = {}
+        self.port: int = 443
+        self.labels: Dict[str, str] = {'name': self.name}
         self.profile: str = ''
 
     def as_labels(self) -> Dict[str, str]:
 
         labels = self.labels.copy()
         if self.token:
             labels['token'] = self.token
```

### Comparing `fortigate-exporter-discovery-0.3.2/fmg_discovery/http_service_discovery.py` & `fortigate-exporter-discovery-0.3.3/fmg_discovery/http_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/PKG-INFO` & `fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/SOURCES.txt` & `fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/setup.py` & `fortigate-exporter-discovery-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.2/tests/test_dummy.py` & `fortigate-exporter-discovery-0.3.3/tests/test_dummy.py`

 * *Files identical despite different names*

