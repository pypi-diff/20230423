# Comparing `tmp/scribber-0.0.9.tar.gz` & `tmp/scribber-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribber-0.0.9.tar", last modified: Sun Nov 20 14:52:19 2022, max compression
+gzip compressed data, was "scribber-0.1.12.tar", last modified: Sun Apr 23 08:11:56 2023, max compression
```

## Comparing `scribber-0.0.9.tar` & `scribber-0.1.12.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/
--rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2022-11-20 06:58:25.000000 scribber-0.0.9/LICENSE
--rw-rw-r--   0 sem       (1000) sem       (1000)     3039 2022-11-20 14:52:19.068946 scribber-0.0.9/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)     2441 2022-11-20 13:00:30.000000 scribber-0.0.9/README.md
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/core/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.0.9/core/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2205 2022-11-20 07:34:33.000000 scribber-0.0.9/core/document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/formats/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.0.9/formats/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/formats/excel/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.0.9/formats/excel/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2503 2022-11-20 08:09:21.000000 scribber-0.0.9/formats/excel/excel_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/formats/markdown/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.0.9/formats/markdown/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3756 2022-11-20 10:20:40.000000 scribber-0.0.9/formats/markdown/markdown_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/formats/text/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.0.9/formats/text/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3288 2022-11-20 07:45:32.000000 scribber-0.0.9/formats/text/text_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/formats/word/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.0.9/formats/word/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2209 2022-11-20 08:09:21.000000 scribber-0.0.9/formats/word/word_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2022-11-20 14:52:19.068946 scribber-0.0.9/scribber.egg-info/
--rw-rw-r--   0 sem       (1000) sem       (1000)     3039 2022-11-20 14:52:19.000000 scribber-0.0.9/scribber.egg-info/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)      474 2022-11-20 14:52:19.000000 scribber-0.0.9/scribber.egg-info/SOURCES.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        1 2022-11-20 14:52:19.000000 scribber-0.0.9/scribber.egg-info/dependency_links.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)      127 2022-11-20 14:52:19.000000 scribber-0.0.9/scribber.egg-info/requires.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       13 2022-11-20 14:52:19.000000 scribber-0.0.9/scribber.egg-info/top_level.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       38 2022-11-20 14:52:19.068946 scribber-0.0.9/setup.cfg
--rw-rw-r--   0 sem       (1000) sem       (1000)     1028 2022-11-20 14:51:51.000000 scribber-0.0.9/setup.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.12/LICENSE
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3135 2023-04-23 08:11:56.643283 scribber-0.1.12/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2516 2023-04-23 08:04:32.000000 scribber-0.1.12/README.md
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.639284 scribber-0.1.12/scribber/
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/core/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.12/scribber/core/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2586 2022-12-04 12:33:46.000000 scribber-0.1.12/scribber/core/document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/examples/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.12/scribber/examples/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)      133 2022-12-04 12:13:22.000000 scribber-0.1.12/scribber/examples/t.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2463 2023-04-23 07:30:20.000000 scribber-0.1.12/scribber/examples/usage.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.12/scribber/formats/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/excel/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.12/scribber/formats/excel/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2909 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/excel/excel_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/markdown/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.12/scribber/formats/markdown/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     4615 2023-04-23 07:40:41.000000 scribber-0.1.12/scribber/formats/markdown/markdown_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/text/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.12/scribber/formats/text/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3618 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/text/text_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/formats/word/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.12/scribber/formats/word/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2550 2023-04-23 07:27:53.000000 scribber-0.1.12/scribber/formats/word/word_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-23 08:11:56.643283 scribber-0.1.12/scribber/scribber.egg-info/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3135 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)      698 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/SOURCES.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/dependency_links.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)      127 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/requires.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)       22 2023-04-23 08:11:56.000000 scribber-0.1.12/scribber/scribber.egg-info/top_level.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-23 08:11:56.643283 scribber-0.1.12/setup.cfg
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1128 2023-04-23 07:58:01.000000 scribber-0.1.12/setup.py
```

### Comparing `scribber-0.0.9/LICENSE` & `scribber-0.1.12/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Evgeniy Semenov
+Copyright (c) 2023 Evgeniy Semenov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `scribber-0.0.9/PKG-INFO` & `scribber-0.1.12/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.0.9
+Version: 0.1.12
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scribber
 
 ---
 
@@ -25,19 +26,19 @@
 ```shell
 pip install scribber
 ```
 
 ## Usage
 
 ```python
