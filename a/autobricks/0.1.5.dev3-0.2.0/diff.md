# Comparing `tmp/autobricks-0.1.5.dev3.tar.gz` & `tmp/autobricks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobricks-0.1.5.dev3.tar", last modified: Sun Mar 26 17:27:32 2023, max compression
+gzip compressed data, was "autobricks-0.2.0.tar", last modified: Sun Apr 23 20:01:06 2023, max compression
```

## Comparing `autobricks-0.1.5.dev3.tar` & `autobricks-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-26 17:27:32.124568 autobricks-0.1.5.dev3/
--rw-r--r--   0 vsts      (1001) docker     (123)      996 2023-03-26 17:27:32.124568 autobricks-0.1.5.dev3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-26 17:27:32.120568 autobricks-0.1.5.dev3/autobricks/
--rw-r--r--   0 vsts      (1001) docker     (123)     8969 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/Cluster.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3552 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/Dbfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3604 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/Job.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/Library.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7585 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/SetupTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9295 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/Workspace.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1272 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/_decode_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-26 17:27:32.124568 autobricks-0.1.5.dev3/autobricks/api_service/
--rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5029 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/_auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1441 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/_auth_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1170 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/_base_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2875 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3031 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/api_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      313 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/autobricks/api_service/autobricks_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-26 17:27:32.120568 autobricks-0.1.5.dev3/autobricks.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      996 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      683 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-03-26 17:27:31.000000 autobricks-0.1.5.dev3/autobricks.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-03-26 17:27:32.124568 autobricks-0.1.5.dev3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1081 2023-03-26 17:27:04.000000 autobricks-0.1.5.dev3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:01:06.151922 autobricks-0.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-23 20:01:06.151922 autobricks-0.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-04-23 20:00:14.000000 autobricks-0.2.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:01:06.151922 autobricks-0.2.0/autobricks/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9015 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Cluster.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3558 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Dbfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3591 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Library.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7638 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/SetupTools.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14308 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Sql.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11141 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/Workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1272 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/_decode_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:01:06.151922 autobricks-0.2.0/autobricks/api_service/
+-rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5024 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1442 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/_auth_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/_base_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4367 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/api_service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      313 2023-04-23 20:00:14.000000 autobricks-0.2.0/autobricks/api_service/autobricks_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:01:06.151922 autobricks-0.2.0/autobricks.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      701 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-04-23 20:01:05.000000 autobricks-0.2.0/autobricks.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-23 20:01:06.151922 autobricks-0.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-04-23 20:00:14.000000 autobricks-0.2.0/setup.py
```

### Comparing `autobricks-0.1.5.dev3/PKG-INFO` & `autobricks-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.1.5.dev3
+Version: 0.2.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.1.5.dev3/README.md` & `autobricks-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autobricks-0.1.5.dev3/autobricks/Cluster.py` & `autobricks-0.2.0/autobricks/Cluster.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     RESTART = 4
     STOP = 5
     DELETE = 6
 
 
 def cluster_name_exists(name: str):
 
-    found = cluster_get_name_ids(name)
+    found = ""  # cluster_get_name_ids(name)
 
     return len(found) > 0
 
 
 def cluster_get_by_name(name: str):
 
     response = cluster_list()
@@ -70,15 +70,15 @@
 
     elif cluster_action == ClusterAction.DELETE:
         action = "permanent-delete"
 
     cluster = dict()
     cluster["cluster_id"] = cluster_id
 
-    logger.info(f"{cluster_action.name} cluster: {cluster_id}")
+    _logger.info(f"{cluster_action.name} cluster: {cluster_id}")
 
     response = _api_service.api_post(endpoint, action, cluster)
 
     return response
 
 
 def clusters_create(
@@ -98,14 +98,15 @@
                 entry.path,
                 pin,
                 stop,
                 delete_if_exists,
                 allow_duplicate_names,
                 init_script_path,
             )
