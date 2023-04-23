# Comparing `tmp/lmao-nlp-0.0.1b1.tar.gz` & `tmp/lmao-nlp-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b1.tar", last modified: Sun Apr 16 16:52:28 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b2.tar", last modified: Sun Apr 23 00:43:53 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b1.tar` & `lmao-nlp-0.0.1b2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.941734 lmao-nlp-0.0.1b1/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b1/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 16:52:28.941565 lmao-nlp-0.0.1b1/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     4299 2023-04-16 15:48:01.000000 lmao-nlp-0.0.1b1/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b1/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-16 16:52:28.941778 lmao-nlp-0.0.1b1/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-16 16:52:25.000000 lmao-nlp-0.0.1b1/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.932905 lmao-nlp-0.0.1b1/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.934102 lmao-nlp-0.0.1b1/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-16 16:52:25.000000 lmao-nlp-0.0.1b1/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.934746 lmao-nlp-0.0.1b1/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-16 15:36:03.000000 lmao-nlp-0.0.1b1/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1095 2023-04-16 15:21:34.000000 lmao-nlp-0.0.1b1/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b1/src/lmao/adapters/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5360 2023-04-16 15:28:06.000000 lmao-nlp-0.0.1b1/src/lmao/adapters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2166 2023-04-16 15:33:44.000000 lmao-nlp-0.0.1b1/src/lmao/adapters/fermi.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b1/src/lmao/factory.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.935143 lmao-nlp-0.0.1b1/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b1/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.936532 lmao-nlp-0.0.1b1/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b1/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-16 15:14:43.000000 lmao-nlp-0.0.1b1/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b1/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1176 2023-04-16 15:28:44.000000 lmao-nlp-0.0.1b1/src/lmao/lm/clients/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b1/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.937644 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-16 15:15:01.000000 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1061 2023-04-16 15:15:31.000000 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-16 14:59:50.000000 lmao-nlp-0.0.1b1/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b1/src/lmao/lm/utils.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.938084 lmao-nlp-0.0.1b1/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b1/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b1/src/lmao/orchestrators/base.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.938880 lmao-nlp-0.0.1b1/src/lmao/prompters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b1/src/lmao/prompters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b1/src/lmao/prompters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1881 2023-04-16 15:22:27.000000 lmao-nlp-0.0.1b1/src/lmao/prompters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b1/src/lmao/prompters/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.940304 lmao-nlp-0.0.1b1/src/lmao/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b1/src/lmao/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      852 2023-04-16 15:38:11.000000 lmao-nlp-0.0.1b1/src/lmao/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b1/src/lmao/tasks/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b1/src/lmao/tasks/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b1/src/lmao/tasks/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 16:52:28.941368 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 16:52:28.000000 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1082 2023-04-16 16:52:28.000000 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-16 16:52:28.000000 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-16 16:52:28.000000 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-16 16:52:28.000000 lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.219284 lmao-nlp-0.0.1b2/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b2/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 00:43:53.219107 lmao-nlp-0.0.1b2/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     4303 2023-04-16 20:19:27.000000 lmao-nlp-0.0.1b2/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b2/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-23 00:43:53.219324 lmao-nlp-0.0.1b2/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-23 00:43:50.000000 lmao-nlp-0.0.1b2/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.209266 lmao-nlp-0.0.1b2/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.210662 lmao-nlp-0.0.1b2/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-23 00:43:50.000000 lmao-nlp-0.0.1b2/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.212256 lmao-nlp-0.0.1b2/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      123 2023-04-22 20:09:59.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      970 2023-04-22 22:15:41.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      758 2023-04-22 22:14:55.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2643 2023-04-22 22:15:34.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1751 2023-04-22 22:10:11.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/client_mixins.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      933 2023-04-22 22:10:02.000000 lmao-nlp-0.0.1b2/src/lmao/adapters/fermi.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b2/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.212824 lmao-nlp-0.0.1b2/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.214464 lmao-nlp-0.0.1b2/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2238 2023-04-22 22:10:41.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5375 2023-04-22 21:40:12.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1164 2023-04-22 22:10:57.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2763 2023-04-22 22:09:36.000000 lmao-nlp-0.0.1b2/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.215661 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1140 2023-04-22 22:11:55.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1056 2023-04-22 22:12:01.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-22 22:12:02.000000 lmao-nlp-0.0.1b2/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b2/src/lmao/lm/utils.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.216034 lmao-nlp-0.0.1b2/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b2/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b2/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.216822 lmao-nlp-0.0.1b2/src/lmao/prompters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1876 2023-04-22 22:12:14.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      751 2023-04-22 22:12:18.000000 lmao-nlp-0.0.1b2/src/lmao/prompters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.218129 lmao-nlp-0.0.1b2/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      842 2023-04-22 22:12:32.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      749 2023-04-22 22:10:17.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1239 2023-04-22 22:09:47.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      616 2023-04-22 22:04:00.000000 lmao-nlp-0.0.1b2/src/lmao/tasks/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-23 00:43:53.218853 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1117 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-23 00:43:53.000000 lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b1/LICENSE` & `lmao-nlp-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b1/PKG-INFO` & `lmao-nlp-0.0.1b2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b1/README.md` & `lmao-nlp-0.0.1b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # 🙊 LMAO: **L**anguage **M**odel **A**dapters and **O**rchestrators
 
 <img src="assets/icon.png" height="210" align="right" />
 
