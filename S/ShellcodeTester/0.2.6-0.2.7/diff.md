# Comparing `tmp/ShellcodeTester-0.2.6.tar.gz` & `tmp/ShellcodeTester-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.6.tar", last modified: Fri Apr 14 23:56:52 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.7.tar", last modified: Sun Apr 23 00:00:44 2023, max compression
```

## Comparing `ShellcodeTester-0.2.6.tar` & `ShellcodeTester-0.2.7.tar`

### file list

```diff
@@ -1,62 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.934079 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 23:56:52.000000 ShellcodeTester-0.2.6/ShellcodeTester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.934079 ShellcodeTester-0.2.6/nasmshell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.934079 ShellcodeTester-0.2.6/nasmshell/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/libs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/nasmshell/nasmshell.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.934079 ShellcodeTester-0.2.6/shell_bins/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:48.000000 ShellcodeTester-0.2.6/shell_bins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.938079 ShellcodeTester-0.2.6/shell_bins/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:48.000000 ShellcodeTester-0.2.6/shell_bins/linux/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1951840 2023-04-14 23:55:57.000000 ShellcodeTester-0.2.6/shell_bins/linux/nasm
--rw-r--r--   0 runner    (1001) docker     (123) 12329280 2023-04-14 23:55:47.000000 ShellcodeTester-0.2.6/shell_bins/linux/objdump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.950080 ShellcodeTester-0.2.6/shell_bins/macosx/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:48.000000 ShellcodeTester-0.2.6/shell_bins/macosx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  3237896 2023-04-14 23:55:57.000000 ShellcodeTester-0.2.6/shell_bins/macosx/nasm
--rw-r--r--   0 runner    (1001) docker     (123)   167120 2023-04-14 23:55:47.000000 ShellcodeTester-0.2.6/shell_bins/macosx/objdump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.954080 ShellcodeTester-0.2.6/shell_bins/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:56:48.000000 ShellcodeTester-0.2.6/shell_bins/windows/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1638912 2023-04-14 23:55:57.000000 ShellcodeTester-0.2.6/shell_bins/windows/nasm.exe
--rwxr-xr-x   0 runner    (1001) docker     (123)  2410600 2023-04-14 23:55:55.000000 ShellcodeTester-0.2.6/shell_bins/windows/objdump.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/shell_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/inlineassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shell_libs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:52.958080 ShellcodeTester-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 23:56:47.000000 ShellcodeTester-0.2.6/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.926153 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 00:00:44.000000 ShellcodeTester-0.2.7/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shell_bins/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:33.000000 ShellcodeTester-0.2.7/shell_bins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shell_bins/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:33.000000 ShellcodeTester-0.2.7/shell_bins/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shell_bins/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:33.000000 ShellcodeTester-0.2.7/shell_bins/macosx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shell_bins/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:00:33.000000 ShellcodeTester-0.2.7/shell_bins/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:44.930153 ShellcodeTester-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-23 00:00:31.000000 ShellcodeTester-0.2.7/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.6/LICENSE` & `ShellcodeTester-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/PKG-INFO` & `ShellcodeTester-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.6
+Version: 0.2.7
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.6/README.md` & `ShellcodeTester-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.7/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.6
+Version: 0.2.7
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.6/ShellcodeTester.egg-info/SOURCES.txt` & `ShellcodeTester-0.2.7/ShellcodeTester.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,22 +14,16 @@
 nasmshell/args.py
 nasmshell/config.py
 nasmshell/nasmshell.py
 nasmshell/libs/__init__.py
 nasmshell/libs/cmd.py
 shell_bins/__init__.py
 shell_bins/linux/__init__.py
-shell_bins/linux/nasm
-shell_bins/linux/objdump
 shell_bins/macosx/__init__.py
-shell_bins/macosx/nasm
-shell_bins/macosx/objdump
 shell_bins/windows/__init__.py
-shell_bins/windows/nasm.exe
-shell_bins/windows/objdump.exe
 shell_libs/__init__.py
 shell_libs/__meta__.py
 shell_libs/asmfile.py
 shell_libs/assembler.py
 shell_libs/color.py
 shell_libs/compiler.py
 shell_libs/disassembler.py
