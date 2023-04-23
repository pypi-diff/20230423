# Comparing `tmp/guitk-0.2.0.tar.gz` & `tmp/guitk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitk-0.2.0.tar", max compression
+gzip compressed data, was "guitk-0.2.1.tar", max compression
```

## Comparing `guitk-0.2.0.tar` & `guitk-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.2.0/LICENSE
--rw-r--r--   0        0        0    18513 2023-04-23 16:49:39.117174 guitk-0.2.0/README.md
--rw-r--r--   0        0        0     1095 2023-04-23 16:48:12.838095 guitk-0.2.0/guitk/__init__.py
--rw-r--r--   0        0        0    18484 2023-04-23 16:48:12.838425 guitk-0.2.0/guitk/__main__.py
--rw-r--r--   0        0        0      195 2023-04-23 16:48:12.838685 guitk-0.2.0/guitk/constants.py
--rw-r--r--   0        0        0     2844 2021-03-10 13:52:24.000000 guitk-0.2.0/guitk/redirect.py
--rw-r--r--   0        0        0     2726 2023-04-23 16:48:12.838952 guitk-0.2.0/guitk/tkroot.py
--rw-r--r--   0        0        0     8651 2021-03-08 00:27:37.000000 guitk-0.2.0/guitk/tooltips.py
--rw-r--r--   0        0        0      268 2023-04-23 16:48:12.839131 guitk-0.2.0/guitk/utils.py
--rw-r--r--   0        0        0     1644 2023-04-23 16:48:12.839399 guitk-0.2.0/guitk/widgets/__init__.py
--rw-r--r--   0        0        0     1328 2023-04-23 16:48:12.839615 guitk-0.2.0/guitk/widgets/debugwindow.py
--rw-r--r--   0        0        0     1827 2023-04-23 16:48:12.839823 guitk-0.2.0/guitk/widgets/events.py
--rw-r--r--   0        0        0     3414 2023-04-23 16:48:12.840033 guitk-0.2.0/guitk/widgets/menu.py
--rw-r--r--   0        0        0    10075 2023-04-23 16:48:12.840354 guitk-0.2.0/guitk/widgets/tk_text.py
--rw-r--r--   0        0        0    11231 2023-04-23 16:48:12.840598 guitk-0.2.0/guitk/widgets/ttk_button.py
--rw-r--r--   0        0        0     4309 2023-04-23 16:48:12.840841 guitk-0.2.0/guitk/widgets/ttk_checkbutton.py
--rw-r--r--   0        0        0     3656 2023-04-23 16:48:12.841086 guitk-0.2.0/guitk/widgets/ttk_combobox.py
--rw-r--r--   0        0        0     8950 2023-04-23 16:48:12.841321 guitk-0.2.0/guitk/widgets/ttk_entry.py
--rw-r--r--   0        0        0     6852 2023-04-23 16:48:12.841549 guitk-0.2.0/guitk/widgets/ttk_label.py
--rw-r--r--   0        0        0     5150 2023-04-23 16:48:12.841698 guitk-0.2.0/guitk/widgets/ttk_notebook.py
--rw-r--r--   0        0        0     4655 2023-04-23 16:48:12.841843 guitk-0.2.0/guitk/widgets/ttk_progressbar.py
--rw-r--r--   0        0        0     5496 2023-04-23 16:48:12.841992 guitk-0.2.0/guitk/widgets/ttk_radiobutton.py
--rw-r--r--   0        0        0     4462 2023-04-23 16:48:12.842174 guitk-0.2.0/guitk/widgets/ttk_scale.py
--rw-r--r--   0        0        0    11640 2023-04-23 16:48:12.842326 guitk-0.2.0/guitk/widgets/ttk_treeview.py
--rw-r--r--   0        0        0      290 2023-04-23 16:48:12.842435 guitk-0.2.0/guitk/widgets/types.py
--rw-r--r--   0        0        0     1842 2023-04-23 16:48:12.842626 guitk-0.2.0/guitk/widgets/utils.py
--rw-r--r--   0        0        0     2875 2023-04-23 16:48:12.842845 guitk-0.2.0/guitk/widgets/widget.py
--rw-r--r--   0        0        0    20899 2023-04-23 16:48:12.843138 guitk-0.2.0/guitk/widgets/window.py
--rw-r--r--   0        0        0      590 2023-04-23 16:50:37.646756 guitk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    19669 1970-01-01 00:00:00.000000 guitk-0.2.0/setup.py
--rw-r--r--   0        0        0    19085 1970-01-01 00:00:00.000000 guitk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.2.1/LICENSE
+-rw-r--r--   0        0        0    18916 2023-04-23 18:56:54.325743 guitk-0.2.1/README.md
+-rw-r--r--   0        0        0     1095 2023-04-23 18:58:08.640279 guitk-0.2.1/guitk/__init__.py
+-rw-r--r--   0        0        0    18484 2023-02-17 19:39:03.000000 guitk-0.2.1/guitk/__main__.py
+-rw-r--r--   0        0        0      195 2023-02-14 15:07:46.000000 guitk-0.2.1/guitk/constants.py
+-rw-r--r--   0        0        0     2844 2021-03-10 13:52:24.000000 guitk-0.2.1/guitk/redirect.py
+-rw-r--r--   0        0        0     2726 2023-02-17 17:18:36.000000 guitk-0.2.1/guitk/tkroot.py
+-rw-r--r--   0        0        0     8651 2021-03-08 00:27:37.000000 guitk-0.2.1/guitk/tooltips.py
+-rw-r--r--   0        0        0      268 2023-02-15 06:15:34.000000 guitk-0.2.1/guitk/utils.py
+-rw-r--r--   0        0        0     1644 2023-04-23 16:31:21.000000 guitk-0.2.1/guitk/widgets/__init__.py
+-rw-r--r--   0        0        0     1328 2023-02-16 14:26:34.000000 guitk-0.2.1/guitk/widgets/debugwindow.py
+-rw-r--r--   0        0        0     1827 2023-02-16 05:38:10.121090 guitk-0.2.1/guitk/widgets/events.py
+-rw-r--r--   0        0        0     3414 2023-02-15 06:05:03.000000 guitk-0.2.1/guitk/widgets/menu.py
+-rw-r--r--   0        0        0    10075 2023-04-23 15:10:08.000000 guitk-0.2.1/guitk/widgets/tk_text.py
+-rw-r--r--   0        0        0    11231 2023-02-18 21:33:17.000000 guitk-0.2.1/guitk/widgets/ttk_button.py
+-rw-r--r--   0        0        0     4309 2023-04-23 16:27:37.000000 guitk-0.2.1/guitk/widgets/ttk_checkbutton.py
+-rw-r--r--   0        0        0     3656 2023-04-23 16:26:00.000000 guitk-0.2.1/guitk/widgets/ttk_combobox.py
+-rw-r--r--   0        0        0     8950 2023-04-23 15:10:08.000000 guitk-0.2.1/guitk/widgets/ttk_entry.py
+-rw-r--r--   0        0        0     6852 2023-04-22 15:34:37.000000 guitk-0.2.1/guitk/widgets/ttk_label.py
+-rw-r--r--   0        0        0     5150 2023-04-23 16:28:15.000000 guitk-0.2.1/guitk/widgets/ttk_notebook.py
+-rw-r--r--   0        0        0     4655 2023-04-23 16:28:49.000000 guitk-0.2.1/guitk/widgets/ttk_progressbar.py
+-rw-r--r--   0        0        0     5496 2023-04-23 16:29:42.000000 guitk-0.2.1/guitk/widgets/ttk_radiobutton.py
+-rw-r--r--   0        0        0     4462 2023-04-22 16:14:22.000000 guitk-0.2.1/guitk/widgets/ttk_scale.py
+-rw-r--r--   0        0        0    11640 2023-04-23 16:26:50.000000 guitk-0.2.1/guitk/widgets/ttk_treeview.py
+-rw-r--r--   0        0        0      290 2023-04-22 15:10:54.000000 guitk-0.2.1/guitk/widgets/types.py
+-rw-r--r--   0        0        0     1842 2023-02-17 18:33:45.000000 guitk-0.2.1/guitk/widgets/utils.py
+-rw-r--r--   0        0        0     2875 2023-02-18 17:40:47.000000 guitk-0.2.1/guitk/widgets/widget.py
+-rw-r--r--   0        0        0    20899 2023-04-22 16:40:19.000000 guitk-0.2.1/guitk/widgets/window.py
+-rw-r--r--   0        0        0      590 2023-04-23 18:58:08.641233 guitk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    19488 1970-01-01 00:00:00.000000 guitk-0.2.1/PKG-INFO
```

### Comparing `guitk-0.2.0/LICENSE` & `guitk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/README.md` & `guitk-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-<!-- DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->
+<!-* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->
 
 # Python GUI Toolkit for TK (guitk)
 
 ## Synopsis
 
 guitk is an experiment to design a lightweight framework that simplifies creating simple GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html).  This is very much early alpha stage but in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
 ## Code Example
 
