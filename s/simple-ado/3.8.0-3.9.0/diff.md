# Comparing `tmp/simple_ado-3.8.0.tar.gz` & `tmp/simple_ado-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ado-3.8.0.tar", max compression
+gzip compressed data, was "simple_ado-3.9.0.tar", max compression
```

## Comparing `simple_ado-3.8.0.tar` & `simple_ado-3.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1183 2019-07-23 10:34:26.383111 simple_ado-3.8.0/LICENSE
--rw-r--r--   0        0        0     1247 2019-07-23 10:34:26.383270 simple_ado-3.8.0/README.md
--rw-r--r--   0        0        0     1234 2022-02-08 20:44:52.819020 simple_ado-3.8.0/pyproject.toml
--rwxr-xr-x   0        0        0     9934 2022-02-03 11:52:35.117183 simple_ado-3.8.0/simple_ado/__init__.py
--rwxr-xr-x   0        0        0     3058 2021-11-23 11:46:28.471732 simple_ado-3.8.0/simple_ado/audit.py
--rwxr-xr-x   0        0        0      599 2020-10-14 11:03:57.942361 simple_ado-3.8.0/simple_ado/base_client.py
--rwxr-xr-x   0        0        0     4598 2020-10-14 12:31:31.058439 simple_ado-3.8.0/simple_ado/builds.py
--rwxr-xr-x   0        0        0     4924 2019-07-23 10:34:26.385237 simple_ado-3.8.0/simple_ado/comments.py
--rwxr-xr-x   0        0        0      925 2019-07-23 10:34:26.385533 simple_ado-3.8.0/simple_ado/exceptions.py
--rwxr-xr-x   0        0        0    23954 2022-02-08 20:41:48.252349 simple_ado-3.8.0/simple_ado/git.py
--rw-r--r--   0        0        0    14517 2022-01-28 12:00:46.523906 simple_ado-3.8.0/simple_ado/governance.py
--rw-r--r--   0        0        0     2735 2022-01-19 15:57:08.102235 simple_ado-3.8.0/simple_ado/graph.py
--rwxr-xr-x   0        0        0    15521 2021-11-23 11:54:19.811064 simple_ado-3.8.0/simple_ado/http_client.py
--rw-r--r--   0        0        0     2214 2022-01-28 12:03:32.080383 simple_ado-3.8.0/simple_ado/identities.py
--rw-r--r--   0        0        0      258 2021-11-05 11:35:42.338214 simple_ado-3.8.0/simple_ado/models/__init__.py
--rw-r--r--   0        0        0      442 2021-11-05 11:35:28.051189 simple_ado-3.8.0/simple_ado/models/audit.py
--rw-r--r--   0        0        0     1699 2021-11-23 11:53:16.205381 simple_ado-3.8.0/simple_ado/models/operations.py
--rw-r--r--   0        0        0     2932 2020-05-05 10:51:50.872983 simple_ado-3.8.0/simple_ado/models/property.py
--rwxr-xr-x   0        0        0     5197 2022-02-08 20:06:10.776393 simple_ado-3.8.0/simple_ado/pipelines.py
--rw-r--r--   0        0        0     6185 2021-11-23 11:46:42.473156 simple_ado-3.8.0/simple_ado/pools.py
--rwxr-xr-x   0        0        0    16868 2021-11-23 11:56:54.926649 simple_ado-3.8.0/simple_ado/pull_requests.py
--rw-r--r--   0        0        0    18979 2022-01-31 14:37:32.573682 simple_ado-3.8.0/simple_ado/security.py
--rw-r--r--   0        0        0      223 2020-05-05 10:51:50.794088 simple_ado-3.8.0/simple_ado/types.py
--rw-r--r--   0        0        0      573 2021-11-23 11:45:10.723787 simple_ado-3.8.0/simple_ado/user.py
--rw-r--r--   0        0        0     1537 2020-05-05 10:51:50.839099 simple_ado-3.8.0/simple_ado/utilities.py
--rw-r--r--   0        0        0     3014 2021-11-23 11:38:17.603274 simple_ado-3.8.0/simple_ado/wiki.py
--rwxr-xr-x   0        0        0    19259 2021-11-23 11:48:35.045966 simple_ado-3.8.0/simple_ado/workitems.py
--rw-r--r--   0        0        0     1998 2022-02-08 20:45:06.813463 simple_ado-3.8.0/setup.py
--rw-r--r--   0        0        0     2338 2022-02-08 20:45:06.813750 simple_ado-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1183 2019-07-23 10:34:26.383111 simple_ado-3.9.0/LICENSE
+-rw-r--r--   0        0        0     1247 2019-07-23 10:34:26.383270 simple_ado-3.9.0/README.md
+-rw-r--r--   0        0        0     1234 2022-02-09 09:45:26.041197 simple_ado-3.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0     9934 2022-02-03 11:52:35.117183 simple_ado-3.9.0/simple_ado/__init__.py
+-rwxr-xr-x   0        0        0     3058 2021-11-23 11:46:28.471732 simple_ado-3.9.0/simple_ado/audit.py
+-rwxr-xr-x   0        0        0      599 2020-10-14 11:03:57.942361 simple_ado-3.9.0/simple_ado/base_client.py
+-rwxr-xr-x   0        0        0     4598 2020-10-14 12:31:31.058439 simple_ado-3.9.0/simple_ado/builds.py
+-rwxr-xr-x   0        0        0     4924 2019-07-23 10:34:26.385237 simple_ado-3.9.0/simple_ado/comments.py
+-rwxr-xr-x   0        0        0      925 2019-07-23 10:34:26.385533 simple_ado-3.9.0/simple_ado/exceptions.py
+-rwxr-xr-x   0        0        0    24761 2022-02-09 09:43:25.791667 simple_ado-3.9.0/simple_ado/git.py
+-rw-r--r--   0        0        0    14517 2022-01-28 12:00:46.523906 simple_ado-3.9.0/simple_ado/governance.py
+-rw-r--r--   0        0        0     2735 2022-01-19 15:57:08.102235 simple_ado-3.9.0/simple_ado/graph.py
+-rwxr-xr-x   0        0        0    15521 2021-11-23 11:54:19.811064 simple_ado-3.9.0/simple_ado/http_client.py
+-rw-r--r--   0        0        0     2214 2022-01-28 12:03:32.080383 simple_ado-3.9.0/simple_ado/identities.py
+-rw-r--r--   0        0        0      258 2021-11-05 11:35:42.338214 simple_ado-3.9.0/simple_ado/models/__init__.py
+-rw-r--r--   0        0        0      442 2021-11-05 11:35:28.051189 simple_ado-3.9.0/simple_ado/models/audit.py
+-rw-r--r--   0        0        0     1699 2021-11-23 11:53:16.205381 simple_ado-3.9.0/simple_ado/models/operations.py
+-rw-r--r--   0        0        0     2932 2020-05-05 10:51:50.872983 simple_ado-3.9.0/simple_ado/models/property.py
+-rwxr-xr-x   0        0        0     5197 2022-02-08 20:06:10.776393 simple_ado-3.9.0/simple_ado/pipelines.py
+-rw-r--r--   0        0        0     6185 2021-11-23 11:46:42.473156 simple_ado-3.9.0/simple_ado/pools.py
+-rwxr-xr-x   0        0        0    16868 2021-11-23 11:56:54.926649 simple_ado-3.9.0/simple_ado/pull_requests.py
+-rw-r--r--   0        0        0    18979 2022-01-31 14:37:32.573682 simple_ado-3.9.0/simple_ado/security.py
+-rw-r--r--   0        0        0      223 2020-05-05 10:51:50.794088 simple_ado-3.9.0/simple_ado/types.py
+-rw-r--r--   0        0        0      573 2021-11-23 11:45:10.723787 simple_ado-3.9.0/simple_ado/user.py
+-rw-r--r--   0        0        0     1537 2020-05-05 10:51:50.839099 simple_ado-3.9.0/simple_ado/utilities.py
+-rw-r--r--   0        0        0     3014 2021-11-23 11:38:17.603274 simple_ado-3.9.0/simple_ado/wiki.py
+-rwxr-xr-x   0        0        0    19259 2021-11-23 11:48:35.045966 simple_ado-3.9.0/simple_ado/workitems.py
+-rw-r--r--   0        0        0     1998 2022-02-09 09:45:46.063506 simple_ado-3.9.0/setup.py
+-rw-r--r--   0        0        0     2338 2022-02-09 09:45:46.063794 simple_ado-3.9.0/PKG-INFO
```

### Comparing `simple_ado-3.8.0/LICENSE` & `simple_ado-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/README.md` & `simple_ado-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/pyproject.toml` & `simple_ado-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple_ado"
-version = "3.8.0"
+version = "3.9.0"
 description = "A simple wrapper around the Azure DevOps REST API"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
