# Comparing `tmp/wafermap-0.2.3.tar.gz` & `tmp/wafermap-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-0.2.3.tar", max compression
+gzip compressed data, was "wafermap-0.2.4.tar", max compression
```

## Comparing `wafermap-0.2.3.tar` & `wafermap-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.3/LICENSE
--rw-r--r--   0        0        0      897 2023-04-20 07:24:42.616048 wafermap-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7982 2023-04-19 13:29:46.122469 wafermap-0.2.3/README.md
--rw-r--r--   0        0        0      171 2023-04-19 10:42:08.837188 wafermap-0.2.3/wafermap/__init__.py
--rw-r--r--   0        0        0     3033 2023-04-17 22:16:54.410477 wafermap-0.2.3/wafermap/utils.py
--rw-r--r--   0        0        0    26571 2023-04-20 07:18:47.386306 wafermap-0.2.3/wafermap/wafermap.py
--rw-r--r--   0        0        0     8633 1970-01-01 00:00:00.000000 wafermap-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-10-23 17:45:58.152508 wafermap-0.2.4/LICENSE
+-rw-r--r--   0        0        0      901 2023-04-23 08:42:29.378279 wafermap-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8086 2023-04-23 08:34:39.102338 wafermap-0.2.4/README.md
+-rw-r--r--   0        0        0      171 2023-04-21 18:46:19.843838 wafermap-0.2.4/wafermap/__init__.py
+-rw-r--r--   0        0        0     3134 2023-04-21 18:46:19.843838 wafermap-0.2.4/wafermap/utils.py
+-rw-r--r--   0        0        0    26854 2023-04-23 08:43:21.523769 wafermap-0.2.4/wafermap/wafermap.py
+-rw-r--r--   0        0        0     8689 1970-01-01 00:00:00.000000 wafermap-0.2.4/PKG-INFO
```

### Comparing `wafermap-0.2.3/LICENSE` & `wafermap-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021, Sotiris Thomas
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021, Sotiris Thomas
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `wafermap-0.2.3/pyproject.toml` & `wafermap-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "wafermap"
-version = "0.2.3"
+version = "0.2.4"
 description = "A python package to plot maps of semiconductor wafers."
-authors = ["Sotiris Thomas <sothomas88@gmail.com>"]
+authors = ["cap1tan"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/cap1tan/wafermap"
 keywords = ["semiconductor", "wafer", "layout", "plot"]
+include = [
+    "LICENSE",
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 folium = "^0.14.0"
 branca = "^0.6.0"
 Pillow = "^9.5.0"
 numpy = "^1.24.2"
-selenium = "^4.8.3"
+html2image = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = {version = "^6.0.0", python = ">=3.8.1"}
 flake8-docstrings = "^1.7.0"
 pytest = "^7.3.1"
```

### Comparing `wafermap-0.2.3/README.md` & `wafermap-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Wafermap
 
