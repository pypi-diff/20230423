# Comparing `tmp/n0struct-0.2.93.tar.gz` & `tmp/n0struct-0.2.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.93.tar", last modified: Sun Apr 23 05:44:12 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.94.tar", last modified: Sun Apr 23 14:01:16 2023, max compression
```

## Comparing `n0struct-0.2.93.tar` & `n0struct-0.2.94.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.452194 n0struct-0.2.93/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.93/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-04-23 05:44:12.452194 n0struct-0.2.93/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.93/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.327218 n0struct-0.2.93/n0struct/
--rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.93/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.93/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.93/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.93/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.93/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.93/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.93/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15645 2023-04-18 03:40:30.000000 n0struct-0.2.93/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4070 2023-04-18 03:45:21.000000 n0struct-0.2.93/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20911 2023-04-18 03:47:04.000000 n0struct-0.2.93/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.93/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    12159 2023-04-18 10:16:45.000000 n0struct-0.2.93/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17317 2023-04-18 04:08:26.000000 n0struct-0.2.93/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7527 2023-04-18 04:15:40.000000 n0struct-0.2.93/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    77456 2023-04-18 04:22:33.000000 n0struct-0.2.93/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.93/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3852 2023-04-18 04:31:43.000000 n0struct-0.2.93/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.93/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.93/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6658 2023-04-18 04:28:52.000000 n0struct-0.2.93/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4117 2023-04-18 04:29:28.000000 n0struct-0.2.93/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.436621 n0struct-0.2.93/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.93/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.93/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.93/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.93/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.93/n0struct/test/test_n0struct3.py
-drwxrwxrwx   0        0        0        0 2023-04-23 05:44:12.405377 n0struct-0.2.93/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 05:44:11.000000 n0struct-0.2.93/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 05:44:12.467867 n0struct-0.2.93/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:01:16.077435 n0struct-0.2.94/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.94/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-04-23 14:01:16.078465 n0struct-0.2.94/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.94/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 14:01:16.047055 n0struct-0.2.94/n0struct/
+-rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.94/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.94/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.94/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13176 2023-04-23 10:14:47.000000 n0struct-0.2.94/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.94/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.94/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.94/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15645 2023-04-18 03:40:30.000000 n0struct-0.2.94/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-18 03:45:21.000000 n0struct-0.2.94/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20911 2023-04-18 03:47:04.000000 n0struct-0.2.94/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.94/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    12168 2023-04-23 10:15:27.000000 n0struct-0.2.94/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17317 2023-04-18 04:08:26.000000 n0struct-0.2.94/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     7515 2023-04-23 06:00:38.000000 n0struct-0.2.94/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    75711 2023-04-23 13:24:17.000000 n0struct-0.2.94/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.94/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-18 04:31:43.000000 n0struct-0.2.94/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.94/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.94/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6658 2023-04-18 04:28:52.000000 n0struct-0.2.94/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4117 2023-04-18 04:29:28.000000 n0struct-0.2.94/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:01:16.077435 n0struct-0.2.94/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.94/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.94/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    33263 2023-04-23 13:25:25.000000 n0struct-0.2.94/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.94/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.94/n0struct/test/test_n0struct3.py
+-rw-rw-rw-   0        0        0     1849 2023-04-23 14:00:38.000000 n0struct-0.2.94/n0struct/test/test_n0struct4.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:01:16.069993 n0struct-0.2.94/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 14:01:15.000000 n0struct-0.2.94/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 14:01:16.079455 n0struct-0.2.94/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.94/setup.py
```

### Comparing `n0struct-0.2.93/LICENSE` & `n0struct-0.2.94/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/PKG-INFO` & `n0struct-0.2.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.93
+Version: 0.2.94
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.93/README.md` & `n0struct-0.2.94/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/__init__.py` & `n0struct-0.2.94/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_arrays.py` & `n0struct-0.2.94/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.94/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_date.py` & `n0struct-0.2.94/n0struct/n0struct_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,19 @@
                     return datetime.datetime.strptime(input_date_str, pyformat_DDMMYYYY).date()     # 16-07-2020
                 except (ValueError, TypeError):
                     try:
                         return datetime.datetime.strptime(input_date_str, "%d.%m.%Y").date()        # 16.07.2020
                     except (ValueError, TypeError):
                         try:
                             return datetime.datetime.strptime(input_date_str, "%m/%d/%Y").date()    # 07/16/2020
-                        except (ValueError, TypeError):
-                            return input_date_str
+                        except (ValueError, TypeError) as ex:
+                            if raise_exception:
+                                raise ex
+                            else:
+                                return input_date_str
 # ******************************************************************************
 # LEGACY
 # ******************************************************************************
 def from_date(input_date_str: str, date_format: str) -> typing.Union[None, datetime.datetime, str]:
     """
     LEGACY
     """
```

### Comparing `n0struct-0.2.93/n0struct/n0struct_files.py` & `n0struct-0.2.94/n0struct/n0struct_files.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_files_csv.py` & `n0struct-0.2.94/n0struct/n0struct_files_csv.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.94/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_findall.py` & `n0struct-0.2.94/n0struct/n0struct_findall.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_git.py` & `n0struct-0.2.94/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_logging.py` & `n0struct-0.2.94/n0struct/n0struct_logging.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_mask.py` & `n0struct-0.2.94/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.94/n0struct/n0struct_n0dict_.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         result = ""
         xpath_list = self.xpath(mode)
         if xpath_list:
             xpath_maxlen = max(len(itm[0]) for itm in xpath_list) + 2  # plus 2 chars '"]'
             for itm in xpath_list:
                 result += ("['%-" + str(xpath_maxlen) + "s = %s\n") % \
                             (
-                                itm[0] + "']",  # Don't move to the main
+                                itm[0] + "']",  # Don't move to the main part
                                 ('"' + str(itm[1]) + '"') if itm[1] else "None"
                             )
         return result
     # **************************************************************************
     # XML
     # **************************************************************************
     def __xml(self, parent: dict, indent: int, inc_indent: int) -> typing.Union[str, None]:
@@ -205,18 +205,18 @@
             elif value is None:
                 result += " "*indent + f'"{key}": null'
             else:
                 raise TypeError(f"Unknown type ({type(value)}) {key} == {value}")
         return result
     # **************************************************************************
     def to_json(self,
-                indent: int = 4,
-                pairs_in_one_line = True,
-                json_convention: bool = True,
-                skip_empty_arrays: bool = False,
+                indent: int = 4,
+                pairs_in_one_line = True,
+                json_convention: bool = True,
+                skip_empty_arrays: bool = False,
                 compress: bool = False,
     ) -> str:
         """
         Public function: export self into json result string
         """
         if compress:
             indent = 0
```

### Comparing `n0struct-0.2.93/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.94/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_n0list_.py` & `n0struct-0.2.94/n0struct/n0struct_n0list_.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,21 +94,21 @@
         if isinstance(xpath, str):
             return self._get(xpath, raise_exception = True)
         else:
             return super(n0list_, self).__getitem__(xpath)
     # # **************************************************************************
     # # def append(self, sigle_item):
     # # if isinstance(sigle_item, (list,n0list_)):
-    # # raise (TypeError, '(%s)%s must be scalar' % (type(sigle_item), sigle_item))
+    # # raise (TypeError, f"({type(sigle_item)}){sigle_item} must be scalar")
     # # super(n0list_, self).append(sigle_item)  #append the item to itself (the list)
     # # return self
     # # **************************************************************************
     # # def extend(self, other_list):
     # # if not isinstance(other_list, (list,n0list_)):
-    # # raise (TypeError, '(%s)%s must be list' % (type(sigle_item), sigle_item))
+    # # raise (TypeError, f"({type(sigle_item)}){sigle_item} must be list")
     # # super(n0list_, self).extend(other_list)
     # # return self
     # # **************************************************************************
     def _in(self, other_list, in_is_expected: bool):
         if not isinstance(other_list, (list, tuple)):
             other_list = [other_list]
         for itm in self:
```

### Comparing `n0struct-0.2.93/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.94/n0struct/n0struct_n0list_n0dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -241,20 +241,15 @@
         if xpath_match(prefix, exclude_xpaths):
             return result
 
         for i, itm in enumerate(self):
             if i >= len(other):
                 # other list is SHORTER that self
                 result["differences"].append(
-                    "List %s is longer %s: %s[%d]='%s' doesn't exist in %s" %
-                    (
-                        self_name, other_name,
-                        self_name, i, str(self[i]),
-                        other_name
-                    )
+                    f"List {self_name} is longer {other_name}: {self_name}[{i}]='{self[i]}' doesn't exist in {other_name}"
                 )
                 if get__flag_compare_return_place():
                     result["self_unique"].append((f"{prefix}[{i}]", self[i]))
                 else:
                     result["self_unique"].append(self[i])
                 continue
             # ######### if i >= len(other):
@@ -291,19 +286,18 @@
                             with contextlib.suppress(ValueError):  # self_value or other_value could not be converted to float
                                 if isinstance(self_value, (datetime.date, datetime.datetime)):
                                     difference = datetime.datetime.fromtimestamp(float(other_value.timestamp()) - float(self_value.timestamp()))
                                 else:
                                     difference = round(float(other_value) - float(self_value), 7)
                             result["not_equal"][-1][1].append(difference)
                         result["differences"].append(
-                            "Values are different: %s[%d]='%s' != %s[\"%s\"]='%s' " %
-                            (
-                                self_name, i, str(self[i]),
-                                other_name, i, str(other[i])
-                            )
+                            "Values are different: " +
+                            f"{self_name}[{i}]='{self[i]}'" +
+                            " != " +
+                            f"{other_name}['{i}']='{other[i]}'"
                         )
                     else:
                         if get__flag_compare_return_equal():
                             result["self_equal"].append(self)
                             result["other_equal"].append(other)
                 elif isinstance(self[i], (list, tuple)):
                     result.update_extend(
@@ -347,46 +341,43 @@
                                 self[i],
                                 type(other[i]),
                                 other[i]
                             )
                         )
                     )
                     result["differences"].append(
-                        f"!!Types are different: {self_name}[{i}]=({type(self[i])}){self[i]} != {other_name}[{i}]=({type(other[i])}){other[i]}"
+                        "!!Types are different: " +
+                        f"{self_name}[{i}]=({type(self[i])}){self[i]}" +
+                        " != " +
+                        f"{other_name}[{i}]=({type(other[i])}){other[i]}"
                     )
                 else:
                     result["not_equal"].append(
                         (
                             f"{prefix}[{i}]",
                             (
                                 self[i],
                                 other[i]
                             )
                         )
                     )
                     result["differences"].append(
-                        "Values are different: %s[%d]='%s' != %s[\"%s\"]='%s' " %
-                        (
-                            self_name, i, str(self[i]),
-                            other_name, i, str(other[i])
-                        )
+                        "Values are different: " +
+                        f"{self_name}[{i}]='{self[i]}'" +
+                        " != " +
+                        f"{other_name}['{i}']='{other[i]}'"
                     )
 
         # ######### for i in enumerate(self)[0]:
         if len(other) > len(self):
             # self list is SHORTER that other
             for i, itm in enumerate(other[len(self):]):
                 i += len(self)
                 result["differences"].append(
-                    "List %s is longer %s: %s[%d]='%s' doesn't exist in %s" %
-                    (
-                        other_name, self_name,
-                        other_name, i, str(other[i]),
-                        self_name
-                    )
+                    f"List {other_name} is longer {self_name}: {other_name}[{i}]='{other[i]}' doesn't exist in {self_name}"
                 )
                 if get__flag_compare_return_place():
                     result["other_unique"].append(("%s[%i]" % (prefix, i), other[i]))
                 else:
                     result["other_unique"].append(other[i])
         return result
     # **************************************************************************
@@ -486,74 +477,68 @@
                 if type(self_value) == type(other_value):
                     if isinstance(self_value, (str, int, float, datetime.date)):
                         if self_value != other_value:
                             if self_i == other_i:
                                 # VERY IMPORTANT TO SHOW ORIGINAL VALUES, NOT TRANSFORMED
                                 result["not_equal"].append(
                                     (
-                                        "%s[%d]" % (prefix, self_i),
+                                        f"{prefix}[{self_i}]",
                                         [
                                             self[self_i],
                                             other[other_i]
                                         ]
                                     )
                                 )
                             else:
                                 # VERY IMPORTANT TO SHOW ORIGINAL VALUES, NOT TRANSFORMED
                                 result["not_equal"].append(
                                     (
-                                        "%s[%d]<>[%d]" % (prefix, self_i, other_i),
+                                        f"{prefix}[{self_i}]<>[{other_i}]",
                                         [
                                             self[self_i],
                                             other[other_i]
                                         ]
                                     )
                                 )
                             if get__flag_compare_return_difference_of_values():
                                 try:
                                     difference = round(float(other_value) - float(self_value), 7)
                                 except ValueError:  # self_value or other_value could not be converted to float
                                     difference = None
                                 result["not_equal"][-1][1].append(difference)
                             result["differences"].append(
-                                "Values are different: %s[%d]='%s' != %s[%d]='%s' " %
-                                (
-                                    self_name, self_i, str(self[self_i]),
-                                    other_name, other_i, str(other[other_i])
-                                )
+                                "Values are different: " +
+                                f"{self_name}[{self_i}]='{self[self_i]}'" +
+                                " != " +
+                                f"{other_name}[{other_i}]='{other[other_i]}'"
                             )
                         else:
                             # NOT TESTED! #2
                             if get__flag_compare_return_equal():
                                 result["self_equal"].append(self)
                                 result["other_equal"].append(other)
                     elif isinstance(self[self_i], (list, tuple)):
                         result.update_extend(
                             n0list(self[self_i]).compare(
                                 n0list(other[other_i]),
-                                "%s[%d]" % (self_name, self_i),
-                                "%s[%d]" % (other_name, other_i),
-                                "%s[%d]%s" % (
-                                    prefix,
-                                    other_i,
-                                    ("<>[%d]" % other_i) if self_i != other_i else ""
-                                ),
+                                f"{self_name}[{self_i}]",
+                                f"{other_name}[{other_i}]",
+                                f"{prefix}[{other_i}]" + f"<>[{other_i}]" if self_i != other_i else "",
                                 composite_key=composite_key, compare_only=compare_only,
                                 exclude_xpaths=exclude_xpaths, transform=transform,
                             )
                         )
                     elif isinstance(self[self_i], dict):
                         result.update_extend(
                             n0dict(self[self_i]).compare(
                                 # n0dict(other[other_i]),  # 0.18
                                 other[other_i],
-                                self_name + "[" + str(self_i) + "]",
-                                other_name + "[" + str(other_i) + "]",
-                                prefix + "[" + str(self_i) + "]" + (
-                                    "<>[" + str(other_i) + "]" if self_i != other_i else ""),
+                                f"{self_name}[{self_i}]",
+                                f"{other_name}[{other_i}]",
+                                f"{prefix}[{self_i}]" + (f"<>[{other_i}]" if self_i != other_i else ""),
                                 one_of_list_compare=self.compare,
                                 composite_key=composite_key, compare_only=compare_only,
                                 exclude_xpaths=exclude_xpaths, transform=transform,
                             )
                         )
                     elif self[self_i] is None:
                         # type(self[self_i]) == type(other[other_i]) and self[self_i] is None
@@ -562,85 +547,76 @@
                     else:
                         raise TypeError(f"Not expected type {type(self[self_i])} in {self_name}[{self_i}]/{other_name}[{other_i}]")
                 # ######### if type(self[i]) == type(other[i]):
                 else:
                     if get__flag_compare_check_different_types():
                         result["difftypes"].append(
                             (
-                                prefix + "[" + str(self_i) + "]",
+                                f"{prefix}[{self_i}]",
                                 (
                                     type(self[self_i]), self[self_i],
                                     type(other[other_i]), other[other_i]
                                 )
                             )
                         )