+            _logger.debug(str(response))
 
 
 def cluster_create(
     cluster_defn_path: str,
     pin: bool = True,
     stop: bool = True,
     delete_if_exists: bool = False,
@@ -175,15 +176,15 @@
     cluster_ids = [c["cluster_id"] for c in clusters]
     _logger.info(f"deleting clusters: {str(cluster_ids)}")
 
     for c in cluster_ids:
         try:
             cluster_action(c, ClusterAction.UNPIN)
 
-        except Exception as e:
+        except Exception:
             _logger.info(f"Warning: Failed to unpin cluster_id={c}")
 
         cluster_action(c, ClusterAction.DELETE)
 
 
 def cluster_list() -> dict:
 
@@ -209,16 +210,16 @@
 def cluster_is_terminated(cluster_id: str):
 
     return get_cluster_state(cluster_id) == ClusterState.TERMINATED
 
 
 def cluster_get(cluster_id: str):
 
-    query = f"cluster_id={cluster_id}"
-    return _api_service.api_get(endpoint, "get", query=query)
+    params = {"cluster_id": cluster_id}
+    return _api_service.api_get(endpoint, "get", params=params)
 
 
 def cluster_wait_until_state(
     cluster_id: str, cluster_state: ClusterState, wait_seconds: int = 10
 ):
 
     _logger.info(
```

### Comparing `autobricks-0.1.5.dev3/autobricks/Dbfs.py` & `autobricks-0.2.0/autobricks/Dbfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .api_service import ApiService, autobricks_logging
 from ._decode_utils import base64_decode, format_path_for_os
 import base64
-import os, fnmatch
+import os
+import fnmatch
 
 _logger = autobricks_logging.get_logger(__name__)
 
 endpoint = "dbfs"
 
 
 _api_service = ApiService()
```

### Comparing `autobricks-0.1.5.dev3/autobricks/Job.py` & `autobricks-0.2.0/autobricks/Job.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 endpoint = "jobs"
 
 _api_service = ApiService()
 
 
 def job_run_get(run_id: int):
 
+    params = {"run_id": run_id}
     try:
-        response = _api_service.api_get(endpoint, "runs/get", query=f"run_id={run_id}")
+        response = _api_service.api_get(endpoint, "runs/get", params=params)
     except Exception as e:
         response = {"run_id": -1, "message": str(e)}
 
     return response
 
 
 def job_runs_list():
@@ -30,15 +31,15 @@
     return response
 
 
 def job_run_delete(run_id: int):
     data = {"run_id": run_id}
     try:
         response = _api_service.api_post(endpoint, "runs/delete", data)
-    except Exception as e:
+    except Exception:
         response = {}
 
     return response
 
 
 def job_run_submit(
     notebook_path: str,
@@ -92,15 +93,14 @@
     idempotency_token: UUID = None,
     cluster_id: str = None,
     wait_seconds: int = 5,
 ):
 
     fmt_notebook_path = format_path_for(notebook_path, OsEnum.LINUX)
 
-    start_time = time.time()
     response = job_run_submit(
         fmt_notebook_path,
         name,
         idempotency_token=idempotency_token,
         cluster_id=cluster_id,
     )
```

### Comparing `autobricks-0.1.5.dev3/autobricks/Library.py` & `autobricks-0.2.0/autobricks/Library.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     dev: int
 
 
 def _is_wheel(entry):
 
     ret = entry.path.endswith(".whl")
     ret = ret and entry.is_file()
-    ret = ret and not ".dirty" in entry.path
+    ret = ret and ".dirty" not in entry.path
 
     return ret
 
 
 def _get_wheel_version(wheel_path: str):
 
     version = inspect_wheel(wheel_path)["version"].split(".")
```

### Comparing `autobricks-0.1.5.dev3/autobricks/SetupTools.py` & `autobricks-0.2.0/autobricks/SetupTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         except OSError as e:
             print(f"Directory not copied. Error: {e}")
 
     def _is_wheel(self, entry):
 
         ret = entry.path.endswith(".whl")
         ret = ret and entry.is_file()
-        ret = ret and not ".dirty" in entry.path
+        ret = ret and ".dirty" not in entry.path
 
         return ret
 
     def _get_wheel_version(self, wheel_path: str):
 
         version = inspect_wheel(wheel_path)["version"].split(".")
 
@@ -116,14 +116,15 @@
 
                 cluster_defn, init_scripts = self._build_cluster_defn(
                     entry.path, semantic_version, init_script_path
                 )
 
                 with open(entry.path, "w") as file:
                     data = yaml.dump(cluster_defn, file)
+                    _logger.debug(data)
 
                 if init_scripts:
                     self._build_init_scripts(init_scripts, entry.name)
 
     def _build_init_scripts(self, init_scripts: dict, cluster_defn_name: str):
 
         cluster_defn_name = cluster_defn_name.replace("yaml", "sh")
@@ -135,29 +136,29 @@
                 to_path = os.path.basename(i["dbfs"]["destination"])
                 to_path = f"{self.databricks_dist_dir}/init_scripts/{to_path}"
 
                 with open(from_path, "r") as from_file:
                     with open(to_path, "w") as to_file:
                         shell = from_file.readlines()
 
-                        for l in shell:
+                        for line in shell:
 
-                            if l[0:11] == "pip install":
-                                path = l.split(" ")[-1]
+                            if line[0:11] == "pip install":
+                                path = line.split(" ")[-1]
                                 filename = os.path.basename(path)
                                 path = path.replace(filename, "")
-                                filename, ext = os.path.splitext(filename)
+                                filename, _ = os.path.splitext(filename)
                                 wheel = self._get_latest_wheel(self.dist, filename)
                                 if wheel:
                                     wheel_filename = os.path.basename(wheel.path)
                                     to_file.write(f"pip install {path}{wheel_filename}")
                                 else:
-                                    to_file.write(l)
+                                    to_file.write(line)
                             else:
-                                to_file.write(l)
+                                to_file.write(line)
 
                 os.remove(from_path)
 
     def _build_cluster_defn(
         self,
         cluster_defn_path: str,
         semantic_version: str = "",
```

### Comparing `autobricks-0.1.5.dev3/autobricks/Workspace.py` & `autobricks-0.2.0/autobricks/Workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .api_service import ApiService, autobricks_logging
+from typing import List, Union
 
 from ._decode_utils import (
     base64_encode,
     base64_decode,
     format_path_for_os,
     format_path_for,
     OS,
@@ -45,26 +46,39 @@
 
 class Language(Enum):
     SCALA = "SCALA"
     PYTHON = "PYTHON"
     SQL = "SQL"
     R = "R"
 
+
+class ObjectType(Enum):
+    DIRECTORY = "DIRECTORY"
+    NOTEBOOK = "NOTEBOOK"
+    LIBRARY = "LIBRARY"
+    FILE = "FILE"
+    REPO = "REPO"
+
+
 def get_language(extension: Extension):
 
     if extension == Extension.py:
         return Language.PYTHON
     elif extension == Extension.sql:
         return Language.SQL
     else:
         raise Exception("unknown language for extension")
 
 
 def workspace_import(
-    from_path: str, to_path: str, format: Format=Format.AUTO, language: Language=None, overwrite=True
+    from_path: str,
+    to_path: str,
+    format: Format = Format.AUTO,
+    language: Language = None,
+    overwrite=True,
 ):
 
     with open(from_path, "rb") as file:
         content = base64_encode(file.read())
 
     data = {
         "path": to_path,
@@ -105,19 +119,76 @@
 def workspace_mkdirs(path: str):
 
     data = {"path": path}
     _logger.info(f"workspace making dirs {path}")
     return _api_service.api_post(endpoint, "mkdirs", data)
 
 
+def workspace_get_folder_id(path: str):
+
+    dir = os.path.basename(path)
+    parent = path.replace(dir, "")
+    ls = workspace_list(parent)["objects"]
+    try:
+        gen = (d for d in ls if d["path"] == path)
+        dir_data = next(gen)
+        object_id = dir_data["object_id"]
+    except Exception as e:
+        msg = f"Path {path} not found in directory listing {ls}"
+        raise Exception(msg) from e
+
+    return object_id
+
+
+def workspace_find_paths(
+    folder_ids: List[str], root_folders: Union[str, List[str]] = None
+):
+
+    if not root_folders:
+        return _workspace_find_paths(folder_ids)
+    if isinstance(root_folders, str):
+        return _workspace_find_paths(folder_ids, f"/{root_folders}")
+    if isinstance(root_folders, list):
+        workpsace_paths = {}
+        for folder in root_folders:
+            paths = _workspace_find_paths(folder_ids, f"/{folder}")
+            workpsace_paths = {**workpsace_paths, **paths}
+
+        return workpsace_paths
+
+
+def _workspace_find_paths(folder_ids: List[str], path="/"):
+    folder_ids = list(dict.fromkeys(folder_ids))
+    ls = workspace_list(path)
+    folder_paths = {}
+    if ls:
+        ls = ls["objects"]
+
+        folder_paths = {}
+
+        for folder in ls:
+            id = folder["object_id"]
+            object_type = ObjectType(folder["object_type"])
+            path = folder["path"]
+            if str(id) in folder_ids:
+                folder_paths[str(id)] = folder["path"]
+            if object_type == ObjectType.DIRECTORY:
+                sub_folder_paths = _workspace_find_paths(folder_ids, path)
+                folder_paths = {**folder_paths, **sub_folder_paths}
+
+    return folder_paths
+
+
 def workspace_export(from_path: str, format: Format, to_path: str):
 
     data = {"path": from_path, "format": format.name.upper(), "direct_download": False}
 
-    _logger.info(f"workspace exporting from path {from_path} format {format.name.upper()}")
+    _logger.info(
+        f"workspace exporting from path {from_path} format {format.name.upper()}"
+    )
     response = _api_service.api_get(endpoint, "export", data)
 
     file_type = response["file_type"]
     filename = os.path.basename(from_path)
     file_path = f"{to_path}/{filename}.{file_type}"
 
     content = base64_decode(response["content"])
@@ -155,25 +226,25 @@
     return response
 
 
 def workspace_dir_exists(path: str):
 
     try:
         reponse = workspace_get_status(path)
-    except Exception as e:
+    except Exception:
         return False
 
     return reponse.get("object_type") == "DIRECTORY" and reponse.get("path") == path
 
 
 def workspace_notebook_exists(path: str):
 
     try:
         reponse = workspace_get_status(path)
-    except Exception as e:
+    except Exception:
         return False
 
     return reponse.get("object_type") == "NOTEBOOK" and reponse.get("path") == path
 
 
 def workspace_import_dir(
     from_notebook_root: str,
@@ -277,18 +348,15 @@
 
     action = {
         "action": "import",
         "from_file_path": from_file_path,
         "to_file_path": to_file_path,
     }
 
-    workspace_import(
-        from_path = from_file_path, 
-        to_path = to_file_path
-    )
+    workspace_import(from_path=from_file_path, to_path=to_file_path)
 
     return action
 
 
 def _deploy_dir(
     source_dir: str, deploy_dir: str, target_dir: str, deploy_mode: DeployMode
 ):
@@ -318,15 +386,15 @@
 
     elif deploy_mode == DeployMode.MOVE:
         new_path = deploy_dir.replace(root, modifier)
 
     elif deploy_mode == DeployMode.PARENT:
         modify_to = f"{modifier.replace('/.','')}{root}"
         new_path = deploy_dir.replace(root, modify_to)
-    
+
     elif deploy_mode == DeployMode.CHILD:
         modify_to = f"{root}{modifier}"
         new_path = deploy_dir.replace(root, modify_to)
 
     elif deploy_mode == DeployMode.ROOT_CHILD:
 
         clean_modifier = modifier.replace("\\", "/")
```

### Comparing `autobricks-0.1.5.dev3/autobricks/_decode_utils.py` & `autobricks-0.2.0/autobricks/_decode_utils.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.1.5.dev3/autobricks/api_service/_auth.py` & `autobricks-0.2.0/autobricks/api_service/_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class UserAuth(Auth):
     def __init__(self, parameters: dict):
 
         try:
             self.bearer_token = parameters["dbutilstoken"]
-        except KeyError as e:
+        except KeyError:
             raise KeyError("dbutilstoken key not found in UserAuth parameters")
 
     def get_headers(self):
         headers = {"Authorization": f"Bearer {self.bearer_token}"}
         return headers
```

### Comparing `autobricks-0.1.5.dev3/autobricks/api_service/_auth_factory.py` & `autobricks-0.2.0/autobricks/api_service/_auth_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     SPMgmtEndpointAdalAuth,
 )
 from . import autobricks_logging
 from ._exceptions import AutobricksAuthTypeNotRegistered
 
 _logger = autobricks_logging.get_logger(__name__)
 
+
 class AuthenticationType(Enum):
 
     USER = 1
     SERVICE_PRINCIPAL = 2
     SERVICE_PRINCIPAL_MGMT_ENDPOINT = 3
     SERVICE_PRINCIPAL_ADAL = 4
     SERVICE_PRINCIPAL_MGMT_ENDPOINT_ADAL = 5
```

### Comparing `autobricks-0.1.5.dev3/autobricks/api_service/_base_api.py` & `autobricks-0.2.0/autobricks/api_service/_base_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,54 @@
 from . import autobricks_logging
 import os
 
 _logger = autobricks_logging.get_logger(__name__)
 
 _ssl_verify = False if os.getenv("SSL_VERIFY", "true").lower() == "false" else True
 if not _ssl_verify:
-    _logger.info(f"WARNING SSL Verification is off!")
+    _logger.info("WARNING SSL Verification is off!")
+
 
 def base_api_get(
-    url: str, headers: dict, json: dict = None, data: dict = None, query: str = None
+    url: str, headers: dict, json: dict = None, data: dict = None, params=None
+):
+
+    response = requests.get(
+        url=url,
+        headers=headers,
+        json=json,
+        data=data,
+        verify=_ssl_verify,
+        params=params,
+    )
+
+    try:
+        response.raise_for_status()
+
+    except HTTPError as e:
+
+        msg = f"{e.response.status_code} error at {url} {e.response.text}"
+        _logger.error(msg)
+        raise e
+
+    return response
+
+
+def base_api_delete(
+    url: str, headers: dict, json: dict = None, data: dict = None, params=None
 ):
 
-    if query:
-        url = f"{url}?{query}"
-    response = requests.get(url=url, headers=headers, json=json, data=data, verify=_ssl_verify)
+    response = requests.delete(
+        url=url,
+        headers=headers,
+        json=json,
+        data=data,
+        verify=_ssl_verify,
+        params=params,
+    )
 
     try:
         response.raise_for_status()
 
     except HTTPError as e:
 
         msg = f"{e.response.status_code} error at {url} {e.response.text}"
@@ -27,15 +58,17 @@
         raise e
 
     return response
 
 
 def base_api_post(url: str, headers: dict, json: dict = None, data: dict = None):
 
-    response = requests.post(url=url, headers=headers, json=json, data=data, verify=_ssl_verify)
+    response = requests.post(
+        url=url, headers=headers, json=json, data=data, verify=_ssl_verify
+    )
 
     try:
         response.raise_for_status()
 
     except HTTPError as e:
 
         msg = f"{e.response.status_code} error at {url} {e.response.text}"
```

### Comparing `autobricks-0.1.5.dev3/autobricks/api_service/_configuration.py` & `autobricks-0.2.0/autobricks/api_service/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,9 +91,9 @@
     "mgmt_resource_endpoint": os.getenv(
         "MGMT_RESOURCE_ENDPOINT", "https://management.core.windows.net/"
     ),
     "workspace_name": os.getenv("WORKSPACE_NAME"),
     "resource_group": os.getenv("RESOURCE_GROUP"),
     "subscription_id": os.getenv("SUBSCRIPTION_ID"),
     "auth_type": os.getenv("AUTH_TYPE", "SERVICE_PRINCIPAL"),
-    "databricks_api_host": os.getenv("DATABRICKS_API_HOST")
+    "databricks_api_host": os.getenv("DATABRICKS_API_HOST"),
 }
```

### Comparing `autobricks-0.1.5.dev3/autobricks/api_service/_exceptions.py` & `autobricks-0.2.0/autobricks/api_service/_exceptions.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.1.5.dev3/autobricks.egg-info/PKG-INFO` & `autobricks-0.2.0/autobricks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.1.5.dev3
+Version: 0.2.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.1.5.dev3/autobricks.egg-info/SOURCES.txt` & `autobricks-0.2.0/autobricks.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 autobricks/Cluster.py
 autobricks/Dbfs.py
 autobricks/Job.py
 autobricks/Library.py
 autobricks/SetupTools.py
+autobricks/Sql.py
 autobricks/Workspace.py
 autobricks/_decode_utils.py
 autobricks.egg-info/PKG-INFO
 autobricks.egg-info/SOURCES.txt
 autobricks.egg-info/dependency_links.txt
 autobricks.egg-info/not-zip-safe
 autobricks.egg-info/requires.txt
```

### Comparing `autobricks-0.1.5.dev3/setup.py` & `autobricks-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "PYPI.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="autobricks",
-    version="0.1.5.dev3",
+    version="0.2.0",
     description="Databricks Deployment Utils",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://autobricks.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/autobricks',
         'Documentation': 'https://autobricks.readthedocs.io/en/latest/'
```

