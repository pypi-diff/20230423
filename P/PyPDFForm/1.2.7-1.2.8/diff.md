# Comparing `tmp/PyPDFForm-1.2.7.tar.gz` & `tmp/PyPDFForm-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.7.tar", last modified: Sat Apr  8 16:18:06 2023, max compression
+gzip compressed data, was "PyPDFForm-1.2.8.tar", last modified: Sun Apr 23 16:09:49 2023, max compression
```

## Comparing `PyPDFForm-1.2.7.tar` & `PyPDFForm-1.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.059944 PyPDFForm-1.2.8/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/setup.py
```

### Comparing `PyPDFForm-1.2.7/LICENSE` & `PyPDFForm-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PKG-INFO` & `PyPDFForm-1.2.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-Metadata-Version: 2.1
-Name: PyPDFForm
-Version: 1.2.7
-Summary: The Python library for PDF forms.
-Home-page: https://github.com/chinapandaman/PyPDFForm
-Author: Jinge Li
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating 
 a Python dictionary with keys matching its annotated names
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.7 Summary: The Python
-library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
-Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
-    chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
+chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
+                    //static.pepy.tech/personalized-badge/
+pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+             [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
 out the GitHub repository for a live demo if you can't see it here.](https://
```

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/constants.py` & `PyPDFForm-1.2.8/PyPDFForm/core/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/filler.py` & `PyPDFForm-1.2.8/PyPDFForm/core/filler.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/font.py` & `PyPDFForm-1.2.8/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/image.py` & `PyPDFForm-1.2.8/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/patterns.py` & `PyPDFForm-1.2.8/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/template.py` & `PyPDFForm-1.2.8/PyPDFForm/core/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,23 @@
 
     try:
         return "{0:b}".format(int(element[constants.FIELD_FLAG_KEY]))[::-1][24] == "1"
     except IndexError:
         return False
 
 
+def is_text_multiline(element: pdfrw.PdfDict) -> bool:
+    """Returns true if a text field is a paragraph field."""
+
+    try:
+        return "{0:b}".format(int(element[constants.FIELD_FLAG_KEY]))[::-1][12] == "1"
+    except (IndexError, TypeError):
+        return False
+
+
 def get_dropdown_choices(element: pdfrw.PdfDict) -> Union[Tuple[str], None]:
     """Returns string options of a dropdown field."""
 
     result = None
     for pattern in DROPDOWN_CHOICE_PATTERNS:
         choices = traverse_pattern(pattern, element)
         if choices:
@@ -274,14 +283,17 @@
                 ) / 2
 
     string_height = element_middleware.font_size * 96 / 72
     height_mid_point = (
         float(element[constants.ANNOTATION_RECTANGLE_KEY][1])
         + float(element[constants.ANNOTATION_RECTANGLE_KEY][3])
     ) / 2
+    y = (height_mid_point - string_height / 2 + height_mid_point) / 2
+    if is_text_multiline(element):
+        y = float(element[constants.ANNOTATION_RECTANGLE_KEY][3]) - string_height / 2
 
     return (
         x
         - (
             character_paddings[0]
             + stringWidth(
                 element_value[:1],
@@ -293,9 +305,9 @@
                 element_middleware.comb is True
                 and length != 0
                 and length % 2 == 0
                 and int(alignment) == 1
             )
             else 0
         ),
-        (height_mid_point - string_height / 2 + height_mid_point) / 2,
+        y,
     )
```

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/utils.py` & `PyPDFForm-1.2.8/PyPDFForm/core/utils.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/core/watermark.py` & `PyPDFForm-1.2.8/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/element.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/template.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/middleware/text.py` & `PyPDFForm-1.2.8/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm/wrapper.py` & `PyPDFForm-1.2.8/PyPDFForm/wrapper.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.7
+Version: 1.2.8
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,14 +13,16 @@
 
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating 
 a Python dictionary with keys matching its annotated names
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.7 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.8 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
-    chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
+chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
+                    //static.pepy.tech/personalized-badge/
+pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+             [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
 out the GitHub repository for a live demo if you can't see it here.](https://
```

### Comparing `PyPDFForm-1.2.7/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.2.8/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.7/README.md` & `PyPDFForm-1.2.8/PyPDFForm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+Metadata-Version: 2.1
+Name: PyPDFForm
+Version: 1.2.8
+Summary: The Python library for PDF forms.
+Home-page: https://github.com/chinapandaman/PyPDFForm
+Author: Jinge Li
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating 
 a Python dictionary with keys matching its annotated names
```

#### html2text {}

```diff
@@ -1,13 +1,22 @@
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.8 Summary: The Python
+library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
+Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
-    chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
+chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
+                    //static.pepy.tech/personalized-badge/
+pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+             [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
 out the GitHub repository for a live demo if you can't see it here.](https://
```

### Comparing `PyPDFForm-1.2.7/setup.py` & `PyPDFForm-1.2.8/setup.py`

 * *Files identical despite different names*

