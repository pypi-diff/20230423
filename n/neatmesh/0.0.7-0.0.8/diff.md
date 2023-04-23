# Comparing `tmp/neatmesh-0.0.7.tar.gz` & `tmp/neatmesh-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neatmesh-0.0.7.tar", last modified: Sat Apr 22 14:14:10 2023, max compression
+gzip compressed data, was "neatmesh-0.0.8.tar", last modified: Sun Apr 23 01:17:00 2023, max compression
```

## Comparing `neatmesh-0.0.7.tar` & `neatmesh-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.899921 neatmesh-0.0.7/
--rw-rw-rw-   0        0        0     1093 2023-02-11 14:00:08.000000 neatmesh-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3898 2023-04-22 14:14:10.899921 neatmesh-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3307 2023-01-08 08:11:50.000000 neatmesh-0.0.7/README.md
--rw-rw-rw-   0        0        0       86 2022-03-17 16:26:16.000000 neatmesh-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      929 2023-04-22 14:14:10.899921 neatmesh-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.837048 neatmesh-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.868661 neatmesh-0.0.7/src/neatmesh/
--rw-rw-rw-   0        0        0      307 2023-04-22 13:54:58.000000 neatmesh-0.0.7/src/neatmesh/__init__.py
--rw-rw-rw-   0        0        0    13410 2023-04-22 14:10:19.000000 neatmesh-0.0.7/src/neatmesh/_analyzer.py
--rw-rw-rw-   0        0        0     2367 2022-09-26 00:23:46.000000 neatmesh-0.0.7/src/neatmesh/_cli.py
--rw-rw-rw-   0        0        0     1646 2022-09-26 17:10:51.000000 neatmesh-0.0.7/src/neatmesh/_common.py
--rw-rw-rw-   0        0        0      486 2022-09-26 00:24:47.000000 neatmesh-0.0.7/src/neatmesh/_exceptions.py
--rw-rw-rw-   0        0        0    12437 2022-09-24 07:10:36.000000 neatmesh-0.0.7/src/neatmesh/_geometry.py
--rw-rw-rw-   0        0        0     3981 2023-04-22 13:54:52.000000 neatmesh-0.0.7/src/neatmesh/_mesh.py
--rw-rw-rw-   0        0        0     8268 2023-04-22 13:54:58.000000 neatmesh-0.0.7/src/neatmesh/_reader.py
--rw-rw-rw-   0        0        0    12253 2023-04-22 14:11:18.000000 neatmesh-0.0.7/src/neatmesh/_reporter.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.884296 neatmesh-0.0.7/src/neatmesh.egg-info/
--rw-rw-rw-   0        0        0     3898 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      704 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.884296 neatmesh-0.0.7/tests/
--rw-rw-rw-   0        0        0     1438 2022-09-25 16:20:17.000000 neatmesh-0.0.7/tests/test_analyzer2d.py
--rw-rw-rw-   0        0        0      596 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_analyzer3d_hex.py
--rw-rw-rw-   0        0        0      962 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_analyzer3d_tetra.py
--rw-rw-rw-   0        0        0      368 2022-09-28 15:59:19.000000 neatmesh-0.0.7/tests/test_dimensionality.py
--rw-rw-rw-   0        0        0     1911 2022-09-28 15:59:19.000000 neatmesh-0.0.7/tests/test_mesh2d.py
--rw-rw-rw-   0        0        0      537 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_pyramid_geometry.py
--rw-rw-rw-   0        0        0      648 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_tri_geometry.py
--rw-rw-rw-   0        0        0      553 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_wedge_geometry.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:00.736309 neatmesh-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2023-02-11 14:00:08.000000 neatmesh-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3898 2023-04-23 01:17:00.736309 neatmesh-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3307 2023-01-08 08:11:50.000000 neatmesh-0.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-17 16:26:16.000000 neatmesh-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      929 2023-04-23 01:17:00.744308 neatmesh-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:00.489606 neatmesh-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:00.616318 neatmesh-0.0.8/src/neatmesh/
+-rw-rw-rw-   0        0        0      307 2023-04-22 13:54:58.000000 neatmesh-0.0.8/src/neatmesh/__init__.py
+-rw-rw-rw-   0        0        0    13528 2023-04-23 01:07:44.000000 neatmesh-0.0.8/src/neatmesh/_analyzer.py
+-rw-rw-rw-   0        0        0     2367 2022-09-26 00:23:46.000000 neatmesh-0.0.8/src/neatmesh/_cli.py
+-rw-rw-rw-   0        0        0     1646 2022-09-26 17:10:51.000000 neatmesh-0.0.8/src/neatmesh/_common.py
+-rw-rw-rw-   0        0        0      486 2022-09-26 00:24:47.000000 neatmesh-0.0.8/src/neatmesh/_exceptions.py
+-rw-rw-rw-   0        0        0    12437 2022-09-24 07:10:36.000000 neatmesh-0.0.8/src/neatmesh/_geometry.py
+-rw-rw-rw-   0        0        0     3981 2023-04-22 13:54:52.000000 neatmesh-0.0.8/src/neatmesh/_mesh.py
+-rw-rw-rw-   0        0        0     8268 2023-04-22 13:54:58.000000 neatmesh-0.0.8/src/neatmesh/_reader.py
+-rw-rw-rw-   0        0        0    12534 2023-04-23 01:12:55.000000 neatmesh-0.0.8/src/neatmesh/_reporter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:00.696339 neatmesh-0.0.8/src/neatmesh.egg-info/
+-rw-rw-rw-   0        0        0     3898 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 01:17:00.000000 neatmesh-0.0.8/src/neatmesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:00.728298 neatmesh-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1438 2022-09-25 16:20:17.000000 neatmesh-0.0.8/tests/test_analyzer2d.py
+-rw-rw-rw-   0        0        0      596 2022-09-26 17:04:13.000000 neatmesh-0.0.8/tests/test_analyzer3d_hex.py
+-rw-rw-rw-   0        0        0      962 2022-09-26 17:04:13.000000 neatmesh-0.0.8/tests/test_analyzer3d_tetra.py
+-rw-rw-rw-   0        0        0      368 2022-09-28 15:59:19.000000 neatmesh-0.0.8/tests/test_dimensionality.py
+-rw-rw-rw-   0        0        0     1911 2022-09-28 15:59:19.000000 neatmesh-0.0.8/tests/test_mesh2d.py
+-rw-rw-rw-   0        0        0      537 2022-09-26 17:04:13.000000 neatmesh-0.0.8/tests/test_pyramid_geometry.py
+-rw-rw-rw-   0        0        0      648 2022-09-26 17:04:13.000000 neatmesh-0.0.8/tests/test_tri_geometry.py
+-rw-rw-rw-   0        0        0      553 2022-09-26 17:04:13.000000 neatmesh-0.0.8/tests/test_wedge_geometry.py
```

### Comparing `neatmesh-0.0.7/LICENSE` & `neatmesh-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/PKG-INFO` & `neatmesh-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neatmesh
-Version: 0.0.7
+Version: 0.0.8
 Summary: Finite Volume Mesh Quality Inspector
 Home-page: https://github.com/eigemx/neatmesh
 Author: Mohamed Emara
 Author-email: mae.emara@gmail.com
 Project-URL: Bug Tracker, https://github.com/eigemx/neatmesh/issues
 Keywords: mesh,scientific,engineering,fvm,fem,finite volume,finite element
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neatmesh-0.0.7/README.md` & `neatmesh-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/setup.cfg` & `neatmesh-0.0.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6561 746d 6573 680d 0a76 6572   = neatmesh..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
+00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
 00000030: 7468 6f72 203d 204d 6f68 616d 6564 2045  thor = Mohamed E
 00000040: 6d61 7261 0d0a 6175 7468 6f72 5f65 6d61  mara..author_ema
 00000050: 696c 203d 206d 6165 2e65 6d61 7261 4067  il = mae.emara@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4669 6e69 7465 2056  ption = Finite V
 00000080: 6f6c 756d 6520 4d65 7368 2051 7561 6c69  olume Mesh Quali
 00000090: 7479 2049 6e73 7065 6374 6f72 0d0a 6c6f  ty Inspector..lo
