# Comparing `tmp/geomapdemo-0.1.4.tar.gz` & `tmp/geomapdemo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.1.4.tar", last modified: Mon Apr 17 03:13:06 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.5.tar", last modified: Sun Apr 23 04:12:57 2023, max compression
```

## Comparing `geomapdemo-0.1.4.tar` & `geomapdemo-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:12:57.848789 geomapdemo-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-23 04:12:57.848789 geomapdemo-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:12:57.844789 geomapdemo-0.1.5/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:12:57.848789 geomapdemo-0.1.5/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 04:12:57.000000 geomapdemo-0.1.5/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 04:12:57.848789 geomapdemo-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-23 04:12:44.000000 geomapdemo-0.1.5/setup.py
```

### Comparing `geomapdemo-0.1.4/LICENSE` & `geomapdemo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.4/PKG-INFO` & `geomapdemo-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,17 +19,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geomapdemo
 
 [![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+[![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
+[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
+![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
+![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
 
 **A python package for interactive mapping, testing.**
 
 
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.1.4/README.md` & `geomapdemo-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # geomapdemo
 
 [![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+[![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
+[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
+![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
+![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
 
 **A python package for interactive mapping, testing.**
 
 
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.1.4/geomapdemo/geomapdemo.py` & `geomapdemo-0.1.5/geomapdemo/geomapdemo.py`

 * *Files 23% similar despite different names*

```diff
@@ -229,22 +229,74 @@
         gdf = gpd.read_file(path)
         geojson = gdf.__geo_interface__
         self.add_geojson(geojson, name=name, **kwargs)
     
     def add_markers(self, center, draggable = False, **kwargs):
         """Adds markers to the map
         Args:
-            center (tuple): The center of the markers.
+            center (tuple| list): The center of the markers.
             draggable (bool, optional): Whether the markers are draggable. Defaults to False.
             **kwargs: Keyword arguments to be passed to the markers.
-        """        
-        marker = ipyleaflet.Marker(location=center, draggable= draggable, **kwargs)
-        self.add_layer(marker)
+        """ 
+        if isinstance(center, list):
+            center = tuple(center)
+        if isinstance(center, tuple):
+            marker = ipyleaflet.Marker(location=center, draggable= draggable, **kwargs)
+            self.add_layer(marker)
+        else:
+            raise TypeError("The center must be a tuple or a list")
 
+    def add_raster(self, url, name ='Raster', fit_bounds= True, **kwargs):
+        """Adds a raster to the map
+        Args:
+            url (str): The url of the raster.
+            name (str, optional): The name of the raster. Defaults to 'Raster'.
+            fit_bounds (bool, optional): Whether to fit the bounds of the raster. Defaults to True.
+            **kwargs: Keyword arguments to be passed to the raster.
+        """ 
+        import httpx
+        titiler_endpoint = "https://titiler.xyz"
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/info",
+            params = {
+                "url": url,
+            }
+        ).json()
+
+        bounds = r["bounds"]
+
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/tilejson.json",
+            params = {
+                "url": url,
+            }
+        ).json()
+
+        tile = r['tiles'][0]
+
+        self.add_tile_layer(url=tile, name=name, **kwargs)
+
+        if fit_bounds:
+            bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
+            self.fit_bounds(bbox)
 
+    def add_local_raster(self, filepath, **kwargs):
+        """Adds a local raster to the map
+        Args:
+            filepath (str): The path to the raster.
+            name (str, optional): The name of the raster. Defaults to 'Raster'.
+            **kwargs: Keyword arguments to be passed to the raster.
+        """ 
+        try:
+            from localtileserver import get_leaflet_tile_layer, TileClient
+            client = TileClient(filepath)
+            tile_layer = get_leaflet_tile_layer(client)
+            self.add_layer(tile_layer)
+        except:
+            raise ImportError("Please install localtileserver")
 
 
 
 def generate_random_string(length=10, upper=False, punctuations=False, digits=False):
     """Generates a random string of fixed length
 
     Args:
```

### Comparing `geomapdemo-0.1.4/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.5/geomapdemo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,17 +19,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geomapdemo
 
 [![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+[![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
+[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
+![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
+![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
 
 **A python package for interactive mapping, testing.**
 
 
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.1.4/setup.py` & `geomapdemo-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

