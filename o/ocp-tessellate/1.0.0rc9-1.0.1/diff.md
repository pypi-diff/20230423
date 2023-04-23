# Comparing `tmp/ocp_tessellate-1.0.0rc9.tar.gz` & `tmp/ocp_tessellate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.0rc9.tar", last modified: Mon Mar  6 08:01:37 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.0.1.tar", last modified: Sun Apr 23 16:08:07 2023, max compression
```

## Comparing `ocp_tessellate-1.0.0rc9.tar` & `ocp_tessellate-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.339228 ocp_tessellate-1.0.0rc9/
--rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-03-06 08:01:37.339287 ocp_tessellate-1.0.0rc9/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.0rc9/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.338524 ocp_tessellate-1.0.0rc9/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1126 2023-03-04 18:58:11.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12354 2023-03-05 17:05:19.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    23309 2023-03-05 17:41:50.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10345 2023-02-27 07:20:24.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19108 2023-03-01 18:54:17.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13212 2023-03-05 18:04:14.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     5824 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.339146 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      532 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      129 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      674 2023-03-06 08:01:37.339547 ocp_tessellate-1.0.0rc9/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1647 2023-03-04 18:58:11.000000 ocp_tessellate-1.0.0rc9/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998796 ocp_tessellate-1.0.1/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-23 16:08:07.998848 ocp_tessellate-1.0.1/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.1/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998112 ocp_tessellate-1.0.1/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.1/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-04-23 16:07:54.000000 ocp_tessellate-1.0.1/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.1/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    26909 2023-04-23 16:07:04.000000 ocp_tessellate-1.0.1/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-21 16:07:20.000000 ocp_tessellate-1.0.1/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.1/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.1/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.1/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.1/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.1/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6137 2023-04-07 10:44:39.000000 ocp_tessellate-1.0.1/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998702 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-04-23 16:08:07.999096 ocp_tessellate-1.0.1/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-04-23 16:07:54.000000 ocp_tessellate-1.0.1/setup.py
```

### Comparing `ocp_tessellate-1.0.0rc9/PKG-INFO` & `ocp_tessellate-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.0.0rc9
+Version: 1.0.1
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/__init__.py` & `ocp_tessellate-1.0.1/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/_version.py` & `ocp_tessellate-1.0.1/ocp_tessellate/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.0rc9"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.0.1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.0.1/ocp_tessellate/cad_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     get_point,
     loc_to_tq,
     get_location,
     np_bbox,
     is_line,
     line,
     make_compound,
+    identity_location,
+    cross,
 )
 from .tessellator import discretize_edge, tessellate, compute_quality
 from .mp_tessellator import is_apply_result, mp_tessellate, init_pool, keymap
 from .defaults import get_default
 
 UNSELECTED = 0
 SELECTED = 1
@@ -88,14 +90,15 @@
     def __init__(
         self, shape, name="Part", color=None, show_faces=True, show_edges=True
     ):
         super().__init__()
         self.name = name
         self.id = None
         self.color = Color(get_default("default_color") if color is None else color)
+        self.loc = identity_location()
 
         self.shape = shape
         self.set_states(show_faces, show_edges)
         self.renderback = False
 
     def set_states(self, show_faces, show_edges):
         self.state_faces = SELECTED if show_faces else UNSELECTED
@@ -150,15 +153,18 @@
                     compute_edges=render_edges,
                     progress=progress,
                 )
 
                 t.info = f"{{quality:{quality:.4f}, angular_tolerance:{angular_tolerance:.2f}}}"
 
         with Timer(timeit, self.name, "bounding box:   ", 2):
-            t, q = loc_to_tq(get_location(loc))
+            combined_loc = get_location(loc, False)
+            if self.loc is not None:
+                combined_loc = combined_loc * self.loc
+            t, q = loc_to_tq(combined_loc)
             if parallel and is_apply_result(mesh):
                 # store the instance mesh
                 if ind is not None and INSTANCES[ind].mesh is None:
                     INSTANCES[ind].mesh = mesh
                     INSTANCES[ind].quality = quality
                 mesh = {"ref": ind, "t": t, "q": q}
                 bb = {}
@@ -182,14 +188,15 @@
         return {
             "id": self.id,
             "type": "shapes",
             "name": self.name,
             "shape": mesh,
             "color": color,
             "alpha": alpha,
+            "loc": None if self.loc is None else loc_to_tq(self.loc),
             "renderback": self.renderback,
             "accuracy": quality,
             "bb": bb,
         }
 
     def compound(self):
         return make_compound(self.shape)
@@ -202,14 +209,15 @@
     def __init__(
         self, faces, name="Faces", color=None, show_faces=True, show_edges=True
     ):
         super().__init__(
             faces, name, color, show_faces, show_edges
         )  # TODO combine faces
         self.color = Color(color or (238, 130, 238))
+        self.loc = None
         self.renderback = True
 
 
 class OCP_Edges(CADObject):
     def __init__(self, edges, name="Edges", color=None, width=1):
         super().__init__()
         self.shape = edges
@@ -219,14 +227,15 @@
         if color is not None:
             if isinstance(color, (list, tuple)) and isinstance(color[0], Color):
                 self.color = color
             elif isinstance(color, Color):
                 self.color = color
             else:
                 self.color = Color(color)
+        self.loc = None
         self.width = width
 
     def to_state(self):
         return [EMPTY, SELECTED]
 
     def to_assembly(self):
         return OCP_PartGroup([self])
@@ -247,15 +256,16 @@
 
         with Timer(timeit, self.name, "bounding box:", 2) as t:
             bb = bounding_box(self.shape, loc=get_location(loc))
             quality = compute_quality(bb, deviation=deviation)
             deflection = quality / 100 if edge_accuracy is None else edge_accuracy
             t.info = str(bb)
 
