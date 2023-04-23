# Comparing `tmp/longalpha_utils-0.40.tar.gz` & `tmp/longalpha_utils-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.40.tar", last modified: Tue Apr 11 15:18:41 2023, max compression
+gzip compressed data, was "longalpha_utils-0.41.tar", last modified: Sun Apr 23 15:45:38 2023, max compression
```

## Comparing `longalpha_utils-0.40.tar` & `longalpha_utils-0.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 15:18:41.233597 longalpha_utils-0.40/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:18:41.233597 longalpha_utils-0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-11 15:18:29.000000 longalpha_utils-0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 15:45:38.880103 longalpha_utils-0.41/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:45:38.880103 longalpha_utils-0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-23 15:45:25.000000 longalpha_utils-0.41/setup.py
```

### Comparing `longalpha_utils-0.40/longalpha_utils/messenger.py` & `longalpha_utils-0.41/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.40/longalpha_utils/transfers.py` & `longalpha_utils-0.41/longalpha_utils/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,19 @@
             index: whether to save the index of the dataframe, only used for parquet
 
 
         Returns:
 
         """
         with tempfile.TemporaryDirectory() as temp_dir:
-            path = os.path.join(temp_dir, object_name)
             if file_format == "parquet":
+                path = os.path.join(temp_dir, "file.parquet")
                 dataframe.to_parquet(path, index=index)
             elif file_format == "pickle":
+                path = os.path.join(temp_dir, "file.pkl")
                 dataframe.to_pickle(path)
             else:
                 raise ValueError("Incorrect file format")
             self.fput(file_path=path, bucket_name=bucket_name, object_name=object_name)
 
     def fget(self, file_path: str, bucket_name: str, object_name: str):
         self.minio_client.fget_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
@@ -91,15 +92,15 @@
         file.close()
         file.release_conn()
         return res
 
     def get_latest(self, bucket_name: str, file_format: str) -> pd.DataFrame:
         """
         get the latest parquet file and read it into pandas. Note that this does not include files in the
-        sub-folders of the bucket.
+        sub-folders of the bucket. To do this, we need to recursively list all the files in the bucket.
         Args:
             bucket_name: bucket_name: Minio bucket_name
             file_format: parquet or pickle
 
         Returns: A pandas dataframe
 
         """
```

### Comparing `longalpha_utils-0.40/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.41/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.40/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.41/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.40/setup.py` & `longalpha_utils-0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.40",
+    version="0.41",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

