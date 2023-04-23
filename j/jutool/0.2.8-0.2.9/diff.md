# Comparing `tmp/jutool-0.2.8-py3-none-any.whl.zip` & `tmp/jutool-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 64308 bytes, number of entries: 62
+Zip file size: 64372 bytes, number of entries: 62
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 08:16 code_util/__init__.py
 -rw-r--r--  2.0 unx     5797 b- defN 23-Feb-13 08:16 code_util/apidoc_generation.py
 -rw-r--r--  2.0 unx     3314 b- defN 23-Feb-13 08:16 code_util/buffer.py
 -rw-r--r--  2.0 unx     1843 b- defN 23-Feb-13 08:16 code_util/env.py
 -rw-r--r--  2.0 unx     2080 b- defN 23-Mar-29 09:48 code_util/file.py
 -rw-r--r--  2.0 unx     5107 b- defN 23-Feb-13 08:16 code_util/log.py
--rw-r--r--  2.0 unx     8813 b- defN 23-Mar-29 10:11 code_util/markdown.py
+-rw-r--r--  2.0 unx     9082 b- defN 23-Apr-21 07:34 code_util/markdown.py
 -rw-r--r--  2.0 unx       49 b- defN 23-Feb-13 08:16 code_util/num.py
 -rw-r--r--  2.0 unx      294 b- defN 23-Feb-13 08:16 code_util/plot.py
 -rw-r--r--  2.0 unx      720 b- defN 23-Feb-13 08:16 code_util/setup.py
 -rw-r--r--  2.0 unx      806 b- defN 23-Feb-13 08:16 code_util/str_adv.py
 -rw-r--r--  2.0 unx     3356 b- defN 23-Feb-13 08:16 code_util/structures.py
 -rw-r--r--  2.0 unx    17977 b- defN 23-Apr-10 07:03 ml2_util/MLModel.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 08:16 ml2_util/__init__.py
@@ -52,13 +52,13 @@
 -rw-r--r--  2.0 unx      885 b- defN 23-Feb-13 08:16 sample_util/SampleSet_import.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 08:16 sample_util/__init__.py
 -rw-r--r--  2.0 unx     1212 b- defN 23-Feb-13 08:16 sample_util/samples_lib.py
 -rw-r--r--  2.0 unx      774 b- defN 23-Mar-23 06:56 sample_util/setup.py
 -rw-r--r--  2.0 unx     9055 b- defN 23-Feb-13 08:16 spider_util/WebGetter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 08:16 spider_util/__init__.py
 -rw-r--r--  2.0 unx      750 b- defN 23-Feb-13 08:16 spider_util/setup.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Apr-10 08:29 jutool-0.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    37623 b- defN 23-Apr-10 08:29 jutool-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 08:29 jutool-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Apr-10 08:29 jutool-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5126 b- defN 23-Apr-10 08:29 jutool-0.2.8.dist-info/RECORD
-62 files, 205870 bytes uncompressed, 56176 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx     1062 b- defN 23-Apr-21 07:34 jutool-0.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    37623 b- defN 23-Apr-21 07:34 jutool-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 07:34 jutool-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Apr-21 07:34 jutool-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5126 b- defN 23-Apr-21 07:34 jutool-0.2.9.dist-info/RECORD
+62 files, 206139 bytes uncompressed, 56240 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -165,23 +165,23 @@
 
 Filename: spider_util/__init__.py
 Comment: 
 
 Filename: spider_util/setup.py
 Comment: 
 
-Filename: jutool-0.2.8.dist-info/LICENSE
+Filename: jutool-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: jutool-0.2.8.dist-info/METADATA
+Filename: jutool-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: jutool-0.2.8.dist-info/WHEEL
+Filename: jutool-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: jutool-0.2.8.dist-info/top_level.txt
+Filename: jutool-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jutool-0.2.8.dist-info/RECORD
+Filename: jutool-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_util/markdown.py

```diff
@@ -75,29 +75,37 @@
         self.nodes = []
         self.node_color = {}
         self.node_shape = {}
         self.lines = []
         self.oriented = "LR" if oriented_left2right else "TD"
         self.node_navigate = {}
         self.node_icon = {}
+        self.id_mapping = {}
 
     def add_node(self, name, id, anchor_title=None, icon=None):
+        if id not in self.id_mapping:
+            self.id_mapping[id] = f"id_{len(self.id_mapping)}"
+        id = self.id_mapping[id]
+
         self.nodes.append((id, name, None))
         if anchor_title is not None:
             self.node_navigate[id] = anchor_title
         if icon is not None:
             self.node_icon[id] = icon
 
     def set_node_color(self, id, color: flowchart_color_enum):
-        self.node_color[id] = color
+        self.node_color[self.id_mapping[id]] = color
 
     def set_node_shape(self, id, shape: flowchart_shape_enum):
-        self.node_shape[id] = shape
+        self.node_shape[self.id_mapping[id]] = shape
 
     def add_line(self, id1, id2, message=None, dot_line=False):
+        id1 = self.id_mapping[id1]
+        id2 = self.id_mapping[id2]
+
         self.lines.append((id1, id2, message, dot_line))
 
 
 class draw_markdownobj_gantt(draw_markdownobj):
     def __init__(self, gantt_title, date_format='YYYY-MM-DD'):
         self.Items = {}
         self.Title = gantt_title
```

