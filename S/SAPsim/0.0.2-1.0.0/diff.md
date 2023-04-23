# Comparing `tmp/SAPsim-0.0.2.tar.gz` & `tmp/SAPsim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-0.0.2.tar", last modified: Fri Apr 21 18:48:51 2023, max compression
+gzip compressed data, was "SAPsim-1.0.0.tar", last modified: Sun Apr 23 03:30:44 2023, max compression
```

## Comparing `SAPsim-0.0.2.tar` & `SAPsim-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 18:48:42.000000 SAPsim-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-21 18:48:51.240523 SAPsim-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-21 18:48:42.000000 SAPsim-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 18:48:42.000000 SAPsim-0.0.2/README_PyPI.md
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 18:48:42.000000 SAPsim-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 18:48:51.240523 SAPsim-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-21 18:48:42.000000 SAPsim-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.236523 SAPsim-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.286396 SAPsim-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 03:30:35.000000 SAPsim-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-23 03:30:44.286396 SAPsim-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 03:30:35.000000 SAPsim-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-23 03:30:35.000000 SAPsim-1.0.0/README_PyPI.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-23 03:30:35.000000 SAPsim-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:30:44.286396 SAPsim-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-23 03:30:35.000000 SAPsim-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.286396 SAPsim-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_instructions.py
```

### Comparing `SAPsim-0.0.2/LICENSE` & `SAPsim-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.2/PKG-INFO` & `SAPsim-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 0.0.2
+Version: 1.0.0
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/sapsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
-License: MIT
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
-Keywords: SAP,SAPsim,UNC,COMP311
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
+Keywords: SAP,SAPsim,simple as possible,UNC,COMP311
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
 
 ![Tests](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 
 # SAPsim
 
 > Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
 
 Please see the rest of the README on [GitHub](https://github.com/jesse-wei/SAPsim).
+
+[Documentation](https://sapsim.readthedocs.io/en/latest/)
```

### Comparing `SAPsim-0.0.2/pyproject.toml` & `SAPsim-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.2/setup.py` & `SAPsim-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 try:
-    from setuptools import setup
+    from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 install_requires: list[str] = [
     "setuptools",
     "tabulate",
 ]
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Version number that appears on PyPI and Test PyPI
-    version="0.0.2",
+    version="1.0.0",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/sapsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
         "SAPsim",
+        "simple as possible",
         "UNC",
         "COMP311",
     ],
     install_requires=install_requires,
     tests_require=install_requires + ["tox", "pytest", "pytest-cov"],
-    # See https://docs.python.org/3/distutils/setupscript.html#listing-whole-packages
-    # or https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
-    # for what these mean
-    package_dir={"": "src"},
-    packages=["SAPsim", "utils"],
+    # See https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `SAPsim-0.0.2/src/SAPsim/__init__.py` & `SAPsim-1.0.0/SAPsim/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from pathlib import Path
 from typing import Any
-from src.utils.parser import parse_csv
-import src.utils.helpers as helpers
-import src.utils.globs as globs
-import src.utils.execute as execute
+from SAPsim.utils.parser import parse_csv
+import SAPsim.utils.helpers as helpers
+import SAPsim.utils.globs as globs
+import SAPsim.utils.execute as execute
 
 
 def run(prog_path: str, **kwargs) -> None:
     r"""Run given .csv program.
 
     :param prog_path:
         .csv file in SAPsim format.
     :type prog_path: ``str``
     :param \**kwargs:
         See below
 
     :Keyword Arguments:
         * *debug* (``bool``) --
             * Whether to run in debug mode (True) or at full speed (False)
+            * Default is full speed
         * *change* (``str``) --
             * Comma-separated list of changes to RAM
             * Useful for debugging programs (edit a value without changing CSV)
             * Also useful for autograding programs (overwrite a reserved instruction/data value)
             * Format: <addr>:<base-10 value>,<addr>:<base-10 value>, ...
         * *format* (``str``) --
             * Table format
             * Options: https://github.com/astanin/python-tabulate#table-format
         * *bits* (``int``) --
             * Number of bits in unsigned registers
+            * Default 8
     :return: ``dict`` containing all final values in globs.py, used for autograding
     :rtype: ``dict``
     """
     path: Path = Path(prog_path)
     assert path.suffix == ".csv"
     helpers.setup_8bit()
     parse_csv(path)
@@ -88,15 +90,15 @@
         execute.execute_full_speed()
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Program halted.")
 
 
 def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
-    r"""Run given .csv program and return final state. Just a wrapper around run() that's used for autograding.
+    r"""Run given .csv program and return final state. Just a wrapper around ``run()`` that can be used for autograding.
 
     The rest of the docstring is identical to that of run().
 
     :param prog_path:
         .csv file in SAPsim format.
     :type prog_path: ``str``
     :param \**kwargs:
```

### Comparing `SAPsim-0.0.2/src/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.0/SAPsim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 0.0.2
+Version: 1.0.0
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/sapsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
-License: MIT
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
-Keywords: SAP,SAPsim,UNC,COMP311
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
+Keywords: SAP,SAPsim,simple as possible,UNC,COMP311
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
 
 ![Tests](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 
 # SAPsim
 
 > Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
 
 Please see the rest of the README on [GitHub](https://github.com/jesse-wei/SAPsim).
+
+[Documentation](https://sapsim.readthedocs.io/en/latest/)
```

### Comparing `SAPsim-0.0.2/src/utils/exceptions.py` & `SAPsim-1.0.0/SAPsim/utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Custom exceptions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.helpers as helpers
-import src.utils.globs as globs
+import SAPsim.utils.helpers as helpers
+import SAPsim.utils.globs as globs
 
 
 def print_debug_info() -> None:
     """When most Exceptions (not DroppedOffBottom) occur, this function is called to print the instruction that caused the Exception and program state (RAM and registers and flags)"""
     curr_instruction = globs.RAM[globs.PC]
     print(
         f"Exception raised during execution of {globs.OPCODE_TO_MNEMONIC[helpers.parse_opcode(curr_instruction)]} {helpers.parse_arg(curr_instruction)} at address {globs.PC}"
@@ -53,15 +53,15 @@
             f"There's somehow a negative number {globs.B} in unsigned register B."
         )
         print_debug_info()
         super().__init__(self.message)
 
 
 class DroppedOffBottom(Exception):
-    """Raised if `PC` > max address in `RAM`."""
+    """Raised if ``PC`` > max address in ``RAM``."""
 
     def __init__(
         self,
         message=f"PC is greater than max address in RAM. Your program does not always HLT.",
     ):
         self.message = message
         helpers.print_RAM(dispPC=True)
```

### Comparing `SAPsim-0.0.2/src/utils/execute.py` & `SAPsim-1.0.0/SAPsim/utils/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Execute instructions in RAM."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.globs as globs
-import src.utils.instructions as instructions
-import src.utils.helpers as helpers
-import src.utils.exceptions as exceptions
+import SAPsim.utils.globs as globs
+import SAPsim.utils.instructions as instructions
+import SAPsim.utils.helpers as helpers
+import SAPsim.utils.exceptions as exceptions
 
 
 def execute_full_speed() -> None:
-    """Execute instructions in `RAM` at full speed until `EXECUTING` is `False` or `PC > max addr`."""
+    """Execute instructions in ``RAM`` at full speed until ``EXECUTING`` is ``False`` or ``PC > max addr``."""
     max_addr: int = 0
     if globs.RAM.keys():
         max_addr = max(globs.RAM.keys())
     while globs.EXECUTING:
         # Check that RAM is non-empty.
         if globs.RAM.keys() and globs.PC > max_addr:
             globs.EXECUTING = False
@@ -26,15 +26,15 @@
 
         instructions.OPCODE_TO_INSTR_PROCEDURE[
             helpers.parse_opcode(globs.RAM[globs.PC])
         ](helpers.parse_arg(globs.RAM[globs.PC]))
 
 
 def execute_next() -> None:
-    """Execute a single instruction at the current `PC` value if `EXECUTING`. If attempting to execute an empty address, `PC += 1` (i.e., doesn't skip to next filled address)."""
+    """Execute a single instruction at the current ``PC`` value if ``EXECUTING``. If attempting to execute an empty address, ``PC += 1`` (i.e., doesn't skip to next filled address)."""
     if globs.EXECUTING:
         if globs.RAM.keys() and globs.PC > max(globs.RAM.keys()):
             globs.EXECUTING = False
             raise exceptions.DroppedOffBottom
 
         # If executing an empty address, just skip and don't execute
         if globs.PC not in globs.RAM:
```

### Comparing `SAPsim-0.0.2/src/utils/globs.py` & `SAPsim-1.0.0/SAPsim/utils/globs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 """Global variables.
 
 If changing anything in this file, also modify SAPsim/__init__.py."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 RAM = {}
-"""`dict[int, int]` mapping `PC`:`byte`, where `byte` can be instruction or data (indistinguishable, mostly)"""
+"""``dict[int, int]`` mapping ``PC``:``byte``, where ``byte`` can be instruction or data (indistinguishable, mostly)"""
 PC: int = 0
-"""Program counter that indexes into `RAM`, default value 0"""
+"""Program counter that indexes into ``RAM``, default value 0"""
 A: int = 0
 """Register A, default value 0"""
 B: int = 0
 """Register B, default value 0"""
 FLAG_C: bool = False
-"""Carry-out bit, modified by `add()` and `sub()`. Default value False (0)."""
+"""Carry-out bit, modified by ``add()`` and ``sub()``. Default value False (0)."""
 FLAG_Z: bool = False
-"""Zero flag = NOR(Sum bits), modified by `add()` and `sub()`. Default value False (0).
+"""Zero flag = NOR(Sum bits), modified by ``add()`` and ``sub()``. Default value False (0).
 
 Lab 3's ALU has default value True (1) for FlagZ because the results register is initially 0.
 
 However, it makes more sense in the simulation to set it to False by default."""
 # Number of bits in registers
 # Same as number of full adders
 # This affects how FLAG_C, FLAG_Z, and result register work
 NUM_BITS_IN_REGISTERS: int = 8
-"""IMPORTANT NOTE: If changing this value, then also change `MAX_UNSIGNED_VAL_IN_REGISTERS`!!! This variable is the #bits in registers and affects how everything works. Default is 8."""
+"""IMPORTANT NOTE: If changing this value, then also change ``MAX_UNSIGNED_VAL_IN_REGISTERS``!!! This variable is the #bits in registers and affects how everything works. Default is 8."""
 MAX_UNSIGNED_VAL_IN_REGISTERS = 2**NUM_BITS_IN_REGISTERS - 1
 """This value needs to be changed whenever NUM_BITS_IN_REGISTERS is changed!"""
 EXECUTING: bool = True
-"""Is the program executing? Set to `False` by `hlt()`"""
+"""Is the program executing? Set to ``False`` by ``hlt()``"""
 
 MNEMONIC_TO_OPCODE = {
     "NOP": 0,
     "LDA": 1,
     "ADD": 2,
     "SUB": 3,
     "STA": 4,
     "LDI": 5,
     "JMP": 6,
     "JC": 7,
     "JZ": 8,
     "OUT": 14,
     "HLT": 15,
 }
-"""Maps `str mnemonic : int opcode`. All mnemonics in this dict are in all caps."""
+"""Maps ``str mnemonic : int opcode``. All mnemonics in this dict are in all caps."""
 
 OPCODE_TO_MNEMONIC = {
     0: "NOP",
     1: "LDA",
     2: "ADD",
     3: "SUB",
     4: "STA",
     5: "LDI",
     6: "JMP",
     7: "JC",
     8: "JZ",
     14: "OUT",
     15: "HLT",
 }
-"""Maps `int opcode : str mnemonic`"""
+"""Maps ``int opcode : str mnemonic``"""
 
 table_fmt: str = "simple_outline"
-"""Tabulate `table_fmt` arg to customize pretty-printing. Defaults to `simple_outline`, see all options: https://github.com/astanin/python-tabulate#table-
+"""Tabulate ``table_fmt`` arg to customize pretty-printing. Defaults to ``simple_outline``, see all options: https://github.com/astanin/python-tabulate#table-
                         format"""
```

### Comparing `SAPsim-0.0.2/src/utils/helpers.py` & `SAPsim-1.0.0/SAPsim/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Miscellaneous helper functions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
+
 from tabulate import tabulate
 from typing import Any
-import src.utils.globs as globs
-import src.utils.exceptions as exceptions
+import SAPsim.utils.globs as globs
+import SAPsim.utils.exceptions as exceptions
 
 
 def parse_byte(byte: int):
     """Given a byte (2 hexits), return the opcode (1 hexit) and arg (1 hexit). Return as dict for readability.
 
     :param byte:
     :type byte: int
@@ -62,20 +63,20 @@
         raise exceptions.InvalidInstructionString(instruction)
     return (globs.MNEMONIC_TO_OPCODE[instruction[:space_position].upper()] << 4) | int(
         instruction[space_position + 1 :]
     )
 
 
 def i2b(instruction: str) -> int:
-    """Alias for `instruction_to_byte()`."""
+    """Alias for ``instruction_to_byte()``."""
     return instruction_to_byte(instruction)
 
 
 def print_RAM(**kwargs):
-    """Pretty print the contents of RAM, sorted by address. | <PC (optional)> | Addr | Instruction | Dec | Hex | (since we can't distinguish instructions from data). Display arrow on current PC value if `dispPC=True` in kwargs. Set `format=` to set tabulate pretty-print format."""
+    """Pretty print the contents of RAM, sorted by address. | <PC (optional)> | Addr | Instruction | Dec | Hex | (since we can't distinguish instructions from data). Display arrow on current PC value if ``dispPC=True`` in kwargs. Set ``format=`` to set tabulate pretty-print format."""
     table = []
     for addr in sorted(globs.RAM.keys()):
         byte = globs.RAM[addr]
         opcode = parse_opcode(byte)
         arg = parse_arg(byte)
         instruction_str = (
             (globs.OPCODE_TO_MNEMONIC[opcode] + " " + str(arg))
@@ -91,15 +92,15 @@
     if "dispPC" in kwargs and kwargs["dispPC"]:
         headers.append("")
     headers.extend(["Addr", "Instruction", "Dec", "Hex"])
     print(tabulate(table, headers=headers, tablefmt=globs.table_fmt))
 
 
 def print_info(**kwargs):
-    """Print the values of everything in global_vars.py except RAM. Set optional parameter `bool=True` to print flags as `bool` instead of `int`. Set `format=` for tabulate pretty-print format."""
+    """Print the values of everything in global_vars.py except RAM. Set optional parameter ``bool=True`` to print flags as ``bool`` instead of ``int``. Set ``format=`` for tabulate pretty-print format."""
     table = [
         ["PC", globs.PC],
         ["Reg A", globs.A],
         ["Reg B", globs.B],
         [
             "FlagC",
             globs.FLAG_C
@@ -118,15 +119,15 @@
 
 def pad_hex(hex: str, width: int):
     """Pad given hex str with 0x prefix to width hexits. That is, 0x prefix not included in the width."""
     return "0x" + hex[2:].zfill(width)
 
 
 def clone_dict(dict):
-    """Returns a deep clone of `dict`. Used to clone `RAM`."""
+    """Returns a deep clone of ``dict``. Used to clone ``RAM``."""
     rv = {}
     for key in dict:
         rv[key] = dict[key]
     return rv
 
 
 def setup_4bit():
@@ -148,15 +149,15 @@
     assert n > 1
     globs.NUM_BITS_IN_REGISTERS = n
     globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**n - 1
     reset_globals()
 
 
 def reset_globals():
-    """Reset global variables (not `NUM_BITS_IN_REGISTERS` and `MAX_UNSIGNED_VAL_IN_REGISTERS` to default values."""
+    """Reset global variables (not ``NUM_BITS_IN_REGISTERS`` and ``MAX_UNSIGNED_VAL_IN_REGISTERS`` to default values."""
     globs.RAM = {}
     globs.PC = 0
     globs.A = 0
     globs.B = 0
     globs.FLAG_C = False
     globs.FLAG_Z = False
     globs.EXECUTING = True
```

### Comparing `SAPsim-0.0.2/src/utils/instructions.py` & `SAPsim-1.0.0/SAPsim/utils/instructions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 """All function docstrings (and even most implementations) are ripped straight from the SAP Instruction Set, with only slight modifications.
 
-This DOES NOT exist in actual SAP but for the purposes of simulation and testing, `add(arg)` and `sub(arg)` have optional kwargs direct_add= and direct_sub= that will cause A = A + arg, A = A - arg instead of A = A + Mem(arg), A = A - Mem(arg).
+This DOES NOT exist in actual SAP but for the purposes of simulation and testing, ``add(arg)`` and ``sub(arg)`` have optional kwargs direct_add= and direct_sub= that will cause A = A + arg, A = A - arg instead of A = A + Mem(arg), A = A - Mem(arg).
 
 This DOES NOT exist in actual SAP but for implementation purposes, instructions that don't need an arg (i.e. NOP, OUT, HLT) get a default parameter so that they can still be called with an argument. In actual SAP, all instructions (byte) have a required Arg, not a default or optional arg.
 
 INSTRUCTIONS dict for using an opcode to call a specific function is defined at the bottom."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.globs as globs
-import src.utils.exceptions as exceptions
-import src.utils.helpers as helpers
 from tabulate import tabulate
+import SAPsim.utils.globs as globs
+import SAPsim.utils.exceptions as exceptions
+import SAPsim.utils.helpers as helpers
 
 
 def nop(arg: int = 0) -> None:
     """Nop
 
     Opcode 0"""
     globs.PC += 1
 
 
 def lda(arg: int) -> None:
-    """`A = Mem(arg)`
+    """``A = Mem(arg)``
 
     Opcode 1"""
     if arg not in globs.RAM:
         raise exceptions.LoadFromUnmappedAddress
     globs.A = globs.RAM[arg]
     if globs.A > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
         raise exceptions.ARegisterNotEnoughBits
     if globs.A < 0:
         raise exceptions.ARegisterNegativeInt
     globs.PC += 1
 
 
 def add(arg: int, **kwargs) -> None:
-    """`A = A + Mem(arg)`. Accounts for `NUM_BITS_IN_REGISTERS` to set `FLAG_C` and `FLAG_Z`. Handles overflow.
+    """``A = A + Mem(arg)``. Accounts for ``NUM_BITS_IN_REGISTERS`` to set ``FLAG_C`` and ``FLAG_Z``. Handles overflow.
 
     Opcode 2
 
     Parameters
     ----------
     arg: int
         memory address, usually
     kwarg
-        `direct_add`: bool
-            Set to `True` to directly add `arg` (i.e. `A = A + arg` instead of `A = A + Mem(arg)`), for testing purposes and use in `sub`.
+        ``direct_add``: bool
+            Set to ``True`` to directly add ``arg`` (i.e. ``A = A + arg`` instead of ``A = A + Mem(arg)``), for testing purposes and use in ``sub``.
 
             This behavior does not exist in actual SAP."""
     if "direct_add" in kwargs and kwargs["direct_add"]:
         globs.B = arg
     else:
         if arg not in globs.RAM:
             raise exceptions.LoadFromUnmappedAddress
@@ -70,25 +70,25 @@
         globs.FLAG_C = 0
     globs.FLAG_Z = globs.A == 0
 
     globs.PC += 1
 
 
 def sub(arg: int, **kwargs) -> None:
-    """`A = A - Mem(arg)`. Accounts for `NUM_BITS_IN_REGISTERS` to set `FLAG_C` and `FLAG_Z`. Calls `add()` twice to perform 2's complement subtraction.
+    """``A = A - Mem(arg)``. Accounts for ``NUM_BITS_IN_REGISTERS`` to set ``FLAG_C`` and ``FLAG_Z``. Calls ``add()`` twice to perform 2's complement subtraction.
 
     Opcode 3
 
     Parameters
     ----------
     arg: int
         memory address, usually
     kwarg
         direct_sub: bool
-            set to `True` to directly sub `arg` (i.e. `A = A - arg` instead of `A = A - Mem(arg)`), for testing purposes.
+            set to ``True`` to directly sub ``arg`` (i.e. ``A = A - arg`` instead of ``A = A - Mem(arg)``), for testing purposes.
 
             This behavior does not exist in actual SAP."""
     if "direct_sub" in kwargs and kwargs["direct_sub"]:
         globs.B = arg
     else:
         if arg not in globs.RAM:
             raise exceptions.LoadFromUnmappedAddress
@@ -118,68 +118,68 @@
 
     # Subtract 1 from PC since there were 2 adds that each did PC += 1
     # Net effect is globs.PC += 1
     globs.PC -= 1
 
 
 def sta(arg: int) -> None:
-    """`Mem(Arg) = A`. CAN store to unmapped addr, which will simply map the addr in RAM.
+    """``Mem(Arg) = A``. CAN store to unmapped addr, which will simply map the addr in RAM.
 
     Opcode 4"""
     globs.RAM[arg] = globs.A
     globs.PC += 1
 
 
 def ldi(arg: int) -> None:
-    """`A = arg`
+    """``A = arg``
 
     Opcode 5"""
     globs.A = arg
     if arg > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
         raise exceptions.ARegisterNotEnoughBits
     if arg < 0:
         raise exceptions.ARegisterNegativeInt
     globs.PC += 1
 
 
 def jmp(arg: int) -> None:
-    """`PC = arg`
+    """``PC = arg``
 
     Opcode 6"""
     if arg < 0:
         raise exceptions.JumpToNegativeAddress
     globs.PC = arg
 
 
 def jc(arg: int) -> None:
-    """If `FC=1` then `PC=arg`; else go on
+    """If ``FC=1`` then ``PC=arg``; else go on
 
     Opcode 7"""
     if globs.FLAG_C:
         if arg < 0:
             raise exceptions.JumpToNegativeAddress
         globs.PC = arg
     else:
         globs.PC += 1
 
 
 def jz(arg: int) -> None:
-    """If `FZ=1` then `PC=arg`; else go on
+    """If ``FZ=1`` then ``PC=arg``; else go on
 
     Opcode 8"""
     if globs.FLAG_Z:
         if arg < 0:
             raise exceptions.JumpToNegativeAddress
         globs.PC = arg
     else:
         globs.PC += 1
 
 
 def out(arg: int = 0) -> None:
-    """`Display = OUT = A`. Prints | PC | A (dec) | A (hex) |
+    """``Display = OUT = A``. Prints | PC | A (dec) | A (hex) |
 
     Opcode 14"""
     arg = helpers.parse_arg(globs.RAM[globs.PC])
     table = [[globs.PC, globs.A, helpers.pad_hex(hex(globs.A), 2)]]
     print(tabulate(table, headers=["PC", "Dec", "Hex"], tablefmt=globs.table_fmt))
     globs.PC += 1
 
@@ -200,10 +200,10 @@
     5: ldi,
     6: jmp,
     7: jc,
     8: jz,
     14: out,
     15: hlt,
 }
-"""This `dict` maps opcodes to the procedures defined in this file.
+"""This ``dict`` maps opcodes to the procedures defined in this file.
 
-The syntax `OPCODE_TO_INSTR_PROCEDURE[opcode](arg)` will execute the correct instruction with `arg` passed as argument! Very cool."""
+The syntax ``OPCODE_TO_INSTR_PROCEDURE[opcode](arg)`` will execute the correct instruction with ``arg`` passed as argument! Very cool."""
```

### Comparing `SAPsim-0.0.2/src/utils/parser.py` & `SAPsim-1.0.0/SAPsim/utils/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Parses a SAP program in the CSV format given in `template.csv` into `globs.RAM`."""
+"""Parses a SAP program in the CSV format given in ``template.csv`` into ``globs.RAM``."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-from src.utils.helpers import *
 from csv import DictReader
-import src.utils.exceptions as exceptions
+import SAPsim.utils.exceptions as exceptions
+import SAPsim.utils.globs as globs
 
 
 def parse_csv(file_path):
-    """Takes a `.csv` file path in `template.csv` format and parses it into `RAM`."""
+    """Takes a ``.csv`` file path in ``template.csv`` format and parses it into ``RAM``."""
     prog = DictReader(open(file_path))
     num_rows = 1
     addresses = set()
 
     for row in prog:
         if not row["Address"]:
             raise exceptions.RowWithNoAddress(num_rows)
```

### Comparing `SAPsim-0.0.2/tests/test_example_progs.py` & `SAPsim-1.0.0/tests/test_example_progs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 This code should be the same (or mostly the same, in case it's updated) as the code that autogrades Lab 4.
 If you have any questions about RESERVED/RETURN VALUE, they can be answered by reading through this.
 If you don't know the test cases your program is failing, you can very easily write a function to check it yourself. It'd probably be exactly the same as what I wrote.
 """
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.globs as globs
-from src.utils import parser
-from src.utils.execute import execute_full_speed
-from src.utils.helpers import setup_8bit
+from SAPsim.utils import globs
+from SAPsim.utils import parser
+from SAPsim.utils.execute import execute_full_speed
+from SAPsim.utils.helpers import setup_8bit
 
 
 def clone_dict(dict):
     """Returns a deep clone of `dict`. Used to clone `RAM`."""
     rv = {}
     for key in dict:
         rv[key] = dict[key]
```

### Comparing `SAPsim-0.0.2/tests/test_helpers.py` & `SAPsim-1.0.0/tests/test_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Test helpers.py."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-from src.utils.helpers import *
-from src.utils.globs import *
 import pytest
-import src.utils.exceptions as exceptions
+from SAPsim.utils.helpers import *
+from SAPsim.utils.globs import *
+import SAPsim.utils.exceptions as exceptions
 
 
 def test_instruction_to_byte_returns_correct_byte():
     """Generate all possible instructions in byte form. Test that `instruction_to_byte` returns the correct byte given the string representation <Mnemonic> <Arg>."""
     # Instructions 0x00 to 0x8f (inclusive)
     for i in range(0x90):
-        assert i == instruction_to_byte(f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}")
+        assert i == instruction_to_byte(
+            f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}"
+        )
     # Instructions 0xe0 to 0xff (inclusive)
-    for i in range(0xe0, 0xff):
-        assert i == instruction_to_byte(f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}")
+    for i in range(0xE0, 0xFF):
+        assert i == instruction_to_byte(
+            f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}"
+        )
 
 
 def test_instruction_to_byte_NOP_OUT_HLT():
     """Test that instruction to byte returns correct opcode and Arg 0 for NOP, OUT, HLT without an arg."""
     assert 0 == instruction_to_byte("NOP")
-    assert 0xe << 4 == instruction_to_byte("OUT")
-    assert 0xf << 4 == instruction_to_byte("HLT")
+    assert 0xE << 4 == instruction_to_byte("OUT")
+    assert 0xF << 4 == instruction_to_byte("HLT")
 
 
 def test_instruction_to_byte_instructions_require_arg():
-    instructions_require_arg = ['LDA', 'ADD', 'SUB', 'STA', 'LDI', 'JMP', 'JC', 'JZ']
+    instructions_require_arg = ["LDA", "ADD", "SUB", "STA", "LDI", "JMP", "JC", "JZ"]
     for instruction in instructions_require_arg:
         with pytest.raises(exceptions.InstructionRequiresArg):
             instruction_to_byte(instruction)
```

### Comparing `SAPsim-0.0.2/tests/test_instructions.py` & `SAPsim-1.0.0/tests/test_instructions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,143 @@
 """Test instructions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.globs as globs
-from src.utils.execute import execute_full_speed, execute_next
-from src.utils.helpers import check_state, check_state_all, print_RAM, print_info
-from src.utils.exceptions import DroppedOffBottom, ARegisterNotEnoughBits, BRegisterNotEnoughBits, LoadFromUnmappedAddress, ARegisterNegativeInt, BRegisterNegativeInt
-from src.utils.helpers import setup_4bit, setup_8bit, reset_globals
-from src.utils import parser
+import SAPsim.utils.globs as globs
+from SAPsim.utils.execute import execute_full_speed, execute_next
+from SAPsim.utils.helpers import check_state, check_state_all
+from SAPsim.utils.exceptions import (
+    DroppedOffBottom,
+    ARegisterNotEnoughBits,
+    LoadFromUnmappedAddress,
+)
+from SAPsim.utils.helpers import setup_4bit
 
 
 def test_nop():
     setup_4bit()
     globs.RAM[0] = 0x00
     globs.RAM[1] = 0x01
     globs.RAM[2] = 0x02
-    globs.RAM[4] = 0x0f
+    globs.RAM[4] = 0x0F
     try:
         execute_full_speed()
         assert False
     except DroppedOffBottom:
         pass
-    check_state_all({0: 0x00, 1: 0x01, 2: 0x02, 4: 0x0f}, 5, 0, 0, False, False, False)
+    check_state_all({0: 0x00, 1: 0x01, 2: 0x02, 4: 0x0F}, 5, 0, 0, False, False, False)
 
 
 def test_lda():
     setup_4bit()
-    globs.RAM[0] = 0x1f
-    globs.RAM[1] = 0x1e
+    globs.RAM[0] = 0x1F
+    globs.RAM[1] = 0x1E
     globs.RAM[14] = 0x3
     globs.RAM[15] = 0x4
     execute_next()
-    check_state_all({0: 0x1f, 1: 0x1e, 14: 0x3, 15: 0x4}, 1, 4, 0, False, False, True)
+    check_state_all({0: 0x1F, 1: 0x1E, 14: 0x3, 15: 0x4}, 1, 4, 0, False, False, True)
     execute_next()
-    check_state_all({0: 0x1f, 1: 0x1e, 14: 0x3, 15: 0x4}, 2, 3, 0, False, False, True)
+    check_state_all({0: 0x1F, 1: 0x1E, 14: 0x3, 15: 0x4}, 2, 3, 0, False, False, True)
 
 
 def test_lda_raises_ARegisterOverflow():
     setup_4bit()
-    globs.RAM[0] = 0x1f
+    globs.RAM[0] = 0x1F
     globs.RAM[15] = 0x10
     try:
         execute_next()
         assert False
     except ARegisterNotEnoughBits:
         pass
 
 
 def test_lda_from_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x1f
+    globs.RAM[0] = 0x1F
     try:
         execute_next()
         assert False
     except LoadFromUnmappedAddress:
         pass
 
 
 def test_add():
     setup_4bit()
-    globs.RAM[0] = 0x2f
-    globs.RAM[1] = 0x2e
-    globs.RAM[14] = 0xf
-    globs.RAM[15] = 0xf
-    execute_next()
-    check_state(RAM={0: 0x2f, 1: 0x2e, 14: 0xf, 15: 0xf}, A=0xf, FLAG_C=False, FLAG_Z=False)
-    execute_next()
-    check_state(RAM={0: 0x2f, 1: 0x2e, 14: 0xf, 15: 0xf}, A=14, FLAG_C=True, Flag_Z=False)
+    globs.RAM[0] = 0x2F
+    globs.RAM[1] = 0x2E
+    globs.RAM[14] = 0xF
+    globs.RAM[15] = 0xF
+    execute_next()
+    check_state(
+        RAM={0: 0x2F, 1: 0x2E, 14: 0xF, 15: 0xF}, A=0xF, FLAG_C=False, FLAG_Z=False
+    )
+    execute_next()
+    check_state(
+        RAM={0: 0x2F, 1: 0x2E, 14: 0xF, 15: 0xF}, A=14, FLAG_C=True, Flag_Z=False
+    )
     try:
         execute_full_speed()
         assert False
     except DroppedOffBottom:
         pass
 
 
 def test_add_from_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2f
+    globs.RAM[0] = 0x2F
     try:
         execute_next()
         assert False
     except LoadFromUnmappedAddress:
         pass
 
 
 def test_sub():
     setup_4bit()
-    globs.RAM[0] = 0x3f
-    globs.RAM[1] = 0x3e
+    globs.RAM[0] = 0x3F
+    globs.RAM[1] = 0x3E
     globs.RAM[14] = 0x1
-    globs.RAM[15] = 0xf
+    globs.RAM[15] = 0xF
     execute_next()
-    check_state(RAM={0: 0x3f, 1: 0x3e, 14: 0x1, 15: 0xf}, A=1, FLAG_C=False, FLAG_Z=False)
+    check_state(
+        RAM={0: 0x3F, 1: 0x3E, 14: 0x1, 15: 0xF}, A=1, FLAG_C=False, FLAG_Z=False
+    )
     execute_next()
-    check_state(RAM={0: 0x3f, 1: 0x3e, 14: 0x1, 15: 0xf}, A=0, FLAG_C=True, FLAG_Z=True)
+    check_state(RAM={0: 0x3F, 1: 0x3E, 14: 0x1, 15: 0xF}, A=0, FLAG_C=True, FLAG_Z=True)
 
 
 def test_sta_to_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2f
-    globs.RAM[1] = 0x4e
-    globs.RAM[15] = 0xf
+    globs.RAM[0] = 0x2F
+    globs.RAM[1] = 0x4E
+    globs.RAM[15] = 0xF
     execute_next()
     execute_next()
-    check_state(RAM={0: 0x2f, 1: 0x4e, 0xe: 0xf, 0xf: 0xf}, A=0xf, FLAG_C=False, FLAG_Z=False, PC=2, EXECUTING=True)
+    check_state(
+        RAM={0: 0x2F, 1: 0x4E, 0xE: 0xF, 0xF: 0xF},
+        A=0xF,
+        FLAG_C=False,
+        FLAG_Z=False,
+        PC=2,
+        EXECUTING=True,
+    )
 
 
 def test_sta_overwrites_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2e
-    globs.RAM[1] = 0x4f
+    globs.RAM[0] = 0x2E
+    globs.RAM[1] = 0x4F
     globs.RAM[14] = 2
     globs.RAM[15] = 1
     try:
         execute_full_speed()
         assert False
     except DroppedOffBottom:
         pass
-    check_state_all({0: 0x2e, 1: 0x4f, 14: 2, 15: 2}, 16, 2, 2, False, False, False)
+    check_state_all({0: 0x2E, 1: 0x4F, 14: 2, 15: 2}, 16, 2, 2, False, False, False)
 
 
 def test_ldi():
     setup_4bit()
     globs.RAM[0] = 0x59
     execute_next()
     check_state_all({0: 0x59}, 1, 9, 0, False, False, True)
@@ -133,19 +149,19 @@
     globs.RAM[0] = 0x55
     execute_next()
     check_state_all({0: 0x55}, 1, 5, 0, False, False, True)
 
 
 def test_ldi_doesnt_modify_flags():
     setup_4bit()
-    globs.RAM[0] = 0x5a
+    globs.RAM[0] = 0x5A
     globs.FLAG_C = True
     globs.FLAG_Z = True
     execute_next()
-    check_state_all({0: 0x5a}, 1, 0xa, 0, True, True, True)
+    check_state_all({0: 0x5A}, 1, 0xA, 0, True, True, True)
 
 
 def test_jmp():
     setup_4bit()
     globs.RAM[0] = 0x67
     execute_next()
     check_state_all({0: 0x67}, 7, 0, 0, False, False, True)
@@ -169,17 +185,17 @@
         assert False
     except DroppedOffBottom:
         pass
 
 
 def test_hlt():
     setup_4bit()
-    globs.RAM[0] = 0xff
+    globs.RAM[0] = 0xFF
     globs.RAM[15] = 0x10
     execute_next()
-    check_state_all({0: 0xff, 15: 0x10}, 0, 0, 0, False, False, False)
+    check_state_all({0: 0xFF, 15: 0x10}, 0, 0, 0, False, False, False)
     for i in range(100):
         execute_next()
-    check_state_all({0: 0xff, 15: 0x10}, 0, 0, 0, False, False, False)
+    check_state_all({0: 0xFF, 15: 0x10}, 0, 0, 0, False, False, False)
     for i in range(1000):
         execute_full_speed()
-    check_state_all({0: 0xff, 15: 0x10}, 0, 0, 0, False, False, False)
+    check_state_all({0: 0xFF, 15: 0x10}, 0, 0, 0, False, False, False)
```