-        with Timer(timeit, self.name, "discretize:  ", 2):
+        with Timer(timeit, self.name, "discretize:  ", 2) as t:
+            t.info = f"quality: {quality}, deflection: {deflection}"
             edges = []
             for edge in self.shape:
                 d = discretize_edge(edge, deflection)
                 if len(d) == 1 and not is_line(edge):
                     num = int(0.1 / deflection)
                     d = discretize_edge(edge, num=num)
                 edges.extend(d)
@@ -272,26 +282,28 @@
 
         return {
             "id": self.id,
             "type": "edges",
             "name": self.name,
             "shape": edges,
             "color": color,
+            "loc": None if self.loc is None else loc_to_tq(self.loc),
             "width": self.width,
             "bb": bb.to_dict(),
         }
 
 
 class OCP_Vertices(CADObject):
     def __init__(self, vertices, name="Vertices", color=None, size=1):
         super().__init__()
         self.shape = vertices
         self.name = name
         self.id = None
         self.color = Color(color or (148, 0, 211))
+        self.loc = None
         self.size = size
 
     def to_state(self):
         return [EMPTY, SELECTED]
 
     def to_assembly(self):
         return OCP_PartGroup([self])
@@ -319,25 +331,26 @@
             "id": self.id,
             "type": "vertices",
             "name": self.name,
             "shape": np.asarray(
                 [get_point(vertex) for vertex in self.shape], dtype="float32"
             ),
             "color": self.color.web_color,
+            "loc": None if self.loc is None else loc_to_tq(self.loc),
             "size": self.size,
             "bb": bb.to_dict(),
         }
 
 
 class OCP_PartGroup(CADObject):
     def __init__(self, objects, name="Group", loc=None):
         super().__init__()
         self.objects = objects
         self.name = name