```

### Comparing `neatmesh-0.0.7/src/neatmesh/_analyzer.py` & `neatmesh-0.0.8/src/neatmesh/_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,18 @@
         self.non_ortho: np.ndarray = np.array([])
         self.adj_ratio: np.ndarray = np.array([])
 
     def duplicate_nodes_count(self) -> int:
         """Count number of duplicate points/nodes"""
         return self.points.shape[0] - np.unique(self.points, axis=0).shape[0]
 
+    def area(self) -> float:
+        """Calculate the area of the mesh"""
+        return np.sum(self.face_areas)
+
     def bounding_box(self) -> Tuple:
         """Return coordinates of bounding box of the mesh (min & max coords)"""
         x_min, y_min = np.min(self.points, axis=0)
         x_max, y_max = np.max(self.points, axis=0)
 
         return (
             (x_min, y_min),
```

### Comparing `neatmesh-0.0.7/src/neatmesh/_cli.py` & `neatmesh-0.0.8/src/neatmesh/_cli.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/src/neatmesh/_common.py` & `neatmesh-0.0.8/src/neatmesh/_common.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/src/neatmesh/_geometry.py` & `neatmesh-0.0.8/src/neatmesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/src/neatmesh/_mesh.py` & `neatmesh-0.0.8/src/neatmesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/src/neatmesh/_reader.py` & `neatmesh-0.0.8/src/neatmesh/_reader.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/src/neatmesh/_reporter.py` & `neatmesh-0.0.8/src/neatmesh/_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,18 @@
             f"Inspecting file [cyan]'{filename}'[/] (file size: {fsize})"
         )
         self.console.print()
 
     def report_bounding_box(self):
         self.console.print("[yellow bold]Mesh bounding box: ")
         for point in self.analyzer.bounding_box():
