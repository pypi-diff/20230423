# Comparing `tmp/one_block-0.1.3.tar.gz` & `tmp/one_block-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one_block-0.1.3.tar", max compression
+gzip compressed data, was "one_block-0.1.4.tar", max compression
```

## Comparing `one_block-0.1.3.tar` & `one_block-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1074 2023-04-23 13:49:22.083825 one_block-0.1.3/LICENSE
--rw-r--r--   0        0        0     1306 2023-04-23 13:49:22.083825 one_block-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-23 13:49:22.083825 one_block-0.1.3/one_block/__init__.py
--rw-r--r--   0        0        0      318 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/__init__.py
--rw-r--r--   0        0        0       90 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/accessory.py
--rw-r--r--   0        0        0      903 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/button.py
--rw-r--r--   0        0        0      500 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/checkbox.py
--rw-r--r--   0        0        0      611 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/option.py
--rw-r--r--   0        0        0      415 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/overflow.py
--rw-r--r--   0        0        0     1314 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/picker.py
--rw-r--r--   0        0        0      454 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/radio.py
--rw-r--r--   0        0        0     2631 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/accessory/selects.py
--rw-r--r--   0        0        0       23 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/actions/__init__.py
--rw-r--r--   0        0        0      353 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/actions/actions.py
--rw-r--r--   0        0        0      641 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/base.py
--rw-r--r--   0        0        0       29 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/context/__init__.py
--rw-r--r--   0        0        0      301 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/context/context.py
--rw-r--r--   0        0        0       27 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/divider/__init__.py
--rw-r--r--   0        0        0      132 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/divider/plain.py
--rw-r--r--   0        0        0       22 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/header/__init__.py
--rw-r--r--   0        0        0      244 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/header/header.py
--rw-r--r--   0        0        0       21 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/image/__init__.py
--rw-r--r--   0        0        0      577 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/image/image.py
--rw-r--r--   0        0        0       49 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/input_blocks/__init__.py
--rw-r--r--   0        0        0      574 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/input_blocks/plain_text_input.py
--rw-r--r--   0        0        0      434 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/input_blocks/selects.py
--rw-r--r--   0        0        0      693 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/input_blocks/text_input.py
--rw-r--r--   0        0        0      143 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/__init__.py
--rw-r--r--   0        0        0      549 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/button.py
--rw-r--r--   0        0        0      426 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/checkbox.py
--rw-r--r--   0        0        0      420 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/image.py
--rw-r--r--   0        0        0      262 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/markdown.py
--rw-r--r--   0        0        0      426 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/overflow.py
--rw-r--r--   0        0        0      878 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/picker.py
--rw-r--r--   0        0        0      267 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/plain_text.py
--rw-r--r--   0        0        0      434 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/radio_buttons.py
--rw-r--r--   0        0        0     2059 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/selects.py
--rw-r--r--   0        0        0      327 2023-04-23 13:49:22.087825 one_block-0.1.3/one_block/section/text_fields.py
--rw-r--r--   0        0        0     1007 2023-04-23 13:49:22.087825 one_block-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 one_block-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-23 13:53:54.748519 one_block-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1306 2023-04-23 13:53:54.748519 one_block-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/accessory.py
+-rw-r--r--   0        0        0      903 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/button.py
+-rw-r--r--   0        0        0      500 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/checkbox.py
+-rw-r--r--   0        0        0      611 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/option.py
+-rw-r--r--   0        0        0      415 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/overflow.py
+-rw-r--r--   0        0        0     1314 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/picker.py
+-rw-r--r--   0        0        0      454 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/radio.py
+-rw-r--r--   0        0        0     2630 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/accessory/selects.py
+-rw-r--r--   0        0        0       23 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/actions/__init__.py
+-rw-r--r--   0        0        0      353 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/actions/actions.py
+-rw-r--r--   0        0        0      641 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/base.py
+-rw-r--r--   0        0        0       29 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/context/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/context/context.py
+-rw-r--r--   0        0        0       27 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/divider/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/divider/plain.py
+-rw-r--r--   0        0        0       22 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/header/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/header/header.py
+-rw-r--r--   0        0        0       21 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/image/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/image/image.py
+-rw-r--r--   0        0        0       49 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/input_blocks/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/input_blocks/plain_text_input.py
+-rw-r--r--   0        0        0      434 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/input_blocks/selects.py
+-rw-r--r--   0        0        0      693 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/input_blocks/text_input.py
+-rw-r--r--   0        0        0      143 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/__init__.py
+-rw-r--r--   0        0        0      549 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/button.py
+-rw-r--r--   0        0        0      426 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/checkbox.py
+-rw-r--r--   0        0        0      420 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/image.py
+-rw-r--r--   0        0        0      262 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/markdown.py
+-rw-r--r--   0        0        0      426 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/overflow.py
+-rw-r--r--   0        0        0      878 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/picker.py
+-rw-r--r--   0        0        0      267 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/plain_text.py
+-rw-r--r--   0        0        0      434 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/radio_buttons.py
+-rw-r--r--   0        0        0     2059 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/selects.py
+-rw-r--r--   0        0        0      327 2023-04-23 13:53:54.748519 one_block-0.1.4/one_block/section/text_fields.py
+-rw-r--r--   0        0        0     1007 2023-04-23 13:53:54.748519 one_block-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 one_block-0.1.4/PKG-INFO
```

### Comparing `one_block-0.1.3/LICENSE` & `one_block-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/README.md` & `one_block-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/accessory/button.py` & `one_block-0.1.4/one_block/accessory/button.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/accessory/option.py` & `one_block-0.1.4/one_block/accessory/option.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/accessory/picker.py` & `one_block-0.1.4/one_block/accessory/picker.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/accessory/selects.py` & `one_block-0.1.4/one_block/accessory/selects.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             ]
         }
         return base
 
 
 class ConversationSelect(Accessory):
     def __init__(self, placeholder, action_id, initial=None, multi=False):
-        self.placeholder = base.BaseText(placeholderg)
+        self.placeholder = base.BaseText(placeholder)
         self.action_id = action_id
         self.initial = initial
         self.multi = multi
 
     def json(self):
         select_type = 'conversations_select' if not self.multi else 'multi_conversations_select'
         base = {
```

### Comparing `one_block-0.1.3/one_block/base.py` & `one_block-0.1.4/one_block/base.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/image/image.py` & `one_block-0.1.4/one_block/image/image.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/input_blocks/plain_text_input.py` & `one_block-0.1.4/one_block/input_blocks/plain_text_input.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/input_blocks/text_input.py` & `one_block-0.1.4/one_block/input_blocks/text_input.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/section/button.py` & `one_block-0.1.4/one_block/section/button.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/section/picker.py` & `one_block-0.1.4/one_block/section/picker.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/one_block/section/selects.py` & `one_block-0.1.4/one_block/section/selects.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.3/pyproject.toml` & `one_block-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one-block"
-version = "0.1.3"
+version = "0.1.4"
 description = "An easy-to-use, opinionated slack blockkit implementation"
 authors = ["Dragos Dumitrache <dragos@afterburner.dev>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "one_block"}]
```

### Comparing `one_block-0.1.3/PKG-INFO` & `one_block-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-block
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy-to-use, opinionated slack blockkit implementation
 License: MIT
 Author: Dragos Dumitrache
 Author-email: dragos@afterburner.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

