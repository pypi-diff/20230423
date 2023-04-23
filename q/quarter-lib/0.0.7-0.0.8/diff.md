# Comparing `tmp/quarter_lib-0.0.7.tar.gz` & `tmp/quarter_lib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarter_lib-0.0.7.tar", last modified: Tue Apr 18 10:02:24 2023, max compression
+gzip compressed data, was "quarter_lib-0.0.8.tar", last modified: Sun Apr 23 15:15:29 2023, max compression
```

## Comparing `quarter_lib-0.0.7.tar` & `quarter_lib-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.717182 quarter_lib-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.717182 quarter_lib-0.0.7/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.717182 quarter_lib-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.717182 quarter_lib-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.717182 quarter_lib-0.0.7/src/quarter_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/quarter_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/src/quarter_lib/akeyless/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/quarter_lib/akeyless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/quarter_lib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/src/quarter_lib/google/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/quarter_lib/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/src/quarter_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-18 10:02:14.000000 quarter_lib-0.0.7/src/quarter_lib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:24.721181 quarter_lib-0.0.7/src/quarter_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-18 10:02:24.000000 quarter_lib-0.0.7/src/quarter_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-18 10:02:24.000000 quarter_lib-0.0.7/src/quarter_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:02:24.000000 quarter_lib-0.0.7/src/quarter_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 10:02:24.000000 quarter_lib-0.0.7/src/quarter_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/akeyless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/akeyless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/top_level.txt
```

### Comparing `quarter_lib-0.0.7/.github/scripts/release.py` & `quarter_lib-0.0.8/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `quarter_lib-0.0.7/.gitignore` & `quarter_lib-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `quarter_lib-0.0.7/src/quarter_lib/akeyless/__init__.py` & `quarter_lib-0.0.8/src/quarter_lib/akeyless/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+import os
+
 import requests
-from dotenv import dotenv_values
+from dotenv import load_dotenv
 
-env_values = dotenv_values("cred.env")
+load_dotenv("cred.env")
 
 AUTH_URL = "https://api.akeyless.io/auth"
 SECRET_URL = "https://api.akeyless.io/get-secret-value"
 TARGET_URL = "https://api.akeyless.io/get-target-details"
 
 HEADERS = {
     "accept": "application/json",
     "content-type": "application/json"
 }
 
 
 def __get_token():
     token_response = requests.post(AUTH_URL, json={
         "access-type": "access_key",
-        "access-id": env_values['access_id'],
-        "access-key": env_values['access_key'],
+        "access-id": os.environ['access_id'],
+        "access-key": os.environ['access_key'],
     }, headers=HEADERS).json()
     return token_response['token']
 
 
 def get_secrets(secrets: list):
     payload = {
         "accessibility": "regular",
```

