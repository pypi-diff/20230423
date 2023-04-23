# Comparing `tmp/pythoness-0.0.4.tar.gz` & `tmp/pythoness-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoness-0.0.4.tar", last modified: Sat Apr 22 06:49:51 2023, max compression
+gzip compressed data, was "pythoness-0.0.5.tar", last modified: Sun Apr 23 19:49:15 2023, max compression
```

## Comparing `pythoness-0.0.4.tar` & `pythoness-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-22 06:49:51.404248 pythoness-0.0.4/
--rw-r--r--   0 emery      (504) staff       (20)     2627 2023-04-22 06:49:51.404143 pythoness-0.0.4/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)     2103 2023-04-22 06:48:43.000000 pythoness-0.0.4/README.md
--rw-r--r--   0 emery      (504) staff       (20)      677 2023-04-22 06:49:26.000000 pythoness-0.0.4/pyproject.toml
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-22 06:49:51.403110 pythoness-0.0.4/pythoness/
--rw-r--r--   0 emery      (504) staff       (20)       56 2023-04-21 22:53:24.000000 pythoness-0.0.4/pythoness/__init__.py
--rw-r--r--   0 emery      (504) staff       (20)     5946 2023-04-22 06:30:31.000000 pythoness-0.0.4/pythoness/pythoness_module.py
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-22 06:49:51.403626 pythoness-0.0.4/pythoness.egg-info/
--rw-r--r--   0 emery      (504) staff       (20)     2627 2023-04-22 06:49:51.000000 pythoness-0.0.4/pythoness.egg-info/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)      330 2023-04-22 06:49:51.000000 pythoness-0.0.4/pythoness.egg-info/SOURCES.txt
--rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-22 06:49:51.000000 pythoness-0.0.4/pythoness.egg-info/dependency_links.txt
--rw-r--r--   0 emery      (504) staff       (20)       35 2023-04-22 06:49:51.000000 pythoness-0.0.4/pythoness.egg-info/requires.txt
--rw-r--r--   0 emery      (504) staff       (20)       10 2023-04-22 06:49:51.000000 pythoness-0.0.4/pythoness.egg-info/top_level.txt
--rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-22 06:49:51.404279 pythoness-0.0.4/setup.cfg
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-22 06:49:51.404016 pythoness-0.0.4/test/
--rw-r--r--   0 emery      (504) staff       (20)      493 2023-04-22 06:29:36.000000 pythoness-0.0.4/test/test-count-all-characters.py
--rw-r--r--   0 emery      (504) staff       (20)      147 2023-04-21 23:09:11.000000 pythoness-0.0.4/test/test-fib-notypes.py
--rw-r--r--   0 emery      (504) staff       (20)      159 2023-04-21 22:54:33.000000 pythoness-0.0.4/test/test-fib.py
--rw-r--r--   0 emery      (504) staff       (20)      502 2023-04-22 06:32:55.000000 pythoness-0.0.4/test/test2.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-23 19:49:15.737521 pythoness-0.0.5/
+-rw-r--r--   0 emery      (504) staff       (20)     4657 2023-04-23 19:49:15.737391 pythoness-0.0.5/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)     4133 2023-04-23 19:48:08.000000 pythoness-0.0.5/README.md
+-rw-r--r--   0 emery      (504) staff       (20)      677 2023-04-23 19:48:57.000000 pythoness-0.0.5/pyproject.toml
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-23 19:49:15.735395 pythoness-0.0.5/pythoness/
+-rw-r--r--   0 emery      (504) staff       (20)       56 2023-04-21 22:53:24.000000 pythoness-0.0.5/pythoness/__init__.py
+-rw-r--r--   0 emery      (504) staff       (20)    11875 2023-04-23 19:46:36.000000 pythoness-0.0.5/pythoness/pythoness_module.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-23 19:49:15.735930 pythoness-0.0.5/pythoness.egg-info/
+-rw-r--r--   0 emery      (504) staff       (20)     4657 2023-04-23 19:49:15.000000 pythoness-0.0.5/pythoness.egg-info/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)      394 2023-04-23 19:49:15.000000 pythoness-0.0.5/pythoness.egg-info/SOURCES.txt
+-rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-23 19:49:15.000000 pythoness-0.0.5/pythoness.egg-info/dependency_links.txt
+-rw-r--r--   0 emery      (504) staff       (20)       35 2023-04-23 19:49:15.000000 pythoness-0.0.5/pythoness.egg-info/requires.txt
+-rw-r--r--   0 emery      (504) staff       (20)       10 2023-04-23 19:49:15.000000 pythoness-0.0.5/pythoness.egg-info/top_level.txt
+-rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-23 19:49:15.737554 pythoness-0.0.5/setup.cfg
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-23 19:49:15.737090 pythoness-0.0.5/test/
+-rw-r--r--   0 emery      (504) staff       (20)      813 2023-04-22 14:35:00.000000 pythoness-0.0.5/test/test-count-all-characters-twice.py
+-rw-r--r--   0 emery      (504) staff       (20)      643 2023-04-22 10:43:13.000000 pythoness-0.0.5/test/test-count-all-characters.py
+-rw-r--r--   0 emery      (504) staff       (20)      147 2023-04-21 23:09:11.000000 pythoness-0.0.5/test/test-fib-notypes.py
+-rw-r--r--   0 emery      (504) staff       (20)      159 2023-04-21 22:54:33.000000 pythoness-0.0.5/test/test-fib.py
+-rw-r--r--   0 emery      (504) staff       (20)      399 2023-04-22 15:54:05.000000 pythoness-0.0.5/test/test-find-words.py
+-rw-r--r--   0 emery      (504) staff       (20)      502 2023-04-22 06:32:55.000000 pythoness-0.0.5/test/test2.py
```

### Comparing `pythoness-0.0.4/PKG-INFO` & `pythoness-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,18 @@
-Metadata-Version: 2.1
-Name: pythoness
-Version: 0.0.4
-Summary: Pythoness: use natural language to define Python functions.
-Author-email: Emery Berger <emery.berger@gmail.com>
-Project-URL: Homepage, https://github.com/plasma-umass/pythoness
-Project-URL: Bug Tracker, https://github.com/plasma-umass/pythoness/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Pythoness
 
