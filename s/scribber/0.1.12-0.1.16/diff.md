# Comparing `tmp/scribber-0.1.12.tar.gz` & `tmp/scribber-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribber-0.1.12.tar", last modified: Sun Apr 23 08:11:56 2023, max compression
+gzip compressed data, was "scribber-0.1.16.tar", last modified: Sun Apr 23 10:27:17 2023, max compression
```

## Comparing `scribber-0.1.12.tar` & `scribber-0.1.16.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/
--rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.12/LICENSE
--rw-rw-r--   0 sem       (1000) sem       (1000)     3135 2023-04-23 08:11:56.643283 scribber-0.1.12/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)     2516 2023-04-23 08:04:32.000000 scribber-0.1.12/README.md
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.639284 scribber-0.1.12/scribber/
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/core/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.12/scribber/core/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2586 2022-12-04 12:33:46.000000 scribber-0.1.12/scribber/core/document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/examples/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.12/scribber/examples/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)      133 2022-12-04 12:13:22.000000 scribber-0.1.12/scribber/examples/t.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2463 2023-04-23 07:30:20.000000 scribber-0.1.12/scribber/examples/usage.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.12/scribber/formats/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/excel/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.12/scribber/formats/excel/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2909 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/excel/excel_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/markdown/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.12/scribber/formats/markdown/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     4615 2023-04-23 07:40:41.000000 scribber-0.1.12/scribber/formats/markdown/markdown_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/text/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.12/scribber/formats/text/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3618 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/text/text_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/word/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.12/scribber/formats/word/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2550 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/word/word_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/scribber.egg-info/
--rw-rw-r--   0 sem       (1000) sem       (1000)     3135 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)      698 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/SOURCES.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/dependency_links.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)      127 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/requires.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       22 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/top_level.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-23 08:11:56.643283 scribber-0.1.12/setup.cfg
--rw-rw-r--   0 sem       (1000) sem       (1000)     1128 2023-04-23 07:58:01.000000 scribber-0.1.12/setup.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.16/LICENSE
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2984 2023-04-23 10:27:17.697623 scribber-0.1.16/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2364 2023-04-23 10:27:08.000000 scribber-0.1.16/README.md
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/
+-rw-rw-r--   0 sem       (1000) sem       (1000)      387 2023-04-23 10:15:35.000000 scribber-0.1.16/scribber/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/core/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.16/scribber/core/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2586 2022-12-04 12:33:46.000000 scribber-0.1.16/scribber/core/document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/examples/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.16/scribber/examples/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2267 2023-04-23 10:27:08.000000 scribber-0.1.16/scribber/examples/usage.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/formats/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.16/scribber/formats/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/formats/excel/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.16/scribber/formats/excel/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2909 2023-04-23 07:27:53.000000 scribber-0.1.16/scribber/formats/excel/excel_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/formats/markdown/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.16/scribber/formats/markdown/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     4615 2023-04-23 07:40:41.000000 scribber-0.1.16/scribber/formats/markdown/markdown_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/formats/text/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.16/scribber/formats/text/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3618 2023-04-23 07:27:53.000000 scribber-0.1.16/scribber/formats/text/text_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber/formats/word/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.16/scribber/formats/word/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2550 2023-04-23 07:27:53.000000 scribber-0.1.16/scribber/formats/word/word_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 10:27:17.697623 scribber-0.1.16/scribber.egg-info/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2984 2023-04-23 10:27:17.000000 scribber-0.1.16/scribber.egg-info/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)      651 2023-04-23 10:27:17.000000 scribber-0.1.16/scribber.egg-info/SOURCES.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-23 10:27:17.000000 scribber-0.1.16/scribber.egg-info/dependency_links.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)      147 2023-04-23 10:27:17.000000 scribber-0.1.16/scribber.egg-info/requires.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        9 2023-04-23 10:27:17.000000 scribber-0.1.16/scribber.egg-info/top_level.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-23 10:27:17.697623 scribber-0.1.16/setup.cfg
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1166 2023-04-23 10:27:08.000000 scribber-0.1.16/setup.py
```

### Comparing `scribber-0.1.12/LICENSE` & `scribber-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/PKG-INFO` & `scribber-0.1.16/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.1.12
+Version: 0.1.16
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Scribber
 
 ---
 
 A simple document generator with not very rich functionality that can export a document to some formats such 
@@ -26,19 +26,27 @@
 ```shell
 pip install scribber
 ```
 
 ## Usage
 
 ```python
-from scribber.core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
-from scribber.formats.excel.excel_document import ExcelDocumentBuilder
-from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
-from scribber.formats.text.text_document import TextDocumentBuilder
-from scribber.formats.word.word_document import WordDocumentBuilder
+from scribber import (
+    SimpleDocument,
+    Title,
+    EmptyLine,
+    Paragraph,
+    Table,
+    Director,
+    CodeBlock,
+    ExcelDocumentBuilder,
+    MarkdownDocumentBuilder,
+    TextDocumentBuilder,
+    WordDocumentBuilder,
+)
 
 doc = SimpleDocument()
 doc.add(Title(title="Funny report"))
 doc.add(EmptyLine())
 doc.add(Paragraph(text="Let me show you report"))
 doc.add(
     Table(
@@ -107,8 +115,7 @@
 ## requirements
 
 - lxml>=4.9.1<5.0.0
 - pydantic>=1.10.2<2.0.0
 - python-docx>=0.8.11<1.0.0
 - typing_extensions>=4.4.0<5.0.0
 - XlsxWriter>=3.0.3<4.0.0
-
```

