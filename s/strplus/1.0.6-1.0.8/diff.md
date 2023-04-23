# Comparing `tmp/strplus-1.0.6.tar.gz` & `tmp/strplus-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.6.tar", max compression
+gzip compressed data, was "strplus-1.0.8.tar", max compression
```

## Comparing `strplus-1.0.6.tar` & `strplus-1.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.6/LICENSE
--rw-r--r--   0        0        0     2846 2023-04-22 09:01:02.179149 strplus-1.0.6/README.md
--rw-r--r--   0        0        0     1027 2023-04-22 09:01:02.179149 strplus-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/__init__.py
--rw-r--r--   0        0        0     5957 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/cases.py
--rw-r--r--   0        0        0     3886 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/functions.py
--rw-r--r--   0        0        0     6342 2023-04-22 09:01:02.179149 strplus-1.0.6/strplus/strplus.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 strplus-1.0.6/setup.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 strplus-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.8/LICENSE
+-rw-r--r--   0        0        0     2907 2023-04-23 15:42:17.477757 strplus-1.0.8/README.md
+-rw-r--r--   0        0        0     1027 2023-04-23 15:42:17.477757 strplus-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-23 15:42:17.477757 strplus-1.0.8/strplus/__init__.py
+-rw-r--r--   0        0        0     5957 2023-04-22 09:01:02.179149 strplus-1.0.8/strplus/cases.py
+-rw-r--r--   0        0        0     9512 2023-04-23 15:42:17.477757 strplus-1.0.8/strplus/functions.py
+-rw-r--r--   0        0        0    12067 2023-04-23 15:42:17.477757 strplus-1.0.8/strplus/strplus.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 strplus-1.0.8/setup.py
+-rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 strplus-1.0.8/PKG-INFO
```

### Comparing `strplus-1.0.6/LICENSE` & `strplus-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.6/README.md` & `strplus-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,28 @@
 [Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀
 
 <br>
 
 ## Features ✨️
 
 - Wrapper Class
-- +234 test in 32 Tests files!
+- +421 test covered in 36 Tests files!
 - Simple use!
 - Made with A.I. contribution 🤖 
 
 <br>
 
+## Install 📀 
+
+```
+pip install strplus
+```
+
+<br>
+
 ### Simple use example 😍
 ```
 my_string = Str('Cast_this_string_TO_Pascal')
 my_string.pascal
 ```
 CastThisStringToPascal
```

#### html2text {}

```diff
@@ -12,16 +12,17 @@
 
 
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
-## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
-- Made with A.I. contribution ð¤
+## Features â¨ï¸ - Wrapper Class - +421 test covered in 36 Tests files! -
+Simple use! - Made with A.I. contribution ð¤
+## Install ð ``` pip install strplus ```
 ### Simple use example ð ``` my_string = Str('Cast_this_string_TO_Pascal')
 my_string.pascal ``` CastThisStringToPascal
 ``` my_string = Str('CastMeUseLikeANormalFunction') my_string.snake ```
 cast_me_use_like_a_normal_function
 * [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
 index.html)!
```

### Comparing `strplus-1.0.6/pyproject.toml` & `strplus-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.6"
+version = "1.0.8"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-1.0.6/strplus/cases.py` & `strplus-1.0.8/strplus/cases.py`

 * *Files identical despite different names*

### Comparing `strplus-1.0.6/setup.py` & `strplus-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.6',
+    'version': '1.0.8',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n\n### Simple use example 😍\n```\nmy_string = Str(\'Cast_this_string_TO_Pascal\')\nmy_string.pascal\n```\nCastThisStringToPascal\n\n<br>\n\n```\nmy_string = Str(\'CastMeUseLikeANormalFunction\')\nmy_string.snake\n```\ncast_me_use_like_a_normal_function\n\n<br>\n\n* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [strplus](https://wiseupdata.github.io/strplus/index.html)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n1. [Wise Up Data](https://github.com/wiseupdata)\n\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +421 test covered in 36 Tests files!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n\n## Install 📀 \n\n```\npip install strplus\n```\n\n<br>\n\n### Simple use example 😍\n```\nmy_string = Str(\'Cast_this_string_TO_Pascal\')\nmy_string.pascal\n```\nCastThisStringToPascal\n\n<br>\n\n```\nmy_string = Str(\'CastMeUseLikeANormalFunction\')\nmy_string.snake\n```\ncast_me_use_like_a_normal_function\n\n<br>\n\n* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [strplus](https://wiseupdata.github.io/strplus/index.html)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n1. [Wise Up Data](https://github.com/wiseupdata)\n\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.6', 'description': 'Python extra functions for strings',
+'1.0.8', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
@@ -16,16 +16,17 @@
 \n\n
 \n
 \n
 \n
 \n
 \n
 \n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
-\n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
-Simple use!\n- Made with A.I. contribution ð¤ \n\n
+\n\n## Features â¨ï¸\n\n- Wrapper Class\n- +421 test covered in 36 Tests
+files!\n- Simple use!\n- Made with A.I. contribution ð¤ \n\n
+\n\n## Install ð \n\n```\npip install strplus\n```\n\n
 \n\n### Simple use example ð\n```\nmy_string = Str
 (\'Cast_this_string_TO_Pascal\')\nmy_string.pascal\n```\nCastThisStringToPascal\n\n
 \n\n```\nmy_string = Str
 (\'CastMeUseLikeANormalFunction\')\nmy_string.snake\n```\ncast_me_use_like_a_normal_function\n\n
 \n\n* [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
 index.html)! \n\n
 \n
```

### Comparing `strplus-1.0.6/PKG-INFO` & `strplus-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.6
+Version: 1.0.8
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -59,20 +59,28 @@
 [Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀
 
 <br>
 
 ## Features ✨️
 
 - Wrapper Class
-- +234 test in 32 Tests files!
+- +421 test covered in 36 Tests files!
 - Simple use!
 - Made with A.I. contribution 🤖 
 
 <br>
 
+## Install 📀 
+
+```
+pip install strplus
+```
+
+<br>
+
 ### Simple use example 😍
 ```
 my_string = Str('Cast_this_string_TO_Pascal')
 my_string.pascal
 ```
 CastThisStringToPascal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.6 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.8 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,17 @@
 
 
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
-## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
-- Made with A.I. contribution ð¤
+## Features â¨ï¸ - Wrapper Class - +421 test covered in 36 Tests files! -
+Simple use! - Made with A.I. contribution ð¤
+## Install ð ``` pip install strplus ```
 ### Simple use example ð ``` my_string = Str('Cast_this_string_TO_Pascal')
 my_string.pascal ``` CastThisStringToPascal
 ``` my_string = Str('CastMeUseLikeANormalFunction') my_string.snake ```
 cast_me_use_like_a_normal_function
 * [Documentation and more examples! ](https://wiseupdata.github.io/strplus/
 index.html)!
```

