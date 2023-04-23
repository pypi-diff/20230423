# Comparing `tmp/workflow_templater-0.2.8.tar.gz` & `tmp/workflow_templater-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workflow_templater-0.2.8.tar", last modified: Fri Dec 30 14:14:26 2022, max compression
+gzip compressed data, was "workflow_templater-0.2.9.tar", last modified: Sat Apr 22 20:17:13 2023, max compression
```

## Comparing `workflow_templater-0.2.8.tar` & `workflow_templater-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 14:14:26.387696 workflow_templater-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2022-12-30 14:14:26.387696 workflow_templater-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 14:14:26.387696 workflow_templater-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1506 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 14:14:26.387696 workflow_templater-0.2.8/workflow_templater/
--rwxr-xr-x   0 runner    (1001) docker     (123)    21304 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/workflow_templater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/workflow_templater/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/workflow_templater/our_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/workflow_templater/quote_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2022-12-30 14:13:31.000000 workflow_templater-0.2.8/workflow_templater/urlopen_jira.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 14:14:26.387696 workflow_templater-0.2.8/workflow_templater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 14:14:26.000000 workflow_templater-0.2.8/workflow_templater.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:17:13.984219 workflow_templater-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-22 20:17:13.984219 workflow_templater-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 20:17:13.984219 workflow_templater-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1506 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:17:13.980219 workflow_templater-0.2.9/workflow_templater/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21337 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/workflow_templater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/workflow_templater/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/workflow_templater/our_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/workflow_templater/quote_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-22 20:16:29.000000 workflow_templater-0.2.9/workflow_templater/urlopen_jira.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:17:13.984219 workflow_templater-0.2.9/workflow_templater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:17:13.000000 workflow_templater-0.2.9/workflow_templater.egg-info/zip-safe
```

### Comparing `workflow_templater-0.2.8/LICENSE` & `workflow_templater-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/PKG-INFO` & `workflow_templater-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workflow_templater
-Version: 0.2.8
+Version: 0.2.9
 Summary: Template engine for (currently) Jira and Email. Uses yaml and jinja2. It helps you create multiple (possibly cross-linked) jira issues and emails from a template.
 Home-page: https://github.com/m-khvoinitsky/workflow-templater
 Author: Mikhail Khvoinitsky
 Author-email: me@khvoinitsky.org
 Keywords: jira email template workflow release
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `workflow_templater-0.2.8/README.md` & `workflow_templater-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/setup.py` & `workflow_templater-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/workflow_templater/__init__.py` & `workflow_templater-0.2.9/workflow_templater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     from .common import pretty_dump
 from jinja2 import StrictUndefined, DebugUndefined
 import datetime
 import smtplib
 import importlib.util
 from email.mime.text import MIMEText
 from appdirs import user_config_dir
+from natsort import natsorted
 
 
 yaml = ruamel.yaml.YAML(typ='safe')
 
 COMMON_VARS_FILES = (
     '0_common.yaml',
     '00_common.yaml',
@@ -399,15 +400,15 @@
         undefined=DebugUndefined,
     )
     jinja_env_strict = OurJinjaEnvironment(
         loader=OurJinjaLoader(args.template_dir),
         undefined=StrictUndefined,
     )
 
-    for filename in sorted(os.listdir(args.template_dir)):
+    for filename in natsorted(os.listdir(args.template_dir)):
         for issue_type_ext, IssueType in ISSUE_TYPES.items():
             if filename.endswith(issue_type_ext):
                 if IssueType == JiraIssue:
                     type_specific_params = { 'jira': args.jira }
                 elif IssueType == EmailIssue:
                     type_specific_params = { 'smtp': args.email_smtp, 'user': args.email_user, 'email_from': args.email_from, 'keyring_service': args.email_keyring_service_name }
                 with open(os.path.join(args.template_dir, filename), 'r', encoding='utf8') as f:
```

### Comparing `workflow_templater-0.2.8/workflow_templater/common.py` & `workflow_templater-0.2.9/workflow_templater/common.py`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/workflow_templater/our_jinja.py` & `workflow_templater-0.2.9/workflow_templater/our_jinja.py`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/workflow_templater/quote_windows.py` & `workflow_templater-0.2.9/workflow_templater/quote_windows.py`

 * *Files identical despite different names*

### Comparing `workflow_templater-0.2.8/workflow_templater/urlopen_jira.py` & `workflow_templater-0.2.9/workflow_templater/urlopen_jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,18 @@
     bad_cookies = False
     for _ in range(3):
         try:
             headers = {
                 'Content-Type': 'application/json',
             }
             if access_token is not None:
-                headers["Authorization"] = f"Bearer {access_token}"
+                if jira_base.endswith('atlassian.net'):
+                    headers["Authorization"] = f"Basic {access_token}"
+                else:
+                    headers["Authorization"] = f"Bearer {access_token}"
             elif user is not None:
                 headers['Cookie'] = get_cookie(keyring_service, user, jira_base=jira_base, overwrite=bad_cookies)
 
             res_obj = urlopen(
                 Request(
                     final_url,
                     data=json.dumps(data).encode() if data is not None else None,
```

### Comparing `workflow_templater-0.2.8/workflow_templater.egg-info/PKG-INFO` & `workflow_templater-0.2.9/workflow_templater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workflow-templater
-Version: 0.2.8
+Version: 0.2.9
 Summary: Template engine for (currently) Jira and Email. Uses yaml and jinja2. It helps you create multiple (possibly cross-linked) jira issues and emails from a template.
 Home-page: https://github.com/m-khvoinitsky/workflow-templater
 Author: Mikhail Khvoinitsky
 Author-email: me@khvoinitsky.org
 Keywords: jira email template workflow release
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

