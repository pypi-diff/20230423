# Comparing `tmp/unwanted_content_detector-0.1.6.tar.gz` & `tmp/unwanted_content_detector-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unwanted_content_detector-0.1.6.tar", max compression
+gzip compressed data, was "unwanted_content_detector-0.1.7.tar", max compression
```

## Comparing `unwanted_content_detector-0.1.6.tar` & `unwanted_content_detector-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      903 2023-04-22 20:53:13.777547 unwanted_content_detector-0.1.6/README.md
--rw-r--r--   0        0        0      639 2023-04-22 21:49:00.494816 unwanted_content_detector-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.6/unwanted_content_detector/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.6/unwanted_content_detector/data/__init__.py
--rw-r--r--   0        0        0    11051 2023-04-22 20:59:25.756725 unwanted_content_detector-0.1.6/unwanted_content_detector/data/data.csv
--rw-r--r--   0        0        0      674 2023-04-22 21:45:30.175899 unwanted_content_detector-0.1.6/unwanted_content_detector/data/data_loader.py
--rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.6/unwanted_content_detector/data/generative_prompts.txt
--rw-r--r--   0        0        0      498 2023-04-22 21:44:07.359639 unwanted_content_detector-0.1.6/unwanted_content_detector/detector.py
--rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.6/unwanted_content_detector/entities.py
--rw-r--r--   0        0        0     1350 2023-04-22 21:45:45.686191 unwanted_content_detector-0.1.6/unwanted_content_detector/evaluator/evaluator.py
--rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.6/unwanted_content_detector/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.6/unwanted_content_detector/models/distilbert_finetuned/__init__.py
--rw-r--r--   0        0        0     1017 2023-04-22 21:44:35.878588 unwanted_content_detector-0.1.6/unwanted_content_detector/models/distilbert_finetuned/inference.py
--rw-r--r--   0        0        0     3844 2023-04-22 21:45:56.970345 unwanted_content_detector-0.1.6/unwanted_content_detector/models/distilbert_finetuned/train.py
--rw-r--r--   0        0        0      964 2023-04-22 21:44:35.881414 unwanted_content_detector-0.1.6/unwanted_content_detector/models/upload.py
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      928 2023-04-22 22:35:19.139135 unwanted_content_detector-0.1.7/README.md
+-rw-r--r--   0        0        0      639 2023-04-22 22:33:34.904828 unwanted_content_detector-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.7/unwanted_content_detector/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.7/unwanted_content_detector/data/__init__.py
+-rw-r--r--   0        0        0    11051 2023-04-22 20:59:25.756725 unwanted_content_detector-0.1.7/unwanted_content_detector/data/data.csv
+-rw-r--r--   0        0        0      936 2023-04-22 22:29:01.290289 unwanted_content_detector-0.1.7/unwanted_content_detector/data/data_loader.py
+-rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.7/unwanted_content_detector/data/generative_prompts.txt
+-rw-r--r--   0        0        0      498 2023-04-22 21:44:07.359639 unwanted_content_detector-0.1.7/unwanted_content_detector/detector.py
+-rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.7/unwanted_content_detector/entities.py
+-rw-r--r--   0        0        0     1350 2023-04-22 21:45:45.686191 unwanted_content_detector-0.1.7/unwanted_content_detector/evaluator/evaluator.py
+-rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.7/unwanted_content_detector/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/__init__.py
+-rw-r--r--   0        0        0     1017 2023-04-22 21:44:35.878588 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/inference.py
+-rw-r--r--   0        0        0     3844 2023-04-22 21:45:56.970345 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/train.py
+-rw-r--r--   0        0        0     1047 2023-04-22 22:26:56.548900 unwanted_content_detector-0.1.7/unwanted_content_detector/models/upload.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.7/PKG-INFO
```

### Comparing `unwanted_content_detector-0.1.6/README.md` & `unwanted_content_detector-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -23,22 +23,21 @@
     "We should all do our part to protect the environment.",
     'Everyone has the right to love who they want.'
 ]})
 
 df['is_unwanted'] = df['text'].apply(lambda x: detector.is_unwanted(x))
 ```
 
-In the terminal:
+To get a view of the complete options type in the terminal:
 
 ```sh
 unwanted_detector 
 ```
 
 
-To get the manual
 
 ## Models
 
 | Model name            | size (mb) 
 |-----------------------|-----------
 | distilbert-finetuned | 300 mb
```

### Comparing `unwanted_content_detector-0.1.6/pyproject.toml` & `unwanted_content_detector-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unwanted-content-detector"
-version = "0.1.6"
+version = "0.1.7"
 description = "A library to detect undesired, unbranded, or harmful content"
 authors = ["Jean Carlo Machado <jean.machado@getyourguide.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "unwanted_content_detector"}]
 
 [tool.poetry.dependencies]
```

### Comparing `unwanted_content_detector-0.1.6/unwanted_content_detector/data/data.csv` & `unwanted_content_detector-0.1.7/unwanted_content_detector/data/data.csv`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.6/unwanted_content_detector/evaluator/evaluator.py` & `unwanted_content_detector-0.1.7/unwanted_content_detector/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.6/unwanted_content_detector/models/distilbert_finetuned/inference.py` & `unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/inference.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.6/unwanted_content_detector/models/distilbert_finetuned/train.py` & `unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/train.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.6/unwanted_content_detector/models/upload.py` & `unwanted_content_detector-0.1.7/unwanted_content_detector/models/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     import pathlib
     current_dir =  str(pathlib.Path(__file__).resolve().parent)
 
     return current_dir + "/../../detector_distilbert_01"
 
 def upload_model():
     from huggingface_hub import HfApi
+    from datetime import datetime;
+    print("Uploading model to HuggingFace Hub")
 
     api = HfApi()
     api.upload_folder(
         folder_path=model_directory(),
         repo_id = REPO_ID,
     )
```

### Comparing `unwanted_content_detector-0.1.6/PKG-INFO` & `unwanted_content_detector-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unwanted-content-detector
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to detect undesired, unbranded, or harmful content
 License: Apache
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -42,22 +42,21 @@
     "We should all do our part to protect the environment.",
     'Everyone has the right to love who they want.'
 ]})
 
 df['is_unwanted'] = df['text'].apply(lambda x: detector.is_unwanted(x))
 ```
 
-In the terminal:
+To get a view of the complete options type in the terminal:
 
 ```sh
 unwanted_detector 
 ```
 
 
-To get the manual
 
 ## Models
 
 | Model name            | size (mb) 
 |-----------------------|-----------
 | distilbert-finetuned | 300 mb
```