-            print(f"\t({point[0]:.4f}, {point[1]:.4f}, {point[2]:.4f})")
+            if len(point) == 3:
+                print(f"\t({point[0]:.4f}, {point[1]:.4f}, {point[2]:.4f})")
+            else:
+                print(f"\t({point[0]:.4f}, {point[1]:.4f})")
         self.console.print()
 
     def report_concerns(self):
         if self.concerns:
             concerns_table = Table(box=None)
             concerns_table.add_column("", justify="left")
 
@@ -135,14 +138,19 @@
             self.console.print()
 
 
 class Reporter2D(Reporter):
     def __init__(self, console: Console, mesh: MeshReader, filename: str) -> None:
         super().__init__(console, mesh, filename)
 
+    def report_mesh_area(self):
+        self.console.print(
+            f"Mesh area = {self.analyzer.area():.4f} [L^2] (in mesh units)\n"
+        )
+
     def report_elements_count(self):
         face_count = self.analyzer.n_faces
         edge_count = self.analyzer.n_edges
         point_count = self.analyzer.n_points
 
         tree = Tree(label="[yellow bold]Elements Stats.")
 
@@ -194,14 +202,15 @@
 
         if not rules:
             self.console.print("No quality rules file found, using defaults.\n")
         else:
             self.console.print(f"Found quality rules file: '{rules['fname']}'\n")
 
         self.report_bounding_box()
+        self.report_mesh_area()
         self.report_elements_count()
 
         quality_metric_dict = {
             "Face Area": {"array": self.analyzer.face_areas, "sci_not": True,},
             "Face Aspect Ratio": {
                 "array": self.analyzer.face_aspect_ratios,
                 "sci_not": False,
@@ -230,17 +239,15 @@
     def report_mesh_volume(self):
         self.console.print(
             f"Mesh volume = {self.analyzer.mesh_volume:.3f} [L^3] (in mesh units)"
         )
 
     def report_mesh_surface_area(self):
         s_area = self.analyzer.surface_area()
-        self.console.print(
-            f"Mesh surface area = {s_area:.3f} [L^2] (in mesh units)\n"
-        )
+        self.console.print(f"Mesh surface area = {s_area:.3f} [L^2] (in mesh units)\n")
 
     def report_elements_count(self):
         cell_count = self.analyzer.n_cells
         face_count = self.analyzer.n_faces
         point_count = self.analyzer.n_points
 
         tree = Tree(label="[yellow bold]Elements Stats.")
```

### Comparing `neatmesh-0.0.7/src/neatmesh.egg-info/PKG-INFO` & `neatmesh-0.0.8/src/neatmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neatmesh
-Version: 0.0.7
+Version: 0.0.8
 Summary: Finite Volume Mesh Quality Inspector
 Home-page: https://github.com/eigemx/neatmesh
 Author: Mohamed Emara
 Author-email: mae.emara@gmail.com
 Project-URL: Bug Tracker, https://github.com/eigemx/neatmesh/issues
 Keywords: mesh,scientific,engineering,fvm,fem,finite volume,finite element
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neatmesh-0.0.7/src/neatmesh.egg-info/SOURCES.txt` & `neatmesh-0.0.8/src/neatmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_analyzer2d.py` & `neatmesh-0.0.8/tests/test_analyzer2d.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_analyzer3d_hex.py` & `neatmesh-0.0.8/tests/test_analyzer3d_hex.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_analyzer3d_tetra.py` & `neatmesh-0.0.8/tests/test_analyzer3d_tetra.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_mesh2d.py` & `neatmesh-0.0.8/tests/test_mesh2d.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_pyramid_geometry.py` & `neatmesh-0.0.8/tests/test_pyramid_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_tri_geometry.py` & `neatmesh-0.0.8/tests/test_tri_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.7/tests/test_wedge_geometry.py` & `neatmesh-0.0.8/tests/test_wedge_geometry.py`

 * *Files identical despite different names*