-> The data scientist's toolkit for adapting large LMs to solve a diverse set of tasks
+> The data scientist's toolkit for adapting large LMs to perform a diverse set of tasks
 
 <br>
 
-`lmao` is an open-source library for integrating large language models (LLMs) from providers like [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) into your NLP workflows. For example, it can be used to pre-annotate text datasets using zero- or few-shot learning with Claude or GPT-4. LMAO is in the (very) early stages of development. New features will be added with high cadence and documentation is coming soon.
+`lmao` is an open-source library for integrating large language models (LLMs) from providers like [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) into your NLP workflows. For example, it can be used to pre-annotate text datasets using zero- or few-shot learning with Claude or GPT-4. `lmao` is in the (very) early stages of development. New features will be added with high cadence and documentation is coming soon.
 
 ## Installation
 The package is available on PyPI and can be installed with pip:
 ```bash
 pip install lmao-nlp
 ```
 > ⚠️ Don't forget the `-nlp` extension on the distribution name!
```

### Comparing `lmao-nlp-0.0.1b1/pyproject.toml` & `lmao-nlp-0.0.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b1/setup.py` & `lmao-nlp-0.0.1b2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.1"
+__version__ = "0.0.1-beta.2"
 
 install_requires = [
     "pydantic>=1.10.7",
     "requests>=2.28.2",
     "tiktoken>=0.3.3",
 ]
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/factory.py` & `lmao-nlp-0.0.1b2/src/lmao/factory.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/clients/anthropic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple, Optional
 
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
-from lmao.lm.schemas.anthropic import AnthropicCompleteSchema
+from lmao.lm.clients import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
+from lmao.lm.schemas import AnthropicCompleteSchema
 
 __all__ = ["AnthropicClient", "AnthropicChatHistory"]
 
 
 class Schema(NamedTuple):
     complete: dict
 
@@ -27,15 +27,15 @@
     def to_prompt(self, end_with_assistant_prompt: bool = True) -> str:
         chat = "\n\n".join([f"{message['role'].title()}: {message['content']}" for message in self._messages])
         if end_with_assistant_prompt:
             chat += "\n\nAssistant:"
         return chat
 
     def to_request_format(self, end_with_assistant_prompt: bool = True):
-        return self.to_prompt(end_with_assistant_prompt=end_with_assistant_prompt)
+        return {"prompt": self.to_prompt(end_with_assistant_prompt=end_with_assistant_prompt)}
 
 
 class AnthropicClient(BaseClient):
     base_url = "https://api.anthropic.com"
     api_env_name = "ANTHROPIC_API_KEY"
     api_header_format = "x-api-key"
 
@@ -50,7 +50,10 @@
             AnthropicCompleteSchema(prompt=prompt, **kwargs).to_request_dict(),
         )
         return ClientResponse(
             text=response["completion"] if status_code == SUCCESS_STATUS_CODE else None,
             raw_response=response,
             status_code=status_code,
         )
+
+    def create_chat_history(self, max_length: int = 5) -> AnthropicChatHistory:
+        return AnthropicChatHistory(max_length=max_length)
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/clients/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,25 +100,25 @@
     api_env_name: Optional[str] = None
     api_header_format: Optional[str] = None
 
     #  If the backoff_factor is 0.1, then sleep() will sleep for [0.0s, 0.2s, 0.4s, …] between retries.
     RETRY_BACKOFF_FACTOR: float = 0.1
     RETRY_STATUS_CODES: List[int] = [429, 500, 502, 503, 504]
 
