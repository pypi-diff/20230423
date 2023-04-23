# Comparing `tmp/txt2ebook-0.1.8.tar.gz` & `tmp/txt2ebook-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2ebook-0.1.8.tar", max compression
+gzip compressed data, was "txt2ebook-0.1.9.tar", max compression
```

## Comparing `txt2ebook-0.1.8.tar` & `txt2ebook-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     3653 2021-10-04 15:51:33.030173 txt2ebook-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0    34523 2017-09-30 07:16:25.000000 txt2ebook-0.1.8/LICENSE
--rw-r--r--   0        0        0     1966 2021-10-04 15:50:22.810196 txt2ebook-0.1.8/README.md
--rw-r--r--   0        0        0      892 2021-10-04 15:50:56.466184 txt2ebook-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      183 2021-10-04 15:51:12.458179 txt2ebook-0.1.8/src/txt2ebook/__init__.py
--rw-r--r--   0        0        0    13075 2021-10-04 13:59:13.902585 txt2ebook-0.1.8/src/txt2ebook/txt2ebook.py
--rw-r--r--   0        0        0     3007 2021-10-04 15:54:22.260786 txt2ebook-0.1.8/setup.py
--rw-r--r--   0        0        0     2888 2021-10-04 15:54:22.261782 txt2ebook-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3975 2021-10-25 03:05:07.450302 txt2ebook-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0    34523 2017-09-30 07:16:25.000000 txt2ebook-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1966 2021-10-10 20:03:32.898089 txt2ebook-0.1.9/README.md
+-rw-r--r--   0        0        0      892 2021-10-25 03:05:30.630188 txt2ebook-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       63 2021-10-25 03:05:20.746231 txt2ebook-0.1.9/src/txt2ebook/__init__.py
+-rw-r--r--   0        0        0      139 2021-10-23 20:56:45.562634 txt2ebook-0.1.9/src/txt2ebook/formats/__init__.py
+-rw-r--r--   0        0        0     3203 2021-10-23 00:49:42.526790 txt2ebook-0.1.9/src/txt2ebook/formats/epub.py
+-rw-r--r--   0        0        0     1241 2021-10-20 23:58:44.003948 txt2ebook-0.1.9/src/txt2ebook/formats/txt.py
+-rw-r--r--   0        0        0     1404 2021-10-23 01:45:09.670659 txt2ebook-0.1.9/src/txt2ebook/formats/writer.py
+-rw-r--r--   0        0        0      146 2021-10-24 02:34:59.033809 txt2ebook-0.1.9/src/txt2ebook/parsers/__init__.py
+-rw-r--r--   0        0        0      528 2021-10-21 00:01:45.671993 txt2ebook-0.1.9/src/txt2ebook/parsers/en.py
+-rw-r--r--   0        0        0     3021 2021-10-23 01:45:09.746649 txt2ebook-0.1.9/src/txt2ebook/parsers/parser.py
+-rw-r--r--   0        0        0     7031 2021-10-23 01:45:09.846637 txt2ebook-0.1.9/src/txt2ebook/parsers/zhcn.py
+-rw-r--r--   0        0        0      139 2021-10-23 01:30:50.522859 txt2ebook-0.1.9/src/txt2ebook/parsers/zhtw.py
+-rw-r--r--   0        0        0     3308 2021-10-23 01:45:09.746649 txt2ebook-0.1.9/src/txt2ebook/txt2ebook.py
+-rw-r--r--   0        0        0     3049 2021-10-26 22:53:29.481711 txt2ebook-0.1.9/setup.py
+-rw-r--r--   0        0        0     2888 2021-10-26 22:53:29.482405 txt2ebook-0.1.9/PKG-INFO
```

### Comparing `txt2ebook-0.1.8/CHANGELOG.md` & `txt2ebook-0.1.9/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## v0.1.9 - 2021-10-26
+Added
+- Add `--format` option to specify output format
+
+Fixed
+- Fix missing deps in requirements.txt
+- Fix issues raised by PyLint
+
+Changed
+- Refactor txt and epub file generation in separate module
+- Refactor txt formatting and parsing in separate module
+- Switch chapter header regex to constant
+
 ## v0.1.8 - 2021-10-04
 Added
 - Allow setting of optional argument for output path and file name
 - Add `--width` option to set line width for paragraph wrapping
 
 Changed
 - Rename `--remove-wrapping` option to `-no-wrapping` to follow the convention