-                        result["differences"].append("++Types are different: %s[%d]=(%s)%s != %s[%d]=(%s)%s" %
-                                                  (
-                                                      self_name, self_i, type(self[self_i]), str(self[self_i]),
-                                                      other_name, other_i, type(other[other_i]), str(other[other_i]),
-                                                  )
-                                                  )
+                        result["differences"].append(
+                            "++Types are different: " +
+                            f"{self_name}[{self_i}]=({type(self[self_i])}){self[self_i]}" +
+                            " != " +
+                            f"{other_name}[{other_i}]=({type(other[other_i])}){other[other_i]}"
+                        )
                     else:
                         if self_i == other_i:
                             result["not_equal"].append(
                                 (
-                                    "%s[%d]" % (prefix, self_i),
+                                    f"{prefix}[{self_i}]",
                                     (
                                         self[self_i],
                                         other[other_i]
                                     )
                                 )
                             )
                         else:
                             result["not_equal"].append(
                                 (
-                                    "%s[%d]<>[%d]" % (prefix, self_i, other_i),
+                                    f"{prefix}[{self_i}]<>[{other_i}]",
                                     (
                                         self[self_i],
                                         other[other_i]
                                     )
                                 )
                             )
                         result["differences"].append(
-                            "Values are different: %s[%d]='%s' != %s[\"%s\"]='%s' " %
-                            (
-                                self_name, self_i, str(self[self_i]),
-                                other_name, other_i, str(other[other_i])
-                            )
+                            "Values are different: " +
+                            f"{self_name}[{self_i}]='{self[self_i]}'" +
+                            " != " +
+                            f"{other_name}[{other_i}]='{other[other_i]}'"
                         )
                 del self_not_exist_in_other[[itm[0] for itm in self_not_exist_in_other].index(composite_key)]
                 del other_not_exist_in_self[[itm[0] for itm in other_not_exist_in_self].index(composite_key)]
             # ######### if key in other_not_exist_in_self:
         # ######### for key in notmutable__self_not_exist_in_other:
 
         if self_not_exist_in_other:
             for composite_key, self_i in self_not_exist_in_other:
                 result["differences"].append(
-                    "Element %s[%d]='%s' doesn't exist in %s" %
-                    (
-                        self_name, self_i, str(self[self_i]),
-                        other_name
-                    )
+                    f"Element {self_name}[{self_i}]='{self[self_i]}' doesn't exist in {other_name}"
                 )
                 if get__flag_compare_return_place():
-                    result["self_unique"].append((prefix + "[" + str(self_i) + "]", self[self_i]))
+                    result["self_unique"].append((f"{prefix}[{self_i}]", self[self_i]))
                 else:
                     result["self_unique"].append(self[self_i])
 
         if other_not_exist_in_self:
             for composite_key, other_i in other_not_exist_in_self:
                 result["differences"].append(
-                    "Element %s[%d]='%s' doesn't exist in %s" %
-                    (
-                        other_name, other_i, str(other[other_i]),
-                        self_name
-                    )
+                    f"Element {other_name}[{other_i}]='{other[other_i]}' doesn't exist in {self_name}"
                 )
                 if get__flag_compare_return_place():
-                    result["other_unique"].append(("%s[%d]" % (prefix, other_i), other[other_i]))
+                    result["other_unique"].append((f"{prefix}[{other_i}]", other[other_i]))
                 else:
                     result["other_unique"].append(other[other_i])
 
         return result
 # ******************************************************************************
 # ******************************************************************************
 # ******************************************************************************
@@ -808,54 +784,53 @@
                     if type(self_value) == type(other_value):
                         if isinstance(self_value, (str, int, float, datetime.date)):
                             if self_value != other_value \
                                 and (not compare_only or xpath_match(fullxpath, compare_only)):
                                 # VERY IMPORTANT TO SHOW ORIGINAL VALUES, NOT TRANSFORMED
                                 result["not_equal"].append(
                                     (
-                                        "%s/%s" % (prefix, key),
+                                        f"{prefix}/{key}",
                                         [
                                             self[key],
                                             other[key]
                                         ]
                                     )
                                 )
                                 if get__flag_compare_return_difference_of_values():
                                     try:
                                         difference = round(float(other_value) - float(self_value), 7)
                                     except ValueError:  # self_value or other_value could not be converted to float
                                         difference = None
                                     result["not_equal"][-1][1].append(difference)
                                 result["differences"].append(
-                                    "Values are different: %s[\"%s\"]=%s != %s[\"%s\"]=%s " %
-                                    (
-                                        self_name, key, self[key],
-                                        other_name, key, other[key]
-                                    )
+                                    "Values are different: " +
+                                    f"{self_name}['{key}']={self[key]}" +
+                                    " != " +
+                                    f"{other_name}['{key}']={other[key]}"
                                 )
                                 is_still_equal = False
                         elif isinstance(self[key], (list, tuple)):
                             result.update_extend(
                                 one_of_list_compare(
                                     n0list(self[key]),
                                     n0list(other[key]),
-                                    '%s["%s"]' % (self_name, key),
-                                    '%s["%s"]' % (other_name, key),
-                                    "%s/%s" % (prefix, key),
+                                    f"{self_name}['{key}']",
+                                    f"{other_name}['{key}']",
+                                    f"{prefix}/{key}",
                                     composite_key=composite_key, compare_only=compare_only,
                                     exclude_xpaths=exclude_xpaths, transform=transform,
                                 )
                             )
                         elif isinstance(self[key], dict):
                             result.update_extend(
                                 n0dict(self[key]).compare(
                                     n0dict(other[key]),
-                                    '%s["%s"]' % (self_name, key),
-                                    '%s["%s"]' % (other_name, key),
-                                    "%s/%s" % (prefix, key),
+                                    f"{self_name}['{key}']",
+                                    f"{other_name}['{key}']",
+                                    f"{prefix}/{key}",
                                     one_of_list_compare=one_of_list_compare,  # Only for n0dict. compare()
                                     composite_key=composite_key, compare_only=compare_only,
                                     exclude_xpaths=exclude_xpaths, transform=transform,
                                 )
                             )
                         elif self[key] is None:
                             # Because of type(self[key]) == type(other[key]) and self[key] is None, so both are None
@@ -864,74 +839,60 @@
                             raise TypeError(f"Not expected type {type(self[key])} in {key}['{self_name}']")
                     else:
                         if not compare_only or xpath_match(fullxpath, compare_only):
                             is_still_equal = False
                             if get__flag_compare_check_different_types():
                                 result["difftypes"].append(
                                     (
-                                        prefix + "/" + str(key),
+                                        f"{prefix}/{key}",
                                         (
                                             type(self[key]), self[key],
                                             type(other[key]), other[key]
                                         )
                                     )
                                 )
                                 result["differences"].append(
-                                    "*Types are different: %s[\"%s\"]=(%s)%s != %s[\"%s\"]=(%s)%s" %
-                                    (
-                                        self_name, key, type(self[key]), str(self[key]),
-                                        other_name, key, type(other[key]), str(other[key]),
-                                    )
+                                    "*Types are different: " +
+                                    f"{self_name}['{key}']=({type(self[key])}){self[key]}" +
+                                    " != " +
+                                    f"{other_name}['{key}']=({type(other[key])}){other[key]}"
                                 )
                             else:
                                 result["not_equal"].append((prefix + "/" + key, (self[key], other[key])))
                                 result["differences"].append(
-                                    "Values are different: %s[\"%s\"]=%s != %s[\"%s\"]=%s " %
-                                    (
-                                        self_name, key, self[key],
-                                        other_name, key, other[key]
-                                    )
+                                    "Values are different: " +
+                                    f"{self_name}['{key}']={self[key]}" +
+                                    " != " +
+                                    f"{other_name}['{key}']={other[key]}"
                                 )
                 self_not_exist_in_other.remove(key)
                 other_not_exist_in_self.remove(key)
 
         if self_not_exist_in_other:
             for key in self_not_exist_in_other:
-                fullxpath = "%s/%s" % (prefix, key)
+                fullxpath = f"{prefix}/{key}"
                 if not xpath_match(fullxpath, exclude_xpaths) \
                    and (not compare_only or xpath_match(fullxpath, compare_only)):
                     is_still_equal = False
                     result["differences"].append(
-                        "Element %s[\"%s\"]='%s' doesn't exist in %s" %
-                        (
-                            self_name,
-                            key,
-                            str(self[key]),
-                            other_name
-                        )
+                        f"Element {self_name}['{key}']='{self[key]}' doesn't exist in {other_name}"
                     )
                     if get__flag_compare_return_place():
                         result["self_unique"].append((fullxpath, self[key]))
                     else:
                         result["self_unique"].append(self[key])