-    def __init__(self, api_key: Optional[str] = None, max_retries: int = 5, default_method_name: str = "complete"):
+    def __init__(self, api_key: Optional[str] = None, max_retries: int = 5):
         self.max_retries = max_retries
         self.__api_key = api_key or os.environ.get(self.api_env_name or "")
         if self.__api_key is None:
             raise ValueError("You must provide an API key or set api_env_name to initialize an LM Client.")
         if self.base_url is None:
             raise ValueError("Client subclasses must define a base URL attribute.")
         if self.api_header_format not in API_HEADER_FORMAT_DICT:
             raise ValueError(f"Client subclasses must have api_header_format in {list(API_HEADER_FORMAT_DICT.keys())}")
         self._api_header = API_HEADER_FORMAT_DICT[self.api_header_format]
-        self.default_method_name = default_method_name
+        self._target_api_endpoint: Optional[str] = None
 
     def _post_request(self, api_path: str, request: dict, extra_headers: Optional[dict] = None) -> Tuple[int, dict]:
         with requests.Session() as session:
             retries = Retry(
                 total=self.max_retries,
                 backoff_factor=self.RETRY_BACKOFF_FACTOR,
                 status_forcelist=self.RETRY_STATUS_CODES,
@@ -138,7 +138,13 @@
         status_code = response.status_code
         try:
             response_dict = response.json()
         except requests.exceptions.JSONDecodeError:
             response_dict = {}
             status_code = 500 if status_code != SUCCESS_STATUS_CODE else status_code
         return status_code, response_dict
+
+    def create_chat_history(self, max_length: int = 10) -> ChatHistory:
+        raise NotImplementedError("Client subclasses must implement create_chat_history.")
+
+    def set_target_api_endpoint(self, name: str):
+        self._target_api_endpoint = name
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/clients/cohere.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/clients/cohere.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple, Optional
 
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE, BaseClient, ClientResponse
-from lmao.lm.schemas.cohere import CohereCompleteSchema
+from lmao.lm.clients import SUCCESS_STATUS_CODE, BaseClient, ClientResponse
+from lmao.lm.schemas import CohereCompleteSchema
 
 __all__ = ["CohereClient"]
 
 
 class Schema(NamedTuple):
     complete: dict
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/clients/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, NamedTuple, Optional
 
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
-from lmao.lm.schemas.openai import OpenAIChatSchema, OpenAICompleteSchema
+from lmao.lm.clients import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
+from lmao.lm.schemas import OpenAIChatSchema, OpenAICompleteSchema
 
 __all__ = ["OpenAIClient", "OpenAIChatHistory"]
 
 
 DEFAULT_SYSTEM_MESSAGE = "You are a helpful assistant."
 
 
@@ -27,15 +27,15 @@
         if "content" not in message:
             raise ValueError("Message must have a 'content' key.")
         if message["role"].lower() not in ["user", "assistant"]:
             raise ValueError("Message role must be 'user' or 'assistant'.")
         return message
 
     def to_request_format(self):
-        return self.messages
+        return {"messages": self.messages}
 
 
 class OpenAIClient(BaseClient):
     base_url = "https://api.openai.com/v1"
     api_env_name = "OPENAI_API_KEY"
     api_header_format = "bearer authentication"
 
@@ -67,7 +67,10 @@
             "completions", OpenAICompleteSchema(prompt=prompt, **kwargs).to_request_dict()
         )
         return ClientResponse(
             text=response["choices"][0]["text"] if status_code == SUCCESS_STATUS_CODE else None,
             raw_response=response,
             status_code=status_code,
         )
+
+    def create_chat_history(self, max_length: int = 10) -> OpenAIChatHistory:
+        return OpenAIChatHistory(max_length=max_length)
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import List, Optional
 
 from pydantic import Extra, Field, validator
 
-from lmao.lm.schemas.base import API_DEFAULTS, BaseSchema
+from lmao.lm.schemas import API_DEFAULTS, BaseSchema
 
 __all__ = ["AnthropicCompleteSchema", "anthropic_model_regex"]
 
 
 anthropic_model_regex = dict(complete=re.compile(r"claude-(?:instant-)?v\d(?:\.\d)?"))
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/schemas/cohere.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/cohere.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 
 from pydantic import Field
 