-[![image](https://img.shields.io/pypi/v/wafermap.svg)](https://pypi.python.org/pypi/wafermap)
-[![image](https://img.shields.io/pypi/pyversions/wafermap.svg)](https://pypi.python.org/pypi/wafermap)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[
+![pypi](https://img.shields.io/pypi/v/wafermap.svg)
+![pypi](https://img.shields.io/pypi/pyversions/wafermap.svg)
+![pypi](https://img.shields.io/github/license/cap1tan/wafermap.svg)
+](https://pypi.org/project/wafermap/)
+[
+![GitHub](https://img.shields.io/github/v/release/cap1tan/wafermap?include_prereleases)
+![GitHub](https://img.shields.io/github/languages/code-size/cap1tan/wafermap)
+![pypi](https://img.shields.io/badge/linting-pylint-yellowgreen)
+](https://github.com/cap1tan/wafermap)
+
 
 
 A python package to plot maps of semiconductor wafers.
 
 Free software: MIT license
 
 
@@ -15,15 +23,15 @@
 * Circular wafers with arbitrary notch orientations.
 * Edge-exclusion and grids with optional margin.
 * Hover-able points, vectors and images.
 * Tooltips with embeddable images.
 * Individual labels and colors for each die.
 * Toggle layers on/off individually.
 * Export zoom-able maps to HTML.
-* Export PNG images with selenium
+* Export PNG images (needs Chromium)
 
 
 ## Examples
 
 - See the full dynamic maps [here](https://cap1tan.github.io/wafermap/)!
 
 - Static png image, just to get a taste:
@@ -68,74 +76,74 @@
 
 ```python
     import wafermap
 ```
 
 First let's define a Wafermap:
 ```python
-wm = wafermap.WaferMap(wafer_radius=100e-3,             # all length dimensions in meters
-                       cell_size=(10e-3, 20e-3),        # (sizeX, sizeY)
-                       cell_margin=(8e-3, 15e-3),       # distance between cell borders (x, y)
-                       grid_offset=(-2.05e-3, -4.1e-3), # grid offset in (x, y)
-                       edge_exclusion=2.2e-3,           # margin from the wafer edge where a red edge exclusion ring is drawn
+wm = wafermap.WaferMap(wafer_radius=100,                # all length dimensions in mm
+                       cell_size=(10, 20),              # (sizeX, sizeY)
+                       cell_margin=(8, 15),             # distance between cell borders (x, y)
+                       grid_offset=(-2.05, -4.1),       # grid offset in (x, y)
+                       edge_exclusion=2.2,              # margin from the wafer edge where a red edge exclusion ring is drawn
                        coverage='full',                 # 'full': will cover wafer with cells, partial cells allowed
                                                         # 'inner': only full cells allowed
                        notch_orientation=270)           # angle of notch in degrees. 270 corresponds to a notch at the bottom
 ```
 
 To add an image at a specific cell/relative cell coordinates simply:
 ```python
 wm.add_image(image_source_file="inspection1.jpg",
              cell=(1, 0),                               # (cell_index_x, cell_index_y)
-             offset=(2.0e-3, 2.0e-3))                   # relative coordinate of the image within the cell
+             offset=(2.0, 2.0))                         # relative coordinate of the image within the cell
 ```
 
 Adding vectors is just as easy. Just define cell and \[(start_rel_coordinates), (end_rel_coordinates)\]:
 ```python
 vectors = [
-            ((3, 0), [(0, 0), (1e-3, 1e-3)]),
-            ((3, 0), [(1e-3, 0), (-5e-3, 5e-3)]),
-            ((3, 0), [(0, 1e-3), (10e-3, -10e-3)]),
-            ((3, 0), [(1e-3, 1e-3), (-20e-3, -20e-3)]),
+            ((3, 0), [(0, 0), (1, 1)]),
+            ((3, 0), [(1, 0), (-5, 5)]),
+            ((3, 0), [(0, 1), (10, -10)]),
+            ((3, 0), [(1, 1), (-20, -20)]),
             ]
 colors = ['green', 'red', 'blue', 'black']
 for color, (cell, vector) in zip(colors, vectors):
     wm.add_vector(vector_points=vector, cell=cell, vector_style={'color': color}, root_style={'radius': 1, 'color': color})
 ```
 
 Let's throw in some points in a normal distribution for good measure too:
 
 ```python
 # add 50 points per cell, in a random distribution
 import random as rnd
 
-cell_size = (10e-3, 20e-3)
-cell_points = [(cell, [(rnd.gauss(cell_size[1] / 2, cell_size[1] / 6),
-                        rnd.gauss(cell_size[0] / 2, cell_size[0] / 6)) for _ in
-                       range(50)]) for cell in wm._cell_map.keys()]
+cell_size = (10, 20)
+cell_points = [(cell, [(rnd.gauss(cell_size[0] / 2, cell_size[0] / 6),
+                        rnd.gauss(cell_size[1] / 2, cell_size[1] / 6)) for _ in
+                       range(50)]) for cell in wm.cell_map.keys()]
 for cell, cell_points_ in cell_points:
     for cell_point in cell_points_:
         wm.add_point(cell=cell, offset=cell_point)
 ```
 
 Finally, nothing would matter if we couldn't see the result:
 ```python
 # save to html
 wm.save_html(f"wafermap.html")
 
-# save to png (Mozilla must be installed)
+# save to png (Chromium must be installed)
 wm.save_png(f"wafermap.png")
 ```
 
 
 ## Dependencies
 
 - __Folium__ & __branca__ -> to make dynamic, zoom-able and pan-able HTML based maps
 - __Pillow__ -> to support embedded images and format the optional image output 
-- Optional for exporting to .png images: __selenium__ and MS Edge browser installed.
+- __Chromium__ -> exporting to .png images
 
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
```

### Comparing `wafermap-0.2.3/wafermap/utils.py` & `wafermap-0.2.4/wafermap/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""Utility functions"""
-
-import colorsys
-import math
-
-import numpy
-
-# Color functions
-
-
-def rgb_to_html(red: float, green: float, blue: float) -> str:
-    """Convert given rgb color to an HTML code"""
-    return "#%02X%02X%02X" % (red, green, blue)
-
-
-def complementary(red: int, green: int, blue: int) -> (int, int, int):
-    """returns RGB components of complementary color"""
-    hsv = colorsys.rgb_to_hsv(red, green, blue)
-    return colorsys.hsv_to_rgb((hsv[0] + 0.5) % 1, hsv[1], hsv[2])
-
-
-# Utility functions
-
-
-def euclidean_distance(point: (float, float), origin: (float, float) = None) -> float:
-    """Calculate euclidean distance from the origin"""
-    if origin is None:
-        return math.sqrt(sum((p**2 for p in point)))
-    assert len(origin) == len(point)
-    return math.sqrt(sum(((p - o) ** 2 for p, o in zip(point, origin))))
-
-
-def bounded_rectangle(
-    rect: [(float, float)], bounds: [(float, float)]
-) -> [(float, float)]:
-    """
-    Resize rectangle given by points into a rectangle that fits within bounds,
-    preserving the aspect ratio.
-    :param rect: Input rectangle [ll, ur], where each point is (y, x)
-    :param bounds: Input bounding rectangle [ll, ur]
-    :return: Bounded rectangle with same aspect ratio
-    """
-    assert len(rect) == len(bounds) == 2
-    assert rect[0][0] <= rect[1][0] and rect[0][1] <= rect[1][1]
-    assert bounds[0][0] <= bounds[1][0] and bounds[0][1] <= bounds[1][1]
-
-    width_input = rect[1][1] - rect[0][1]
-    height_input = rect[1][0] - rect[0][0]
-    width_bound = bounds[1][1] - bounds[0][1]
-    height_bound = bounds[1][0] - bounds[0][0]
-
-    width = width_input
-    height = height_input
-
-    # find new rect points
-    while width > width_bound or height > height_bound:
-        if width > width_bound:
-            # need to bound w
-            a_w = width_bound / width
-            width = width_bound
-            height = height * a_w
-
-        if height > height_bound:
-            # need to bound w
-            a_h = height_bound / height
-            height = height_bound
-            width = width * a_h
-
-    rect_out = [rect[0], (rect[0][0] + height, rect[0][1] + width)]
-
-    return rect_out
-
-
-def rotate(
-    points: [(float, float)], anchor: (float, float), angle: float = 90.0
-) -> [(float, float)]:
-    """Rotates points (nx2) about anchor (x, y) by angle in degrees"""
-    points = numpy.array(points)
-    anchor = numpy.array(anchor)
-    angle = math.radians(-angle)
-    return (
-        numpy.dot(
-            points - anchor,
-            [[math.cos(angle), math.sin(angle)], [-math.sin(angle), math.cos(angle)]],
-        )
-        + anchor
-    )
-
-
-def cart2pol(x: float, y: float) -> (float, float):
-    """Convert cartesian coordinates x, y into polar rho, phi"""
-    rho = numpy.sqrt(x**2 + y**2)
-    phi = numpy.arctan2(y, x)
-    return rho, phi
-
-
-def pol2cart(rho: float, phi: float) -> (float, float):
-    """Convert polar coordinates rho, phi into cartesian x, y"""
-    x = rho * numpy.cos(phi)
-    y = rho * numpy.sin(phi)
-    return x, y
+"""Utility functions"""
+
+import colorsys
+import math
+
+import numpy
+
+# Color functions
+
+
+def rgb_to_html(red: float, green: float, blue: float) -> str:
+    """Convert given rgb color to an HTML code"""
+    return "#%02X%02X%02X" % (red, green, blue)
+
+
+def complementary(red: int, green: int, blue: int) -> (int, int, int):
+    """returns RGB components of complementary color"""
+    hsv = colorsys.rgb_to_hsv(red, green, blue)
+    return colorsys.hsv_to_rgb((hsv[0] + 0.5) % 1, hsv[1], hsv[2])
+
+
+# Utility functions
+
+
+def euclidean_distance(point: (float, float), origin: (float, float) = None) -> float:
+    """Calculate euclidean distance from the origin"""
+    if origin is None:
+        return math.sqrt(sum((p**2 for p in point)))
+    assert len(origin) == len(point)
+    return math.sqrt(sum(((p - o) ** 2 for p, o in zip(point, origin))))
+
+
+def bounded_rectangle(
+    rect: [(float, float)], bounds: [(float, float)]
+) -> [(float, float)]:
+    """
+    Resize rectangle given by points into a rectangle that fits within bounds,
+    preserving the aspect ratio.
+    :param rect: Input rectangle [ll, ur], where each point is (y, x)
+    :param bounds: Input bounding rectangle [ll, ur]
+    :return: Bounded rectangle with same aspect ratio
+    """
+    assert len(rect) == len(bounds) == 2
+    assert rect[0][0] <= rect[1][0] and rect[0][1] <= rect[1][1]
+    assert bounds[0][0] <= bounds[1][0] and bounds[0][1] <= bounds[1][1]
+
+    width_input = rect[1][1] - rect[0][1]
+    height_input = rect[1][0] - rect[0][0]
+    width_bound = bounds[1][1] - bounds[0][1]
+    height_bound = bounds[1][0] - bounds[0][0]
+
+    width = width_input
+    height = height_input
+
+    # find new rect points
+    while width > width_bound or height > height_bound:
+        if width > width_bound:
+            # need to bound w
+            a_w = width_bound / width
+            width = width_bound
+            height = height * a_w
+
+        if height > height_bound:
+            # need to bound w
+            a_h = height_bound / height
+            height = height_bound
+            width = width * a_h
+
+    rect_out = [rect[0], (rect[0][0] + height, rect[0][1] + width)]
+
+    return rect_out
+
+
+def rotate(
+    points: [(float, float)], anchor: (float, float), angle: float = 90.0
+) -> [(float, float)]:
+    """Rotates points (nx2) about anchor (x, y) by angle in degrees"""
+    points = numpy.array(points)
+    anchor = numpy.array(anchor)
+    angle = math.radians(-angle)
+    return (
+        numpy.dot(
+            points - anchor,
+            [[math.cos(angle), math.sin(angle)], [-math.sin(angle), math.cos(angle)]],
+        )
+        + anchor
+    )
+
+
+def cart2pol(x: float, y: float) -> (float, float):
+    """Convert cartesian coordinates x, y into polar rho, phi"""
+    rho = numpy.sqrt(x**2 + y**2)
+    phi = numpy.arctan2(y, x)
+    return rho, phi
+
+
+def pol2cart(rho: float, phi: float) -> (float, float):
+    """Convert polar coordinates rho, phi into cartesian x, y"""
+    x = rho * numpy.cos(phi)
+    y = rho * numpy.sin(phi)
+    return x, y
```

### Comparing `wafermap-0.2.3/PKG-INFO` & `wafermap-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: wafermap
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python package to plot maps of semiconductor wafers.
 Home-page: https://github.com/cap1tan/wafermap
 License: MIT
 Keywords: semiconductor,wafer,layout,plot
-Author: Sotiris Thomas
-Author-email: sothomas88@gmail.com
+Author: cap1tan
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: branca (>=0.6.0,<0.7.0)
 Requires-Dist: folium (>=0.14.0,<0.15.0)
+Requires-Dist: html2image (>=2.0.3,<3.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Project-URL: Repository, https://github.com/cap1tan/wafermap
 Description-Content-Type: text/markdown
 
 # Wafermap
 
-[![image](https://img.shields.io/pypi/v/wafermap.svg)](https://pypi.python.org/pypi/wafermap)
-[![image](https://img.shields.io/pypi/pyversions/wafermap.svg)](https://pypi.python.org/pypi/wafermap)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[
+![pypi](https://img.shields.io/pypi/v/wafermap.svg)
+![pypi](https://img.shields.io/pypi/pyversions/wafermap.svg)
+![pypi](https://img.shields.io/github/license/cap1tan/wafermap.svg)
+](https://pypi.org/project/wafermap/)
+[
+![GitHub](https://img.shields.io/github/v/release/cap1tan/wafermap?include_prereleases)
+![GitHub](https://img.shields.io/github/languages/code-size/cap1tan/wafermap)
+![pypi](https://img.shields.io/badge/linting-pylint-yellowgreen)
+](https://github.com/cap1tan/wafermap)
+
 
 
 A python package to plot maps of semiconductor wafers.
 
 Free software: MIT license
 
 
@@ -39,15 +46,15 @@
 * Circular wafers with arbitrary notch orientations.
 * Edge-exclusion and grids with optional margin.
 * Hover-able points, vectors and images.
 * Tooltips with embeddable images.
 * Individual labels and colors for each die.
 * Toggle layers on/off individually.
 * Export zoom-able maps to HTML.
-* Export PNG images with selenium
+* Export PNG images (needs Chromium)
 
 
 ## Examples
 
 - See the full dynamic maps [here](https://cap1tan.github.io/wafermap/)!
 
 - Static png image, just to get a taste:
@@ -92,74 +99,74 @@
 
 ```python
     import wafermap
 ```
 
 First let's define a Wafermap:
 ```python
-wm = wafermap.WaferMap(wafer_radius=100e-3,             # all length dimensions in meters
-                       cell_size=(10e-3, 20e-3),        # (sizeX, sizeY)
-                       cell_margin=(8e-3, 15e-3),       # distance between cell borders (x, y)
-                       grid_offset=(-2.05e-3, -4.1e-3), # grid offset in (x, y)
-                       edge_exclusion=2.2e-3,           # margin from the wafer edge where a red edge exclusion ring is drawn
+wm = wafermap.WaferMap(wafer_radius=100,                # all length dimensions in mm
+                       cell_size=(10, 20),              # (sizeX, sizeY)
+                       cell_margin=(8, 15),             # distance between cell borders (x, y)
+                       grid_offset=(-2.05, -4.1),       # grid offset in (x, y)
+                       edge_exclusion=2.2,              # margin from the wafer edge where a red edge exclusion ring is drawn
                        coverage='full',                 # 'full': will cover wafer with cells, partial cells allowed
                                                         # 'inner': only full cells allowed
                        notch_orientation=270)           # angle of notch in degrees. 270 corresponds to a notch at the bottom
 ```
 
 To add an image at a specific cell/relative cell coordinates simply:
 ```python
 wm.add_image(image_source_file="inspection1.jpg",
              cell=(1, 0),                               # (cell_index_x, cell_index_y)
-             offset=(2.0e-3, 2.0e-3))                   # relative coordinate of the image within the cell
+             offset=(2.0, 2.0))                         # relative coordinate of the image within the cell
 ```
 
 Adding vectors is just as easy. Just define cell and \[(start_rel_coordinates), (end_rel_coordinates)\]:
 ```python
 vectors = [
-            ((3, 0), [(0, 0), (1e-3, 1e-3)]),
-            ((3, 0), [(1e-3, 0), (-5e-3, 5e-3)]),
-            ((3, 0), [(0, 1e-3), (10e-3, -10e-3)]),
-            ((3, 0), [(1e-3, 1e-3), (-20e-3, -20e-3)]),
+            ((3, 0), [(0, 0), (1, 1)]),
+            ((3, 0), [(1, 0), (-5, 5)]),
+            ((3, 0), [(0, 1), (10, -10)]),
+            ((3, 0), [(1, 1), (-20, -20)]),
             ]
 colors = ['green', 'red', 'blue', 'black']
 for color, (cell, vector) in zip(colors, vectors):
     wm.add_vector(vector_points=vector, cell=cell, vector_style={'color': color}, root_style={'radius': 1, 'color': color})
 ```
 
 Let's throw in some points in a normal distribution for good measure too:
 
 ```python
 # add 50 points per cell, in a random distribution
 import random as rnd
 
-cell_size = (10e-3, 20e-3)
-cell_points = [(cell, [(rnd.gauss(cell_size[1] / 2, cell_size[1] / 6),
-                        rnd.gauss(cell_size[0] / 2, cell_size[0] / 6)) for _ in
-                       range(50)]) for cell in wm._cell_map.keys()]
+cell_size = (10, 20)
+cell_points = [(cell, [(rnd.gauss(cell_size[0] / 2, cell_size[0] / 6),
+                        rnd.gauss(cell_size[1] / 2, cell_size[1] / 6)) for _ in
+                       range(50)]) for cell in wm.cell_map.keys()]
 for cell, cell_points_ in cell_points:
     for cell_point in cell_points_:
         wm.add_point(cell=cell, offset=cell_point)
 ```
 
 Finally, nothing would matter if we couldn't see the result:
 ```python
 # save to html
 wm.save_html(f"wafermap.html")
 
-# save to png (Mozilla must be installed)
+# save to png (Chromium must be installed)
 wm.save_png(f"wafermap.png")
 ```
 
 
 ## Dependencies
 
 - __Folium__ & __branca__ -> to make dynamic, zoom-able and pan-able HTML based maps
 - __Pillow__ -> to support embedded images and format the optional image output 
-- Optional for exporting to .png images: __selenium__ and MS Edge browser installed.
+- __Chromium__ -> exporting to .png images
 
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
```