-                        
+
         if other_not_exist_in_self:
             for key in other_not_exist_in_self:
-                fullxpath = "%s/%s" % (prefix, key)
+                fullxpath = f"{prefix}/{key}"
                 if not xpath_match(fullxpath, exclude_xpaths) \
                    and (not compare_only or xpath_match(fullxpath, compare_only)):
                     is_still_equal = False
                     result["differences"].append(
-                        "Element %s[\"%s\"]='%s' doesn't exist in %s" %
-                        (
-                            other_name,
-                            key,
-                            str(other[key]),
-                            self_name
-                        )
+                        f"Element {other_name}['{key}']='{other[key]}' doesn't exist in {self_name}"
                     )
                     if get__flag_compare_return_place():
                         result["other_unique"].append((fullxpath, other[key]))
                     else:
                         result["other_unique"].append(other[key])
 
         if is_still_equal and get__flag_compare_return_equal():
@@ -1035,17 +996,17 @@
                         else:
                             raise TypeError(f"If index is in '{cur_node_name_index}', then ({type(cur_node_index)})'{cur_node_index}' must be str")
                 else:
                     nxt_parent_node = cur_parent_node
 
                 if node_index or len(xpath_list) > 1:
                     if node_index:
-                        return self._find(["[%s]" % str(node_index)] + xpath_list[1:], nxt_parent_node, return_lists, cur_found_xpath_str)
+                        return self._find([f"[{node_index}]"] + xpath_list[1:], nxt_parent_node, return_lists, cur_found_xpath_str)
                     else:
-                        return self._find(                             xpath_list[1:], nxt_parent_node, return_lists, cur_found_xpath_str)
+                        return self._find(                      xpath_list[1:], nxt_parent_node, return_lists, cur_found_xpath_str)
                 else:
                     # ================================
                     # FOUND: the last is n0dict
                     # ================================
                     return cur_parent_node, cur_node_name_index, nxt_parent_node, xpath_found_str + '/' + cur_node_name_index, None
             # ..................................................................
             # Try to parse as list
@@ -1122,21 +1083,21 @@
                                 parent_node[node_name],
                                 return_lists,
                                 xpath_found_str + '/' + node_name
                 )
             else:
                 return self._find(
                                 [
-                                    "[%s%s'%s']" % (node_index[0], node_index[1], node_index[2]) \
-                                    if isinstance(node_index, tuple) else \
-                                    "[%s]" % str(node_index) # Because of mypy: error: Not all arguments converted during string formatting
+                                    f"[{node_index[0]}{node_index[1]}'{node_index[2]}']"
+                                    if isinstance(node_index, tuple)
+                                    else f"[{node_index}]"  # Because of mypy: error: Not all arguments converted during string formatting
                                 ] + xpath_list[1:],
                                 parent_node[node_name],
                                 return_lists,
-                                xpath_found_str + '/' + node_name
+                                f"{xpath_found_str}/{node_name}"
                 )
         # ##########################################################################################
         # Index in n0list (node_index is not None)
         # ##########################################################################################
         else:
             #--------------------------------
             # NOT FOUND: new element in n0list
@@ -1154,15 +1115,15 @@
                 if not isinstance(parent_node, (list, tuple)):
                     # Hidden list. Convert single item into list
                     parent_node = [parent_node]
                 cur_values = n0list()
                 fst_parent_node = fst_node_name_index = fst_value = fst_found_xpath_str = None
                 for i,cur_node in enumerate(parent_node):
                     cur_parent_node, cur_node_name_index, cur_value, cur_found_xpath_str, \
-                        cur_not_found_xpath_list = self._find(["[%d]" % i] + xpath_list[1:], parent_node, return_lists, xpath_found_str)
+                        cur_not_found_xpath_list = self._find([f"[{i}]"] + xpath_list[1:], parent_node, return_lists, xpath_found_str)
                     if not cur_not_found_xpath_list:
                         cur_values.append(cur_value)
                         if not fst_found_xpath_str:
                             fst_parent_node, fst_node_name_index, fst_value, fst_found_xpath_str = \
                                 cur_parent_node, cur_node_name_index, cur_value, cur_found_xpath_str
                 if not return_lists and len(cur_values) == 1:
                     cur_values = cur_values[0]
@@ -1217,18 +1178,18 @@
 
                     if not isinstance(parent_node, dict):
                         raise IndexError(f"If key '{node_index[0]}' is set, then ({type(parent_node)})'{str(parent_node)}' must be n0dict at '{xpath_found_str}'")
                     if node_index[0] not in parent_node:
                         return parent_node, None, None, xpath_found_str, xpath_list
 
                     return self._find(
-                                        ["[text()%s%s]" % (node_index[1], node_index[2]), ".."] + xpath_list[1:],
+                                        [f"[text(){node_index[1]}{node_index[2]}]", ".."] + xpath_list[1:],
                                         parent_node[node_index[0]],
                                         return_lists,
-                                        xpath_found_str + '/' + node_index[0]
+                                        f"{xpath_found_str}/{node_index[0]}"
                     )
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
             # Pure index
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
             else:
                 try:
                     node_index_int = n0eval(node_index)
@@ -1241,26 +1202,26 @@
                     len__parent_node = 1
                     parent_node = [parent_node]
 
                 if node_index_int >= len__parent_node or node_index_int < -len__parent_node:
                     #--------------------------------
                     # NOT FOUND: Element in n0list
                     #--------------------------------
-                    return parent_node, "[%d]" % node_index_int, None, xpath_found_str, xpath_list
+                    return parent_node, f"[{node_index_int}]", None, xpath_found_str, xpath_list
 
                 if len(xpath_list) == 1:
                     #================================
                     # FOUND: the last is n0list
                     #================================
-                    return parent_node, "[%d]" % node_index_int, parent_node[node_index_int], xpath_found_str, None
+                    return parent_node, f"[{node_index_int}]", parent_node[node_index_int], xpath_found_str, None
                 else:
                     #*******************************
                     # Deeper: any type under n0dict
                     #*******************************
-                    return self._find(xpath_list[1:], parent_node[node_index_int], return_lists, "%s[%d]" % (xpath_found_str, node_index_int))
+                    return self._find(xpath_list[1:], parent_node[node_index_int], return_lists, f"{xpath_found_str}[{node_index_int}]")
     # **************************************************************************
     # **************************************************************************
     def _add(self, parent_node, node_name_index: typing.Union[str, tuple], xpath_list: list) -> typing.Tuple[str, str]:
         if node_name_index:
             # or cur_node_name OR cur_node_index MUST have value, both could NOT have values
             cur_node_name, cur_node_index = split_name_index(node_name_index)
         else:
@@ -1301,15 +1262,15 @@
                         next_node = parent_node
                         next_node_name_index = next_node_name
                 else:
                     # Node is EXISTED
                     if next_node_index:
                         parent_node.update({next_node_name: [parent_node[next_node_name]]})
                         next_node = parent_node[next_node_name]
-                        next_node_name_index = "[%s]" % next_node_index
+                        next_node_name_index = f"[{next_node_index}]"
                     else:
                         raise IndexError(f"Nonsense! How to create already existed node '{next_node_name}'?")
             else:
                 if next_node_index != "new()":
                     raise IndexError(f"Expect new() for adding index, but got '{next_node_index}'")
                 parent_node.append(None)
                 next_node = parent_node
@@ -1339,21 +1300,21 @@
                         next_node = parent_node[-1]
                         next_node_name_index = next_node_name
                     else:
                         # Next is list under dict
                         parent_node.append(n0dict({next_node_name: n0list()}))
                         next_node = parent_node[-1][next_node_name]
                         # Expected to have 'new()' in next_node_index, else it will be failed at the next step
-                        next_node_name_index = "[%s]" % str(next_node_index)
+                        next_node_name_index = f"[{next_node_index}]"
                 elif next_node_index:
                     # List under list: [0][0] or [0]/[0]
                     parent_node.append(n0list([]))
                     next_node = parent_node[-1]
                     # Expected to have 'new()' in next_node_index, else it will be failed at the next step
