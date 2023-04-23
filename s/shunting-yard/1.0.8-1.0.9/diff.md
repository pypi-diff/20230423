# Comparing `tmp/shunting-yard-1.0.8.tar.gz` & `tmp/shunting-yard-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shunting-yard-1.0.8.tar", last modified: Mon Apr 17 09:00:10 2023, max compression
+gzip compressed data, was "shunting-yard-1.0.9.tar", last modified: Mon Apr 17 20:04:54 2023, max compression
```

## Comparing `shunting-yard-1.0.8.tar` & `shunting-yard-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.137452 shunting-yard-1.0.8/
--rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 shunting-yard-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3870 2023-04-17 09:00:10.138452 shunting-yard-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3493 2023-04-17 08:55:23.000000 shunting-yard-1.0.8/README.md
--rw-rw-rw-   0        0        0      110 2023-02-28 14:21:46.000000 shunting-yard-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-17 09:00:10.140452 shunting-yard-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-04-17 08:51:19.000000 shunting-yard-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.119933 shunting-yard-1.0.8/shunting_yard/
--rw-rw-rw-   0        0        0      898 2023-03-02 07:03:42.000000 shunting-yard-1.0.8/shunting_yard/__init__.py
--rw-rw-rw-   0        0        0      517 2023-03-13 07:45:42.000000 shunting-yard-1.0.8/shunting_yard/__main__.py
--rw-rw-rw-   0        0        0      398 2023-03-13 11:44:14.000000 shunting-yard-1.0.8/shunting_yard/constants.py
--rw-rw-rw-   0        0        0     3288 2023-04-17 08:39:24.000000 shunting-yard-1.0.8/shunting_yard/rpn.py
--rw-rw-rw-   0        0        0     4360 2023-04-17 08:46:39.000000 shunting-yard-1.0.8/shunting_yard/shunting_yard.py
--rw-rw-rw-   0        0        0     2653 2023-04-17 08:51:05.000000 shunting-yard-1.0.8/shunting_yard/tokenize.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.131453 shunting-yard-1.0.8/shunting_yard.egg-info/
--rw-rw-rw-   0        0        0     3870 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.136452 shunting-yard-1.0.8/tests/
--rw-rw-rw-   0        0        0     1879 2023-03-01 13:58:52.000000 shunting-yard-1.0.8/tests/test_rpn.py
--rw-rw-rw-   0        0        0     3081 2023-04-17 08:46:41.000000 shunting-yard-1.0.8/tests/test_shunting_yard.py
--rw-rw-rw-   0        0        0     6926 2023-04-17 08:56:27.000000 shunting-yard-1.0.8/tests/test_tokenize.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:04:54.905726 shunting-yard-1.0.9/
+-rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 shunting-yard-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3870 2023-04-17 20:04:54.905726 shunting-yard-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3493 2023-04-17 08:55:23.000000 shunting-yard-1.0.9/README.md
+-rw-rw-rw-   0        0        0      110 2023-02-28 14:21:46.000000 shunting-yard-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-17 20:04:54.907726 shunting-yard-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-04-17 20:02:30.000000 shunting-yard-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:04:54.888728 shunting-yard-1.0.9/shunting_yard/
+-rw-rw-rw-   0        0        0      898 2023-03-02 07:03:42.000000 shunting-yard-1.0.9/shunting_yard/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-03-13 07:45:42.000000 shunting-yard-1.0.9/shunting_yard/__main__.py
+-rw-rw-rw-   0        0        0      433 2023-04-17 20:01:13.000000 shunting-yard-1.0.9/shunting_yard/constants.py
+-rw-rw-rw-   0        0        0     3288 2023-04-17 09:19:16.000000 shunting-yard-1.0.9/shunting_yard/rpn.py
+-rw-rw-rw-   0        0        0     4360 2023-04-17 09:19:05.000000 shunting-yard-1.0.9/shunting_yard/shunting_yard.py
+-rw-rw-rw-   0        0        0     2653 2023-04-17 08:51:05.000000 shunting-yard-1.0.9/shunting_yard/tokenize.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:04:54.898725 shunting-yard-1.0.9/shunting_yard.egg-info/
+-rw-rw-rw-   0        0        0     3870 2023-04-17 20:04:54.000000 shunting-yard-1.0.9/shunting_yard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-17 20:04:54.000000 shunting-yard-1.0.9/shunting_yard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:04:54.000000 shunting-yard-1.0.9/shunting_yard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 20:04:54.000000 shunting-yard-1.0.9/shunting_yard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 20:04:54.903730 shunting-yard-1.0.9/tests/
+-rw-rw-rw-   0        0        0     1879 2023-03-01 13:58:52.000000 shunting-yard-1.0.9/tests/test_rpn.py
+-rw-rw-rw-   0        0        0     3081 2023-04-17 08:46:41.000000 shunting-yard-1.0.9/tests/test_shunting_yard.py
+-rw-rw-rw-   0        0        0     7210 2023-04-17 20:01:00.000000 shunting-yard-1.0.9/tests/test_tokenize.py
```

### Comparing `shunting-yard-1.0.8/LICENSE` & `shunting-yard-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/PKG-INFO` & `shunting-yard-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shunting-yard
-Version: 1.0.8
+Version: 1.0.9
 Summary: Compute any math expression
 Home-page: https://www.github.com/charon25/ShuntingYard
-Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz
+Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.9.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shuting-yard algorithm
```

### Comparing `shunting-yard-1.0.8/README.md` & `shunting-yard-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/setup.py` & `shunting-yard-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fi:
     long_description = fi.read()
 
 setuptools.setup(
 	name="shunting-yard",
-	version="1.0.8",
+	version="1.0.9",
 	author="Paul 'charon25' Kern",
 	description="Compute any math expression",
 	long_description=long_description,
     long_description_content_type='text/markdown',
 	python_requires=">=3.9",
 	url="https://www.github.com/charon25/ShuntingYard",
 	license="MIT",
 	packages=['shunting_yard'],
-	download_url="https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz"
+	download_url="https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.9.tar.gz"
 )
```

### Comparing `shunting-yard-1.0.8/shunting_yard/__init__.py` & `shunting-yard-1.0.9/shunting_yard/__init__.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/shunting_yard/__main__.py` & `shunting-yard-1.0.9/shunting_yard/__main__.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/shunting_yard/rpn.py` & `shunting-yard-1.0.9/shunting_yard/rpn.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import math
 from operator import add, mul, neg, pos, sub, truediv
 from typing import Any, Callable, Optional, Union
-import math
 
 from shunting_yard.constants import NUMBER_CHARS
 
 
 class WrongExpressionError(Exception):
     pass
```

### Comparing `shunting-yard-1.0.8/shunting_yard/shunting_yard.py` & `shunting-yard-1.0.9/shunting_yard/shunting_yard.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
-from typing import Optional
 import math
 import re
+from typing import Optional
 
 from shunting_yard.tokenize import tokenize
 from shunting_yard.constants import BASE_OPERATORS, NUMBER_CHARS, FUNCTION_CHARS, SEPARATORS, SEPARATORS_NO_CLOSING_BRACKET, UNARY_OPERATORS_SYMBOLS
 
 
 class MismatchedBracketsError(Exception):
     pass
```

### Comparing `shunting-yard-1.0.8/shunting_yard/tokenize.py` & `shunting-yard-1.0.9/shunting_yard/tokenize.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/shunting_yard.egg-info/PKG-INFO` & `shunting-yard-1.0.9/shunting_yard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shunting-yard
-Version: 1.0.8
+Version: 1.0.9
 Summary: Compute any math expression
 Home-page: https://www.github.com/charon25/ShuntingYard
-Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz
+Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.9.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shuting-yard algorithm
```

### Comparing `shunting-yard-1.0.8/tests/test_rpn.py` & `shunting-yard-1.0.9/tests/test_rpn.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/tests/test_shunting_yard.py` & `shunting-yard-1.0.9/tests/test_shunting_yard.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.8/tests/test_tokenize.py` & `shunting-yard-1.0.9/tests/test_tokenize.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,19 @@
         self.assertListEqual(list(tokenize('min(-1, 2)')), ['min', '(', '-u', '1', ',', '2', ')'])
         self.assertListEqual(list(tokenize('min(1, -2)')), ['min', '(', '1', ',', '-u', '2', ')'])
         self.assertListEqual(list(tokenize('min(1, -(2+sin(3)))')), ['min', '(', '1', ',', '-u', '(', '2', '+', 'sin', '(', '3', ')', ')', ')'])
 
     def test_digits_in_function_name(self):
         self.assertListEqual(list(tokenize('min3(1, 2)')), ['min3', '(', '1', ',', '2', ')'])
 
+    def test_upper_case_functions(self):
+        self.assertListEqual(list(tokenize('Sin(x)')), ['Sin', '(', 'x', ')'])
+        self.assertListEqual(list(tokenize('sIN(x)')), ['sIN', '(', 'x', ')'])
+        self.assertListEqual(list(tokenize('SIN(x)')), ['SIN', '(', 'x', ')'])
+
 
 class TestRemoveImplicitMultiplication(unittest.TestCase):
 
     def test_no_implicit_mult(self):
         self.assertEqual(_remove_implicit_multiplication('1+1'), '1+1')
         self.assertEqual(_remove_implicit_multiplication('1-1'), '1-1')
         self.assertEqual(_remove_implicit_multiplication('1*1'), '1*1')
```

