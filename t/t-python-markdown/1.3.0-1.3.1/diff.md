# Comparing `tmp/t_python_markdown-1.3.0.tar.gz` & `tmp/t_python_markdown-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_python_markdown-1.3.0.tar", last modified: Sat Apr 22 23:25:21 2023, max compression
+gzip compressed data, was "t_python_markdown-1.3.1.tar", last modified: Sun Apr 23 16:05:36 2023, max compression
```

## Comparing `t_python_markdown-1.3.0.tar` & `t_python_markdown-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7527 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 23:25:21.869182 t_python_markdown-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.867182 t_python_markdown-1.3.0/t_python_markdown/
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.868182 t_python_markdown-1.3.0/t_python_markdown/extensions/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/extensions/mkdocs.py
--rw-rw-rw-   0 root         (0) root         (0)    10268 2023-04-22 23:25:01.000000 t_python_markdown-1.3.0/t_python_markdown/t_python_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 23:25:21.868182 t_python_markdown-1.3.0/t_python_markdown.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7527 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-22 23:25:21.000000 t_python_markdown-1.3.0/t_python_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 16:05:36.193213 t_python_markdown-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7525 2023-04-23 16:05:36.192213 t_python_markdown-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5652 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 16:05:36.193213 t_python_markdown-1.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 16:05:36.191213 t_python_markdown-1.3.1/t_python_markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/t_python_markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 16:05:36.192213 t_python_markdown-1.3.1/t_python_markdown/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/t_python_markdown/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/t_python_markdown/extensions/mkdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10281 2023-04-23 16:05:13.000000 t_python_markdown-1.3.1/t_python_markdown/t_python_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 16:05:36.192213 t_python_markdown-1.3.1/t_python_markdown.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7525 2023-04-23 16:05:36.000000 t_python_markdown-1.3.1/t_python_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-23 16:05:36.000000 t_python_markdown-1.3.1/t_python_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 16:05:36.000000 t_python_markdown-1.3.1/t_python_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-23 16:05:36.000000 t_python_markdown-1.3.1/t_python_markdown.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-23 16:05:36.000000 t_python_markdown-1.3.1/t_python_markdown.egg-info/top_level.txt
```

### Comparing `t_python_markdown-1.3.0/LICENSE` & `t_python_markdown-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.3.0/PKG-INFO` & `t_python_markdown-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_python_markdown
-Version: 1.3.0
+Version: 1.3.1
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -250,14 +250,12 @@
 t >> ["2", UnorderedList(["Item a", "Item b"])]
 ul = UnorderedList(["Item 1", t, "Item 3"])
 doc >> ul
 ```
 
 resulting in:
 
->>>
-- Item 1
-- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
-- Item 3
->>>
+> - Item 1
+> - <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+> - Item 3
 
 _Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

### Comparing `t_python_markdown-1.3.0/README.md` & `t_python_markdown-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,12 @@
 t >> ["2", UnorderedList(["Item a", "Item b"])]
 ul = UnorderedList(["Item 1", t, "Item 3"])
 doc >> ul
 ```
 
 resulting in:
 
->>>
-- Item 1
-- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
-- Item 3
->>>
+> - Item 1
+> - <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+> - Item 3
 
-_Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
+_Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

### Comparing `t_python_markdown-1.3.0/pyproject.toml` & `t_python_markdown-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "t_python_markdown"
 description = "A simple to use markdown generator for Python."
 readme = "README.md"
-version = "1.3.0"
+version = "1.3.1"
 license = {file = "LICENSE"}
 keywords = ["markdown"]
 authors = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
 ]
 maintainers = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
```

### Comparing `t_python_markdown-1.3.0/t_python_markdown/__init__.py` & `t_python_markdown-1.3.1/t_python_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.3.0/t_python_markdown/extensions/mkdocs.py` & `t_python_markdown-1.3.1/t_python_markdown/extensions/mkdocs.py`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.3.0/t_python_markdown/t_python_markdown.py` & `t_python_markdown-1.3.1/t_python_markdown/t_python_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 
   def _render(self, _parent):
     _rv = super()._render(_parent)
     header = "|" + "|".join(list(self.__format_header(x) for x in self.__heading)) + "|"
     alignment = "|" + "|".join(list(f" {_} " for _ in self.__alignment)) + "|"
     if isinstance(_parent, (Table, List)):
       if markdown:
-        return markdown.markdown(f"{header}\n{alignment}\n{_rv}", extensions=['tables']).replace("\n", "")
+        return markdown.markdown(f"{header}\n{alignment}\n{_rv}", extensions=['tables', 'attr_list']).replace("\n", "")
       raise BadFormatException(f"Cannot embed Table in {_parent.__class__.__name__} without markdown package.")
     return f"\n\n{header}\n{alignment}\n{_rv}\n"
 
   def __format_header(self, _o):
     if _o:
       return f" **{_o}** "
     return ""
```

### Comparing `t_python_markdown-1.3.0/t_python_markdown.egg-info/PKG-INFO` & `t_python_markdown-1.3.1/t_python_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t-python-markdown
-Version: 1.3.0
+Version: 1.3.1
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -250,14 +250,12 @@
 t >> ["2", UnorderedList(["Item a", "Item b"])]
 ul = UnorderedList(["Item 1", t, "Item 3"])
 doc >> ul
 ```
 
 resulting in:
 
->>>
-- Item 1
-- <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
-- Item 3
->>>
+> - Item 1
+> - <table><thead><tr><th style="text-align: right;"><strong>Id</strong></th><th style="text-align: right;"><strong>Description</strong></th></tr></thead><tbody><tr><td style="text-align: right;">1</td><td style="text-align: right;">One</td></tr><tr><td style="text-align: right;">2</td><td style="text-align: right;"><ul><li>Item a</li><li>Item b</li></ul></td></tr></tbody></table>
+> - Item 3
 
 _Note: Embedding requires the [Markdown](https://pypi.org/project/Markdown/) package to be installed._
```