```

### Comparing `txt2ebook-0.1.8/LICENSE` & `txt2ebook-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2ebook-0.1.8/README.md` & `txt2ebook-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `txt2ebook-0.1.8/pyproject.toml` & `txt2ebook-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "txt2ebook"
-version = "0.1.8"
+version = "0.1.9"
 description = "Console tool to convert txt file to different ebook format"
 authors = ["Kian-Meng Ang <kianmeng@cpan.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/kianmeng/txt2ebook"
 repository = "https://github.com/kianmeng/txt2ebook"
 keywords = ["txt", "ebook", "epub"]
```

### Comparing `txt2ebook-0.1.8/setup.py` & `txt2ebook-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['txt2ebook']
+['txt2ebook', 'txt2ebook.formats', 'txt2ebook.parsers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['CJKwrap>=2.2,<3.0',
  'EbookLib>=0.17.1,<0.18.0',
@@ -19,15 +19,15 @@
  'langdetect>=1.0.9,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['txt2ebook = txt2ebook.txt2ebook:main']}
 
 setup_kwargs = {
     'name': 'txt2ebook',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Console tool to convert txt file to different ebook format',
     'long_description': '# txt2ebook\n\nConsole tool to convert txt file to different ebook format.\n\n## Installation\n\nFrom PyPI:\n\n```\npip install txt2ebook\n```\n\n## Usage\n\nShowing help message:\n\n```bash\n$ txt2ebook --help\nUsage: txt2ebook [OPTIONS] INPUT_FILE [OUTPUT_FILE]\n\n  Console tool to convert txt file to different ebook format.\n\nOptions:\n  -t, --title TEXT                Set the title of the ebook.\n  -l, --language TEXT             Set the language of the ebook.\n  -a, --author TEXT               Set the author of the ebook.\n  -c, --cover PATH                Set the cover of the ebook.\n  -d, --debug                     Enable debugging log.\n  -nb, --no-backup                Do not backup source txt file.  [default:\n                                  False]\n  -nw, --no-wrapping              Remove word wrapping.  [default: False]\n  -w, --width INTEGER             Set the width for line wrapping.\n  -dr, --delete-regex TEXT        Regex to delete word or phrase.\n  -rr, --replace-regex TEXT...    Regex to replace word or phrase.\n  -dlr, --delete-line-regex TEXT  Regex to delete whole line.\n  --version                       Show the version and exit.\n  --help                          Show this message and exit.\n```\n\nConvert a txt file into epub:\n\n```bash\ntxt2book ebook.txt\n```\n\n## Copyright and License\n\nCopyright (c) 2021 Kian-Meng, Ang\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU Affero General Public License as\npublished by the Free Software Foundation, either version 3 of the\nLicense, or (at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU Affero General Public License for more details.\n\nYou should have received a copy of the GNU Affero General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n',
     'author': 'Kian-Meng Ang',
     'author_email': 'kianmeng@cpan.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kianmeng/txt2ebook',
```

### Comparing `txt2ebook-0.1.8/PKG-INFO` & `txt2ebook-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2ebook
-Version: 0.1.8
+Version: 0.1.9
 Summary: Console tool to convert txt file to different ebook format
 Home-page: https://github.com/kianmeng/txt2ebook
 License: AGPL-3.0-or-later
 Keywords: txt,ebook,epub
 Author: Kian-Meng Ang
 Author-email: kianmeng@cpan.org
 Requires-Python: >=3.9,<4.0
```

