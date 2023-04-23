# Comparing `tmp/range-css-compiler-0.2.0.tar.gz` & `tmp/range-css-compiler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range-css-compiler-0.2.0.tar", last modified: Sat Apr  8 11:05:59 2023, max compression
+gzip compressed data, was "range-css-compiler-0.2.1.tar", last modified: Sun Apr 23 17:24:38 2023, max compression
```

## Comparing `range-css-compiler-0.2.0.tar` & `range-css-compiler-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 11:05:59.941022 range-css-compiler-0.2.0/
--rw-rw-rw-   0        0        0     7942 2023-04-08 11:05:59.941022 range-css-compiler-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6126 2023-01-29 05:44:29.000000 range-css-compiler-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 11:05:59.917141 range-css-compiler-0.2.0/range_css_compiler/
--rw-rw-rw-   0        0        0     3522 2023-01-29 09:57:10.000000 range-css-compiler-0.2.0/range_css_compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:05:59.940085 range-css-compiler-0.2.0/range_css_compiler/parts/
--rw-rw-rw-   0        0        0     1122 2023-01-21 06:56:04.000000 range-css-compiler-0.2.0/range_css_compiler/parts/gen_compiled_rcss.py
--rw-rw-rw-   0        0        0    27290 2023-04-08 11:04:58.000000 range-css-compiler-0.2.0/range_css_compiler/parts/pypi_tool_file_binder.py
--rw-rw-rw-   0        0        0     8153 2023-01-29 08:42:39.000000 range-css-compiler-0.2.0/range_css_compiler/parts/to_qp_mat_js.py
--rw-rw-rw-   0        0        0     8739 2023-01-14 05:33:36.000000 range-css-compiler-0.2.0/range_css_compiler/parts/yaml_style_to_equid.py
--rw-rw-rw-   0        0        0      434 2023-01-21 06:30:47.000000 range-css-compiler-0.2.0/range_css_compiler/test.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:05:59.921654 range-css-compiler-0.2.0/range_css_compiler.egg-info/
--rw-rw-rw-   0        0        0     7942 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-04-08 11:05:59.000000 range-css-compiler-0.2.0/range_css_compiler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 11:05:59.942042 range-css-compiler-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-04-08 11:05:55.000000 range-css-compiler-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.675748 range-css-compiler-0.2.1/
+-rw-rw-rw-   0        0        0     7942 2023-04-23 17:24:38.673226 range-css-compiler-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6126 2023-01-29 05:44:29.000000 range-css-compiler-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.640781 range-css-compiler-0.2.1/range_css_compiler/
+-rw-rw-rw-   0        0        0     3522 2023-01-29 09:57:10.000000 range-css-compiler-0.2.1/range_css_compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.673226 range-css-compiler-0.2.1/range_css_compiler/parts/
+-rw-rw-rw-   0        0        0     1122 2023-01-21 06:56:04.000000 range-css-compiler-0.2.1/range_css_compiler/parts/gen_compiled_rcss.py
+-rw-rw-rw-   0        0        0    27318 2023-04-23 17:23:47.000000 range-css-compiler-0.2.1/range_css_compiler/parts/pypi_tool_file_binder.py
+-rw-rw-rw-   0        0        0     8153 2023-01-29 08:42:39.000000 range-css-compiler-0.2.1/range_css_compiler/parts/to_qp_mat_js.py
+-rw-rw-rw-   0        0        0     8739 2023-01-14 05:33:36.000000 range-css-compiler-0.2.1/range_css_compiler/parts/yaml_style_to_equid.py
+-rw-rw-rw-   0        0        0      434 2023-01-21 06:30:47.000000 range-css-compiler-0.2.1/range_css_compiler/test.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.655498 range-css-compiler-0.2.1/range_css_compiler.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:24:38.675748 range-css-compiler-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-04-23 17:24:32.000000 range-css-compiler-0.2.1/setup.py
```

### Comparing `range-css-compiler-0.2.0/PKG-INFO` & `range-css-compiler-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-css-compiler
-Version: 0.2.0
+Version: 0.2.1
 Summary: More intuitive HTML placement and assignment tool than CSS.
 Home-page: https://github.co.jp/
 Author: le_lattelle
 Author-email: g.tiger.ml@gmail.com
 License: CC0 v1.0
 Description: # range-css-compiler
```

### Comparing `range-css-compiler-0.2.0/README.md` & `range-css-compiler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/range_css_compiler/__init__.py` & `range-css-compiler-0.2.1/range_css_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/range_css_compiler/parts/gen_compiled_rcss.py` & `range-css-compiler-0.2.1/range_css_compiler/parts/gen_compiled_rcss.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/range_css_compiler/parts/pypi_tool_file_binder.py` & `range-css-compiler-0.2.1/range_css_compiler/parts/pypi_tool_file_binder.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,18 @@
 
 // 1つの要素についてstyleを適用
 function apply_style_one_ele(one_ele_style){
     // 対象要素を見つける
     var target = document.getElementById(one_ele_style["css_id"]);
     // cssのスタイル適用
     target.style.position = "fixed";
-    target.style.left = one_ele_style["posX"];
-    target.style.top = one_ele_style["posY"];
-    target.style.width = one_ele_style["width"];
-    target.style.height = one_ele_style["height"];
+    target.style.left = one_ele_style["posX"] + "px";
+    target.style.top = one_ele_style["posY"] + "px";
+    target.style.width = one_ele_style["width"] + "px";
+    target.style.height = one_ele_style["height"] + "px";
 }
 
 // スタイル適用関数
 function apply_rcss_style(rcss_solved_style){
     for(one_ele_style of rcss_solved_style){
         if (one_ele_style["css_id"] == "rcss_frame") {continue;}
         // 1つの要素についてstyleを適用
```

### Comparing `range-css-compiler-0.2.0/range_css_compiler/parts/to_qp_mat_js.py` & `range-css-compiler-0.2.1/range_css_compiler/parts/to_qp_mat_js.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/range_css_compiler/parts/yaml_style_to_equid.py` & `range-css-compiler-0.2.1/range_css_compiler/parts/yaml_style_to_equid.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/range_css_compiler.egg-info/PKG-INFO` & `range-css-compiler-0.2.1/range_css_compiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-css-compiler
-Version: 0.2.0
+Version: 0.2.1
 Summary: More intuitive HTML placement and assignment tool than CSS.
 Home-page: https://github.co.jp/
 Author: le_lattelle
 Author-email: g.tiger.ml@gmail.com
 License: CC0 v1.0
 Description: # range-css-compiler
```

### Comparing `range-css-compiler-0.2.0/range_css_compiler.egg-info/SOURCES.txt` & `range-css-compiler-0.2.1/range_css_compiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.0/setup.py` & `range-css-compiler-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 公開用パッケージの作成 [ezpip]
 import ezpip
 
 # 公開用パッケージの作成 [ezpip]
 with ezpip.packager(develop_dir = "./_develop_range_css_compiler/") as p:
 	setup(
 		name = "range-css-compiler",
-		version = "0.2.0",
+		version = "0.2.1",
 		description = "More intuitive HTML placement and assignment tool than CSS.",
 		author = "le_lattelle",
 		author_email = "g.tiger.ml@gmail.com",
 		url = "https://github.co.jp/",
 		packages = p.packages,
 		install_requires = ["relpath", "ezpip", "sout", "fies", "tqdm", "equid", "indent-template", "ezptn"],
 		long_description = p.long_description,
```

