# Comparing `tmp/pca-1.9.2.tar.gz` & `tmp/pca-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-1.9.2.tar", last modified: Sat Mar 25 14:02:14 2023, max compression
+gzip compressed data, was "pca-2.0.0.tar", last modified: Sun Apr 23 10:11:34 2023, max compression
```

## Comparing `pca-1.9.2.tar` & `pca-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 14:02:14.314607 pca-1.9.2/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-1.9.2/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10006 2023-03-25 14:02:14.313609 pca-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     9441 2023-03-20 21:41:12.000000 pca-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 14:02:14.267511 pca-1.9.2/pca/
--rw-rw-rw-   0        0        0     1450 2023-03-25 13:33:51.000000 pca-1.9.2/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 14:02:14.302406 pca-1.9.2/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-1.9.2/pca/data/__init__.py
--rw-rw-rw-   0        0        0    28439 2023-03-25 14:01:28.000000 pca-1.9.2/pca/examples.py
--rw-rw-rw-   0        0        0    81898 2023-03-25 13:41:03.000000 pca-1.9.2/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-03-25 14:02:14.308910 pca-1.9.2/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-1.9.2/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10988 2023-03-25 13:33:15.000000 pca-1.9.2/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-03-25 14:02:14.300800 pca-1.9.2/pca.egg-info/
--rw-rw-rw-   0        0        0    10006 2023-03-25 14:02:13.000000 pca-1.9.2/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-03-25 14:02:14.000000 pca-1.9.2/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 14:02:13.000000 pca-1.9.2/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-03-25 14:02:13.000000 pca-1.9.2/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-25 14:02:13.000000 pca-1.9.2/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 14:02:14.314607 pca-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-03-25 13:43:46.000000 pca-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.050449 pca-2.0.0/
+-rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9981 2023-04-23 10:11:34.050449 pca-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9457 2023-04-23 08:28:30.000000 pca-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.033471 pca-2.0.0/pca/
+-rw-rw-rw-   0        0        0     1272 2023-04-23 09:53:19.000000 pca-2.0.0/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.048432 pca-2.0.0/pca/data/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.0/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    31375 2023-04-23 09:41:51.000000 pca-2.0.0/pca/examples.py
+-rw-rw-rw-   0        0        0    73611 2023-04-23 09:40:00.000000 pca-2.0.0/pca/pca.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.049428 pca-2.0.0/pca/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.0/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.0/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.047433 pca-2.0.0/pca.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:11:34.051423 pca-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.0/setup.py
```

### Comparing `pca-1.9.2/LICENSE` & `pca-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-1.9.2/PKG-INFO` & `pca-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 1.9.2
+Version: 2.0.0
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/1.9.2.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/logo.png" width="600" />
+  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
 
 
 
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/pypi/pyversions/pca)
 [![Pypi](https://img.shields.io/pypi/v/pca)](https://pypi.org/project/pca/)
@@ -102,15 +100,15 @@
           <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png?raw=true" width="400" />
         </a>
       </p>    
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#biplot">
-          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_biplot.png?raw=true" width="350" />
+          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/custom_example_2.png?raw=true" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
 
 
@@ -129,15 +127,15 @@
         <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_plot.png" width="350" />
         </a>
       </p>
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#d-plots">
-        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter3d.png" width="350" />
+        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_3d_density.png" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
 
 
@@ -235,9 +233,7 @@
 ---
 
 ## Support
 
 Your ❤️ is important to keep maintaining this package. You can [support](https://erdogant.github.io/pca/pages/html/Documentation.html) in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues and feature extensions at [github page](https://github.com/erdogant/pca).
 
 <a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: pca Version: 1.9.2 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.0 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/1.9.2.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE
-       [https://github.com/erdogant/pca/blob/master/docs/figs/logo.png]
+Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE
+   [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
 pca?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
@@ -48,19 +47,19 @@
 [documentation pages](https://erdogant.github.io/pca/) you can find detailed
 information about the working of the ``pca`` with many examples. --- ##
 Installation ```bash pip install pca ``` ##### Import pca package ```python
 from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
-fig_scatter.png?raw=true]              fig_biplot.png?raw=true]
+fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
-master/docs/figs/fig_plot.png]         master/docs/figs/fig_scatter3d.png]
+master/docs/figs/fig_plot.png]         master/docs/figs/iris_3d_density.png]
 # * [Example: Set alpha transparency](https://erdogant.github.io/pca/pages/
 html/Plots.html#alpha-transparency)
 [https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png]
 # * [Example: Normalizing out Principal Components](https://erdogant.github.io/
 pca/pages/html/Algorithm.html#normalizing-out-pcs) Normalizing out the 1st and
 more components from the data. This is usefull if the data is seperated in its
 first component(s) by unwanted or biased variance. Such as sex or experiment
```

### Comparing `pca-1.9.2/README.md` & `pca-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/logo.png" width="600" />
+  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
 
 
 
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/pypi/pyversions/pca)
 [![Pypi](https://img.shields.io/pypi/v/pca)](https://pypi.org/project/pca/)
@@ -85,15 +85,15 @@
           <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png?raw=true" width="400" />
         </a>
       </p>    
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#biplot">
-          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_biplot.png?raw=true" width="350" />
+          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/custom_example_2.png?raw=true" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
 
 
@@ -112,15 +112,15 @@
         <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_plot.png" width="350" />
         </a>
       </p>
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#d-plots">
-        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter3d.png" width="350" />
+        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_3d_density.png" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-       [https://github.com/erdogant/pca/blob/master/docs/figs/logo.png]
+   [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
 pca?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
@@ -40,19 +40,19 @@
 [documentation pages](https://erdogant.github.io/pca/) you can find detailed
 information about the working of the ``pca`` with many examples. --- ##
 Installation ```bash pip install pca ``` ##### Import pca package ```python
 from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
-fig_scatter.png?raw=true]              fig_biplot.png?raw=true]
+fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
-master/docs/figs/fig_plot.png]         master/docs/figs/fig_scatter3d.png]
+master/docs/figs/fig_plot.png]         master/docs/figs/iris_3d_density.png]
 # * [Example: Set alpha transparency](https://erdogant.github.io/pca/pages/
 html/Plots.html#alpha-transparency)
 [https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png]
 # * [Example: Normalizing out Principal Components](https://erdogant.github.io/
 pca/pages/html/Algorithm.html#normalizing-out-pcs) Normalizing out the 1st and
 more components from the data. This is usefull if the data is seperated in its
 first component(s) by unwanted or biased variance. Such as sex or experiment
```

### Comparing `pca-1.9.2/pca/__init__.py` & `pca-2.0.0/pca/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,53 +5,49 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.9.2'
+__version__ = '2.0.0'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
 Description
 -----------
 pca: A Python Package for Principal Component Analysis.
 
 Examples
 --------
 >>> from pca import pca
->>> # Load example data
->>> from sklearn.datasets import load_iris
->>> X = pd.DataFrame(data=load_iris().data, columns=load_iris().feature_names, index=load_iris().target)
 >>>
 >>> Initialize
 >>> model = pca(n_components=3)
->>> # Fit using PCA
->>> results = model.fit_transform(X)
 >>>
->>> # Make plots
->>> fig, ax = model.scatter()
+>>> # Load example data
+>>> df = model.import_example(data='iris')
+>>>
+>>> # Fit using PCA
+>>> results = model.fit_transform(df)
 >>>
 >>> # Scree plot together with explained variance.
 >>> fig, ax = model.plot()
 >>>
 >>> # Plot loadings
 >>> fig, ax = model.biplot()
->>>
->>> # Plot loadings with outliers
->>> fig, ax = model.biplot(SPE=True, hotellingt2=True)
+>>> fig, ax = model.biplot(density=True, SPE=True, HT2=True)
+>>> fig, ax = model.scatter()
 >>>
 >>> 3D plots
 >>> fig, ax = model.scatter3d()
->>> fig, ax = model.biplot3d()
->>> fig, ax = model.biplot3d(SPE=True, hotellingt2=True)
+>>> fig, ax = model.biplot3d(density=True, SPE=True, HT2=True)
 >>>
 >>> # Normalize out PCs
 >>> X_norm = model.norm(X)
 
 References
 ----------
 * Blog: https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559
```

### Comparing `pca-1.9.2/pca/examples.py` & `pca-2.0.0/pca/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,251 @@
 from pca import pca
 import pandas as pd
 import numpy as np
 import matplotlib as mpl
 
-# %% Test examples
-import pca
-# Import example
-df = pca.import_example('sprinkler')
-df = pca.import_example('titanic')
-df = pca.import_example('student')
+import numpy as np
+from sklearn.datasets import load_iris
+import pandas as pd
 
