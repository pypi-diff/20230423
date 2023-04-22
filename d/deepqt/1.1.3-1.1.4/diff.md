# Comparing `tmp/deepqt-1.1.3.tar.gz` & `tmp/deepqt-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepqt-1.1.3.tar", last modified: Fri Apr 14 15:59:17 2023, max compression
+gzip compressed data, was "deepqt-1.1.4.tar", last modified: Sat Apr 22 22:44:02 2023, max compression
```

## Comparing `deepqt-1.1.3.tar` & `deepqt-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.3/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-14 15:59:17.837984 deepqt-1.1.3/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.3/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.834651 deepqt-1.1.3/deepqt/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.3/deepqt/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.3/deepqt/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.3/deepqt/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-14 15:57:00.000000 deepqt-1.1.3/deepqt/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18001 2022-10-03 22:02:43.000000 deepqt-1.1.3/deepqt/api_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5701 2023-04-14 15:55:16.000000 deepqt-1.1.3/deepqt/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1706 2022-10-14 20:43:00.000000 deepqt-1.1.3/deepqt/driver_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/driver_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    34986 2023-04-03 00:53:22.000000 deepqt-1.1.3/deepqt/driver_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/driver_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.3/deepqt/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7574 2022-11-29 16:04:36.000000 deepqt-1.1.3/deepqt/glossary.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6260 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.3/deepqt/main.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.3/deepqt/quote_protection.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.3/deepqt/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/rc_generated_files/fallback_icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.3/deepqt/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/term_extractor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.3/deepqt/trie.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.3/deepqt/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2579 2022-10-14 20:41:09.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/worker_thread.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/xml_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.3/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-14 15:59:17.837984 deepqt-1.1.3/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.3/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.954064 deepqt-1.1.4/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.4/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-22 22:44:02.954064 deepqt-1.1.4/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.4/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.950730 deepqt-1.1.4/deepqt/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.954064 deepqt-1.1.4/deepqt/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.4/deepqt/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.4/deepqt/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.4/deepqt/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-22 22:42:23.000000 deepqt-1.1.4/deepqt/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19121 2023-04-22 22:39:27.000000 deepqt-1.1.4/deepqt/api_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5755 2023-04-22 22:39:05.000000 deepqt-1.1.4/deepqt/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2171 2023-04-22 21:12:39.000000 deepqt-1.1.4/deepqt/driver_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/driver_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35067 2023-04-22 21:38:56.000000 deepqt-1.1.4/deepqt/driver_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/driver_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.4/deepqt/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8040 2023-04-22 21:40:28.000000 deepqt-1.1.4/deepqt/glossary.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6260 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.4/deepqt/main.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.4/deepqt/quote_protection.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.954064 deepqt-1.1.4/deepqt/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.4/deepqt/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/rc_generated_files/fallback_icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.4/deepqt/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/term_extractor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.4/deepqt/trie.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.954064 deepqt-1.1.4/deepqt/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.4/deepqt/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3497 2023-04-22 21:01:56.000000 deepqt-1.1.4/deepqt/ui_generated_files/ui_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.4/deepqt/ui_generated_files/ui_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/ui_generated_files/ui_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.4/deepqt/ui_generated_files/ui_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/worker_thread.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.4/deepqt/xml_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-22 22:44:02.950730 deepqt-1.1.4/deepqt.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-22 22:44:02.000000 deepqt-1.1.4/deepqt.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.4/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-22 22:44:02.957397 deepqt-1.1.4/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.4/setup.py
```

### Comparing `deepqt-1.1.3/LICENSE` & `deepqt-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/PKG-INFO` & `deepqt-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.3
+Version: 1.1.4
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.3/README.md` & `deepqt-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/CustomQ/CComboBox.py` & `deepqt-1.1.4/deepqt/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/CustomQ/CTableWidget.py` & `deepqt-1.1.4/deepqt/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/api_interface.py` & `deepqt-1.1.4/deepqt/api_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import deepqt.quote_protection as qp
 import deepqt.structures as st
 import deepqt.worker_thread as wt
 import deepqt.xml_parser as xp
 
 
 # The DeepL API requires a limit of 128kB per request.
-# Use 100kB to be safe.
-API_MAX_BYTES = 100_000
+# Use 40kB to be safe. 70kB was apparently too much in some instances, despite the limit being set to 100kB.
+# API_MAX_BYTES = 100_000
+API_MAX_BYTES = 25_000
 
 
 class Abort(Exception):
     """
     Exception to abort the worker.
     """
 
@@ -267,14 +268,22 @@
 
                         if self.config.tl_mock:
                             translation = self.mock_translate_text(chunk, is_html=True)
                         else:
                             translation = self.try_translate(chunk, key, is_html=True)
 
                         translations.append(translation.text)
