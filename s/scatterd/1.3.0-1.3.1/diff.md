# Comparing `tmp/scatterd-1.3.0.tar.gz` & `tmp/scatterd-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.3.0.tar", last modified: Sat Apr 22 16:13:46 2023, max compression
+gzip compressed data, was "scatterd-1.3.1.tar", last modified: Sun Apr 23 09:54:36 2023, max compression
```

## Comparing `scatterd-1.3.0.tar` & `scatterd-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.905522 scatterd-1.3.0/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-04-22 16:13:46.905522 scatterd-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.896527 scatterd-1.3.0/scatterd/
--rw-rw-rw-   0        0        0     1570 2023-04-22 16:12:59.000000 scatterd-1.3.0/scatterd/__init__.py
--rw-rw-rw-   0        0        0     6836 2023-04-22 15:54:10.000000 scatterd-1.3.0/scatterd/examples.py
--rw-rw-rw-   0        0        0    20055 2023-04-22 16:09:15.000000 scatterd-1.3.0/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.904505 scatterd-1.3.0/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-04-22 16:13:46.911486 scatterd-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.160917 scatterd-1.3.1/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-04-23 09:54:36.161914 scatterd-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.153303 scatterd-1.3.1/scatterd/
+-rw-rw-rw-   0        0        0     1833 2023-04-22 20:09:57.000000 scatterd-1.3.1/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     6870 2023-04-22 20:10:09.000000 scatterd-1.3.1/scatterd/examples.py
+-rw-rw-rw-   0        0        0    20903 2023-04-22 23:31:27.000000 scatterd-1.3.1/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.160917 scatterd-1.3.1/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-23 09:54:36.000000 scatterd-1.3.1/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-04-23 09:54:36.163306 scatterd-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.1/setup.py
```

### Comparing `scatterd-1.3.0/LICENSE` & `scatterd-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.0/PKG-INFO` & `scatterd-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.0
+Version: 1.3.1
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.0.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.0 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.1 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.0.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.1.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.0/README.md` & `scatterd-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.0/scatterd/__init__.py` & `scatterd-1.3.1/scatterd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing, gradient_on_density_color
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Description
@@ -37,14 +37,18 @@
 >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True)
 >>>
 >>> # Scatter with density and gradient
 >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF')
 >>>
 >>> # Only density
 >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=None, density=True)
+>>>
+>>> # Various settings
+>>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, density_on_top=True, args_density={'alpha': 0.3}, gradient='#FFFFFF', edgecolor='#FFFFFF', grid=True, fontweight='normal', fontsize=26, legend=2)
+>>>
 
 References
 ----------
 * github: https://github.com/erdogant/scatterd
 * Documentation: https://erdogant.github.io/scatterd/
 * Colormap: https://matplotlib.org/examples/color/colormaps_reference.html
```

### Comparing `scatterd-1.3.0/scatterd/examples.py` & `scatterd-1.3.1/scatterd/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,20 @@
                    labels=df['labx'],
                    density=True,
                    density_on_top=True,
                    args_density={'alpha': 0.3},
                    gradient='#FFFFFF',
                    edgecolor='#FFFFFF',
                    grid=True,
-                   fontweight='bold',
+                   fontweight='normal',
                    fontsize=26,
+                   legend=2,
                    )
 
+
 # %%
 # Import example iris dataet
 from sklearn import datasets
 iris = datasets.load_iris()
 X = iris.data[:, :2]
 labels = iris.target
```

### Comparing `scatterd-1.3.0/scatterd/scatterd.py` & `scatterd-1.3.1/scatterd/scatterd.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
              gradient=None,
              density=False,
              density_on_top=False,
              norm=False,
              cmap='tab20c',
              figsize=(25, 15),
              dpi=100,
-             legend=True,
+             legend=None,
              jitter=None,
              xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, grid=False, fontweight='normal',
              args_density = {'cmap': 'Reds', 'fill': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False},
              visible=True,
              fig=None,
              ax=None,
              verbose=3):
@@ -91,16 +91,22 @@
         '#000000' : If the input is a single color, all fonts will get this color.
     grid: str or bool (default: False)
         False or None : Do not plot grid
         True : Set axis color to: '#dddddd'
         '#dddddd' : Specify color with hex
     norm : Bool, optional
         Normalize datapoints. The default is False.
-    legend : bool, (default: False)
-        Plot the legend.
+    legend : int, default: 0
+        None: Set automatically based number of labels.
+        False : Disable.
+        True : Best position.
+        1 : 'upper right'
+        2 : 'upper left'
+        3 : 'lower left'
+        4 : 'lower right'
     jitter : float, default: None
         Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
             * None or False: Do not add jitter
             * True : adds 0.01
             * 0.05 : Specify the amount jitter to add.
     cmap : String, optional
         'Set1'       (default)
@@ -149,14 +155,15 @@
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], gradient='#FFFFFF', cmap='Set2')
     >>>
     >>> # Scatter with density
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True)
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=False, gradient='#FFFFFF', edgecolor='#FFFFFF')
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF', edgecolor='#FFFFFF')
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF', c=None)
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, density_on_top=True, args_density={'alpha': 0.3}, gradient='#FFFFFF', edgecolor='#FFFFFF', grid=True, fontweight='normal', fontsize=26, legend=2)
     >>>
     >>> # Scatter with density and gradient
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF')
     >>>
 
     References
     -------