-from core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
-from formats.excel.excel_document import ExcelDocumentBuilder
-from formats.markdown.markdown_document import MarkdownDocumentBuilder
-from formats.text.text_document import TextDocumentBuilder
-from formats.word.word_document import WordDocumentBuilder
+from scribber.core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
+from scribber.formats.excel.excel_document import ExcelDocumentBuilder
+from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
+from scribber.formats.text.text_document import TextDocumentBuilder
+from scribber.formats.word.word_document import WordDocumentBuilder
 
 doc = SimpleDocument()
 doc.add(Title(title="Funny report"))
 doc.add(EmptyLine())
 doc.add(Paragraph(text="Let me show you report"))
 doc.add(
     Table(
@@ -101,13 +102,13 @@
 Total
 =====
 It's Ok!
 ```
 
 ## requirements
 
-- lxml==4.9.1
-- pydantic==1.10.2
-- python-docx==0.8.11
-- typing_extensions==4.4.0
-- XlsxWriter==3.0.3
+- lxml>=4.9.1<5.0.0
+- pydantic>=1.10.2<2.0.0
+- python-docx>=0.8.11<1.0.0
+- typing_extensions>=4.4.0<5.0.0
+- XlsxWriter>=3.0.3<4.0.0
```

### Comparing `scribber-0.0.9/README.md` & `scribber-0.1.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 ```shell
 pip install scribber
 ```
 
 ## Usage
 
 ```python
-from core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
-from formats.excel.excel_document import ExcelDocumentBuilder
-from formats.markdown.markdown_document import MarkdownDocumentBuilder
-from formats.text.text_document import TextDocumentBuilder
-from formats.word.word_document import WordDocumentBuilder
+from scribber.core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
+from scribber.formats.excel.excel_document import ExcelDocumentBuilder
+from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
+from scribber.formats.text.text_document import TextDocumentBuilder
+from scribber.formats.word.word_document import WordDocumentBuilder
 
 doc = SimpleDocument()
 doc.add(Title(title="Funny report"))
 doc.add(EmptyLine())
 doc.add(Paragraph(text="Let me show you report"))
 doc.add(
     Table(
@@ -85,12 +85,12 @@
 Total
 =====
 It's Ok!
 ```
 
 ## requirements
 
-- lxml==4.9.1
-- pydantic==1.10.2
-- python-docx==0.8.11
-- typing_extensions==4.4.0
-- XlsxWriter==3.0.3
+- lxml>=4.9.1<5.0.0
+- pydantic>=1.10.2<2.0.0
+- python-docx>=0.8.11<1.0.0
+- typing_extensions>=4.4.0<5.0.0
+- XlsxWriter>=3.0.3<4.0.0
```

### Comparing `scribber-0.0.9/core/document.py` & `scribber-0.1.12/scribber/core/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,24 @@
 
     @validator("text")
     def field_not_empty(cls, v):
         assert len(v) > 0, "must be one or more symbols"
         return v
 
 
+class CodeBlock(BaseModel):
+    code: str
+    style: str
+
+    @validator("code")
+    def field_not_empty(cls, v):
+        assert len(v) > 0, "must be one or more symbols"
+        return v
+
+
 class Table(BaseModel):
     headers: List[str]
     content: List[Any]
 
     @validator("headers", "content")
     def not_empty(cls, v):
         assert len(v) > 0, "must not be empty"
@@ -67,14 +77,18 @@
         pass
 
     @abstractmethod
     def add_paragraph(self, paragraph: Paragraph) -> None:
         pass
 
     @abstractmethod
+    def add_code_block(self, code_block: CodeBlock) -> None:
+        pass
+
+    @abstractmethod
     def add_brake(self):
         pass
 
 
 class Director:
     def __init__(self) -> None:
         self._builder = None
@@ -93,7 +107,9 @@
                 self.builder.add_title(item)
             elif isinstance(item, Paragraph):
                 self.builder.add_paragraph(item)
             elif isinstance(item, EmptyLine):
                 self.builder.add_brake()
             elif isinstance(item, Table):
                 self.builder.add_table(item)
+            elif isinstance(item, CodeBlock):
+                self.builder.add_code_block(item)
```

### Comparing `scribber-0.0.9/formats/excel/excel_document.py` & `scribber-0.1.12/scribber/formats/excel/excel_document.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from pydantic import FilePath
 
-from core.document import Title, Paragraph, EmptyLine, Table, Builder
+from scribber.core.document import Title, Paragraph, EmptyLine, Table, Builder, CodeBlock
 
 import xlsxwriter
 
 
 class ExcelDocument:
     def __init__(self) -> None:
         self._row = 0
@@ -29,24 +29,31 @@
                 self._render_title(item)
             elif isinstance(item, Paragraph):
                 self._render_paragraph(item)
             elif isinstance(item, EmptyLine):
                 self._render_brake()
             elif isinstance(item, Table):
                 self._render_table(item)
+            elif isinstance(item, CodeBlock):
+                self._render_code_block(item)
         return self._workbook
 
     def save(self, filename: FilePath):
         self._workbook.filename = filename
         self.get_result().close()
 
     def _render_paragraph(self, paragraph: Paragraph):
         self._report.write(self._row, self._col, paragraph.text)
         self._row += 1
 
+    def _render_code_block(self, code_block: CodeBlock):
+        for line in code_block.code.split(sep="\n"):
+            self._report.write(self._row, self._col, line)
+            self._row += 1
+
     def _render_brake(self):
         self._row += 1
 
     def _render_table(self, item):
         for header in item.headers:
             self._report.write(self._row, self._col, header, self._bold_format)
             self._col += 1
@@ -81,7 +88,10 @@
         self._excel_report.add(table)
 
     def add_paragraph(self, paragraph: Paragraph) -> None:
         self._excel_report.add(paragraph)
 
     def add_brake(self):
         self._excel_report.add(EmptyLine())
+
+    def add_code_block(self, code_block: CodeBlock):
+        self._excel_report.add(code_block)
```

### Comparing `scribber-0.0.9/formats/markdown/markdown_document.py` & `scribber-0.1.12/scribber/formats/text/text_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from typing import Any
 
 from pydantic import FilePath
 
-from core.document import Title, Paragraph, EmptyLine, Table, Builder
+from scribber.core.document import Title, Paragraph, EmptyLine, Table, Builder, CodeBlock
 
 
-class MarkdownDocument:
+class TextDocument:
     def __init__(self) -> None:
         self.parts = []
         self._report = ""
         self._line_brake = "\n"
         self._line_divider = "-"
         self._col_divider = "|"
-        self._title_starter = "#"
-        self._col_starter = self._col_divider + " "
-        self._col_stopper = " " + self._col_divider
-        self._col_justify = " :---: "
 
     def add(self, part: Any) -> None:
         self.parts.append(part)
 
     def _render_title(self, title: Title) -> None:
         str_len = len(title.title)
-        self._report += (self._title_starter * title.level) + " " + title.title + self._line_brake
+        self._report += title.title + self._line_brake
+        self._report += "=" * str_len + self._line_brake
 
     def get_result(self) -> str:
         for item in self.parts:
             if isinstance(item, Title):
                 self._render_title(item)
             elif isinstance(item, Paragraph):
                 self._render_paragraph(item)
             elif isinstance(item, EmptyLine):
                 self._render_brake()
             elif isinstance(item, Table):
                 self._render_table(item)
+            elif isinstance(item, CodeBlock):
+                self._render_code_block(item)
         return self._report
 
     def save(self, filename: FilePath):
         with open(filename, "w") as f:
             f.write(self.get_result())
 
     def _render_paragraph(self, paragraph: Paragraph):
-        self._report += paragraph.text + (self._line_brake * 2)
+        self._report += paragraph.text + self._line_brake
+
+    def _render_code_block(self, code_block: CodeBlock):
+        self._report += code_block.code + self._line_brake
 
     def _render_brake(self):
         self._report += self._line_brake
 
     def _render_table(self, item):
         col_length = []
         col_count = len(item.headers)
@@ -57,45 +59,42 @@
             column_content_length = max([len(str(_[col])) for _ in item.content])
             if col_length[col] < column_content_length + 2:
                 col_length[col] = column_content_length + 2
             col += 1
         table_line_separator = (
             self._line_divider * (sum(col_length) + sep_count) + self._line_brake
         )
-        # self._report += table_line_separator
+        self._report += table_line_separator
         headers_justified = []
-        headers_bottom = []
         i = 0
         for itm in item.headers:
             headers_justified.append(f"{itm : ^{col_length[i]}}")
-            headers_bottom.append(self._col_justify)
             i += 1
-        self._report += self._col_starter + self._col_divider.join(headers_justified) + self._col_stopper + self._line_brake
-        # self._report += table_line_separator
-        self._report += self._col_starter + self._col_divider.join(headers_bottom) + self._col_stopper + self._line_brake
+        self._report += self._col_divider.join(headers_justified) + self._line_brake
+        self._report += table_line_separator
 
         for line in item.content:
             i = 0
             content_justified = []
             for itm in item.headers:
-                content_justified.append(f"{line[i] : ^{col_length[i]}}")
+                content_justified.append(f"{str(line[i]) : ^{col_length[i]}}")
                 i += 1
-            self._report += self._col_starter + self._col_divider.join(content_justified) + self._col_starter + self._line_brake
-        self._report += self._line_brake
+            self._report += self._col_divider.join(content_justified) + self._line_brake
+        self._report += table_line_separator
 
 
-class MarkdownDocumentBuilder(Builder):
+class TextDocumentBuilder(Builder):
     def __init__(self) -> None:
         self.reset()
 
     def reset(self) -> None:
-        self._text_report = MarkdownDocument()
+        self._text_report = TextDocument()
 
     @property
-    def parts(self) -> MarkdownDocument:
+    def parts(self) -> TextDocument:
         parts = self._text_report
         self.reset()
         return parts
 
     def add_title(self, title: Title) -> None:
         self._text_report.add(title)
 
@@ -103,7 +102,10 @@
         self._text_report.add(table)
 
     def add_paragraph(self, paragraph: Paragraph) -> None:
         self._text_report.add(paragraph)
 
     def add_brake(self):
         self._text_report.add(EmptyLine())
+
+    def add_code_block(self, code_block: CodeBlock):
+        self._text_report.add(code_block)
```

### Comparing `scribber-0.0.9/formats/text/text_document.py` & `scribber-0.1.12/scribber/formats/word/word_document.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,84 @@
 from typing import Any
 
 from pydantic import FilePath
 
-from core.document import Title, Paragraph, EmptyLine, Table, Builder
+from scribber.core.document import Title, Paragraph, EmptyLine, Table, Builder, CodeBlock
+from docx import Document
 
 
-class TextDocument:
+class WordDocument:
     def __init__(self) -> None:
         self.parts = []
-        self._report = ""
-        self._line_brake = "\n"
-        self._line_divider = "-"
-        self._col_divider = "|"
+        self._report = Document()
 
     def add(self, part: Any) -> None:
         self.parts.append(part)
 
     def _render_title(self, title: Title) -> None:
-        str_len = len(title.title)
-        self._report += title.title + self._line_brake
-        self._report += "=" * str_len + self._line_brake
+        # str_len = len(title.title)
+        self._report.add_heading(title.title, title.level - 1)
 
-    def get_result(self) -> str:
+    def get_result(self) -> Document:
         for item in self.parts:
             if isinstance(item, Title):
                 self._render_title(item)
             elif isinstance(item, Paragraph):
                 self._render_paragraph(item)
             elif isinstance(item, EmptyLine):
                 self._render_brake()
             elif isinstance(item, Table):
                 self._render_table(item)
+            elif isinstance(item, CodeBlock):
+                self._render_code_block(item)
         return self._report
 
     def save(self, filename: FilePath):
-        with open(filename, "w") as f:
-            f.write(self.get_result())
+        self.get_result().save(filename)
 
     def _render_paragraph(self, paragraph: Paragraph):
-        self._report += paragraph.text + self._line_brake
+        self._report.add_paragraph(paragraph.text)
+
+    def _render_code_block(self, code_block: CodeBlock):
+        self._report.add_paragraph(code_block.code, style='Intense Quote')
 
     def _render_brake(self):
-        self._report += self._line_brake
+        self._report.add_paragraph("")
 
     def _render_table(self, item):
-        col_length = []
-        col_count = len(item.headers)
-        sep_count = col_count - 1 if col_count > 1 else 1
-        for itm in item.headers:
-            col_length.append(len(itm) + 2)
-        col = 0
-        for itm in item.headers:
-            column_content_length = max([len(str(_[col])) for _ in item.content])
-            if col_length[col] < column_content_length + 2:
-                col_length[col] = column_content_length + 2
-            col += 1
-        table_line_separator = (
-            self._line_divider * (sum(col_length) + sep_count) + self._line_brake
-        )
-        self._report += table_line_separator
-        headers_justified = []
-        i = 0
-        for itm in item.headers:
-            headers_justified.append(f"{itm : ^{col_length[i]}}")
-            i += 1
-        self._report += self._col_divider.join(headers_justified) + self._line_brake
-        self._report += table_line_separator
-
-        for line in item.content:
-            i = 0
-            content_justified = []
-            for itm in item.headers:
-                content_justified.append(f"{line[i] : ^{col_length[i]}}")
-                i += 1
-            self._report += self._col_divider.join(content_justified) + self._line_brake
-        self._report += table_line_separator
+        table = self._report.add_table(rows=1, cols=len(item.headers))
+        hdr_cells = table.rows[0].cells
+        for i, hdr in enumerate(item.headers):
+            hdr_cells[i].text = hdr
+        for row in item.content:
+            row_cells = table.add_row().cells
+            for j, itm in enumerate(row):
+                row_cells[j].text = str(itm)
 
 
-class TextDocumentBuilder(Builder):
+class WordDocumentBuilder(Builder):
     def __init__(self) -> None:
         self.reset()
 
     def reset(self) -> None:
-        self._text_report = TextDocument()
+        self._word_report = WordDocument()
 
     @property
-    def parts(self) -> TextDocument:
-        parts = self._text_report
+    def parts(self) -> WordDocument:
+        parts = self._word_report
         self.reset()
         return parts
 
     def add_title(self, title: Title) -> None:
-        self._text_report.add(title)
+        self._word_report.add(title)
 
     def add_table(self, table: Table) -> None:
-        self._text_report.add(table)
+        self._word_report.add(table)
 
     def add_paragraph(self, paragraph: Paragraph) -> None:
-        self._text_report.add(paragraph)
+        self._word_report.add(paragraph)
 
     def add_brake(self):
-        self._text_report.add(EmptyLine())
+        self._word_report.add(EmptyLine())
+
+    def add_code_block(self, code_block: CodeBlock):
+        self._word_report.add(code_block)
```

### Comparing `scribber-0.0.9/scribber.egg-info/PKG-INFO` & `scribber-0.1.12/scribber/scribber.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.0.9
+Version: 0.1.12
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scribber
 
 ---
 
@@ -25,19 +26,19 @@
 ```shell
 pip install scribber
 ```
 
 ## Usage
 
 ```python
-from core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
-from formats.excel.excel_document import ExcelDocumentBuilder
-from formats.markdown.markdown_document import MarkdownDocumentBuilder
-from formats.text.text_document import TextDocumentBuilder
-from formats.word.word_document import WordDocumentBuilder
+from scribber.core.document import SimpleDocument, Title, EmptyLine, Paragraph, Table, Director
+from scribber.formats.excel.excel_document import ExcelDocumentBuilder
+from scribber.formats.markdown.markdown_document import MarkdownDocumentBuilder
+from scribber.formats.text.text_document import TextDocumentBuilder
+from scribber.formats.word.word_document import WordDocumentBuilder
 
 doc = SimpleDocument()
 doc.add(Title(title="Funny report"))
 doc.add(EmptyLine())
 doc.add(Paragraph(text="Let me show you report"))
 doc.add(
     Table(
@@ -101,13 +102,13 @@
 Total
 =====
 It's Ok!
 ```
 
 ## requirements
 
-- lxml==4.9.1
-- pydantic==1.10.2
-- python-docx==0.8.11
-- typing_extensions==4.4.0
-- XlsxWriter==3.0.3
+- lxml>=4.9.1<5.0.0
+- pydantic>=1.10.2<2.0.0
+- python-docx>=0.8.11<1.0.0
+- typing_extensions>=4.4.0<5.0.0
+- XlsxWriter>=3.0.3<4.0.0
```

### Comparing `scribber-0.0.9/setup.py` & `scribber-0.1.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scribber",
-    version="v0.0.9",
+    version="v0.1.12",
     author="Evgeniy Semenov",
     author_email="edelwi@yandex.ru",
+    license="MIT",
     description="A simple document generator with not very rich functionality that can export a document to "
                 "some formats such as text, docx, xlsx and markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edelwi/scribber",
-    packages=setuptools.find_packages(),
+    package_dir={"": "scribber"},
+    packages=setuptools.find_packages(where="scribber"),
     # entry_points={},
     install_requires=[
         'lxml>=4.9.0,<5.0.0',
         'pydantic>=1.10.2,<2.0.0',
         'python-docx>=0.8.11,<1.0.0',
         'typing_extensions>=4.4.0,<5.0.0',
         'XlsxWriter>=3.0.3,<4.0.0',
         ],
+    python_requires=">=3.10",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

