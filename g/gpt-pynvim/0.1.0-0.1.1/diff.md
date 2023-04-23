# Comparing `tmp/gpt-pynvim-0.1.0.tar.gz` & `tmp/gpt-pynvim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-pynvim-0.1.0.tar", last modified: Sun Apr 23 08:01:20 2023, max compression
+gzip compressed data, was "gpt-pynvim-0.1.1.tar", last modified: Sun Apr 23 09:27:09 2023, max compression
```

## Comparing `gpt-pynvim-0.1.0.tar` & `gpt-pynvim-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 08:01:20.137679 gpt-pynvim-0.1.0/
--rw-r--r--   0 kiyota     (501) staff       (20)     1072 2023-04-22 01:47:52.000000 gpt-pynvim-0.1.0/LICENSE
--rw-r--r--   0 kiyota     (501) staff       (20)     3858 2023-04-23 08:01:20.137254 gpt-pynvim-0.1.0/PKG-INFO
--rw-r--r--   0 kiyota     (501) staff       (20)     3253 2023-04-23 08:00:48.000000 gpt-pynvim-0.1.0/README.md
-drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 08:01:20.136460 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/
--rw-r--r--   0 kiyota     (501) staff       (20)     3858 2023-04-23 08:01:20.000000 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/PKG-INFO
--rw-r--r--   0 kiyota     (501) staff       (20)      220 2023-04-23 08:01:20.000000 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/SOURCES.txt
--rw-r--r--   0 kiyota     (501) staff       (20)        1 2023-04-23 08:01:20.000000 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/dependency_links.txt
--rw-r--r--   0 kiyota     (501) staff       (20)       14 2023-04-23 08:01:20.000000 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/requires.txt
--rw-r--r--   0 kiyota     (501) staff       (20)        1 2023-04-23 08:01:20.000000 gpt-pynvim-0.1.0/gpt_pynvim.egg-info/top_level.txt
--rw-r--r--   0 kiyota     (501) staff       (20)       38 2023-04-23 08:01:20.137764 gpt-pynvim-0.1.0/setup.cfg
--rw-r--r--   0 kiyota     (501) staff       (20)      907 2023-04-23 07:49:51.000000 gpt-pynvim-0.1.0/setup.py
-drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 08:01:20.136739 gpt-pynvim-0.1.0/tests/
--rw-r--r--   0 kiyota     (501) staff       (20)      127 2023-04-23 07:38:10.000000 gpt-pynvim-0.1.0/tests/test_gpt_pynvim.py
+drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 09:27:09.529488 gpt-pynvim-0.1.1/
+-rw-r--r--   0 kiyota     (501) staff       (20)     1072 2023-04-22 01:47:52.000000 gpt-pynvim-0.1.1/LICENSE
+-rw-r--r--   0 kiyota     (501) staff       (20)     3756 2023-04-23 09:27:09.529213 gpt-pynvim-0.1.1/PKG-INFO
+-rw-r--r--   0 kiyota     (501) staff       (20)     3151 2023-04-23 08:04:26.000000 gpt-pynvim-0.1.1/README.md
+drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 09:27:09.528230 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/
+-rw-r--r--   0 kiyota     (501) staff       (20)     3756 2023-04-23 09:27:09.000000 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/PKG-INFO
+-rw-r--r--   0 kiyota     (501) staff       (20)      220 2023-04-23 09:27:09.000000 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/SOURCES.txt
+-rw-r--r--   0 kiyota     (501) staff       (20)        1 2023-04-23 09:27:09.000000 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/dependency_links.txt
+-rw-r--r--   0 kiyota     (501) staff       (20)       14 2023-04-23 09:27:09.000000 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/requires.txt
+-rw-r--r--   0 kiyota     (501) staff       (20)        1 2023-04-23 09:27:09.000000 gpt-pynvim-0.1.1/gpt_pynvim.egg-info/top_level.txt
+-rw-r--r--   0 kiyota     (501) staff       (20)       38 2023-04-23 09:27:09.529573 gpt-pynvim-0.1.1/setup.cfg
+-rw-r--r--   0 kiyota     (501) staff       (20)      907 2023-04-23 09:27:07.000000 gpt-pynvim-0.1.1/setup.py
+drwxr-xr-x   0 kiyota     (501) staff       (20)        0 2023-04-23 09:27:09.528478 gpt-pynvim-0.1.1/tests/
+-rw-r--r--   0 kiyota     (501) staff       (20)       42 2023-04-23 08:45:04.000000 gpt-pynvim-0.1.1/tests/test_gpt_pynvim.py
```

### Comparing `gpt-pynvim-0.1.0/LICENSE` & `gpt-pynvim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-pynvim-0.1.0/PKG-INFO` & `gpt-pynvim-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-pynvim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A neovim plugin to generate code comments using OpenAI API.
 Home-page: https://github.com/JFK/gpt-pynvim-plugin
 Author: Your Name
 Author-email: fumikazu.kiyota@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT-PyNvim
 
-[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![Downloads](https://static.pepy.tech/badge/gpt-pynvim/month)](https://pepy.tech/project/gpt-pynvim) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
+[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
 
 
 GPT-PyNvim is a Neovim plugin that uses OpenAI's GPT language model to generate code comments or documentation based on selected text within Neovim. This plugin requires Python 3.10 or higher.
 
 ## Directory Tree
 
 ```
```

### Comparing `gpt-pynvim-0.1.0/README.md` & `gpt-pynvim-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GPT-PyNvim
 
-[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![Downloads](https://static.pepy.tech/badge/gpt-pynvim/month)](https://pepy.tech/project/gpt-pynvim) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
+[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
 
 
 GPT-PyNvim is a Neovim plugin that uses OpenAI's GPT language model to generate code comments or documentation based on selected text within Neovim. This plugin requires Python 3.10 or higher.
 
 ## Directory Tree
 
 ```
```

### Comparing `gpt-pynvim-0.1.0/gpt_pynvim.egg-info/PKG-INFO` & `gpt-pynvim-0.1.1/gpt_pynvim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-pynvim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A neovim plugin to generate code comments using OpenAI API.
 Home-page: https://github.com/JFK/gpt-pynvim-plugin
 Author: Your Name
 Author-email: fumikazu.kiyota@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT-PyNvim
 
-[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![Downloads](https://static.pepy.tech/badge/gpt-pynvim/month)](https://pepy.tech/project/gpt-pynvim) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
+[![lint](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/lint.yml) [![test](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/test.yml) [![linkcheck](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/JFK/gpt-pynvim-plugin/actions/workflows/linkcheck.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40kiyotaman)](https://twitter.com/kiyotaman)
 
 
 GPT-PyNvim is a Neovim plugin that uses OpenAI's GPT language model to generate code comments or documentation based on selected text within Neovim. This plugin requires Python 3.10 or higher.
 
 ## Directory Tree
 
 ```
```

### Comparing `gpt-pynvim-0.1.0/setup.py` & `gpt-pynvim-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-pynvim",
-    version="0.1.0",
+    version="0.1.1",
     author="Your Name",
     author_email="fumikazu.kiyota@gmail.com",
     description="A neovim plugin to generate code comments using OpenAI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFK/gpt-pynvim-plugin",
     packages=find_packages(),
```

