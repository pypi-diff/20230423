# Comparing `tmp/qemu-runner-1.3.1.tar.gz` & `tmp/qemu-runner-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qemu-runner-1.3.1.tar", last modified: Sat Apr 22 14:51:54 2023, max compression
+gzip compressed data, was "qemu-runner-1.3.2.tar", last modified: Sun Apr 23 18:11:20 2023, max compression
```

## Comparing `qemu-runner-1.3.1.tar` & `qemu-runner-1.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.940073 qemu-runner-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.948073 qemu-runner-1.3.1/src/qemu_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layer_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layers/virt-cortex-m.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner/make_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/variable_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.956073 qemu-runner-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_find_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_qemu_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_qemu_argument_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_runner_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_utllities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layer_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layers/virt-cortex-m.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/make_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/variable_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_find_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_qemu_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_qemu_argument_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_runner_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_utllities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_venv.py
```

### Comparing `qemu-runner-1.3.1/LICENSE.txt` & `qemu-runner-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/PKG-INFO` & `qemu-runner-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.1
+Version: 1.3.2
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.1/README.md` & `qemu-runner-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/setup.py` & `qemu-runner-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open(os.path.dirname(os.path.abspath(__file__)) + '/README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='qemu-runner',
-    version='1.3.1',
+    version='1.3.2',
     description='Create self-contained wrappers around QEMU to hide & share long command-line invocations',
     url='https://github.com/Novakov/qemu-runner',
     long_description=description,
     long_description_content_type='text/markdown',
     author='Maciej Nowak',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `qemu-runner-1.3.1/src/qemu_runner/argument.py` & `qemu-runner-1.3.2/src/qemu_runner/argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/find_qemu.py` & `qemu-runner-1.3.2/src/qemu_runner/find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/layer.py` & `qemu-runner-1.3.2/src/qemu_runner/layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/layer_locator.py` & `qemu-runner-1.3.2/src/qemu_runner/layer_locator.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/make_runner/__main__.py` & `qemu-runner-1.3.2/src/qemu_runner/make_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/make_runner/make.py` & `qemu-runner-1.3.2/src/qemu_runner/make_runner/make.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner/make_runner/runner.py` & `qemu-runner-1.3.2/src/qemu_runner/make_runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import subprocess
 import sys
 from configparser import ConfigParser
 from pathlib import Path
 from typing import List, Optional
 
 
+def make_path_absolute(v: str) -> str:
+    return os.path.abspath(v)
+
 def make_arg_parser():
     parser = argparse.ArgumentParser()
     parser.formatter_class = argparse.RawDescriptionHelpFormatter
 
     parser.description = '''QEMU runner wraps series of layers describing QEMU arguments as standalone executable file (ZIP file actually)
 requiring only Python 3.8+ standard library. 
 '''
@@ -57,15 +60,15 @@
     qemu_args = parser.add_argument_group('QEMU arguments')
     qemu_args.add_argument('--halted', action='store_true', help='Halt machine on startup')
     qemu_args.add_argument('--debug', action='store_true', help='Enable QEMU gdbserver')
     qemu_args.add_argument('--debug-listen', help='QEMU gdbserver listen address', metavar='device')
 
     program_args = parser.add_argument_group('Program arguments')
     program_args.add_argument('--dry-run', action='store_true', help='Do not execute QEMU, just output command line')
-    program_args.add_argument('kernel', help='Executable to run under QEMU', nargs='?')
+    program_args.add_argument('kernel', help='Executable to run under QEMU', nargs='?', type=make_path_absolute)
     program_args.add_argument('arguments', nargs=argparse.REMAINDER, help='Arguments passed to executable', default=[])
 
     return parser
 
 
 def make_layer_from_args(args: argparse.Namespace) -> 'Layer':
     from qemu_runner.layer import GeneralSettings, Layer
```

### Comparing `qemu-runner-1.3.1/src/qemu_runner/variable_resolution.py` & `qemu-runner-1.3.2/src/qemu_runner/variable_resolution.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/src/qemu_runner.egg-info/PKG-INFO` & `qemu-runner-1.3.2/src/qemu_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.1
+Version: 1.3.2
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.1/src/qemu_runner.egg-info/SOURCES.txt` & `qemu-runner-1.3.2/src/qemu_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_find_layer.py` & `qemu-runner-1.3.2/tests/test_find_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_find_qemu.py` & `qemu-runner-1.3.2/tests/test_find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_layer.py` & `qemu-runner-1.3.2/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_layer_cmdline.py` & `qemu-runner-1.3.2/tests/test_layer_cmdline.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_layer_equality.py` & `qemu-runner-1.3.2/tests/test_layer_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_layer_parsing.py` & `qemu-runner-1.3.2/tests/test_layer_parsing.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_qemu_argument.py` & `qemu-runner-1.3.2/tests/test_qemu_argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_qemu_argument_equality.py` & `qemu-runner-1.3.2/tests/test_qemu_argument_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_runner_flow.py` & `qemu-runner-1.3.2/tests/test_runner_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional, Union, Sequence, List
 
 import pytest
 
-from .test_utllities import place_echo_args, with_env
+from .test_utllities import place_echo_args, with_env, with_cwd
 
 CmdlineArg = Union[str, os.PathLike]
 
 
 def run_make_runner(*args: CmdlineArg, cwd: Optional[os.PathLike] = None) -> None:
     cp = subprocess.run(
         [sys.executable, '-m', 'qemu_runner.make_runner', *map(str, args)],
@@ -45,34 +45,36 @@
     ]
 
 
 def test_runner_flow(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
     run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
-    cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf', 'arg1', 'arg2')
+    with with_cwd(tmp_path):
+        cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf', 'arg1', 'arg2')
 
     assert cmdline == [
         engine,
         '-machine', 'virt_cortex_m,flash_kb=1024',
-        '-kernel', 'abc.elf',
+        '-kernel',  str(tmp_path / 'abc.elf'),
         '-append', 'arg1 arg2'
     ]
 
 
 def test_runner_flow_no_args(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
     run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
-    cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf')
+    with with_cwd(tmp_path):
+        cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf')
 
     assert cmdline == [
         engine,
         '-machine', 'virt_cortex_m,flash_kb=1024',
-        '-kernel', 'abc.elf',
+        '-kernel',  str(tmp_path / 'abc.elf'),
     ]
 
 
 def assert_arg_set_in_cmdline(arg_set: List[str], cmdline: List[str]):
     if len(arg_set) == 1:
         assert arg_set[0] in cmdline
     else:
@@ -131,20 +133,22 @@
         [device:test_id]
         @=test_device
         addr=12
         """)
 
     run_make_runner('-l', 'virt-cortex-m.ini', 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
-    with with_env({'QEMU_DEV': 'my-qemu'}):
+    with with_env({'QEMU_DEV': 'my-qemu'}), with_cwd(tmp_path):
         cp = execute_runner(tmp_path / 'test.pyz', ['--debug', '--dry-run', 'abc.elf', 'a', 'b', 'c'])
 
-    assert cp.stdout.strip() == (
+    kernel_path = tmp_path / 'abc.elf'
+
+    assert cp.stdout.strip().replace("-kernel '", '-kernel ').replace("' -append", ' -append') == (
             "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 " +
-            "-s -kernel abc.elf -append 'a b c'")
+            f"-s -kernel {kernel_path} -append 'a b c'")
 
 
 def test_extract_base_command_line_no_kernel(tmp_path: Path):
     with open(tmp_path / 'my-layer.ini', 'w') as f:
         f.write("""
         [device:test_id]
         @=test_device
@@ -180,21 +184,22 @@
     run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'base_runner.pyz', cwd=tmp_path)
 
     execute_runner(
         tmp_path / 'base_runner.pyz', ['--layers', './layer2.ini', '--derive', './derived.pyz'],
         cwd=tmp_path
     )
 
-    cmdline = capture_runner_cmdline(tmp_path / 'derived.pyz', 'abc.elf')
+    with with_cwd(tmp_path):
+        cmdline = capture_runner_cmdline(tmp_path / 'derived.pyz', 'abc.elf')
 
     assert cmdline == [
         engine,
         '-device', 'test,id=d1',
         '-device', 'test,id=d2',
-        '-kernel', 'abc.elf',
+        '-kernel', str(tmp_path / 'abc.elf'),
     ]
 
 
 def test_derive_keep_qemu_path(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'dir1' / 'qemu' / 'my-qemu')
 
     with open(tmp_path / 'layer1.ini', 'w') as f:
@@ -289,23 +294,23 @@
         engine = my-qemu
 
         [machine]
         @=test
         """)
 
     run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'runner.pyz', cwd=tmp_path)
-    with with_env({'QEMU_FLAGS': '-s -device test,id=2'}):
+    with with_env({'QEMU_FLAGS': '-s -device test,id=2'}), with_cwd(tmp_path):
         cmdline = capture_runner_cmdline(tmp_path / 'runner.pyz', 'abc.elf')
 
     assert cmdline == [
         engine,
         '-s',
         '-device', 'test,id=2',
         '-machine', 'test',
-        '-kernel', 'abc.elf'
+        '-kernel', str(tmp_path / 'abc.elf')
     ]
 
 
 def test_env_runner_flags(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'my-qemu')
 
     with open(tmp_path / 'layer1.ini', 'w') as f:
@@ -314,23 +319,23 @@
         engine = my-qemu
 
         [machine]
         @=test
         """)
 
     run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'runner.pyz', cwd=tmp_path)
