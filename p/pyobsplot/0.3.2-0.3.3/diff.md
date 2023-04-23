# Comparing `tmp/pyobsplot-0.3.2.tar.gz` & `tmp/pyobsplot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsplot-0.3.2.tar", max compression
+gzip compressed data, was "pyobsplot-0.3.3.tar", max compression
```

## Comparing `pyobsplot-0.3.2.tar` & `pyobsplot-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.2/LICENSE
--rw-r--r--   0        0        0     3843 2023-04-08 15:49:45.532400 pyobsplot-0.3.2/README.md
--rw-r--r--   0        0        0     1251 2023-04-12 09:10:42.356278 pyobsplot-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-06 08:28:46.892341 pyobsplot-0.3.2/src/pyobsplot/__init__.py
--rw-r--r--   0        0        0     3428 2023-04-11 14:13:06.230946 pyobsplot-0.3.2/src/pyobsplot/data.py
--rw-r--r--   0        0        0     2045 2023-04-12 08:53:57.503120 pyobsplot-0.3.2/src/pyobsplot/jsdom.py
--rw-r--r--   0        0        0     1963 2023-04-09 22:23:38.052708 pyobsplot-0.3.2/src/pyobsplot/jsmodules.py
--rw-r--r--   0        0        0     3802 2023-04-09 22:23:38.052708 pyobsplot-0.3.2/src/pyobsplot/obsplot.py
--rw-r--r--   0        0        0     6158 2023-04-11 14:11:53.254582 pyobsplot-0.3.2/src/pyobsplot/parsing.py
--rw-r--r--   0        0        0       89 2023-04-12 09:12:28.362119 pyobsplot-0.3.2/src/pyobsplot/static/styles.css
--rw-r--r--   0        0        0  2268272 2023-04-12 09:12:28.362119 pyobsplot-0.3.2/src/pyobsplot/static/widget.js
--rw-r--r--   0        0        0      344 2023-04-09 22:23:38.084708 pyobsplot-0.3.2/src/pyobsplot/utils.py
--rw-r--r--   0        0        0     1179 2023-04-09 22:23:38.084708 pyobsplot-0.3.2/src/pyobsplot/widget.py
--rw-r--r--   0        0        0     5115 1970-01-01 00:00:00.000000 pyobsplot-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4287 2023-04-16 14:13:49.662823 pyobsplot-0.3.3/README.md
+-rw-r--r--   0        0        0     1303 2023-04-23 17:32:40.447995 pyobsplot-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.3/src/pyobsplot/__init__.py
+-rw-r--r--   0        0        0     3428 2023-04-11 14:13:06.230946 pyobsplot-0.3.3/src/pyobsplot/data.py
+-rw-r--r--   0        0        0     1894 2023-04-23 17:25:31.529014 pyobsplot-0.3.3/src/pyobsplot/jsdom.py
+-rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.3/src/pyobsplot/jsmodules.py
+-rw-r--r--   0        0        0     5896 2023-04-23 17:28:15.464378 pyobsplot-0.3.3/src/pyobsplot/obsplot.py
+-rw-r--r--   0        0        0     6158 2023-04-11 14:11:53.254582 pyobsplot-0.3.3/src/pyobsplot/parsing.py
+-rw-r--r--   0        0        0       89 2023-04-23 17:34:03.547991 pyobsplot-0.3.3/src/pyobsplot/static/styles.css
+-rw-r--r--   0        0        0  2268563 2023-04-23 17:34:03.547991 pyobsplot-0.3.3/src/pyobsplot/static/widget.js
+-rw-r--r--   0        0        0     2552 2023-04-23 17:25:05.613152 pyobsplot-0.3.3/src/pyobsplot/utils.py
+-rw-r--r--   0        0        0     1437 2023-04-23 17:12:16.978286 pyobsplot-0.3.3/src/pyobsplot/widget.py
+-rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 pyobsplot-0.3.3/PKG-INFO
```

### Comparing `pyobsplot-0.3.2/LICENSE` & `pyobsplot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.2/README.md` & `pyobsplot-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyobsplot
 
 [![PyPI](https://img.shields.io/pypi/v/pyobsplot.svg?color=green)](https://pypi.org/project/pyobsplot)
+[![npm](https://img.shields.io/npm/v/pyobsplot?color=green)](https://www.npmjs.com/package/pyobsplot)
 [![Tests](https://github.com/juba/pyobsplot/actions/workflows/tests.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/tests.yml)
 [![Documentation](https://github.com/juba/pyobsplot/actions/workflows/publish.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/publish.yml)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
+[![Open In Colab](https://github.com/juba/pyobsplot/raw/main/doc/img/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
 
 
 `pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in [Jupyter](https://jupyter.org) notebooks, [VSCode](https://code.visualstudio.com) notebooks, [Google Colab](https://colab.research.google.com) and [Quarto](https://quarto.org) documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
 
 It allows to do things like :
 
 ```python
@@ -46,22 +47,26 @@
 ```
 
 For usage instructions, see the [documentation website](https://juba.github.io/pyobsplot):
 
 - See [getting started](https://juba.github.io/pyobsplot/getting_started.html) for a quick usage overview.
 - See [usage](https://juba.github.io/pyobsplot/usage.html) for more detailed usage instructions.
 
+If you just want to try this package without installing it on your computer, you can open an introduction notebook in Google Colab: 
+
+[![](https://github.com/juba/pyobsplot/raw/main/doc/img/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
+
 
 ## Features and limitations
 
 **Features:**
 
 - Syntax as close as possible to the JavaScript one
-- Two renderers available: `widget`, which generates plots as Jupyter widgets, and `jsdom`, which generate SVG or HTML outputs
-- [Pandas](https://pandas.pydata.org) and [polars](https://pola.rs) DataFrame and Series objects are serialized using [Arrow](https://arrow.apache.org) IPC format for improved speed and data type conversions
+- Two renderers available: `widget`, which generates plots as Jupyter widgets, and `jsdom`, which generates SVG or HTML outputs
+- [Pandas](https://pandas.pydata.org) and [polars](https://pola.rs) DataFrame and Series objects are serialized using [Arrow](https://arrow.apache.org) IPC format for improved speed and better data type conversions
 - Works offline, no iframe or dependency to Observable runtime
 - Caching mechanism of data objects if they are used several times in the same plot
 - Custom JavaScript code can be passed as strings with the `js` method
 - Python `date` and `datetime` objects are automatically converted to JavaScript `Date` objects
 - Works with Jupyter notebooks and Quarto HTML documents. Plots without legends are also supported in PDF and docx outputs with the `jsdom` renderer.
 
 **Limitations:**
@@ -72,8 +77,8 @@
 
 
 ## Credits
 
 - [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot), developed by [Mike Bostock](https://observablehq.com/@mbostock) and [Philippe Rivière](https://observablehq.com/@fil) among others.
 - The widget is developed thanks to the [anywidget](https://anywidget.dev) framework.
 - Some code from the `jsdom` renderer has been adapted from [altair_saver](https://github.com/altair-viz/altair_saver).
-- The documentation website is generated by [Quarto].
+- The documentation website is generated by [Quarto](https://quarto.org).
```

### Comparing `pyobsplot-0.3.2/pyproject.toml` & `pyobsplot-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobsplot"
-version = "0.3.2"
+version = "0.3.3"
 description = "Observable Plot in Jupyter notebooks and Quarto documents"
 authors = ["Julien Barnier <julien@nozav.org>"]
 license = "MIT"
 readme = "README.md"
 include = ["src/pyobsplot/static/*"]
 homepage = "https://github.com/juba/pyobsplot"
 documentation = "https://juba.github.io/pyobsplot"
@@ -19,20 +19,22 @@
 ]
 
 [tool.poetry.urls]
 changelog = "https://github.com/juba/pyobsplot/blob/main/NEWS.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-anywidget = {extras = ["dev"], version = "^0.2.0"}
+anywidget = {extras = ["dev"], version = "^0.2.2"}
 pandas = ">=1.2.0"
 polars = ">=0.16.0"
 pyarrow = "^11.0.0"
 ipywidgets = ">=8.0.0"
+jupyterlab_widgets = ">=3.0.0"
 jupyterlab = ">=3.6.0"
+requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.259"
 black = "^23.1.0"
 pytest = "^7.2.2"
 requests = "^2.28.2"
 geopandas = "^0.12.2"
```

### Comparing `pyobsplot-0.3.2/src/pyobsplot/__init__.py` & `pyobsplot-0.3.3/src/pyobsplot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.2/src/pyobsplot/data.py` & `pyobsplot-0.3.3/src/pyobsplot/data.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.2/src/pyobsplot/jsdom.py` & `pyobsplot-0.3.3/src/pyobsplot/jsdom.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Obsplot jsdom handling.
 """
 
-import subprocess
-import os
 import json
-import shutil
+import requests
 from IPython.display import HTML, SVG
 
 from typing import Any
 
 from .parsing import SpecParser
 
 
@@ -19,53 +17,53 @@
     The class takes a plot specification as input and generates a plot as SVG or HTML
     by calling a JSDom script with node.
 
     The specification can be given as a dict, a Plot function call or as
     Python kwargs.
     """
 
-    def __init__(self, spec: Any, default: dict = {}, debug: bool = False) -> None:
+    def __init__(
+        self,
+        spec: Any,
+        port: int,
+        default: dict = {},
+        debug: bool = False,
+    ) -> None:
         """
         Constructor. Parse the spec given as argument.
         """
         # Create parser
         parser = SpecParser(renderer="jsdom", default=default)
         # Parse spec code
         parser.spec = spec
         code = parser.parse_spec()
         # Create spec object
         spec = {"data": parser.serialize_data(), "code": code, "debug": debug}
         self.spec = spec
+        self.port = port
 
     def plot(self):
-        """Generates the plot by calling node script.
+        """Generates the plot by sending request to http node server.
 
         Returns:
             Either an HTML or SVG IPython.display object.
         """
 
-        # Check for node executable
-        npx = shutil.which("npx")
-        if not npx:
-            raise RuntimeError("npx executable has not been found.")
-        # Run node script with JSON spec as input
-        p = subprocess.run(
-            ["npx", "pyobsplot"],
-            input=json.dumps(self.spec),
-            capture_output=True,
-            encoding="Utf8",
-            # Use shell=True if we are on Windows. Otherwise PATH
-            # is not parsed and npx is not found.
-            shell=os.name == "nt",
-        )
-        if p.returncode != 0:
-            raise RuntimeError(
-                f"jsdom script error (${p.returncode}): ${p.stderr} - ${p.stdout}"
+        # Make POST request with plot spec
+        url = f"http://localhost:{self.port}/plot"
+        try:
+            r = requests.post(url, data=json.dumps(self.spec))
+        except ConnectionRefusedError:
+            print(
+                f"Error: can't connect to generator server on port {self.port}. Please recreate your generator object."  # noqa: E501
             )
-        # Get script output
-        out = p.stdout
+        # Read back result
+        if r.status_code == 500:
+            raise RuntimeError(r.content.decode())
+        out = r.content.decode()
+
         # If output is svg, returns IPython.display.SVG
         if out[0:4] == "<svg":
             return SVG(out)
         # Else, returns IPython.display.HTML
         else:
             return HTML(out)
```

### Comparing `pyobsplot-0.3.2/src/pyobsplot/jsmodules.py` & `pyobsplot-0.3.3/src/pyobsplot/jsmodules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,65 @@
+from functools import partial
+
 from .obsplot import ObsplotWidgetCreator, ObsplotJsdomCreator
 from .widget import ObsplotWidget
+from .utils import plot_methods
 
 # Default renderer for Plot.plot() calls.
 # Not documented, only internal use for documentation generation
 _plot_renderer = "widget"
 
 
+class Plot:
+    """Plot methods class."""
+
+    @staticmethod
+    def plot(*args, **kwargs) -> ObsplotWidget:
+        """
+        Plot.plot static method. If called directly, create an ObsplotWidget
+        or an ObpsplotJsdom with args and kwargs.
+        """
+        if _plot_renderer == "widget":
+            op = ObsplotWidgetCreator()
+        if _plot_renderer == "jsdom":
+            op = ObsplotJsdomCreator()
+        return op(*args, **kwargs)
+
+
+def method_to_spec(*args, **kwargs) -> dict:
+    """Function used for creating Plot.xyz static methods.
+    Generates a dict of specification with method name and args.
+
+    Returns:
+        dict: Plot function specification.
+    """
+    name = kwargs["name"]
+    if len(kwargs) > 1:
+        raise ValueError(f"kwargs must not be passed to Plot.{name} : {kwargs}")
+    return {
+        "pyobsplot-type": "function",
+        "module": "Plot",
+        "method": name,
+        "args": args,
+    }
+
+
+# For each exitsting JS Plot method, create a static Python Plot method with the
+# same name which calls method_to_spec()
+for method in plot_methods:
+    if method != "plot":
+        setattr(Plot, method, staticmethod(partial(method_to_spec, name=method)))
+
+
 class JSModule(type):
     """metaclass to allow JavaScript module and methods handling."""
 
     def __getattr__(cls: type, name: str) -> callable:
         """Intercept methods calling and returns a parsed and typed dict object."""
 
-        # If "Plot.plot" is called, returns it as is.
-        # This is to allow users to use `Plot.plot` directly to generate charts
-        # without having to call Plot.plot = Obsplot() first.
-        if ("pyobsplot.parsing", "Plot", "plot") == (
-            cls.__module__,
-            cls.__name__,
-            name,
-        ):
-            return Plot.plot
-
         def wrapper(*args, **kwargs) -> dict:
             if kwargs:
                 raise ValueError(
                     f"kwargs must not be passed to {cls.__name__}.{name} : {kwargs}"
                 )
             return {
                 "pyobsplot-type": "function",
@@ -33,30 +67,14 @@
                 "method": name,
                 "args": args,
             }
 
         return wrapper
 
 
-class Plot(metaclass=JSModule):
-    """JSModule class to allow Plot objects in specification."""
-
-    @staticmethod
-    def plot(*args, **kwargs) -> ObsplotWidget:
-        """
-        Plot.plot static method. If called directly, create an ObsplotWidget
-        or an ObpsplotJsdom with args and kwargs.
-        """
-        if _plot_renderer == "widget":
-            op = ObsplotWidgetCreator()
-        if _plot_renderer == "jsdom":
-            op = ObsplotJsdomCreator()
-        return op(*args, **kwargs)
-
-
 class d3(metaclass=JSModule):
     """JSModule class to allow d3 objects in specification."""
 
     pass
 
 
 class Math(metaclass=JSModule):
```

### Comparing `pyobsplot-0.3.2/src/pyobsplot/parsing.py` & `pyobsplot-0.3.3/src/pyobsplot/parsing.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.2/src/pyobsplot/static/widget.js` & `pyobsplot-0.3.3/src/pyobsplot/static/widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82033,29 +82033,40 @@
     try {
         spec["data"] = unserialize_data(spec["data"], renderer);
         out = parse_spec(spec["code"], spec["data"]);
         if (spec["code"]["pyobsplot-type"] == "function") {
             out = out.plot();
         } else {
             if (spec["debug"]) {
-                console.log("--- start pyobsplot debugging output ---");
-                console.log(out);
-                console.log("--- end pyobsplot debugging output ---");
+                debug_output(out, renderer);
             }
             out = plot2(out);
         }
     } catch (error) {
         out = document.createElement("pre");
-        out.style.color = "#CC0000";
-        out.style.padding = "1em 1.5em";
+        out.style.color = "#DD3333";
+        out.style.padding = ".5em 1em";
         out.textContent = "\u26A0 " + error;
     }
     return out;
 }
 
+function debug_output(out, renderer) {
+    if (renderer == "widget") {
+        console.log("--- start pyobsplot debugging output ---");
+        console.log(out);
+        console.log("--- end pyobsplot debugging output ---");
+    }
+    if (renderer == "jsdom") {
+        console.log("<br>--- start pyobsplot debugging output ---<br>");
+        console.log(out);
+        console.log("<br>--- end pyobsplot debugging output ---</br>");
+    }
+}
+
 // js/widget/widget.js
 window.d3 = src_exports;
 window.Plot = src_exports2;
 
 function render(view) {
     let spec = () => view.model.get("spec");
     let plot_div = document.createElement("div");
```

### Comparing `pyobsplot-0.3.2/src/pyobsplot/widget.py` & `pyobsplot-0.3.3/src/pyobsplot/widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,22 @@
 
     The class takes a plot specification as input and generates a plot.
 
     The specification can be given as a dict, a Plot function call or as
     Python kwargs.
     """
 
-    _esm = bundler_output_dir / "widget.js"
-    _css = bundler_output_dir / "styles.css"
+    # Disable _esm and _css watching and live reload to avoid "exception not rethrown"
+    # error with pytest.
+    _esm = anywidget._file_contents.FileContents(
+        bundler_output_dir / "widget.js", start_thread=False
+    )
+    _css = anywidget._file_contents.FileContents(
+        bundler_output_dir / "styles.css", start_thread=False
+    )
     # spec traitlet : plot specification
     spec = traitlets.Dict().tag(sync=True)
 
     def __init__(self, spec, default: dict = {}, debug: bool = False):
         """Obsplot widget constructor."""
         self._debug = debug
         self._default = default
```

### Comparing `pyobsplot-0.3.2/PKG-INFO` & `pyobsplot-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobsplot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Observable Plot in Jupyter notebooks and Quarto documents
 Home-page: https://github.com/juba/pyobsplot
 License: MIT
 Author: Julien Barnier
 Author-email: julien@nozav.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,31 +14,34 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Dist: anywidget[dev] (>=0.2.0,<0.3.0)
+Requires-Dist: anywidget[dev] (>=0.2.2,<0.3.0)
 Requires-Dist: ipywidgets (>=8.0.0)
 Requires-Dist: jupyterlab (>=3.6.0)
+Requires-Dist: jupyterlab_widgets (>=3.0.0)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: polars (>=0.16.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://juba.github.io/pyobsplot
 Project-URL: Repository, https://github.com/juba/pyobsplot
 Project-URL: changelog, https://github.com/juba/pyobsplot/blob/main/NEWS.md
 Description-Content-Type: text/markdown
 
 # pyobsplot
 
 [![PyPI](https://img.shields.io/pypi/v/pyobsplot.svg?color=green)](https://pypi.org/project/pyobsplot)
+[![npm](https://img.shields.io/npm/v/pyobsplot?color=green)](https://www.npmjs.com/package/pyobsplot)
 [![Tests](https://github.com/juba/pyobsplot/actions/workflows/tests.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/tests.yml)
 [![Documentation](https://github.com/juba/pyobsplot/actions/workflows/publish.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/publish.yml)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
+[![Open In Colab](https://github.com/juba/pyobsplot/raw/main/doc/img/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
 
 
 `pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in [Jupyter](https://jupyter.org) notebooks, [VSCode](https://code.visualstudio.com) notebooks, [Google Colab](https://colab.research.google.com) and [Quarto](https://quarto.org) documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
 
 It allows to do things like :
 
 ```python
@@ -77,22 +80,26 @@
 ```
 
 For usage instructions, see the [documentation website](https://juba.github.io/pyobsplot):
 
 - See [getting started](https://juba.github.io/pyobsplot/getting_started.html) for a quick usage overview.
 - See [usage](https://juba.github.io/pyobsplot/usage.html) for more detailed usage instructions.
 
+If you just want to try this package without installing it on your computer, you can open an introduction notebook in Google Colab: 
+
+[![](https://github.com/juba/pyobsplot/raw/main/doc/img/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
+
 
 ## Features and limitations
 
 **Features:**
 
 - Syntax as close as possible to the JavaScript one
-- Two renderers available: `widget`, which generates plots as Jupyter widgets, and `jsdom`, which generate SVG or HTML outputs
-- [Pandas](https://pandas.pydata.org) and [polars](https://pola.rs) DataFrame and Series objects are serialized using [Arrow](https://arrow.apache.org) IPC format for improved speed and data type conversions
+- Two renderers available: `widget`, which generates plots as Jupyter widgets, and `jsdom`, which generates SVG or HTML outputs
+- [Pandas](https://pandas.pydata.org) and [polars](https://pola.rs) DataFrame and Series objects are serialized using [Arrow](https://arrow.apache.org) IPC format for improved speed and better data type conversions
 - Works offline, no iframe or dependency to Observable runtime
 - Caching mechanism of data objects if they are used several times in the same plot
 - Custom JavaScript code can be passed as strings with the `js` method
 - Python `date` and `datetime` objects are automatically converted to JavaScript `Date` objects
 - Works with Jupyter notebooks and Quarto HTML documents. Plots without legends are also supported in PDF and docx outputs with the `jsdom` renderer.
 
 **Limitations:**
@@ -103,9 +110,9 @@
 
 
 ## Credits
 
 - [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot), developed by [Mike Bostock](https://observablehq.com/@mbostock) and [Philippe Rivière](https://observablehq.com/@fil) among others.
 - The widget is developed thanks to the [anywidget](https://anywidget.dev) framework.
 - Some code from the `jsdom` renderer has been adapted from [altair_saver](https://github.com/altair-viz/altair_saver).
-- The documentation website is generated by [Quarto].
+- The documentation website is generated by [Quarto](https://quarto.org).
```

