# Comparing `tmp/cloudlanguagetools-5.2.tar.gz` & `tmp/cloudlanguagetools-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-5.2.tar", last modified: Thu Apr 13 04:54:30 2023, max compression
+gzip compressed data, was "cloudlanguagetools-5.3.tar", last modified: Sun Apr 23 13:26:11 2023, max compression
```

## Comparing `cloudlanguagetools-5.2.tar` & `cloudlanguagetools-5.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 04:54:30.180134 cloudlanguagetools-5.2/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-04-13 04:54:30.180134 cloudlanguagetools-5.2/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-03-31 05:42:35.000000 cloudlanguagetools-5.2/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 04:54:30.179134 cloudlanguagetools-5.2/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23228 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4288 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2104 2023-04-04 02:45:57.000000 cloudlanguagetools-5.2/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-03-31 05:42:35.000000 cloudlanguagetools-5.2/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8418 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6035 2023-04-04 02:45:57.000000 cloudlanguagetools-5.2/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    12687 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-04-13 04:54:02.000000 cloudlanguagetools-5.2/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1705 2023-04-13 04:54:02.000000 cloudlanguagetools-5.2/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17689 2023-04-04 02:45:57.000000 cloudlanguagetools-5.2/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1115 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-04-04 02:45:57.000000 cloudlanguagetools-5.2/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-03-28 05:23:58.000000 cloudlanguagetools-5.2/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 04:54:30.180134 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-04-13 04:54:29.000000 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1367 2023-04-13 04:54:30.000000 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 04:54:29.000000 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 04:54:29.000000 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-04-13 04:54:30.000000 cloudlanguagetools-5.2/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 04:54:30.180134 cloudlanguagetools-5.2/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      893 2023-04-13 04:54:25.000000 cloudlanguagetools-5.2/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 13:26:11.427140 cloudlanguagetools-5.3/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-04-23 13:26:11.427140 cloudlanguagetools-5.3/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-03-31 05:42:35.000000 cloudlanguagetools-5.3/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 13:26:11.426139 cloudlanguagetools-5.3/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23228 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4288 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2104 2023-04-04 02:45:57.000000 cloudlanguagetools-5.3/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-03-31 05:42:35.000000 cloudlanguagetools-5.3/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8418 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6035 2023-04-04 02:45:57.000000 cloudlanguagetools-5.3/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    12687 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-04-13 04:54:02.000000 cloudlanguagetools-5.3/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1705 2023-04-13 04:54:02.000000 cloudlanguagetools-5.3/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17689 2023-04-04 02:45:57.000000 cloudlanguagetools-5.3/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1115 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-04-04 02:45:57.000000 cloudlanguagetools-5.3/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-03-28 05:23:58.000000 cloudlanguagetools-5.3/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 13:26:11.427140 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-04-23 13:26:10.000000 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1367 2023-04-23 13:26:11.000000 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-23 13:26:10.000000 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-04-23 13:26:11.000000 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-04-23 13:26:11.000000 cloudlanguagetools-5.3/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-23 13:26:11.427140 cloudlanguagetools-5.3/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-04-23 13:26:07.000000 cloudlanguagetools-5.3/setup.py
```

### Comparing `cloudlanguagetools-5.2/LICENSE` & `cloudlanguagetools-5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/PKG-INFO` & `cloudlanguagetools-5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.2
+Version: 5.3
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/amazon.py` & `cloudlanguagetools-5.3/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-5.3/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/azure.py` & `cloudlanguagetools-5.3/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-5.3/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/constants.py` & `cloudlanguagetools-5.3/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/deepl.py` & `cloudlanguagetools-5.3/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-5.3/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-5.3/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/encryption.py` & `cloudlanguagetools-5.3/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/epitran.py` & `cloudlanguagetools-5.3/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/forvo.py` & `cloudlanguagetools-5.3/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/fptai.py` & `cloudlanguagetools-5.3/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/google.py` & `cloudlanguagetools-5.3/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/keys.py` & `cloudlanguagetools-5.3/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/languages.py` & `cloudlanguagetools-5.3/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-5.3/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-5.3/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/naver.py` & `cloudlanguagetools-5.3/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/openai.py` & `cloudlanguagetools-5.3/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-5.3/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-5.3/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/spacy.py` & `cloudlanguagetools-5.3/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/test_services.py` & `cloudlanguagetools-5.3/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-5.3/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-5.3/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-5.3/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-5.3/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-5.3/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/voicen.py` & `cloudlanguagetools-5.3/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/watson.py` & `cloudlanguagetools-5.3/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-5.3/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-5.3/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.2
+Version: 5.3
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.2/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-5.3/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.2/setup.py` & `cloudlanguagetools-5.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='5.2',
+      version='5.3',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],      
       license='GPL',
       packages=['cloudlanguagetools'],
       install_requires=[
           'clt_wenlin>=1.0',
-          'clt_requirements>=0.8'
+          'clt_requirements>=0.8',
+          'pinyin_jyutping>=0.8',
       ],
       )
```