-    with with_env({'QEMU_RUNNER_FLAGS': '--halted --debug'}):
+    with with_env({'QEMU_RUNNER_FLAGS': '--halted --debug'}), with_cwd(tmp_path):
         cmdline = capture_runner_cmdline(tmp_path / 'runner.pyz', 'abc.elf')
 
     assert cmdline == [
         engine,
         '-machine', 'test',
         '-S',
         '-s',
-        '-kernel', 'abc.elf',
+        '-kernel', str(tmp_path / 'abc.elf')
     ]
 
 
 @pytest.mark.parametrize('args', [
     ['--inspect', '--derive', 'abc.pyz'],
     ['--derive', 'abc.pyz', 'kernel.elf'],
     ['--derive', 'abc.pyz', 'kernel.elf', 'a', 'b'],
@@ -373,7 +378,36 @@
     engine = place_echo_args(tmp_path / 'my-qemu' / 'qemu')
 
     run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     args = capture_runner_cmdline(tmp_path / 'test.pyz', '--qemu', engine, 'abc.elf')
 
     assert args[0] == engine
+
+
+def test_resolve_kernel_dir_to_absolute_path(tmp_path: Path) -> None:
+    engine = place_echo_args(tmp_path / 'qemu' / 'my-qemu')
+
+    with open(tmp_path / 'layer1.ini', 'w') as f:
+        f.write("""
+            [general]
+            engine = my-qemu
+
+            [machine]
+            @=test
+            
+            [device]
+            @=path
+            value=${KERNEL_DIR}/dir/file.bin
+            """)
+
+    run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'runner.pyz', cwd=tmp_path)
+
+    with with_cwd(tmp_path):
+        args = capture_runner_cmdline(tmp_path / 'runner.pyz', 'kernel/abc.elf')
+
+    idx = args.index('-device')
+    resolved_arg = args[idx + 1]
+
+    file_bin = tmp_path / 'kernel' / 'dir' / 'file.bin'
+
+    assert resolved_arg.replace('\\', '/') == f'path,value={file_bin}'.replace('\\', '/')
```

### Comparing `qemu-runner-1.3.1/tests/test_utllities.py` & `qemu-runner-1.3.2/tests/test_utllities.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.1/tests/test_venv.py` & `qemu-runner-1.3.2/tests/test_venv.py`

 * *Files identical despite different names*

