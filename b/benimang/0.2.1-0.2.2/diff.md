# Comparing `tmp/benimang-0.2.1.tar.gz` & `tmp/benimang-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.2.1.tar", last modified: Sun Apr 23 09:52:59 2023, max compression
+gzip compressed data, was "benimang-0.2.2.tar", last modified: Sun Apr 23 11:00:56 2023, max compression
```

## Comparing `benimang-0.2.1.tar` & `benimang-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.876685 benimang-0.2.1/
--rw-rw-rw-   0        0        0       29 2022-09-20 03:37:30.000000 benimang-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-04-23 09:52:59.876685 benimang-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-09-20 03:37:30.000000 benimang-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.869685 benimang-0.2.1/beni/
--rw-rw-rw-   0        0        0        0 2022-09-20 06:33:04.000000 benimang-0.2.1/beni/__init__.py
--rw-rw-rw-   0        0        0     6223 2022-09-20 06:33:43.000000 benimang-0.2.1/beni/bbyte.py
--rw-rw-rw-   0        0        0     6312 2023-04-20 08:42:14.000000 benimang-0.2.1/beni/bcache.py
--rw-rw-rw-   0        0        0    10207 2023-04-23 09:51:57.000000 benimang-0.2.1/beni/bcmd.py
--rw-rw-rw-   0        0        0     1906 2022-09-20 03:37:31.000000 benimang-0.2.1/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-04-20 08:42:43.000000 benimang-0.2.1/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-04-21 01:32:03.000000 benimang-0.2.1/beni/bfile.py
--rw-rw-rw-   0        0        0     5009 2023-04-23 08:32:41.000000 benimang-0.2.1/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-04-21 01:32:29.000000 benimang-0.2.1/beni/bhttp.py
--rw-rw-rw-   0        0        0     2310 2023-04-23 08:04:15.000000 benimang-0.2.1/beni/binput.py
--rw-rw-rw-   0        0        0     5653 2023-04-20 09:28:08.000000 benimang-0.2.1/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-04-21 01:58:47.000000 benimang-0.2.1/beni/blog.py
--rw-rw-rw-   0        0        0     5585 2023-04-23 08:15:55.000000 benimang-0.2.1/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-04-21 01:24:20.000000 benimang-0.2.1/beni/bplaywright.py
--rw-rw-rw-   0        0        0      841 2023-02-27 04:00:30.000000 benimang-0.2.1/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-04-23 09:28:40.000000 benimang-0.2.1/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10553 2023-04-21 01:31:13.000000 benimang-0.2.1/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-04-21 02:20:59.000000 benimang-0.2.1/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2022-11-09 09:34:30.000000 benimang-0.2.1/beni/btable.py
--rw-rw-rw-   0        0        0     2941 2023-04-20 08:53:07.000000 benimang-0.2.1/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-02-28 02:25:16.000000 benimang-0.2.1/beni/btime.py
--rw-rw-rw-   0        0        0     2397 2023-04-23 07:11:54.000000 benimang-0.2.1/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.874685 benimang-0.2.1/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 09:52:59.000000 benimang-0.2.1/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-04-23 09:48:24.000000 benimang-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 09:52:59.876685 benimang-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 09:52:59.875685 benimang-0.2.1/test/
--rw-rw-rw-   0        0        0      638 2023-02-24 01:48:48.000000 benimang-0.2.1/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.717546 benimang-0.2.2/
+-rw-rw-rw-   0        0        0       29 2022-09-20 03:37:30.000000 benimang-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-04-23 11:00:56.717546 benimang-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:37:30.000000 benimang-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.710546 benimang-0.2.2/beni/
+-rw-rw-rw-   0        0        0        0 2022-09-20 06:33:04.000000 benimang-0.2.2/beni/__init__.py
+-rw-rw-rw-   0        0        0     6223 2022-09-20 06:33:43.000000 benimang-0.2.2/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6312 2023-04-20 08:42:14.000000 benimang-0.2.2/beni/bcache.py
+-rw-rw-rw-   0        0        0    10207 2023-04-23 09:51:57.000000 benimang-0.2.2/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1906 2022-09-20 03:37:31.000000 benimang-0.2.2/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-04-20 08:42:43.000000 benimang-0.2.2/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-04-21 01:32:03.000000 benimang-0.2.2/beni/bfile.py
+-rw-rw-rw-   0        0        0     5009 2023-04-23 08:32:41.000000 benimang-0.2.2/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-04-21 01:32:29.000000 benimang-0.2.2/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2310 2023-04-23 08:04:15.000000 benimang-0.2.2/beni/binput.py
+-rw-rw-rw-   0        0        0     5653 2023-04-20 09:28:08.000000 benimang-0.2.2/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-04-21 01:58:47.000000 benimang-0.2.2/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-04-23 10:53:28.000000 benimang-0.2.2/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-04-21 01:24:20.000000 benimang-0.2.2/beni/bplaywright.py
+-rw-rw-rw-   0        0        0      841 2023-02-27 04:00:30.000000 benimang-0.2.2/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-04-23 09:28:40.000000 benimang-0.2.2/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10553 2023-04-21 01:31:13.000000 benimang-0.2.2/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-04-21 02:20:59.000000 benimang-0.2.2/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2022-11-09 09:34:30.000000 benimang-0.2.2/beni/btable.py
+-rw-rw-rw-   0        0        0     2941 2023-04-20 08:53:07.000000 benimang-0.2.2/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-02-28 02:25:16.000000 benimang-0.2.2/beni/btime.py
+-rw-rw-rw-   0        0        0     2397 2023-04-23 07:11:54.000000 benimang-0.2.2/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.715548 benimang-0.2.2/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-04-23 10:55:35.000000 benimang-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 11:00:56.717546 benimang-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.716546 benimang-0.2.2/test/
+-rw-rw-rw-   0        0        0      638 2023-02-24 01:48:48.000000 benimang-0.2.2/test/test_sample.py
```

### Comparing `benimang-0.2.1/beni/bbyte.py` & `benimang-0.2.2/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bcache.py` & `benimang-0.2.2/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bcmd.py` & `benimang-0.2.2/beni/bcmd.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bcolor.py` & `benimang-0.2.2/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bexecute.py` & `benimang-0.2.2/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bfile.py` & `benimang-0.2.2/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bfunc.py` & `benimang-0.2.2/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bhttp.py` & `benimang-0.2.2/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/binput.py` & `benimang-0.2.2/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/block.py` & `benimang-0.2.2/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/blog.py` & `benimang-0.2.2/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bpath.py` & `benimang-0.2.2/beni/bpath.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,24 +210,26 @@
 
 @asynccontextmanager
 async def useTempFile():
     tempFile = getTempFile()
     try:
         yield tempFile
     finally:
