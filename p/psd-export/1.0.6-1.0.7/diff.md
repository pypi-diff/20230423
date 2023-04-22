# Comparing `tmp/psd_export-1.0.6.tar.gz` & `tmp/psd_export-1.0.7.tar.gz`

## Comparing `psd_export-1.0.6.tar` & `psd_export-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/blendfuncs.py
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/composite.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/export.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/filters.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.6/src/psd_export/util.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.6/LICENSE
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.6/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/__init__.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/blendfuncs.py
+-rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/composite.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/export.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/filters.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.7/src/psd_export/util.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.7/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.7/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.7/PKG-INFO
```

### Comparing `psd_export-1.0.6/.github/workflows/python-publish.yml` & `psd_export-1.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/src/psd_export/blendfuncs.py` & `psd_export-1.0.7/src/psd_export/blendfuncs.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/src/psd_export/composite.py` & `psd_export-1.0.7/src/psd_export/composite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import pathlib
 import threading
+from collections import Counter
 
 import cv2
 import numpy as np
 from psd_tools import PSDImage
 from psd_tools.api.layers import Layer
 from psd_tools.constants import BlendMode, Clipping, Tag
 
@@ -16,27 +17,25 @@
 
 class WrappedLayer():
     def __init__(self, layer:Layer, clip_layers=[], parent:WrappedLayer=None):
         self.layer:Layer = layer
         self.parent:WrappedLayer = parent
         self.name = layer.name
         self.visible = True if layer.kind == 'psdimage' else layer.visible
-        self.skip = False
         self.custom_op = None
         self.children:list[WrappedLayer] = []
         self.flat_children:list[WrappedLayer] = []
         self.clip_layers:list[WrappedLayer] = clip_layers
         self.composite_cache = {}
+        self.composite_cache_counter = Counter()
         self.data_cache = {}
         self.data_cache_lock = threading.Lock()
+        self.data_cache_counter = 0
         self.tags = []
         self.visibility_dependency = None
-        self.tag_dependency = None
-        self.cache_hit = ''
-        self.worker_counter = 0
 
         if self.layer.is_group():
             for sublayer, sub_clip_layers in get_layer_and_clip_groupings(self.layer):
                 sub_clip_layers = [WrappedLayer(s, parent=self) for s in sub_clip_layers]
                 sublayer = WrappedLayer(sublayer, sub_clip_layers, self)
                 self.children.append(sublayer)
                 self.flat_children.append(sublayer)
@@ -120,83 +119,98 @@
         if sublayer == layer:
             found = True
         if found:
             get_visibility_all_children(sublayer, visited, visit_all)
     if layer.parent.parent != None and layer.parent.layer.blend_mode == BlendMode.PASS_THROUGH:
         get_visibility_dependency_sub(layer.parent, visited, visit_all)
 
-def get_visibility_dependency(layer:WrappedLayer, visit_all=False):
+def get_visibility_dependency(layer:WrappedLayer, possible_deps, visit_all=False):
     visited = set()
     get_visibility_dependency_sub(layer, visited, visit_all)
+    visited = visited.intersection(possible_deps)
     return frozenset(visited)
 
+def flattened_tree(psd:WrappedLayer):
+    flat_list = []
+    def sub(layer):
+        for sublayer in layer.flat_children:
+            sub(sublayer)
+        flat_list.append(layer)
+    sub(psd)
+    return flat_list
+
+def possible_dependencies(layer:WrappedLayer, flat_list):
+    v = set()
+    for sublayer in flat_list:
+        v.add(sublayer)
+        if sublayer == layer:
+            break
+    for clip in layer.clip_layers:
+        for sublayer in clip.descendants():
+            v.add(clip)
+    return v
+
 def set_layer_extra_data(layer:WrappedLayer, tile_count, size):
-    set_tag_dependency(layer)
+    flat_list = flattened_tree(layer)
     for sublayer in layer.descendants():
-        sublayer.worker_counter = tile_count
-        sublayer.cache_hit = ''
-        sublayer.visibility_dependency = get_visibility_dependency(sublayer)
+        sublayer.visibility_dependency = get_visibility_dependency(sublayer, possible_dependencies(sublayer, flat_list))
         if sublayer.custom_op is not None:
             sublayer.custom_op_barrier = asyncio.Barrier(tile_count)
             sublayer.custom_op_condition = asyncio.Condition()
             sublayer.custom_op_finished = False
             sublayer.custom_op_color = np.zeros(size + (3,))
             sublayer.custom_op_alpha = np.zeros(size + (1,))
 
