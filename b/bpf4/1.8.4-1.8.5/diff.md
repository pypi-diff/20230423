# Comparing `tmp/bpf4-1.8.4.tar.gz` & `tmp/bpf4-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpf4-1.8.4.tar", last modified: Tue Feb 21 19:14:02 2023, max compression
+gzip compressed data, was "bpf4-1.8.5.tar", last modified: Sun Apr 23 20:53:36 2023, max compression
```

## Comparing `bpf4-1.8.4.tar` & `bpf4-1.8.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-02-21 19:14:02.907461 bpf4-1.8.4/
--rwxrwxrwx   0 em        (1000) em        (1000)       19 2023-01-31 10:27:02.000000 bpf4-1.8.4/MANIFEST.in
--rw-rw-r--   0 em        (1000) em        (1000)     5052 2023-02-21 19:14:02.908461 bpf4-1.8.4/PKG-INFO
--rwxrwxr-x   0 em        (1000) em        (1000)     4593 2022-05-02 11:41:42.000000 bpf4-1.8.4/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-02-21 19:14:02.902461 bpf4-1.8.4/bpf4/
--rwxrwxr-x   0 em        (1000) em        (1000)      192 2023-01-31 10:44:01.000000 bpf4-1.8.4/bpf4/__init__.py
--rwxrwxr-x   0 em        (1000) em        (1000)    15595 2023-01-17 09:07:18.000000 bpf4-1.8.4/bpf4/api.py
--rw-rw-r--   0 em        (1000) em        (1000)     1859 2021-11-22 13:04:27.000000 bpf4-1.8.4/bpf4/arraytools.py
--rwxrwxr-x   0 em        (1000) em        (1000)      392 2021-11-22 13:04:27.000000 bpf4-1.8.4/bpf4/bench.py
--rwxrwxr-x   0 em        (1000) em        (1000)      341 2022-05-16 23:13:25.000000 bpf4-1.8.4/bpf4/config.py
--rw-rw-r--   0 em        (1000) em        (1000)  4912982 2023-01-31 10:28:20.000000 bpf4-1.8.4/bpf4/core.c
--rw-r--r--   0 em        (1000) em        (1000)     7501 2022-10-28 22:21:20.000000 bpf4-1.8.4/bpf4/core.pyi
--rwxrwxr-x   0 em        (1000) em        (1000)   176802 2023-01-22 21:28:52.000000 bpf4-1.8.4/bpf4/core.pyx
--rwxrwxr-x   0 em        (1000) em        (1000)     8159 2021-11-22 13:04:27.000000 bpf4-1.8.4/bpf4/csvtools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4027 2022-05-27 09:35:57.000000 bpf4-1.8.4/bpf4/plot.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2023-01-31 10:20:38.000000 bpf4-1.8.4/bpf4/py.typed
--rwxrwxr-x   0 em        (1000) em        (1000)     1289 2023-01-17 09:06:07.000000 bpf4-1.8.4/bpf4/pyinterp.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1420 2021-11-22 13:04:27.000000 bpf4-1.8.4/bpf4/tests.py
--rwxrwxr-x   0 em        (1000) em        (1000)    30349 2023-01-26 22:07:20.000000 bpf4-1.8.4/bpf4/util.py
--rwxrwxr-x   0 em        (1000) em        (1000)       85 2023-02-21 19:13:10.000000 bpf4-1.8.4/bpf4/version.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-02-21 19:14:02.905461 bpf4-1.8.4/bpf4.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     5052 2023-02-21 19:14:02.000000 bpf4-1.8.4/bpf4.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      430 2023-02-21 19:14:02.000000 bpf4-1.8.4/bpf4.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-02-21 19:14:02.000000 bpf4-1.8.4/bpf4.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       28 2023-02-21 19:14:02.000000 bpf4-1.8.4/bpf4.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        5 2023-02-21 19:14:02.000000 bpf4-1.8.4/bpf4.egg-info/top_level.txt
--rw-r--r--   0 em        (1000) em        (1000)      140 2022-04-15 16:33:34.000000 bpf4-1.8.4/pyproject.toml
--rw-r--r--   0 em        (1000) em        (1000)      265 2023-02-21 19:14:02.909461 bpf4-1.8.4/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1574 2023-02-21 19:13:44.000000 bpf4-1.8.4/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-02-21 19:14:02.906461 bpf4-1.8.4/tests/
--rwxrwxr-x   0 em        (1000) em        (1000)     1906 2021-11-22 13:04:27.000000 bpf4-1.8.4/tests/tests.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 20:53:36.346258 bpf4-1.8.5/
+-rwxrwxrwx   0 em        (1000) em        (1000)       19 2023-01-31 10:27:02.000000 bpf4-1.8.5/MANIFEST.in
+-rw-rw-r--   0 em        (1000) em        (1000)     5072 2023-04-23 20:53:36.347258 bpf4-1.8.5/PKG-INFO
+-rwxrwxr-x   0 em        (1000) em        (1000)     4593 2022-05-02 11:41:42.000000 bpf4-1.8.5/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 20:53:36.342258 bpf4-1.8.5/bpf4/
+-rwxrwxr-x   0 em        (1000) em        (1000)      192 2023-01-31 10:44:01.000000 bpf4-1.8.5/bpf4/__init__.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    15595 2023-01-17 09:07:18.000000 bpf4-1.8.5/bpf4/api.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1859 2021-11-22 13:04:27.000000 bpf4-1.8.5/bpf4/arraytools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)      392 2021-11-22 13:04:27.000000 bpf4-1.8.5/bpf4/bench.py
+-rwxrwxr-x   0 em        (1000) em        (1000)      341 2022-05-16 23:13:25.000000 bpf4-1.8.5/bpf4/config.py
+-rw-rw-r--   0 em        (1000) em        (1000)  4912982 2023-01-31 10:28:20.000000 bpf4-1.8.5/bpf4/core.c
+-rw-r--r--   0 em        (1000) em        (1000)     7577 2023-04-23 20:52:43.000000 bpf4-1.8.5/bpf4/core.pyi
+-rwxrwxr-x   0 em        (1000) em        (1000)   176802 2023-01-22 21:28:52.000000 bpf4-1.8.5/bpf4/core.pyx
+-rwxrwxr-x   0 em        (1000) em        (1000)     8159 2021-11-22 13:04:27.000000 bpf4-1.8.5/bpf4/csvtools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4027 2022-05-27 09:35:57.000000 bpf4-1.8.5/bpf4/plot.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2023-01-31 10:20:38.000000 bpf4-1.8.5/bpf4/py.typed
+-rwxrwxr-x   0 em        (1000) em        (1000)     1289 2023-01-17 09:06:07.000000 bpf4-1.8.5/bpf4/pyinterp.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1420 2021-11-22 13:04:27.000000 bpf4-1.8.5/bpf4/tests.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    30349 2023-01-26 22:07:20.000000 bpf4-1.8.5/bpf4/util.py
+-rwxrwxr-x   0 em        (1000) em        (1000)       85 2023-04-23 20:53:24.000000 bpf4-1.8.5/bpf4/version.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 20:53:36.345258 bpf4-1.8.5/bpf4.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     5072 2023-04-23 20:53:36.000000 bpf4-1.8.5/bpf4.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      430 2023-04-23 20:53:36.000000 bpf4-1.8.5/bpf4.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-23 20:53:36.000000 bpf4-1.8.5/bpf4.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       28 2023-04-23 20:53:36.000000 bpf4-1.8.5/bpf4.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        5 2023-04-23 20:53:36.000000 bpf4-1.8.5/bpf4.egg-info/top_level.txt
+-rw-r--r--   0 em        (1000) em        (1000)      140 2022-04-15 16:33:34.000000 bpf4-1.8.5/pyproject.toml
+-rw-r--r--   0 em        (1000) em        (1000)      265 2023-04-23 20:53:36.350258 bpf4-1.8.5/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     1574 2023-02-21 19:13:44.000000 bpf4-1.8.5/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 20:53:36.346258 bpf4-1.8.5/tests/
+-rwxrwxr-x   0 em        (1000) em        (1000)     1906 2021-11-22 13:04:27.000000 bpf4-1.8.5/tests/tests.py
```

### Comparing `bpf4-1.8.4/PKG-INFO` & `bpf4-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: bpf4
-Version: 1.8.4
+Version: 1.8.5
 Summary: Piece-wise interpolation and lazy evaluation in cython
 Home-page: https://github.com/gesellkammer/bpf4
