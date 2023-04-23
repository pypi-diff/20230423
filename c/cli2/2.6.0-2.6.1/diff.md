# Comparing `tmp/cli2-2.6.0.tar.gz` & `tmp/cli2-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli2-2.6.0.tar", last modified: Fri Apr 21 22:28:26 2023, max compression
+gzip compressed data, was "cli2-2.6.1.tar", last modified: Sun Apr 23 14:48:33 2023, max compression
```

## Comparing `cli2-2.6.0.tar` & `cli2-2.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.778579 cli2-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 18:09:22.000000 cli2-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-21 22:28:26.778579 cli2-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-21 18:09:22.000000 cli2-2.6.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 18:09:22.000000 cli2-2.6.0/classifiers.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.775245 cli2-2.6.0/cli2/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11933 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/argument.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2023-04-21 19:16:37.000000 cli2-2.6.0/cli2/command.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/entry_point.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/group.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/node.py
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11376 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_group.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-21 21:56:13.000000 cli2-2.6.0/cli2/test_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.778579 cli2-2.6.0/cli2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 22:28:26.778579 cli2-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-21 22:28:26.000000 cli2-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.659612 cli2-2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 18:09:22.000000 cli2-2.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-04-23 14:48:33.659612 cli2-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-21 18:09:22.000000 cli2-2.6.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 18:09:22.000000 cli2-2.6.1/classifiers.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.656279 cli2-2.6.1/cli2/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12039 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/argument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5840 2023-04-21 19:16:37.000000 cli2-2.6.1/cli2/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/entry_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test_entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/test_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-21 21:56:13.000000 cli2-2.6.1/cli2/test_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.659612 cli2-2.6.1/cli2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 14:48:33.659612 cli2-2.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-23 14:48:33.000000 cli2-2.6.1/setup.py
```

### Comparing `cli2-2.6.0/PKG-INFO` & `cli2-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.6.0
+Version: 2.6.1
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Keywords: cli
 Requires-Python: >=3.6
```

### Comparing `cli2-2.6.0/README.rst` & `cli2-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/argument.py` & `cli2-2.6.1/cli2/argument.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,18 +228,19 @@
         )
 
     @property
     def value(self):
         """Return the value bound to this argument."""
         try:
             return self.cmd.bound.arguments[self.param.name]
-        except KeyError:
+        except KeyError as exc:
             if self.default != self.param.empty:
                 return self.default
-            raise
+            msg = f'{self.param.name} has no CLI bound value nor default'
+            raise ValueError(msg) from exc
 
     @value.setter
     def value(self, value):
         if value == self.param.empty:
             # the getter will return the default or raise
             return
         elif self.param.kind == self.param.VAR_POSITIONAL:
```

### Comparing `cli2-2.6.0/cli2/cli.py` & `cli2-2.6.1/cli2/cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/colors.py` & `cli2-2.6.1/cli2/colors.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/command.py` & `cli2-2.6.1/cli2/command.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/entry_point.py` & `cli2-2.6.1/cli2/entry_point.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/group.py` & `cli2-2.6.1/cli2/group.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/node.py` & `cli2-2.6.1/cli2/node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/table.py` & `cli2-2.6.1/cli2/table.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test.py` & `cli2-2.6.1/cli2/test.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test_cli.py` & `cli2-2.6.1/cli2/test_cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test_command.py` & `cli2-2.6.1/cli2/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 def test_vararg_after_kwarg():
     def foo(one=None, *two): return (one, two)
     cmd = Command(foo)
 
     cmd.parse('x')
     assert cmd['one'].value == 'x'
-    with pytest.raises(KeyError):
+    with pytest.raises(ValueError):
         cmd['two'].value
 
 
 def test_positional_only_looksahead():
     def foo(one=None, /, *two, three=None):  # noqa
         return (one, two)
     cmd = Command(foo)
@@ -301,15 +301,15 @@
 
 
 def test_kwarg_priority():
     def foo(missing, **kwarg):
         """docstring"""
     cmd = Command(foo)
     cmd.parse('foo=bar')
-    with pytest.raises(KeyError):
+    with pytest.raises(ValueError):
         cmd['missing'].value
 
 
 def test_kwargs_find_their_values():
     def foo(*a, b: str = '', c: str = '', **d):
         """docstring"""
     cmd = Command(foo)
```

### Comparing `cli2-2.6.0/cli2/test_decorators.py` & `cli2-2.6.1/cli2/test_decorators.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test_group.py` & `cli2-2.6.1/cli2/test_group.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test_inject.py` & `cli2-2.6.1/cli2/test_inject.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             [],
             None,
         ),
         (
             # default should not be enabled
             dict(),
             [],
-            KeyError,
+            ValueError,
         ),
         # test bools
         (
             # test default enabled by default
             dict(default=True),
             [],
             True,
@@ -104,15 +104,15 @@
     cmd = TestCommand(lambda test: test)
     assert cmd() is sentinel
 
     # but is not passed when not in signature
     cmd = TestCommand(lambda: None)
     assert cmd() is None
 
-    # we don't want no KeyError though
+    # we don't want no ValueError though
     class TestCommand2(TestCommand):
         def call(self, *args, **kwargs):
             return self['test'].value
 
     # argument value is available and passed as seen above
     cmd = TestCommand2(lambda test: test)
     assert cmd() is sentinel
```

### Comparing `cli2-2.6.0/cli2/test_node.py` & `cli2-2.6.1/cli2/test_node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2/test_table.py` & `cli2-2.6.1/cli2/test_table.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/cli2.egg-info/PKG-INFO` & `cli2-2.6.1/cli2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.6.0
+Version: 2.6.1
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Keywords: cli
 Requires-Python: >=3.6
```

### Comparing `cli2-2.6.0/cli2.egg-info/SOURCES.txt` & `cli2-2.6.1/cli2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli2-2.6.0/setup.py` & `cli2-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='cli2',
-    version='2.6.0',
+    version='2.6.1',
     setup_requires='setupmeta',
     install_requires=['docstring_parser==0.7.1'],
     extras_require=dict(
         test=[
             'freezegun',
             'pytest',
             'pytest-cov',
```

