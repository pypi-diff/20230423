# Comparing `tmp/n0struct-0.2.92.tar.gz` & `tmp/n0struct-0.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.92.tar", last modified: Tue Apr 18 04:33:57 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.93.tar", last modified: Sun Apr 23 05:44:12 2023, max compression
```

## Comparing `n0struct-0.2.92.tar` & `n0struct-0.2.93.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.884253 n0struct-0.2.92/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.92/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-04-18 04:33:57.885253 n0struct-0.2.92/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.92/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.808189 n0struct-0.2.92/n0struct/
--rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.92/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.92/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.92/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.92/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.92/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.92/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.92/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15645 2023-04-18 03:40:30.000000 n0struct-0.2.92/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4070 2023-04-18 03:45:21.000000 n0struct-0.2.92/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20911 2023-04-18 03:47:04.000000 n0struct-0.2.92/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.92/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    11636 2023-04-18 04:27:09.000000 n0struct-0.2.92/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17317 2023-04-18 04:08:26.000000 n0struct-0.2.92/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7527 2023-04-18 04:15:40.000000 n0struct-0.2.92/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    77456 2023-04-18 04:22:33.000000 n0struct-0.2.92/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.92/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3852 2023-04-18 04:31:43.000000 n0struct-0.2.92/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.92/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.92/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6658 2023-04-18 04:28:52.000000 n0struct-0.2.92/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4117 2023-04-18 04:29:28.000000 n0struct-0.2.92/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.880258 n0struct-0.2.92/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.92/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.92/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.92/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.92/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.92/n0struct/test/test_n0struct3.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.857859 n0struct-0.2.92/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2023-04-18 04:33:57.000000 n0struct-0.2.92/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 04:33:57.891284 n0struct-0.2.92/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.452194 n0struct-0.2.93/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.93/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-04-23 05:44:12.452194 n0struct-0.2.93/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.93/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.327218 n0struct-0.2.93/n0struct/
+-rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.93/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.93/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.93/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.93/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.93/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.93/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.93/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15645 2023-04-18 03:40:30.000000 n0struct-0.2.93/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-18 03:45:21.000000 n0struct-0.2.93/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20911 2023-04-18 03:47:04.000000 n0struct-0.2.93/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.93/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    12159 2023-04-18 10:16:45.000000 n0struct-0.2.93/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17317 2023-04-18 04:08:26.000000 n0struct-0.2.93/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     7527 2023-04-18 04:15:40.000000 n0struct-0.2.93/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    77456 2023-04-18 04:22:33.000000 n0struct-0.2.93/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.93/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-18 04:31:43.000000 n0struct-0.2.93/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.93/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.93/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6658 2023-04-18 04:28:52.000000 n0struct-0.2.93/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4117 2023-04-18 04:29:28.000000 n0struct-0.2.93/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.436621 n0struct-0.2.93/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.93/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.93/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.93/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.93/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.93/n0struct/test/test_n0struct3.py
+drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.405377 n0struct-0.2.93/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 05:44:12.467867 n0struct-0.2.93/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.93/setup.py
```

### Comparing `n0struct-0.2.92/LICENSE` & `n0struct-0.2.93/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/PKG-INFO` & `n0struct-0.2.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.92
+Version: 0.2.93
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.92/README.md` & `n0struct-0.2.93/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/__init__.py` & `n0struct-0.2.93/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_arrays.py` & `n0struct-0.2.93/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.93/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_date.py` & `n0struct-0.2.93/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_files.py` & `n0struct-0.2.93/n0struct/n0struct_files.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_files_csv.py` & `n0struct-0.2.93/n0struct/n0struct_files_csv.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.93/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_findall.py` & `n0struct-0.2.93/n0struct/n0struct_findall.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_git.py` & `n0struct-0.2.93/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_logging.py` & `n0struct-0.2.93/n0struct/n0struct_logging.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_mask.py` & `n0struct-0.2.93/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.93/n0struct/n0struct_n0dict_.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         if parent is not None:
             if isinstance(parent, dict):
                 if not len(parent.items()):
                     return ""
                 for key, value in parent.items():
                     if result:
                         result += "\n"
+                        
                     if isinstance(value, (list, tuple)):
                         for i, subitm in enumerate(value):
                             if i:
                                 result += "\n"
                             sub_result = self.__xml(subitm, indent+inc_indent, inc_indent)
                             if not sub_result:
                                 if isinstance(sub_result, str):
@@ -114,17 +115,25 @@
                                 else:
                                     result += " "*indent + f"<{key}/>"
                             else:
                                 if '>' in sub_result:
                                     result += " "*indent + f"<{key}>\n{sub_result}\n" + " "*indent + f"</{key}>"
                                 else:
                                     result += " "*indent + f"<{key}>{sub_result}</{key}>"
-                    elif isinstance(value, (str, int, float)):
+                    elif isinstance(value, (int, float)):
                         if not key.startswith("@"):
-                            result += " "*indent + f"<{key}>{str(value).translate(html_entities)}</{key}>"
+                            result += " "*indent + f"<{key}>{value}</{key}>"
+                    elif isinstance(value, str):
+                        if not key.startswith("@"):
+                            result += " "*indent + f"<{key}>"
+                            if value.lstrip().upper().startswith("<![CDATA[") and value.rstrip().endswith("]]>"):
+                                result += value
+                            else:
+                                result += value.translate(html_entities)
+                            result += f"</{key}>"
                     elif isinstance(value, dict):
                         sub_result = self.__xml(value, indent+inc_indent, inc_indent)
 
                         attribs = ""
                         attribs_of_current_key = [(__key[1:], __value) for __key,__value in value.items() if __key.startswith("@")]
                         if len(attribs_of_current_key):
                             for __key, __value in attribs_of_current_key:
@@ -149,19 +158,19 @@
             else:
                 raise TypeError(f"__xml(..): Unknown type ({type(parent)}) == {parent}")
 
             return result
         else:
             return ""
     # **************************************************************************
-    def to_xml(self, indent: int = 4, encoding: str = "utf-8") -> str:
+    def to_xml(self, indent: int = 4, encoding: str = "utf-8", quote: str = '"') -> str:
         """
         Public function: export self into xml result string
         """
-        return (f'<?xml version="1.0" encoding="{encoding}"?>\n' if encoding else '') + \
+        return (f'<?xml version={quote}1.0{quote} encoding={quote}{encoding}{quote}?>\n' if encoding else '') + \
             self.__xml(self, 0, indent)
     # **************************************************************************
     # JSON
     # **************************************************************************
     def __json(self, parent: dict, indent: int, inc_indent: int) -> str:
         """
         Private function: recursively export n0dict into json result string
```

### Comparing `n0struct-0.2.92/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.93/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_n0list_.py` & `n0struct-0.2.93/n0struct/n0struct_n0list_.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.93/n0struct/n0struct_n0list_n0dict.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_random.py` & `n0struct-0.2.93/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_references.py` & `n0struct-0.2.93/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.93/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_utils.py` & `n0struct-0.2.93/n0struct/n0struct_utils.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.93/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/n0struct_utils_find.py` & `n0struct-0.2.93/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/test/test_n0struct.py` & `n0struct-0.2.93/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/test/test_n0struct2.py` & `n0struct-0.2.93/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct/test/test_n0struct3.py` & `n0struct-0.2.93/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.93/n0struct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.92
+Version: 0.2.93
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.92/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.93/n0struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.92/setup.py` & `n0struct-0.2.93/setup.py`

 * *Files identical despite different names*