-def get_tile_cache(layer:WrappedLayer, offset):
-    if offset not in layer.composite_cache:
-        layer.composite_cache[offset] = {}
-    return layer.composite_cache[offset]
+def increment_get_counter(counter, key):
+    counter[key] += 1
+
+def decrement_get_counter(counter, cache, key):
+    counter[key] -= 1
+    if counter[key] == 0:
+        if key in cache:
+            del cache[key]
+    elif counter[key] < 0:
+        pass
+
+def inc_composite_cache(layer:WrappedLayer):
+    increment_get_counter(layer.composite_cache_counter, layer.visibility_dependency)
+
+def dec_composite_cache(layer:WrappedLayer):
+    decrement_get_counter(layer.composite_cache_counter, layer.composite_cache, layer.visibility_dependency)
+
+def is_counter_zero(layer:WrappedLayer):
+    return layer.composite_cache_counter[layer.visibility_dependency] <= 0
+
+def inc_data_cache(layer:WrappedLayer):
+    layer.data_cache_counter += 1
+
+def dec_data_cache(layer:WrappedLayer):
+    layer.data_cache_counter -= 1
+    if layer.data_cache_counter == 0:
+        layer.data_cache.clear()
+    if layer.data_cache_counter < 0:
+        pass
+
+def get_tile_cache(layer:WrappedLayer, key):
+    if key not in layer.composite_cache:
+        layer.composite_cache[key] = {}
+    return layer.composite_cache[key]
 
 def get_cached_composite(layer:WrappedLayer, offset):
-    return get_tile_cache(layer, offset).get(layer.visibility_dependency, None)
+    return get_tile_cache(layer, layer.visibility_dependency).get(offset, None)
 
 def set_cached_composite(layer:WrappedLayer, offset, tile_data):
     for data in tile_data:
         if not np.isscalar(data):
             data.flags.writeable = False
-    get_tile_cache(layer, offset)[layer.visibility_dependency] = tile_data
-
-def clear_all_caches(layer:WrappedLayer):
-    layer.composite_cache.clear()
-    layer.data_cache.clear()
-    for sublayer in layer.descendants():
-        sublayer.composite_cache.clear()
-        sublayer.data_cache.clear()
+    get_tile_cache(layer, layer.visibility_dependency)[offset] = tile_data
 
-def clear_descendants_caches(layer:WrappedLayer):
+def clear_count_mode(layer:WrappedLayer):
     for sublayer in layer.descendants():
         sublayer.composite_cache.clear()
-        sublayer.data_cache.clear()
-
-def set_tag_dependency(layer:WrappedLayer):
-    for sublayer in layer.descendants():
-        if sublayer.tag_dependency is None:
-            v = get_visibility_dependency(sublayer, True)
-            sublayer.tag_dependency = False
-            for v_layer in v:
-                tags = [not tag.ignore for tag in v_layer.tags]
-                if any(tags):
-                    sublayer.tag_dependency = True
-                    break
-
-def set_skip_to_last_untagged(layer:WrappedLayer):
-    skip = False
-    for child in reversed(layer.children):
-        if not child.tag_dependency and not skip:
-            skip = True
-            continue
-        if skip and child.composite_cache:
-            child.skip = True
-            child.data_cache.clear()
-            child.composite_cache.clear()
-
-def set_skips(layer:WrappedLayer):
-    for sublayer in layer.descendants():
-        set_skip_to_last_untagged(sublayer)
 
 def get_cached_layer_data(layer:WrappedLayer, channel):
     with layer.data_cache_lock:
         if channel not in layer.data_cache:
             data = layer.layer.numpy(channel)
             if data is not None:
                 data = data.astype(np.float64)
@@ -296,30 +310,28 @@
         color_dst, alpha_dst = backdrop
     else:
         color_dst = 0.0
         alpha_dst = 0.0
 
     sublayer:WrappedLayer
     for sublayer in layer:
-        try:
-            if not sublayer.visible or sublayer.skip:
-                if sublayer.custom_op is not None:
-                    await barrier_skip(sublayer.custom_op_barrier)
-                continue
+        if not sublayer.visible:
+            if sublayer.custom_op is not None:
+                await barrier_skip(sublayer.custom_op_barrier)
+            continue
 
