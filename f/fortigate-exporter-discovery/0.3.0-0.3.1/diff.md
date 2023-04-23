# Comparing `tmp/fortigate-exporter-discovery-0.3.0.tar.gz` & `tmp/fortigate-exporter-discovery-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate-exporter-discovery-0.3.0.tar", last modified: Sat Mar 25 22:24:00 2023, max compression
+gzip compressed data, was "fortigate-exporter-discovery-0.3.1.tar", last modified: Sun Apr 23 10:40:04 2023, max compression
```

## Comparing `fortigate-exporter-discovery-0.3.0.tar` & `fortigate-exporter-discovery-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/fmg_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/fmg_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/fw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/fmg_discovery/http_service_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-25 22:24:00.000000 fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:24:00.610832 fortigate-exporter-discovery-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-25 22:23:32.000000 fortigate-exporter-discovery-0.3.0/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.425112 fortigate-exporter-discovery-0.3.1/fmg_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fmg_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/fw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/fmg_discovery/http_service_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 10:40:04.000000 fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:40:04.429113 fortigate-exporter-discovery-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 10:39:37.000000 fortigate-exporter-discovery-0.3.1/tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.3.0/LICENSE` & `fortigate-exporter-discovery-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/PKG-INFO` & `fortigate-exporter-discovery-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.0/README.md` & `fortigate-exporter-discovery-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/__init__.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/__main__.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/environments.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/file_service_discovery.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/file_service_discovery.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 import os
 from typing import List, Dict, Any
 
 import yaml
 
 from fmg_discovery.environments import FMG_DISCOVERY_PROMETHEUS_SD_FILE_DIRECTORY, FMG_DISCOVERY_CONFIG
 from fmg_discovery.fmg_api import FMG
+from fmg_discovery.fmglogging import Log
+
+
+log = Log(__name__)
 
 
 def file_service_discovery():
     # Run for as file service discovery
     if not os.getenv(FMG_DISCOVERY_PROMETHEUS_SD_FILE_DIRECTORY):
         print(f"Env FMG_PROMETHEUS_SD_FILE_DIRECTORY must be set to a existing directory path")
         exit(1)
@@ -53,10 +57,11 @@
             if adom_name not in prometheus_file_sd:
                 prometheus_file_sd[adom_name] = []
             prometheus_file_sd[adom_name].append(fw.as_prometheus_file_sd_entry())
 
         # Generate configuration
         with open(f"{os.getenv(FMG_DISCOVERY_PROMETHEUS_SD_FILE_DIRECTORY)}/{adom_name}.yaml", 'w') as config_file:
             try:
-                yaml.safe_dump(prometheus_file_sd[adom_name], config_file)
+                if adom_name in prometheus_file_sd:
+                    yaml.safe_dump(prometheus_file_sd[adom_name], config_file)
             except yaml.YAMLError as err:
                 print(err)
```

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/fmg_api.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/fmg_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
 import json
 
 from typing import List, Dict, Any
 
 import requests
 import urllib3
-import logging
+
 from fmg_discovery.fw import Fortigate
+from fmg_discovery.fmglogging import Log
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-log = logging.getLogger(__name__)
+log = Log(__name__)
 
 
 class FMG:
     def __init__(self, config):
         """
         Init
         :param credentials: a dict {'host': 'localhost:3443', 'username': 'abc', 'password': 'XYZ'}
@@ -57,30 +58,31 @@
              "url": "/sys/login/user"}]}
         try:
             response_raw = requests.post(self.request_url, data=json.dumps(datagram),
                                          headers={'content-type': 'application/json'}, verify=False, timeout=10)
             response_login = response_raw.json()
             assert response_login['id'] == datagram['id']
             self.session = response_login["session"]
-
+            log.error("HALLO")
         except requests.exceptions.ConnectionError as err:
+
             log.error(f"Connection error on login: {err}")
         except Exception as err:
             log.error(f"Error on login: {err}")
 
     def get_fmg_devices(self) -> Dict[str, List[Fortigate]]:
         """
         Get FW data from FMG
         """
 
         if self.session is None:
             self._fmg_login()
         # Get all Firewalls in this ADOM
         if not self.fmg_configuration['fmg']['adoms']:
-            log.warning(f"ADOM is not configured. No data received from FortiManager.")
+            log.warn(f"ADOM is not configured. No data received from FortiManager.")
             return {}
         # Loop for each adom
         all_adom_devices = {}
         for adom in self.fmg_configuration['fmg']['adoms']:
             all_devices = []
             devices = self._get_fw_devices(adom['name'])
             for device in devices:
@@ -94,14 +96,19 @@
                     fw.labels.update(adom['labels'])
                 if 'token' in adom['fortigate']:
                     fw.token = adom['fortigate']['token']
                 if 'port' in adom['fortigate']:
                     fw.port = adom['fortigate']['port']
                 if 'profile' in adom['fortigate']:
                     fw.profile = adom['fortigate']['profile']
+                valid, cause = fw.valid()
+                if not valid:
+                    log.warn_fmt({'operation': 'fw_validate', 'adom': adom['name'], 'fw': fw.name, "status": 'false',
+                                  "cause": cause})
+                    continue
                 all_devices.append(fw)
             all_adom_devices[adom['name']] = all_devices
 
         return all_adom_devices
 
     def get_adoms(self) -> List[str]:
         """
```

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/fmglogging.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/fw.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/fw.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with fortigate-exporter-discovery.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-from typing import Dict, Any
+from typing import Dict, Any, Tuple
+import ipaddress
 
 
 class Fortigate:
     def __init__(self, name: str, ip: str):
         self.name: str = name
         self.ip: str = ip
         self.token: str = ''