-Download-URL: https://github.com/gesellkammer/bpf4
 Author: eduardo moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: BSD 3-Clause License
+Download-URL: https://github.com/gesellkammer/bpf4
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 BPF4
 ====
 
@@ -219,7 +220,9 @@
 r = 3 + (5*theta).cos()
 
 ax = plt.axes(polar=True)
 r.plot(axes=ax)
 
 ```
 ![](docs/assets/polar1.png)
+
+
```

### Comparing `bpf4-1.8.4/README.md` & `bpf4-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/api.py` & `bpf4-1.8.5/bpf4/api.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/arraytools.py` & `bpf4-1.8.5/bpf4/arraytools.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/core.c` & `bpf4-1.8.5/bpf4/core.c`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/core.pyi` & `bpf4-1.8.5/bpf4/core.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
        
     def __add__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
     
     def __sub__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
     
     def __mul__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
 
-	def __div__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+    def __div__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
 
-	def __truediv__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+    def __truediv__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
 
-	def __pow__(a: BpfInterface | float, b: BpfInterface | float, module: float) -> BpfInterface: ...
+    def __pow__(a: BpfInterface | float, b: BpfInterface | float, module: float) -> BpfInterface: ...
 
     def __neg__(self: BpfInterface) -> BpfInterface: ...
     
     def __mod__(self, other: BpfInterface | float) -> BpfInterface:
     
     def __abs__(self) -> BpfInterface: ...
     
