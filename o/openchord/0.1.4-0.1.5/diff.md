# Comparing `tmp/openchord-0.1.4.tar.gz` & `tmp/openchord-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openchord-0.1.4.tar", last modified: Fri Apr 21 07:30:13 2023, max compression
+gzip compressed data, was "openchord-0.1.5.tar", last modified: Sun Apr 23 21:40:45 2023, max compression
```

## Comparing `openchord-0.1.4.tar` & `openchord-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 07:30:13.520383 openchord-0.1.4/
--rw-rw-rw-   0        0        0    35823 2023-04-20 10:08:25.000000 openchord-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2103 2023-04-21 07:30:13.519386 openchord-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1572 2023-04-20 18:38:40.000000 openchord-0.1.4/README.md
--rw-rw-rw-   0        0        0      707 2023-04-21 07:29:43.000000 openchord-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 07:30:13.521383 openchord-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 07:30:13.497444 openchord-0.1.4/src/
--rw-rw-rw-   0        0        0        0 2023-04-20 18:38:40.000000 openchord-0.1.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:30:13.516395 openchord-0.1.4/src/openchord.egg-info/
--rw-rw-rw-   0        0        0     2103 2023-04-21 07:30:13.000000 openchord-0.1.4/src/openchord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 07:30:13.000000 openchord-0.1.4/src/openchord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 07:30:13.000000 openchord-0.1.4/src/openchord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-21 07:30:13.000000 openchord-0.1.4/src/openchord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-21 07:30:13.000000 openchord-0.1.4/src/openchord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6261 2023-04-20 18:38:40.000000 openchord-0.1.4/src/openchord.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.436657 openchord-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-20 10:08:25.000000 openchord-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2313 2023-04-23 21:40:45.434689 openchord-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2023-04-23 21:37:55.000000 openchord-0.1.5/README.md
+-rw-rw-rw-   0        0        0      786 2023-04-23 09:31:26.000000 openchord-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 21:40:45.436657 openchord-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.402621 openchord-0.1.5/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 09:15:38.000000 openchord-0.1.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.432557 openchord-0.1.5/src/openchord.egg-info/
+-rw-rw-rw-   0        0        0     2313 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7362 2023-04-23 21:16:00.000000 openchord-0.1.5/src/openchord.py
```

### Comparing `openchord-0.1.4/LICENSE` & `openchord-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openchord-0.1.4/PKG-INFO` & `openchord-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install openchord
+pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -37,15 +37,19 @@
 labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
-fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
+fig.colormap = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
+
+## More tutorials and examples
+I wrote a few more tutorials available via the link below and in the `/example` directory
+1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
```

### Comparing `openchord-0.1.4/README.md` & `openchord-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install openchord
+pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -23,15 +23,19 @@
 labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
-fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
+fig.colormap = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
+
+## More tutorials and examples
+I wrote a few more tutorials available via the link below and in the `/example` directory
+1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
```

### Comparing `openchord-0.1.4/pyproject.toml` & `openchord-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openchord"
-version = "0.1.4"
+dynamic = ["version"]
 authors = [
     {name = "Kenny Pang", email = "pangkhangee@gmail.com"},
 ]
 description = "A library for ploting chord diagrams"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["plot", "data science", "Jupyter", "network", "graph"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "drawsvg~=2.0",
+    "drawsvg ~= 2.0",
     "numpy ~= 1.16"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pke1029/open-chord"
 
+[tool.setuptools.dynamic]
+version = {attr = "openchord.__version__"}
+
```

### Comparing `openchord-0.1.4/src/openchord.egg-info/PKG-INFO` & `openchord-0.1.5/src/openchord.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install openchord
+pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -37,15 +37,19 @@
 labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
-fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
+fig.colormap = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
+
+## More tutorials and examples
+I wrote a few more tutorials available via the link below and in the `/example` directory
+1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
```

### Comparing `openchord-0.1.4/src/openchord.py` & `openchord-0.1.5/src/openchord.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import drawsvg as dw
 
+__version__ = "0.1.5"
+
 def pol2cart(rho, phi):
     x = rho * np.cos(phi)
     y = rho * np.sin(phi)
     return x, -y
 
 def get_arc(radius, start_angle, end_angle):
     # calculate coords
@@ -44,43 +46,63 @@
         A = np.array(A)
         m, n = A.shape
         if m != n:
             return False
         return np.allclose(A, A.T)
 
 class Chord:
+
+    colormap_default = ["#FFB6C1", "#FFD700", "#FFA07A", "#90EE90", "#87CEFA", "#DA70D6", "#FF69B4", "#20B2AA"]
+    colormap_vibrant = ["#FF6B6B", "#F9844A", "#F9C74F", "#90BE6D", "#43AA8B", "#4D908E", "#577590", "#277DA1"]
     
-    def __init__(self, data, labels=[], fig_size=500, radius=200, gap=0.01):
-        self.fig_size = fig_size
+    def __init__(self, data, labels=[], radius=200, gap_size=0.01):
         self.data = np.array(data)
         self.labels = labels
         self.radius = radius
+        self.padding = 50
+        self.font_size = 10
+        self.font_family = "Arial"
+        self._gap_size = gap_size
+        self.bg_color = "#ffffff"
+        self.bg_transparancy = 1.0
         self.shape = self.data.shape[0]
         self.row_sum = np.sum(self.data, axis=0)
         self.total = np.sum(self.data)
-        self.gap = gap
-        self.font_size = 10
-        self.conversion_rate = (2*np.pi-gap*self.shape)/self.total
+        self.conversion_rate = (2*np.pi-self.gap_size*self.shape)/self.total
         self.is_symmetric = is_symmetric(self.data)
-        self.ideogram_ends = self.get_ideogram_ends(gap)
+        self.ideogram_ends = self.get_ideogram_ends()
         self.ribbon_ends = self.get_ribbon_ends()
-        self._color_map = ['#001d5c', '#50216c', '#892070', '#ba2769', '#e1405a', '#fa6644', '#ff9228', '#ffc000']
+        self._colormap = self.colormap_default
         self.gradients = self.get_gradients()
 
     @property
-    def color_map(self):
-        return self._color_map
+    def colormap(self):
+        return self._colormap
 
-    @color_map.setter
-    def color_map(self, value):
-        self._color_map = value
+    @colormap.setter
+    def colormap(self, value):
+        self._colormap = value
         self.gradients = self.get_gradients()
+
+    @property
+    def gap_size(self):
+        return self._gap_size
+
+    @gap_size.setter
+    def gap_size(self, value):
+        self._gap_size = value
+        self.conversion_rate = (2*np.pi-self.gap_size*self.shape)/self.total
+        self.ideogram_ends = self.get_ideogram_ends()
+        self.ribbon_ends = self.get_ribbon_ends()
         
     def show(self):
-        fig = dw.Drawing(self.fig_size, self.fig_size, origin='center')
+        fig_size = 2*(self.radius + self.padding)
+        fig = dw.Drawing(fig_size, fig_size, origin='center')
+        # background
+        fig.append(dw.Rectangle(-0.5*fig_size, -0.5*fig_size, fig_size, fig_size, fill=self.bg_color, fill_opacity=self.bg_transparancy))
         # make ideogram
         for i,v in enumerate(self.ideogram_ends):
             fig.append(arc(self.radius, v[0], v[1], color=self.get_color(i)))
         # make ribbon
         for i,v in enumerate(self.ribbon_ends):
             fig.append(ribbon(self.radius*0.99, v[0], v[1], v[2], v[3], color=self.gradients[i]))
         # draw labels
@@ -91,25 +113,25 @@
             angle = midpoint * 180.0/np.pi
             if midpoint > 0.5*np.pi and midpoint < 1.5*np.pi:
                 r *= -1
                 angle = -(180.0-angle)
                 anchor = "end"
             else:
                 anchor = "start"
-            fig.append(dw.Text(v, font_size=self.font_size, x=r, y=0, text_anchor=anchor, dominant_baseline='middle', transform=f"rotate(%f)"%(-angle)))
+            fig.append(dw.Text(v, font_size=self.font_size, x=r, y=0, text_anchor=anchor, dominant_baseline='middle', transform=f"rotate(%f)"%(-angle), font_family=self.font_family))
         return fig
     
-    def get_ideogram_ends(self, gap):
+    def get_ideogram_ends(self):
         arc_lens = self.row_sum * self.conversion_rate
         ideogram_ends = []
         left = 0 
         for arc_len in arc_lens:
             right = left + arc_len
             ideogram_ends.append([left, right])
-            left = right + gap
+            left = right + self.gap_size
         return np.array(ideogram_ends)
     
     def get_ribbon_ends(self):
         n = self.shape
         arc_lens = self.data * self.conversion_rate
         regions = np.zeros((n, n+1))
         for i in range(n):
@@ -158,10 +180,15 @@
         fig.save_svg(filename)
 
     def save_png(self, filename):
         fig = self.show()
         fig.save_png(filename)
     
     def get_color(self, i):
-        n = len(self.color_map)
-        return self.color_map[i % n]
-        
+        n = len(self.colormap)
+        return self.colormap[i % n]
+
+    def show_colormap(self):
+        swatch = dw.Drawing(66*len(self.colormap), 60)
+        for i,col in enumerate(self.colormap):
+            swatch.append(dw.Rectangle(i*(66), 0, 60, 60, fill=self.colormap[i]))
+        return swatch
```

