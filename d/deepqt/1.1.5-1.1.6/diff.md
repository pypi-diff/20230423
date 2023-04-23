# Comparing `tmp/deepqt-1.1.5.tar.gz` & `tmp/deepqt-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepqt-1.1.5.tar", last modified: Sun Apr 23 13:35:39 2023, max compression
+gzip compressed data, was "deepqt-1.1.6.tar", last modified: Sun Apr 23 13:44:11 2023, max compression
```

## Comparing `deepqt-1.1.5.tar` & `deepqt-1.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.441092 deepqt-1.1.5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.5/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:35:39.441092 deepqt-1.1.5/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.5/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.437758 deepqt-1.1.5/deepqt/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.441092 deepqt-1.1.5/deepqt/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.5/deepqt/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.5/deepqt/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.5/deepqt/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-23 13:35:33.000000 deepqt-1.1.5/deepqt/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19121 2023-04-22 22:39:27.000000 deepqt-1.1.5/deepqt/api_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5755 2023-04-23 13:20:53.000000 deepqt-1.1.5/deepqt/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2213 2023-04-23 11:59:44.000000 deepqt-1.1.5/deepqt/driver_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/driver_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35336 2023-04-23 13:12:39.000000 deepqt-1.1.5/deepqt/driver_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/driver_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.5/deepqt/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8040 2023-04-22 21:40:28.000000 deepqt-1.1.5/deepqt/glossary.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6272 2023-04-22 23:12:13.000000 deepqt-1.1.5/deepqt/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.5/deepqt/main.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.5/deepqt/quote_protection.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.441092 deepqt-1.1.5/deepqt/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.5/deepqt/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/rc_generated_files/fallback_icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.5/deepqt/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/term_extractor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.5/deepqt/trie.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.441092 deepqt-1.1.5/deepqt/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.5/deepqt/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3497 2023-04-22 21:01:56.000000 deepqt-1.1.5/deepqt/ui_generated_files/ui_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.5/deepqt/ui_generated_files/ui_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/ui_generated_files/ui_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.5/deepqt/ui_generated_files/ui_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/worker_thread.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.5/deepqt/xml_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:35:39.437758 deepqt-1.1.5/deepqt.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-23 13:35:39.000000 deepqt-1.1.5/deepqt.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.5/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-23 13:35:39.441092 deepqt-1.1.5/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.5/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.6/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:44:11.221088 deepqt-1.1.6/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.6/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.214422 deepqt-1.1.6/deepqt/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.6/deepqt/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.6/deepqt/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.6/deepqt/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-23 13:43:59.000000 deepqt-1.1.6/deepqt/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19121 2023-04-22 22:39:27.000000 deepqt-1.1.6/deepqt/api_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5755 2023-04-23 13:20:53.000000 deepqt-1.1.6/deepqt/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2308 2023-04-23 13:43:45.000000 deepqt-1.1.6/deepqt/driver_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/driver_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35336 2023-04-23 13:12:39.000000 deepqt-1.1.6/deepqt/driver_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/driver_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.6/deepqt/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8040 2023-04-22 21:40:28.000000 deepqt-1.1.6/deepqt/glossary.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6272 2023-04-22 23:12:13.000000 deepqt-1.1.6/deepqt/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.6/deepqt/main.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.6/deepqt/quote_protection.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.6/deepqt/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/rc_generated_files/fallback_icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.6/deepqt/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/term_extractor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.6/deepqt/trie.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.6/deepqt/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3497 2023-04-22 21:01:56.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/worker_thread.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/xml_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.6/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-23 13:44:11.221088 deepqt-1.1.6/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.6/setup.py
```

### Comparing `deepqt-1.1.5/LICENSE` & `deepqt-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/PKG-INFO` & `deepqt-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.5/README.md` & `deepqt-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/CustomQ/CComboBox.py` & `deepqt-1.1.6/deepqt/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/CustomQ/CTableWidget.py` & `deepqt-1.1.6/deepqt/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/api_interface.py` & `deepqt-1.1.6/deepqt/api_interface.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/config.py` & `deepqt-1.1.6/deepqt/config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/driver_api_config.py` & `deepqt-1.1.6/deepqt/driver_api_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         self.comboBox_api_type.setCurrentIndex(1 if config.is_pro_version else 0)
 
     def get_key(self):
         """
         If the api is supposed to be PRO, remove :fx from the key and vice versa.
         """
         key = self.lineEdit_api_key.text().strip()
+        # Don't try to fix an empty key.
+        if key == "":
+            return key
+        
         if self.comboBox_api_type.currentIndex() == 1:
             key = re.sub(":fx$", "", key)
         else:
             key = re.sub("^(.*?)(:fx)?$", r"\1:fx", key)
         return key
     
     def show_api_help(self):
```

### Comparing `deepqt-1.1.5/deepqt/driver_epub_preview.py` & `deepqt-1.1.6/deepqt/driver_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/driver_mainwindow.py` & `deepqt-1.1.6/deepqt/driver_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/driver_text_preview.py` & `deepqt-1.1.6/deepqt/driver_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/file_table.py` & `deepqt-1.1.6/deepqt/file_table.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/glossary.py` & `deepqt-1.1.6/deepqt/glossary.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/helpers.py` & `deepqt-1.1.6/deepqt/helpers.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/main.py` & `deepqt-1.1.6/deepqt/main.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/quote_protection.py` & `deepqt-1.1.6/deepqt/quote_protection.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/rc_generated_files/fallback_icons_rc.py` & `deepqt-1.1.6/deepqt/rc_generated_files/fallback_icons_rc.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/structures.py` & `deepqt-1.1.6/deepqt/structures.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/term_extractor.py` & `deepqt-1.1.6/deepqt/term_extractor.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/trie.py` & `deepqt-1.1.6/deepqt/trie.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/ui_generated_files/ui_api_config.py` & `deepqt-1.1.6/deepqt/ui_generated_files/ui_api_config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/ui_generated_files/ui_epub_preview.py` & `deepqt-1.1.6/deepqt/ui_generated_files/ui_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/ui_generated_files/ui_mainwindow.py` & `deepqt-1.1.6/deepqt/ui_generated_files/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/ui_generated_files/ui_text_preview.py` & `deepqt-1.1.6/deepqt/ui_generated_files/ui_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/worker_thread.py` & `deepqt-1.1.6/deepqt/worker_thread.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt/xml_parser.py` & `deepqt-1.1.6/deepqt/xml_parser.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/deepqt.egg-info/PKG-INFO` & `deepqt-1.1.6/deepqt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.5/deepqt.egg-info/SOURCES.txt` & `deepqt-1.1.6/deepqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.5/setup.cfg` & `deepqt-1.1.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepqt
-version = 1.1.5
+version = 1.1.6
 description = Harness the power of the DeepL API with this friendly user interface.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/VoxelCubes/DeepQt
 keywords = deepl, deepl api, qt, pyside6
 license_files = LICENSE
 classifiers =
```