@@ -36,9 +37,27 @@
         labels = self.labels.copy()
         if self.token:
             labels['token'] = self.token
         if self.profile:
             labels['profile'] = self.profile
         return labels
 
+    def valid(self) -> Tuple[bool, str]:
+        valid = True
+        cause = ""
+        if not self.name:
+            cause = f"Missing name {cause}"
+            valid = False
+        if not self.ip:
+            cause = f"Missing ip {cause}"
+            valid = False
+        if not ipaddress.ip_address(self.ip):
+            cause = f"Not a ip4/ip6 address {cause}"
+            valid = False
+        if not self.token:
+            cause = f"Missing token {cause}"
+            valid = False
+
+        return valid, cause
+
     def as_prometheus_file_sd_entry(self) -> Dict[str, Any]:
         return {'targets': [f"https://{self.ip}:{self.port}"], 'labels': self.as_labels()}
```

### Comparing `fortigate-exporter-discovery-0.3.0/fmg_discovery/http_service_discovery.py` & `fortigate-exporter-discovery-0.3.1/fmg_discovery/http_service_discovery.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sys
 import time
 from typing import List, Any, Annotated, Dict
 
 import uvicorn
 import yaml
 
-from fastapi import FastAPI, Response, Depends, HTTPException, status
+from fastapi import FastAPI, Request, Response, Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 
 import logging.config as lc
 
 from fmg_discovery.environments import FMG_DISCOVERY_CONFIG
 from fmg_discovery.fmg_api import FMG
 from fmg_discovery.fmglogging import Log
@@ -65,17 +65,25 @@
 log = Log(__name__)
 
 app = FastAPI()
 
 security = HTTPBasic()
 
 
-def basic_auth(credentials: Annotated[HTTPBasicCredentials, Depends(security)]) -> bool:
-    if not os.getenv(FMG_DISCOVERY_BASIC_AUTH_ENABLED):
+async def optional_security(request: Request):
+    if os.getenv(FMG_DISCOVERY_BASIC_AUTH_ENABLED) and os.getenv(FMG_DISCOVERY_BASIC_AUTH_ENABLED) == "true":
+        return await security(request)
+    else:
+        return None
+
+
+async def basic_auth(credentials: Annotated[HTTPBasicCredentials, Depends(optional_security)]) -> bool:
+    if not os.getenv(FMG_DISCOVERY_BASIC_AUTH_ENABLED) or os.getenv(FMG_DISCOVERY_BASIC_AUTH_ENABLED) == "false":
         return True
+
     current_username_bytes = credentials.username.encode("utf8")
     correct_username_bytes = bytes(os.getenv(FMG_DISCOVERY_BASIC_AUTH_USERNAME), 'utf-8')
     is_correct_username = secrets.compare_digest(
         current_username_bytes, correct_username_bytes
     )
     current_password_bytes = credentials.password.encode("utf8")
     correct_password_bytes = bytes(os.getenv(FMG_DISCOVERY_BASIC_AUTH_PASSWORD), 'utf-8')
@@ -126,15 +134,15 @@
         self._expire = time.time() + self._ttl
         self._cache = data
 
     def get(self):
         if time.time() < self._expire:
             log.info_fmt({"operation": "cache", "hit": True})
             return self._cache
-        log.info_fmt({"operation": "cache", "hist": False})
+        log.info_fmt({"operation": "cache", "hit": False})
         return {}
 
 
 @app.get('/')
 def hello_world():
     return Response("fmg_discovery alive!", status_code=status.HTTP_200_OK, media_type=MIME_TYPE_TEXT_HTML)
```

### Comparing `fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/PKG-INFO` & `fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.3.0/fortigate_exporter_discovery.egg-info/SOURCES.txt` & `fortigate-exporter-discovery-0.3.1/fortigate_exporter_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/setup.py` & `fortigate-exporter-discovery-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.0/tests/test_dummy.py` & `fortigate-exporter-discovery-0.3.1/tests/test_dummy.py`

 * *Files identical despite different names*

