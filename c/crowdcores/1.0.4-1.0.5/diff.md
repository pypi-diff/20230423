# Comparing `tmp/crowdcores-1.0.4.tar.gz` & `tmp/crowdcores-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-1.0.4.tar", last modified: Fri Apr 21 23:09:28 2023, max compression
+gzip compressed data, was "crowdcores-1.0.5.tar", last modified: Sun Apr 23 00:24:21 2023, max compression
```

## Comparing `crowdcores-1.0.4.tar` & `crowdcores-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.667064 crowdcores-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 23:09:28.667064 crowdcores-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-19 23:05:28.000000 crowdcores-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.663064 crowdcores-1.0.4/crowdcores/
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-19 23:02:37.000000 crowdcores-1.0.4/crowdcores/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-04-21 22:25:15.000000 crowdcores-1.0.4/crowdcores/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.667064 crowdcores-1.0.4/crowdcores.egg-info/
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 23:09:28.667064 crowdcores-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-21 23:09:11.000000 crowdcores-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:24:21.713662 crowdcores-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-23 00:24:21.713662 crowdcores-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      977 2023-04-23 00:23:36.000000 crowdcores-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:24:21.713662 crowdcores-1.0.5/crowdcores/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-19 23:02:37.000000 crowdcores-1.0.5/crowdcores/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-23 00:23:04.000000 crowdcores-1.0.5/crowdcores/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:24:21.713662 crowdcores-1.0.5/crowdcores.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-23 00:24:21.000000 crowdcores-1.0.5/crowdcores.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-23 00:24:21.000000 crowdcores-1.0.5/crowdcores.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 00:24:21.000000 crowdcores-1.0.5/crowdcores.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-23 00:24:21.000000 crowdcores-1.0.5/crowdcores.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-23 00:24:21.000000 crowdcores-1.0.5/crowdcores.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 00:24:21.713662 crowdcores-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-23 00:23:57.000000 crowdcores-1.0.5/setup.py
```

### Comparing `crowdcores-1.0.4/LICENSE.txt` & `crowdcores-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-1.0.4/crowdcores/pipeline.py` & `crowdcores-1.0.5/crowdcores/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,13 +22,7 @@
         x = requests.post(url, headers=headers, data=json_data)
         
         data=x.json()
         if data["success"] == 1:
             return data["pipeline_response_result"]
         if data["success"] == 0:
             raise getattr(__builtins__, data["exception_name"])(data["exception_message"])
-
-
-generator=crowdcores_pipeline('text-generation', model='gpt2');
-r=generator("how are you doing ", max_length=30, num_return_sequences=4)
-print(r)
-
```

