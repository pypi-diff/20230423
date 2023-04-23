# Comparing `tmp/atlasapi-3.0.1b6.tar.gz` & `tmp/atlasapi-3.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasapi-3.0.1b6.tar", last modified: Mon Mar 27 11:07:43 2023, max compression
+gzip compressed data, was "atlasapi-3.0.1b7.tar", last modified: Sun Apr 23 20:50:26 2023, max compression
```

## Comparing `atlasapi-3.0.1b6.tar` & `atlasapi-3.0.1b7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.544278 atlasapi-3.0.1b6/
--rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/LICENSE
--rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-03-27 11:07:43.543700 atlasapi-3.0.1b6/PKG-INFO
--rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/README.rst
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.536459 atlasapi-3.0.1b6/atlasapi/
--rw-r--r--   0 mgm        (502) staff       (20)      672 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/atlasapi/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/alerts.py
--rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/api_keys.py
--rw-r--r--   0 mgm        (502) staff       (20)   110669 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/atlas.py
--rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/atlas_types.py
--rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b6/atlasapi/atlas_users.py
--rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b6/atlasapi/cloud_backup.py
--rw-r--r--   0 mgm        (502) staff       (20)    36466 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/clusters.py
--rw-r--r--   0 mgm        (502) staff       (20)     8544 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/errors.py
--rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/events.py
--rw-r--r--   0 mgm        (502) staff       (20)    60586 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/events_event_types.py
--rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/invoices_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/lib.py
--rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/logs.py
--rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/maintenance_window.py
--rw-r--r--   0 mgm        (502) staff       (20)    15755 2022-06-22 22:40:25.000000 atlasapi-3.0.1b6/atlasapi/measurements.py
--rw-r--r--   0 mgm        (502) staff       (20)    10967 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/atlasapi/network.py
--rw-r--r--   0 mgm        (502) staff       (20)      863 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/organizations.py
--rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b6/atlasapi/projects.py
--rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/serverless_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)    11207 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/settings.py
--rw-r--r--   0 mgm        (502) staff       (20)    23713 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/specs.py
--rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b6/atlasapi/teams.py
--rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/whitelist.py
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.539936 atlasapi-3.0.1b6/atlasapi.egg-info/
--rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/PKG-INFO
--rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/entry_points.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/requires.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/top_level.txt
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.542785 atlasapi-3.0.1b6/atlascli/
--rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/atlaserrors.py
--rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/atlaskey.py
--rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/cli.py
--rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/listcommand.py
--rw-r--r--   0 mgm        (502) staff       (20)       38 2023-03-27 11:07:43.544443 atlasapi-3.0.1b6/setup.cfg
--rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/setup.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.572742 atlasapi-3.0.1b7/
+-rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/LICENSE
+-rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-04-23 20:50:26.572304 atlasapi-3.0.1b7/PKG-INFO
+-rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/README.rst
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.548271 atlasapi-3.0.1b7/atlasapi/
+-rw-r--r--   0 mgm        (502) staff       (20)      672 2023-04-23 20:39:28.000000 atlasapi-3.0.1b7/atlasapi/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/alerts.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/api_keys.py
+-rw-r--r--   0 mgm        (502) staff       (20)   110669 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/atlas.py
+-rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/atlas_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b7/atlasapi/atlas_users.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b7/atlasapi/cloud_backup.py
+-rw-r--r--   0 mgm        (502) staff       (20)    36466 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/clusters.py
+-rw-r--r--   0 mgm        (502) staff       (20)     8523 2023-04-23 20:36:51.000000 atlasapi-3.0.1b7/atlasapi/errors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/events.py
+-rw-r--r--   0 mgm        (502) staff       (20)    60586 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/events_event_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/invoices_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/lib.py
+-rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/logs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/maintenance_window.py
+-rw-r--r--   0 mgm        (502) staff       (20)    15755 2022-06-22 22:40:25.000000 atlasapi-3.0.1b7/atlasapi/measurements.py
+-rw-r--r--   0 mgm        (502) staff       (20)    10967 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/network.py
+-rw-r--r--   0 mgm        (502) staff       (20)      863 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/organizations.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b7/atlasapi/projects.py
+-rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/serverless_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11207 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/settings.py
+-rw-r--r--   0 mgm        (502) staff       (20)    23713 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/specs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b7/atlasapi/teams.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/whitelist.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.550566 atlasapi-3.0.1b7/atlasapi.egg-info/
+-rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/PKG-INFO
+-rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/entry_points.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/requires.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/top_level.txt
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.571675 atlasapi-3.0.1b7/atlascli/
+-rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/atlaserrors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/atlaskey.py
+-rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/cli.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/listcommand.py
+-rw-r--r--   0 mgm        (502) staff       (20)       38 2023-04-23 20:50:26.572859 atlasapi-3.0.1b7/setup.cfg
+-rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-04-23 20:39:28.000000 atlasapi-3.0.1b7/setup.py
```

### Comparing `atlasapi-3.0.1b6/LICENSE` & `atlasapi-3.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/PKG-INFO` & `atlasapi-3.0.1b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b6
+Version: 3.0.1b7
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b6/README.rst` & `atlasapi-3.0.1b7/README.rst`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/__init__.py` & `atlasapi-3.0.1b7/atlasapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "3.0.1b6"
+__version__ = "3.0.1b7"
```

