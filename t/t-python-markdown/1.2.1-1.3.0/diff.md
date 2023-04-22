# Comparing `tmp/t_python_markdown-1.2.1.tar.gz` & `tmp/t_python_markdown-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_python_markdown-1.2.1.tar", last modified: Sun Mar  5 14:08:39 2023, max compression
+gzip compressed data, was "t_python_markdown-1.3.0.tar", last modified: Sat Apr 22 23:25:21 2023, max compression
```

## Comparing `t_python_markdown-1.2.1.tar` & `t_python_markdown-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 14:08:39.799586 t_python_markdown-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6691 2023-03-05 14:08:39.798586 t_python_markdown-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4847 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-05 14:08:39.799586 t_python_markdown-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 14:08:39.797586 t_python_markdown-1.2.1/t_python_markdown/
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/t_python_markdown/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 14:08:39.798586 t_python_markdown-1.2.1/t_python_markdown/extensions/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/t_python_markdown/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/t_python_markdown/extensions/mkdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-03-05 14:08:19.000000 t_python_markdown-1.2.1/t_python_markdown/t_python_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 14:08:39.798586 t_python_markdown-1.2.1/t_python_markdown.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6691 2023-03-05 14:08:39.000000 t_python_markdown-1.2.1/t_python_markdown.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-05 14:08:39.000000 t_python_markdown-1.2.1/t_python_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-05 14:08:39.000000 t_python_markdown-1.2.1/t_python_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-05 14:08:39.000000 t_python_markdown-1.2.1/t_python_markdown.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-05 14:08:39.000000 t_python_markdown-1.2.1/t_python_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7527 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.867182 t_python_markdown-1.3.0/t_python_markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.868182 t_python_markdown-1.3.0/t_python_markdown/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/extensions/mkdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10268 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/t_python_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.868182 t_python_markdown-1.3.0/t_python_markdown.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7527 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/top_level.txt
```

### Comparing `t_python_markdown-1.2.1/LICENSE` & `t_python_markdown-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.2.1/PKG-INFO` & `t_python_markdown-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_python_markdown
-Version: 1.2.1
+Version: 1.3.0
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -29,14 +29,15 @@
 Project-URL: homepage, https://www.cix.co.uk/~toyne/t-python-markdown/
 Project-URL: documentation, https://www.cix.co.uk/~toyne/t-python-markdown/
 Keywords: markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dependencies
 License-File: LICENSE
 
 # t-python-markdown
 
 A simple to use markdown generator for Python.
 
 ## Installation
@@ -236,7 +237,27 @@
 
 ```python
 t = Table(["Id", "Description"], alignment=[":--"])
 t >> ["1", "One"]
 t >> ["2", "Two"]
 doc >> t
 ```
+
+Since 1.3.0 it is now possible to easily embed tables in both lists and tables as follows:
+
+```python
+t = Table(["Id", "Description"], alignment=["--:"])
+t >> ["1", "One"]
+t >> ["2", UnorderedList(["Item a", "Item b"])]
+ul = UnorderedList(["Item 1", t, "Item 3"])
+doc >> ul
+```
+
+resulting in:
+
+>>>
+- Item 1
+- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+- Item 3
+>>>
+
+_Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

### Comparing `t_python_markdown-1.2.1/README.md` & `t_python_markdown-1.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -199,7 +199,27 @@
 
 ```python
 t = Table(["Id", "Description"], alignment=[":--"])
 t >> ["1", "One"]
 t >> ["2", "Two"]
 doc >> t
 ```
+
+Since 1.3.0 it is now possible to easily embed tables in both lists and tables as follows:
+
+```python
+t = Table(["Id", "Description"], alignment=["--:"])
+t >> ["1", "One"]
+t >> ["2", UnorderedList(["Item a", "Item b"])]
+ul = UnorderedList(["Item 1", t, "Item 3"])
+doc >> ul
+```
+
+resulting in:
+
+>>>
+- Item 1
+- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+- Item 3
+>>>
+
+_Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

### Comparing `t_python_markdown-1.2.1/pyproject.toml` & `t_python_markdown-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "t_python_markdown"
 description = "A simple to use markdown generator for Python."
 readme = "README.md"
-version = "1.2.1"
+version = "1.3.0"
 license = {file = "LICENSE"}
 keywords = ["markdown"]
 authors = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
 ]
 maintainers = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
@@ -20,13 +20,18 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "PyYAML"
 ]
 
+[project.optional-dependencies]
+dependencies = [
+    "markdown"
+]
+
 [project.urls]
 homepage = "https://www.cix.co.uk/~toyne/t-python-markdown/"
 documentation = "https://www.cix.co.uk/~toyne/t-python-markdown/"
 
 [tool.setuptools.packages]
 find = {}