-![hello.py example](examples/hello.py.png "Hello World example")
+![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk
 
 
@@ -40,31 +40,29 @@
 # run your event loop
 if __name__ == "__main__":
     HelloWindow().run()
 ```
 
 ## Motivation
 
-I did not set out to create yet another python GUI framework -- there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
+I did not set out to create yet another python GUI framework -* there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
 
 I settled on using tkinter because it's included with python, well-supported on multiple platforms, and relatively light-weight.  However, I found tkinter took a bit too much boiler plate compared to PySimpleGUI and I missed the simplicity of PySimpleGUI's single event loop for quick prototyping.  
 
 guitk is my attempt to provide an event-loop interface to tkinter.  It is not intended to abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.  guitk also provides a callback style interface if you prefer that over a single event-loop.
 
 ## Installation
 
-* `git clone git@github.com:RhetTbull/guitk.git`
-* `cd guitk`
-* `python3 setup.py install`
+* `python3 -m pip install guitk`
 
 Once this gets past the early alpha stage, I'll package for PyPI.
 
 ## Anatomy of a guitk program 
 
-![hello2.py example](examples/hello2.py.png "Hello World example")
+![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk
 
 
@@ -194,15 +192,15 @@
     # instantiate your Window class and run it
     name = HelloWorld().run()
     print(f"HelloWorld: {name}")
 ```
 
 guitk GUIs are created using a lists of lists where each element in the lists corresponds to a ttk or tk element.  This design pattern is borrowed from PySimpleGUI.
 
-![layout_lol.py example](examples/layouts_lol.py.png "Layout using lists of lists example")
+![layout_lol.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/layouts_lol.py.png "Layout using lists of lists example")
 
 ```python
 """ Example for guitk showing how to use lists of lists for creating GUI layout """
 
 import guitk
 
 
@@ -223,15 +221,15 @@
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 Because layouts are simply lists of lists, you can use python to create layouts programmatically, for example using list comprehensions.
 
 
-![layout2.py example](examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
+![layout2.py example](https://github.com/RhetTbull/guitk/raw/main/examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
 
 ```python
 """ Example for guitk showing how to use list comprehensions to create a GUI """
 
 import guitk
 
 
@@ -259,15 +257,15 @@
 
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 A more complex example showing how to use the event handler to react to events and change the value of other GUI elements.
 
-![hello4.py example](examples/hello4.py.png "A more complex example showing how to use the event handler.")
+![hello4.py example](https://github.com/RhetTbull/guitk/raw/main/examples/hello4.py.png "A more complex example showing how to use the event handler.")
 
 ```python
 """ Another Hello World example for guitk showing how to use the event handler """
 
 import guitk
 import tkinter as tk
 
@@ -348,15 +346,15 @@
     # add some padding around GUI elements to make it prettier
     HelloWorld().run()
 ```
 
 You can create virtual events that fire after a time delay and these can be repeating.
 
 
-![bind_timer_event example](examples/bind_timer_event.py.png "Creating timed virtual events.")
+![bind_timer_event example](https://github.com/RhetTbull/guitk/raw/main/examples/bind_timer_event.py.png "Creating timed virtual events.")
 
 ```python
 """ Example showing how to use bind_timer_event """
 
 import time
 import tkinter as tk
 
@@ -408,15 +406,15 @@
 
 if __name__ == "__main__":
     TimerWindow().run()
 ```
 
 You can access the underlying ttk widget, for example, to change style.  guitk also implements some additional widgets link `LinkLabel` which is a `ttk.Label()` that generates an event when clicked and changes mouse cursor to pointing hand (like a URL does).
 
-![LinkLabel example](examples/link.py.png "Using LinkLabel widget.")
+![LinkLabel example](https://github.com/RhetTbull/guitk/raw/main/examples/link.py.png "Using LinkLabel widget.")
 
 ```python
 """ Demonstrates use of LinkLabel widget """
 
 import guitk
 from tkinter import ttk
 
@@ -470,25 +468,29 @@
 
 ## Contributors
 
 Contributions welcome! If this project interests you, open an Issue or send a PR!
 
 ## TODO
 
-- [x] Basic prototype
-- [x] Frame
-- [x] Label
-- [x] Entry
-- [x] Button
-- [x] Checkbutton
-- [x] Text
-- [x] ScrolledText
-- [ ] Other widgets
-- [x] Tooltips
-- [ ] Documentation
-- [ ] Add docstrings
-- [ ] Add typehints to public API
-- [ ] Tests
+* [x] Basic prototype
+* [x] Frame
+* [x] Label
+* [x] Entry
+* [x] Button
+* [x] Checkbutton
+* [x] Radiobutton
+* [x] Text
+* [x] ScrolledText
+* [x] Treeview
+* [x] Listbox
+* [x] Combobox
+* [ ] Other widgets
+* [x] Tooltips
+* [ ] Documentation
+* [x] Add docstrings
+* [x] Add type hints to public API
+* [ ] Tests
 
 ## License
 
-MIT License with exception of `tooltips.py` which is licensed under the Python Software Foundation License Version 2.  Both are very permissive licenses.
+MIT License with exception of `tooltips.py` which is licensed under the Python Software Foundation License Version 2 because it includes code from the Python standard library. Both are very permissive licenses.
```

### Comparing `guitk-0.2.0/guitk/__init__.py` & `guitk-0.2.1/guitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # TODO: add way to specify tooltip delay
 # TODO: add style to all controls
 # TODO: standardize value_type
 
 from .tkroot import *
 from .widgets import *
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "Rhet Turnbull"
 
 __all__ = [
     "BrowseDirectoryButton",
     "BrowseFileButton",
     "Button",
     "CheckButton",
```

### Comparing `guitk-0.2.0/guitk/__main__.py` & `guitk-0.2.1/guitk/__main__.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/redirect.py` & `guitk-0.2.1/guitk/redirect.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/tkroot.py` & `guitk-0.2.1/guitk/tkroot.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/tooltips.py` & `guitk-0.2.1/guitk/tooltips.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/__init__.py` & `guitk-0.2.1/guitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/debugwindow.py` & `guitk-0.2.1/guitk/widgets/debugwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/events.py` & `guitk-0.2.1/guitk/widgets/events.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/menu.py` & `guitk-0.2.1/guitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/tk_text.py` & `guitk-0.2.1/guitk/widgets/tk_text.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_button.py` & `guitk-0.2.1/guitk/widgets/ttk_button.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_checkbutton.py` & `guitk-0.2.1/guitk/widgets/ttk_checkbutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_combobox.py` & `guitk-0.2.1/guitk/widgets/ttk_combobox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_entry.py` & `guitk-0.2.1/guitk/widgets/ttk_entry.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_label.py` & `guitk-0.2.1/guitk/widgets/ttk_label.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_notebook.py` & `guitk-0.2.1/guitk/widgets/ttk_notebook.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_progressbar.py` & `guitk-0.2.1/guitk/widgets/ttk_progressbar.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_radiobutton.py` & `guitk-0.2.1/guitk/widgets/ttk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_scale.py` & `guitk-0.2.1/guitk/widgets/ttk_scale.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/ttk_treeview.py` & `guitk-0.2.1/guitk/widgets/ttk_treeview.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/utils.py` & `guitk-0.2.1/guitk/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/widget.py` & `guitk-0.2.1/guitk/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/guitk/widgets/window.py` & `guitk-0.2.1/guitk/widgets/window.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.0/pyproject.toml` & `guitk-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guitk"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python."
 authors = ["Rhet Turnbull <rturnbull+git@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `guitk-0.2.0/PKG-INFO` & `guitk-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: guitk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.
 License: MIT
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-<!-- DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->
+<!-* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->
 
 # Python GUI Toolkit for TK (guitk)
 
 ## Synopsis
 
 guitk is an experiment to design a lightweight framework that simplifies creating simple GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html).  This is very much early alpha stage but in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
 ## Code Example
 
-![hello.py example](examples/hello.py.png "Hello World example")
+![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk
 
 
@@ -55,31 +55,29 @@
 # run your event loop
 if __name__ == "__main__":
     HelloWindow().run()
 ```
 
 ## Motivation
 
-I did not set out to create yet another python GUI framework -- there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
+I did not set out to create yet another python GUI framework -* there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
 
 I settled on using tkinter because it's included with python, well-supported on multiple platforms, and relatively light-weight.  However, I found tkinter took a bit too much boiler plate compared to PySimpleGUI and I missed the simplicity of PySimpleGUI's single event loop for quick prototyping.  
 
 guitk is my attempt to provide an event-loop interface to tkinter.  It is not intended to abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.  guitk also provides a callback style interface if you prefer that over a single event-loop.
 
 ## Installation
 
-* `git clone git@github.com:RhetTbull/guitk.git`
-* `cd guitk`
-* `python3 setup.py install`
+* `python3 -m pip install guitk`
 
 Once this gets past the early alpha stage, I'll package for PyPI.
 
 ## Anatomy of a guitk program 
 
-![hello2.py example](examples/hello2.py.png "Hello World example")
+![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk
 
 
@@ -209,15 +207,15 @@
     # instantiate your Window class and run it
     name = HelloWorld().run()
     print(f"HelloWorld: {name}")
 ```
 
 guitk GUIs are created using a lists of lists where each element in the lists corresponds to a ttk or tk element.  This design pattern is borrowed from PySimpleGUI.
 
-![layout_lol.py example](examples/layouts_lol.py.png "Layout using lists of lists example")
+![layout_lol.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/layouts_lol.py.png "Layout using lists of lists example")
 
 ```python
 """ Example for guitk showing how to use lists of lists for creating GUI layout """
 
 import guitk
 
 
@@ -238,15 +236,15 @@
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 Because layouts are simply lists of lists, you can use python to create layouts programmatically, for example using list comprehensions.
 
 
-![layout2.py example](examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
+![layout2.py example](https://github.com/RhetTbull/guitk/raw/main/examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
 
 ```python
 """ Example for guitk showing how to use list comprehensions to create a GUI """
 
 import guitk
 
 
@@ -274,15 +272,15 @@
 
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 A more complex example showing how to use the event handler to react to events and change the value of other GUI elements.
 
-![hello4.py example](examples/hello4.py.png "A more complex example showing how to use the event handler.")
+![hello4.py example](https://github.com/RhetTbull/guitk/raw/main/examples/hello4.py.png "A more complex example showing how to use the event handler.")
 
 ```python
 """ Another Hello World example for guitk showing how to use the event handler """
 
 import guitk
 import tkinter as tk
 
@@ -363,15 +361,15 @@
     # add some padding around GUI elements to make it prettier
     HelloWorld().run()
 ```
 
 You can create virtual events that fire after a time delay and these can be repeating.
 
 
-![bind_timer_event example](examples/bind_timer_event.py.png "Creating timed virtual events.")
+![bind_timer_event example](https://github.com/RhetTbull/guitk/raw/main/examples/bind_timer_event.py.png "Creating timed virtual events.")
 
 ```python
 """ Example showing how to use bind_timer_event """
 
 import time
 import tkinter as tk
 
@@ -423,15 +421,15 @@
 
 if __name__ == "__main__":
     TimerWindow().run()
 ```
 
 You can access the underlying ttk widget, for example, to change style.  guitk also implements some additional widgets link `LinkLabel` which is a `ttk.Label()` that generates an event when clicked and changes mouse cursor to pointing hand (like a URL does).
 
-![LinkLabel example](examples/link.py.png "Using LinkLabel widget.")
+![LinkLabel example](https://github.com/RhetTbull/guitk/raw/main/examples/link.py.png "Using LinkLabel widget.")
 
 ```python
 """ Demonstrates use of LinkLabel widget """
 
 import guitk
 from tkinter import ttk
 
@@ -485,26 +483,30 @@
 
 ## Contributors
 
 Contributions welcome! If this project interests you, open an Issue or send a PR!
 
 ## TODO
 
-- [x] Basic prototype
-- [x] Frame
-- [x] Label
-- [x] Entry
-- [x] Button
-- [x] Checkbutton
-- [x] Text
-- [x] ScrolledText
-- [ ] Other widgets
-- [x] Tooltips
-- [ ] Documentation
-- [ ] Add docstrings
-- [ ] Add typehints to public API
-- [ ] Tests
+* [x] Basic prototype
+* [x] Frame
+* [x] Label
+* [x] Entry
+* [x] Button
+* [x] Checkbutton
+* [x] Radiobutton
+* [x] Text
+* [x] ScrolledText
+* [x] Treeview
+* [x] Listbox
+* [x] Combobox
+* [ ] Other widgets
+* [x] Tooltips
+* [ ] Documentation
+* [x] Add docstrings
+* [x] Add type hints to public API
+* [ ] Tests
 
 ## License
 
-MIT License with exception of `tooltips.py` which is licensed under the Python Software Foundation License Version 2.  Both are very permissive licenses.
+MIT License with exception of `tooltips.py` which is licensed under the Python Software Foundation License Version 2 because it includes code from the Python standard library. Both are very permissive licenses.
```