### Comparing `scribber-0.1.12/README.md` & `scribber-0.1.16/scribber.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: scribber
+Version: 0.1.16
+Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
+Home-page: https://github.com/edelwi/scribber
+Author: Evgeniy Semenov
+Author-email: edelwi@yandex.ru
+License: MIT
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Scribber
 
 ---
 
 A simple document generator with not very rich functionality that can export a document to some formats such 
 as text, docx, xlsx and markdown.
 
@@ -9,19 +26,27 @@
 ```shell
 pip install scribber
 ```
 
 ## Usage
 
 ```python
-from scribber.core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
-from scribber.formats.excel.excel_document import ExcelDocumentBuilder
-from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
-from scribber.formats.text.text_document import TextDocumentBuilder
-from scribber.formats.word.word_document import WordDocumentBuilder
+from scribber import (
+    SimpleDocument,
+    Title,
+    EmptyLine,
+    Paragraph,
+    Table,
+    Director,
+    CodeBlock,
+    ExcelDocumentBuilder,
+    MarkdownDocumentBuilder,
+    TextDocumentBuilder,
+    WordDocumentBuilder,
+)
 
 doc = SimpleDocument()
 doc.add(Title(title="Funny report"))
 doc.add(EmptyLine())
 doc.add(Paragraph(text="Let me show you report"))
 doc.add(
     Table(
@@ -89,8 +114,8 @@
 
 ## requirements
 
 - lxml>=4.9.1<5.0.0
 - pydantic>=1.10.2<2.0.0
 - python-docx>=0.8.11<1.0.0
 - typing_extensions>=4.4.0<5.0.0
-- XlsxWriter>=3.0.3<4.0.0
+- XlsxWriter>=3.0.3<4.0.0
```

### Comparing `scribber-0.1.12/scribber/core/document.py` & `scribber-0.1.16/scribber/core/document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/scribber/examples/usage.py` & `scribber-0.1.16/scribber/examples/usage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from scribber.core.document import (
+from scribber import (
     SimpleDocument,
     Title,
     EmptyLine,
     Paragraph,
     Table,
     Director,
     CodeBlock,
+    ExcelDocumentBuilder,
+    MarkdownDocumentBuilder,
+    TextDocumentBuilder,
+    WordDocumentBuilder,
 )
-from scribber.formats.excel.excel_document import ExcelDocumentBuilder
-from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
-from scribber.formats.text.text_document import TextDocumentBuilder
-from scribber.formats.word.word_document import WordDocumentBuilder
 
 CODE_EXAMPLE = """
 import platform
 
 def main():
     print("Hello World!")
     print(f"OS: {platform.system()}")
```

### Comparing `scribber-0.1.12/scribber/formats/excel/excel_document.py` & `scribber-0.1.16/scribber/formats/excel/excel_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/scribber/formats/markdown/markdown_document.py` & `scribber-0.1.16/scribber/formats/markdown/markdown_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/scribber/formats/text/text_document.py` & `scribber-0.1.16/scribber/formats/text/text_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/scribber/formats/word/word_document.py` & `scribber-0.1.16/scribber/formats/word/word_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.12/scribber/scribber.egg-info/SOURCES.txt` & `scribber-0.1.16/scribber.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 README.md
 setup.py
+scribber/__init__.py
+scribber.egg-info/PKG-INFO
+scribber.egg-info/SOURCES.txt
+scribber.egg-info/dependency_links.txt
+scribber.egg-info/requires.txt
+scribber.egg-info/top_level.txt
 scribber/core/__init__.py
 scribber/core/document.py
 scribber/examples/__init__.py
-scribber/examples/t.py
 scribber/examples/usage.py
 scribber/formats/__init__.py
 scribber/formats/excel/__init__.py
 scribber/formats/excel/excel_document.py
 scribber/formats/markdown/__init__.py
 scribber/formats/markdown/markdown_document.py
 scribber/formats/text/__init__.py
 scribber/formats/text/text_document.py
 scribber/formats/word/__init__.py
-scribber/formats/word/word_document.py
-scribber/scribber.egg-info/PKG-INFO
-scribber/scribber.egg-info/SOURCES.txt
-scribber/scribber.egg-info/dependency_links.txt
-scribber/scribber.egg-info/requires.txt
-scribber/scribber.egg-info/top_level.txt
+scribber/formats/word/word_document.py
```

### Comparing `scribber-0.1.12/setup.py` & `scribber-0.1.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scribber",
-    version="v0.1.12",
+    version="v0.1.16",
     author="Evgeniy Semenov",
     author_email="edelwi@yandex.ru",
     license="MIT",
     description="A simple document generator with not very rich functionality that can export a document to "
                 "some formats such as text, docx, xlsx and markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edelwi/scribber",
-    package_dir={"": "scribber"},
-    packages=setuptools.find_packages(where="scribber"),
+    packages=setuptools.find_packages(exclude=["examples.test.*"]),
     # entry_points={},
     install_requires=[
         'lxml>=4.9.0,<5.0.0',
         'pydantic>=1.10.2,<2.0.0',
         'python-docx>=0.8.11,<1.0.0',
         'typing_extensions>=4.4.0,<5.0.0',
         'XlsxWriter>=3.0.3,<4.0.0',
         ],
+    extras_require={
+        "dev": ["twine>=4.0.2"],
+    },
     python_requires=">=3.10",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