-        _remove(tempFile)
+        await remove(tempFile)
 
 
 @asynccontextmanager
-async def useTempDir():
+async def useTempDir(isMakeDir: bool = False):
     tempDir = getTempDir()
+    if isMakeDir:
+        await make(tempDir)
     try:
         yield tempDir
     finally:
-        _remove(tempDir)
+        await remove(tempDir)
 
 
 @asynccontextmanager
 async def useDir(path: str | Path):
     path = Path(path)
     currentPath = os.getcwd()
     try:
```

### Comparing `benimang-0.2.1/beni/bplaywright.py` & `benimang-0.2.2/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bprogress.py` & `benimang-0.2.2/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bqiniu.py` & `benimang-0.2.2/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bsqlite.py` & `benimang-0.2.2/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bstorage.py` & `benimang-0.2.2/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/btable.py` & `benimang-0.2.2/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/btask.py` & `benimang-0.2.2/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/btime.py` & `benimang-0.2.2/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/beni/bzip.py` & `benimang-0.2.2/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/benimang.egg-info/SOURCES.txt` & `benimang-0.2.2/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.2.1/pyproject.toml` & `benimang-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "0.2.1"
+version = "0.2.2"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-0.2.1/test/test_sample.py` & `benimang-0.2.2/test/test_sample.py`

 * *Files identical despite different names*

