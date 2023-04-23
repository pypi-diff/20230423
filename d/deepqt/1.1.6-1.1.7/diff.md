# Comparing `tmp/deepqt-1.1.6.tar.gz` & `tmp/deepqt-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepqt-1.1.6.tar", last modified: Sun Apr 23 13:44:11 2023, max compression
+gzip compressed data, was "deepqt-1.1.7.tar", last modified: Sun Apr 23 17:35:49 2023, max compression
```

## Comparing `deepqt-1.1.6.tar` & `deepqt-1.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.6/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:44:11.221088 deepqt-1.1.6/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.6/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.214422 deepqt-1.1.6/deepqt/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.6/deepqt/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.6/deepqt/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.6/deepqt/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-23 13:43:59.000000 deepqt-1.1.6/deepqt/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19121 2023-04-22 22:39:27.000000 deepqt-1.1.6/deepqt/api_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5755 2023-04-23 13:20:53.000000 deepqt-1.1.6/deepqt/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2308 2023-04-23 13:43:45.000000 deepqt-1.1.6/deepqt/driver_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/driver_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35336 2023-04-23 13:12:39.000000 deepqt-1.1.6/deepqt/driver_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/driver_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.6/deepqt/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8040 2023-04-22 21:40:28.000000 deepqt-1.1.6/deepqt/glossary.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6272 2023-04-22 23:12:13.000000 deepqt-1.1.6/deepqt/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.6/deepqt/main.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.6/deepqt/quote_protection.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.6/deepqt/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/rc_generated_files/fallback_icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.6/deepqt/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/term_extractor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.6/deepqt/trie.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.6/deepqt/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3497 2023-04-22 21:01:56.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.6/deepqt/ui_generated_files/ui_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/worker_thread.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.6/deepqt/xml_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 13:44:11.217755 deepqt-1.1.6/deepqt.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-23 13:44:11.000000 deepqt-1.1.6/deepqt.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.6/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-23 13:44:11.221088 deepqt-1.1.6/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.6/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.7/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 17:35:48.997665 deepqt-1.1.7/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.7/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/deepqt/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/deepqt/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.7/deepqt/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.7/deepqt/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.7/deepqt/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-23 17:35:23.000000 deepqt-1.1.7/deepqt/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19121 2023-04-22 22:39:27.000000 deepqt-1.1.7/deepqt/api_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5755 2023-04-23 13:20:53.000000 deepqt-1.1.7/deepqt/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2308 2023-04-23 13:43:45.000000 deepqt-1.1.7/deepqt/driver_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5022 2023-04-23 16:26:06.000000 deepqt-1.1.7/deepqt/driver_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35696 2023-04-23 17:34:38.000000 deepqt-1.1.7/deepqt/driver_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3213 2023-04-23 16:25:57.000000 deepqt-1.1.7/deepqt/driver_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.7/deepqt/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8040 2023-04-22 21:40:28.000000 deepqt-1.1.7/deepqt/glossary.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6272 2023-04-22 23:12:13.000000 deepqt-1.1.7/deepqt/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.7/deepqt/main.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.7/deepqt/quote_protection.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/deepqt/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.7/deepqt/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.7/deepqt/rc_generated_files/fallback_icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.7/deepqt/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.7/deepqt/term_extractor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.7/deepqt/trie.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/deepqt/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.7/deepqt/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3497 2023-04-22 21:01:56.000000 deepqt-1.1.7/deepqt/ui_generated_files/ui_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.7/deepqt/ui_generated_files/ui_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.7/deepqt/ui_generated_files/ui_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.7/deepqt/ui_generated_files/ui_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.7/deepqt/worker_thread.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.7/deepqt/xml_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-23 17:35:48.997665 deepqt-1.1.7/deepqt.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-23 17:35:48.000000 deepqt-1.1.7/deepqt.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.7/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-23 17:35:48.997665 deepqt-1.1.7/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.7/setup.py
```

### Comparing `deepqt-1.1.6/LICENSE` & `deepqt-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/PKG-INFO` & `deepqt-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.6
+Version: 1.1.7
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.6/README.md` & `deepqt-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/CustomQ/CComboBox.py` & `deepqt-1.1.7/deepqt/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/CustomQ/CTableWidget.py` & `deepqt-1.1.7/deepqt/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/api_interface.py` & `deepqt-1.1.7/deepqt/api_interface.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/config.py` & `deepqt-1.1.7/deepqt/config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/driver_api_config.py` & `deepqt-1.1.7/deepqt/driver_api_config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/driver_epub_preview.py` & `deepqt-1.1.7/deepqt/driver_epub_preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     Also offer to save the previews to a file.
     """
 
     config: cfg.Config
     epub_file: st.EpubFile
 
     def __init__(self, parent, epub_file: st.EpubFile, config: cfg.Config):
-        Qw.QDialog.__init__(self, parent=parent)
+        # Don't pass the parent due to a bug in PySide6.
+        Qw.QDialog.__init__(self)
         self.setupUi(self)
         self.setWindowTitle(f"{epub_file.path.name} - Preview")
 
         self.config = config
         self.epub_file = epub_file
 
         # Abort if the epub file was not initialized.
```

### Comparing `deepqt-1.1.6/deepqt/driver_mainwindow.py` & `deepqt-1.1.7/deepqt/driver_mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,30 +462,37 @@
         self.threadpool.start(worker)
 
     def char_count_warning(self, translator: deepl.Translator) -> bool:
         # Make sure the user is aware of how many characters will be translated.
         # Check if the allotted character count won't exceed the quota.
         total_chars = sum(file.char_count for file in self.file_table.files.values())
         api_usage = translator.get_usage()
-        allowed_chars = api_usage.character.limit - api_usage.character.count
-        remaining_chars = allowed_chars - total_chars
-        warning_msg = (
-            f"You are about to translate {hp.format_char_count(total_chars)} "
-            f"{hp.f_plural(total_chars, 'character')},\n"
-            f"leaving you with {hp.format_char_count(remaining_chars)} "
-            f"{hp.f_plural(remaining_chars, 'character')}."
-            f"\nProceed?"
-        )
-        if api_usage.character.limit_reached:
-            warning_msg = "You have reached your character limit.\nProceed anyway?"
-        elif total_chars > allowed_chars:
+        if api_usage.character.limit != DEEPL_USAGE_UNLIMITED:
+            allowed_chars = api_usage.character.limit - api_usage.character.count
+            remaining_chars = allowed_chars - total_chars
             warning_msg = (
                 f"You are about to translate {hp.format_char_count(total_chars)} "
-                f"{hp.f_plural(total_chars, 'character')}, "
-                f"which exceeds your remaining character limit of {hp.format_char_count(allowed_chars)}.\nProceed anyway?"
+                f"{hp.f_plural(total_chars, 'character')},\n"
+                f"leaving you with {hp.format_char_count(remaining_chars)} "
+                f"{hp.f_plural(remaining_chars, 'character')}."
+                f"\nProceed?"
+            )
+            if api_usage.character.limit_reached:
+                warning_msg = "You have reached your character limit.\nProceed anyway?"
+            elif total_chars > allowed_chars:
+                warning_msg = (
+                    f"You are about to translate {hp.format_char_count(total_chars)} "
+                    f"{hp.f_plural(total_chars, 'character')}, "
+                    f"which exceeds your remaining character limit of {hp.format_char_count(allowed_chars)}.\nProceed anyway?"
+                )
+        else:
+            warning_msg = (
+                f"You are about to translate {hp.format_char_count(total_chars)} "
+                f"{hp.f_plural(total_chars, 'character')}."
+                f"\nProceed?"
             )
         # Ask the user if he wants to proceed, just in case.
         logger.info(f"Character limit warning: {warning_msg}")
         affirmation = show_question(self, "API Limit", warning_msg)
         if not affirmation:
             logger.info("Translation cancelled.")
             return False
```

### Comparing `deepqt-1.1.6/deepqt/driver_text_preview.py` & `deepqt-1.1.7/deepqt/driver_text_preview.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     Also offer to save the previews to a file.
     """
 
     config: cfg.Config
     text_file: st.TextFile
 
     def __init__(self, parent, text_file: st.TextFile, config: cfg.Config):