-            cached_composite = get_cached_composite(sublayer, offset)
-            if cached_composite is not None:
-                color_dst, alpha_dst = cached_composite
-                sublayer.cache_hit = True
-                if sublayer.custom_op is not None:
-                    await barrier_skip(sublayer.custom_op_barrier)
-                continue
-            else:
-                sublayer.cache_hit = False
+        cached_composite = get_cached_composite(sublayer, offset)
+        dec_composite_cache(sublayer)
+        if cached_composite is not None:
+            color_dst, alpha_dst = cached_composite
+            if sublayer.custom_op is not None:
+                await barrier_skip(sublayer.custom_op_barrier)
+            continue
 
+        try:
             blend_mode = sublayer.layer.blend_mode
 
             if sublayer.layer.is_group():
                 next_backdrop = None
                 if blend_mode == BlendMode.PASS_THROUGH:
                     next_backdrop = (color_dst, alpha_dst)
                 color_src, alpha_src = await composite_group_layer(sublayer, size, offset, next_backdrop)
@@ -411,20 +423,18 @@
                     color_dst = color_src
 
                 # Finally we can intersect the mask with the alpha_src and blend the alpha_dst together.
                 if mask_src is not None:
                     await peval(lambda: np.multiply(alpha_src, mask_src, out=alpha_src))
                 alpha_dst = await peval(lambda: blendfuncs.normal_alpha(alpha_dst, alpha_src))
 
-            set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
+            if not is_counter_zero(sublayer):
+                set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
         finally:
-            sublayer.worker_counter -= 1
-            if sublayer.worker_counter == 0 and not sublayer.tag_dependency:
-                sublayer.data_cache.clear()
-                clear_descendants_caches(sublayer)
+            dec_data_cache(sublayer)
 
     if np.isscalar(color_dst):
         return None, None
 
     return color_dst.copy(), alpha_dst.copy()
 
 debug_path = pathlib.Path('')
@@ -454,26 +464,63 @@
         while x < width:
             size_y = min(tile_height, height - y)
             size_x = min(tile_width, width - x)
             yield ((size_y, size_x), (y, x))
             x += tile_width
         y += tile_height
 
-async def composite(psd:WrappedLayer, tile_size=(256,256)):
+async def has_alpha(layer, size, offset):
+    if not has_tile_data(layer.layer, size, offset):
+        return False
+    if await is_zero_alpha(layer, size, offset):
+        return False
+    return True
+
+# Partially simulate compositing. This should match the recursive structure of composite_layers.
+# This could be inlined into composite_layers, but it starts to get very messy.
+async def count_tile(layer:WrappedLayer, size, offset):
+    alpha_dst = False
+    for sublayer in layer:
+        if not sublayer.visible:
+            continue
+        inc_composite_cache(sublayer)
+        if get_cached_composite(sublayer, offset) is not None:
+            continue
+        if sublayer.layer.is_group():
+            alpha_src = await count_tile(sublayer, size, offset)
+        else:
+            alpha_src = await has_alpha(sublayer, size, offset)
+        inc_data_cache(sublayer)
+        if alpha_src == False:
+            set_cached_composite(sublayer, offset, (0, 0))
+            await count_tile(sublayer.clip_layers, size, offset)
+            continue
+        if sublayer.layer.blend_mode != BlendMode.PASS_THROUGH:
+            await count_tile(sublayer.clip_layers, size, offset)
+        set_cached_composite(sublayer, offset, (1, 1))
+        alpha_dst = alpha_src
+    return alpha_dst
+
+async def composite(psd:WrappedLayer, tile_size=(256,256), count_mode=False):
     '''
     Composite the given PSD and return color (RGB) and alpha arrays.
     `tile_size` is arranged by (height, width)
     '''
     size = psd.layer.height, psd.layer.width
-    color = np.zeros(size + (3,))
-    alpha = np.zeros(size + (1,))
+    if count_mode:
+        color = None
+        alpha = None
+    else:
+        color = np.zeros(size + (3,))
+        alpha = np.zeros(size + (1,))
 
     tiles = list(generate_tiles(size, tile_size))
     set_layer_extra_data(psd, len(tiles), size)
 
     async with asyncio.TaskGroup() as tg:
         for (tile_size, tile_offset) in tiles:
