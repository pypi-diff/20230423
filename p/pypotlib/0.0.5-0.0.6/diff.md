# Comparing `tmp/pypotlib-0.0.5.tar.gz` & `tmp/pypotlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotlib-0.0.5.tar", last modified: Sat Apr 22 21:21:51 2023, max compression
+gzip compressed data, was "pypotlib-0.0.6.tar", last modified: Sat Apr 22 21:52:24 2023, max compression
```

## Comparing `pypotlib-0.0.5.tar` & `pypotlib-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.clang-format
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.github/workflows/build_test.yml
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.gitignore
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.5/CODEOWNERS
--rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.5/LICENSE
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pypotlib-0.0.5/README.md
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.5/environment.yml
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 pypotlib-0.0.5/meson.build
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.cc
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.hpp
--rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.cc
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.hpp
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_potential.cc
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_potential.hpp
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_pottypes.cc
--rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_wrapper.cc
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_wrapper.hpp
--rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pypotlib/__init__.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pypotlib/ase_adapters.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.5/subprojects/potlib.wrap
--rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 pypotlib-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.clang-format
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.github/workflows/build_test.yml
+-rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.gitignore
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.6/CODEOWNERS
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pypotlib-0.0.6/README.md
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.6/environment.yml
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 pypotlib-0.0.6/meson.build
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.cc
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.hpp
+-rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.cc
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.hpp
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_potential.cc
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_potential.hpp
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_pottypes.cc
+-rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_wrapper.cc
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_wrapper.hpp
+-rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pypotlib/__init__.py
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pypotlib/ase_adapters.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.6/subprojects/potlib.wrap
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 pypotlib-0.0.6/PKG-INFO
```

### Comparing `pypotlib-0.0.5/.clang-format` & `pypotlib-0.0.6/.clang-format`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/.github/workflows/build_wheels.yml` & `pypotlib-0.0.6/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/.gitignore` & `pypotlib-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/CODEOWNERS` & `pypotlib-0.0.6/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/CODE_OF_CONDUCT.md` & `pypotlib-0.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/LICENSE` & `pypotlib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/README.md` & `pypotlib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/meson.build` & `pypotlib-0.0.6/meson.build`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('pypotlib', 'cpp',
-       version: '0.0.5',
+       version: '0.0.6',
   default_options : ['warning_level=2', 'cpp_std=c++17'])
 # IMPORTANT!! warning_level=3 passes -fimplicit-none
 # Many of the older Fortran codes need implicit typing
 
 host_system = host_machine.system()
 
 # Add C++ compiler options
```

### Comparing `pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.hpp` & `pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.hpp` & `pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/pyb11_srcs/py_potential.hpp` & `pypotlib-0.0.6/pyb11_srcs/py_potential.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/pyb11_srcs/py_wrapper.hpp` & `pypotlib-0.0.6/pyb11_srcs/py_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.5/pypotlib/ase_adapters.py` & `pypotlib-0.0.6/pypotlib/ase_adapters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 __all__ = ["PyPotLibCalc"]
 
 import warnings
 import numpy as np
 from ase.calculators.calculator import Calculator, all_changes
 
+
 class PyPotLibCalc(Calculator):
-    implemented_properties = ['energy', 'forces']
+    implemented_properties = ["energy", "forces"]
     discard_results_on_any_change = True
 
     def __init__(self, cpot_instance):
         Calculator.__init__(self)
         self.cpot = cpot_instance
 
-    def calculate(self, atoms=None,
-                  properties=['energy'],
-                  system_changes=all_changes):
-        Calculator.calculate(self, atoms,
-                             properties, system_changes)
+    def calculate(
+        self, atoms=None, properties=["energy"], system_changes=all_changes
+    ):
+        Calculator.calculate(self, atoms, properties, system_changes)
         positions = atoms.get_positions()
         atmtypes = atoms.get_atomic_numbers()
         box = atoms.get_cell()
         if np.all(box == np.zeros(3)):
             warnings.warn("Box is zero, setting to rectangular 100, 100, 100")
-            box = np.eye(3)*100
+            box = np.eye(3) * 100
         energy, forces = self.cpot(positions, atmtypes, box)
-        self.results['energy'] = energy
-        self.results['forces'] = forces
+        self.results["energy"] = energy
+        self.results["forces"] = forces
```

### Comparing `pypotlib-0.0.5/pyproject.toml` & `pypotlib-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.pdm]
 
 [project]
 name = "pypotlib"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python bindings and ASE adapters for potlib"
 authors = [
     {name = "Rohit Goswami", email = "rog32@hi.is"},
 ]
 # These are only if ase integration is requested, consider a group
 dependencies = [
     "numpy>=1.24.2",
     "ase>=3.22.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "MIT"}
 
+[project.urls]
+"Source Code" = "https://github.com/TheochemUI/pypotlib"
+"Bug Tracker" = "https://github.com/TheochemUI/pypotlib/issues"
+
 [build-system]
 requires = ["wheel", "setuptools", "pybind11", "meson-python"]
 build-backend = "mesonpy"
 
 [tool.cibuildwheel.linux]
 manylinux-x86_64-image = "manylinux2014"
 manylinux-i686-image = "manylinux2014"
@@ -34,7 +38,20 @@
 repair-wheel-command = ""
 # Openblas for musllinux is painful, so don't install / test
 test-skip = "*-musllinux*"
 
 [tool.cibuildwheel.macos]
 environment = { RUNNER_OS="macOS" }
 before-all = "brew install gfortran && brew unlink gfortran && brew link gfortran"
+
+[tool.pdm.dev-dependencies]
+lint = [
+    "black>=23.1.0",
+]
+
+[tool.pdm.scripts]
+lint = "black"
+all = {composite = ["lint pypotlib/"]}
+
+[tool.black]
+line-length = 80
+target-version = ['py310']
```

### Comparing `pypotlib-0.0.5/PKG-INFO` & `pypotlib-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: pypotlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python bindings and ASE adapters for potlib
 Author-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
+Project-URL: Source code, https://github.com/TheochemUI/pypotlib
+Project-URL: Bug tracker, https://github.com/TheochemUI/pypotlib/issues
 Requires-Python: >=3.10
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: ase>=3.22.1
 Description-Content-Type: text/markdown
 
 # `pypotlib` [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) ![Builds](https://github.com/TheochemUI/pypotlib/actions/workflows/build_test.yml/badge.svg) ![Wheels](https://github.com/TheochemUI/pypotlib/actions/workflows/build_wheels.yml/badge.svg)
```

