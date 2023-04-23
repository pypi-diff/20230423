# Comparing `tmp/tkinter_form-0.1.4.1.tar.gz` & `tmp/tkinter_form-0.1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_form-0.1.4.1.tar", last modified: Fri Apr 21 09:27:22 2023, max compression
+gzip compressed data, was "tkinter_form-0.1.5.0.tar", last modified: Sun Apr 23 06:15:42 2023, max compression
```

## Comparing `tkinter_form-0.1.4.1.tar` & `tkinter_form-0.1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.199248 tkinter_form-0.1.4.1/
--rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.4.1/LICENSE
--rw-rw-rw-   0        0        0     2809 2023-04-21 09:27:22.198248 tkinter_form-0.1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 09:27:22.199248 tkinter_form-0.1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-04-21 09:26:56.000000 tkinter_form-0.1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.180244 tkinter_form-0.1.4.1/tkinter_form/
--rw-rw-rw-   0        0        0       44 2023-04-21 09:19:56.000000 tkinter_form-0.1.4.1/tkinter_form/__init__.py
--rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.4.1/tkinter_form/tkinter_form.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.197248 tkinter_form-0.1.4.1/tkinter_form.egg-info/
--rw-rw-rw-   0        0        0     2809 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 06:15:42.080705 tkinter_form-0.1.5.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    10526 2023-04-23 06:15:42.079705 tkinter_form-0.1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:15:42.080705 tkinter_form-0.1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-04-23 06:15:16.000000 tkinter_form-0.1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:15:42.051699 tkinter_form-0.1.5.0/tkinter_form/
+-rw-rw-rw-   0        0        0       44 2023-04-21 09:19:56.000000 tkinter_form-0.1.5.0/tkinter_form/__init__.py
+-rw-rw-rw-   0        0        0     8204 2023-04-23 06:10:08.000000 tkinter_form-0.1.5.0/tkinter_form/tkinter_form.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:15:42.077704 tkinter_form-0.1.5.0/tkinter_form.egg-info/
+-rw-rw-rw-   0        0        0    10526 2023-04-23 06:15:41.000000 tkinter_form-0.1.5.0/tkinter_form.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-23 06:15:41.000000 tkinter_form-0.1.5.0/tkinter_form.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:15:41.000000 tkinter_form-0.1.5.0/tkinter_form.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-04-23 06:15:41.000000 tkinter_form-0.1.5.0/tkinter_form.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 06:15:41.000000 tkinter_form-0.1.5.0/tkinter_form.egg-info/top_level.txt
```

### Comparing `tkinter_form-0.1.4.1/LICENSE` & `tkinter_form-0.1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.4.1/setup.py` & `tkinter_form-0.1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "readme.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.4.1"
+VERSION = "0.1.5.0"
 DESCRIPTION = "form for tkinter"
 LONG_DESCRIPTION = "create a form for tkinter from a base dictionary"
 
 # Setting up
 setup(
     name="tkinter_form",
     version=VERSION,
```

### Comparing `tkinter_form-0.1.4.1/tkinter_form/tkinter_form.py` & `tkinter_form-0.1.5.0/tkinter_form/tkinter_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,29 +191,31 @@
         self.widgets = {}
         self.__vars = {}
         for index, dict_vals in enumerate(form_dict.items()):
             name_key = dict_vals[0]
             value = dict_vals[1]
 
             type_value = str(type(value))[8:-2]
-
+            tk.Grid.rowconfigure(self, index, weight=1)
             if type_value == "dict":
                 widget = Form(self, name_key, value, button=False)
                 widget.grid(row=index, column=0, columnspan=2, sticky="nesw")
 
                 self.__vars[name_key] = widget
                 self.widgets[name_key] = widget
 
                 continue
 
             variable = self.__type_vars[type_value]()
             self.__vars[name_key] = variable
             widget = self.__type_widgets[type_value](self)
+            tk.Grid.columnconfigure(self, 1, weight=1)
             widget.grid(row=index, column=1, sticky="nesw", padx=2, pady=2)
             label = ttk.Label(self, text=name_key)
+            tk.Grid.columnconfigure(self, 0, weight=1)
             label.grid(row=index, column=0, sticky="nes", padx=2, pady=2)
 
             config = self.__configure_widgets[type_value]
 
             config(widget, variable, value)
 
             self.widgets[name_key] = [label, widget]
@@ -254,7 +256,24 @@
 
         Args:
             set_dict (dict): values to be set
 
         """
         for key, var in set_dict.items():
             self.__vars[key].set(var)
+
+    def set_labels_text(self, set_labels: dict) -> None:
+        """
+        Edit text labels Interfaces
+
+        Args:
+            set_labels (dict): labels to_edit
+        """
+        for key, var_name in set_labels.items():
+            if key == "__form__":
+                self.config(text=var_name)
+                continue
+            if isinstance(var_name, dict):
+                self.widgets[key].set_labels_text(var_name)
+                continue
+
+            self.widgets[key][0].config(text=var_name)
```