-                    next_node_name_index = "[%s]" % str(next_node_index)
+                    next_node_name_index = f"[{next_node_index}]"
                 else:
                     raise ValueError("Nonsence! Both next_node_name and next_node_index could NOT be empty")
             elif cur_node_index == "last()":
                 # Came from previous level: we create [None] and point to [last()] for exchange
                 if not isinstance(parent_node, (list, tuple, n0list)):
                     raise ValueError(f"Nonsence! if index '{cur_node_index}' is set, then ({type(parent_node)}){str(parent_node)} must be n0list")
                 if next_node_name:
@@ -1364,21 +1325,21 @@
                         next_node_name_index = next_node_name
                     else:
                         # Next is list under dict
                         # parent_node[-1] = n0dict({next_node_name: n0list([])})
                         parent_node[-1] = n0dict({next_node_name: n0list()})
                         next_node = parent_node[-1][next_node_name]
                         # Expected to have 'new()' in next_node_index, else it will be failed at the next step
-                        next_node_name_index = "[%s]" % str(next_node_index)
+                        next_node_name_index = f"[{next_node_index}]"
                 elif next_node_index:
                     # List under list: [0][0] or [0]/[0]
                     parent_node.append(n0list([]))
                     next_node = parent_node[-1]
                     # Expected to have 'new()' in next_node_index, else it will be failed at the next step
-                    next_node_name_index = "[%s]" % str(next_node_index)
+                    next_node_name_index = f"[{next_node_index}]"
             # New fix
             elif n0eval(cur_node_index) == len(parent_node):
                 parent_node.append(None)
                 next_node = parent_node
                 next_node_name_index = "[last()]"
             else:
                 raise SyntaxError(f"Nonsence! Impossible to add item {cur_node_index} to the list {str(parent_node)}")
```

### Comparing `n0struct-0.2.93/n0struct/n0struct_random.py` & `n0struct-0.2.94/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_references.py` & `n0struct-0.2.94/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.94/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_utils.py` & `n0struct-0.2.94/n0struct/n0struct_utils.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.94/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/n0struct_utils_find.py` & `n0struct-0.2.94/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/test/test_n0struct.py` & `n0struct-0.2.94/n0struct/test/test_n0struct.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,28 +68,30 @@
         n0print("*"*3 + " " + key)
         for itm in differences2_wise_compare[key]:
             n0print(itm)
 
     n0print("="*80)
     n0debug("differences1_direct_compare")
     n0debug_calc(notemptyitems(differences1_direct_compare["differences"]), 'notemptyitems(differences1_direct_compare["differences"])')
-    assert notemptyitems(differences1_direct_compare["differences"]) == 1
+    assert notemptyitems(differences1_direct_compare["differences"])        == 1
     n0debug_calc(notemptyitems(differences1_direct_compare["not_equal"]), 'notemptyitems(differences1_direct_compare["not_equal"])')
-    assert notemptyitems(differences1_direct_compare["not_equal"]) == 4
-    assert notemptyitems(differences1_direct_compare["difftypes"]) == 0
-    assert notemptyitems(differences1_direct_compare["other_unique"]) == 0
-    assert notemptyitems(differences1_direct_compare["self_unique"]) == 0
+    assert notemptyitems(differences1_direct_compare["not_equal"])          == 4
+    assert notemptyitems(differences1_direct_compare["difftypes"])          == 0
+    assert notemptyitems(differences1_direct_compare["other_unique"])       == 0
+    assert notemptyitems(differences1_direct_compare["self_unique"])        == 0
 
     n0print("="*80)
     n0debug("differences2_wise_compare")
-    assert differences1_direct_compare["differences"]     == differences2_wise_compare["differences"]
-    assert differences1_direct_compare["not_equal"]     == differences2_wise_compare["not_equal"]
+    assert differences1_direct_compare["differences"]  == differences2_wise_compare["differences"]
+    # n0debug_calc(differences1_direct_compare["not_equal"],  'differences1_direct_compare["not_equal"]')
+    # n0debug_calc(differences2_wise_compare["not_equal"],    'differences2_wise_compare["not_equal"]')
+    assert differences1_direct_compare["not_equal"]    == differences2_wise_compare["not_equal"]
     assert differences1_direct_compare["difftypes"]    == differences2_wise_compare["difftypes"]
     assert differences1_direct_compare["other_unique"] == differences2_wise_compare["other_unique"]
-    assert differences1_direct_compare["self_unique"]== differences2_wise_compare["self_unique"]
+    assert differences1_direct_compare["self_unique"]  == differences2_wise_compare["self_unique"]
 # ******************************************************************************
 def test_unsorted_lists():
     n0print("*"*80 + " 3 = Unsorted list in dictionary = direct_compare")
     differences1_direct_compare = dict1.direct_compare(dict3, "dict1", "dict3")
     for key in differences1_direct_compare:
         n0print("*"*3 + " " + key)
         for itm in differences1_direct_compare[key]:
@@ -104,34 +106,34 @@
         n0print("*"*3 + " " + key)
         for itm in differences2_wise_compare[key]:
             n0print(itm)
 
     n0print("="*80)
     n0debug("differences1_direct_compare")
     n0debug_calc(notemptyitems(differences1_direct_compare["differences"]), 'notemptyitems(differences1_direct_compare["differences"]')
-    assert notemptyitems(differences1_direct_compare["differences"]) == 12
+    assert notemptyitems(differences1_direct_compare["differences"])        == 12
     n0debug_calc(notemptyitems(differences1_direct_compare["not_equal"]), 'differences1_direct_compare["not_equal"]')
-    assert notemptyitems(differences1_direct_compare["not_equal"]) == 44
-    assert notemptyitems(differences1_direct_compare["difftypes"]) == 0
+    assert notemptyitems(differences1_direct_compare["not_equal"])          == 44
+    assert notemptyitems(differences1_direct_compare["difftypes"])          == 0
     n0debug_calc(notemptyitems(differences1_direct_compare["other_unique"]), 'notemptyitems(differences1_direct_compare["other_unique"])')
-    assert notemptyitems(differences1_direct_compare["other_unique"]) == 6
+    assert notemptyitems(differences1_direct_compare["other_unique"])       == 6
     n0debug_calc(notemptyitems(differences1_direct_compare["self_unique"]), 'notemptyitems(differences1_direct_compare["self_unique"])')
-    assert notemptyitems(differences1_direct_compare["self_unique"]) == 0
+    assert notemptyitems(differences1_direct_compare["self_unique"])        == 0
 
     n0print("="*80)
     n0debug("differences2_wise_compare")
     n0debug_calc(notemptyitems(differences2_wise_compare["differences"]), 'notemptyitems(differences2_wise_compare["differences"]')
-    assert notemptyitems(differences2_wise_compare["differences"]) == 2
+    assert notemptyitems(differences2_wise_compare["differences"])          == 2
     n0debug_calc(notemptyitems(differences2_wise_compare["not_equal"]), 'differences2_wise_compare["not_equal"]')
-    assert notemptyitems(differences2_wise_compare["not_equal"]) == 4
-    assert notemptyitems(differences2_wise_compare["difftypes"]) == 0
+    assert notemptyitems(differences2_wise_compare["not_equal"])            == 4
+    assert notemptyitems(differences2_wise_compare["difftypes"])            == 0
     n0debug_calc(notemptyitems(differences2_wise_compare["other_unique"]), 'notemptyitems(differences2_wise_compare["other_unique"])')
-    assert notemptyitems(differences2_wise_compare["other_unique"]) == 6
+    assert notemptyitems(differences2_wise_compare["other_unique"])         == 6
     n0debug_calc(notemptyitems(differences2_wise_compare["self_unique"]), 'notemptyitems(differences2_wise_compare["self_unique"])')
-    assert notemptyitems(differences2_wise_compare["self_unique"]) == 0
+    assert notemptyitems(differences2_wise_compare["self_unique"])          == 0
 # ******************************************************************************
 def main():
     n0print("="*80)
     n0debug_calc(dict1,"dict1")
     n0print("="*80)
     n0debug_calc(dict2,"dict2")
     n0print("="*80)
@@ -152,62 +154,62 @@
     n0debug_calc(dict1,'dict1')
     dict1["moreone/node[last()]/value"] = 2
     dict1["moreone/node[last()]/code"] = "two"
     dict1["moreone/node[new()]/value"] = 3
     dict1["moreone/node[-1]/value"] = 4
     dict1["moreone/node[-1]/code"] = "four"
 