```

### Comparing `t_python_markdown-1.2.1/t_python_markdown/__init__.py` & `t_python_markdown-1.3.0/t_python_markdown/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 from .t_python_markdown import BoldItalic
 from .t_python_markdown import Strikethrough
 from .t_python_markdown import Code
 from .t_python_markdown import CodeBlock
 from .t_python_markdown import UnorderedList
 from .t_python_markdown import OrderedList
 from .t_python_markdown import Table
+
+from .t_python_markdown import NotAllowedException
+from .t_python_markdown import BadFormatException
```

### Comparing `t_python_markdown-1.2.1/t_python_markdown/extensions/mkdocs.py` & `t_python_markdown-1.3.0/t_python_markdown/extensions/mkdocs.py`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.2.1/t_python_markdown/t_python_markdown.py` & `t_python_markdown-1.3.0/t_python_markdown/t_python_markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Simple markdown generator for Python."""
 import yaml
+try:
+  import markdown
+except:  # pylint: disable=W0702
+  markdown = None  # pylint: disable=C0103
 
 
 class NotAllowedException(Exception):
   """Not allowed exception"""
 
-  def __init__(self):
-    pass
+
+class BadFormatException(Exception):
+  """Bad formatting detected"""
 
 
 class MarkdownElement():
   """Top level markdown element"""
 
   def __init__(self, objects=None):
     if objects is None:
@@ -274,14 +279,22 @@
   """Represents markdown parent list (abstract)"""
 
   def __init__(self, o=None):
     if o is None:
       o = []
     super().__init__(o)
 
+  def _render(self, _parent):
+    _rv = super()._render(_parent)
+    if isinstance(_parent, Table):
+      if markdown:
+        return markdown.markdown(_rv).replace("\n", "")
+      raise BadFormatException(f"Cannot embed List in {_parent.__class__.__name__} without markdown package.")
+    return _rv
+
   def _render_item(self, _parent, _child, _item):
     _pad = "".join(" " for _ in range(self.__check_indent(self) * 3))
     _rv = self._render_list_item(isinstance(_child, (List)), _pad, "".join(_item))
     return _rv
 
   def _render_list_item(self, _child_is_list, _pad, _item):
     raise NotAllowedException()
@@ -337,14 +350,18 @@
     self.__alignment = alignment[0:_lh]
     self.__alignment.extend([next(reversed(alignment), ":-:") for _ in range(_lh - len(alignment))])
 
   def _render(self, _parent):
     _rv = super()._render(_parent)
     header = "|" + "|".join(list(self.__format_header(x) for x in self.__heading)) + "|"
     alignment = "|" + "|".join(list(f" {_} " for _ in self.__alignment)) + "|"
+    if isinstance(_parent, (Table, List)):
+      if markdown:
+        return markdown.markdown(f"{header}\n{alignment}\n{_rv}", extensions=['tables']).replace("\n", "")
+      raise BadFormatException(f"Cannot embed Table in {_parent.__class__.__name__} without markdown package.")
     return f"\n\n{header}\n{alignment}\n{_rv}\n"
 
   def __format_header(self, _o):
     if _o:
       return f" **{_o}** "
     return ""
```

### Comparing `t_python_markdown-1.2.1/t_python_markdown.egg-info/PKG-INFO` & `t_python_markdown-1.3.0/t_python_markdown.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t-python-markdown
-Version: 1.2.1
+Version: 1.3.0
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -29,14 +29,15 @@
 Project-URL: homepage, https://www.cix.co.uk/~toyne/t-python-markdown/
 Project-URL: documentation, https://www.cix.co.uk/~toyne/t-python-markdown/
 Keywords: markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dependencies
 License-File: LICENSE
 
 # t-python-markdown
 
 A simple to use markdown generator for Python.
 
 ## Installation
@@ -236,7 +237,27 @@
 
 ```python
 t = Table(["Id", "Description"], alignment=[":--"])
 t >> ["1", "One"]
 t >> ["2", "Two"]
 doc >> t
 ```
+
+Since 1.3.0 it is now possible to easily embed tables in both lists and tables as follows:
+
+```python
+t = Table(["Id", "Description"], alignment=["--:"])
+t >> ["1", "One"]
+t >> ["2", UnorderedList(["Item a", "Item b"])]
+ul = UnorderedList(["Item 1", t, "Item 3"])
+doc >> ul
+```
+
+resulting in:
+
+>>>
+- Item 1
+- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+- Item 3
+>>>
+
+_Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

