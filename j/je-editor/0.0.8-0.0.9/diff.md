# Comparing `tmp/je_editor-0.0.8.tar.gz` & `tmp/je_editor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_editor-0.0.8.tar", last modified: Sat Sep  4 13:56:25 2021, max compression
+gzip compressed data, was "dist\je_editor-0.0.9.tar", last modified: Sat Sep  4 14:08:51 2021, max compression
```

## Comparing `je_editor-0.0.8.tar` & `je_editor-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/
--rw-rw-rw-   0        0        0     1084 2021-07-27 15:59:34.000000 je_editor-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1476 2021-09-04 13:56:25.000000 je_editor-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      822 2021-08-29 10:01:10.000000 je_editor-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/
--rw-rw-rw-   0        0        0       54 2021-08-31 18:23:15.000000 je_editor-0.0.8/je_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/ui/
--rw-rw-rw-   0        0        0       28 2021-07-27 21:06:38.000000 je_editor-0.0.8/je_editor/ui/__init__.py
--rw-rw-rw-   0        0        0     8076 2021-09-04 13:54:28.000000 je_editor-0.0.8/je_editor/ui/tkinter_editor.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/
--rw-rw-rw-   0        0        0       31 2021-07-27 21:06:38.000000 je_editor-0.0.8/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/code_tag/
--rw-rw-rw-   0        0        0        0 2021-08-28 10:32:00.000000 je_editor-0.0.8/je_editor/utils/code_tag/__init__.py
--rw-rw-rw-   0        0        0       65 2021-08-29 10:24:32.000000 je_editor-0.0.8/je_editor/utils/code_tag/keyword_list.py
--rw-rw-rw-   0        0        0     1349 2021-09-01 14:06:56.000000 je_editor-0.0.8/je_editor/utils/code_tag/tag_keyword.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/editor_content/
--rw-rw-rw-   0        0        0       46 2021-08-02 03:41:58.000000 je_editor-0.0.8/je_editor/utils/editor_content/__init__.py
--rw-rw-rw-   0        0        0     1325 2021-08-31 09:42:51.000000 je_editor-0.0.8/je_editor/utils/editor_content/content_save.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/exception/
--rw-rw-rw-   0        0        0       41 2021-07-30 21:21:05.000000 je_editor-0.0.8/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      413 2021-08-03 14:08:05.000000 je_editor-0.0.8/je_editor/utils/exception/je_editor_exception_tag.py
--rw-rw-rw-   0        0        0     1600 2021-08-03 14:21:22.000000 je_editor-0.0.8/je_editor/utils/exception/je_editor_exceptions.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/file/
--rw-rw-rw-   0        0        0       36 2021-07-31 00:44:48.000000 je_editor-0.0.8/je_editor/utils/file/__init__.py
--rw-rw-rw-   0        0        0     1025 2021-09-04 13:51:29.000000 je_editor-0.0.8/je_editor/utils/file/open_file.py
--rw-rw-rw-   0        0        0     1705 2021-09-04 13:54:28.000000 je_editor-0.0.8/je_editor/utils/file/save_file.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/string_translate/
--rw-rw-rw-   0        0        0        0 2021-08-31 08:37:16.000000 je_editor-0.0.8/je_editor/utils/string_translate/__init__.py
--rw-rw-rw-   0        0        0        0 2021-08-31 08:37:26.000000 je_editor-0.0.8/je_editor/utils/string_translate/used_string.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/text_process/
--rw-rw-rw-   0        0        0       44 2021-07-30 21:49:48.000000 je_editor-0.0.8/je_editor/utils/text_process/__init__.py
--rw-rw-rw-   0        0        0      444 2021-08-31 11:45:46.000000 je_editor-0.0.8/je_editor/utils/text_process/exec_text.py
--rw-rw-rw-   0        0        0      296 2021-08-31 11:44:13.000000 je_editor-0.0.8/je_editor/utils/text_process/shell_text.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor/utils/theme/
--rw-rw-rw-   0        0        0        0 2021-09-02 08:09:26.000000 je_editor-0.0.8/je_editor/utils/theme/__init__.py
--rw-rw-rw-   0        0        0       61 2021-09-02 08:09:26.000000 je_editor-0.0.8/je_editor/utils/theme/theme.py
-drwxrwxrwx   0        0        0        0 2021-09-04 13:56:25.000000 je_editor-0.0.8/je_editor.egg-info/
--rw-rw-rw-   0        0        0     1476 2021-09-04 13:56:22.000000 je_editor-0.0.8/je_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2021-09-04 13:56:22.000000 je_editor-0.0.8/je_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-04 13:56:22.000000 je_editor-0.0.8/je_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-09-04 13:56:22.000000 je_editor-0.0.8/je_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-04 13:56:25.000000 je_editor-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      900 2021-09-04 13:54:28.000000 je_editor-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2021-07-27 15:59:34.000000 je_editor-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1476 2021-09-04 14:08:51.000000 je_editor-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2021-08-29 10:01:10.000000 je_editor-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/
+-rw-rw-rw-   0        0        0       54 2021-08-31 18:23:15.000000 je_editor-0.0.9/je_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/ui/
+-rw-rw-rw-   0        0        0       28 2021-07-27 21:06:38.000000 je_editor-0.0.9/je_editor/ui/__init__.py
+-rw-rw-rw-   0        0        0     8282 2021-09-04 14:05:47.000000 je_editor-0.0.9/je_editor/ui/tkinter_editor.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/utils/
+-rw-rw-rw-   0        0        0       31 2021-07-27 21:06:38.000000 je_editor-0.0.9/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/utils/code_tag/
+-rw-rw-rw-   0        0        0        0 2021-08-28 10:32:00.000000 je_editor-0.0.9/je_editor/utils/code_tag/__init__.py
+-rw-rw-rw-   0        0        0       65 2021-08-29 10:24:32.000000 je_editor-0.0.9/je_editor/utils/code_tag/keyword_list.py
+-rw-rw-rw-   0        0        0     1349 2021-09-01 14:06:56.000000 je_editor-0.0.9/je_editor/utils/code_tag/tag_keyword.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/editor_content/
+-rw-rw-rw-   0        0        0       46 2021-08-02 03:41:58.000000 je_editor-0.0.9/je_editor/utils/editor_content/__init__.py
+-rw-rw-rw-   0        0        0     1325 2021-08-31 09:42:51.000000 je_editor-0.0.9/je_editor/utils/editor_content/content_save.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0       41 2021-07-30 21:21:05.000000 je_editor-0.0.9/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      413 2021-08-03 14:08:05.000000 je_editor-0.0.9/je_editor/utils/exception/je_editor_exception_tag.py
+-rw-rw-rw-   0        0        0     1600 2021-08-03 14:21:22.000000 je_editor-0.0.9/je_editor/utils/exception/je_editor_exceptions.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/file/
+-rw-rw-rw-   0        0        0       36 2021-07-31 00:44:48.000000 je_editor-0.0.9/je_editor/utils/file/__init__.py
+-rw-rw-rw-   0        0        0     1025 2021-09-04 13:51:29.000000 je_editor-0.0.9/je_editor/utils/file/open_file.py
+-rw-rw-rw-   0        0        0     1705 2021-09-04 13:54:28.000000 je_editor-0.0.9/je_editor/utils/file/save_file.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/string_translate/
+-rw-rw-rw-   0        0        0        0 2021-08-31 08:37:16.000000 je_editor-0.0.9/je_editor/utils/string_translate/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-08-31 08:37:26.000000 je_editor-0.0.9/je_editor/utils/string_translate/used_string.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/text_process/
+-rw-rw-rw-   0        0        0       44 2021-07-30 21:49:48.000000 je_editor-0.0.9/je_editor/utils/text_process/__init__.py
+-rw-rw-rw-   0        0        0      444 2021-08-31 11:45:46.000000 je_editor-0.0.9/je_editor/utils/text_process/exec_text.py
+-rw-rw-rw-   0        0        0      296 2021-08-31 11:44:13.000000 je_editor-0.0.9/je_editor/utils/text_process/shell_text.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/theme/
+-rw-rw-rw-   0        0        0        0 2021-09-02 08:09:26.000000 je_editor-0.0.9/je_editor/utils/theme/__init__.py
+-rw-rw-rw-   0        0        0       61 2021-09-02 08:09:26.000000 je_editor-0.0.9/je_editor/utils/theme/theme.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor.egg-info/
+-rw-rw-rw-   0        0        0     1476 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-09-04 14:08:51.000000 je_editor-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      900 2021-09-04 14:08:12.000000 je_editor-0.0.9/setup.py
```

### Comparing `je_editor-0.0.8/LICENSE` & `je_editor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/PKG-INFO` & `je_editor-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple editor
 Home-page: https://github.com/JE-Chen/je_editor
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_editor-0.0.8/README.md` & `je_editor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor/ui/tkinter_editor.py` & `je_editor-0.0.9/je_editor/ui/tkinter_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,27 @@
     def open_file_to_read(self, event=None):
         temp_to_check_file = open_file()
         if temp_to_check_file is not None and temp_to_check_file != "":
             self.file_to_output_content = temp_to_check_file[0]
             self.code_editor.delete(self.start_position, self.end_position)
             self.code_editor.insert(self.end_position, temp_to_check_file[1])
             self.current_file = temp_to_check_file[0]