-    assert isinstance(dict1["moreone/node[0]/value"],n0dict) == True
-    assert (dict1["moreone/node[1]/value"] is None) == True
-    assert isinstance(dict1["moreone/node[2]/value"],str) == True
-    assert (not dict1["moreone/node[2]/value"]) == True
-    assert dict1["moreone/node[3]/value"] == 2
-    assert dict1["moreone/node[4]/value"] == 4
+    assert isinstance(dict1["moreone/node[0]/value"],n0dict)                == True
+    assert (dict1["moreone/node[1]/value"] is None)                         == True
+    assert isinstance(dict1["moreone/node[2]/value"],str)                   == True
+    assert (not dict1["moreone/node[2]/value"])                             == True
+    assert dict1["moreone/node[3]/value"]                                   == 2
+    assert dict1["moreone/node[4]/value"]                                   == 4
 
     n0print(dict1.to_json())
     n0print(dict1.to_xml())
 
     n0print(dict1["moreone/node"])
 
-    assert len(dict1["moreone/node"]) == 5
-    assert len(dict1["moreone/node[*]"]) == 5
+    assert len(dict1["moreone/node"])                                       == 5
+    assert len(dict1["moreone/node[*]"])                                    == 5
 
     n0print(dict1["moreone"])
     assert len(dict1["moreone"]) == 1
 
     n0print(dict1["moreone/node/code[text()='four']/../value"])
-    assert dict1["moreone/node/code[text()='four']/../value"][0] == 4
-    assert dict1["moreone/node/code[text()='four']/../value"] == [4]
+    assert dict1["moreone/node/code[text()='four']/../value"][0]            == 4
+    assert dict1["moreone/node/code[text()='four']/../value"]               == [4]
 
 
     n0print(dict1["moreone/node/code[text()='two']/../value"])
-    assert dict1["moreone/node/code[text()='two']/../value"] == [2]
+    assert dict1["moreone/node/code[text()='two']/../value"]                == [2]
 
     dict1["moreone/node/code[text()='two']/../value"] = 6
     n0print(dict1["moreone/node/code[text()='two']/../value"])
-    assert dict1["moreone/node/code[text()='two']/../value"] == [6]
-    assert dict1["moreone/node/code[text()=two]/../value"] == [6]
-    assert dict1['moreone/node/code[text()="two"]/../value'] == [6]
+    assert dict1["moreone/node/code[text()='two']/../value"]                == [6]
+    assert dict1["moreone/node/code[text()=two]/../value"]                  == [6]
+    assert dict1['moreone/node/code[text()="two"]/../value']                == [6]
 
     n0print(dict1["moreone/node[code='two']/value"])
-    assert dict1["moreone/node[code='two']/value"] == [6]
+    assert dict1["moreone/node[code='two']/value"]                          == [6]
 
     dict1["moretwo/node/code"] = "seven"
     dict1["moretwo/node/value"] = 7
     n0print(dict1["moretwo/node/code[text()='seven']/../value"])
-    assert dict1["moretwo/node/code[text()='seven']/../value"] == 7
+    assert dict1["moretwo/node/code[text()='seven']/../value"]              == 7
 
     n0print(dict1["moretwo/node[code='seven']/value"])
-    assert dict1["moretwo/node[code='seven']/value"] == 7
+    assert dict1["moretwo/node[code='seven']/value"]                        == 7
 
     n0print(dict1.get("moretwo/node/code[text()='eight']/../value"))
-    assert dict1.get("moretwo/node/code[text()='eight']/../value") is None
+    assert dict1.get("moretwo/node/code[text()='eight']/../value")          is None
 
     n0print(dict1["?moretwo/node/code[text()='eight']/../value"] or None)
-    assert (dict1["?moretwo/node/code[text()='eight']/../value"] or None) is None
+    assert (dict1["?moretwo/node/code[text()='eight']/../value"] or None)   is None
 
     # set__debug_output(sys.stdout.write)
 
     str_json = """
     {
         "root": {
             "a": 1.0,
@@ -231,90 +233,90 @@
                 8
             ]
         }
     }
     """
     dict_from_json_default = n0dict(str_json)
     n0debug("dict_from_json_default")
-    assert isinstance(dict_from_json_default, n0dict) == True
-    assert isinstance(dict_from_json_default["root"], dict) == True
-    assert isinstance(dict_from_json_default["root/a"], float) == True # XML supports only str, for JSON float
-    assert isinstance(dict_from_json_default["root/b"], dict) == True
-    assert isinstance(dict_from_json_default["root/b/d"], dict) == True
-    assert isinstance(dict_from_json_default["root/b/d/e"], dict) == True
-    assert isinstance(dict_from_json_default["root/b/d/g"], list) == True # For recursively=False
-    assert isinstance(dict_from_json_default["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_json_default["root/b/d/g[1]"], dict) == True
-    assert isinstance(dict_from_json_default["root/b/d/g[1]/h"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_default["root/b/d/i"], list) == True # For JSON list
-    assert isinstance(dict_from_json_default["root/b/d/i[0]"], dict) == True
-    assert isinstance(dict_from_json_default["root/b/d/i[0]/j"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_default["root/k"], list) == True # For recursively=False
-    assert isinstance(dict_from_json_default["root/k[0]"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_default["root/k[1]"], int) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_default, n0dict)                                   == True
+    assert isinstance(dict_from_json_default["root"], dict)                             == True
+    assert isinstance(dict_from_json_default["root/a"], float)                          == True # XML supports only str, for JSON float
+    assert isinstance(dict_from_json_default["root/b"], dict)                           == True
+    assert isinstance(dict_from_json_default["root/b/d"], dict)                         == True
+    assert isinstance(dict_from_json_default["root/b/d/e"], dict)                       == True
+    assert isinstance(dict_from_json_default["root/b/d/g"], list)                       == True # For recursively=False
+    assert isinstance(dict_from_json_default["root/b/d/g[0]"], str)                     == True
+    assert isinstance(dict_from_json_default["root/b/d/g[1]"], dict)                    == True
+    assert isinstance(dict_from_json_default["root/b/d/g[1]/h"], int)                   == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_default["root/b/d/i"], list)                       == True # For JSON list
+    assert isinstance(dict_from_json_default["root/b/d/i[0]"], dict)                    == True
+    assert isinstance(dict_from_json_default["root/b/d/i[0]/j"], int)                   == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_default["root/k"], list)                           == True # For recursively=False
+    assert isinstance(dict_from_json_default["root/k[0]"], int)                         == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_default["root/k[1]"], int)                         == True # XML supports only str, for JSON int
     dict_from_json_default.to_json(); dict_from_json_default.to_xml(); dict_from_json_default.to_xpath()
 
     dict_from_json_force_n0dict = n0dict(str_json, force_n0dict = True)
     n0debug("dict_from_json_force_n0dict")
-    assert isinstance(dict_from_json_force_n0dict, n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/a"], float) == True # XML supports only str, for JSON float
-    assert isinstance(dict_from_json_force_n0dict["root/b"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/g"], list) == True # For recursively n0list
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[1]/h"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/i"], list) == True # For JSON list, for JSON recursively n0list
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_json_force_n0dict["root/b/d/i[0]/j"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_force_n0dict["root/k"], list) == True # For recursively n0list
-    assert isinstance(dict_from_json_force_n0dict["root/k[0]"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_force_n0dict["root/k[1]"], int) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_force_n0dict, n0dict)                              == True
+    assert isinstance(dict_from_json_force_n0dict["root"], n0dict)                      == True
+    assert isinstance(dict_from_json_force_n0dict["root/a"], float)                     == True # XML supports only str, for JSON float
+    assert isinstance(dict_from_json_force_n0dict["root/b"], n0dict)                    == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d"], n0dict)                  == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/e"], n0dict)                == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/g"], list)                  == True # For recursively n0list
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[0]"], str)                == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[1]"], n0dict)             == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/g[1]/h"], int)              == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/i"], list)                  == True # For JSON list, for JSON recursively n0list
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/i[0]"], n0dict)             == True
+    assert isinstance(dict_from_json_force_n0dict["root/b/d/i[0]/j"], int)              == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_force_n0dict["root/k"], list)                      == True # For recursively n0list
+    assert isinstance(dict_from_json_force_n0dict["root/k[0]"], int)                    == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_force_n0dict["root/k[1]"], int)                    == True # XML supports only str, for JSON int
     dict_from_json_force_n0dict.to_json(); dict_from_json_force_n0dict.to_xml(); dict_from_json_force_n0dict.to_xpath()
 
     dict_from_json_recursevely = n0dict(str_json, recursively=True)
     n0debug("dict_from_json_recursevely")