## Comparing `jutool-0.2.8.dist-info/LICENSE` & `jutool-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jutool-0.2.8.dist-info/METADATA` & `jutool-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jutool
-Version: 0.2.8
+Version: 0.2.9
 Summary: Some base methods for developing
 Home-page: http://www.example.com/~cschultz/bvote/
 Author: Ke
 Author-email: jiangke1207@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `jutool-0.2.8.dist-info/RECORD` & `jutool-0.2.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 code_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 code_util/apidoc_generation.py,sha256=BQ359EcsQHOp2xTr8thv5_Z3JmvxjlFpUTe8VnD4ipI,5797
 code_util/buffer.py,sha256=wMxVlj7VSJVTBMMVT07RNSdxBNX30hVxhP6jzOuAa9c,3314
 code_util/env.py,sha256=pMEs2qP-xb8Rc05a6Q42essvPAhY1BDNJYeMS50rrIw,1843
 code_util/file.py,sha256=k4F2iXtY50UaJJzwGKhgEIwRi6aPzepHEcJoPio_wik,2080
 code_util/log.py,sha256=2nCkG4EhclpsYsCwquhQrilpo9hTtq3WkqD4xfUfKcE,5107
-code_util/markdown.py,sha256=o7avZGH_9nkYGEQxwq1mgapmCMh8QxjukVh4SDHU5U0,8813
+code_util/markdown.py,sha256=a1vqJAczCmtyx8_BvMK37-74c6pAInLWjmPU-V4vkcU,9082
 code_util/num.py,sha256=u2jSN-x_LnF8MrS_YVrIcPMn3iF2cuwifrBWu3YO_es,49
 code_util/plot.py,sha256=U9gaiVpId6iisHoFnK4jNXPCVYg6LTYCJc0Cha_Ylfs,294
 code_util/setup.py,sha256=MhNBUQeImYcxVBv5NzNz7UF1btA-w-WpAkS--afV4iI,720
 code_util/str_adv.py,sha256=oXGSyI6defZA6P4rUwz0YYcAtEhhhGzJb8NEXj-OL1g,806
 code_util/structures.py,sha256=Q46FYfC4Tai1KxfmPgv35L0rGxIlvxvjJaG-jdX11ME,3356
 ml2_util/MLModel.py,sha256=mMWBMJ4R0DekvewQvu9kXbnoXZj0IOVBvTAs9PDMwQE,17977
 ml2_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -51,12 +51,12 @@
 sample_util/SampleSet_import.py,sha256=Lcfwa55oalIqs8GfNP0_7BMvPUp7xDZZOpidBF7E0x0,885
 sample_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sample_util/samples_lib.py,sha256=5pX9aVf84-HbqlDxo_BXMJLcMlfzfS-6dmcIFqy6dZ8,1212
 sample_util/setup.py,sha256=7Z-vmHtydUvPyo1FV_dXSWLuBMBunCzMZqBYE9URBJQ,774
 spider_util/WebGetter.py,sha256=bIhIcY_Z0Nc8Qh9dnK11GBpgNZugDsgWPywGWZJVr64,9055
 spider_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spider_util/setup.py,sha256=KpoqLZm4c2AVk3JgNW5mOkbuftgMemns6vMqGXMOlRM,750
-jutool-0.2.8.dist-info/LICENSE,sha256=RzIgj4q7MEKYv9nQW2BLmdUebEBGg8PuLPI1Mh4IxBE,1062
-jutool-0.2.8.dist-info/METADATA,sha256=JILUrcuVzjrCe_tZz2qDbm2qDn0SpYRtzWy0WkDQpVQ,37623
-jutool-0.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-jutool-0.2.8.dist-info/top_level.txt,sha256=vV13hbPptfbOECE7PljL6e7QcT8_sUkiM5og8osKNNI,60
-jutool-0.2.8.dist-info/RECORD,,
+jutool-0.2.9.dist-info/LICENSE,sha256=RzIgj4q7MEKYv9nQW2BLmdUebEBGg8PuLPI1Mh4IxBE,1062
+jutool-0.2.9.dist-info/METADATA,sha256=_D80oiAk56woqlDZiuTvV7AG-3xtDig2DiNKTcfFtiE,37623
+jutool-0.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+jutool-0.2.9.dist-info/top_level.txt,sha256=vV13hbPptfbOECE7PljL6e7QcT8_sUkiM5og8osKNNI,60
+jutool-0.2.9.dist-info/RECORD,,
```