@@ -91,28 +91,28 @@
     def log10(self) -> BpfInterface: ... 
 
     def log(self, base: float = 2.718281828459045) -> BpfInterface: ... 
     
     def m2f(self) -> BpfInterface: ... 
 
     def f2m(self) -> BpfInterface: ... 
-	def db2amp(self) -> BpfInterface: ... 
-	def amp2db(self) -> BpfInterface: ... 
-	def clip(self, y0: float = float('-inf'), y1: float = float('inf')) -> BpfInterface: ...
+    def db2amp(self) -> BpfInterface: ... 
+    def amp2db(self) -> BpfInterface: ... 
+    def clip(self, y0: float = float('-inf'), y1: float = float('inf')) -> BpfInterface: ...
     def derivative(self) -> BpfInterface: ...
     def integrated(self) -> BpfInterface: ...
-	def integrate(self) -> float: ...
-	def integrate_between(self, x0: float, x1: float, N: int = 0) -> float: ...
-	def mean(self) -> float: ...
-	def zeros(self, h: float = 0.01, N: int = 0, 
-	          x0: float = float('nan'), x1: float = float('nan'), maxzeros: int = 0) -> list[float]: ...
-	def max(self, b: BpfInterface|float) -> BpfInterface: ...
-	def min(self, b: BpfInterface|float) -> BpfInterface: ...
-	def __call__(self, other: float) -> float: ...
-	
+    def integrate(self) -> float: ...
+    def integrate_between(self, x0: float, x1: float, N: int = 0) -> float: ...
+    def mean(self) -> float: ...
+    def zeros(self, h: float = 0.01, N: int = 0, 
+              x0: float = float('nan'), x1: float = float('nan'), maxzeros: int = 0) -> list[float]: ...
+    def max(self, b: BpfInterface|float) -> BpfInterface: ...
+    def min(self, b: BpfInterface|float) -> BpfInterface: ...
+    def __call__(self, other: float) -> float: ...
+    
     def keep_slope(self, epsilon: float 0.) -> BpfInterface ...
         
     def outbound(self, y0: float, y1: float) -> BpfInterface: ...
         
     def apply(self, func) -> BpfInterface: ...
         
     def preapply(self, func) -> BpfInterface ...:
@@ -131,15 +131,15 @@
     def fromseq(cls, *points: float|tuple[float, float], **kws) -> BpfInterface: ...
         
     def copy(self) -> BpfInterface: ...
 
         
 class BpfBase(BpfInterface):
 
-    def __init__(BpfBase self, xs: np.ndarray|list[float], ys: np.ndarray | list[float]): ...
+    def __init__(self, xs: np.ndarray|list[float], ys: np.ndarray | list[float]): ...
         
     @property
     def descriptor(self) -> str: ... 
             
     def mapn_between(self, n: int, xstart: float, xend: float, out: np.ndarray = None) -> np.ndarray: ...
        
     def points(self) -> tuple[np.ndarray, np.ndarray]: ...
@@ -184,17 +184,17 @@
 class NoInterpol(BpfBase): ...
 
     
 class Nearest(BpfBase): ...
 
 
 class Sampled(BpfInterface): 
-	@property
-	def ys(self) -> np.ndarray: ...
-	
+    @property
+    def ys(self) -> np.ndarray: ...
+    
     def __init__(self, samples: np.ndarray, dx: float, x0: float = 0., interpolation: str = 'linear'): ...
         
     @property
     def samplerate(self) -> float: ...
         
     @property
     def xs(self) -> np.ndarray: ...
@@ -213,26 +213,26 @@
 
     
 
 class USpline(BpfInterface): ...
 
     
 class Slope(BpfInterface): ...
-	@property
-	def slope(self) -> float: ...
+    @property
+    def slope(self) -> float: ...
 
-	@slope.setter
-	def slope(self, value: float) -> None: ...
-	
-	@property
-	def offset(self) -> float:
-
-	@offset.setter
-	def offset(self, value: float) -> None: ...
-	
+    @slope.setter
+    def slope(self, value: float) -> None: ...
+    
+    @property
+    def offset(self) -> float:
+
+    @offset.setter
+    def offset(self, value: float) -> None: ...
+    
 
     
 class _BpfCompose(BpfInterface): ...
 
 
 class _BpfConcat(BpfInterface): ...
```

### Comparing `bpf4-1.8.4/bpf4/core.pyx` & `bpf4-1.8.5/bpf4/core.pyx`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/csvtools.py` & `bpf4-1.8.5/bpf4/csvtools.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/plot.py` & `bpf4-1.8.5/bpf4/plot.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/pyinterp.py` & `bpf4-1.8.5/bpf4/pyinterp.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/tests.py` & `bpf4-1.8.5/bpf4/tests.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4/util.py` & `bpf4-1.8.5/bpf4/util.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/bpf4.egg-info/PKG-INFO` & `bpf4-1.8.5/bpf4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: bpf4
-Version: 1.8.4
+Version: 1.8.5
 Summary: Piece-wise interpolation and lazy evaluation in cython
 Home-page: https://github.com/gesellkammer/bpf4
-Download-URL: https://github.com/gesellkammer/bpf4
 Author: eduardo moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: BSD 3-Clause License
+Download-URL: https://github.com/gesellkammer/bpf4
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 BPF4
 ====
 
@@ -219,7 +220,9 @@
 r = 3 + (5*theta).cos()
 
 ax = plt.axes(polar=True)
 r.plot(axes=ax)
 
 ```
 ![](docs/assets/polar1.png)
+
+
```

### Comparing `bpf4-1.8.4/setup.py` & `bpf4-1.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `bpf4-1.8.4/tests/tests.py` & `bpf4-1.8.5/tests/tests.py`

 * *Files identical despite different names*

