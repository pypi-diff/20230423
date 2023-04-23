# Comparing `tmp/candlestick-chart-2.6.0.tar.gz` & `tmp/candlestick-chart-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candlestick-chart-2.6.0.tar", last modified: Fri Apr 14 19:55:36 2023, max compression
+gzip compressed data, was "candlestick-chart-2.7.0.tar", last modified: Sun Apr 23 21:05:20 2023, max compression
```

## Comparing `candlestick-chart-2.6.0.tar` & `candlestick-chart-2.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.768699 candlestick-chart-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/src/candlestick_chart/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/candle_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/info_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/volume_pane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/y_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:05:20.758448 candlestick-chart-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-23 21:05:20.758448 candlestick-chart-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-23 21:05:20.758448 candlestick-chart-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:05:20.754448 candlestick-chart-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:05:20.758448 candlestick-chart-2.7.0/src/candlestick_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/candle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/chart_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/info_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/volume_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart/y_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:05:20.758448 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 21:05:20.000000 candlestick-chart-2.7.0/src/candlestick_chart.egg-info/top_level.txt
```

### Comparing `candlestick-chart-2.6.0/LICENSE` & `candlestick-chart-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/PKG-INFO` & `candlestick-chart-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlestick-chart
-Version: 2.6.0
+Version: 2.7.0
 Summary: Draw candlesticks charts right into your terminal, using Python!
 Home-page: https://github.com/BoboTiG/py-candlestick-chart
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: LICENSE
 Project-URL: Documentation, https://github.com/BoboTiG/py-candlestick-chart
 Project-URL: Source, https://github.com/BoboTiG/py-candlestick-chart
@@ -18,14 +18,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Terminals
 Requires-Python: >=3.10
```

### Comparing `candlestick-chart-2.6.0/README.md` & `candlestick-chart-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/setup.cfg` & `candlestick-chart-2.7.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	Intended Audience :: Education
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Financial and Insurance Industry
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Graphics :: Viewers
 	Topic :: Office/Business :: Financial
 	Topic :: Scientific/Engineering :: Visualization
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Software Development :: User Interfaces
 	Topic :: Terminals
 
@@ -65,11 +66,21 @@
 [tool:isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 120
 
+[tool:pytest]
+pythonpath = src
+addopts = 
+	--showlocals
+	--strict-markers
+	-r fE
+	-v
+	--cov=candlestick_chart
+	--cov-report=term-missing
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/__init__.py` & `candlestick-chart-2.7.0/src/candlestick_chart/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module is maintained by Mickaël Schoentgen <contact@tiger-222.fr>.
 
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/py-candlestrick-charts
 If that URL should fail, try contacting the author.
 """
 
-__version__ = "2.6.0"
+__version__ = "2.7.0"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2022-2023, Mickaël 'Tiger-222' Schoentgen
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
 and that both that copyright notice and this permission notice appear
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/__main__.py` & `candlestick-chart-2.7.0/src/candlestick_chart/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-m",
         "--mode",
         help="Select the method for retrieving the candles.",
         choices=["stdin", "csv-file", "json-file"],
         required=True,
     )
     parser.add_argument("-f", "--file", help="[MODE:*-file] File to read candles from.")
-    parser.add_argument("--chart-name", help="Sets the chart name.")
+    parser.add_argument("--chart-name", default="", help="Sets the chart name.")
     parser.add_argument("--bear-color", help="Sets the descending candles color in hexadecimal.")
     parser.add_argument("--bull-color", help="Sets the ascending candles color in hexadecimal.")
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
     return parser.parse_args(sys.argv[1:])
 
 
 def main() -> int:
@@ -56,9 +56,9 @@
         r, g, b = hexa_to_rgb(options.bull_color)
         chart.set_bull_color(r, g, b)
 
     chart.draw()
     return 0
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: nocover
     sys.exit(main())
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/candle.py` & `candlestick-chart-2.7.0/src/candlestick_chart/candle.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/candle_set.py` & `candlestick-chart-2.7.0/src/candlestick_chart/candle_set.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/chart.py` & `candlestick-chart-2.7.0/src/candlestick_chart/chart.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/chart_data.py` & `candlestick-chart-2.7.0/src/candlestick_chart/chart_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os import get_terminal_size
+from shutil import get_terminal_size
 
 from . import constants
 from .candle import Candles
 from .candle_set import CandleSet
 from .volume_pane import VolumePane
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/chart_renderer.py` & `candlestick-chart-2.7.0/src/candlestick_chart/chart_renderer.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/colors.py` & `candlestick-chart-2.7.0/src/candlestick_chart/colors.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/constants.py` & `candlestick-chart-2.7.0/src/candlestick_chart/constants.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/info_bar.py` & `candlestick-chart-2.7.0/src/candlestick_chart/info_bar.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/utils.py` & `candlestick-chart-2.7.0/src/candlestick_chart/utils.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/volume_pane.py` & `candlestick-chart-2.7.0/src/candlestick_chart/volume_pane.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart/y_axis.py` & `candlestick-chart-2.7.0/src/candlestick_chart/y_axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return (
             (candle.high - min_value) / diff * height,  # high_y
             (candle.low - min_value) / diff * height,  # low_y
             (max_open - min_value) / diff * height,  # max_y
             (min_open - min_value) / diff * height,  # min_y
         )
 
-    def render_line(self, y: int, highlights: Dict[str, str | Tuple[int, int, int]] = None) -> str:
+    def render_line(self, y: int, highlights: Dict[str, str | Tuple[int, int, int]] | None = None) -> str:
         return (
             self.render_empty(y=y, highlights=highlights)
             if y % constants.Y_AXIS_SPACING
             else self._render_tick(y, highlights or {})
         )
 
     def _round_price(
@@ -79,15 +79,17 @@
             f" {color(f'├ {price:<{cell_min_length}}', custom_color)}"
             if constants.Y_AXIS_ON_THE_RIGHT
             else f"{color(f'{price:<{cell_min_length}} ┤', custom_color)}{' ' * constants.MARGIN_RIGHT}"
         )
 
         return has_special_price, price
 
-    def render_empty(self, y: float = None, highlights: Dict[str, str | Tuple[int, int, int]] = None) -> str:
+    def render_empty(
+        self, y: float | None = None, highlights: Dict[str, str | Tuple[int, int, int]] | None = None
+    ) -> str:
         if highlights and y:
             has_special_price, price = self._render_price(y, highlights)
             if has_special_price:
                 return price
 
         if constants.Y_AXIS_ON_THE_RIGHT:
             return " │"
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart.egg-info/PKG-INFO` & `candlestick-chart-2.7.0/src/candlestick_chart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlestick-chart
-Version: 2.6.0
+Version: 2.7.0
 Summary: Draw candlesticks charts right into your terminal, using Python!
 Home-page: https://github.com/BoboTiG/py-candlestick-chart
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: LICENSE
 Project-URL: Documentation, https://github.com/BoboTiG/py-candlestick-chart
 Project-URL: Source, https://github.com/BoboTiG/py-candlestick-chart
@@ -18,14 +18,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Terminals
 Requires-Python: >=3.10
```

### Comparing `candlestick-chart-2.6.0/src/candlestick_chart.egg-info/SOURCES.txt` & `candlestick-chart-2.7.0/src/candlestick_chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

