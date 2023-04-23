# Comparing `tmp/openthaigpt-0.0.9.tar.gz` & `tmp/openthaigpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openthaigpt-0.0.9.tar", last modified: Sun Mar 19 14:16:40 2023, max compression
+gzip compressed data, was "openthaigpt-0.1.0.tar", last modified: Sun Apr 23 17:03:39 2023, max compression
```

## Comparing `openthaigpt-0.0.9.tar` & `openthaigpt-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-03-19 14:16:40.701942 openthaigpt-0.0.9/
--rw-r--r--   0 kv         (501) staff       (20)      130 2023-03-11 07:31:58.000000 openthaigpt-0.0.9/AUTHORS.md
--rw-r--r--   0 kv         (501) staff       (20)     3406 2023-03-11 07:32:57.000000 openthaigpt-0.0.9/CONTRIBUTING.md
--rw-r--r--   0 kv         (501) staff       (20)      303 2023-03-19 14:06:09.000000 openthaigpt-0.0.9/HISTORY.md
--rw-r--r--   0 kv         (501) staff       (20)      595 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/LICENSE
--rw-r--r--   0 kv         (501) staff       (20)      257 2023-03-11 07:31:36.000000 openthaigpt-0.0.9/MANIFEST.in
--rw-r--r--   0 kv         (501) staff       (20)     2926 2023-03-19 14:16:40.702002 openthaigpt-0.0.9/PKG-INFO
--rw-r--r--   0 kv         (501) staff       (20)     1502 2023-03-19 14:05:46.000000 openthaigpt-0.0.9/README.md
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-03-19 14:16:40.699640 openthaigpt-0.0.9/docs/
--rw-r--r--   0 kv         (501) staff       (20)      612 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/docs/Makefile
--rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:31:16.000000 openthaigpt-0.0.9/docs/authors.rst
--rwxr-xr-x   0 kv         (501) staff       (20)     4862 2023-03-11 07:31:10.000000 openthaigpt-0.0.9/docs/conf.py
--rw-r--r--   0 kv         (501) staff       (20)       32 2023-03-11 07:31:04.000000 openthaigpt-0.0.9/docs/contributing.rst
--rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:30:55.000000 openthaigpt-0.0.9/docs/history.rst
--rw-r--r--   0 kv         (501) staff       (20)      308 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/docs/index.rst
--rw-r--r--   0 kv         (501) staff       (20)     1142 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/docs/installation.rst
--rw-r--r--   0 kv         (501) staff       (20)      809 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/docs/make.bat
--rw-r--r--   0 kv         (501) staff       (20)       26 2023-03-11 07:30:59.000000 openthaigpt-0.0.9/docs/readme.rst
--rw-r--r--   0 kv         (501) staff       (20)       77 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/docs/usage.rst
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-03-19 14:16:40.700444 openthaigpt-0.0.9/openthaigpt/
--rw-r--r--   0 kv         (501) staff       (20)      199 2023-03-19 14:03:59.000000 openthaigpt-0.0.9/openthaigpt/__init__.py
--rw-r--r--   0 kv         (501) staff       (20)     1367 2023-03-19 14:16:33.000000 openthaigpt-0.0.9/openthaigpt/openthaigpt_module.py
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-03-19 14:16:40.701418 openthaigpt-0.0.9/openthaigpt.egg-info/
--rw-r--r--   0 kv         (501) staff       (20)     2926 2023-03-19 14:16:40.000000 openthaigpt-0.0.9/openthaigpt.egg-info/PKG-INFO
--rw-r--r--   0 kv         (501) staff       (20)      561 2023-03-19 14:16:40.000000 openthaigpt-0.0.9/openthaigpt.egg-info/SOURCES.txt
--rw-r--r--   0 kv         (501) staff       (20)        1 2023-03-19 14:16:40.000000 openthaigpt-0.0.9/openthaigpt.egg-info/dependency_links.txt
--rw-r--r--   0 kv         (501) staff       (20)        1 2023-02-28 01:42:10.000000 openthaigpt-0.0.9/openthaigpt.egg-info/not-zip-safe
--rw-r--r--   0 kv         (501) staff       (20)       43 2023-03-19 14:16:40.000000 openthaigpt-0.0.9/openthaigpt.egg-info/requires.txt
--rw-r--r--   0 kv         (501) staff       (20)       12 2023-03-19 14:16:40.000000 openthaigpt-0.0.9/openthaigpt.egg-info/top_level.txt
--rw-r--r--   0 kv         (501) staff       (20)      383 2023-03-19 14:16:40.702244 openthaigpt-0.0.9/setup.cfg
--rw-r--r--   0 kv         (501) staff       (20)     1749 2023-03-19 14:13:47.000000 openthaigpt-0.0.9/setup.py
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-03-19 14:16:40.701708 openthaigpt-0.0.9/tests/
--rw-r--r--   0 kv         (501) staff       (20)       41 2023-02-28 01:06:54.000000 openthaigpt-0.0.9/tests/__init__.py
--rw-r--r--   0 kv         (501) staff       (20)      526 2023-02-28 10:15:59.000000 openthaigpt-0.0.9/tests/test_openthaigpt.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069864 openthaigpt-0.1.0/
+-rw-r--r--   0 kv         (501) staff       (20)      130 2023-03-11 07:31:58.000000 openthaigpt-0.1.0/AUTHORS.md
+-rw-r--r--   0 kv         (501) staff       (20)     3406 2023-03-11 07:32:57.000000 openthaigpt-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 kv         (501) staff       (20)      428 2023-04-23 17:01:09.000000 openthaigpt-0.1.0/HISTORY.md
+-rw-r--r--   0 kv         (501) staff       (20)      595 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/LICENSE
+-rw-r--r--   0 kv         (501) staff       (20)      257 2023-03-11 07:31:36.000000 openthaigpt-0.1.0/MANIFEST.in
+-rw-r--r--   0 kv         (501) staff       (20)     3909 2023-04-23 17:03:39.069923 openthaigpt-0.1.0/PKG-INFO
+-rw-r--r--   0 kv         (501) staff       (20)     2360 2023-04-23 17:01:09.000000 openthaigpt-0.1.0/README.md
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.068089 openthaigpt-0.1.0/docs/
+-rw-r--r--   0 kv         (501) staff       (20)      612 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/Makefile
+-rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:31:16.000000 openthaigpt-0.1.0/docs/authors.rst
+-rwxr-xr-x   0 kv         (501) staff       (20)     4862 2023-03-11 07:31:10.000000 openthaigpt-0.1.0/docs/conf.py
+-rw-r--r--   0 kv         (501) staff       (20)       32 2023-03-11 07:31:04.000000 openthaigpt-0.1.0/docs/contributing.rst
+-rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:30:55.000000 openthaigpt-0.1.0/docs/history.rst
+-rw-r--r--   0 kv         (501) staff       (20)      308 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/index.rst
+-rw-r--r--   0 kv         (501) staff       (20)     1142 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/installation.rst
+-rw-r--r--   0 kv         (501) staff       (20)      809 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/make.bat
+-rw-r--r--   0 kv         (501) staff       (20)       26 2023-03-11 07:30:59.000000 openthaigpt-0.1.0/docs/readme.rst
+-rw-r--r--   0 kv         (501) staff       (20)       77 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/usage.rst
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.068448 openthaigpt-0.1.0/openthaigpt/
+-rw-r--r--   0 kv         (501) staff       (20)      199 2023-04-23 17:03:21.000000 openthaigpt-0.1.0/openthaigpt/__init__.py
+-rw-r--r--   0 kv         (501) staff       (20)     2540 2023-04-23 16:50:59.000000 openthaigpt-0.1.0/openthaigpt/openthaigpt_module.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069481 openthaigpt-0.1.0/openthaigpt.egg-info/
+-rw-r--r--   0 kv         (501) staff       (20)     3909 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/PKG-INFO
+-rw-r--r--   0 kv         (501) staff       (20)      561 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/SOURCES.txt
+-rw-r--r--   0 kv         (501) staff       (20)        1 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/dependency_links.txt
+-rw-r--r--   0 kv         (501) staff       (20)        1 2023-02-28 01:42:10.000000 openthaigpt-0.1.0/openthaigpt.egg-info/not-zip-safe
+-rw-r--r--   0 kv         (501) staff       (20)       56 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/requires.txt
+-rw-r--r--   0 kv         (501) staff       (20)       12 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/top_level.txt
+-rw-r--r--   0 kv         (501) staff       (20)      383 2023-04-23 17:03:39.070150 openthaigpt-0.1.0/setup.cfg
+-rw-r--r--   0 kv         (501) staff       (20)     1776 2023-04-23 17:03:11.000000 openthaigpt-0.1.0/setup.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069736 openthaigpt-0.1.0/tests/
+-rw-r--r--   0 kv         (501) staff       (20)       41 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/tests/__init__.py
+-rw-r--r--   0 kv         (501) staff       (20)      548 2023-04-23 17:03:01.000000 openthaigpt-0.1.0/tests/test_openthaigpt.py
```

### Comparing `openthaigpt-0.0.9/CONTRIBUTING.md` & `openthaigpt-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/LICENSE` & `openthaigpt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/PKG-INFO` & `openthaigpt-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-Metadata-Version: 2.1
-Name: openthaigpt
-Version: 0.0.9
-Summary: OpenThaiGPT focuses on developing a Thai Chatbot system to have capabilities equivalent to ChatGPT, as well as being able to connect to external systems and be able to retrieve data flexibly. Easily expandable and customizable and developed into Free open source software for everyone.
-Home-page: https://github.com/OpenThaiGPT/openthaigpt
-Author: Kobkrit Viriyayudhakorn
-Author-email: kobkrit@iapp.co.th
-License: Apache Software License 2.0
-Keywords: openthaigpt
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Natural Language :: Thai
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # OpenThaiGPT
 
 [![](https://img.shields.io/pypi/v/openthaigpt.svg)](https://pypi.python.org/pypi/openthaigpt) [![](https://pyup.io/repos/github/OpenThaiGPT/openthaigpt/shield.svg)](https://pyup.io/repos/github/OpenThaiGPT/openthaigpt/)
 
 OpenThaiGPT focuses on developing a Thai Chatbot system to have capabilities equivalent to ChatGPT, as well as being able to connect to external systems and be able to retrieve data flexibly. Easily expandable and customizable and developed into Free open source software for everyone.
 
 * Free software: Apache Software License 2.0
 * Project Homepage: https://openthaigpt.aieat.or.th
 * Documentation: https://openthaigpt.readthedocs.io.
 
 ## Features
 
-* The Fourth PoC Model for OpenThaiGPT 0.0.4
+* You can now select the model_name as follows:
+* kobkrit/openthaigpt-0.1.0-alpha
+* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4
+* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.3
+* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.2
+* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.1
 
 ## Installation
 Python>=3.6
 
 ### CPU-Only
 ``$ pip install openthaigpt torch --extra-index-url https://download.pytorch.org/whl/cpu``
 
@@ -54,28 +35,26 @@
 ```
 import openthaigpt
 
 print(openthaigpt.generate("Q: อยากลดความอ้วนทำไง\n\nA:"))
 print(openthaigpt.zero("การลดน้ำหนักเป็นเรื่องที่ต้องพิจารณาอย่างละเอียดและรอบคอบเพื่อให้ได้ผลลัพธ์ที่ดีและมีประสิทธิภาพมากที่สุด"))
 ```
 
-# History
-
-0.0.9 (2023-03-19)
-
-* Release OpenThaiGPT Zero
-
-0.0.8 (2023-03-12)
-
-* Update Readme
-
-0.0.7 (2023-03-12)
-
-* Update Model to Version 0.0.4 (https://huggingface.co/kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4)
-
-0.0.6 (2023-03-05)
-
-* Update README
+## Using 0.1.0-alpha model
+```
+import openthaigpt
 
-0.0.5 (2023-02-28)
+print(openthaigpt.generate(instruction="แปลภาษาอังกฤษเป็นภาษาไทย", input="We want to reduce weight.", model_name = "kobkrit/openthaigpt-0.1.0-alpha", min_length=50, max_length=300,  top_k=20, num_beams=5, no_repeat_ngram_size=20, temperature=1, early_stopping=True))
+```
 
-* First release on PyPI.
+## Collaboration By
+* Artificial Intelligence Entrepreneur Association of Thailand (AIEAT)
+* Artificial Intelligence Association of Thailand (AIAT)
+
+## Supported By
+* NECTEC
+* iApp Technology
+* Pantip
+* NVIDIA
+* Microsoft
+* Mahidol University
+* Gitbook
```

### Comparing `openthaigpt-0.0.9/docs/Makefile` & `openthaigpt-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/docs/conf.py` & `openthaigpt-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/docs/installation.rst` & `openthaigpt-0.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/docs/make.bat` & `openthaigpt-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/openthaigpt.egg-info/SOURCES.txt` & `openthaigpt-0.1.0/openthaigpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.0.9/setup.py` & `openthaigpt-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 with open('HISTORY.md') as history_file:
     history = history_file.read()
 
 requirements = [
     'transformers[sentencepiece]',
     'torch',
-    'evaluate'
+    'evaluate',
+    'loralib',
+    'peft'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Kobkrit Viriyayudhakorn",
     author_email='kobkrit@iapp.co.th',
@@ -42,10 +44,10 @@
     include_package_data=True,
     keywords='openthaigpt',
     name='openthaigpt',
     packages=find_packages(include=['openthaigpt', 'openthaigpt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/OpenThaiGPT/openthaigpt',
-    version='0.0.9',
+    version='0.1.0',
     zip_safe=False,
 )
```

### Comparing `openthaigpt-0.0.9/tests/test_openthaigpt.py` & `openthaigpt-0.1.0/tests/test_openthaigpt.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 
     def tearDown(self):
         """Tear down test fixtures, if any."""
 
     def test_0000_usage(self):
         """Test something."""
         answer = openthaigpt_module.generate("Q: สวัสดีครับ")
+        print(answer)
         assert answer is not None
```