+                        
+                        self.check_aborted()
+                        self.signals.progress.emit(
+                            key,
+                            f"Translating file {i + 2} / {input_file.file_count}",  # +2 because of toc.ncx and 0-indexing.
+                            self.processed_chars,
+                            self.total_chars,
+                        )
 
                     html_file.translation = "".join(translations)
                     # logger.debug(f"Translation: {translation.text}")
                 self.signals.progress.emit(
                     key,
                     f"Translated file {input_file.file_count} / {input_file.file_count} ",
                     self.processed_chars,
@@ -292,15 +301,20 @@
         :param is_html: Whether the text is html or not.
         """
         tag_handling = "html" if is_html else None
         tries = 1
         while True:
             try:
                 if isinstance(chunk, str):
-                    logger.debug(f"Requesting translation of {len(chunk.encode('utf-8')):n} bytes.")
+                    logger.debug(f"Requesting translation of {len(chunk.encode('utf-8')):n} bytes, {len(chunk):n} chars.")
+                else:
+                    logger.debug(
+                        f"Requesting translation of {sum(len(c.encode('utf-8')) for c in chunk):n} bytes, "
+                        f"{sum(len(c) for c in chunk):n} chars, split into {len(chunk)} chunks."
+                    )
                 t_start = time.time()
                 translation = self.translator.translate_text(
                     chunk,
                     source_lang=self.config.lang_from,
                     target_lang=self.config.lang_to,
                     preserve_formatting=self.config.tl_preserve_formatting,
                     tag_handling=tag_handling,
@@ -353,15 +367,21 @@
         """
         Mock translation.
 
         :param chunk: The text to translate.
         :param is_html: Whether the text is html or not.
         """
         logger.info("Mocking translation.")
-        logger.debug(f"Requesting translation of {len(chunk.encode('utf-8')):n} bytes.")
+        if isinstance(chunk, str):
+            logger.debug(f"Requesting translation of {len(chunk.encode('utf-8')):n} bytes, {len(chunk):n} chars.")
+        else:
+            logger.debug(
+                f"Requesting translation of {sum(len(c.encode('utf-8')) for c in chunk):n} bytes, "
+                f"{sum(len(c) for c in chunk):n} chars, split into {len(chunk)} chunks."
+            )
         time.sleep(1)
         if isinstance(chunk, list):
             return [deepl.TextResult(text="Translated " + text, detected_source_lang="EN") for text in chunk]
         else:
             translation = deepl.TextResult(text="Translated" + chunk, detected_source_lang="EN")
         # Pretend that we make progress.
         if is_html:
```

### Comparing `deepqt-1.1.3/deepqt/config.py` & `deepqt-1.1.4/deepqt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     fixed_output_path: str
 
     glossary_path: str
     use_glossary: bool
     use_quote_protection: bool
 
     api_key: str
+    is_pro_version: bool
 
     # Advanced options.
     tl_max_chunks: int
     tl_min_chunk_size: int
     tl_preserve_formatting: bool
     tl_mock: bool
     dump_on_abort: bool
@@ -158,16 +159,17 @@
         lang_to="",
         use_fixed_output_path=False,
         fixed_output_path="",
         glossary_path="",
         use_glossary=True,
         use_quote_protection=True,
         api_key="",
+        is_pro_version=False,
         tl_max_chunks=20,
-        tl_min_chunk_size=10_000,
+        tl_min_chunk_size=5_000,
         tl_preserve_formatting=True,
         tl_mock=False,
         dump_on_abort=True,
         epub_nuke_kobo=True,
         epub_nuke_ruby=True,
         epub_nuke_indents=True,
         epub_make_text_horizontal=True,
```

### Comparing `deepqt-1.1.3/deepqt/driver_api_config.py` & `deepqt-1.1.4/deepqt/driver_api_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import PySide6.QtWidgets as Qw
 
 import deepqt.config as cfg
 from deepqt.ui_generated_files.ui_api_config import Ui_Dialog_API
 from deepqt.helpers import show_info
 
 
@@ -16,14 +17,27 @@
         self.setupUi(self)
 
         self.lineEdit_api_key.setText(config.api_key)
         self.lineEdit_api_key.setFocus()
 
         self.buttonBox.helpRequested.connect(self.show_api_help)
 
+        self.comboBox_api_type.setCurrentIndex(1 if config.is_pro_version else 0)
+
+    def get_key(self):
+        """
+        If the api is supposed to be PRO, remove :fx from the key and vice versa.
+        """
+        key = self.lineEdit_api_key.text().strip()
+        if self.comboBox_api_type.currentIndex() == 1:
+            key = re.sub(":fx$", "", key)
+        else:
+            key = re.sub("^(.*?)(:fx)?$", r"\1:fx", key)
+        return key
+    
     def show_api_help(self):
         """
         Show the deepl api documentation in a web browser.
         Open the github page for this.
         """
         show_info(
             self,
```

### Comparing `deepqt-1.1.3/deepqt/driver_epub_preview.py` & `deepqt-1.1.4/deepqt/driver_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/driver_mainwindow.py` & `deepqt-1.1.4/deepqt/driver_mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,16 @@
         """
         Configure the DeepL API.
         """
         api_conf_dialog = ConfigureAccount(self, self.config)
         response = api_conf_dialog.exec()
         if response == Qw.QDialog.Accepted:
             # Adopt changes from the dialog.
-            self.config.api_key = api_conf_dialog.lineEdit_api_key.text()
+            self.config.api_key = api_conf_dialog.get_key()
+            self.config.is_pro_version = api_conf_dialog.comboBox_api_type.currentIndex() == 1
             self.config.save()
             self.load_config_to_ui()
 
     """
     Misc helpers
     """
```

### Comparing `deepqt-1.1.3/deepqt/driver_text_preview.py` & `deepqt-1.1.4/deepqt/driver_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/file_table.py` & `deepqt-1.1.4/deepqt/file_table.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/glossary.py` & `deepqt-1.1.4/deepqt/glossary.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 import pyexcel_xlsx
 import pyexcel_htmlr
 from logzero import logger
 
 import deepqt.structures as st
 
 
+class UnsupportedFileType(Exception):
+    """
+    Exception raised when an unsupported file type is encountered.
+    """
+
+    pass
+
 def make_imports_used_so_they_dont_get_auto_removed():
     # Never call this function.
     # It purely serves to distract the linter from removing the imports,
     # so that they get included in pyinstaller builds.
     pyexcel_io.io.get_data()
     pyexcel_odsr.get_data()
     pyexcel_xls.get_data()
@@ -91,15 +98,20 @@
     Parse an ods file into a glossary.
     Exceptions need to be handled by the caller.
 
     :param path: The ods file to parse.
     :param glossary: The glossary structure to write into.
     """
 
-    workbook = pyexcel.get_book_dict(file_name=str(path))
+    try:
+        workbook = pyexcel.get_book_dict(file_name=str(path))
+    except pyexcel.exceptions.FileTypeNotSupported:
+        logger.error(f"File type not supported for: {path}")
+        raise UnsupportedFileType(f"File type '{path.suffix}' not supported for: {path}\n\n"
+                                  f"Glossaries are expected to be spreadsheets in .ods, .xlsx, .csv etc. format.")
 
     # Pyexcel inserts comment text into cells, which we need to remove using the comment pattern.
     pattern = re.compile(r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}.*?\n")
 
     for sheet in workbook.values():
 
         for row in sheet:
```

### Comparing `deepqt-1.1.3/deepqt/helpers.py` & `deepqt-1.1.4/deepqt/helpers.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/main.py` & `deepqt-1.1.4/deepqt/main.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/quote_protection.py` & `deepqt-1.1.4/deepqt/quote_protection.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/rc_generated_files/fallback_icons_rc.py` & `deepqt-1.1.4/deepqt/rc_generated_files/fallback_icons_rc.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/structures.py` & `deepqt-1.1.4/deepqt/structures.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/term_extractor.py` & `deepqt-1.1.4/deepqt/term_extractor.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/trie.py` & `deepqt-1.1.4/deepqt/trie.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/ui_generated_files/ui_epub_preview.py` & `deepqt-1.1.4/deepqt/ui_generated_files/ui_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/ui_generated_files/ui_mainwindow.py` & `deepqt-1.1.4/deepqt/ui_generated_files/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/ui_generated_files/ui_text_preview.py` & `deepqt-1.1.4/deepqt/ui_generated_files/ui_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/worker_thread.py` & `deepqt-1.1.4/deepqt/worker_thread.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt/xml_parser.py` & `deepqt-1.1.4/deepqt/xml_parser.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/deepqt.egg-info/PKG-INFO` & `deepqt-1.1.4/deepqt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.3
+Version: 1.1.4
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.3/deepqt.egg-info/SOURCES.txt` & `deepqt-1.1.4/deepqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.3/setup.cfg` & `deepqt-1.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepqt
-version = 1.1.3
+version = 1.1.4
 description = Harness the power of the DeepL API with this friendly user interface.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/VoxelCubes/DeepQt
 keywords = deepl, deepl api, qt, pyside6
 license_files = LICENSE
 classifiers =
```