-from lmao.lm.schemas.base import API_DEFAULTS, BaseSchema
+from lmao.lm.schemas import API_DEFAULTS, BaseSchema
 
 __all__ = ["CohereCompleteSchema"]
 
 
 class CohereCompleteSchema(BaseSchema):
     """API Reference: https://docs.cohere.ai/reference/generate"""
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/schemas/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b1/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b2/src/lmao/lm/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b1/src/lmao/prompters/classification.py` & `lmao-nlp-0.0.1b2/src/lmao/prompters/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lmao.prompters.base import Prompter, build_prompt_template
+from lmao.prompters import Prompter, build_prompt_template
 
 __all__ = ["ClassificationPrompter", "SentimentAnalysisPrompter"]
 
 
 class ClassificationPrompter(Prompter):
     task = "classification"
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/prompters/fermi.py` & `lmao-nlp-0.0.1b2/src/lmao/prompters/fermi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lmao.prompters.base import Prompter, build_prompt_template
+from lmao.prompters import Prompter, build_prompt_template
 
 __all__ = ["FermiProblemPrompter"]
 
 
 class FermiProblemPrompter(Prompter):
     template = build_prompt_template(
         intro=(
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/tasks/base.py` & `lmao-nlp-0.0.1b2/src/lmao/tasks/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import NamedTuple, Protocol, runtime_checkable
 
-from lmao.adapters.base import BaseAdapter
-from lmao.lm.clients.base import ClientResponse
+from lmao.adapters import BaseAdapter
+from lmao.lm.clients import ClientResponse
 
 __all__ = ["task_errors", "ModelTaskProtocol", "QATaskProtocol", "TaskResponse"]
 
 
 class TaskErrors(NamedTuple):
     CLIENT_ERROR: str
     PREDICTION_ERROR: str
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/tasks/chatbot.py` & `lmao-nlp-0.0.1b2/src/lmao/tasks/chatbot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from lmao.adapters.base import BaseChatbotAdapter
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE, ClientResponse
+from lmao.adapters import BaseChatbotAdapter
+from lmao.lm.clients import SUCCESS_STATUS_CODE, ClientResponse
 
 __all__ = ["Chatbot"]
 
 
 class Chatbot:
     def __init__(self, adapter: BaseChatbotAdapter):
         self.adapter = adapter
         self.client = adapter.client
         self.history = adapter.chat_history
 
     def chat(self, message: str, **kwargs) -> ClientResponse:
         self.history.add_human_message(message)
-        kwargs.update(self.adapter.to_endpoint_kwargs(self.history.to_request_format()))
-        response = getattr(self.client, self.adapter.endpoint_method_name)(**kwargs)
+        kwargs.update((self.history.to_request_format()))
+        response = getattr(self.client, str(self.client._target_api_endpoint))(**kwargs)
         if response.status_code == SUCCESS_STATUS_CODE:
             self.history.add_assistant_message(response.text)
         return self.adapter.postprocess_response(response)
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao/tasks/classification.py` & `lmao-nlp-0.0.1b2/src/lmao/tasks/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from lmao.adapters import TextClassificationAdapter
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE
-from lmao.tasks.base import TaskResponse, task_errors
+from lmao.lm.clients import SUCCESS_STATUS_CODE
+from lmao.tasks import TaskResponse, task_errors
 
 __all__ = ["TextClassification"]
 
 
 class TextClassification:
     def __init__(self, adapter: TextClassificationAdapter):
         self.categories = adapter.categories
         self.adapter: TextClassificationAdapter = adapter
 
     def predict(self, text: str, **kwargs) -> TaskResponse:
         success = True
         input_text = self.adapter.prompter.create_prompt(text)
-        kwargs.update(self.adapter.to_endpoint_kwargs(input_text))
-        response = getattr(self.adapter.client, self.adapter.endpoint_method_name)(**kwargs)
+        kwargs.update(self.adapter.prepare_input_content(input_text))
+        response = getattr(self.adapter.client, str(self.adapter.client._target_api_endpoint))(**kwargs)
         if response.status_code == SUCCESS_STATUS_CODE:
             prediction = response.text.strip().lower() if self.adapter.lowercase else response.text.strip()
             prediction = prediction.replace(".", "")
             if prediction not in self.categories:
                 prediction = task_errors.PREDICTION_ERROR
                 success = False
         else:
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b1/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b2/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/lmao/__init__.py
 src/lmao/factory.py
 src/lmao/adapters/__init__.py
 src/lmao/adapters/base.py
 src/lmao/adapters/chatbot.py
 src/lmao/adapters/classification.py
+src/lmao/adapters/client_mixins.py
 src/lmao/adapters/fermi.py
 src/lmao/lm/__init__.py
 src/lmao/lm/utils.py
 src/lmao/lm/clients/__init__.py
 src/lmao/lm/clients/anthropic.py
 src/lmao/lm/clients/base.py
 src/lmao/lm/clients/cohere.py
```