@@ -167,14 +174,15 @@
     """
     if len(x)!=len(y): raise Exception('[scatterd] >Error: input parameter x should be the same size of y.')
     if isinstance(c, str): raise Exception('[scatterd] >Error: input parameter c(olors) should be RGB of type tuple [0,0,0] .')
     if not isinstance(s, int) and len(s)!=len(x): raise Exception('[scatterd] >Error: input parameter s(ize) should be of same size of X.')
     if (z is not None) and len(x)!=len(z): raise Exception('[scatterd] >Error: input parameter z should be the same size of x and y.')
     if s is None: s=0
     if c is None: s, c = 0, [0, 0, 0]
+    if isinstance(s, (int, float)) and s==0: fontsize=0
     zorder = None if density_on_top else 10
 
     # Defaults
     defaults_density = {'cmap': 'Reds', 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}
     args_density = {**defaults_density, **args_density}
 
     # Preprocessing
@@ -197,50 +205,54 @@
     # Add density as bottom layer to the scatterplot
     if density:
         ax = sns.kdeplot(x=X[:, 0], y=X[:, 1], ax=ax, **args_density)
 
     # Scatter all at once
     if (labels is None) and isinstance(marker, str):
         if z is None:
-            ax.scatter(X[:, 0], X[:, 1], c=c_rgb, s=s, edgecolor=edgecolor, marker=marker, alpha=alpha)
+            ax.scatter(X[:, 0], X[:, 1], c=c_rgb, s=s, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
         else:
-            ax.scatter(X[:, 0], X[:, 1], X[:, 2], s=s, c=c_rgb, edgecolor=edgecolor, marker=marker, alpha=alpha)
+            ax.scatter(X[:, 0], X[:, 1], X[:, 2], s=s, c=c_rgb, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
     else:
         uilabels = np.unique(labels)
         for label in uilabels:
             Iloc1 = label==labels
             # Extract the unique markers
             for m in np.unique(marker[Iloc1]):
                 Iloc2 = np.logical_and(Iloc1, m==marker)
                 if z is None:
                     ax.scatter(X[Iloc2, 0], X[Iloc2, 1], c=c_rgb[Iloc2], s=s[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=alpha[Iloc2], zorder=zorder)
                 else:
-                    # Let op: alpha[Iloc2] geeft een foutmelding
-                    ax.scatter(X[Iloc2, 0], X[Iloc2, 1], X[Iloc2, 2], s=s[Iloc2], c=c_rgb[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=0.8)
+                    # Note: alpha[Iloc2] throws an error
+                    ax.scatter(X[Iloc2, 0], X[Iloc2, 1], X[Iloc2, 2], s=s[Iloc2], c=c_rgb[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=0.8, zorder=zorder)
 
     # Show legend (only if labels are present)
-    if legend and labels is not None: ax.legend()
+    if isinstance(legend, bool): legend = 0 if legend else -1
+    if legend is None: legend = -1 if len(np.unique(labels))>20 else 0
+    if legend>=0: ax.legend(loc=legend, fontsize=14)
 
     # Return
     return fig, ax
 
 
 # %% Setup figure properties
 def _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, ax):
     # Set axis fontsizes
     if grid is None: grid=False
     if grid is True: grid='#dddddd'
     font = {'family': 'DejaVu Sans', 'weight': fontweight, 'size': fontsize}
     matplotlib.rc('font', **font)
+    for item in ([ax.title, ax.xaxis.label, ax.yaxis.label] + ax.get_xticklabels() + ax.get_yticklabels()):
+        item.set_fontsize(20)
 
     # Plot labels
     if (labels is not None) and (fontcolor is not None):
         for uilabel in fontcolor.keys():
             # Compute median for better center compared to mean
-            XYmean = np.median(X[labels==uilabel, :], axis=0)
+            XYmean = np.mean(X[labels==uilabel, :], axis=0)
             if X.shape[1]==2:
                 ax.text(XYmean[0], XYmean[1], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize}, zorder=15)
             else:
                 ax.text(XYmean[0], XYmean[1], XYmean[2], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize})
 
     # Labels on axis
     ax.set_xlabel(xlabel)
@@ -432,14 +444,16 @@
     """Initialize figure."""
     if ax is None:
         fig = plt.figure(figsize=figsize, dpi=dpi)
         if z is None:
             ax = fig.add_subplot()
         else:
             ax = fig.add_subplot(projection='3d')
+            # Rotate
+            ax.view_init(-140, 60)
 
     if fig is not None:
         fig.set_visible(visible)
 
     return fig, ax
```

### Comparing `scatterd-1.3.0/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.1/scatterd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.0
+Version: 1.3.1
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.0.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.0 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.1 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.0.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.1.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.0/setup.py` & `scatterd-1.3.1/setup.py`

 * *Files identical despite different names*