-        self.loc = loc
+        self.loc = identity_location() if loc is None else loc
         self.id = None
 
     def to_nav_dict(self):
         return {
             "type": "node",
             "name": self.name,
             "id": self.id,
@@ -374,14 +387,15 @@
         else:
             combined_loc = loc * self.loc
 
         result = {
             "parts": [],
             "loc": None if self.loc is None else loc_to_tq(self.loc),
             "name": self.name,
+            "id": self.id,
         }
         for obj in self.objects:
             result["parts"].append(
                 obj.collect_shapes(
                     self.id,
                     combined_loc,
                     deviation,
@@ -425,13 +439,14 @@
         return result
 
     def compound(self):
         return make_compound(self.compounds())
 
 
 class CoordSystem(OCP_Edges):
-    def __init__(self, name, origin, x_dir, y_dir, z_dir, length):
-        x_edge = line(origin, [o + v * length for o, v in zip(origin, x_dir)])
-        y_edge = line(origin, [o + v * length for o, v in zip(origin, y_dir)])
-        z_edge = line(origin, [o + v * length for o, v in zip(origin, z_dir)])
+    def __init__(self, name, origin, X, Z, size=1):
+        Y = cross(X, Z)
+        x_edge = line(origin, [o + v * size for o, v in zip(origin, X)])
+        y_edge = line(origin, [o + v * size for o, v in zip(origin, Y)])
+        z_edge = line(origin, [o + v * size for o, v in zip(origin, Z)])
         colors = (Color("red"), Color("green"), Color("blue"))
         super().__init__([x_edge, y_edge, z_edge], name, colors, width=3)
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/convert.py` & `ocp_tessellate-1.0.1/ocp_tessellate/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from collections.abc import Iterable
 
+import json
+
 from .cad_objects import (
     CoordSystem,
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_PartGroup,
     OCP_Vertices,
@@ -45,14 +47,15 @@
     is_build123d_shape,
     is_build123d,
     is_cadquery_assembly,
     is_cadquery_massembly,
     is_cadquery_sketch,
     is_cadquery,
     is_compound,
+    is_mixed_compound,
     is_edge_list,
     is_face_list,
     is_compound_list,
     is_solid_list,
     is_toploc_location,
     is_topods_compound,
     is_topods_edge,
@@ -67,33 +70,34 @@
     is_wrapped,
     make_compound,
     np_bbox,
     ocp_color,
     vertex,
     loc_to_tq,
 )
-from .utils import Color
+
+from .utils import Color, make_unique, numpy_to_json
 
 EDGE_COLOR = "Silver"
 THICK_EDGE_COLOR = "MediumOrchid"
 VERTEX_COLOR = "MediumOrchid"
 FACE_COLOR = "Violet"
 
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
 GROUP_NAME_LUT = {
-    "OCP_Part": "Solids",
-    "OCP_Faces": "Faces",
-    "OCP_Edges": "Edges",
-    "OCP_Vertices": "Vertices",
+    "OCP_Part": "Solid",
+    "OCP_Faces": "Face",
+    "OCP_Edges": "Edge",
+    "OCP_Vertices": "Vertex",
 }
 
 
-def _debug(msg):
-    # print("DEBUG:", msg)
+def _debug(*msg):
+    # print("DEBUG:", *msg)
     pass
 
 
 def web_color(name):
     wc = Color(name)
     return ocp_color(*wc.percentage)
 
@@ -226,223 +230,181 @@
                 )
             ]
         cad_objs.extend(objs)
 
     return cad_objs
 
 
-def conv(cad_obj, grp_id=1, obj_name=None, obj_color=None, obj_alpha=1.0):
-    if isinstance(cad_obj, OCP_PartGroup):
-        return cad_obj
-
-    elif isinstance(cad_obj, (OCP_Faces, OCP_Edges, OCP_Vertices)):
-        cad_obj.name = f"{cad_obj.name}_{grp_id}"
-        pg = OCP_PartGroup([cad_obj], name=cad_obj.name)
-        return pg
-
+def conv(cad_obj, obj_name=None, obj_color=None, obj_alpha=1.0):
     default_color = get_default("default_color")
 
     if obj_name is None and hasattr(cad_obj, "label") and cad_obj.label != "":
         obj_name = cad_obj.label
 
     cad_objs = []
 
     # BuildPart, BuildSketch, BuildLine
     if is_build123d(cad_obj):
-        _debug(f"build123d Builder {grp_id}: {type(cad_obj)}")
+        _debug(f"        conv: build123d Builder {type(cad_obj)}")
         cad_obj = getattr(cad_obj, cad_obj._obj_name)  # convert to direct API
 
     if is_build123d_compound(cad_obj):
-        # build123d assembly
-        if is_build123d_assembly(cad_obj):
-            _debug(f"build123d Assembly {grp_id}: {type(cad_obj)}")
-            cad_objs = []
-            raise NotImplemented("build123d assemblies not implemented yet")
-
-        # build123d Compound
-        else:
-            _debug(f"build123d Compound {grp_id}: {type(cad_obj)}")
-            cad_objs = [cad_obj.wrapped]
+        _debug(f"        conv: build123d Compound {type(cad_obj)}")
+        cad_objs = [cad_obj.wrapped]
 
     elif is_build123d_shape(cad_obj):
-        _debug(f"build123d Shape {grp_id}: {type(cad_obj)}")
+        _debug(f"        conv: build123d Shape {type(cad_obj)}")
         cad_objs = get_downcasted_shape(cad_obj.wrapped)
 
     elif is_cadquery_sketch(cad_obj):
+        _debug("        conv: cadquery sketch")
         cad_objs = conv_sketch(cad_obj)
 
     elif is_cadquery(cad_obj):
+        _debug("        conv: cadquery")
         cad_objs = []
         for v in cad_obj.vals():
             if is_cadquery_sketch(v):
                 obj = conv_sketch(v)
 
             elif is_vector(v):
                 obj = [vertex(v.wrapped)]
 
             else:
                 obj = [v.wrapped]
 
             cad_objs.extend(obj)
 
     elif is_wrapped(cad_obj):
+        _debug("        conv: wrapped object")
         if is_vector(cad_obj):
             cad_objs = [vertex(cad_obj.wrapped)]
         else:
             cad_objs = [cad_obj.wrapped]
 
     elif isinstance(cad_obj, Iterable):
+        _debug("        conv: iterable")
         objs = list(cad_obj)
         if len(objs) > 0 and is_wrapped(objs[0]):
             # ShapeList
-            _debug(f"build123d ShapeList {grp_id}: {type(cad_obj)}")
+            _debug(f"        conv: build123d ShapeList {type(cad_obj)}")
             cad_objs = [downcast(obj.wrapped) for obj in objs]
         else:
             raise ValueError("Empty list cannot be tessellated")
 
     elif is_topods_compound(cad_obj):
-        _debug(f"CAD Obj {grp_id}: TopoDS Compound")
+        _debug(f"        conv: CAD Obj TopoDS Compound")
 
         # Get the highest level shape
         cad_objs = [cad_obj]
 
     elif is_topods_shape(cad_obj):
-        _debug(f"CAD Obj {grp_id}: TopoDS Shape")
+        _debug(f"        conv: CAD Obj TopoDS Shape")
         cad_objs = [downcast(cad_obj)]
 
     else:
         raise RuntimeError(f"Cannot transform {cad_objs}({type(cad_objs)}) to OCP")
 
+    if is_compound_list(cad_objs):
+        cad_objs = get_downcasted_shape(cad_objs[0])
+
     # Convert to PartGroup
 
     if is_solid_list(cad_objs):
-        name = f"{obj_name if obj_name is not None else 'Solid'}_{grp_id}"
+        _debug("          conv: solid_list")
         return OCP_Part(
             cad_objs,
-            name=name,
+            name=get_name(obj_name, cad_objs, "Solid", "Solids"),
             color=get_rgba(obj_color, obj_alpha, Color(default_color)),
         )
 
     elif is_face_list(cad_objs):
-        name = f"{obj_name if obj_name is not None else 'Face'}_{grp_id}"
+        _debug("          conv: face_list")
         return OCP_Faces(
-            cad_objs, name=name, color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR))
+            cad_objs,
+            name=get_name(obj_name, cad_objs, "Face", "Faces"),
+            color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR)),
         )
 
     elif is_wire_list(cad_objs):
+        _debug("          conv: wire_list")
         edges = []
         for wire in cad_objs:
             edges.extend(get_edges(wire))
 
-        name = f"{obj_name if obj_name is not None else 'Wire'}_{grp_id}"
         return OCP_Edges(
             edges,
-            name=name,
+            name=get_name(obj_name, cad_objs, "Wire", "Wires"),
             color=get_rgba(obj_color, 1.0, Color(THICK_EDGE_COLOR)),
             width=2,
         )
 
     elif is_edge_list(cad_objs):
-        name = f"{obj_name if obj_name is not None else 'Edge'}_{grp_id}"
+        _debug("          conv: edge_list")
         return OCP_Edges(
             cad_objs,
-            name=name,
+            name=get_name(obj_name, cad_objs, "Edge", "Edges"),
             color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
             width=2,
         )
 
     elif is_vertex_list(cad_objs):
