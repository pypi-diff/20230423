# Comparing `tmp/lmao-nlp-0.0.1b2.tar.gz` & `tmp/lmao-nlp-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b2.tar", last modified: Sun Apr 23 00:43:53 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b3.tar", last modified: Sun Apr 23 01:05:21 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b2.tar` & `lmao-nlp-0.0.1b3.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.219284 lmao-nlp-0.0.1b2/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b2/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 00:43:53.219107 lmao-nlp-0.0.1b2/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     4303 2023-04-16 20:19:27.000000 lmao-nlp-0.0.1b2/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b2/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-23 00:43:53.219324 lmao-nlp-0.0.1b2/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-23 00:43:50.000000 lmao-nlp-0.0.1b2/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.209266 lmao-nlp-0.0.1b2/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.210662 lmao-nlp-0.0.1b2/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-23 00:43:50.000000 lmao-nlp-0.0.1b2/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.212256 lmao-nlp-0.0.1b2/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      123 2023-04-22 20:09:59.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      970 2023-04-22 22:15:41.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      758 2023-04-22 22:14:55.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2643 2023-04-22 22:15:34.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1751 2023-04-22 22:10:11.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/client_mixins.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      933 2023-04-22 22:10:02.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/fermi.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b2/src/lmao/factory.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.212824 lmao-nlp-0.0.1b2/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.214464 lmao-nlp-0.0.1b2/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2238 2023-04-22 22:10:41.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5375 2023-04-22 21:40:12.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1164 2023-04-22 22:10:57.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2763 2023-04-22 22:09:36.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.215661 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1140 2023-04-22 22:11:55.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1056 2023-04-22 22:12:01.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-22 22:12:02.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b2/src/lmao/lm/utils.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.216034 lmao-nlp-0.0.1b2/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b2/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b2/src/lmao/orchestrators/base.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.216822 lmao-nlp-0.0.1b2/src/lmao/prompters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1876 2023-04-22 22:12:14.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      751 2023-04-22 22:12:18.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.218129 lmao-nlp-0.0.1b2/src/lmao/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      842 2023-04-22 22:12:32.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      749 2023-04-22 22:10:17.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1239 2023-04-22 22:09:47.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      616 2023-04-22 22:04:00.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.218853 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1117 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.705405 lmao-nlp-0.0.1b3/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b3/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 01:05:21.705240 lmao-nlp-0.0.1b3/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     4303 2023-04-16 20:19:27.000000 lmao-nlp-0.0.1b3/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b3/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-23 01:05:21.705452 lmao-nlp-0.0.1b3/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-23 01:05:18.000000 lmao-nlp-0.0.1b3/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.699426 lmao-nlp-0.0.1b3/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.700536 lmao-nlp-0.0.1b3/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      181 2023-04-23 01:05:18.000000 lmao-nlp-0.0.1b3/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.701323 lmao-nlp-0.0.1b3/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      123 2023-04-22 20:09:59.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      961 2023-04-23 00:54:22.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      776 2023-04-23 00:55:01.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2658 2023-04-23 00:55:30.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1745 2023-04-23 00:55:48.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/client_mixins.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      948 2023-04-23 00:56:35.000000 lmao-nlp-0.0.1b3/src/lmao/adapters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.702079 lmao-nlp-0.0.1b3/src/lmao/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      111 2023-04-23 00:57:18.000000 lmao-nlp-0.0.1b3/src/lmao/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2234 2023-04-23 00:58:01.000000 lmao-nlp-0.0.1b3/src/lmao/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5375 2023-04-22 21:40:12.000000 lmao-nlp-0.0.1b3/src/lmao/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1160 2023-04-23 00:58:21.000000 lmao-nlp-0.0.1b3/src/lmao/clients/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2763 2023-04-22 22:09:36.000000 lmao-nlp-0.0.1b3/src/lmao/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.702709 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1130 2023-04-23 00:57:03.000000 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1046 2023-04-23 00:57:14.000000 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2703 2023-04-23 00:57:27.000000 lmao-nlp-0.0.1b3/src/lmao/clients/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b3/src/lmao/clients/utils.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2880 2023-04-23 01:01:24.000000 lmao-nlp-0.0.1b3/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.702923 lmao-nlp-0.0.1b3/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b3/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b3/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.703355 lmao-nlp-0.0.1b3/src/lmao/prompters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b3/src/lmao/prompters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b3/src/lmao/prompters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1867 2023-04-23 00:58:48.000000 lmao-nlp-0.0.1b3/src/lmao/prompters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      742 2023-04-23 00:58:58.000000 lmao-nlp-0.0.1b3/src/lmao/prompters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.704260 lmao-nlp-0.0.1b3/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b3/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      833 2023-04-23 00:59:15.000000 lmao-nlp-0.0.1b3/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      740 2023-04-23 00:59:26.000000 lmao-nlp-0.0.1b3/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1225 2023-04-23 00:59:44.000000 lmao-nlp-0.0.1b3/src/lmao/tasks/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      607 2023-04-23 01:01:33.000000 lmao-nlp-0.0.1b3/src/lmao/tasks/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 01:05:21.705009 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 01:05:21.000000 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1108 2023-04-23 01:05:21.000000 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-23 01:05:21.000000 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-23 01:05:21.000000 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-23 01:05:21.000000 lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b2/LICENSE` & `lmao-nlp-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/PKG-INFO` & `lmao-nlp-0.0.1b3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b2/README.md` & `lmao-nlp-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/pyproject.toml` & `lmao-nlp-0.0.1b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/setup.py` & `lmao-nlp-0.0.1b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.2"
+__version__ = "0.0.1-beta.3"
 
 install_requires = [
     "pydantic>=1.10.7",
     "requests>=2.28.2",
     "tiktoken>=0.3.3",
 ]
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/adapters/base.py` & `lmao-nlp-0.0.1b3/src/lmao/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
-from lmao.lm.clients import BaseClient, ClientResponse
-from lmao.prompters import Prompter
+from ..clients import BaseClient, ClientResponse
+from ..prompters import Prompter
 
 __all__ = ["BaseAdapter", "BaseTaskAdapter"]
 
 
 class BaseAdapter(ABC):
     def __init__(self, api_key: Optional[str] = None, **kwargs):
         self.client = self.load_client(api_key, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/adapters/chatbot.py` & `lmao-nlp-0.0.1b3/src/lmao/adapters/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
-from lmao.adapters import AnthropicAdapterMixin, BaseAdapter, OpenAIAdapterMixin
+from .base import BaseAdapter
+from .client_mixins import AnthropicAdapterMixin, OpenAIAdapterMixin
 
 __all__ = ["AnthropicChatbotAdapter", "BaseChatbotAdapter", "OpenAIChatbotAdapter"]
 
 
 class BaseChatbotAdapter(BaseAdapter):
     def __init__(self, chat_history_length: int = 5, api_key: Optional[str] = None, **kwargs):
         super().__init__(api_key, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/adapters/classification.py` & `lmao-nlp-0.0.1b3/src/lmao/adapters/classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional
 
-from lmao.adapters import AnthropicAdapterMixin, BaseTaskAdapter, CohereAdapterMixin, OpenAIAdapterMixin
-from lmao.prompters import ClassificationPrompter, Prompter, SentimentAnalysisPrompter
+from ..prompters import ClassificationPrompter, Prompter, SentimentAnalysisPrompter
+from .base import BaseTaskAdapter
+from .client_mixins import AnthropicAdapterMixin, CohereAdapterMixin, OpenAIAdapterMixin
 
 __all__ = [
     "AnthropicSentimentAnalysisAdapter",
     "AnthropicTextClassificationAdapter",
     "CohereSentimentAnalysisAdapter",
     "CohereTextClassificationAdapter",
     "OpenAISentimentAnalysisAdapter",
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/adapters/client_mixins.py` & `lmao-nlp-0.0.1b3/src/lmao/adapters/client_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from lmao.lm.clients import AnthropicClient, ClientResponse, CohereClient, OpenAIClient
+from ..clients import AnthropicClient, ClientResponse, CohereClient, OpenAIClient
 
 __all__ = ["AnthropicAdapterMixin", "CohereAdapterMixin", "OpenAIAdapterMixin"]
 
 
 class AnthropicAdapterMixin:
     def load_client(self, api_key: Optional[str] = None, **kwargs):
         client = AnthropicClient(api_key, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/adapters/fermi.py` & `lmao-nlp-0.0.1b3/src/lmao/adapters/fermi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
-from lmao.adapters import AnthropicAdapterMixin, BaseTaskAdapter, CohereAdapterMixin, OpenAIAdapterMixin
-from lmao.prompters import FermiProblemPrompter
+from ..prompters import FermiProblemPrompter
+from .base import BaseTaskAdapter
+from .client_mixins import AnthropicAdapterMixin, CohereAdapterMixin, OpenAIAdapterMixin
 
 __all__ = [
     "FermiProblemAdapter",
     "AnthropicFermiProblemAdapter",
     "CohereFermiProblemAdapter",
     "OpenAIFermiProblemAdapter",
 ]
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/factory.py` & `lmao-nlp-0.0.1b3/src/lmao/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import NamedTuple, Tuple, Union
 
-import lmao.adapters as adapters
-import lmao.lm.clients as clients
-import lmao.tasks as tasks
+from . import adapters, clients, tasks
 
 __all__ = ["create_chatbot", "create_client", "create_task"]
 
 
 class ObjectMapping(NamedTuple):
     name_to_client: dict = {
         "anthropic": clients.AnthropicClient,
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/anthropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple, Optional
 
-from lmao.lm.clients import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
-from lmao.lm.schemas import AnthropicCompleteSchema
+from ..clients import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
+from ..clients.schemas import AnthropicCompleteSchema
 
 __all__ = ["AnthropicClient", "AnthropicChatHistory"]
 
 
 class Schema(NamedTuple):
     complete: dict
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/clients/cohere.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/cohere.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple, Optional
 
-from lmao.lm.clients import SUCCESS_STATUS_CODE, BaseClient, ClientResponse
-from lmao.lm.schemas import CohereCompleteSchema
+from ..clients import SUCCESS_STATUS_CODE, BaseClient, ClientResponse
+from ..clients.schemas import CohereCompleteSchema
 
 __all__ = ["CohereClient"]
 
 
 class Schema(NamedTuple):
     complete: dict
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/schemas/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import List, Optional
 
 from pydantic import Extra, Field, validator
 
-from lmao.lm.schemas import API_DEFAULTS, BaseSchema
+from .base import API_DEFAULTS, BaseSchema
 
 __all__ = ["AnthropicCompleteSchema", "anthropic_model_regex"]
 
 
 anthropic_model_regex = dict(complete=re.compile(r"claude-(?:instant-)?v\d(?:\.\d)?"))
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/cohere.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/schemas/cohere.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 
 from pydantic import Field
 
-from lmao.lm.schemas import API_DEFAULTS, BaseSchema
+from .base import API_DEFAULTS, BaseSchema
 
 __all__ = ["CohereCompleteSchema"]
 
 
 class CohereCompleteSchema(BaseSchema):
     """API Reference: https://docs.cohere.ai/reference/generate"""
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/schemas/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import Dict, List, Optional, Union
 
 from pydantic import Extra, Field, validator
 
-from lmao.lm.schemas import API_DEFAULTS, BaseSchema
+from .base import API_DEFAULTS, BaseSchema
 
 __all__ = ["OpenAIChatSchema", "OpenAICompleteSchema", "openai_model_regex"]
 
 
 model_versions = r"(?:3\.5-turbo|4)"
 date_label_pattern = r"(?:0[1-9]|1[012])(?:0[1-9]|[12][0-9]|3[01])$"
 openai_model_regex = dict(
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b3/src/lmao/clients/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b2/src/lmao/prompters/classification.py` & `lmao-nlp-0.0.1b3/src/lmao/prompters/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lmao.prompters import Prompter, build_prompt_template
+from .base import Prompter, build_prompt_template
 
 __all__ = ["ClassificationPrompter", "SentimentAnalysisPrompter"]
 
 
 class ClassificationPrompter(Prompter):
     task = "classification"
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/prompters/fermi.py` & `lmao-nlp-0.0.1b3/src/lmao/prompters/fermi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lmao.prompters import Prompter, build_prompt_template
+from .base import Prompter, build_prompt_template
 
 __all__ = ["FermiProblemPrompter"]
 
 
 class FermiProblemPrompter(Prompter):
     template = build_prompt_template(
         intro=(
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/tasks/base.py` & `lmao-nlp-0.0.1b3/src/lmao/tasks/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import NamedTuple, Protocol, runtime_checkable
 
-from lmao.adapters import BaseAdapter
-from lmao.lm.clients import ClientResponse
+from ..adapters import BaseAdapter
+from ..clients import ClientResponse
 
 __all__ = ["task_errors", "ModelTaskProtocol", "QATaskProtocol", "TaskResponse"]
 
 
 class TaskErrors(NamedTuple):
     CLIENT_ERROR: str
     PREDICTION_ERROR: str
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/tasks/chatbot.py` & `lmao-nlp-0.0.1b3/src/lmao/tasks/chatbot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from lmao.adapters import BaseChatbotAdapter
-from lmao.lm.clients import SUCCESS_STATUS_CODE, ClientResponse
+from ..adapters import BaseChatbotAdapter
+from ..clients import SUCCESS_STATUS_CODE, ClientResponse
 
 __all__ = ["Chatbot"]
 
 
 class Chatbot:
     def __init__(self, adapter: BaseChatbotAdapter):
         self.adapter = adapter
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/tasks/classification.py` & `lmao-nlp-0.0.1b3/src/lmao/tasks/classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from lmao.adapters import TextClassificationAdapter
-from lmao.lm.clients import SUCCESS_STATUS_CODE
-from lmao.tasks import TaskResponse, task_errors
+from ..adapters import TextClassificationAdapter
+from ..clients import SUCCESS_STATUS_CODE
+from .base import TaskResponse, task_errors
 
 __all__ = ["TextClassification"]
 
 
 class TextClassification:
     def __init__(self, adapter: TextClassificationAdapter):
         self.categories = adapter.categories
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao/tasks/fermi.py` & `lmao-nlp-0.0.1b3/src/lmao/tasks/fermi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from lmao.adapters import FermiProblemAdapter
-from lmao.lm.clients import ClientResponse
+from ..adapters import FermiProblemAdapter
+from ..clients import ClientResponse
 
 __all__ = ["FermiProblem"]
 
 
 class FermiProblem:
     def __init__(self, adapter: FermiProblemAdapter):
         self.adapter = adapter
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b3/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 src/lmao/factory.py
 src/lmao/adapters/__init__.py
 src/lmao/adapters/base.py
 src/lmao/adapters/chatbot.py
 src/lmao/adapters/classification.py
 src/lmao/adapters/client_mixins.py
 src/lmao/adapters/fermi.py
-src/lmao/lm/__init__.py
-src/lmao/lm/utils.py
-src/lmao/lm/clients/__init__.py
-src/lmao/lm/clients/anthropic.py
-src/lmao/lm/clients/base.py
-src/lmao/lm/clients/cohere.py
-src/lmao/lm/clients/openai.py
-src/lmao/lm/schemas/__init__.py
-src/lmao/lm/schemas/anthropic.py
-src/lmao/lm/schemas/base.py
-src/lmao/lm/schemas/cohere.py
-src/lmao/lm/schemas/openai.py
+src/lmao/clients/__init__.py
+src/lmao/clients/anthropic.py
+src/lmao/clients/base.py
+src/lmao/clients/cohere.py
+src/lmao/clients/openai.py
+src/lmao/clients/utils.py
+src/lmao/clients/schemas/__init__.py
+src/lmao/clients/schemas/anthropic.py
+src/lmao/clients/schemas/base.py
+src/lmao/clients/schemas/cohere.py
+src/lmao/clients/schemas/openai.py
 src/lmao/orchestrators/__init__.py
 src/lmao/orchestrators/base.py
 src/lmao/prompters/__init__.py
 src/lmao/prompters/base.py
 src/lmao/prompters/classification.py
 src/lmao/prompters/fermi.py
 src/lmao/tasks/__init__.py
```