-> Pythoness: The priestess of the oracle of Apollo at Delphi.
+![Pythoness](https://raw.githubusercontent.com/plasma-umass/pythoness/main/pythoness-logo.jpg)
+
+_Pythoness: The priestess of the oracle of Apollo at Delphi._
 
 by [Emery Berger](https://emeryberger.com)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pythoness.svg)](https://pypi.org/project/pythoness/)[![Downloads](https://pepy.tech/badge/pythoness)](https://pepy.tech/project/pythoness) [![Downloads](https://pepy.tech/badge/pythoness/month)](https://pepy.tech/project/pythoness) ![Python versions](https://img.shields.io/pypi/pyversions/pythoness.svg?style=flat-square)
 
-Pythoness is a Python module that automatically generates Python code based on natural language descriptions of the desired functionality.
+Pythoness is a Python module that automatically generates Python code from natural language descriptions.
 
 *NOTE*: To use pythoness, you must first set up an OpenAI API key. If you
 already have an API key, you can set it as an environment variable
 called `OPENAI_API_KEY`. If you do not have one yet,
 you can get a key here: https://platform.openai.com/account/api-keys
 
 ```
@@ -46,30 +35,85 @@
 import pythoness
 
 @pythoness.spec("Compute the nth number in the Fibonacci series.")
 def myfib(n: int) -> int:
     ""
 ```
 
-This code will generate a Python function named `myfib` that computes the nth number in the Fibonacci series.
-
-To actually execute the function, you can call it as you would any other Python function:
+This code will internally generate a Python function named `myfib`
+that computes the nth number in the Fibonacci series.  To actually
+execute the function, you can call it as you would any other Python
+function:
 
 ```python
 for i in range(20):
     print(myfib(i))
 ```
 
 Pythoness caches the results of translating natural language to
 Python, so subsequent executions in the same directory will run much
-faster.
+faster (Pythoness creates a database called `pythoness-cache.db` that
+saves these translations).
 
-If you want Pythoness to replace the code with the generated function, just add `replace=True`:
+### Incorporating tests
+
+You can guide Pythoness by providing some tests. Pythoness will use
+tests both to generate the Python code and to validate it. Tests are just
+a list of strings containing Python code which should all evaluate to `True`.
 
 ```python
-@pythoness.spec("Compute the nth number in the Fibonacci series.", replace=True)
+@pythoness.spec("Compute the nth number in the Fibonacci series.",
+                tests=["myfib(1) == 1", "myfib(2) == 1"])
 def myfib(n: int) -> int:
     ""
 ```
 
-Setting the `replace` flag will cause Pythoness to rewrite the program with the synthesized function definition(s).
+### Replacing Pythoness functions with Python
+
+You can have Pythoness to replace the spec directly in your file with
+the generated function: just add `replace=True`:
+
+```python
+@pythoness.spec("Compute the nth number in the Fibonacci series.",
+                tests=["myfib(1) == 1", "myfib(2) == 1"],
+		replace=True)
+def myfib(n: int) -> int:
+    ""
+```
+
+For example, Pythoness produced this code:
+
+```
+def myfib(n: int) -> int:
+    """
+    Compute the nth number in the Fibonacci series.
+
+    :param n: The position of the desired number in the Fibonacci series
+    :type n: int
+    :return: The nth number in the Fibonacci series
+    :rtype: int
+    """
+    if n <= 0:
+        raise ValueError("n must be a positive integer")
+    elif n == 1 or n == 2:
+        return 1
+    else:
+        fib1, fib2 = 1, 1
+        for _ in range(3, n + 1):
+            fib1, fib2 = fib2, fib1 + fib2
+        return fib2
+```
+
+### Other ways to control Pythoness
+
+Pythoness offers a few other ways to control its behavior. These are
+all arguments to `spec`. The provided values indicate the the default
+value.
+
+* `max_retries=3`: controls the maximum number of retries due to failures (e.g., a function that fails one of the provided tests).
+
+* `min_confidence=0.7`: sets the minimum level of confidence that the AI system reports regarding the correctness of the generated function (a number between 0 and 1, corresponding to 0% and 100%). Increasing the confidence level may require increasing `max_retries`.
+
+* `verbose=False`: set this to `True` to have Pythoness to output details as it generates and validates code. Mostly useful for developers and for keeping tabs on progress.
+
+* `output=False`: set this to `True` to have Pythoness output the generated code the first time the function is called.
```

### Comparing `pythoness-0.0.4/pyproject.toml` & `pythoness-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pythoness"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
 ]
 dependencies = ["openai>=0.27.0", "ast-comments>=1.0.0"]
 description = "Pythoness: use natural language to define Python functions."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pythoness-0.0.4/pythoness.egg-info/PKG-INFO` & `pythoness-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pythoness
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pythoness: use natural language to define Python functions.
 Author-email: Emery Berger <emery.berger@gmail.com>
 Project-URL: Homepage, https://github.com/plasma-umass/pythoness
 Project-URL: Bug Tracker, https://github.com/plasma-umass/pythoness/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pythoness
 
-> Pythoness: The priestess of the oracle of Apollo at Delphi.
+![Pythoness](https://raw.githubusercontent.com/plasma-umass/pythoness/main/pythoness-logo.jpg)
+
+_Pythoness: The priestess of the oracle of Apollo at Delphi._
 
 by [Emery Berger](https://emeryberger.com)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pythoness.svg)](https://pypi.org/project/pythoness/)[![Downloads](https://pepy.tech/badge/pythoness)](https://pepy.tech/project/pythoness) [![Downloads](https://pepy.tech/badge/pythoness/month)](https://pepy.tech/project/pythoness) ![Python versions](https://img.shields.io/pypi/pyversions/pythoness.svg?style=flat-square)
 
-Pythoness is a Python module that automatically generates Python code based on natural language descriptions of the desired functionality.
+Pythoness is a Python module that automatically generates Python code from natural language descriptions.
 
 *NOTE*: To use pythoness, you must first set up an OpenAI API key. If you
 already have an API key, you can set it as an environment variable
 called `OPENAI_API_KEY`. If you do not have one yet,
 you can get a key here: https://platform.openai.com/account/api-keys
 
 ```
@@ -46,30 +48,85 @@
 import pythoness
 
 @pythoness.spec("Compute the nth number in the Fibonacci series.")
 def myfib(n: int) -> int:
     ""
 ```
 
-This code will generate a Python function named `myfib` that computes the nth number in the Fibonacci series.
-
-To actually execute the function, you can call it as you would any other Python function:
+This code will internally generate a Python function named `myfib`
+that computes the nth number in the Fibonacci series.  To actually
+execute the function, you can call it as you would any other Python
+function:
 
 ```python
 for i in range(20):
     print(myfib(i))
 ```
 
 Pythoness caches the results of translating natural language to
 Python, so subsequent executions in the same directory will run much
-faster.
+faster (Pythoness creates a database called `pythoness-cache.db` that
+saves these translations).
+
+### Incorporating tests
+
+You can guide Pythoness by providing some tests. Pythoness will use
+tests both to generate the Python code and to validate it. Tests are just
+a list of strings containing Python code which should all evaluate to `True`.
+
+```python
+@pythoness.spec("Compute the nth number in the Fibonacci series.",
+                tests=["myfib(1) == 1", "myfib(2) == 1"])
+def myfib(n: int) -> int:
+    ""
+```
 
-If you want Pythoness to replace the code with the generated function, just add `replace=True`:
+### Replacing Pythoness functions with Python
+
+You can have Pythoness to replace the spec directly in your file with
+the generated function: just add `replace=True`:
 
 ```python
-@pythoness.spec("Compute the nth number in the Fibonacci series.", replace=True)
+@pythoness.spec("Compute the nth number in the Fibonacci series.",
+                tests=["myfib(1) == 1", "myfib(2) == 1"],
+		replace=True)
 def myfib(n: int) -> int:
     ""
 ```
 
-Setting the `replace` flag will cause Pythoness to rewrite the program with the synthesized function definition(s).
+For example, Pythoness produced this code:
+
+```
+def myfib(n: int) -> int:
+    """
+    Compute the nth number in the Fibonacci series.
+
+    :param n: The position of the desired number in the Fibonacci series
+    :type n: int
+    :return: The nth number in the Fibonacci series
+    :rtype: int
+    """
+    if n <= 0:
+        raise ValueError("n must be a positive integer")
+    elif n == 1 or n == 2:
+        return 1
+    else:
+        fib1, fib2 = 1, 1
+        for _ in range(3, n + 1):
+            fib1, fib2 = fib2, fib1 + fib2
+        return fib2
+```
+
+### Other ways to control Pythoness
+
+Pythoness offers a few other ways to control its behavior. These are
+all arguments to `spec`. The provided values indicate the the default
+value.
+
+* `max_retries=3`: controls the maximum number of retries due to failures (e.g., a function that fails one of the provided tests).
+
+* `min_confidence=0.7`: sets the minimum level of confidence that the AI system reports regarding the correctness of the generated function (a number between 0 and 1, corresponding to 0% and 100%). Increasing the confidence level may require increasing `max_retries`.
+
+* `verbose=False`: set this to `True` to have Pythoness to output details as it generates and validates code. Mostly useful for developers and for keeping tabs on progress.
+
+* `output=False`: set this to `True` to have Pythoness output the generated code the first time the function is called.
```