-# %% change marker
+
+# %%
+from sklearn.datasets import make_friedman1
+X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
+
+model = pca()
+model.fit_transform(X)
+
+# model.scatter(density=True)
+# model.biplot(c=[0,0,0], density=True)
+
+# model.scatter3d(fontsize=16, PC=[0,1,3])
+# model.scatter3d(density=True)
+
+model.biplot3d(arrowdict={'weight':'bold'},  c=None, n_feat=5)
+
+
+# %%
+from pca import pca
+from sklearn.datasets import load_wine
+import pandas as pd
+
+# Load dataset
+data = load_wine()
+X = data.data
+y = data.target
+labels = data.feature_names
+# Make dataframe
+df = pd.DataFrame(data=X, columns=labels, index=y)
+
+model = pca(normalize=True, n_components=None)
+# Fit transform with dataframe
+results = model.fit_transform(df)
+
+model.biplot(labels=df['flavanoids'].values, legend=False, cmap='seismic', n_feat=3, fontsize=20, arrowdict={'fontsize':28, 'c':'g'}, density=True)
+model.biplot3d(legend=False, n_feat=3, fontcolor='r', arrowdict={'fontsize':22, 'c':'k'}, density=True)
+
+
+# %% Demonstration of specifying colors, markers, alpha, and size per sample
 # Import library
 import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib.colors as mcolors
 from sklearn.datasets import make_friedman1
 from pca import pca
 
 # Make data set
 X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
 # All available markers
 markers = np.array(['.', 'o', 'v', '^', '<', '>', '8', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X'])
+# Create colors
+cmap = plt.cm.get_cmap('tab20c', len(markers))
 # Generate random integers
 random_integers = np.random.randint(0, len(markers), size=X.shape[0])
 # Draw markers
 marker = markers[random_integers]
+# Set colors
+color = cmap.colors[random_integers, 0:3]
+# Set Size
+size = np.random.randint(50, 1000, size=X.shape[0])
+# Set alpha
+alpha = np.random.rand(1, X.shape[0])[0][random_integers]
 
 # Init
 model = pca(verbose=3)
 # Fit
 model.fit_transform(X)
 # Make plot with blue arrows and text
-fig, ax = model.biplot(c=[0, 0, 0], 
-                       marker=marker,
-                       label=False,
-                       title='Demonstration of specifying colors, markers, alpha, and size per sample.',
-                       n_feat=5,
-                       legend=False)
+fig, ax = model.biplot(
+                        SPE=True,
+                        HT2=True,
+                        c=color,
+                        s=size,
+                        marker=marker,
+                        alpha=0.4,
+                        color_arrow='k',
+                        title='Demonstration of specifying colors, markers, alpha, and size per sample.',
+                        n_feat=5,
+                        fontsize=20,
+                        fontweight='normal',
+                        arrowdict={'fontsize': 18},
+                        density=True,
+                        density_on_top=False,
+                        )
 
 
-# %% Demonstration of specifying colors, markers, alpha, and size per sample
+# %%
+from df2onehot import df2onehot
+from pca import pca
+
+model = pca()
+df = model.import_example(data='titanic')
+
+# Create one-hot array
+df_hot = df2onehot(df,
+                   remove_mutual_exclusive=True,
+                   excl_background=['PassengerId', 'None'],
+                   y_min=10,
+                   verbose=4)['onehot']
+
+# Initialize
+model = pca(normalize=True, detect_outliers=['HT2', 'SPE'])
+
+# Fit
+model.fit_transform(df_hot)
+
+# model.scatter(legend=False)
+# model.biplot(legend=False)
+
+model.biplot(SPE=True,
+              HT2=True,
+              marker=df['Survived'],
+              s=df['Age']*20,
+              n_feat=2,
+              labels=df['Sex'],
+              title='Biplot with with the pca library.',
+              color_arrow='k',
+              fontsize=28,
+              fontcolor=None,
+              arrowdict={'fontsize': 18},
+              cmap='bwr_r',
+              edgecolor='#FFFFFF',
+              gradient='#FFFFFF',
+              density=True,
+              density_on_top=False,
+              visible=True,
+              )
+
+
+
+
+
+
+# %%
+# Load pca
+from pca import pca
+
+# Initialize pca
+model = pca()
+
+# Load example data set
+df = model.import_example(data='iris')
+
+# Fit transform
+results = model.fit_transform(X)
+
+# Make plot
+model.biplot(HT2=True,
+             SPE=True,
+             s=np.random.randint(20, 500, size=df.shape[0]),
+             marker=y,
+             cmap='bwr_r',
+             fontsize=22,
+             legend=2,
+             density=True,
+             title='Biplot with with the pca library.')
+
+# %%
+df = pd.read_pickle('WIM-data PCA bug')
+df = df.iloc[0:10000, :]
+X = df.drop(['SUBCATEGORIE','UTCPASSAGEDATUM','STROOKVOLGNUMMER','TWEESTROKEN'],axis=1)
+y = df['SUBCATEGORIE']
+model = pca(normalize=True, n_components=0.95)
+results = model.fit_transform(X, col_labels=X.columns, row_labels=y)
+
+# results = model.fit_transform(X)
+model.scatter3d()
+model.biplot3d()
+
+
+model.scatter()
+model.scatter(fontsize=20, c=None)
+model.scatter(fontsize=20, cmap=None)
+model.scatter(edgecolor='#FFFFFF')
+model.scatter(edgecolor='#FFFFFF', gradient='#FFFFFF')
+model.scatter(density=True)
+model.scatter(density=True, c=None)
+model.scatter(density=True, c=None, legend=False)
+model.scatter(density=True, c=None, fontsize=0)
+model.scatter(density=True, s=10, edgecolor=None, fontsize=0, alpha=0.2)
+
+model.scatter(fontsize=20)
+model.biplot()
+model.scatter(c=[0,0,0], legend=True)
+model.scatter(alpha=None)
+model.scatter(alpha=0.8)
+model.scatter(alpha=0.8, density=True)
+model.scatter(s=250, alpha=0.8, gradient='#FFFFFF', edgecolor=None)
+
+model.biplot()
+model.biplot(cmap=None, n_feat=5)
+model.biplot3d()
+model.biplot3d(cmap=None, n_feat=8)
+
+
+
+
+
+
+# %% Test examples
+import pca
+# Import example
+df = pca.import_example('sprinkler')
+df = pca.import_example('titanic')
+df = pca.import_example('student')
+
+# %% change marker
 # Import library
 import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.colors as mcolors
 from sklearn.datasets import make_friedman1
 from pca import pca
 
 # Make data set
 X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
 # All available markers
 markers = np.array(['.', 'o', 'v', '^', '<', '>', '8', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X'])
-# Create colors
-colors = plt.cm.get_cmap('tab20c', len(markers))
 # Generate random integers
 random_integers = np.random.randint(0, len(markers), size=X.shape[0])
 # Draw markers
 marker = markers[random_integers]
-# Set colors
-color = colors.colors[random_integers, :]
-# Set Size
-size = np.random.randint(50, 150, size=X.shape[0])
-# Set alpha
-alpha = np.random.rand(1, X.shape[0])[0][random_integers]
 
 # Init
 model = pca(verbose=3)
 # Fit
 model.fit_transform(X)
 # Make plot with blue arrows and text
-fig, ax = model.biplot(c=color,
-                       s=size,
+fig, ax = model.biplot(c=[0, 0, 0],
                        marker=marker,
-                       alpha_transparency=alpha,
-                       label=False,
-                       fontdict={'size':10, 'weight':'normal'},
-                       color_arrow='blue',
                        title='Demonstration of specifying colors, markers, alpha, and size per sample.',
-                       hotellingt2=True,
                        n_feat=5,
-                       legend=False, 
-                       visible=True)
+                       legend=None)
+
+
 
 
 # %%
 
 
 # Import library
 from pca import pca
@@ -131,15 +291,15 @@
 # 646      False       True   True  False  ...   False   False   False    True
 # 647      False       True  False   True  ...   False   False   False   False
 # 648      False       True  False   True  ...   False   False   False   False
 
 # [649 rows x 177 columns]
 
 model = pca(normalize=True,
-            detect_outliers=['ht2', 'spe'],
+            detect_outliers=['HT2', 'SPE'],
             alpha=0.05,
             n_std=3,
             multipletests='fdr_bh')
 
 results = model.fit_transform(df_hot)
 
 overlapping_outliers = np.logical_and(results['outliers']['y_bool'], results['outliers']['y_bool_spe'])
@@ -153,26 +313,25 @@
 # 610     MS   F   19       R     GT3       A  ...     4       1        0  8  0  0
 
 # [5 rows x 33 columns]
 
 
 # Make biplot
 model.biplot(SPE=True,
-             hotellingt2=True,
+             HT2=True,
              jitter=0.1,
              n_feat=10,
-             legend=True,
-             label=False,
-             y=df['sex'],
+             legend=False,
+             labels=df['sex'],
              title='Student Performance',
              figsize=(20, 12),
              color_arrow='k',
-             fontdict={'size':16, 'c':'k'},
-              cmap='bwr_r',
+             cmap='bwr_r',
              gradient='#FFFFFF',
+             density=True,
              )
 
 
 # %%
 # Import library
 from pca import pca
 from sklearn.datasets import make_friedman1
@@ -180,18 +339,18 @@
 
 # Init
 model = pca()
 # Fit
 model.fit_transform(X)
 
 # Make plot with blue arrows and text
-fig, ax = model.biplot(c=[0,0,0], s=25, fontdict={'size':10, 'weight':'normal'}, color_arrow='blue', title=None, hotellingt2=True, n_feat=10, visible=True)
+fig, ax = model.biplot(c=[0,0,0], fontsize=20, color_arrow='blue', title=None, HT2=True, n_feat=10, visible=True)
 
 # Use the existing fig and create new edits such red arrows for the first three loadings. Also change the font sizes.
-fig, ax = model.biplot(c=[0,0,0], s=25, fontdict={'size':16, 'weight':'bold'}, color_arrow='red', n_feat=3, title='updated fig.', visible=True, fig=fig)
+fig, ax = model.biplot(c=[0,0,0], fontsize=20, arrowdict={'weight':'bold'}, color_arrow='red', n_feat=3, title='updated fig.', visible=True, fig=fig)
 
 
 # %%
 # https://github.com/erdogant/pca/issues/40
 
 # Import iris dataset and other required libraries
 from sklearn.datasets import load_iris
@@ -214,34 +373,34 @@
 model.biplot()
 
 # Use custom cmap for classlabels (as an example I explicitely provide three colors).
 model.biplot(cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
 
 # Set custom classlabels. Coloring is based on the input colormap (cmap).
 y[10:15]=4
-model.biplot(y=y, cmap='Set2')
+model.biplot(labels=y, cmap='Set2')
 
 # Set custom classlabels and also use custom colors.
 c = colourmap.fromlist(y, cmap='Set2')[0]
 c[10:15] = [0,0,0]
-model.biplot(y=y, c=c)
+model.biplot(labels=y, c=c)
 
 
 # Remove scatterpoints by setting cmap=None
 model.biplot(cmap=None)
 
 
 # Color on classlabel (Unchanged)
 model.biplot()
 # Use cmap colors for classlabels (unchanged)
-model.biplot(y=y, cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
+model.biplot(labels=y, cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
 # Do not show points when cmap=None (unchanged)
-model.biplot(y=load_iris().target, cmap=None)
+model.biplot(labels=load_iris().target, cmap=None)
 # Plot all points as unique entity (unchanged)
-model.biplot(y=y, gradient='#ffffff', cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
+model.biplot(labels=y, gradient='#ffffff', cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
 
 
 # %%
 import numpy as np
 from sklearn.datasets import load_iris
 
 # Load dataset
@@ -253,97 +412,87 @@
 model = pca(n_components=3)
 results = model.fit_transform(X, verbose=2)
 
 
 model.scatter()
 model.scatter(gradient='#ffffff')
 model.scatter(gradient='#ffffff', cmap='tab20')
-model.scatter(gradient='#ffffff', cmap='tab20', y=np.ones_like(model.results['PC'].index.values))
+model.scatter(gradient='#ffffff', cmap='tab20', labels=np.ones_like(model.results['PC'].index.values))
 
 model.scatter(gradient='#5dfa02')
 model.scatter(gradient='#5dfa02', cmap='tab20')
-model.scatter(gradient='#5dfa02', cmap='tab20', y=np.ones_like(model.results['PC'].index.values))
+model.scatter(gradient='#5dfa02', cmap='tab20', labels=np.ones_like(model.results['PC'].index.values))
 
 
 # %%
 # import pca
 # print(pca.__version__)
 
 # np.random.seed(0)
 # x, y = np.random.random((2,30))
 # fig, ax = plt.subplots()
 # plt.plot(x, y, 'bo')
 # texts = [plt.text(x[i], y[i], 'Text%s' %i) for i in range(len(x))]
 # adjust_text(texts)
 
-# %%
-from sklearn.datasets import make_friedman1
-X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
-# model = pca(method='sparse_pca')
-model = pca(method='trunc_svd')
-model.fit_transform(X)
-model.plot(title=None)
-model.biplot(fontdict={'size':16, 'weight':'bold'}, title=None)
-model.biplot3d()
-model.scatter()
 
 # %% Detect outliers in new unseen data.
 # Import libraries
 from pca import pca
 import pandas as pd
 import numpy as np
 
 # Create dataset with 100 samples
 X = np.array(np.random.normal(0, 1, 500)).reshape(100, 5)
 
 # Initialize model. Alpha is the threshold for the hotellings T2 test to determine outliers in the data.
-model = pca(alpha=0.05, detect_outliers=['ht2', 'spe'])
+model = pca(alpha=0.05, detect_outliers=['HT2', 'SPE'])
 
 # Fit transform
 model.fit_transform(X)
 
 # Create 5 outliers
 X_unseen = np.array(np.random.uniform(5, 10, 25)).reshape(5, 5)
 
 # map the new "unseen" data in the existing space
 PCnew = model.transform(X_unseen)
 
 # Plot image
-model.biplot(SPE=True, hotellingt2=True)
+model.biplot(SPE=True, HT2=True, density=True)
 
 # %% Detect unseen outliers
 # Import libraries
 from pca import pca
 import pandas as pd
 import numpy as np
 
 # Create dataset with 100 samples
 X = np.array(np.random.normal(0, 1, 500)).reshape(100, 5)
 
 # Initialize model. Alpha is the threshold for the hotellings T2 test to determine outliers in the data.
-model = pca(alpha=0.05, detect_outliers=['ht2', 'spe'])
+model = pca(alpha=0.05, detect_outliers=['HT2', 'SPE'])
 # model = pca(alpha=0.05, detect_outliers=None)
 
 # Fit transform
 model.fit_transform(X)
 
-model.scatter(SPE=True, hotellingt2=True)
+model.scatter(SPE=True, HT2=True)
 
 for i in range(0, 10):
     # Create 5 outliers
     X_unseen = np.array(np.random.uniform(5, 10, 25)).reshape(5, 5)
 
     # Transform new "unseen" data.
     PCnew = model.transform(X_unseen, row_labels=np.repeat('mapped_' + str(i), X_unseen.shape[0]), update_outlier_params=True)
 
     # Scatterplot
-    model.scatter(SPE=True, hotellingt2=True)
+    model.scatter(SPE=True, HT2=True)
     # Biplot
-    # Model.biplot(SPE=True, hotellingt2=True)
+    # Model.biplot(SPE=True, HT2=True)
 
 
 # %%
 from sklearn.datasets import make_friedman1
 X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
 model = pca(method='sparse_pca')
@@ -380,23 +529,23 @@
 index_name[index_name=='1'] = load_iris().target_names[1]
 index_name[index_name=='2'] = load_iris().target_names[2]
 
 X = pd.DataFrame(data=load_iris().data, columns=load_iris().feature_names, index=index_name)
 model = pca(n_components=3, normalize=True)
 
 out = model.fit_transform(X)
-# fig, ax = model.biplot(label=True, legend=False, PC=[1,0])
+# fig, ax = model.biplot(legend=False, PC=[1,0])
 print(out['topfeat'])
 
-fig, ax = model.biplot(cmap='Set1', label=True, legend=True, fontdict={'size':16})
-fig, ax = model.biplot(cmap='Set1', label=True, legend=False)
-fig, ax = model.biplot(cmap='Set1', label=False, legend=False)
-fig, ax = model.biplot(cmap=None, label=False, legend=False)
-fig, ax = model.biplot(cmap=None, label=False, legend=True)
-fig, ax = model.biplot(cmap=None, label=False, legend=True)
+fig, ax = model.biplot(cmap='Set1', legend=True)
+fig, ax = model.biplot(cmap='Set1', legend=False)
+fig, ax = model.biplot(cmap='Set1', legend=False)
+fig, ax = model.biplot(cmap=None, legend=False)
+fig, ax = model.biplot(cmap=None, legend=True)
+fig, ax = model.biplot(cmap=None, legend=True)
 
 # %%
 import numpy as np
 from sklearn.datasets import load_iris
 
 # Load dataset
 X = pd.DataFrame(data=load_iris().data, columns=load_iris().feature_names, index=load_iris().target)
@@ -412,42 +561,42 @@
 
 # Fit transform
 results = model.fit_transform(X)
 
 # model.plot()
 
 model.scatter(gradient='#ffffff', cmap='Set1')
-model.scatter(cmap='Set1', legend=True, label=True, gradient='#ffffff')
-model.scatter(cmap='Set1', legend=True, label=True, gradient=None)
+model.scatter(cmap='Set1', legend=True, gradient='#ffffff')
+model.scatter(cmap='Set1', legend=True, gradient=None)
 
-model.scatter3d(cmap='Set1', legend=True, label=True, gradient='#ffffff')
-model.scatter3d(cmap='Set1', legend=True, label=True, gradient=None)
+model.scatter3d(cmap='Set1', legend=True, gradient='#ffffff')
+model.scatter3d(cmap='Set1', legend=True, gradient=None)
 
-model.biplot(legend=True, SPE=True, hotellingt2=True, visible=True, gradient='#ffffff')
-model.biplot(legend=True, SPE=True, hotellingt2=True, visible=True, gradient=None)
-model.biplot3d(legend=True, SPE=True, hotellingt2=True, visible=True, gradient=None)
-model.biplot3d(legend=True, SPE=True, hotellingt2=True, visible=True, gradient='#ffffff')
+model.biplot(legend=True, SPE=True, HT2=True, visible=True, gradient='#ffffff')
+model.biplot(legend=True, SPE=True, HT2=True, visible=True, gradient=None)
+model.biplot3d(legend=True, SPE=True, HT2=True, visible=True, gradient=None)
+model.biplot3d(legend=True, SPE=True, HT2=True, visible=True, gradient='#ffffff')
 
 
 # %%
 from pca import pca
 from sklearn.datasets import load_iris
 X = pd.DataFrame(data=load_iris().data, columns=load_iris().feature_names, index=load_iris().target)
 model = pca(n_components=3, normalize=True)
 
 out = model.fit_transform(X)
-# fig, ax = model.biplot(label=True, legend=False, PC=[1,0])
+# fig, ax = model.biplot(legend=False, PC=[1,0])
 print(out['topfeat'])
 
-fig, ax = model.biplot(cmap='Set1', label=True, legend=True)
-fig, ax = model.biplot(cmap='Set1', label=True, legend=False)
-fig, ax = model.biplot(cmap='Set1', label=False, legend=False)
-fig, ax = model.biplot(cmap=None, label=False, legend=False)
-fig, ax = model.biplot(cmap=None, label=False, legend=True)
-fig, ax = model.biplot(cmap=None, label=False, legend=True)
+fig, ax = model.biplot(cmap='Set1', legend=True)
+fig, ax = model.biplot(cmap='Set1', legend=False)
+fig, ax = model.biplot(cmap='Set1', legend=False)
+fig, ax = model.biplot(cmap=None, legend=False)
+fig, ax = model.biplot(cmap=None, legend=True)
+fig, ax = model.biplot(cmap=None, legend=True)
 
 
 # %%
 import numpy as np
 import pandas as pd
 from pca import pca
 
@@ -489,36 +638,36 @@
 # 7  PC1  feat_8 -0.000000  weak
 
 # Plot the explained variance
 model.plot()
 # Biplot with the loadings
 ax = model.biplot(legend=False)
 # Biplot with the loadings
-ax = model.biplot(n_feat=3, legend=False, label=False)
+ax = model.biplot(n_feat=3, legend=False, )
 # Cleaning the biplot by removing the scatter, and looking only at the top 3 features.
-ax = model.biplot(n_feat=3, legend=False, label=False, cmap=None)
+ax = model.biplot(n_feat=3, legend=False, cmap=None)
 # Make plot with 3 dimensions
-model.biplot3d(n_feat=3, legend=False, label=False, cmap=None)
+model.biplot3d(n_feat=3, legend=False, cmap=None)
 
-ax = model.biplot(n_feat=3, legend=False, label=False, cmap=None, PC=[1,2])
-ax = model.biplot(n_feat=3, legend=False, label=False, cmap=None, PC=[2,3])
+ax = model.biplot(n_feat=3, legend=False, cmap=None, PC=[1,2])
+ax = model.biplot(n_feat=3, legend=False, cmap=None, PC=[2,3])
 
 
-ax = model.biplot(n_feat=10, legend=False, cmap=None, label=False)
-ax = model.biplot(n_feat=10, legend=False, PC=[0, 1], label=None)
+ax = model.biplot(n_feat=10, legend=False, cmap=None, )
+ax = model.biplot(n_feat=10, legend=False, PC=[0, 1], )
 ax = model.biplot(n_feat=10, legend=False, PC=[1, 0])
 ax = model.biplot(n_feat=10, legend=False, PC=[0, 1, 2], d3=True)
 ax = model.biplot(n_feat=10, legend=False, PC=[2, 1, 0], d3=True)
 ax = model.biplot(n_feat=10, legend=False, PC=[2, 0, 1], d3=True)
 ax = model.biplot(n_feat=10, legend=False, PC=[0, 1])
 ax = model.biplot(n_feat=10, legend=False, PC=[0, 2])
 ax = model.biplot(n_feat=10, legend=False, PC=[2, 1])
 ax = model.biplot3d(n_feat=10, legend=False)
 
-# model.scatter(y=X.index.values==0)
+# model.scatter(labels=X.index.values==0)
 
 # %%
 from pca import pca
 
 # Initialize
 model = pca(alpha=0.05, n_std=2)
 
@@ -527,15 +676,15 @@
 X = np.random.randint(low=1, high=10, size=(n_total, n_features))
 
 # Example with Numpy array
 row_labels = np.arange(0, X.shape[0]).astype(str)
 # Fit transform
 out = model.fit_transform(X, row_labels=row_labels)
 # Make plot
-model.biplot(legend=False, PC=[0, 1], label=None)
+model.biplot(legend=False, PC=[0, 1], )
 
 # %%
 # Example with DataFrame
 X = pd.DataFrame(data=X, columns=np.arange(0, X.shape[1]).astype(str))
 # Fit transform
 out = model.fit_transform(X)
 # Make plot
@@ -592,17 +741,17 @@
 
 # Example with DataFrame
 X = np.array(np.random.normal(0, 1, 500)).reshape(100, 5)
 X = pd.DataFrame(data=X, columns=np.arange(0, X.shape[1]).astype(str))
 # Fit transform
 out = model.fit_transform(X)
 # Make plot
-fig, ax = model.biplot(cmap=None, label=False, legend=False, visible=True)
-fig, ax = model.biplot(cmap='Set2', label=True, legend=False, visible=True)
-fig, ax = model.biplot(cmap=None, label=False, legend=False, visible=False)
+fig, ax = model.biplot(cmap=None, legend=False, visible=True)
+fig, ax = model.biplot(cmap='Set2', legend=False, visible=True)
+fig, ax = model.biplot(cmap=None, legend=False, visible=False)
 
 
 # %%
 from pca import pca
 
 X = np.array(np.random.normal(0, 1, 500)).reshape(100, 5)
 outliers = np.array(np.random.uniform(5, 10, 25)).reshape(5, 5)
@@ -613,42 +762,42 @@
 # Fit transform
 out = model.fit_transform(X)
 out['topfeat']
 print(out['outliers'])
 
 model.biplot(legend=True, visible=True)
 
-model.biplot(legend=True, SPE=True, hotellingt2=True, visible=True)
-model.biplot(legend=True, SPE=True, hotellingt2=False)
-model.biplot(legend=True, SPE=False, hotellingt2=True)
-model.biplot(legend=True, SPE=False, hotellingt2=False)
-
-model.biplot3d(legend=True, SPE=True, hotellingt2=True)
-model.biplot3d(legend=True, SPE=True, hotellingt2=False)
-model.biplot3d(legend=True, SPE=False, hotellingt2=True)
-model.biplot3d(legend=True, SPE=False, hotellingt2=False)
-
-model.scatter(legend=True, SPE=True, hotellingt2=True)
-model.scatter(legend=True, SPE=True, hotellingt2=False)
-model.scatter(legend=True, SPE=False, hotellingt2=True)
-model.scatter(legend=True, SPE=False, hotellingt2=False)
-
-model.scatter3d(legend=True, SPE=True, hotellingt2=True, visible=True)
-model.scatter3d(legend=True, SPE=True, hotellingt2=False)
-model.scatter3d(legend=True, SPE=False, hotellingt2=True)
-model.scatter3d(legend=True, SPE=False, hotellingt2=False)
+model.biplot(legend=True, SPE=True, HT2=True, visible=True)
+model.biplot(legend=True, SPE=True, HT2=False)
+model.biplot(legend=True, SPE=False, HT2=True)
+model.biplot(legend=True, SPE=False, HT2=False)
+
+model.biplot3d(legend=True, SPE=True, HT2=True)
+model.biplot3d(legend=True, SPE=True, HT2=False)
+model.biplot3d(legend=True, SPE=False, HT2=True)
+model.biplot3d(legend=True, SPE=False, HT2=False)
+
+model.scatter(legend=True, SPE=True, HT2=True)
+model.scatter(legend=True, SPE=True, HT2=False)
+model.scatter(legend=True, SPE=False, HT2=True)
+model.scatter(legend=True, SPE=False, HT2=False)
+
+model.scatter3d(legend=True, SPE=True, HT2=True, visible=True)
+model.scatter3d(legend=True, SPE=True, HT2=False)
+model.scatter3d(legend=True, SPE=False, HT2=True)
+model.scatter3d(legend=True, SPE=False, HT2=False)
 
 
-ax = model.biplot(n_feat=4, legend=False, label=False)
+ax = model.biplot(n_feat=4, legend=False, )
 
 import pca
 outliers_hot = pca.hotellingsT2(out['PC'].values, alpha=0.05)
 outliers_spe = pca.spe_dmodx(out['PC'].values, n_std=2)
 
-model.biplot(SPE=True, hotellingt2=False)
+model.biplot(SPE=True, HT2=False)
 
 # Select the outliers
 Xoutliers = X[out['outliers']['y_bool'],:]
 
 # Select the other set
 Xnormal = X[~out['outliers']['y_bool'],:]
 
@@ -674,15 +823,15 @@
 # Fit transform
 out = model.fit_transform(X)
 
 # Transform new "unseen" data
 PCnew = model.transform(X_unseen)
 
 # Plot PC space
-model.scatter(alpha_transparency=0.5)
+model.scatter(alpha=0.5)
 # Plot the new "unseen" samples on top of the existing space
 plt.scatter(PCnew.iloc[:, 0], PCnew.iloc[:, 1], marker='x')
 
 
 # %%
 # from hnet import hnet
 # df = pd.read_csv('C://temp//usarrest.txt')
@@ -708,19 +857,19 @@
 # out['outliers']
 
 # ax = model.scatter(legend=False, )
 # ax = model.scatter3d(legend=False)
 
 # # Make plot
 # ax = model.biplot(n_feat=4, legend=False)
-# ax = model.biplot(n_feat=4, legend=False, label=False)
+# ax = model.biplot(n_feat=4, legend=False, )
 
 # ax = model.biplot3d(n_feat=1, legend=False)
 # ax = model.biplot3d(n_feat=2, legend=False)
-# ax = model.biplot3d(n_feat=4, legend=False, label=False)
+# ax = model.biplot3d(n_feat=4, legend=False, )
 
 # %%
 from sklearn.datasets import load_iris
 import pandas as pd
 from pca import pca
 
 # Initialize
@@ -869,18 +1018,18 @@
 model2.fit_transform(X)
 model2.plot()
 model2.biplot(n_feat=4)
 model2.scatter()
 model2.biplot3d(n_feat=10)
 
 # Set custom transparency levels
-model2.biplot3d(n_feat=10, alpha_transparency=0.5)
-model2.biplot(n_feat=10, alpha_transparency=0.5)
-model2.scatter3d(alpha_transparency=0.5)
-model2.scatter(alpha_transparency=0.5)
+model2.biplot3d(n_feat=10, alpha=0.5)
+model2.biplot(n_feat=10, alpha=0.5)
+model2.scatter3d(alpha=0.5)
+model2.scatter(alpha=0.5)
 
 
 model = pca(normalize=False, method='pca')
 model.fit_transform(X)
 model.biplot(n_feat=3)
 
 # Initialize
```

### Comparing `pca-1.9.2/pca/pca.py` & `pca-2.0.0/pca/pca.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """pca: A Python Package for Principal Component Analysis."""
 
 # %% Libraries
 import requests
 from urllib.parse import urlparse
 from tqdm import tqdm
-import scatterd as scatterd
+from scatterd import scatterd
 from sklearn.decomposition import PCA, SparsePCA, TruncatedSVD  # MiniBatchSparsePCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.metrics.pairwise import euclidean_distances
 from scipy import stats
-from mpl_toolkits.mplot3d import Axes3D
 from matplotlib.patches import Ellipse
 import scipy.sparse as sp
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 from adjustText import adjust_text
@@ -76,14 +75,16 @@
     * Documentation: https://erdogant.github.io/pca/
 
     """
 
     def __init__(self, n_components=0.95, n_feat=25, method='pca', alpha=0.05, multipletests='fdr_bh', n_std=3, onehot=False, normalize=False, detect_outliers=['ht2', 'spe'], random_state=None, verbose=3):
         """Initialize pca with user-defined parameters."""
         if isinstance(detect_outliers, str): detect_outliers = [detect_outliers]
+        if detect_outliers is not None: detect_outliers=list(map(str.lower, detect_outliers))
+
         if onehot:
             if verbose>=3: print('[pca] >Method is set to: [sparse_pca] because onehot=True.')
             method = 'sparse_pca'
 
         # Store in object
         self.n_components = n_components
         self.method = method.lower()
@@ -227,20 +228,20 @@
         >>> # Fit using PCA
         >>> results = model.fit_transform(X)
         >>>
         >>> # Make plots
         >>> fig, ax = model.scatter()
         >>> fig, ax = model.plot()
         >>> fig, ax = model.biplot()
-        >>> fig, ax = model.biplot(SPE=True, hotellingt2=True)
+        >>> fig, ax = model.biplot(SPE=True, HT2=True)
         >>>
         >>> 3D plots
         >>> fig, ax = model.scatter3d()
         >>> fig, ax = model.biplot3d()
-        >>> fig, ax = model.biplot3d(SPE=True, hotellingt2=True)
+        >>> fig, ax = model.biplot3d(SPE=True, HT2=True)
         >>>
         >>> # Normalize out PCs
         >>> X_norm = model.norm(X)
 
         """
         if verbose is None: verbose = self.verbose
         percentExplVar=None
@@ -341,16 +342,14 @@
         # Return
         return loadings
 
     # Top scoring components
     def compute_topfeat(self, loadings=None, verbose=3):
         """Compute the top-scoring features.
 
-        Description
-        -----------
         Per Principal Component, the feature with absolute maximum loading is stored.
         This can result into the detection of PCs that contain the same features. The feature that were never detected are stored as "weak".
 
         Parameters
         ----------
         loadings : array-like
             The array containing the loading information of the Principal Components.
@@ -414,39 +413,47 @@
         if self.n_components is None:
             self.n_components = X.shape[1] - 1
             if verbose>=3: print('[pca] >n_components is set to %d' %(self.n_components))
 
         self.n_feat = np.min([self.n_feat, X.shape[1]])
 
         if (not self.onehot) and (not self.normalize) and isinstance(X, pd.DataFrame) and (str(X.values.dtype)=='bool'):
-            if verbose>=2: print('[pca] >Warning: Sparse or one-hot boolean input data is detected, it is highly recommended to set onehot=True or alternatively, normalize=True')
-
-        # if sp.issparse(X):
-            # if verbose>=1: print('[PCA] Error: A sparse matrix was passed, but dense data is required for method=barnes_hut. Use X.toarray() to convert to a dense numpy array if the array is small enough for it to fit in memory.')
-        if isinstance(X, pd.DataFrame):
-            if verbose>=3: print('[pca] >Processing dataframe..')
+            if verbose>=2: print('[pca] >[WARNING]: Sparse or one-hot boolean input data is detected, it is highly recommended to set onehot=True or alternatively, normalize=True')
+        
+        # Set col labels
+        if isinstance(X, pd.DataFrame) and col_labels is None:
+            if verbose>=3: print('[pca] >Extracting column labels from dataframe.')
             col_labels = X.columns.values
-            row_labels = X.index.values
-            X = X.values
-        if sp.issparse(X) and self.normalize:
-            if verbose>=3: print('[pca] >Can not normalize a sparse matrix. Normalize is set to [False]')
-            self.normalize=False
         if col_labels is None or len(col_labels)==0 or len(col_labels)!=X.shape[1]:
             if verbose>=3: print('[pca] >Column labels are auto-completed.')
             col_labels = np.arange(1, X.shape[1] + 1).astype(str)
+        # if isinstance(col_labels, list):
+        col_labels=np.array(col_labels)
+
+        # Set row labels
+        if isinstance(X, pd.DataFrame) and row_labels is None:
+            if verbose>=3: print('[pca] >Extracting row labels from dataframe.')
+            row_labels = X.index.values
         if row_labels is None or len(row_labels)!=X.shape[0]:
-            row_labels=np.ones(X.shape[0])
+            # row_labels = np.ones(X.shape[0]).astype(int)
+            row_labels = np.arange(0, X.shape[0]).astype(int)
             if verbose>=3: print('[pca] >Row labels are auto-completed.')
-        if isinstance(row_labels, list):
-            row_labels=np.array(row_labels)
-        if isinstance(col_labels, list):
-            col_labels=np.array(col_labels)
+        # if isinstance(row_labels, list):
+        row_labels=np.array(row_labels)
+        
+
+        if isinstance(X, pd.DataFrame):
+            X = X.values
+
+        if sp.issparse(X) and self.normalize:
+            if verbose>=3: print('[pca] >[WARNING]: Can not normalize a sparse matrix. Normalize is set to [False]')
+            self.normalize=False
         if (sp.issparse(X) is False) and (self.n_components > X.shape[1]):
             # raise Exception('[pca] >Number of components can not be more then number of features.')
-            if verbose>=2: print('[pca] >Warning: >Number of components can not be more then number of features. n_components is set to %d' %(X.shape[1] - 1))
+            if verbose>=2: print('[pca] >[WARNING]: >Number of components can not be more then number of features. n_components is set to %d' %(X.shape[1] - 1))
             self.n_components = X.shape[1] - 1
 
         # normalize data
         if self.normalize:
             if verbose>=3: print('[pca] >Normalizing input data per feature (zero mean and unit variance)..')
             # Plot the data distribution
             # fig,(ax1,ax2)=plt.subplots(1,2, figsize=(15,5))
@@ -466,472 +473,332 @@
             # Plot the data distribution
             # ax2.hist(X.ravel().astype(float), bins=50)
             # ax2.set_ylabel('frequency')
             # ax2.set_xlabel('Values')
             # ax2.set_title('Zero-mean with unit variance normalized')
             # ax2.grid(True)
 
-        return (X, row_labels, col_labels, scaler)
+        return X, row_labels, col_labels, scaler
 
     # Figure pre processing
-    def _fig_preprocessing(self, y, n_feat, d3):
+    def _fig_preprocessing(self, labels, n_feat, d3):
         if hasattr(self, 'PC'): raise Exception('[pca] >Error: Principal components are not derived yet. Tip: run fit_transform() first.')
         if self.results['PC'].shape[1]<1: raise Exception('[pca] >Requires at least 1 PC to make plot.')
 
         if (n_feat is not None):
             topfeat = self.compute_topfeat()
             # n_feat = np.maximum(np.minimum(n_feat, self.results['loadings'].shape[0]), 2)
         else:
             topfeat = self.results['topfeat']
             n_feat = self.n_feat
 
         if d3:
-            n_feat = np.maximum(np.minimum(n_feat, self.results['loadings'].shape[1]), 3)
+            n_feat = np.maximum(np.minimum(n_feat, self.results['loadings'].shape[1]), 1)
         else:
-            n_feat = np.maximum(np.minimum(n_feat, self.results['loadings'].shape[1]), 2)
+            n_feat = np.maximum(np.minimum(n_feat, self.results['loadings'].shape[1]), 1)
 
-        if (y is not None):
-            if len(y)!=self.results['PC'].shape[0]: raise Exception('[pca] >Error: Input variable [y] should have some length as the number input samples: [%d].' %(self.results['PC'].shape[0]))
-            y = y.astype(str)
+        if (labels is not None):
+            if len(labels)!=self.results['PC'].shape[0]: raise Exception('[pca] >Error: Input variable [labels] should have some length as the number input samples: [%d].' %(self.results['PC'].shape[0]))
+            labels = labels.astype(str)
         else:
-            y = self.results['PC'].index.values.astype(str)
+            labels = self.results['PC'].index.values.astype(str)
+
+        # if all labels appear to be not uniuqe. Do not plot because it takes to much time.
+        if len(np.unique(labels))==self.results['PC'].shape[0]: labels=None
 
         if self.method=='sparse_pca':
             print('[pca] >sparse pca does not supported variance ratio and therefore, biplots will not be supported. <return>')
             self.results['explained_var'] = [None, None]
             self.results['model'].explained_variance_ratio_ = [0, 0]
             self.results['pcp'] = 0
 
         if (self.results['explained_var'] is None) or len(self.results['explained_var'])<=1:
             raise Exception('[pca] >Error: No PCs are found with explained variance.')
 
-        return y, topfeat, n_feat
-
-    # Scatter plot
-    def scatter3d(self,
-                  y=None,
-                  c=None,
-                  s=50,
-                  marker='.',
-                  jitter=None,
-                  label=True,
-                  PC=[0, 1, 2],
-                  SPE=False,
-                  hotellingt2=False,
-                  alpha_transparency=1,
-                  gradient=None,
-                  fontdict={'weight': 'normal', 'size': 12, 'ha': 'center', 'va': 'center', 'c': 'black'},
-                  cmap='Set1',
-                  title=None,
-                  legend=True,
-                  figsize=(15, 10),
-                  visible=True,
-                  fig=None,
-                  ax=None,
-                  verbose=None):
-        """Scatter 3d plot.
-
-        Parameters
-        ----------
-        y : array-like, default: None
-            Label for each sample. The labeling is used for coloring the samples.
-        c: list/array of RGB colors for each sample.
-            Color of samples in RGB colors.
-            [0,0,0]: If a single color is given, all samples get that color.
-        s: Int or list/array (default: 50)
-            Size(s) of the scatter-points.
-            [20, 10, 50, ...]: In case of list: should be same size as the number of PCs -> .results['PC']
-            50: all points get this size.
-        marker: list/array of strings (default: '.').
-            Marker for the samples.
-            '.' : All data points get this marker
-            ['.', '*', 's', ..]: Specify per sample the marker type.
-        jitter : float, default: None
-            Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
-        label : Bool, default: True
-            True Show the labels.
-            False: Do not show the labels
-            None: Ignore all labels (this will significanly speed up the scatterplot)
-        PC : list, default : [0, 1, 2]
-            Plot the first three Principal Components. Note that counting starts from 0. PC1=0, PC2=1, PC3=2, etc
-        SPE : Bool, default: False
-            Show the outliers based on SPE/DmodX method.
-        hotellingt2 : Bool, default: False
-            Show the outliers based on the hotelling T2 test.
-        alpha_transparency: float or array-like of floats (default: 1).
-            The alpha blending value ranges between 0 (transparent) and 1 (opaque).
-            1: All data points get this alpha
-            [1, 0.8, 0.2, ...]: Specify per sample the alpha
-        gradient : String, (default: None)
-            Hex (ending) color for the gradient of the scatterplot colors.
-            '#FFFFFF'
-        fontdict : dict.
-            dictionary containing properties for the arrow font-text
-            {'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': 'black'}
-        cmap : String, optional, default: 'Set1'
-            Colormap. If set to None, no points are shown.
-        title : str, default: None
-            Title of the figure.
-            None: Automatically create title text based on results.
-            '' : Remove all title text.
-            'title text' : Add custom title text.
-        legend : Bool, default: True
-            Show the legend based on the unique y-labels.
-        figsize : (int, int), optional, default: (15, 10)
-            (width, height) in inches.
-        visible : Bool, default: True
-            Visible status of the Figure. When False, figure is created on the background.
-        Verbose : int (default : 3)
-            Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace
-
-        Returns
-        -------
-        tuple containing (fig, ax)
-
-        """
-        if verbose is None: verbose = self.verbose
-        if self.results['PC'].shape[1]>=3:
-            fig, ax = self.scatter(y=y,
-                                   c=c,
-                                   s=s,
-                                   marker=marker,
-                                   jitter=jitter,
-                                   d3=True,
-                                   label=label,
-                                   PC=PC, SPE=SPE,
-                                   hotellingt2=hotellingt2,
-                                   alpha_transparency=alpha_transparency,
-                                   gradient=gradient,
-                                   fontdict=fontdict,
-                                   cmap=cmap,
-                                   title=title,
-                                   legend=legend,
-                                   figsize=figsize,
-                                   visible=visible,
-                                   fig=fig,
-                                   ax=ax,
-                                   verbose=verbose)
-        else:
-            print('[pca] >Error: There are not enough PCs to make a 3d-plot.')
-            fig, ax = None, None
-        return fig, ax
+        return labels, topfeat, n_feat
 
     # Scatter plot
     def scatter(self,
-                y=None,
-                c=None,
-                s=50,
-                marker='.',
-                jitter=None,
-                d3=False,
-                label=True,
-                PC=[0, 1],
+                labels=None,
+                c=[0,0.1,0.4],
+                s=150,
+                marker='o',
+                edgecolor='#000000',
                 SPE=False,
-                hotellingt2=False,
-                alpha_transparency=1,
+                HT2=False,
+                jitter=None,
+                PC=None,
+                alpha=0.8,
                 gradient=None,
-                fontdict={'weight': 'normal', 'size': 12, 'ha': 'center', 'va': 'center', 'c': 'black'},
-                cmap='Set1',
+                density=False,
+                density_on_top=False,
+                fontcolor=[0,0,0],
+                fontsize=18,
+                fontweight='normal',
+                cmap='tab20c',
                 title=None,
-                legend=True,
-                figsize=(20, 15),
+                legend=None,
+                figsize=(25, 15),
+                dpi=100,
                 visible=True,
                 fig=None,
                 ax=None,
+                y=None,  # deprecated
+                label=None,  # deprecated
                 verbose=3):
         """Scatter 2d plot.
 
         Parameters
         ----------
-        y : array-like, default: None
+        labels : array-like, default: None
             Label for each sample. The labeling is used for coloring the samples.
         c: list/array of RGB colors for each sample.
-            Color of samples in RGB colors.
-            [0,0,0]: If a single color is given, all samples get that color.
+            The marker colors. Possible values:
+                * A scalar or sequence of n numbers to be mapped to colors using cmap and norm.
+                * A 2D array in which the rows are RGB or RGBA.
+                * A sequence of colors of length n.
+                * A single color format string.
         s: Int or list/array (default: 50)
             Size(s) of the scatter-points.
             [20, 10, 50, ...]: In case of list: should be same size as the number of PCs -> .results['PC']
             50: all points get this size.
-        marker: list/array of strings (default: '.').
+        marker: list/array of strings (default: 'o').
             Marker for the samples.
-            '.' : All data points get this marker
-            ['.', '*', 's', ..]: Specify per sample the marker type.
+                * 'x' : All data points get this marker
+                * ('.', 'o', 'v', '^', '<', '>', '8', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X') : Specify per sample the marker type.
         jitter : float, default: None
             Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
-        d3 : Bool, default: False
-            3d plot is created when True.
-        label : Bool, default: True
-            True Show the labels.
-            False: Do not show the labels
-            None: Ignore all labels (this will significanly speed up the scatterplot)
-        PC : list, default : [0, 1]
-            Plot the first two Principal Components. Note that counting starts from 0. PC1=0, PC2=1, PC3=2, etc
+        PC : tupel, default: None
+            Plot the selected Principal Components. Note that counting starts from 0. PC1=0, PC2=1, PC3=2, etc.
+            None : Take automatically the first 2 components and 3 in case d3=True.
+            [0, 1] : Define the PC for 2D.
+            [0, 1, 2] : Define the PCs for 3D
         SPE : Bool, default: False
             Show the outliers based on SPE/DmodX method.
-        hotellingt2 : Bool, default: False
+                * None : Auto detect. If outliers are detected. it is set to True.
+                * True : Show outliers
+                * False : Do not show outliers
+        HT2 : Bool, default: False
             Show the outliers based on the hotelling T2 test.
-        alpha_transparency: float or array-like of floats (default: 1).
+                * None : Auto detect. If outliers are detected. it is set to True.
+                * True : Show outliers
+                * False : Do not show outliers
+        alpha: float or array-like of floats (default: 1).
             The alpha blending value ranges between 0 (transparent) and 1 (opaque).
             1: All data points get this alpha
             [1, 0.8, 0.2, ...]: Specify per sample the alpha
         gradient : String, (default: None)
             Hex color to make a lineair gradient for the scatterplot.
             '#FFFFFF'
-        fontdict : dict.
-            dictionary containing properties for the arrow font-text
-            {'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': 'black'}
+        density : Bool (default: False)
+            Include the kernel density in the scatter plot.
+        density_on_top : bool, (default: False)
+            True : The density is the highest layer.
+            False : The density is the lowest layer.
+        fontsize : String, optional
+            The fontsize of the y labels that are plotted in the graph. The default is 16.
+        fontcolor: list/array of RGB colors with same size as X (default : None)
+            None : Use same colorscheme as for c
+            '#000000' : If the input is a single color, all fonts will get this color.
         cmap : String, optional, default: 'Set1'
             Colormap. If set to None, no points are shown.
         title : str, default: None
             Title of the figure.
             None: Automatically create title text based on results.
             '' : Remove all title text.
             'title text' : Add custom title text.
-        legend : Bool, default: True
-            Show the legend based on the unique y-labels.
-        figsize : (int, int), optional, default: (15, 10)
+        legend : int, default: None
+            None: Set automatically based on number of labels.
+            False : No legend.
+            True : Best position.
+            1 : 'upper right'
+            2 : 'upper left'
+            3 : 'lower left'
+            4 : 'lower right'
+        figsize : (int, int), optional, default: (25, 15)
             (width, height) in inches.
         visible : Bool, default: True
             Visible status of the Figure. When False, figure is created on the background.
         Verbose : int (default : 3)
             Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace
 
         Returns
         -------
         tuple containing (fig, ax)
 
         """
         if verbose is None: verbose = self.verbose
-        if c is None: c=[[0, 0, 0]]
-        if (gradient is not None) and ((not isinstance(gradient, str)) or (len(gradient)!=7)): raise Exception('[pca]> Error: gradient must be of type string with Hex color or None.')
-        fontdict = _set_fontdict(fontdict)
-
-        # Setup figure
-        if fig is None and ax is None:
-            # Create entire new figure.
-            fig = plt.figure(figsize=figsize)
-            if d3:
-                ax = fig.add_subplot(projection='3d')
-            else:
-                ax = fig.add_subplot()
-        elif fig is not None and ax is None:
-            # Extract axes from fig.
-            ax = fig.axes[0]
-
-        # fig, ax = plt.subplots(figsize=figsize, edgecolor='k')
-        if fig is not None:
-            fig.set_visible(visible)
-
-        # Mark the outliers for plotting purposes.
-        Ioutlier1 = np.repeat(False, self.results['PC'].shape[0])
-        Ioutlier2 = np.repeat(False, self.results['PC'].shape[0])
+        _show_deprecated_warning(label, y, verbose)
+        if not hasattr(self, 'results'):
+            if verbose>=2: print('[pca]> No results to plot. Hint: model.fit(X) <return>.')
+            return None, None
 
-        if y is None:
-            y, _, _ = self._fig_preprocessing(y, None, d3)
+        # Set parameters based on intuition
+        if c is None: s=0
+        if cmap is None: s=0
+        if alpha is None: alpha=0.8
+        if PC is None: PC=[0, 1]
+        d3 = True if len(PC)==3 else False
 
+        # Set the labels
+        if labels is None: labels, _, _ = self._fig_preprocessing(labels, None, d3)
         # Get coordinates
-        xs, ys, zs, ax = _get_coordinates(self.results['PC'], PC, fig, ax, d3)
-
-        # Set the markers
-        if marker is None: marker='.'
-        if isinstance(marker, str): marker = np.repeat(marker, len(xs))
-        marker = np.array(marker)
-        if len(marker)!=len(xs): raise Exception('Marker length (k=%d) should match the number of samples (n=%d).' %(len(marker), len(xs)))
-
-        # Set Alpha
-        if alpha_transparency is None: alpha_transparency=1
-        if isinstance(alpha_transparency, (float, int)): alpha_transparency = np.repeat(alpha_transparency, len(xs))
-        alpha_transparency = np.array(alpha_transparency)
-        if len(alpha_transparency)!=len(xs): raise Exception('alpha_transparency length (k=%d) should match the number of samples (n=%d).' %(len(alpha_transparency), len(xs)))
-
-        # Set Size
-        if s is None: s=50
-        if isinstance(s, (float, int)): s = np.repeat(s, len(xs))
-        s = np.array(s)
-        if len(s)!=len(xs): raise Exception('Size (s) length (k=%d) should match the number of samples (n=%d).' %(len(s), len(xs)))
-
-        # Add jitter
-        if jitter is not None:
-            xs = xs + np.random.normal(0, jitter, size=len(xs))
-            if ys is not None: ys = ys + np.random.normal(0, jitter, size=len(ys))
-            if zs is not None: zs = zs + np.random.normal(0, jitter, size=len(zs))
-
-        # Get the colors
-        if cmap is None:
-            # Hide the scatterpoints by making them all white.
-            getcolors = np.repeat([1., 1., 1.], len(y), axis=0).reshape(-1, 3)
-        else:
-            # Figure properties
-            xyz, _ = scatterd._preprocessing(xs, ys, zs, y)
-            getcolors, fontcolor = scatterd.set_colors(xyz, y, None, c, cmap, gradient=gradient)
-
-        if hotellingt2 and ('y_bool' in self.results['outliers'].columns):
-            Ioutlier1 = self.results['outliers']['y_bool'].values
-        if SPE and ('y_bool_spe' in self.results['outliers'].columns):
-            Ioutlier2 = self.results['outliers']['y_bool_spe'].values
-            if not d3:
-                # Plot the ellipse
-                g_ellipse = spe_dmodx(np.c_[xs, ys], n_std=self.n_std, color='green', calpha=0.3, verbose=0)[1]
-                if g_ellipse is not None: ax.add_artist(g_ellipse)
-
-        # Make scatter plot of all not-outliers
-        # uiy = np.unique(y)
-        # if (len(uiy)==len(y)) and (len(uiy)>=1000) and (label is not None) and np.unique(marker)==1:
-        #     if verbose>=2: print('[pca] >Set parameter "label=None" to ignore the labels and significanly speed up the scatter plot.')
-        # Add the labels
-        # if (label is None):
-        #     if d3:
-        #         ax.scatter(xs, ys, zs, s=s, alpha=alpha_transparency, color=getcolors, label=None, marker=marker[0])
-        #     else:
-        #         ax.scatter(xs, ys, s=s, alpha=alpha_transparency, color=getcolors, label=None, marker=marker[0])
-        # else:
-        for Iloc_sampl, _ in tqdm(enumerate(y), desc="[pca] >Plotting", position=0, leave=False, disable=(verbose==0)):
-            if d3:
-                ax.scatter(xs[Iloc_sampl], ys[Iloc_sampl], zs[Iloc_sampl], s=np.maximum(s[Iloc_sampl], 0), label=y[Iloc_sampl], alpha=float(alpha_transparency[Iloc_sampl]), color=getcolors[Iloc_sampl, :], marker=marker[Iloc_sampl])
-                if label: ax.text(np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]), np.mean(zs[Iloc_sampl]), str(y[Iloc_sampl]), color=[0, 0, 0], fontdict=fontdict)
-            else:
-                ax.scatter(xs[Iloc_sampl], ys[Iloc_sampl], s=np.maximum(s[Iloc_sampl], 0), label=y[Iloc_sampl], alpha=float(alpha_transparency[Iloc_sampl]), color=getcolors[Iloc_sampl, :], marker=marker[Iloc_sampl])
-                if label: ax.text(np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]), str(y[Iloc_sampl]), color=[0, 0, 0], fontdict=fontdict)
-                # if label: ax.annotate(yk, np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]))
-
-            # for yk in uiy:
-            #     Iloc_sampl = (yk==y)
-
-            #     if d3:
-            #         ax.scatter(xs[Iloc_sampl], ys[Iloc_sampl], zs[Iloc_sampl], s=s + 10, label=yk, alpha=alpha_transparency, color=getcolors[Iloc_sampl, :], marker=marker[Iloc_sampl])
-            #         if label: ax.text(np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]), np.mean(zs[Iloc_sampl]), str(yk), color=[0, 0, 0], fontdict=fontdict)
-            #     else:
-            #         ax.scatter(xs[Iloc_sampl], ys[Iloc_sampl], s=s + 10, label=yk, alpha=alpha_transparency, color=getcolors[Iloc_sampl, :], marker=marker[Iloc_sampl])
-            #         if label: ax.text(np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]), str(yk), color=[0, 0, 0], fontdict=fontdict)
-            #         # if label: ax.annotate(yk, np.mean(xs[Iloc_sampl]), np.mean(ys[Iloc_sampl]))
-
-        # Plot outliers for hotelling T2 test.
-        if SPE and ('y_bool_spe' in self.results['outliers'].columns):
-            label_spe = str(sum(Ioutlier2)) + ' outliers (SPE/DmodX)'
-            if d3:
-                ax.scatter(xs[Ioutlier2], ys[Ioutlier2], zs[Ioutlier2], marker='x', color=[0.5, 0.5, 0.5], s=50, label=label_spe, alpha=alpha_transparency)
-            else:
-                ax.scatter(xs[Ioutlier2], ys[Ioutlier2], marker='d', color=[0.5, 0.5, 0.5], s=50, label=label_spe, alpha=alpha_transparency)
-                # Plot the ellipse
-                # g_ellipse = spe_dmodx(np.c_[xs, ys], n_std=self.n_std, color='green', calpha=0.3, verbose=0)[1]
-                # if g_ellipse is not None: ax.add_artist(g_ellipse)
-
-        # Plot outliers for hotelling T2 test.
-        if hotellingt2 and ('y_bool' in self.results['outliers'].columns):
-            label_t2 = str(sum(Ioutlier1)) + ' outliers (hotelling t2)'
-            if d3:
-                ax.scatter(xs[Ioutlier1], ys[Ioutlier1], zs[Ioutlier1], marker='d', color=[0, 0, 0], s=50, label=label_t2, alpha=alpha_transparency)
-            else:
-                ax.scatter(xs[Ioutlier1], ys[Ioutlier1], marker='x', color=[0, 0, 0], s=50, label=label_t2, alpha=alpha_transparency)
-
-        # Set y
-        ax.set_xlabel('PC' + str(PC[0] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[0]] * 100)[0:4] + '% expl.var)')
-        if len(self.results['model'].explained_variance_ratio_)>=2:
-            ax.set_ylabel('PC' + str(PC[1] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[1]] * 100)[0:4] + '% expl.var)')
-        else:
-            ax.set_ylabel('PC2 (0% expl.var)')
-        if d3 and (len(self.results['model'].explained_variance_ratio_)>=3):
-            ax.set_zlabel('PC' + str(PC[2] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[2]] * 100)[0:4] + '% expl.var)')
+        xs, ys, zs = _get_coordinates(self.results['PC'], PC)
+        # Setup figure
+        # fig, ax = _setup_figure(fig, ax, d3, visible, figsize, dpi)
 
-        if title is None:
-            title = str(self.n_components) + ' Principal Components explain [' + str(self.results['pcp'] * 100)[0:5] + '%] of the variance'
-        ax.set_title(title)
-        if legend: ax.legend()
-        ax.grid(True)
+        fig, ax = scatterd(x=xs,
+                           y=ys,
+                           z=zs,
+                           s=s,
+                           c=c,
+                           labels=labels,
+                           edgecolor=edgecolor,
+                           alpha=alpha,
+                           marker=marker,
+                           jitter=jitter,
+                           density=density,
+                           density_on_top=density_on_top,
+                           gradient=gradient,
+                           cmap=cmap,
+                           legend=legend,
+                           fontcolor=fontcolor,
+                           fontsize=fontsize,
+                           fontweight=fontweight,
+                           dpi=dpi,
+                           figsize=figsize,
+                           visible=visible,
+                           fig=fig,
+                           ax=ax)
+
+        # Plot the SPE with Elipse
+        fig, ax = _add_plot_SPE(self, xs, ys, zs, SPE, d3, alpha, s, fig, ax)
+        # Plot hotelling T2
+        fig, ax = _add_plot_HT2(self, xs, ys, zs, HT2, d3, alpha, s, fig, ax)
+        # Add figure properties
+        fig, ax = _add_plot_properties(self, PC, d3, title, legend, labels, fig, ax, fontsize, verbose)
         # Return
         return (fig, ax)
 
     def biplot(self,
-               y=None,
-               c=None,
-               s=50,
-               marker='.',
+               labels=None,
+               c=[0,0.1,0.4],
+               s=150,
+               marker='o',
+               edgecolor='#000000',
                jitter=None,
                n_feat=None,
-               d3=False,
-               label=True,
-               PC=[0, 1],
-               SPE=False,
-               hotellingt2=False,
-               alpha_transparency=1,
+               PC=None,
+               SPE=None,
+               HT2=None,
+               alpha=0.8,
                gradient=None,
-               color_arrow='r',
-               fontdict={'weight': 'normal', 'size': 12, 'ha': 'center', 'va': 'center', 'c': 'color_arrow'},
-               cmap='Set1',
+               density=False,
+               density_on_top=False,
+               fontcolor=[0,0,0],
+               fontsize=18,
+               fontweight='normal',
+               color_arrow='#000000',
+               arrowdict={'fontsize': None, 'c': None, 'weight': None, 'ha': 'center', 'va': 'center'},
+               cmap='tab20c',
                title=None,
-               legend=True,
-               figsize=(15, 10),
+               legend=None,
+               figsize=(25, 15),
                visible=True,
                fig=None,
                ax=None,
+               dpi=100,
+               y=None,  # deprecated
+               label=None,  # deprecated
                verbose=None):
         """Create the Biplot.
 
-        Description
-        -----------
         Plots the Principal components with the samples, and the best performing features.
         Per PC, The feature with absolute highest loading is gathered. This can result into features that are seen over multiple PCs, and some features may never be detected.
         For vizualization purposes we will keep only the unique feature-names and plot them with red arrows and green labels.
         The feature-names that were never discovered (described as weak) are colored yellow.
 
         Parameters
         ----------
-        y : array-like, default: None
+        labels : array-like, default: None
             Label for each sample. The labeling is used for coloring the samples.
         c: list/array of RGB colors for each sample.
-            Color of samples in RGB colors.
-            [0,0,0]: If a single color is given, all samples get that color.
-        s: Int or list/array (default: 50)
+            The marker colors. Possible values:
+                * A scalar or sequence of n numbers to be mapped to colors using cmap and norm.
+                * A 2D array in which the rows are RGB or RGBA.
+                * A sequence of colors of length n.
+                * A single color format string.
+        s : Int or list/array (default: 50)
             Size(s) of the scatter-points.
             [20, 10, 50, ...]: In case of list: should be same size as the number of PCs -> .results['PC']
             50: all points get this size.
-        marker: list/array of strings (default: '.').
+        marker: list/array of strings (default: 'o').
             Marker for the samples.
-            '.' : All data points get this marker
-            ['.', '*', 's', ..]: Specify per sample the marker type.
-        jitter : float, default: None
-            Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
+                * 'x' : All data points get this marker
+                * ('.', 'o', 'v', '^', '<', '>', '8', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X') : Specify per sample the marker type.
         n_feat : int, default: 10
             Number of features that explain the space the most, dervied from the loadings. This parameter is used for vizualization purposes only.
-        d3 : Bool, default: False
-            3d plot is created when True.
-        label : Bool, default: True
-            True Show the labels.
-            False: Do not show the labels
-            None: Ignore all labels (this will significanly speed up the scatterplot)
-        PC : list, default : [0, 1]
+        jitter : float, default: None
+            Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
+        PC : tupel, default: None
             Plot the selected Principal Components. Note that counting starts from 0. PC1=0, PC2=1, PC3=2, etc.
+            None : Take automatically the first 2 components and 3 in case d3=True.
+            [0, 1] : Define the PC for 2D.
+            [0, 1, 2] : Define the PCs for 3D
         SPE : Bool, default: False
             Show the outliers based on SPE/DmodX method.
-        hotellingt2 : Bool, default: False
+                * None : Auto detect. If outliers are detected. it is set to True.
+                * True : Show outliers
+                * False : Do not show outliers
+        HT2 : Bool, default: False
             Show the outliers based on the hotelling T2 test.
-        alpha_transparency: float or array-like of floats (default: 1).
+                * None : Auto detect. If outliers are detected. it is set to True.
+                * True : Show outliers
+                * False : Do not show outliers
+        alpha: float or array-like of floats (default: 1).
             The alpha blending value ranges between 0 (transparent) and 1 (opaque).
             1: All data points get this alpha
             [1, 0.8, 0.2, ...]: Specify per sample the alpha
         gradient : String, (default: None)
             Hex (ending) color for the gradient of the scatterplot colors.
             '#FFFFFF'
-        color_arrow : String, (default: 'r')
+        density : Bool (default: False)
+            Include the kernel density in the scatter plot.
+        density_on_top : bool, (default: False)
+            True : The density is the highest layer.
+            False : The density is the lowest layer.
+        color_arrow : String, (default: '#000000')
             color for the arrow.
-            'r' (default)
-        fontdict : dict.
+            * '#000000'
+            * 'r'
+        arrowdict : dict.
             dictionary containing properties for the arrow font-text.
-            Note that the [c]olor: 'color_arrow' inherits the color used in color_arrow.
-            {'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': 'color_arrow'}
+            Note that the [c]olor: None inherits the color used in color_arrow.
+            {'fontsize': None, 'c': None, 'weight': None, 'ha': 'center', 'va': 'center'}
+        fontsize : String, optional
+            The fontsize of the y labels that are plotted in the graph. The default is 16.
+        fontcolor: list/array of RGB colors with same size as X (default : None)
+            None : Use same colorscheme as for c
+            '#000000' : If the input is a single color, all fonts will get this color.
         cmap : String, optional, default: 'Set1'
             Colormap. If set to None, no points are shown.
         title : str, default: None
             Title of the figure.
             None: Automatically create title text based on results.
             '' : Remove all title text.
             'title text' : Add custom title text.
-        legend : Bool, default: True
-            Show the legend based on the unique y-labels.
-        figsize : (int, int), optional, default: (15, 10)
+        legend : int, default: None
+            None: Set automatically based on number of labels.
+            False : No legend.
+            True : Best position.
+            1 : 'upper right'
+            2 : 'upper left'
+            3 : 'lower left'
+            4 : 'lower right'
+        figsize : (int, int), optional, default: (25, 15)
             (width, height) in inches.
         visible : Bool, default: True
             Visible status of the Figure. When False, figure is created on the background.
         fig : Figure, optional (default: None)
             Matplotlib figure.
         ax : Axes, optional (default: None)
             Matplotlib Axes object
@@ -946,200 +813,52 @@
         References
         ----------
             * https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559
             * https://stackoverflow.com/questions/50796024/feature-variable-importance-after-a-pca-analysis/50845697#50845697
 
         """
         if verbose is None: verbose = self.verbose
-        # Input checks
-        fontdict, cmap = _biplot_input_checks(self.results, PC, cmap, fontdict, d3, color_arrow, verbose)
+        _show_deprecated_warning(label, y, verbose)
+        if not hasattr(self, 'results'):
+            if verbose>=2: print('[pca]> [WARNING]: No results to plot. Hint: model.fit(X) <return>')
+            return None, None
 
+        # Input checks
+        arrowdict, cmap, PC, d3, s = _biplot_input_checks(self.results, PC, cmap, arrowdict, color_arrow, fontsize, fontweight, c, s, verbose)
         # Pre-processing
-        y, topfeat, n_feat = self._fig_preprocessing(y, n_feat, d3)
-        topfeat = pd.concat([topfeat.iloc[PC, :], topfeat.loc[~topfeat.index.isin(PC), :]])
-        topfeat.reset_index(inplace=True)
-
-        # Collect coefficients
-        coeff = self.results['loadings'].iloc[PC, :]
-
-        # Use the PCs only for scaling purposes
-        mean_x = np.mean(self.results['PC'].iloc[:, PC[0]].values)
-        mean_y = np.mean(self.results['PC'].iloc[:, PC[1]].values)
-
-        # Plot and scale values for arrows and text by taking the absolute minimum range of the x-axis and y-axis.
-        # max_axis = np.min(np.abs(self.results['PC'].iloc[:,0:2]).max())
-        max_axis = np.max(np.abs(self.results['PC'].iloc[:, PC]).min(axis=1))
-        max_arrow = np.abs(coeff).max().max()
-        scale = (np.max([1, np.round(max_axis / max_arrow, 2)])) * 0.93
-
-        # Include additional parameters if 3d-plot is desired.
-        if d3:
-            if self.results['PC'].shape[1]<3:
-                if verbose>=2: print('[pca] >Warning: requires 3 PCs to make 3d plot <return>.')
-                return None, None
-            mean_z = np.mean(self.results['PC'].iloc[:, PC[2]].values)
-            # zs = self.results['PC'].iloc[:,2].values
-            fig, ax = self.scatter3d(y=y, label=label, legend=legend, PC=PC, SPE=SPE, hotellingt2=hotellingt2, cmap=cmap, visible=visible, figsize=figsize, alpha_transparency=alpha_transparency, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, verbose=verbose)
-        else:
-            fig, ax = self.scatter(y=y, label=label, legend=legend, PC=PC, SPE=SPE, hotellingt2=hotellingt2, cmap=cmap, visible=visible, figsize=figsize, alpha_transparency=alpha_transparency, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, verbose=verbose)
-
-        # For vizualization purposes we will keep only the unique feature-names
-        topfeat = topfeat.drop_duplicates(subset=['feature'])
-        if topfeat.shape[0]<n_feat:
-            n_feat = topfeat.shape[0]
-            if verbose>=2: print('[pca] >Warning: n_feat can not be reached because of the limitation of n_components (=%d). n_feat is reduced to %d.' %(self.n_components, n_feat))
-
-        # Plot arrows and text
-        texts = []
-        for i in range(0, n_feat):
-            getfeat = topfeat['feature'].iloc[i]
-            label = getfeat + ' (' + ('%.3g' %topfeat['loading'].iloc[i]) + ')'
-            getcoef = coeff[getfeat].values
-            # Set first PC vs second PC direction. Note that these are not neccarily the best loading.
-            xarrow = getcoef[0] * scale  # First PC in the x-axis direction
-            yarrow = getcoef[1] * scale  # Second PC in the y-axis direction
-            txtcolor = 'y' if topfeat['type'].iloc[i] == 'weak' else 'g'
-
-            if d3:
-                zarrow = getcoef[2] * scale
-                ax.quiver(mean_x, mean_y, mean_z, xarrow - mean_x, yarrow - mean_y, zarrow - mean_z, color=color_arrow, alpha=0.8, lw=2)
-                texts.append(ax.text(xarrow, yarrow, zarrow, label, color=txtcolor, ha='center', va='center'))
-            else:
-                ax.arrow(mean_x, mean_y, xarrow - mean_x, yarrow - mean_y, color=color_arrow, alpha=0.8, width=0.002, head_width=0.1, head_length=0.1 * 1.1, length_includes_head=True)
-                texts.append(ax.text(xarrow, yarrow, label, color=txtcolor, fontdict=fontdict))
-
-        # Plot the adjusted text labels to prevent overlap
-        if len(texts)>0: adjust_text(texts)
-        # if visible: plt.show()
-        return (fig, ax)
+        labels, topfeat, n_feat = self._fig_preprocessing(labels, n_feat, d3)
+        # Scatterplot
+        fig, ax = self.scatter(labels=labels, legend=legend, PC=PC, SPE=SPE, HT2=HT2, cmap=cmap, visible=visible, figsize=figsize, alpha=alpha, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, fontcolor=fontcolor, fontweight=fontweight, fontsize=fontsize, edgecolor=edgecolor, density=density, density_on_top=density_on_top, dpi=dpi, verbose=verbose)
+        # Add the loadings with arrow to the plot
+        fig, ax = _plot_loadings(self, topfeat, n_feat, PC, d3, color_arrow, arrowdict, fig, ax, verbose)
+        # Plot
+        if visible: plt.show()
+        # Return
+        return fig, ax
 
-    def biplot3d(self,
-                 y=None,
-                 c=None,
-                 s=50,
-                 marker='.',
-                 jitter=None,
-                 n_feat=None,
-                 label=True,
-                 PC=[0, 1, 2],
-                 SPE=False,
-                 hotellingt2=False,
-                 alpha_transparency=1,
-                 gradient=None,
-                 color_arrow='r',
-                 fontdict={'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': 'color_arrow'},
-                 cmap='Set1',
-                 title=None,
-                 legend=True,
-                 figsize=(15, 10),
-                 visible=True,
-                 fig=None,
-                 ax=None,
-                 verbose=None):
-        """Make biplot in 3d.
+    def scatter3d(self, PC=[0, 1, 2], **args):
+        """Scatter 3d plot.
 
         Parameters
         ----------
-        y : array-like, default: None
-            Label for each sample. The labeling is used for coloring the samples.
-        c: list/array of RGB colors for each sample.
-            Color of samples in RGB colors.
-            [0,0,0]: If a single color is given, all samples get that color.
-        s: Int or list/array (default: 50)
-            Size(s) of the scatter-points.
-            [20, 10, 50, ...]: In case of list: should be same size as the number of PCs -> .results['PC']
-            50: all points get this size.
-        marker: list/array of strings (default: '.').
-            Marker for the samples.
-            '.' : All data points get this marker
-            ['.', '*', 's', ..]: Specify per sample the marker type.
-        jitter : float, default: None
-            Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
-        n_feat : int, default: 10
-            Number of features that explain the space the most, dervied from the loadings. This parameter is used for vizualization purposes only.
-        label : Bool, default: True
-            True Show the labels.
-            False: Do not show the labels
-            None: Ignore all labels (this will significanly speed up the scatterplot)
-        PC : list, default : [0, 1, 2]
-            Plot the selected Principal Components. Note that counting starts from 0. PC1=0, PC2=1, PC3=2, etc.
-        SPE : Bool, default: False
-            Show the outliers based on SPE/DmodX method.
-        hotellingt2 : Bool, default: False
-            Show the outliers based on the hotelling T2 test.
-        alpha_transparency: float or array-like of floats (default: 1).
-            The alpha blending value ranges between 0 (transparent) and 1 (opaque).
-            1: All data points get this alpha
-            [1, 0.8, 0.2, ...]: Specify per sample the alpha
-        gradient : String, (default: None)
-            Hex (ending) color for the gradient of the scatterplot colors.
-            '#FFFFFF'
-        color_arrow : String, (default: 'r')
-            color for the arrow.
-            'r' (default)
-        fontdict : dict.
-            dictionary containing properties for the arrow font-text
-            Note that the [c]olor: 'color_arrow' inherits the color used in color_arrow.
-            {'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': 'color_arrow'}
-        cmap : String, optional, default: 'Set1'
-            Colormap. If set to None, no points are shown.
-        title : str, default: None
-            Title of the figure.
-            None: Automatically create title text based on results.
-            '' : Remove all title text.
-            'title text' : Add custom title text.
-        legend : Bool, default: True
-            Show the legend based on the unique y-labels.
-        figsize : (int, int), optional, default: (15, 10)
-            (width, height) in inches.
-        visible : Bool, default: True
-            Visible status of the Figure. When False, figure is created on the background.
-        fig : Figure, optional (default: None)
-            Matplotlib figure.
-        ax : Axes, optional (default: None)
-            Matplotlib Axes object
-        Verbose : int (default : 3)
-            The higher the number, the more information is printed.
-            Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace
-
-        Returns
-        -------
-        tuple containing (fig, ax)
-
+        Input parameters are described under <scatter>.
         """
-        if verbose is None: verbose = self.verbose
-        if self.results['PC'].shape[1]<3:
-            print('[pca] >Requires 3 PCs to make 3d plot. Try to use biplot() instead.')
-            return None, None
+        fig, ax = self.scatter(PC=PC, **args)
+        return fig, ax
 
-        fig, ax = self.biplot(y=y,
-                              n_feat=n_feat,
-                              c=c,
-                              s=s,
-                              marker=marker,
-                              jitter=jitter,
-                              d3=True,
-                              label=label,
-                              PC=PC,
-                              SPE=SPE,
-                              hotellingt2=hotellingt2,
-                              alpha_transparency=alpha_transparency,
-                              gradient=gradient,
-                              color_arrow=color_arrow,
-                              fontdict=fontdict,
-                              cmap=cmap,
-                              title=title,
-                              legend=legend,
-                              figsize=figsize,
-                              visible=visible,
-                              fig=fig,
-                              ax=ax,
-                              verbose=verbose)
+    def biplot3d(self, PC=[0, 1, 2], alpha=0.8, **args):
+        """Biplot 3d plot.
 
-        return (fig, ax)
+        Parameters
+        ----------
+        Input parameters are described under <scatter>.
+        """
+        if not isinstance(alpha, (int, float)): alpha=0.8
+        fig, ax = self.biplot(PC=PC, alpha=alpha, **args)
+        return fig, ax
 
     # Show explained variance plot
     def plot(self, n_components=None, xsteps=None, title=None, visible=True, figsize=(15, 10), fig=None, ax=None, verbose=None):
         """Scree-plot together with explained variance.
 
         Parameters
         ----------
@@ -1153,15 +872,15 @@
             None: Automatically create title text based on results.
             '' : Remove all title text.
             'title text' : Add custom title text.
         visible : Bool, default: True
             Visible status of the Figure
             True : Figure is shown.
             False: Figure is created on the background.
-        figsize : (int, int)
+        figsize : (int, int): (default: 25, 15)
             (width, height) in inches.
         fig : Figure, optional (default: None)
             Matplotlib figure.
         ax : Axes, optional (default: None)
             Matplotlib Axes object
         Verbose : int (default : 3)
             The higher the number, the more information is printed.
@@ -1175,15 +894,15 @@
         if verbose is None: verbose = self.verbose
 
         if self.method=='sparse_pca':
             print('[pca] >sparse pca does not support variance ratio and therefores scree plots are not supported. <return>')
             return None, None
         if n_components is not None:
             if n_components>len(self.results['explained_var']):
-                if verbose>=2: print('[pca] >Warning: Input "n_components=%s" is > then number of PCs (=%s)' %(n_components, len(self.results['explained_var'])))
+                if verbose>=2: print('[pca] >[WARNING]: Input "n_components=%s" is > then number of PCs (=%s)' %(n_components, len(self.results['explained_var'])))
             n_components = np.minimum(len(self.results['explained_var']), n_components)
             explvarCum = self.results['explained_var'][0:n_components]
             explvar = self.results['variance_ratio'][0:n_components]
         else:
             explvarCum = self.results['explained_var']
             explvar = self.results['variance_ratio']
         xtick_idx = np.arange(1, len(explvar) + 1)
@@ -1229,16 +948,14 @@
         # Return
         return (fig, ax)
 
     # Top scoring components
     def norm(self, X, n_components=None, pcexclude=[1]):
         """Normalize out PCs.
 
-        Description
-        -----------
         Normalize your data using the variance seen in hte Principal Components. This allows to remove (technical)
         variation in the data by normalizing out e.g., the 1st or 2nd etc component. This function transforms the
         original data using the PCs that you want to normalize out. As an example, if you aim to remove the variation
         seen in the 1st PC, the returned dataset will contain only the variance seen from the 2nd PC and more.
 
         Parameters
         ----------
@@ -1277,68 +994,71 @@
         ndims = (np.setdiff1d(ndims + 1, pcexclude)) - 1
         # Transform data
         out = np.repeat(np.mean(X, axis=1).reshape(-1, 1), X.shape[1], axis=1) + np.dot(score.values[:, ndims], coeff[:, ndims].T)
         # Return
         return out
 
     # Import example
-    def import_example(self, data='titanic', url=None, sep=','):
+    def import_example(self, data='iris', url=None, sep=','):
         """Import example dataset from github source.
 
-        Description
-        -----------
         Import one of the few datasets from github source or specify your own download url link.
 
         Parameters
         ----------
         data : str
-            Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
+            Name of datasets
+                * 'iris'
+                * 'sprinkler'
+                * 'titanic'
+                * 'student'
+                * 'fifa'
+                * 'cancer'
+                * 'waterpump'
+                * 'retail'
         url : str
             url link to to dataset.
 
         Returns
         -------
         pd.DataFrame()
             Dataset containing mixed features.
 
         """
         return import_example(data=data, url=url, sep=sep)
 
 
 # %%
-def _get_coordinates(PCs, PC, fig, ax, d3):
+def _get_coordinates(PCs, PC):
     xs = PCs.iloc[:, PC[0]].values
     ys = np.zeros(len(xs))
     zs = None
 
     # Get y-axis
     if PCs.shape[1]>1:
         ys = PCs.iloc[:, PC[1]].values
 
     # Get Z-axis
-    if d3:
+    if len(PC)>=3:
         zs = PCs.iloc[:, PC[2]].values
-        ax = Axes3D(fig, rect=[0, 0, .95, 1], elev=48, azim=134)
 
-    return xs, ys, zs, ax
+    return xs, ys, zs
 
 
 # %%
 def _eigsorted(cov, n_std):
     vals, vecs = np.linalg.eigh(cov)
     # vecs = vecs * np.sqrt(scipy.stats.chi2.ppf(0.95, n_std))
     order = vals.argsort()[::-1]
     return vals[order], vecs[:, order]
 
 
-def spe_dmodx(X, n_std=3, param=None, calpha=0.3, color='green', showfig=False, verbose=3):
+def spe_dmodx(X, n_std=3, param=None, calpha=0.3, color='green', visible=False, verbose=3):
     """Compute SPE/distance to model (DmodX).
 
-    Description
-    -----------
     Outlier can be detected using SPE/DmodX (distance to model) based on the mean and covariance of the first 2 dimensions of X.
     On the model plane (SPE ≈ 0). Note that the SPE or Hotelling’s T2 are complementary to each other.
 
     Parameters
     ----------
     X : Array-like
         Input data, in this case the Principal components.
@@ -1346,15 +1066,15 @@
         Standard deviation. The default is 2.
     param : 2-element tuple (default: None)
         Pre-computed g_ell_center and cov in the past run. None to compute from scratch with X.
     calpha : float, (default: 0.3)
         transperancy color.
     color : String, (default: 'green')
         Color of the ellipse.
-    showfig : bool, (default: False)
+    visible : bool, (default: False)
         Scatter the points with the ellipse and mark the outliers.
 
     Returns
     -------
     outliers : pd.DataFrame()
         column with boolean outliers and euclidean distance of each sample to the center of the ellipse.
     ax : object
@@ -1394,35 +1114,33 @@
         # Mark the samples outside the ellipse
         outliers = rad_cc>1
 
         # Plot the raw points.
         g_ellipse = Ellipse(xy=g_ell_center, width=width, height=height, angle=angle, color=color, alpha=calpha)
         y_score = list(map(lambda x: euclidean_distances([g_ell_center], x.reshape(1, -1))[0][0], X))
 
-        if showfig:
+        if visible:
             ax = plt.gca()
             ax.add_artist(g_ellipse)
             ax.scatter(X[~outliers, 0], X[~outliers, 1], c='black', linewidths=0.3, label='normal')
             ax.scatter(X[outliers, 0], X[outliers, 1], c='red', linewidths=0.3, label='outlier')
-            ax.legend()
+            ax.legend(loc=0)
     else:
         outliers = np.repeat(False, X.shape[1])
         y_score = np.repeat(None, X.shape[1])
 
     # Store in dataframe
     out = pd.DataFrame(data={'y_bool_spe': outliers, 'y_score_spe': y_score})
     return out, g_ellipse, param
 
 
 # %% Outlier detection
 def hotellingsT2(X, alpha=0.05, df=1, n_components=5, multipletests='fdr_bh', param=None, verbose=3):
     """Test for outlier using hotelling T2 test.
 
-    Description
-    -----------
     Test for outliers using chi-square tests for each of the n_components.
     The resulting P-value matrix is then combined using fishers method per sample.
     The results can be used to priortize outliers as those samples that are an outlier
     across multiple dimensions will be more significant then others.
 
     Parameters
     ----------
@@ -1591,25 +1309,31 @@
     out['topfeat'] = topfeat
     out['outliers'] = outliers
     out['outliers_params'] = outliers_params
     return out
 
 
 # %% Import example dataset from github.
-def import_example(data='titanic', url=None, sep=',', verbose=3):
+def import_example(data='iris', url=None, sep=',', verbose=3):
     """Import example dataset from github source.
 
-    Description
-    -----------
     Import one of the few datasets from github source or specify your own download url link.
 
     Parameters
     ----------
     data : str
-        Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
+        Name of datasets
+            * 'iris'
+            * 'sprinkler'
+            * 'titanic'
+            * 'student'
+            * 'fifa'
+            * 'cancer'
+            * 'waterpump'
+            * 'retail'
     url : str
         url link to to dataset.
 	verbose : int, (default: 20)
 		Print progress to screen. The default is 3.
 		60: None, 40: Error, 30: Warn, 20: Info, 10: Debug
 
     Returns
@@ -1629,16 +1353,22 @@
             url='https://erdogant.github.io/datasets/cancer_dataset.zip'
         elif data=='fifa':
             url='https://erdogant.github.io/datasets/FIFA_2018.zip'
         elif data=='waterpump':
             url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
         elif data=='retail':
             url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
-    else:
-        data = wget.filename_from_url(url)
+        elif data=='iris':
+            from sklearn.datasets import load_iris
+            label = load_iris().feature_names
+            y = load_iris().target
+            X = pd.DataFrame(data=load_iris().data, columns=label, index=y)
+            return X
+        else:
+            data = wget.filename_from_url(url)
 
     if url is None:
         if verbose>=3: print('Nothing to download.')
         return None
 
     curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     filename = os.path.basename(urlparse(url).path)
@@ -1658,16 +1388,14 @@
     return df
 
 
 # %%
 def _get_explained_variance(X, components):
     """Get the explained variance.
 
-    Description
-    -----------
     Get the explained variance from the principal components of the
     data. This follows the method outlined in [1] section 3.4 (Adjusted Total
     Variance). For an alternate approach (not implemented here), see [2].
 
     Parameters
     ----------
     X : ndarray, shape (n_samples, n_features)
@@ -1713,37 +1441,45 @@
     Y = np.tensordot(X, proj_corrected_vecs.T, axes=(1, 0))
     YYT = np.tensordot(Y.T, Y, axes=(1, 0))
     explained_variance = np.diag(YYT) / (n_samples - 1)
 
     return explained_variance
 
 
-def _biplot_input_checks(results, PC, cmap, fontdict, d3, color_arrow, verbose):
+def _biplot_input_checks(results, PC, cmap, arrowdict, color_arrow, fontsize, fontweight, c, s, verbose):
+    if c is None: s=0
+    if cmap is None: s=0
+    if isinstance(s, (int, float)) and s==0: fontsize=0
+    if PC is None: PC=[0, 1]
+    d3 = True if len(PC)>=3 else False
+
     # Check PCs
     if results['PC'].shape[1]<2: raise ValueError('[pca] >[Error] Requires 2 PCs to make 2d plot.')
-    if d3 and len(PC)<3: raise ValueError('[pca] >[Error] in case of biplot3d or d3=True, at least 3 PCs are required.')
     if np.max(PC)>=results['PC'].shape[1]: raise ValueError('[pca] >[Error] PC%.0d does not exist!' %(np.max(PC) + 1))
     if verbose>=3 and d3:
         print('[pca] >Plot PC%.0d vs PC%.0d vs PC%.0d with loadings.' %(PC[0] + 1, PC[1] + 1, PC[2] + 1))
     elif verbose>=3:
         print('[pca] >Plot PC%.0d vs PC%.0d with loadings.' %(PC[0] + 1, PC[1] + 1))
-    if cmap is False: cmap=None
-    # Set defaults in fontdict
-    fontdict =_set_fontdict(fontdict, color_arrow)
-    # Set font dictionary
+
+    # Set defaults in arrowdict
+    arrowdict =_set_arrowdict(arrowdict, color_arrow=color_arrow, fontsize=fontsize, fontweight=fontweight)
     # Return
-    return fontdict, cmap
+    return arrowdict, cmap, PC, d3, s
 
 
-def _set_fontdict(fontdict, color_arrow=None):
+def _set_arrowdict(arrowdict, color_arrow=None, fontsize=18, fontweight='normal'):
     color_arrow = 'black' if (color_arrow is None) else color_arrow
-    fontdict = {**{'weight': 'normal', 'size': 10, 'ha': 'center', 'va': 'center', 'c': color_arrow}, **fontdict}
-    if fontdict.get('c')=='color_arrow' and (color_arrow is not None):
-        fontdict['c'] = color_arrow
-    return fontdict
+    arrowdict = {**{'fontsize': 18 if fontsize==0 else fontsize, 'c': color_arrow, 'weight': fontweight, 'ha': 'center', 'va': 'center'}, **arrowdict}
+    if arrowdict.get('c') is None and (color_arrow is not None):
+        arrowdict['c'] = color_arrow
+    if arrowdict.get('fontsize') is None:
+        arrowdict['fontsize'] = 18 if fontsize==0 else fontsize
+    if arrowdict.get('weight') is None:
+        arrowdict['weight'] = fontweight
+    return arrowdict
 
 
 # %% Retrieve files files.
 class wget:
     """Retrieve file from url."""
 
     def filename_from_url(url):
@@ -1764,8 +1500,153 @@
         -------
         None.
 
         """
         r = requests.get(url, stream=True)
         with open(writepath, "wb") as fd:
             for chunk in r.iter_content(chunk_size=1024):
-                fd.write(chunk)
+                fd.write(chunk)
+
+
+def _setup_figure(fig, ax, d3, visible, figsize, dpi):
+    if fig is None and ax is None:
+        # Create new figure.
+        fig = plt.figure(figsize=figsize, dpi=dpi)
+
+        # Add d3 projection
+        if d3:
+            ax = fig.add_subplot(projection='3d')
+            # ax = Axes3D(fig, rect=[0, 0, .95, 1], elev=48, azim=134)
+        else:
+            ax = fig.add_subplot()
+    elif fig is not None and ax is None:
+        # Extract axes from fig.
+        ax = fig.axes[0]
+
+    if fig is not None:
+        fig.set_visible(visible)
+
+    return fig, ax
+
+
+def _plot_loadings(self, topfeat, n_feat, PC, d3, color_arrow, arrowdict, fig, ax, verbose):
+    topfeat = pd.concat([topfeat.iloc[PC, :], topfeat.loc[~topfeat.index.isin(PC), :]])
+    topfeat.reset_index(inplace=True)
+    # Collect coefficients
+    coeff = self.results['loadings'].iloc[PC, :]
+
+    # Use the PCs only for scaling purposes
+    mean_x = np.mean(self.results['PC'].iloc[:, PC[0]].values)
+    mean_y = np.mean(self.results['PC'].iloc[:, PC[1]].values)
+    if d3: mean_z = np.mean(self.results['PC'].iloc[:, PC[2]].values)
+
+    # Plot and scale values for arrows and text by taking the absolute minimum range of the x-axis and y-axis.
+    max_axis = np.max(np.abs(self.results['PC'].iloc[:, PC]).min(axis=1))
+    max_arrow = np.abs(coeff).max().max()
+    scale = (np.max([1, np.round(max_axis / max_arrow, 2)])) * 0.93
+
+    # For vizualization purposes we will keep only the unique feature-names
+    topfeat = topfeat.drop_duplicates(subset=['feature'])
+    if topfeat.shape[0]<n_feat:
+        n_feat = topfeat.shape[0]
+        if verbose>=2: print('[pca] >[WARNING]: n_feat can not be reached because of the limitation of n_components (=%d). n_feat is reduced to %d.' %(self.n_components, n_feat))
+
+    # Plot arrows and text
+    texts = []
+    for i in range(0, n_feat):
+        getfeat = topfeat['feature'].iloc[i]
+        label = getfeat + ' (' + ('%.3g' %topfeat['loading'].iloc[i]) + ')'
+        getcoef = coeff[getfeat].values
+        # Set first PC vs second PC direction. Note that these are not neccarily the best loading.
+        xarrow = getcoef[0] * scale  # First PC in the x-axis direction
+        yarrow = getcoef[1] * scale  # Second PC in the y-axis direction
+        txtcolor = 'y' if topfeat['type'].iloc[i] == 'weak' else 'g'
+
+        if d3:
+            zarrow = getcoef[2] * scale
+            ax.quiver(mean_x, mean_y, mean_z, xarrow - mean_x, yarrow - mean_y, zarrow - mean_z, color=color_arrow, alpha=0.8, lw=2)
+            texts.append(ax.text(xarrow, yarrow, zarrow, label, color=arrowdict['c'], ha='center', va='center', fontsize=arrowdict['fontsize'], zorder=25))
+        else:
+            ax.arrow(mean_x, mean_y, xarrow - mean_x, yarrow - mean_y, color=color_arrow, alpha=0.8, width=0.002, head_width=0.1, head_length=0.1 * 1.1, length_includes_head=True, zorder=10)
+            texts.append(ax.text(xarrow, yarrow, label, fontdict=arrowdict, zorder=10))
+
+    # Plot the adjusted text labels to prevent overlap
+    if len(texts)>0 and not d3: adjust_text(texts)
+
+    # Return
+    return fig, ax
+
+
+def _add_plot_SPE(self, xs, ys, zs, SPE, d3, alpha, s, fig, ax):
+    # Get the outliers
+    Ioutlier2 = np.repeat(False, self.results['PC'].shape[0])
+    if SPE and ('y_bool_spe' in self.results['outliers'].columns):
+        Ioutlier2 = self.results['outliers']['y_bool_spe'].values
+        if not d3:
+            # Plot the ellipse
+            g_ellipse = spe_dmodx(np.c_[xs, ys], n_std=self.n_std, color='green', calpha=0.1, visible=False, verbose=0)[1]
+            if g_ellipse is not None:
+                ax.add_artist(g_ellipse)
+                # Set the order of the layer at 1. At this point it is over the density layer which looks nicer.
+                g_ellipse.set_zorder(1)
+
+    # Plot outliers for hotelling T2 test.
+    if isinstance(s, (int, float)): s = 150 if s>0 else 0
+    if not isinstance(s, (int, float)): s=150
+    if SPE and ('y_bool_spe' in self.results['outliers'].columns):
+        label_spe = str(sum(Ioutlier2)) + ' outlier(s) (SPE/DmodX)'
+        if d3:
+            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], zs[Ioutlier2], marker='x', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha)
+        else:
+            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], marker='d', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha)
+
+    return fig, ax
+
+
+def _add_plot_HT2(self, xs, ys, zs, HT2, d3, alpha, s, fig, ax):
+    # Plot outliers for hotelling T2 test.
+    if isinstance(s, (int, float)): s = 150 if s>0 else 0
+    if not isinstance(s, (int, float)): s=150
+    # Plot outliers for hotelling T2 test.
+    if HT2 and ('y_bool' in self.results['outliers'].columns):
+        Ioutlier1 = self.results['outliers']['y_bool'].values
+
+    if HT2 and ('y_bool' in self.results['outliers'].columns):
+        label_t2 = str(sum(Ioutlier1)) + ' outlier(s) (hotelling t2)'
+        if d3:
+            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], zs[Ioutlier1], marker='d', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha)
+        else:
+            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], marker='x', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha)
+
+    return fig, ax
+
+
+def _add_plot_properties(self, PC, d3, title, legend, labels, fig, ax, fontsize, verbose):
+    # Set labels
+    ax.set_xlabel('PC' + str(PC[0] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[0]] * 100)[0:4] + '% expl.var)')
+    if len(self.results['model'].explained_variance_ratio_)>=2:
+        ax.set_ylabel('PC' + str(PC[1] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[1]] * 100)[0:4] + '% expl.var)')
+    else:
+        ax.set_ylabel('PC2 (0% expl.var)')
+    if d3 and (len(self.results['model'].explained_variance_ratio_)>=3):
+        ax.set_zlabel('PC' + str(PC[2] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[2]] * 100)[0:4] + '% expl.var)')
+
+    # Set title
+    if title is None:
+        title = str(self.n_components) + ' Principal Components explain [' + str(self.results['pcp'] * 100)[0:5] + '%] of the variance'
+
+    # Determine the legend status if set to None
+    if isinstance(legend, bool): legend = 0 if legend else -1
+    if legend is None: legend = -1 if len(np.unique(labels))>20 else 0
+    if legend>=0: ax.legend(loc=legend, fontsize=14)
+
+    ax.set_title(title, fontsize=18)
+    ax.grid(True)
+    # Return
+    return fig, ax
+
+
+def _show_deprecated_warning(label, y, verbose):
+    if label is not None:
+        if verbose>=2: print('[pca]> [WARNING]: De parameter <label> is deprecated and will not be supported in future version.')
+    if y is not None:
+        if verbose>=2: print('[pca]> [WARNING]: De parameter <y> is deprecated and will not be supported in future version. Use <labels> instead.')
```

### Comparing `pca-1.9.2/pca/tests/test_pca.py` & `pca-2.0.0/pca/tests/test_pca.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         color = colors.colors[random_integers, :]
         # Set Size
         size = np.random.randint(10, 250, size=X.shape[0])
         # Set alpha
         alpha = np.random.rand(1, X.shape[0])[0][random_integers]
         
         param_grid = {
-        	'marker': [None, marker, '.'],
+        	'marker': [marker, 'o'],
         	'color':[None, color, [0,0,0]],
-        	'size' : [None, size, 50],
-            'alpha' : [None, alpha, 1]
+        	'size' : [size, 50],
+            'alpha' : [alpha, 1]
         	}
         
         allNames = param_grid.keys()
         combinations = it.product(*(param_grid[Name] for Name in allNames))
         combinations=list(combinations)
 
         # Init
@@ -46,20 +46,19 @@
         # Fit
         model.fit_transform(X)
         # Make plot with blue arrows and text
         for combination in combinations:
             fig, ax = model.biplot(c=combination[1],
                                    s=combination[2],
                                    marker=combination[0],
-                                   alpha_transparency=combination[3],
-                                   label=False,
-                                   fontdict={'size':10, 'weight':'normal'},
+                                   alpha=combination[3],
+                                   arrowdict={'weight':'normal'},
                                    color_arrow='blue',
                                    title='Demonstration of specifying colors, markers, alpha, and size per sample.',
-                                   hotellingt2=True,
+                                   HT2=True,
                                    n_feat=5,
                                    legend=False, 
                                    visible=False)
 
     def test_medium_blog(self):
         from sklearn.datasets import load_wine
         import pandas as pd
@@ -70,24 +69,24 @@
         # Initialize pca to also detected outliers.
         model = pca(normalize=True, detect_outliers=['ht2', 'spe'], n_std=2, multipletests=None)
         # Fit and transform
         results = model.fit_transform(df)
         assert np.sum(results['outliers']['y_proba']<=0.05)==9
 
         # Plot Hotellings T2
-        model.biplot(SPE=False, hotellingt2=True, title='Outliers marked using Hotellings T2 method.')
+        model.biplot(SPE=False, HT2=True, title='Outliers marked using Hotellings T2 method.')
         # Make a plot in 3 dimensions
-        model.biplot3d(SPE=False, hotellingt2=True, title='Outliers marked using Hotellings T2 method.')
+        model.biplot3d(SPE=False, HT2=True, title='Outliers marked using Hotellings T2 method.')
 
         # Get the outliers using SPE/DmodX method.
         df.loc[results['outliers']['y_bool'], :]
         # Plot SPE/DmodX method
-        model.biplot(SPE=True, hotellingt2=False, title='Outliers marked using SPE/dmodX method.')
+        model.biplot(SPE=True, HT2=False, title='Outliers marked using SPE/dmodX method.', marker=data.target)
         # Make a plot in 3 dimensions
-        model.biplot(SPE=True, hotellingt2=True, title='Outliers marked using SPE/dmodX method and Hotelling T2.')
+        model.biplot(SPE=True, HT2=True, title='Outliers marked using SPE/dmodX method and Hotelling T2.', marker=data.target)
         # Get the outliers using SPE/DmodX method.
         df.loc[results['outliers']['y_bool_spe'], :]
         Ioverlap = np.logical_and(results['outliers']['y_bool'], results['outliers']['y_bool_spe'])
         df.loc[Ioverlap, :]
 
         # Initialize
         model = pca()
@@ -123,56 +122,56 @@
         ######## TEST WITHOUT OUTLIERS #########
         model = pca(alpha=0.05, detect_outliers=None)
         # Fit transform
         out = model.fit_transform(X)
         assert out['outliers'].empty
         
         ######## TEST FOR TRANSPARENCY WITH MATPLOTLIB VERSION #########
-        assert model.scatter(alpha_transparency=0.1)
-        assert model.scatter3d(alpha_transparency=0.1)
-        assert model.biplot(alpha_transparency=0.1)
-        assert model.biplot3d(alpha_transparency=0.1)
-        assert model.scatter(alpha_transparency=None)
-        assert model.scatter3d(alpha_transparency=None)
-        assert model.biplot(alpha_transparency=None)
-        assert model.biplot3d(alpha_transparency=None)
-        assert model.scatter(alpha_transparency=0.5)
-        assert model.scatter3d(alpha_transparency=0.5)
-        assert model.biplot(alpha_transparency=0.5)
-        assert model.biplot3d(alpha_transparency=0.5)
+        assert model.scatter(alpha=0.1)
+        assert model.scatter3d(alpha=0.1)
+        assert model.biplot(alpha=0.1)
+        assert model.biplot3d(alpha=0.1)
+        assert model.scatter(alpha=None)
+        assert model.scatter3d(alpha=None)
+        assert model.biplot(alpha=None)
+        assert model.biplot3d(alpha=None)
+        assert model.scatter(alpha=0.5)
+        assert model.scatter3d(alpha=0.5)
+        assert model.biplot(alpha=0.5)
+        assert model.biplot3d(alpha=0.5)
 
     def test_plot_combinations(self):
 
         X = load_iris().data
         labels=load_iris().feature_names
         y=load_iris().target
         
         X = pd.DataFrame(data=load_iris().data, columns=load_iris().feature_names, index=load_iris().target)
         
         param_grid = {
-        	'n_components':[None, 0.01, 1, 0.95, 2, 100000000000],
+        	# 'n_components':[None, 0.01, 1, 0.95, 2, 100000000000],
         	'row_labels':[None, [], y],
         	'detect_outliers' : [None, 'ht2','spe'],
-            'gradient' : [None, '#FFFFFF']
+            # 'gradient' : [None, '#FFFFFF']
         	}
         
         allNames = param_grid.keys()
         combinations = it.product(*(param_grid[Name] for Name in allNames))
         combinations=list(combinations)
-        
+
         for combination in combinations:
          	model = pca(n_components=combination[0])
-         	model = pca(n_components=0.95)
+         	model = pca(n_components=3)
          	model.fit_transform(X)
-         	assert model.plot()
-         	assert model.biplot(y=y, SPE=True, hotellingt2=True, gradient=combination[3])
-         	assert model.biplot3d(y=y, SPE=True, hotellingt2=True, gradient=combination[3])
-         	assert model.biplot(y=y, SPE=True, hotellingt2=False, gradient=combination[3])
-         	assert model.biplot(y=y, SPE=False, hotellingt2=True, gradient=combination[3])
-         	assert model.biplot(y=y, SPE=False, hotellingt2=False, gradient=combination[3])
+         	assert model.plot(visible=False)
+         	assert model.biplot(labels=y, SPE=True, HT2=True, visible=False)
+         	assert model.biplot3d(labels=y, SPE=True, HT2=True, visible=False)
+         	assert model.biplot(labels=y, SPE=True, HT2=False, visible=False)
+         	assert model.biplot(labels=y, SPE=False, HT2=True, visible=False)
+         	assert model.biplot(labels=y, SPE=False, HT2=False, visible=False)
          	assert model.results['PC'].shape[1]==model.n_components
 
 
     def test_correct_ordering_features_in_biplot(self):
 
         f1=np.random.randint(0,100,250)
         f2=np.random.randint(0,50,250)
```

### Comparing `pca-1.9.2/pca.egg-info/PKG-INFO` & `pca-2.0.0/pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 1.9.2
+Version: 2.0.0
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/1.9.2.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/logo.png" width="600" />
+  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
 
 
 
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/pypi/pyversions/pca)
 [![Pypi](https://img.shields.io/pypi/v/pca)](https://pypi.org/project/pca/)
@@ -102,15 +100,15 @@
           <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png?raw=true" width="400" />
         </a>
       </p>    
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#biplot">
-          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_biplot.png?raw=true" width="350" />
+          <img src="https://github.com/erdogant/pca/blob/master/docs/figs/custom_example_2.png?raw=true" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
 
 
@@ -129,15 +127,15 @@
         <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_plot.png" width="350" />
         </a>
       </p>
     </td>
     <td>
       <p align="left">
         <a href="https://erdogant.github.io/pca/pages/html/Plots.html#d-plots">
-        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter3d.png" width="350" />
+        <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_3d_density.png" width="350" />
         </a>
       </p>
     </td>
   </tr>
 </table>
 
 
@@ -235,9 +233,7 @@
 ---
 
 ## Support
 
 Your ❤️ is important to keep maintaining this package. You can [support](https://erdogant.github.io/pca/pages/html/Documentation.html) in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues and feature extensions at [github page](https://github.com/erdogant/pca).
 
 <a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: pca Version: 1.9.2 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.0 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/1.9.2.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE
-       [https://github.com/erdogant/pca/blob/master/docs/figs/logo.png]
+Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE
+   [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
 pca?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
@@ -48,19 +47,19 @@
 [documentation pages](https://erdogant.github.io/pca/) you can find detailed
 information about the working of the ``pca`` with many examples. --- ##
 Installation ```bash pip install pca ``` ##### Import pca package ```python
 from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
-fig_scatter.png?raw=true]              fig_biplot.png?raw=true]
+fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
-master/docs/figs/fig_plot.png]         master/docs/figs/fig_scatter3d.png]
+master/docs/figs/fig_plot.png]         master/docs/figs/iris_3d_density.png]
 # * [Example: Set alpha transparency](https://erdogant.github.io/pca/pages/
 html/Plots.html#alpha-transparency)
 [https://github.com/erdogant/pca/blob/master/docs/figs/fig_scatter.png]
 # * [Example: Normalizing out Principal Components](https://erdogant.github.io/
 pca/pages/html/Algorithm.html#normalizing-out-pcs) Normalizing out the 1st and
 more components from the data. This is usefull if the data is seperated in its
 first component(s) by unwanted or biased variance. Such as sex or experiment
```

### Comparing `pca-1.9.2/setup.py` & `pca-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['requests', 'statsmodels', 'matplotlib','numpy','scikit-learn','scipy','colourmap>=1.1.10','pandas','tqdm','scatterd>=1.2.5', 'adjustText'],
+     install_requires=['requests', 'statsmodels', 'matplotlib','numpy','scikit-learn','scipy','colourmap>=1.1.11','pandas','tqdm','scatterd>=1.3.1', 'adjusttext'],
      python_requires='>=3',
      name='pca',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="pca: A Python Package for Principal Component Analysis.",
      long_description=long_description,
```