```

### Comparing `ShellcodeTester-0.2.6/nasmshell/args.py` & `ShellcodeTester-0.2.7/nasmshell/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/nasmshell/config.py` & `ShellcodeTester-0.2.7/nasmshell/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/nasmshell/libs/cmd.py` & `ShellcodeTester-0.2.7/nasmshell/libs/cmd.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/nasmshell/nasmshell.py` & `ShellcodeTester-0.2.7/nasmshell/nasmshell.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/setup.py` & `ShellcodeTester-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/asmfile.py` & `ShellcodeTester-0.2.7/shell_libs/asmfile.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/assembler.py` & `ShellcodeTester-0.2.7/shell_libs/assembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/color.py` & `ShellcodeTester-0.2.7/shell_libs/color.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/disassembler.py` & `ShellcodeTester-0.2.7/shell_libs/disassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/inlineassembler.py` & `ShellcodeTester-0.2.7/shell_libs/inlineassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/logger.py` & `ShellcodeTester-0.2.7/shell_libs/logger.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/process.py` & `ShellcodeTester-0.2.7/shell_libs/process.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/runner.py` & `ShellcodeTester-0.2.7/shell_libs/runner.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/tools.py` & `ShellcodeTester-0.2.7/shell_libs/tools.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shell_libs/transform.py` & `ShellcodeTester-0.2.7/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shellcodetester/args.py` & `ShellcodeTester-0.2.7/shellcodetester/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 
         custom.add_argument('--fill-with-nop',
                             action='store_true',
                             default=False,
                             dest='fill',
                             help=Color.s('Fill entire page with NOP (default: {G}false{W})'))
 
+        custom.add_argument('--writable-text',
+                            action='store_true',
+                            default=False,
+                            dest='writable_text',
+                            help=Color.s('Mark the output .text section as writable{W}'))
+
         custom.add_argument('--list',
                             action='store_true',
                             default=False,
                             dest='format_list',
                             help=Color.s('List all supported output format{W}'))
 
         custom.add_argument('-f',
```

### Comparing `ShellcodeTester-0.2.6/shellcodetester/config.py` & `ShellcodeTester-0.2.7/shellcodetester/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     platform = ''
     remove = False
     transform_format = 0
     breakpoint = False
     fill = False
     bad_chars = bytearray([0x00])
     cave_size = 200
+    writable_text = False
 
     @staticmethod
     def initialize():
         '''
             Sets up default initial configuration values.
             Also sets config values based on command-line arguments.
         '''
@@ -120,16 +121,18 @@
         if args.out_file:
             Configuration.out_file = args.out_file
 
         Configuration.cave_size = int(args.cave_size)
         Configuration.breakpoint = args.breakpoint
         Configuration.remove = args.remove
         Configuration.fill = args.fill
+        Configuration.writable_text = args.writable_text
         Configuration.transform_format = Transform.parse_format(args.transform_format)
 
+        Logger.pl('     {C}writable .text section:{O} %s{W}' % Configuration.writable_text)
         Logger.pl('     {C}code cave size:{O} %s{W}' % Configuration.cave_size)
         Logger.pl('     {C}transform format:{O} %s{W}' % (Transform.get_name(Configuration.transform_format)))
 
         if len(Configuration.bad_chars) > 0:
             Logger.pl('     {C}bad chars:{O} %s{W}' % (', '.join([
                 f"0x{format(x, '02x')}" for x in Configuration.bad_chars
             ])))
```

### Comparing `ShellcodeTester-0.2.6/shellcodetester/password.py` & `ShellcodeTester-0.2.7/shellcodetester/password.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.6/shellcodetester/shellcodetester.py` & `ShellcodeTester-0.2.7/shellcodetester/shellcodetester.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,19 @@
                 if len(asm.assembled_data) != len(fill_data):
                     Logger.pl('{!} {R}Bad chars found. {GR}Disassembly without bad chars{W}')
                     dis = Disassembler(filename='', assembled_data=fill_data, platform=Configuration.platform, arch=asm.arch)
                     dis.dump(Configuration.bad_chars, quiet=True)
 
             asm.print_payload(Configuration.transform_format, Configuration.bad_chars)
 
-            comp = Compiler(Configuration.asm_file, asm.assembled_data, Configuration.bad_chars, Configuration.remove)
+            comp = Compiler(Configuration.asm_file,
+                            asm.assembled_data,
+                            Configuration.bad_chars,
+                            Configuration.remove,
+                            Configuration.writable_text)
             if not comp.compile():
                 sys.exit(2)
 
         except Exception as e:
             Color.pl("\n{!} {R}Error: {O}%s" % str(e))
             if Configuration.verbose > 0 or True:
                 Color.pl('\n{!} {O}Full stack trace below')
```

