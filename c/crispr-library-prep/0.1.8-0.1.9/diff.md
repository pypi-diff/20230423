# Comparing `tmp/crispr_library_prep-0.1.8.tar.gz` & `tmp/crispr_library_prep-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_library_prep-0.1.8.tar", max compression
+gzip compressed data, was "crispr_library_prep-0.1.9.tar", max compression
```

## Comparing `crispr_library_prep-0.1.8.tar` & `crispr_library_prep-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       57 2023-04-19 13:40:06.389263 crispr_library_prep-0.1.8/crispr_library_prep/__init__.py
--rw-r--r--   0        0        0    21646 2023-04-21 16:23:45.302150 crispr_library_prep-0.1.8/crispr_library_prep/CrisprLibraryPrep.py
--rw-r--r--   0        0        0      529 2023-04-21 16:24:03.664225 crispr_library_prep-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.8/README.md
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.8/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-04-19 13:40:06.389263 crispr_library_prep-0.1.9/crispr_library_prep/__init__.py
+-rw-r--r--   0        0        0    21994 2023-04-21 17:54:10.958823 crispr_library_prep-0.1.9/crispr_library_prep/CrisprLibraryPrep.py
+-rw-r--r--   0        0        0      529 2023-04-21 17:56:45.510204 crispr_library_prep-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.9/README.md
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.9/setup.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.9/PKG-INFO
```

### Comparing `crispr_library_prep-0.1.8/crispr_library_prep/CrisprLibraryPrep.py` & `crispr_library_prep-0.1.9/crispr_library_prep/CrisprLibraryPrep.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,38 +287,43 @@
     result_series_list = []
     for result_dict in result_dict_list:
         
         target_coverage_suggested_list = []
         target_read_amount_suggested_list = []
         gDNA_for_target_coverage_list = []
         for suggested_target_coverage_amount in suggested_target_coverage_amounts:
+            max_gDNA_amount = result_dict["max_gDNA_target_coverage_suggested_result"][0]
             gDNA_for_target_coverage = result_dict["get_gDNA_for_suggested_target_coverage_callable"](suggested_target_coverage_amount)
+            if gDNA_for_target_coverage <= max_gDNA_amount:
+                target_coverage_result = result_dict["get_target_coverage_for_gDNA_callable"](gDNA_for_target_coverage)  
             
-            target_coverage_result = result_dict["get_target_coverage_for_gDNA_callable"](gDNA_for_target_coverage)  
-            
-            target_coverage_suggested = target_coverage_result["target_coverage_suggested"]
-            target_read_amount_suggested = target_coverage_result["target_read_amount_suggested"]
+                target_coverage_suggested = target_coverage_result["target_coverage_suggested"]
+                target_read_amount_suggested = target_coverage_result["target_read_amount_suggested"]
+            else:
+                gDNA_for_target_coverage = np.nan
+                target_coverage_suggested = np.nan
+                target_read_amount_suggested = np.nan
 
             target_coverage_suggested_list.append(target_coverage_suggested)
             target_read_amount_suggested_list.append(target_read_amount_suggested)
             gDNA_for_target_coverage_list.append(gDNA_for_target_coverage)
 
         
         added_values = []
         added_indices = []    
-        for i in range(len(suggested_target_coverage_amounts)):
+        for i, suggested_target_coverage_amount in enumerate(suggested_target_coverage_amounts):
             added_values.extend([
                 gDNA_for_target_coverage_list[i],
                 target_coverage_suggested_list[i], 
                 target_read_amount_suggested_list[i]])
             
             added_indices.extend([
-                f"gDNA_for_suggested_target_coverage_{suggested_target_coverage_amounts[i]}",
-                f"coverage_for_suggested_target_coverage_{suggested_target_coverage_amounts[i]}",
-                f"reads_for_suggested_target_coverage_{suggested_target_coverage_amounts[i]}"])
+                f"gDNA_for_suggested_target_coverage_{suggested_target_coverage_amount}",
+                f"coverage_for_suggested_target_coverage_{suggested_target_coverage_amount}",
+                f"reads_for_suggested_target_coverage_{suggested_target_coverage_amount}"])
         
         result_series_values = [
             f"{result_dict['target_gDNA_for_max_coverage_result'][0]:.2f}",
             f"{result_dict['target_gDNA_for_max_coverage_result'][1]['target_coverage_suggested']:.2f}" if result_dict['target_gDNA_for_max_coverage_result'][1] is not None else None,
             f"{result_dict['target_gDNA_for_max_coverage_result'][2]:.2f}",
             f"{result_dict['max_gDNA_target_coverage_suggested_result'][0]:.2f}",
             f"{result_dict['max_gDNA_target_coverage_suggested_result'][1]['target_coverage_suggested']:.2f}" if result_dict['max_gDNA_target_coverage_suggested_result'][1] is not None else None,
```

### Comparing `crispr_library_prep-0.1.8/pyproject.toml` & `crispr_library_prep-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crispr-library-prep"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Basheer Becerra <bbecerr@outlook.com>"]
 readme = "README.md"
 packages = [{include = "crispr_library_prep"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `crispr_library_prep-0.1.8/setup.py` & `crispr_library_prep-0.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'numpy>=1.23,<2.0',
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'typeguard>=3.0.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'crispr-library-prep',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '',
     'author': 'Basheer Becerra',
     'author_email': 'bbecerr@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `crispr_library_prep-0.1.8/PKG-INFO` & `crispr_library_prep-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-library-prep
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

