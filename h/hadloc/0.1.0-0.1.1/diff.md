# Comparing `tmp/hadloc-0.1.0.tar.gz` & `tmp/hadloc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadloc-0.1.0.tar", last modified: Sun Apr 23 02:23:53 2023, max compression
+gzip compressed data, was "hadloc-0.1.1.tar", last modified: Sun Apr 23 08:06:09 2023, max compression
```

## Comparing `hadloc-0.1.0.tar` & `hadloc-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-23 02:23:50.000000 hadloc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 02:23:50.000000 hadloc-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-23 02:23:53.192225 hadloc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-23 02:23:50.000000 hadloc-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.188225 hadloc-0.1.0/hadloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19849 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/codewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/assembler/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    61132 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/compiler/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/compiler/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/emulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/emulator/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/emulator/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/emulator/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/emulator/word.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/grammar/abstract_syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/grammar/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/grammar/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/grammar/token_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/text_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/text_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/text_utils/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/text_utils/code_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/text_utils/positioned_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.192225 hadloc-0.1.0/hadloc/translator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/codewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/parser_errors.json
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/translator/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-23 02:23:50.000000 hadloc-0.1.0/hadloc/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:23:53.188225 hadloc-0.1.0/hadloc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 02:23:53.000000 hadloc-0.1.0/hadloc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 02:23:53.192225 hadloc-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-23 02:23:51.000000 hadloc-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-23 08:06:07.000000 hadloc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 08:06:07.000000 hadloc-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-23 08:06:09.324705 hadloc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-23 08:06:07.000000 hadloc-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.320705 hadloc-0.1.1/hadloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19849 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/codewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/assembler/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61132 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/compiler/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/compiler/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/emulator/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/emulator/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/emulator/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/emulator/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/grammar/abstract_syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/grammar/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/grammar/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/grammar/token_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/text_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/text_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/text_utils/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/text_utils/code_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/text_utils/positioned_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.324705 hadloc-0.1.1/hadloc/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/codewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/parser_errors.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/translator/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-23 08:06:07.000000 hadloc-0.1.1/hadloc/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:06:09.320705 hadloc-0.1.1/hadloc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 08:06:09.000000 hadloc-0.1.1/hadloc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 08:06:09.324705 hadloc-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-23 08:06:07.000000 hadloc-0.1.1/setup.py
```

### Comparing `hadloc-0.1.0/LICENSE` & `hadloc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/PKG-INFO` & `hadloc-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: hadloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool to build, emulate and load programs for the HaDLOC 8-bit computer
 Home-page: https://github.com/nicholasprowse/HADLoC
 Author: Nic Prowse
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: Console :: Curses
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Assemblers
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HaDLOC
 Command line tool containing several utilities for HADLoC.
```

### Comparing `hadloc-0.1.0/README.md` & `hadloc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/__main__.py` & `hadloc-0.1.1/hadloc/__main__.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/assembler/codewriter.py` & `hadloc-0.1.1/hadloc/assembler/codewriter.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/assembler/label_encoder.py` & `hadloc-0.1.1/hadloc/assembler/label_encoder.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/assembler/parser.py` & `hadloc-0.1.1/hadloc/assembler/parser.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/assembler/tokenizer.py` & `hadloc-0.1.1/hadloc/assembler/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/compiler/compiler.py` & `hadloc-0.1.1/hadloc/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/compiler/parser.py` & `hadloc-0.1.1/hadloc/compiler/parser.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/compiler/tokenizer.py` & `hadloc-0.1.1/hadloc/compiler/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/emulator/disassembler.py` & `hadloc-0.1.1/hadloc/emulator/disassembler.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/emulator/display.py` & `hadloc-0.1.1/hadloc/emulator/display.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/emulator/emulator.py` & `hadloc-0.1.1/hadloc/emulator/emulator.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/emulator/word.py` & `hadloc-0.1.1/hadloc/emulator/word.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/error.py` & `hadloc-0.1.1/hadloc/error.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/grammar/abstract_syntax_tree.py` & `hadloc-0.1.1/hadloc/grammar/abstract_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/grammar/grammar.py` & `hadloc-0.1.1/hadloc/grammar/grammar.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/text_utils/code.py` & `hadloc-0.1.1/hadloc/text_utils/code.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/text_utils/code_object.py` & `hadloc-0.1.1/hadloc/text_utils/code_object.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/text_utils/positioned_string.py` & `hadloc-0.1.1/hadloc/text_utils/positioned_string.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/translator/codewriter.py` & `hadloc-0.1.1/hadloc/translator/codewriter.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/translator/parser.py` & `hadloc-0.1.1/hadloc/translator/parser.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/translator/parser_errors.json` & `hadloc-0.1.1/hadloc/translator/parser_errors.json`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/translator/tokenizer.py` & `hadloc-0.1.1/hadloc/translator/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/utils.py` & `hadloc-0.1.1/hadloc/utils.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc/writer.py` & `hadloc-0.1.1/hadloc/writer.py`

 * *Files identical despite different names*

### Comparing `hadloc-0.1.0/hadloc.egg-info/PKG-INFO` & `hadloc-0.1.1/hadloc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: hadloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool to build, emulate and load programs for the HaDLOC 8-bit computer
 Home-page: https://github.com/nicholasprowse/HADLoC
 Author: Nic Prowse
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: Console :: Curses
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Assemblers
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HaDLOC
 Command line tool containing several utilities for HADLoC.
```

### Comparing `hadloc-0.1.0/hadloc.egg-info/SOURCES.txt` & `hadloc-0.1.1/hadloc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