```

### Comparing `simple_ado-3.8.0/simple_ado/__init__.py` & `simple_ado-3.9.0/simple_ado/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/audit.py` & `simple_ado-3.9.0/simple_ado/audit.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/base_client.py` & `simple_ado-3.9.0/simple_ado/base_client.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/builds.py` & `simple_ado-3.9.0/simple_ado/builds.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/comments.py` & `simple_ado-3.9.0/simple_ado/comments.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/exceptions.py` & `simple_ado-3.9.0/simple_ado/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/git.py` & `simple_ado-3.9.0/simple_ado/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,18 @@
 
         :param str project_id: The ID of the project
         :param str repository_id: The ID of the repository
 
         :returns: The ADO response with the data in it
         """
         self.log.debug(f"Getting repository {repository_id}")
-        request_url = f"{self.http_client.api_endpoint(project_id=project_id)}/git/repositories/{repository_id}?api-version=6.0"
+        request_url = (
+            f"{self.http_client.api_endpoint(project_id=project_id)}/git/"
+            + f"repositories/{repository_id}?api-version=6.0"
+        )
         response = self.http_client.get(request_url)
         return self.http_client.decode_response(response)
 
     def get_status(self, *, sha: str, project_id: str, repository_id: str) -> ADOResponse:
         """Set a status on a PR.
 
         :param str sha: The SHA of the commit to add the status to.