-        name = f"{obj_name if obj_name is not None else 'Vertex'}_{grp_id}"
+        _debug("          conv: vertex_list")
         return OCP_Vertices(
             cad_objs,
-            name=name,
+            name=get_name(obj_name, cad_objs, "Vertex", "Vertices"),
             color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
             size=6,
         )
-    elif is_compound_list(cad_objs):
-        obj_list = get_downcasted_shape(cad_objs[0])
-        if is_solid_list(obj_list):
-            name = f"{obj_name if obj_name is not None else 'Solids'}_{grp_id}"
-            return OCP_Part(
-                cad_objs,  # use compound
-                name=name,
-                color=get_rgba(obj_color, obj_alpha, Color(default_color)),
-            )
-        elif is_face_list(obj_list):
-            name = f"{obj_name if obj_name is not None else 'Faces'}_{grp_id}"
-            return OCP_Faces(
-                cad_objs,  # use compound
-                name=name,
-                color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR)),
-            )
-
-        elif is_edge_list(obj_list) or is_wire_list(obj_list):
-            if is_wire_list(obj_list):
-                edges = []
-                for wire in obj_list:
-                    edges.extend(get_edges(wire))
-                obj_list = edges
-
-            name = f"{obj_name if obj_name is not None else 'Edges'}_{grp_id}"
-            return OCP_Edges(
-                obj_list,  # use object list
-                name=name,
-                color=get_rgba(obj_color, 1.0, Color(THICK_EDGE_COLOR)),
-                width=2,
-            )
-
-        elif is_vertex_list(obj_list):
-            name = f"{obj_name if obj_name is not None else 'Vertices'}_{grp_id}"
-            return OCP_Vertices(
-                obj_list,  # use object list
-                name=name,
-                color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
-                size=6,
-            )
 
     else:
         raise RuntimeError(
             f"Cannot transform {cad_objs}, e.g. mixed Compounds not supported here?"
         )
 
 
-def get_instance(obj, grp_id, name, rgba, instances, progress):
+def get_instance(obj, name, rgba, instances, progress):
     is_instance = False
     part = None
 
+    obj, loc = relocate(obj)
+
     # check if the same instance is already available
     for i, ref in enumerate(instances):
         if ref[0] == get_tshape(obj):
             # create a referential OCP_Part
             part = OCP_Part(
                 {"ref": i},
-                f"{name}_{grp_id}",
+                name if name is not None else "Solid",
                 rgba,
             )
             # and stop the loop
             is_instance = True
 
             if progress is not None:
                 progress.update("-")
 
             break
 
     if not is_instance:
         # Transform the new instance to OCP
-        part = conv(obj, grp_id, name, rgba[:3], rgba[3])
+        part = conv(obj, name, rgba[:3], rgba[3])
         if not isinstance(part, OCP_PartGroup):
             # append the new instance
             instances.append((get_tshape(obj), part.shape[0]))
             # and create a referential OCP_Part
             part = OCP_Part(
                 {"ref": len(instances) - 1},
                 part.name,
                 rgba,
             )
 
+    part.loc = loc
+    part.loc_t = loc_to_tq(loc)
+
     return part
 
 
 def relocate(obj):
     loc = get_location(obj)
 
     if loc is None or not hasattr(obj, "wrapped"):
@@ -453,35 +415,44 @@
     tshape = get_tshape(obj)
     obj.wrapped.Move(loc.Inverted())
     obj.wrapped.TShape(tshape)
 
     return obj, loc
 
 
-def get_name(part, grp_id):
-    return f"{GROUP_NAME_LUT.get(part.__class__.__name__, 'Part')}_{grp_id}"
+def get_object_name(part):
+    return GROUP_NAME_LUT.get(part.__class__.__name__, "Part")
+
+
+def get_name(name, obj, singular, plural):
+    if name is not None:
+        return name
+    return plural if len(obj) > 1 else singular
 
 
 def _to_assembly(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     render_mates=None,
+    render_joints=None,
     mate_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
-    grp_id=0,
     mates=None,
     instances=None,
     progress=None,
+    is_assembly=False,
 ):
     if names is None:
         names = [None] * len(cad_objs)
+    else:
+        names = make_unique(names)
 
     if colors is None:
         colors = [None] * len(cad_objs)
 
     if alphas is None:
         alphas = [None] * len(cad_objs)
 
@@ -489,17 +460,15 @@
         default_color = (
             get_default("default_color") if default_color is None else default_color
         )
 
     if instances is None:
         instances = []
 
-    pg = OCP_PartGroup([], f"Group_{grp_id}", identity_location())
-
-    rename_top = True
+    pg = OCP_PartGroup([], "Group", identity_location())
 
     for obj_name, obj_color, obj_alpha, cad_obj in zip(names, colors, alphas, cad_objs):
         #
         # Retrieve the provided color or get default color
         # OCP_Faces, OCP_edges and OCP_Vertices bring their own color info
         # TODO default color for shapes is used
         #
@@ -509,50 +478,63 @@
                 *color, alpha = get_rgba(cad_obj.color, obj_alpha, Color(default_color))
             else:
                 color, alpha = obj_color, obj_alpha
             rgba = get_rgba(color, alpha, Color(default_color))
         else:
             color, alpha = None, None
 
+        if obj_name is None:
+            if (
+                hasattr(cad_obj, "label")
+                and cad_obj.label is not None
+                and cad_obj.label != ""
+            ):
+                obj_name = cad_obj.label
+            elif (
+                hasattr(cad_obj, "name")
+                and cad_obj.name is not None
+                and cad_obj.name != ""
+            ):
+                obj_name = cad_obj.name
+
         if is_cadquery_assembly(cad_obj):
+            _debug("to_assembly: cadquery assembly", obj_name)
+
             #
             # Iterate over CadQuery Assembly
             #