-    assert isinstance(dict_from_json_recursevely, n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/a"], float) == True # XML supports only str, for JSON float
-    assert isinstance(dict_from_json_recursevely["root/b"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d/g"], n0list) == True # For recursively=True
-    assert isinstance(dict_from_json_recursevely["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d/g[1]/h"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely["root/b/d/i"], n0list) == True # For JSON list, for JSON recursively n0list
-    assert isinstance(dict_from_json_recursevely["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely["root/b/d/i[0]/j"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely["root/k"], n0list) == True # For recursively=True
-    assert isinstance(dict_from_json_recursevely["root/k[0]"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely["root/k[1]"], int) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely, n0dict)                               == True
+    assert isinstance(dict_from_json_recursevely["root"], n0dict)                       == True
+    assert isinstance(dict_from_json_recursevely["root/a"], float)                      == True # XML supports only str, for JSON float
+    assert isinstance(dict_from_json_recursevely["root/b"], n0dict)                     == True
+    assert isinstance(dict_from_json_recursevely["root/b/d"], n0dict)                   == True
+    assert isinstance(dict_from_json_recursevely["root/b/d/e"], n0dict)                 == True
+    assert isinstance(dict_from_json_recursevely["root/b/d/g"], n0list)                 == True # For recursively=True
+    assert isinstance(dict_from_json_recursevely["root/b/d/g[0]"], str)                 == True
+    assert isinstance(dict_from_json_recursevely["root/b/d/g[1]"], n0dict)              == True
+    assert isinstance(dict_from_json_recursevely["root/b/d/g[1]/h"], int)               == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely["root/b/d/i"], n0list)                 == True # For JSON list, for JSON recursively n0list
+    assert isinstance(dict_from_json_recursevely["root/b/d/i[0]"], n0dict)              == True
+    assert isinstance(dict_from_json_recursevely["root/b/d/i[0]/j"], int)               == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely["root/k"], n0list)                     == True # For recursively=True
+    assert isinstance(dict_from_json_recursevely["root/k[0]"], int)                     == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely["root/k[1]"], int)                     == True # XML supports only str, for JSON int
     dict_from_json_recursevely.to_json(); dict_from_json_recursevely.to_xml(); dict_from_json_recursevely.to_xpath()
 
     dict_from_json_recursevely_force_n0dict = n0dict(str_json, recursively=True, force_n0dict = True)
     n0debug("dict_from_json_recursevely_force_n0dict")
-    assert isinstance(dict_from_json_recursevely_force_n0dict, n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/a"], float) == True # XML supports only str, for JSON float
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g"], n0list) == True # For recursively=True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g[0]"], str) == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict, n0dict)                  == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root"], n0dict)          == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/a"], float)         == True # XML supports only str, for JSON float
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b"], n0dict)        == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d"], n0dict)      == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/e"], n0dict)    == True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g"], n0list)    == True # For recursively=True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g[0]"], str)    == True
     assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g[1]/h"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/i"], n0list) == True # For JSON list, for JSON recursively n0list
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/g[1]/h"], int)  == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/i"], n0list)    == True # For JSON list, for JSON recursively n0list
     assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/i[0]/j"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k"], n0list) == True # For recursively=True
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k[0]"], int) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k[1]"], int) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/b/d/i[0]/j"], int)  == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k"], n0list)        == True # For recursively=True
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k[0]"], int)        == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_json_recursevely_force_n0dict["root/k[1]"], int)        == True # XML supports only str, for JSON int
     dict_from_json_recursevely_force_n0dict.to_json(); dict_from_json_recursevely_force_n0dict.to_xml(); dict_from_json_recursevely_force_n0dict.to_xpath()
 
     str_xml = """
     <root>
         <a>1</a>
         <b>
             <c>2</c>
@@ -335,91 +337,91 @@
         </b>
         <k>7</k>
         <k>8</k>
     </root>
     """
     dict_from_xml_default = n0dict(str_xml)
     n0debug("dict_from_xml_default")
-    assert isinstance(dict_from_xml_default, n0dict) == True
-    assert isinstance(dict_from_xml_default["root"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/a"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_default["root/b"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/b/d/g"], list) == True # For recursively=False
-    assert isinstance(dict_from_xml_default["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_xml_default["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/b/d/g[1]/h"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_default["root/b/d/i"], n0dict) == True # For JSON list, for JSON recursively n0list
-    assert isinstance(dict_from_xml_default["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_xml_default["root/b/d/i[0]/j"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_default["root/k"], list) == True # For recursively=False
-    assert isinstance(dict_from_xml_default["root/k[0]"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_default["root/k[1]"], str) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_default, n0dict)                                    == True
+    assert isinstance(dict_from_xml_default["root"], n0dict)                            == True
+    assert isinstance(dict_from_xml_default["root/a"], str)                             == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_default["root/b"], n0dict)                          == True
+    assert isinstance(dict_from_xml_default["root/b/d"], n0dict)                        == True
+    assert isinstance(dict_from_xml_default["root/b/d/e"], n0dict)                      == True
+    assert isinstance(dict_from_xml_default["root/b/d/g"], list)                        == True # For recursively=False
+    assert isinstance(dict_from_xml_default["root/b/d/g[0]"], str)                      == True
+    assert isinstance(dict_from_xml_default["root/b/d/g[1]"], n0dict)                   == True
+    assert isinstance(dict_from_xml_default["root/b/d/g[1]/h"], str)                    == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_default["root/b/d/i"], n0dict)                      == True # For JSON list, for JSON recursively n0list
+    assert isinstance(dict_from_xml_default["root/b/d/i[0]"], n0dict)                   == True
+    assert isinstance(dict_from_xml_default["root/b/d/i[0]/j"], str)                    == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_default["root/k"], list)                            == True # For recursively=False
+    assert isinstance(dict_from_xml_default["root/k[0]"], str)                          == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_default["root/k[1]"], str)                          == True # XML supports only str, for JSON int
     dict_from_xml_default.to_json(); dict_from_xml_default.to_xml(); dict_from_xml_default.to_xpath()
 
     # force_n0dict = True for XML is useless, in any cases dictionaries will be n0dict
     dict_from_xml_force_n0dict = n0dict(str_xml, force_n0dict = True)
     n0debug("dict_from_xml_force_n0dict")
-    assert isinstance(dict_from_xml_force_n0dict, n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/a"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_force_n0dict["root/b"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g"], list) == True # For recursively=False
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[1]/h"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i"], n0dict) == True # For JSON list
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i[0]/j"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_force_n0dict["root/k"], list) == True # For recursively=False
-    assert isinstance(dict_from_xml_force_n0dict["root/k[0]"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_force_n0dict["root/k[1]"], str) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_force_n0dict, n0dict)                               == True
+    assert isinstance(dict_from_xml_force_n0dict["root"], n0dict)                       == True
+    assert isinstance(dict_from_xml_force_n0dict["root/a"], str)                        == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_force_n0dict["root/b"], n0dict)                     == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d"], n0dict)                   == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/e"], n0dict)                 == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g"], list)                   == True # For recursively=False
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[0]"], str)                 == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[1]"], n0dict)              == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/g[1]/h"], str)               == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i"], n0dict)                 == True # For JSON list
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i[0]"], n0dict)              == True
+    assert isinstance(dict_from_xml_force_n0dict["root/b/d/i[0]/j"], str)               == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_force_n0dict["root/k"], list)                       == True # For recursively=False
+    assert isinstance(dict_from_xml_force_n0dict["root/k[0]"], str)                     == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_force_n0dict["root/k[1]"], str)                     == True # XML supports only str, for JSON int
     dict_from_xml_force_n0dict.to_json(); dict_from_xml_force_n0dict.to_xml(); dict_from_xml_force_n0dict.to_xpath()
 
     dict_from_xml_recursevely = n0dict(str_xml, recursively=True)
     n0debug("dict_from_xml_recursevely")
