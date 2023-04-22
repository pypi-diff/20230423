# Comparing `tmp/psd_export-1.0.7.tar.gz` & `tmp/psd_export-1.0.8.tar.gz`

## Comparing `psd_export-1.0.7.tar` & `psd_export-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/blendfuncs.py
--rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/composite.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/export.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/filters.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/util.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.7/LICENSE
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.7/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/__init__.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/blendfuncs.py
+-rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/composite.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/export.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/filters.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/util.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.8/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.8/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.8/PKG-INFO
```

### Comparing `psd_export-1.0.7/.github/workflows/python-publish.yml` & `psd_export-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/src/psd_export/blendfuncs.py` & `psd_export-1.0.8/src/psd_export/blendfuncs.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/src/psd_export/composite.py` & `psd_export-1.0.8/src/psd_export/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from psd_tools.api.layers import Layer
 from psd_tools.constants import BlendMode, Clipping, Tag
 
 from . import blendfuncs
 from . import util
 from .util import peval
 
+dtype = np.float32
+
 class WrappedLayer():
     def __init__(self, layer:Layer, clip_layers=[], parent:WrappedLayer=None):
         self.layer:Layer = layer
         self.parent:WrappedLayer = parent
         self.name = layer.name
         self.visible = True if layer.kind == 'psdimage' else layer.visible
         self.custom_op = None
@@ -153,16 +155,16 @@
     flat_list = flattened_tree(layer)
     for sublayer in layer.descendants():
         sublayer.visibility_dependency = get_visibility_dependency(sublayer, possible_dependencies(sublayer, flat_list))
         if sublayer.custom_op is not None:
             sublayer.custom_op_barrier = asyncio.Barrier(tile_count)
             sublayer.custom_op_condition = asyncio.Condition()
             sublayer.custom_op_finished = False
-            sublayer.custom_op_color = np.zeros(size + (3,))
-            sublayer.custom_op_alpha = np.zeros(size + (1,))
+            sublayer.custom_op_color = np.zeros(size + (3,), dtype=dtype)
+            sublayer.custom_op_alpha = np.zeros(size + (1,), dtype=dtype)
 
 def increment_get_counter(counter, key):
     counter[key] += 1
 
 def decrement_get_counter(counter, cache, key):
     counter[key] -= 1
     if counter[key] == 0:
@@ -209,25 +211,25 @@
         sublayer.composite_cache.clear()
 
 def get_cached_layer_data(layer:WrappedLayer, channel):
     with layer.data_cache_lock:
         if channel not in layer.data_cache:
             data = layer.layer.numpy(channel)
             if data is not None:
-                data = data.astype(np.float64)
+                data = data.astype(dtype)
             layer.data_cache[channel] = data
             return data
         return layer.data_cache[channel]
 
 async def get_padded_data(layer:WrappedLayer, channel, size, offset, data_offset, fill=0.0):
     data = await peval(lambda: get_cached_layer_data(layer, channel))
     if data is None:
         return None
     shape = size + data.shape[2:]
-    pad = await peval(lambda: util.full(shape, fill))
+    pad = await peval(lambda: util.full(shape, fill, dtype=dtype))
     await peval(lambda: blit(pad, data, np.array(util.swap(data_offset)) - np.array(offset)))
     return pad
 
 def intersection(a, b):
     return (max(a[0], b[0]), max(a[1], b[1]), min(a[2], b[2]), min(a[3], b[3]))
 
 def is_intersecting(a, b):
@@ -254,15 +256,15 @@
 async def get_pixel_layer_data(layer:WrappedLayer, size, offset):
     if not has_tile_data(layer.layer, size, offset):
         return None, None
     if await is_zero_alpha(layer, size, offset):
         return None, None
     alpha_src = await get_padded_data(layer, 'shape', size, offset, layer.layer.offset)
     if alpha_src is None:
-        alpha_src = np.ones(size + (1,))
+        alpha_src = np.ones(size + (1,), dtype=dtype)
     color_src = await get_padded_data(layer, 'color', size, offset, layer.layer.offset)
     return color_src, alpha_src
 
 async def get_mask_data(layer:WrappedLayer, size, offset):
     mask = layer.layer.mask
     if mask and not mask.disabled:
         return await get_padded_data(layer, 'mask', size, offset, (mask.left, mask.top), mask.background_color / 255.0)
@@ -506,16 +508,16 @@
     `tile_size` is arranged by (height, width)
     '''
     size = psd.layer.height, psd.layer.width
     if count_mode:
         color = None
         alpha = None
     else:
-        color = np.zeros(size + (3,))
-        alpha = np.zeros(size + (1,))
+        color = np.zeros(size + (3,), dtype=dtype)
+        alpha = np.zeros(size + (1,), dtype=dtype)
 
     tiles = list(generate_tiles(size, tile_size))
     set_layer_extra_data(psd, len(tiles), size)
 
     async with asyncio.TaskGroup() as tg:
         for (tile_size, tile_offset) in tiles:
             if count_mode:
```

### Comparing `psd_export-1.0.7/src/psd_export/export.py` & `psd_export-1.0.8/src/psd_export/export.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/src/psd_export/filters.py` & `psd_export-1.0.8/src/psd_export/filters.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/src/psd_export/util.py` & `psd_export-1.0.8/src/psd_export/util.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/.gitignore` & `psd_export-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/LICENSE` & `psd_export-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/README.md` & `psd_export-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.7/pyproject.toml` & `psd_export-1.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psd-export"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
     { name = "cromachina" }
 ]
 license = { file = "LICENSE" }
 description = "Fast exporting of PSDs with [tagged] layers for variants."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `psd_export-1.0.7/PKG-INFO` & `psd_export-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psd-export
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fast exporting of PSDs with [tagged] layers for variants.
 Project-URL: Homepage, https://github.com/cromachina/psd-export
 Author: cromachina
 License: MIT License
         
         Copyright (c) 2022 cromachina
```

