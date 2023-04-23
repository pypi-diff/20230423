# Comparing `tmp/MazeSolvingAlgos-1.4.tar.gz` & `tmp/MazeSolvingAlgos-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PyModulesByCPP\MazeSolvingAlgos\dist\.tmp-o6klm5kz\MazeSolvingAlgos-1.4.tar", last modified: Thu Apr  6 15:01:23 2023, max compression
+gzip compressed data, was "dist\MazeSolvingAlgos-1.5.tar", last modified: Sun Apr 23 06:21:09 2023, max compression
```

## Comparing `MazeSolvingAlgos-1.4.tar` & `MazeSolvingAlgos-1.5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 15:01:23.242438 MazeSolvingAlgos-1.4/
-drwxrwxrwx   0        0        0        0 2023-04-06 15:01:23.236122 MazeSolvingAlgos-1.4/MazeSolvingAlgos.egg-info/
--rw-rw-rw-   0        0        0     3646 2023-04-06 15:01:23.000000 MazeSolvingAlgos-1.4/MazeSolvingAlgos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-06 15:01:23.000000 MazeSolvingAlgos-1.4/MazeSolvingAlgos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 15:01:23.000000 MazeSolvingAlgos-1.4/MazeSolvingAlgos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-06 15:01:23.000000 MazeSolvingAlgos-1.4/MazeSolvingAlgos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3646 2023-04-06 15:01:23.241435 MazeSolvingAlgos-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2811 2023-04-06 14:58:37.000000 MazeSolvingAlgos-1.4/README.md
--rw-rw-rw-   0        0        0     2501 2023-04-06 14:33:55.000000 MazeSolvingAlgos-1.4/main.cpp
--rw-rw-rw-   0        0        0      940 2023-04-06 15:00:59.000000 MazeSolvingAlgos-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 15:01:23.243441 MazeSolvingAlgos-1.4/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-04-06 11:57:50.000000 MazeSolvingAlgos-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:21:09.759736 MazeSolvingAlgos-1.5/
+drwxrwxrwx   0        0        0        0 2023-04-23 06:21:09.757755 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-04-23 06:21:09.000000 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-23 06:21:09.000000 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:21:09.000000 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-23 06:21:09.000000 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 06:21:09.000000 MazeSolvingAlgos-1.5/MazeSolvingAlgos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      667 2023-04-23 06:21:09.758736 MazeSolvingAlgos-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1917 2023-04-23 06:01:17.000000 MazeSolvingAlgos-1.5/main.cpp
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:21:09.760736 MazeSolvingAlgos-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-23 06:20:55.000000 MazeSolvingAlgos-1.5/setup.py
```

### Comparing `MazeSolvingAlgos-1.4/main.cpp` & `MazeSolvingAlgos-1.5/main.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-#include "C:/Users/mahmo/AppData/Roaming/Python/Python39/site-packages/pybind11/include/pybind11/pybind11.h"
-#include "C:/Users/mahmo/AppData/Roaming/Python/Python39/site-packages/pybind11/include/pybind11/detail/common.h"
-#include "C:/Users/mahmo/AppData/Roaming/Python/Python39/site-packages/pybind11/include/pybind11/stl.h"
-#include "C:/Users/mahmo/AppData/Roaming/Python/Python39/site-packages/pybind11/include/pybind11/cast.h"
-#include "C:/Users/mahmo/AppData/Roaming/Python/Python39/site-packages/pybind11/include/pybind11/complex.h"
-
-
-
-#include "D:/PyModulesByCPP/MazeSolvingAlgos/GraphTraversalAlgorithms.h"
-#include "D:/PyModulesByCPP/MazeSolvingAlgos/MazeGenerator.h"
-//#include "Graph.h"
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include "GraphTraversalAlgorithms.h"
+#include "MazeGenerator.h"
 namespace py = pybind11;
 #define AddGTAclass(GTA /*GraphTraversalAlgorithm*/){               \
     py::class_<GTA>(m, #GTA)                                        \
         .def(py::init<Grid&, Index, Index>(),                       \
             py::arg("grid"), py::arg("start"), py::arg("end"))      \
         .def("solve", &GTA::solve)                                  \
         .def("SrcToDestPath", &GTA::SrcToDestPath)                  \
```