-            tg.create_task(composite_tile(psd, tile_size, tile_offset, color, alpha))
-
-    set_skips(psd)
+            if count_mode:
+                tg.create_task(count_tile(psd, tile_size, tile_offset))
+            else:
+                tg.create_task(composite_tile(psd, tile_size, tile_offset, color, alpha))
 
     return color, alpha
```

### Comparing `psd_export-1.0.6/src/psd_export/export.py` & `psd_export-1.0.7/src/psd_export/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     if config.subfolders:
         next_file_name = base_file_name.with_stem(f'{base_file_name.stem}{primary_tag}')
         next_file_name = next_file_name.parent / group_name / next_file_name.name
     else:
         next_file_name = base_file_name.with_stem(f'{base_file_name.stem}{primary_tag}-{group_name}')
     return next_file_name
 
-async def export_variant(psd, file_name, config, enabled_tags):
+async def export_variant(psd, file_name, config, enabled_tags, count_mode):
     export_name = compute_file_name(file_name, config, enabled_tags)
 
-    if config.dryrun:
+    if config.dryrun and not count_mode:
         logging.info(f'would export: {export_name}')
         return
 
     # Configure tagged layers
     for layer in psd.descendants():
         custom_ops = []
         def add_op(tag):
@@ -88,45 +88,47 @@
             if tag.ignore:
                 add_op(tag)
             elif (tag.name, tag.xor_group) in enabled_tags:
                 layer.visible = True
                 add_op(tag)
         layer.custom_op = filters.compose_ops(custom_ops)
 
-    image = await composite.composite(psd)
+    image = await composite.composite(psd, count_mode=count_mode)
+
+    if count_mode:
+        return
 
     export_name.parent.mkdir(parents=True, exist_ok=True)
     util.save_file(export_name, image, [cv2.IMWRITE_PNG_COMPRESSION, config.png_compression, cv2.IMWRITE_JPEG_QUALITY, config.jpg_quality])
 
-async def export_combinations(psd, file_name, config, secondary_tags, enabled_tags):
+async def export_combinations(psd, file_name, config, secondary_tags, enabled_tags, count_mode):
     if not secondary_tags:
         return
 
     items = list(secondary_tags.items())
     items.sort()
 
     for xor_group, tags in items:
         secondary_tags = secondary_tags.remove(xor_group)
         for tag in tags:
             next_enabled = enabled_tags.append((tag, xor_group))
-            await export_variant(psd, file_name, config, next_enabled)
-            await export_combinations(psd, file_name, config, secondary_tags, next_enabled)
+            await export_variant(psd, file_name, config, next_enabled, count_mode)
+            await export_combinations(psd, file_name, config, secondary_tags, next_enabled, count_mode)
 
 def get_least_tagged_layer(layer_map):
     lowest = None
     for pair in layer_map.items():
         if lowest is None or len(pair[1]) < len(lowest[1]):
             lowest = pair
-    return lowest
+    return lowest[1]
 
-def remove_tag_and_clear_cache(layer_map, tag):
+def remove_tag(layer_map, tag):
     for layer, tags in layer_map.items():
         tags = tags.discard(tag)
         if not tags:
-            composite.clear_all_caches(layer)
             layer_map = layer_map.discard(layer)
         else:
             layer_map = layer_map.set(layer, tags)
     return layer_map
 
 def is_reachable(layer:composite.WrappedLayer):
     while layer is not None:
@@ -138,62 +140,76 @@
 async def export_all_variants(file_name, config):
     psd = composite.PSDOpen(file_name)
 
     file_name = pathlib.Path(file_name).with_suffix(f'.{config.output_type}')
 
     primary_layers = pmap()
     secondary_tags = pmap()
+    primary_filter = config.primary_filter.split()
+    secondary_filter = config.secondary_filter.split()
 
     for layer in psd.descendants():
         tags = parse_tags(layer.name)
         layer.tags = tags
 
     for layer in psd.descendants():
         if not is_reachable(layer):
             continue
         for tag in layer.tags:
             if tag.ignore:
                 continue
             if tag.xor_group is None:
-                s = primary_layers.get(layer, pset()).add(tag.name)
-                primary_layers = primary_layers.set(layer, s)
+                if not primary_filter or tag.name in primary_filter:
+                    s = primary_layers.get(layer, pset()).add(tag.name)
+                    primary_layers = primary_layers.set(layer, s)
             else:
-                group = secondary_tags.get(tag.xor_group, pset()).add(tag.name)
-                secondary_tags = secondary_tags.set(tag.xor_group, group)
+                if not secondary_filter or tag.name in secondary_filter:
+                    group = secondary_tags.get(tag.xor_group, pset()).add(tag.name)
+                    secondary_tags = secondary_tags.set(tag.xor_group, group)
 
     if not primary_layers:
         primary_layers = primary_layers.set(psd, pset(['']))
 
+    primary_tags = []
     while primary_layers:
-        _, tags = get_least_tagged_layer(primary_layers)
+        tags = get_least_tagged_layer(primary_layers)
         primary_tag = next(iter(tags))
-        enabled = pvector([(primary_tag, None)])
-        if not config.only_secondary_tags:
-            await export_variant(psd, file_name, config, enabled)
-        await export_combinations(psd, file_name, config, secondary_tags, enabled)
-        primary_layers = remove_tag_and_clear_cache(primary_layers, primary_tag)
+        primary_tags.append(primary_tag)
+        primary_layers = remove_tag(primary_layers, primary_tag)
+
+    for count_mode in [True, False]:
+        for primary_tag in primary_tags:
+            enabled = pvector([(primary_tag, None)])
+            if not config.only_secondary_tags:
+                await export_variant(psd, file_name, config, enabled, count_mode)
+            await export_combinations(psd, file_name, config, secondary_tags, enabled, count_mode)
+        composite.clear_count_mode(psd)
 
 arg_parser = argparse.ArgumentParser()
 arg_parser.add_argument('--subfolders', action=argparse.BooleanOptionalAction, default=True,
     help='Export secondary tags to subfolders.')
 arg_parser.add_argument('--primary-sub', action=argparse.BooleanOptionalAction, default=False,
     help='Make primary tags into subfolders.')
 arg_parser.add_argument('--dryrun', action=argparse.BooleanOptionalAction, default=False,
     help='Show what files would have been exported, but do not actually export anything.')
 arg_parser.add_argument('--only-secondary-tags', action=argparse.BooleanOptionalAction, default=False,
     help='Only export secondary tags. This is useful for when exporting a primary tag by itself does not produce a meaningful picture.')
+arg_parser.add_argument('--primary-filter', default="", type=str,
+    help='Only export primary tags matching the given names.')
+arg_parser.add_argument('--secondary-filter', default="", type=str,
+    help='Only export secondary tags matching the given names.')
 arg_parser.add_argument('--mosaic-factor', default=filters.mosaic_factor_default, type=float,
     help='Set the mosaic proportion factor of censors, based on the minimum image dimension.')
 arg_parser.add_argument('--png-compression', default=1, type=int,
     help='Set the compression level for PNG output (0 to 9).')
 arg_parser.add_argument('--jpg-quality', default=95, type=int,
     help='Set the quality level for JPG output (0 to 100).')
-arg_parser.add_argument('--output-type', type=str, default='png',
+arg_parser.add_argument('--output-type', default='png', type=str,
     help='Output type, whatever is supported by OpenCV, for example: png, jpg, webp, tiff.')
-arg_parser.add_argument('--file-name', type=str, default='*.psd',
+arg_parser.add_argument('--file-name',  default='*.psd', type=str,
     help='PSD files to process; can use a glob pattern.')
 
 async def async_main():
     logging.basicConfig(level=logging.INFO)
     args = arg_parser.parse_args()
     filters.mosaic_factor_default = args.mosaic_factor
     start = time.perf_counter()
```

### Comparing `psd_export-1.0.6/src/psd_export/filters.py` & `psd_export-1.0.7/src/psd_export/filters.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/src/psd_export/util.py` & `psd_export-1.0.7/src/psd_export/util.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/.gitignore` & `psd_export-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/LICENSE` & `psd_export-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/README.md` & `psd_export-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.6/pyproject.toml` & `psd_export-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psd-export"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name = "cromachina" }
 ]
 license = { file = "LICENSE" }
 description = "Fast exporting of PSDs with [tagged] layers for variants."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `psd_export-1.0.6/PKG-INFO` & `psd_export-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psd-export
-Version: 1.0.6
+Version: 1.0.7
 Summary: Fast exporting of PSDs with [tagged] layers for variants.
 Project-URL: Homepage, https://github.com/cromachina/psd-export
 Author: cromachina
 License: MIT License
         
         Copyright (c) 2022 cromachina
```