### Comparing `atlasapi-3.0.1b6/atlasapi/alerts.py` & `atlasapi-3.0.1b7/atlasapi/alerts.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/api_keys.py` & `atlasapi-3.0.1b7/atlasapi/api_keys.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/atlas.py` & `atlasapi-3.0.1b7/atlasapi/atlas.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/atlas_users.py` & `atlasapi-3.0.1b7/atlasapi/atlas_users.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/cloud_backup.py` & `atlasapi-3.0.1b7/atlasapi/cloud_backup.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/clusters.py` & `atlasapi-3.0.1b7/atlasapi/clusters.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/errors.py` & `atlasapi-3.0.1b7/atlasapi/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Provides all specific Exceptions
 """
 
 from atlasapi.settings import Settings
 from pprint import pprint
 import logging
-
+from typing import Tuple
 logger = logging.getLogger('Error_Handler')
 
 
 class ErrRole(Exception):
     """A role is not compatible with Atlas"""
     pass
 
@@ -82,53 +82,42 @@
 
     Args:
         msg (str): Short description of the error
         c (int): HTTP code
         details (dict): Response payload
     """
 
-    def __init__(self, msg, c, details):
+    def __init__(self, msg: str, c: int, details: dict):
         super().__init__(msg)
         self.code = c
         self.details = details
 
-    def getAtlasResponse(self):
+    def getAtlasResponse(self) -> Tuple[int, dict]:
         """Get details about the Atlas response
 
         Returns:
             int, str: HTTP code, Response payload
 
         """
         return self.code, self.details
 
 
-class ErrNameError(ErrAtlasGeneric):
-    """Atlas : Atlas NamingRelatedError
-
-    Constructor
-
-    Args:
-        c (int): HTTP code
-        details (dict): Response payload
-    """
-
-    def __init__(self, c, details):
-        super().__init__(details.get('detail', f'Atlas Naming Error: {details.get("detail")} '), c, details)
-
-
 class ErrMaintenanceError(ErrAtlasGeneric):
     """Atlas : Atlas MaintenanceRelatedError
 
     Constructor
 
     Args:
         c (int): HTTP code
         details (dict): Response payload
     """
 
+    def __init__(self, c, details):
+        super().__init__(details.get('detail', f'Atlas Maintenance Error: {details.get("detail")} '), c, details)
+
 
 class ErrAtlasBadRequest(ErrAtlasGeneric):
     """Atlas : Bad Request
 
     Constructor
 
     Args:
@@ -151,15 +140,16 @@
         ['DUPLICATE_SERVERLESS_INSTANCE_NAME', 'SERVERLESS_INSTANCE_NAME_INVALID']):
             raise (ErrNameError(c, details))
 
         else:
             logger.critical(f"A generic error was raised")
             logger.critical(details)
 
-        super().__init__("Something was wrong with the client request.", c, details)
+        super().__init__(f"Something was wrong with the client request. ({details.get('detail', None)})"
+                         f" [{details.get('errorCode', None)}]", c, details)
 
 
 class ErrAtlasJobError(ErrAtlasGeneric):
     """Atlas : Job error Clustername
 
     Constructor
```

### Comparing `atlasapi-3.0.1b6/atlasapi/events.py` & `atlasapi-3.0.1b7/atlasapi/events.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/events_event_types.py` & `atlasapi-3.0.1b7/atlasapi/events_event_types.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/invoices_pydantic.py` & `atlasapi-3.0.1b7/atlasapi/invoices_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/lib.py` & `atlasapi-3.0.1b7/atlasapi/lib.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/maintenance_window.py` & `atlasapi-3.0.1b7/atlasapi/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/measurements.py` & `atlasapi-3.0.1b7/atlasapi/measurements.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/network.py` & `atlasapi-3.0.1b7/atlasapi/network.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/organizations.py` & `atlasapi-3.0.1b7/atlasapi/organizations.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/projects.py` & `atlasapi-3.0.1b7/atlasapi/projects.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/serverless_pydantic.py` & `atlasapi-3.0.1b7/atlasapi/serverless_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/settings.py` & `atlasapi-3.0.1b7/atlasapi/settings.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/specs.py` & `atlasapi-3.0.1b7/atlasapi/specs.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/teams.py` & `atlasapi-3.0.1b7/atlasapi/teams.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi/whitelist.py` & `atlasapi-3.0.1b7/atlasapi/whitelist.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlasapi.egg-info/PKG-INFO` & `atlasapi-3.0.1b7/atlasapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b6
+Version: 3.0.1b7
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b6/atlasapi.egg-info/SOURCES.txt` & `atlasapi-3.0.1b7/atlasapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlascli/__init__.py` & `atlasapi-3.0.1b7/atlascli/__init__.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlascli/atlaserrors.py` & `atlasapi-3.0.1b7/atlascli/atlaserrors.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlascli/atlaskey.py` & `atlasapi-3.0.1b7/atlascli/atlaskey.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlascli/cli.py` & `atlasapi-3.0.1b7/atlascli/cli.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/atlascli/listcommand.py` & `atlasapi-3.0.1b7/atlascli/listcommand.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b6/setup.py` & `atlasapi-3.0.1b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import find_packages, setup
 
 setup(
     name='atlasapi',
-    version='3.0.1b6',
+    version='3.0.1b7',
     python_requires='>=3.7',
     packages=find_packages(exclude=("tests",)),
     install_requires=['requests', 'python-dateutil', 'isodate', 'future', 'pytz','coolname',
                       'humanfriendly', 'pydantic', 'pyhumps', 'nose'],
     setup_requires=['wheel'],
     # Metadata
     author="Matthew G. Monteleone",
```