-            if self.current_file is not None and self.auto_save is None:
+            if self.auto_save is not None:
+                self.auto_save.file = self.current_file
+            elif self.current_file is not None and self.auto_save is None:
                 self.auto_save = SaveThread(self.current_file, self.code_editor)
                 self.auto_save.start()
 
     def save_file_to_open(self, event=None):
         temp_to_check_file = save_file(self.code_editor.get(self.start_position, self.end_position))
         if temp_to_check_file is not None and temp_to_check_file != "":
             self.current_file = temp_to_check_file[0]
-            if self.current_file is not None and self.auto_save is None:
+            if self.auto_save is not None:
+                self.auto_save.file = self.current_file
+            elif self.current_file is not None and self.auto_save is None:
                 self.auto_save = SaveThread(self.current_file, self.code_editor)
                 self.auto_save.start()
 
     def open_last_edit_file(self):
         temp_to_check_file = read_file(self.file_to_output_content)
         if temp_to_check_file is not None:
             self.code_editor.delete(self.start_position, self.end_position)
```

### Comparing `je_editor-0.0.8/je_editor/utils/code_tag/tag_keyword.py` & `je_editor-0.0.9/je_editor/utils/code_tag/tag_keyword.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor/utils/editor_content/content_save.py` & `je_editor-0.0.9/je_editor/utils/editor_content/content_save.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor/utils/exception/je_editor_exceptions.py` & `je_editor-0.0.9/je_editor/utils/exception/je_editor_exceptions.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor/utils/file/open_file.py` & `je_editor-0.0.9/je_editor/utils/file/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor/utils/file/save_file.py` & `je_editor-0.0.9/je_editor/utils/file/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/je_editor.egg-info/PKG-INFO` & `je_editor-0.0.9/je_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple editor
 Home-page: https://github.com/JE-Chen/je_editor
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_editor-0.0.8/je_editor.egg-info/SOURCES.txt` & `je_editor-0.0.9/je_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor-0.0.8/setup.py` & `je_editor-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_editor",
-    version="0.0.8",
+    version="0.0.9",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="simple editor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/je_editor",
     packages=setuptools.find_packages(),
```