-    assert isinstance(dict_from_xml_recursevely, n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/a"], str) == True # XML supports only str
-    assert isinstance(dict_from_xml_recursevely["root/b"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/g"], n0list) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/g[1]/h"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely["root/b/d/i"], n0dict) == True # For JSON list
-    assert isinstance(dict_from_xml_recursevely["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely["root/b/d/i[0]/j"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely["root/k"], n0list) == True
-    assert isinstance(dict_from_xml_recursevely["root/k[0]"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely["root/k[1]"], str) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely, n0dict)                                == True
+    assert isinstance(dict_from_xml_recursevely["root"], n0dict)                        == True
+    assert isinstance(dict_from_xml_recursevely["root/a"], str)                         == True # XML supports only str
+    assert isinstance(dict_from_xml_recursevely["root/b"], n0dict)                      == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d"], n0dict)                    == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/e"], n0dict)                  == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/g"], n0list)                  == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/g[0]"], str)                  == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/g[1]"], n0dict)               == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/g[1]/h"], str)                == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely["root/b/d/i"], n0dict)                  == True # For JSON list
+    assert isinstance(dict_from_xml_recursevely["root/b/d/i[0]"], n0dict)               == True
+    assert isinstance(dict_from_xml_recursevely["root/b/d/i[0]/j"], str)                == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely["root/k"], n0list)                      == True
+    assert isinstance(dict_from_xml_recursevely["root/k[0]"], str)                      == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely["root/k[1]"], str)                      == True # XML supports only str, for JSON int
     dict_from_xml_recursevely.to_json(); dict_from_xml_recursevely.to_xml(); dict_from_xml_recursevely.to_xpath()
 
     dict_from_xml_recursevely_force_n0dict = n0dict(str_xml, recursively=True, force_n0dict = True)
     n0debug("dict_from_xml_recursevely_force_n0dict")
-    assert isinstance(dict_from_xml_recursevely_force_n0dict, n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/a"], str) == True # XML supports only str
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/e"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g"], n0list) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[0]"], str) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[1]"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[1]/h"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i"], n0dict) == True # For JSON list
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i[0]"], n0dict) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i[0]/j"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k"], n0list) == True
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k[0]"], str) == True # XML supports only str, for JSON int
-    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k[1]"], str) == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely_force_n0dict, n0dict)                   == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root"], n0dict)           == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/a"], str)            == True # XML supports only str
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b"], n0dict)         == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d"], n0dict)       == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/e"], n0dict)     == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g"], n0list)     == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[0]"], str)     == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[1]"], n0dict)  == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/g[1]/h"], str)   == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i"], n0dict)     == True # For JSON list
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i[0]"], n0dict)  == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/b/d/i[0]/j"], str)   == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k"], n0list)         == True
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k[0]"], str)         == True # XML supports only str, for JSON int
+    assert isinstance(dict_from_xml_recursevely_force_n0dict["root/k[1]"], str)         == True # XML supports only str, for JSON int
     dict_from_xml_recursevely_force_n0dict.to_json(); dict_from_xml_recursevely_force_n0dict.to_xml(); dict_from_xml_recursevely_force_n0dict.to_xpath()
 
     str_xml_empty = "<root/>"
     dict_from_xml_empty = n0dict(str_xml_empty)
     n0debug("dict_from_xml_empty")
     assert isinstance(dict_from_xml_empty, n0dict) == True
     assert (dict_from_xml_empty["root"] is None) == True
@@ -433,25 +435,25 @@
                 "d": {
                     "e": 3
                 }
             }
         }
     )
     n0debug("dict4")
-    assert isinstance(dict4, n0dict) == True
-    assert dict4["a"] == 1
-    assert dict4["b/c"] == 2
-    assert dict4["b/d/e"] == 3
-    assert dict4.get("b/d/e", "ALREADY_DELETED") == 3
-    assert dict4.pop("b/d/e") == 3
-    assert dict4.get("b/d/e", "ALREADY_DELETED") == "ALREADY_DELETED"
-    assert dict4.delete("b/c")["a"] == 1
-    assert dict4.get("b/c", "ALREADY_DELETED") == "ALREADY_DELETED"
+    assert isinstance(dict4, n0dict)                                                    == True
+    assert dict4["a"]                                                                   == 1
+    assert dict4["b/c"]                                                                 == 2
+    assert dict4["b/d/e"]                                                               == 3
+    assert dict4.get("b/d/e", "ALREADY_DELETED")                                        == 3
+    assert dict4.pop("b/d/e")                                                           == 3
+    assert dict4.get("b/d/e", "ALREADY_DELETED")                                        == "ALREADY_DELETED"
+    assert dict4.delete("b/c")["a"]                                                     == 1
+    assert dict4.get("b/c", "ALREADY_DELETED")                                          == "ALREADY_DELETED"
     assert dict4.delete("b/d", recursively=True)
-    assert dict4.get("b", "ALREADY_DELETED") == "ALREADY_DELETED"
+    assert dict4.get("b", "ALREADY_DELETED")                                            == "ALREADY_DELETED"
     n0debug("dict4")
 
     dict5 = n0dict().update(
         {
             "a": {
                 "b": {
                     "c": {
@@ -491,16 +493,16 @@
                 ],
             },
         }
     })
     n0debug("dict6")
     n0debug_calc(dict6.findall("//Root/Node1"))
     n0debug_calc(dict6.findall("//Root/Node2/Subnode2_1/tag[text()==PARAM1]/../value"))
-    assert list(dict6.findall("//Root/Node2/Subnode2_1/tag[text()==PARAM1]/../value").keys())[0] == "//Root/Node2/Subnode2_1[0]/value"
-    assert list(dict6.findall("//Root/Node2/Subnode2_1/tag[text()==PARAM1]/../value").values())[0] == "VALUE1 from subnode2_1"
+    assert list(dict6.findall("//Root/Node2/Subnode2_1/tag[text()==PARAM1]/../value").keys())[0]    == "//Root/Node2/Subnode2_1[0]/value"
+    assert list(dict6.findall("//Root/Node2/Subnode2_1/tag[text()==PARAM1]/../value").values())[0]  == "VALUE1 from subnode2_1"
 
     dict7 = n0dict({
         "Root": {
             "Nodes": [
                 [
                     {"tag": "PARAM1", "value": "VALUE1 from subnode0_0"},
                     {"tag": "PARAM2", "value": "VALUE2 from subnode0_1"},
@@ -519,13 +521,13 @@
                 ],
             ],
         }
     })
     n0print("\n" + list(dict7.findall("//").values())[0].to_xpath())
     found = dict7.findall("//Root/Nodes/tag[text()==PARAM1]/../value")
     n0debug_calc(found, '"//Root/Nodes/tag[text()==PARAM1]/../value"')
-    assert len(found) == 4
-    assert list(found.values())[2] == "VALUE1 from subnode2_0"
+    assert len(found)                                                                               == 4
+    assert list(found.values())[2]                                                                  == "VALUE1 from subnode2_0"
 
 if __name__ == '__main__':
     main()
     n0print("Mission acomplished")
```

### Comparing `n0struct-0.2.93/n0struct/test/test_n0struct2.py` & `n0struct-0.2.94/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct/test/test_n0struct3.py` & `n0struct-0.2.94/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.93/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.94/n0struct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.93
+Version: 0.2.94
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.93/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.94/n0struct.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 n0struct.egg-info/not-zip-safe
 n0struct.egg-info/requires.txt
 n0struct.egg-info/top_level.txt
 n0struct/test/__init__.py
 n0struct/test/__main__.py
 n0struct/test/test_n0struct.py
 n0struct/test/test_n0struct2.py
-n0struct/test/test_n0struct3.py
+n0struct/test/test_n0struct3.py
+n0struct/test/test_n0struct4.py
```

### Comparing `n0struct-0.2.93/setup.py` & `n0struct-0.2.94/setup.py`

 * *Files identical despite different names*

