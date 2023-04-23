# Comparing `tmp/wsiserver-1.0.0.tar.gz` & `tmp/wsiserver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsiserver-1.0.0.tar", last modified: Sat Apr 22 01:06:35 2023, max compression
+gzip compressed data, was "wsiserver-1.0.1.tar", last modified: Sun Apr 23 02:51:13 2023, max compression
```

## Comparing `wsiserver-1.0.0.tar` & `wsiserver-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-22 01:06:35.779836 wsiserver-1.0.0/
--rw-r--r--   0 takumi     (501) staff       (20)    11357 2023-04-19 13:54:50.000000 wsiserver-1.0.0/LICENSE
--rw-r--r--   0 takumi     (501) staff       (20)    13575 2023-04-22 01:06:35.779149 wsiserver-1.0.0/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      325 2023-04-20 02:57:31.000000 wsiserver-1.0.0/README.md
--rw-r--r--   0 takumi     (501) staff       (20)      677 2023-04-22 01:03:50.000000 wsiserver-1.0.0/pyproject.toml
--rw-r--r--   0 takumi     (501) staff       (20)       38 2023-04-22 01:06:35.780161 wsiserver-1.0.0/setup.cfg
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-22 01:06:35.773538 wsiserver-1.0.0/src/
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-22 01:06:35.775899 wsiserver-1.0.0/src/wsiserver/
--rw-r--r--   0 takumi     (501) staff       (20)       22 2023-04-19 13:57:59.000000 wsiserver-1.0.0/src/wsiserver/__init__.py
--rw-r--r--   0 takumi     (501) staff       (20)     2290 2023-04-20 14:30:00.000000 wsiserver-1.0.0/src/wsiserver/app.py
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-22 01:06:35.778449 wsiserver-1.0.0/src/wsiserver.egg-info/
--rw-r--r--   0 takumi     (501) staff       (20)    13575 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      303 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/SOURCES.txt
--rw-r--r--   0 takumi     (501) staff       (20)        1 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/dependency_links.txt
--rw-r--r--   0 takumi     (501) staff       (20)       49 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/entry_points.txt
--rw-r--r--   0 takumi     (501) staff       (20)       40 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/requires.txt
--rw-r--r--   0 takumi     (501) staff       (20)       10 2023-04-22 01:06:35.000000 wsiserver-1.0.0/src/wsiserver.egg-info/top_level.txt
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-23 02:51:13.907863 wsiserver-1.0.1/
+-rw-r--r--   0 takumi     (501) staff       (20)    11357 2023-04-19 13:54:50.000000 wsiserver-1.0.1/LICENSE
+-rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-04-23 02:51:13.907429 wsiserver-1.0.1/PKG-INFO
+-rw-r--r--   0 takumi     (501) staff       (20)      326 2023-04-22 01:08:13.000000 wsiserver-1.0.1/README.md
+-rw-r--r--   0 takumi     (501) staff       (20)      677 2023-04-22 01:03:50.000000 wsiserver-1.0.1/pyproject.toml
+-rw-r--r--   0 takumi     (501) staff       (20)       38 2023-04-23 02:51:13.907954 wsiserver-1.0.1/setup.cfg
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-23 02:51:13.902479 wsiserver-1.0.1/src/
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-23 02:51:13.904476 wsiserver-1.0.1/src/wsiserver/
+-rw-r--r--   0 takumi     (501) staff       (20)       22 2023-04-23 02:50:41.000000 wsiserver-1.0.1/src/wsiserver/__init__.py
+-rw-r--r--   0 takumi     (501) staff       (20)     2306 2023-04-23 02:48:32.000000 wsiserver-1.0.1/src/wsiserver/app.py
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-23 02:51:13.906972 wsiserver-1.0.1/src/wsiserver.egg-info/
+-rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/PKG-INFO
+-rw-r--r--   0 takumi     (501) staff       (20)      303 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 takumi     (501) staff       (20)        1 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       49 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/entry_points.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       40 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/requires.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       10 2023-04-23 02:51:13.000000 wsiserver-1.0.1/src/wsiserver.egg-info/top_level.txt
```

### Comparing `wsiserver-1.0.0/LICENSE` & `wsiserver-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.0/PKG-INFO` & `wsiserver-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.0
+Version: 1.0.1
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,10 +214,10 @@
 Very simple wsi patching server
 
 # installation
 - install [openslide](https://openslide.org/download/)
   - e.g.: `apt-get install openslide-tools` (Ubuntu)
 - `pip install git+https://github.com/tand826/wsiserver`
 
-# run with sample viewer
+# run with example viewer
 1. run `wsiserver [wsi path]`
 2. open `example/index.html` in web browser
```

### Comparing `wsiserver-1.0.0/pyproject.toml` & `wsiserver-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.0/src/wsiserver/app.py` & `wsiserver-1.0.1/src/wsiserver/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,12 +69,12 @@
         tile = canvas
     buf = BytesIO()
     tile.save(buf, "png", quality=70)
     return Response(content=buf.getvalue(), media_type="image/png")
 
 
 def main():
-    uvicorn.run("wsiserver.app:app", port=args.port, log_level="info")
+    uvicorn.run("wsiserver.app:app", host="0.0.0.0", port=args.port, log_level="info")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wsiserver-1.0.0/src/wsiserver.egg-info/PKG-INFO` & `wsiserver-1.0.1/src/wsiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.0
+Version: 1.0.1
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,10 +214,10 @@
 Very simple wsi patching server
 
 # installation
 - install [openslide](https://openslide.org/download/)
   - e.g.: `apt-get install openslide-tools` (Ubuntu)
 - `pip install git+https://github.com/tand826/wsiserver`
 
-# run with sample viewer
+# run with example viewer
 1. run `wsiserver [wsi path]`
 2. open `example/index.html` in web browser
```