@@ -376,14 +379,34 @@
         response_data = self.http_client.decode_response(response)
         return self.http_client.extract_value(response_data)
 
         # pylint: enable=too-complex
 
     # pylint: enable=too-many-locals
 
+    def get_stats_for_branch(
+        self, *, project_id: str, repository_id: str, branch_name: str
+    ) -> ADOResponse:
+        """Get the stats for a branch.
+
+        :param str project_id: The ID of the project
+        :param str repository_id: The ID for the repository
+        :param str branch_name: The name of the branch to get the stats for
+
+        :returns: The ADO response with the data in it
+        """
+
+        self.log.debug("Getting stats")
+
+        request_url = f"{self.http_client.api_endpoint(project_id=project_id)}/git/repositories/{repository_id}"
+        request_url += f"/stats/branches?name={branch_name}&api-version=6.0"
+
+        response = self.http_client.get(request_url)
+        return self.http_client.decode_response(response)
+
     def get_commit(
         self,
         *,
         commit_id: str,
         project_id: str,
         repository_id: str,
         change_count: Optional[int] = None,
```

### Comparing `simple_ado-3.8.0/simple_ado/governance.py` & `simple_ado-3.9.0/simple_ado/governance.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/graph.py` & `simple_ado-3.9.0/simple_ado/graph.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/http_client.py` & `simple_ado-3.9.0/simple_ado/http_client.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/identities.py` & `simple_ado-3.9.0/simple_ado/identities.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/models/operations.py` & `simple_ado-3.9.0/simple_ado/models/operations.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/models/property.py` & `simple_ado-3.9.0/simple_ado/models/property.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/pipelines.py` & `simple_ado-3.9.0/simple_ado/pipelines.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/pools.py` & `simple_ado-3.9.0/simple_ado/pools.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/pull_requests.py` & `simple_ado-3.9.0/simple_ado/pull_requests.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/security.py` & `simple_ado-3.9.0/simple_ado/security.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/user.py` & `simple_ado-3.9.0/simple_ado/user.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/utilities.py` & `simple_ado-3.9.0/simple_ado/utilities.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/wiki.py` & `simple_ado-3.9.0/simple_ado/wiki.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/simple_ado/workitems.py` & `simple_ado-3.9.0/simple_ado/workitems.py`

 * *Files identical despite different names*

### Comparing `simple_ado-3.8.0/setup.py` & `simple_ado-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['deserialize>=1.5.1,<2.0.0', 'requests>=2.21,<3.0', 'tenacity>=6.2.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'simple-ado',
-    'version': '3.8.0',
+    'version': '3.9.0',
     'description': 'A simple wrapper around the Azure DevOps REST API',
     'long_description': "# simple_ado\n\n`simple_ado` is a Python wrapper around the Azure DevOps REST API.\n\nWhy does it exist when there is an existing Python SDK for the ADO API? \n\nSimply put, it's because the existing one is very complex and difficult to use. This version aims to be as simple as possible to use.\n\n\n# Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.\n\nWhen you submit a pull request, a CLA bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n",
     'author': 'Dale Myers',
     'author_email': 'dalemy@microsoft.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Microsoft/simple_ado',
```

### Comparing `simple_ado-3.8.0/PKG-INFO` & `simple_ado-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ado
-Version: 3.8.0
+Version: 3.9.0
 Summary: A simple wrapper around the Azure DevOps REST API
 Home-page: https://github.com/Microsoft/simple_ado
 License: MIT
 Keywords: azure,devops,ado
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.6.2,<4.0.0
```

