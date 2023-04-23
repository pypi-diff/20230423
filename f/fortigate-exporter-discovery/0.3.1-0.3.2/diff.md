# Comparing `tmp/fortigate-exporter-discovery-0.3.1.tar.gz` & `tmp/fortigate-exporter-discovery-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate-exporter-discovery-0.3.1.tar", last modified: Sun Apr 23 10:40:04 2023, max compression
+gzip compressed data, was "fortigate-exporter-discovery-0.3.2.tar", last modified: Sun Apr 23 11:01:35 2023, max compression
```

## Comparing `fortigate-exporter-discovery-0.3.1.tar` & `fortigate-exporter-discovery-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.425112 fortigate-exporter-discovery-0.3.1/fmg_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fmg_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/http_service_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.099308 fortigate-exporter-discovery-0.3.2/fmg_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fmg_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/fw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/fmg_discovery/http_service_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:01:35.000000 fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:35.103308 fortigate-exporter-discovery-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 11:01:14.000000 fortigate-exporter-discovery-0.3.2/tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.3.1/LICENSE` & `fortigate-exporter-discovery-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/PKG-INFO` & `fortigate-exporter-discovery-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.1/README.md` & `fortigate-exporter-discovery-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/__init__.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/__main__.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/environments.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/file_service_discovery.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/file_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/fmg_api.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/fmg_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
              "url": "/sys/login/user"}]}
         try:
             response_raw = requests.post(self.request_url, data=json.dumps(datagram),
                                          headers={'content-type': 'application/json'}, verify=False, timeout=10)
             response_login = response_raw.json()
             assert response_login['id'] == datagram['id']
             self.session = response_login["session"]
-            log.error("HALLO")
         except requests.exceptions.ConnectionError as err:
 
             log.error(f"Connection error on login: {err}")
         except Exception as err:
             log.error(f"Error on login: {err}")
 
     def get_fmg_devices(self) -> Dict[str, List[Fortigate]]:
```

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/fmglogging.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/fw.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/fw.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         cause = ""
         if not self.name:
             cause = f"Missing name {cause}"
             valid = False
         if not self.ip:
             cause = f"Missing ip {cause}"
             valid = False
-        if not ipaddress.ip_address(self.ip):
+        if self.ip and not ipaddress.ip_address(self.ip):
             cause = f"Not a ip4/ip6 address {cause}"
             valid = False
         if not self.token:
             cause = f"Missing token {cause}"
             valid = False
 
         return valid, cause
```

### Comparing `fortigate-exporter-discovery-0.3.1/fmg_discovery/http_service_discovery.py` & `fortigate-exporter-discovery-0.3.2/fmg_discovery/http_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/PKG-INFO` & `fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/SOURCES.txt` & `fortigate-exporter-discovery-0.3.2/fortigate_exporter_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/setup.py` & `fortigate-exporter-discovery-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.1/tests/test_dummy.py` & `fortigate-exporter-discovery-0.3.2/tests/test_dummy.py`

 * *Files identical despite different names*