-        Qw.QDialog.__init__(self, parent=parent)
+        # Don't pass the parent due to a bug in PySide6.
+        Qw.QDialog.__init__(self)
         self.setupUi(self)
         self.setWindowTitle(f"{text_file.path.name} - Preview")
 
         self.config = config
         self.text_file = text_file
 
         self.preview_text()
```

### Comparing `deepqt-1.1.6/deepqt/file_table.py` & `deepqt-1.1.7/deepqt/file_table.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/glossary.py` & `deepqt-1.1.7/deepqt/glossary.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/helpers.py` & `deepqt-1.1.7/deepqt/helpers.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/main.py` & `deepqt-1.1.7/deepqt/main.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/quote_protection.py` & `deepqt-1.1.7/deepqt/quote_protection.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/rc_generated_files/fallback_icons_rc.py` & `deepqt-1.1.7/deepqt/rc_generated_files/fallback_icons_rc.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/structures.py` & `deepqt-1.1.7/deepqt/structures.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/term_extractor.py` & `deepqt-1.1.7/deepqt/term_extractor.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/trie.py` & `deepqt-1.1.7/deepqt/trie.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/ui_generated_files/ui_api_config.py` & `deepqt-1.1.7/deepqt/ui_generated_files/ui_api_config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/ui_generated_files/ui_epub_preview.py` & `deepqt-1.1.7/deepqt/ui_generated_files/ui_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/ui_generated_files/ui_mainwindow.py` & `deepqt-1.1.7/deepqt/ui_generated_files/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/ui_generated_files/ui_text_preview.py` & `deepqt-1.1.7/deepqt/ui_generated_files/ui_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/worker_thread.py` & `deepqt-1.1.7/deepqt/worker_thread.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt/xml_parser.py` & `deepqt-1.1.7/deepqt/xml_parser.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/deepqt.egg-info/PKG-INFO` & `deepqt-1.1.7/deepqt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.6
+Version: 1.1.7
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.6/deepqt.egg-info/SOURCES.txt` & `deepqt-1.1.7/deepqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.6/setup.cfg` & `deepqt-1.1.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepqt
-version = 1.1.6
+version = 1.1.7
 description = Harness the power of the DeepL API with this friendly user interface.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/VoxelCubes/DeepQt
 keywords = deepl, deepl api, qt, pyside6
 license_files = LICENSE
 classifiers =
```