-            rename_top = False  # CadQuery assembly names are unique in one hierarchy
+            is_assembly = True
 
             pg.name = cad_obj.name
             pg.loc = get_location(cad_obj, as_none=False)
 
             if cad_obj.obj is not None:
                 # Get an existing instance id or tessellate this object
 
                 if is_cadquery_massembly(cad_obj):
                     # get_instance fails for MAssemblies when a mate is not at the
                     # shape origin after relocation, see hexapod "top" object
                     # workaround: do not handle TShapes
-                    part = conv(cad_obj.obj, grp_id, cad_obj.name, color, alpha)
+                    part = conv(cad_obj.obj, cad_obj.name, color, alpha)
                 else:
-                    part = get_instance(
-                        cad_obj.obj, grp_id, pg.name, rgba, instances, progress
-                    )
+                    part = get_instance(cad_obj.obj, pg.name, rgba, instances, progress)
                 pg.add(part)
 
             # render mates
             top_level_mates = None
             if render_mates and hasattr(cad_obj, "mates") and cad_obj.mates is not None:
                 top_level_mates = cad_obj.mates if mates is None else mates
 
                 # create a new part group for mates
                 pg2 = OCP_PartGroup(
                     [
                         CoordSystem(
                             name,
                             get_tuple(mate_def.mate.origin),
                             get_tuple(mate_def.mate.x_dir),
-                            get_tuple(mate_def.mate.y_dir),
                             get_tuple(mate_def.mate.z_dir),
                             mate_scale,
                         )
                         for name, mate_def in top_level_mates.items()
                         if mate_def.assembly == cad_obj
                     ],
                     name="mates",
@@ -561,198 +543,321 @@
 
                 # add mates partgroup
                 if pg2.objects:
                     pg.add(pg2)
 
             # iterate recursively over all children
             for child in cad_obj.children:
-                part, instances, grp_id = _to_assembly(
+                part, instances = _to_assembly(
                     child,
                     loc=loc,
-                    grp_id=grp_id,
                     default_color=default_color,
                     names=[obj_name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     mates=top_level_mates,
                     render_mates=render_mates,
+                    render_joints=render_joints,
                     mate_scale=mate_scale,
                     instances=instances,
                     progress=progress,
+                    is_assembly=is_assembly,
                 )
                 pg.add(part)
 
-        elif is_compound(cad_obj):
+        elif is_cadquery_sketch(cad_obj):
+            _debug("to_assembly: cadquery sketch", obj_name)
             #
-            # Iterate over Compound (includes build123d assemblies)
+            # Special treatment for cadquery sketches
             #
 
-            # use the build123d label info as name if exists
-            if (
-                hasattr(cad_obj, "label")
-                and cad_obj.label is not None
-                and cad_obj.label != ""
-            ):
-                pg.name = cad_obj.label
+            for child in conv_sketch(cad_obj):
+                part, instances = _to_assembly(
+                    child,
+                    default_color=default_color,
+                    names=[obj_name],
+                    colors=[obj_color],
+                    alphas=[obj_alpha],
+                    render_mates=render_mates,
+                    render_joints=render_joints,
+                    mate_scale=mate_scale,
+                    instances=instances,
+                    progress=progress,
+                )
+                if len(part.objects) == 1:
+                    pg.add(part.objects[0])
+                else:
+                    pg.add(part)
 
-            done = False
-            if not isinstance(cad_obj, Iterable):
-                # For non iterable compounds transform obj to OCP
-                part = conv(cad_obj, grp_id, obj_name, color, alpha)
-                # if obj_name is not given, get the name for the OCP_* type
-                if obj_name is None:
-                    part.name = get_name(part, grp_id)
-                pg.add(part)
-                done = True
+        # if Iterable but not a Compound and not a ShapeList
+        elif (
+            isinstance(cad_obj, Iterable)
+            and not hasattr(cad_obj, "wrapped")
+            and not hasattr(cad_obj, "first")
+            and not hasattr(cad_obj, "last")
+        ):
+            _debug(
+                "to_assembly: iterables other then Compounds and ShapeLists", obj_name
+            )
+
+            for child in cad_obj:
+                part, instances = _to_assembly(
+                    child,
+                    default_color=default_color,
+                    names=None,
+                    colors=[obj_color],
+                    alphas=[obj_alpha],
+                    render_mates=render_mates,
+                    render_joints=render_joints,
+                    mate_scale=mate_scale,
+                    instances=instances,
+                    progress=progress,
+                    is_assembly=is_assembly,
+                )
+                if isinstance(part, OCP_PartGroup) and len(part.objects) == 1:
+                    pg.add(part.objects[0])
+                else:
+                    pg.add(part)
+
+        elif is_compound(cad_obj):
+            _debug("to_assembly: compound")
+
+            #
+            # Iterate over Compound (includes build123d assemblies)
+            #
 
-            elif is_build123d_assembly(cad_obj):
-                # There is no top level shape, hence only get childern
-                children = cad_obj.children
-                for child in children:
-                    part, instances, grp_id = _to_assembly(
+            if is_build123d_assembly(cad_obj):
+                _debug("  to_assembly: build123d assembly", obj_name)
+                # There is no top level shape, hence only get children
+                is_assembly = True
+                name = "Assembly" if obj_name is None else obj_name
+                pg2 = OCP_PartGroup([], name, get_location(cad_obj, as_none=False))
+                for child in cad_obj.children:
+                    part, instances = _to_assembly(
                         child,
-                        grp_id=grp_id,
                         default_color=default_color,
-                        names=[obj_name],
+                        names=None,
                         colors=[obj_color],
                         alphas=[obj_alpha],
                         render_mates=render_mates,
+                        render_joints=render_joints,
                         mate_scale=mate_scale,
                         instances=instances,
                         progress=progress,
+                        is_assembly=is_assembly,
                     )
+                    if len(part.objects) == 1:
+                        if part.objects[0].loc is None:
+                            part.objects[0].loc = part.loc
+                        else:
+                            part.objects[0].loc = part.loc * part.objects[0].loc
+                        pg2.add(part.objects[0])
+                    else:
+                        pg2.add(part)
+
+                pg.add(pg2)
+
+            elif is_mixed_compound(cad_obj):
+                _debug("  to_assembly: mixed compound", obj_name)
+                for child in cad_obj:
+                    part = conv(child.wrapped, obj_name, color, alpha)
                     pg.add(part)
 
             else:
-                part = conv(cad_obj.wrapped, grp_id, obj_name, color, alpha)
-                pg.add(part)
+                _debug("  to_assembly: generic case", obj_name)
+                if hasattr(cad_obj, "_dim") and cad_obj._dim == 3:
+                    if not isinstance(cad_obj, Iterable):
+                        _debug("    to_assembly: no iterable", obj_name)
+                        part = get_instance(
+                            cad_obj, obj_name, rgba, instances, progress
+                        )
 
-        elif is_cadquery_sketch(cad_obj):
-            #
-            # Special treatment for cadquery sketches
-            #
+                    elif isinstance(cad_obj, Iterable) and len(cad_obj.solids()) == 1:
+                        _debug("    to_assembly: single solid", obj_name)
+                        part = get_instance(
+                            cad_obj.solids()[0], obj_name, rgba, instances, progress
+                        )
+
+                    else:
+                        _debug("    to_assembly: no iterable", obj_name)
+                        part = conv(cad_obj.wrapped, obj_name, color, alpha)
+
+                else:
+                    _debug("    to_assembly: everything else", obj_name)
+                    part = conv(cad_obj.wrapped, obj_name, color, alpha)
+
+                if is_assembly and obj_name is not None:
+                    part.name = f"{obj_name}"
 
-            for child in conv_sketch(cad_obj):
-                part, instances, grp_id = _to_assembly(
-                    child,
-                    grp_id=grp_id,
-                    default_color=default_color,
-                    names=[obj_name],
-                    colors=[obj_color],
-                    alphas=[obj_alpha],
-                    render_mates=render_mates,
-                    mate_scale=mate_scale,
-                    instances=instances,
-                    progress=progress,
-                )
                 pg.add(part)
 
+                if (
+                    render_joints
+                    and hasattr(cad_obj, "joints")
+                    and len(cad_obj.joints) > 0
+                ):
+                    _debug("    to_assembly: joints")
+                    pg.name = obj_name
+                    part.name = "shape"
+                    # create a new part group for mates
+                    pg2 = OCP_PartGroup(
+                        [
+                            conv(joint.symbol.wrapped, name)
+                            for name, joint in cad_obj.joints.items()
+                            if hasattr(joint, "symbol")
+                        ],
+                        name="joints",
+                        loc=identity_location(),  # mates inherit the parent location, so actually add a no-op
+                    )
+
+                    # add mates partgroup
+                    if pg2.objects:
+                        pg.add(pg2)
+
         else:
+            _debug("to_assembly: generic case", obj_name)
             #
             # Render non iterable objects
             #
 
             # cad_obj.wrapped and cad_obj.obj.wrapped behave the same way
             if hasattr(cad_obj, "obj"):
                 cad_obj = cad_obj.obj
 
-            # Use the objects label as obj_name (build123d)
-            if hasattr(cad_obj, "label") and cad_obj.label != "":
-                obj_name = cad_obj.label
-
-            # or its name attribute (cadquery)
-            if hasattr(cad_obj, "name") and cad_obj.name != "":
-                obj_name = cad_obj.name
-
             is_solid = False
 
             if hasattr(cad_obj, "wrapped") and not is_vector(cad_obj):
                 solids = get_downcasted_shape(cad_obj.wrapped)
-                # TODO: what to do with mixed compounds
                 is_solid = all([is_topods_solid(solid) for solid in solids])
 
             # TODO Fix parent
             parent = None
-            if show_parent and hasattr(cad_obj, "parent"):
-                parent = cad_obj.parent
-
-            if parent is not None:
-                pg.add(conv(parent, grp_id, "parent", None, None))
-                pg.objects[0].state_faces = 0
+            if show_parent:
+                if hasattr(cad_obj, "parent"):
+                    parent = cad_obj.parent
+                    topo = False
+                elif hasattr(cad_obj, "topo_parent"):
+                    parent = cad_obj.topo_parent
+                    topo = True
+                elif (
+                    isinstance(cad_obj, Iterable)
+                    and len(cad_obj) > 0
+                    and hasattr(cad_obj[0], "topo_parent")
+                ):
+                    parent = cad_obj[0].topo_parent
+                    topo = True
+
+            ind = 0
+            parents = []
+            while parent is not None:
+                pname = "parent" if ind == 0 else f"parent({ind})"
+                parents.insert(0, conv(parent, pname, None, None))
+                parent = parent.topo_parent if topo else None
+                ind -= 1
+
+            for p in parents:
+                pg.add(p)
+                pg.objects[-1].state_faces = 0
 
             if is_solid:
-                # Split solids into a solid at the XY plane origin and the location
-                cad_obj, loc = relocate(cad_obj)
-                # create a partgroup and move part location into it
-                pg2 = OCP_PartGroup([], name=f"Group_{grp_id}", loc=loc)
-
                 # transform the solid to OCP
-                part = get_instance(
-                    cad_obj, grp_id, obj_name, rgba, instances, progress
-                )
-
+                part = get_instance(cad_obj, obj_name, rgba, instances, progress)
                 if obj_name is None:
-                    part.name = get_name(part, grp_id)
-                # change part's location to identity, since location is in partgroup
-                pg.loc = identity_location()
+                    part.name = get_object_name(part)
 
-                pg2.add(part)
+                pg.add(part)
 
-                if len(pg2.objects) == 1:
-                    pg2.name = pg2.objects[0].name
+            elif isinstance(cad_obj, OCP_PartGroup):
+                pg = cad_obj
 
-                # add additional partgroup
-                pg.add(pg2)
+            elif isinstance(cad_obj, (OCP_Faces, OCP_Edges, OCP_Vertices)):
+                pg.add(cad_obj)
 
             else:
-                part = conv(cad_obj, grp_id, obj_name, color, alpha)
-                if obj_name is None:
-                    part.name = get_name(part, grp_id)
+                part = conv(cad_obj, obj_name, color, alpha)
+                if part.name is None:
+                    part.name = get_object_name(part)
                 pg.add(part)  # no clear way to relocated
 
-            grp_id += 1
-
         if pg.loc is None:
-            raise RuntimeError("location is None")
-            # pg.loc = identity_location()
-
-    if len(pg.objects) == 1 and isinstance(pg.objects[0], OCP_PartGroup):
-        pg = pg.objects[0]
+            pg.loc = identity_location()
 
-    if len(pg.objects) == 1 and rename_top:
-        pg.name = pg.objects[0].name
+    names = make_unique([obj.name for obj in pg.objects])
+    for name, obj in zip(names, pg.objects):
+        obj.name = name
 
-    return pg, instances, grp_id
+    return pg, instances
 
 
 def to_assembly(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     render_mates=None,
+    render_joints=None,
     mate_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
-    grp_id=0,
     mates=None,
     instances=None,
     progress=None,
 ):
-    pg, instances, _ = _to_assembly(
+    pg, instances = _to_assembly(
         *cad_objs,
         names=names,
         colors=colors,
         alphas=alphas,
         render_mates=render_mates,
+        render_joints=render_joints,
         mate_scale=mate_scale,
         default_color=default_color,
         show_parent=show_parent,
         loc=loc,
-        grp_id=grp_id,
         mates=mates,
         instances=instances,
         progress=progress,
     )
+
+    if len(pg.objects) == 1 and isinstance(pg.objects[0], OCP_PartGroup):
+        if pg.objects[0].loc is None:
+            pg.objects[0].loc = pg.loc
+        elif pg.loc is not None:
+            pg.objects[0].loc = pg.loc * pg.objects[0].loc
+        pg = pg.objects[0]
+
     set_instances([instance[1] for instance in instances])
     return pg
+
+
+def export_three_cad_viewer_json(obj, filename=None):
+    def decode(instances, shapes):
+        def walk(obj):
+            typ = None
+            for attr in obj.keys():
+                if attr == "parts":
+                    for part in obj["parts"]:
+                        walk(part)
+
+                elif attr == "type":
+                    typ = obj["type"]
+
+                elif attr == "shape":
+                    if typ == "shapes":
+                        if obj["shape"].get("ref") is not None:
+                            ind = obj["shape"]["ref"]
+                            obj["shape"] = instances[ind]
+
+        walk(shapes)
+
+    part_group = to_assembly(obj)
+    instances, shapes, states = tessellate_group(part_group)
+    decode(instances, shapes)
+
+    j = numpy_to_json([shapes, states])
+    if filename is None:
+        return j
+    else:
+        with open(filename, "w") as fd:
+            fd.write(j)
+        return json.dumps({"exported": filename})
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/defaults.py` & `ocp_tessellate-1.0.1/ocp_tessellate/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         - edge_accuracy:      Edges: Precision of edge discretization (default=None, i.e. mesh quality / 100)
         - default_color:      Default face color (default=(232, 176, 36))
         - default_edgecolor:  Default edge color (default="#707070")
         - optimal_bb:         Use optimal bounding box (default=False)
         - render_normals:     Render vertex normals(default=False)
         - render_edges:       Render edges  (default=True)
         - render_mates:       Render mates (for MAssemblies, default=False)
+        - render_joints:      Render build12d joints (default=False)
         - mate_scale:         Scale of rendered mates (for MAssemblies, default=1)
 
         VIEWER OPTIONS
         - control:            Use trackball controls ('trackball') or orbit controls ('orbit') (default='trackball')
         - up:                 Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (or 'L' for legacy z-axis up mode)
         - axes:               Show axes (default=False)
         - axes0:              Show axes at (0,0,0) (default=False)
@@ -116,18 +117,20 @@
             # render options
             #
             "angular_tolerance": 0.2,
             "deviation": 0.1,
             "edge_accuracy": None,
             "default_color": (232, 176, 36),
             "default_edgecolor": "#707070",
+            "default_opacity": 0.5,
             "optimal_bb": False,
             "render_normals": False,
             "render_edges": True,
             "render_mates": False,
+            "render_joints": False,
             "parallel": False,
             "mate_scale": 1,
             #
             # viewer options
             #
             "control": "trackball",
             "up": "Z",
@@ -277,14 +280,15 @@
             "edge_accuracy",
             "default_color",
             "default_edgecolor",
             "optimal_bb",
             "render_normals",
             "render_edges",
             "render_mates",
+            "render_joints",
             "mate_scale",
             "quality",
             "parallel",
         ]
     }
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.0.1/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.0.1/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.0.1/ocp_tessellate/ocp_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -561,17 +561,19 @@
 def is_topods_edge(topods_shape):
     return isinstance(topods_shape, TopoDS_Edge)
 
 
 def is_topods_vertex(topods_shape):
     return isinstance(topods_shape, TopoDS_Vertex)
 
+
 def is_compound_list(topods_list):
     return all([is_topods_compound(obj) for obj in topods_list])
 
+
 def is_solid_list(topods_list):
     return all([is_topods_solid(obj) for obj in topods_list])
 
 
 def is_face_list(topods_list):
     return all([is_topods_face(obj) for obj in topods_list])
 
@@ -588,14 +590,31 @@
     return all([is_topods_vertex(obj) for obj in topods_list])
 
 
 def is_compound(obj):
     return hasattr(obj, "wrapped") and is_topods_compound(obj.wrapped)
 
 
+def unroll_compound(compound):
+    result = []
+    for o in compound:
+        if is_compound(o):
+            result.extend(unroll_compound(o))
+        else:
+            result.extend(get_downcasted_shape(o.wrapped))
+    return result
+
+
+def is_mixed_compound(compound):
+    if not isinstance(compound, Iterable):
+        return False
+    u_compound = unroll_compound(compound)
+    return len(set([o.__class__.__name__ for o in u_compound])) > 1
+
+
 # Check compounds for containing same types only
 
 
 # def is_solids_compound(topods_shape):
 #     if isinstance(topods_shape, TopoDS_Compound):
 #         e = get_solids(topods_shape)
 #         return next(e, None) is not None
@@ -686,14 +705,21 @@
     return downcast(BRepBuilderAPI_MakeVertex(gp_Pnt(x, y, z)).Vertex())
 
 
 def line(start, end):
     return downcast(BRepBuilderAPI_MakeEdge(gp_Pnt(*start), gp_Pnt(*end)).Edge())
 
 
+def cross(v1, v2):
+    x = gp_Vec(*v1).Normalized()
+    z = gp_Vec(*v2).Normalized()
+    y = x.Crossed(z).Normalized()
+    return (y.X(), y.Y(), y.Z())
+
+
 def tq_to_loc(t, q):
     T = gp_Trsf()
     Q = gp_Quaternion(*q)
     V = gp_Vec(*t)
     T.SetTransformation(Q, V)
     return TopLoc_Location(T)
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.0.1/ocp_tessellate/tessellator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     elif isinstance(obj, np.ndarray):
         size += obj.size * obj.dtype.itemsize
     elif isinstance(obj, (tuple, list)):
         size += sum([get_size(i) for i in obj])
     return size
 
 
-cache_size = os.environ.get("JCQ_CACHE_SIZE_MB")
+cache_size = os.environ.get("OCP_CACHE_SIZE_MB")
 if cache_size is None:
     cache_size = 128 * 1024 * 1024
 else:
     cache_size = int(cache_size) * 1024 * 1024
 cache = LRUCache(maxsize=cache_size, getsizeof=get_size)
 
 
@@ -339,15 +339,15 @@
         "edges": tess.get_edges(),
     }
 
 
 def discretize_edge(edge, deflection=0.1, num=None):
     curve_adaptator = BRepAdaptor_Curve(edge)
 
-    if num is not None:
+    if num is not None and num > 1:
         discretizer = GCPnts_QuasiUniformAbscissa()
         discretizer.Initialize(curve_adaptator, num)
     else:
         discretizer = GCPnts_QuasiUniformDeflection()
         discretizer.Initialize(
             curve_adaptator,
             deflection,
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate/utils.py` & `ocp_tessellate-1.0.1/ocp_tessellate/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -208,7 +208,20 @@
 
     warn_format = warnings.formatwarning
     warnings.formatwarning = warning_on_one_line
     warnings.simplefilter(when, warning)
     warnings.warn(message + "\n", warning)
     warnings.formatwarning = warn_format
     warnings.simplefilter("ignore", warning)
+
+
+def make_unique(names):
+    found = {}
+    unique_names = []
+    for name in names:
+        if found.get(name) is None:
+            found[name] = 1
+            unique_names.append(name)
+        else:
+            found[name] += 1
+            unique_names.append(f"{name}({found[name]})")
+    return unique_names
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.0.1/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.0.0rc9
+Version: 1.0.1
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.0.1/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ocp_tessellate/_version.py
 ocp_tessellate/cad_objects.py
 ocp_tessellate/convert.py
 ocp_tessellate/defaults.py
 ocp_tessellate/mp_tess.py
 ocp_tessellate/mp_tessellator.py
 ocp_tessellate/ocp_utils.py
+ocp_tessellate/stepreader.py
 ocp_tessellate/tessellator.py
 ocp_tessellate/utils.py
 ocp_tessellate.egg-info/PKG-INFO
 ocp_tessellate.egg-info/SOURCES.txt
 ocp_tessellate.egg-info/dependency_links.txt
 ocp_tessellate.egg-info/not-zip-safe
 ocp_tessellate.egg-info/requires.txt
```

### Comparing `ocp_tessellate-1.0.0rc9/setup.cfg` & `ocp_tessellate-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0rc9
+current_version = 1.0.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.0rc9/setup.py` & `ocp_tessellate-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.0rc9",
+    "version": "1.0.1",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
         "numpy-quaternion",
         "cachetools~=5.2.0",
-        "cadquery_ocp>=7.6.3a0,<7.8",
+        # "cadquery_ocp>=7.6.3a0,<7.8",
     ],
     "extras_require": {
         "dev": {"twine", "bumpversion", "black", "pylint", "pyYaml"},
     },
     "packages": find_packages(),
     "zip_safe": False,
     "author": "Bernhard Walter",
```

