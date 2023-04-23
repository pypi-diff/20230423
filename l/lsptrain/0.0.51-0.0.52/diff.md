# Comparing `tmp/lsptrain-0.0.51.tar.gz` & `tmp/lsptrain-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.51.tar", last modified: Sun Apr 23 10:25:29 2023, max compression
+gzip compressed data, was "lsptrain-0.0.52.tar", last modified: Sun Apr 23 10:29:14 2023, max compression
```

## Comparing `lsptrain-0.0.51.tar` & `lsptrain-0.0.52.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.037510 lsptrain-0.0.51/
--rw-rw-rw-   0        0        0      492 2023-04-23 10:25:29.037510 lsptrain-0.0.51/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.51/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.017510 lsptrain-0.0.51/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.51/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.027510 lsptrain-0.0.51/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.51/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.51/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.51/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.031510 lsptrain-0.0.51/lsptrain/nlp_classification_server/
--rw-rw-rw-   0        0        0       82 2023-04-23 08:34:51.000000 lsptrain-0.0.51/lsptrain/nlp_classification_server/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-04-23 09:53:04.000000 lsptrain-0.0.51/lsptrain/nlp_classification_server/fastapi_server.py
--rw-rw-rw-   0        0        0     4743 2023-04-23 10:25:13.000000 lsptrain-0.0.51/lsptrain/nlp_classification_server/predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.036510 lsptrain-0.0.51/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.51/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.51/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.51/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:25:29.023510 lsptrain-0.0.51/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      492 2023-04-23 10:25:28.000000 lsptrain-0.0.51/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-23 10:25:28.000000 lsptrain-0.0.51/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:25:28.000000 lsptrain-0.0.51/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-23 10:25:28.000000 lsptrain-0.0.51/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 10:25:28.000000 lsptrain-0.0.51/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:25:29.038510 lsptrain-0.0.51/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-04-23 10:25:13.000000 lsptrain-0.0.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.181724 lsptrain-0.0.52/
+-rw-rw-rw-   0        0        0      492 2023-04-23 10:29:14.180725 lsptrain-0.0.52/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.52/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.160724 lsptrain-0.0.52/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.52/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.170725 lsptrain-0.0.52/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.52/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.52/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.52/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.174725 lsptrain-0.0.52/lsptrain/nlp_classification_server/
+-rw-rw-rw-   0        0        0       82 2023-04-23 08:34:51.000000 lsptrain-0.0.52/lsptrain/nlp_classification_server/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-04-23 09:53:04.000000 lsptrain-0.0.52/lsptrain/nlp_classification_server/fastapi_server.py
+-rw-rw-rw-   0        0        0     4744 2023-04-23 10:29:09.000000 lsptrain-0.0.52/lsptrain/nlp_classification_server/predictor.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.179725 lsptrain-0.0.52/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.52/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.52/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.52/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:29:14.167724 lsptrain-0.0.52/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      492 2023-04-23 10:29:14.000000 lsptrain-0.0.52/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-23 10:29:14.000000 lsptrain-0.0.52/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:29:14.000000 lsptrain-0.0.52/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-23 10:29:14.000000 lsptrain-0.0.52/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 10:29:14.000000 lsptrain-0.0.52/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:29:14.181724 lsptrain-0.0.52/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-23 10:29:09.000000 lsptrain-0.0.52/setup.py
```

### Comparing `lsptrain-0.0.51/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.52/lsptrain/nlp_classification/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.51/lsptrain/nlp_classification/train_scripts.py` & `lsptrain-0.0.52/lsptrain/nlp_classification/train_scripts.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.51/lsptrain/nlp_classification_server/fastapi_server.py` & `lsptrain-0.0.52/lsptrain/nlp_classification_server/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.51/lsptrain/nlp_classification_server/predictor.py` & `lsptrain-0.0.52/lsptrain/nlp_classification_server/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def __init__(self, label_file_name: str, save_dir: str = "checkpoint",
                  pretrained_model: str = "hfl/chinese-roberta-wwm-ext", device: str = "cuda:0",
                  model_file_name: str = "model_best.pt", max_length: int = 64
                  ):
         # init info labels
         self.info_labels = []
         with open(file=os.path.join(save_dir, label_file_name), mode="r", encoding="utf-8") as f:
-            lines = f.readline()
+            lines = f.readlines()
         self.info_labels = [x.strip() for x in lines if len(x.strip()) > 0]
 
         self.model = Model(pretrained_model=pretrained_model, info_labels=self.info_labels)
         self.model.load_state_dict(
             torch.load(os.path.join(save_dir, model_file_name), map_location=lambda storage, loc: storage)
         )
         self.device = "cpu"
```

### Comparing `lsptrain-0.0.51/lsptrain.egg-info/SOURCES.txt` & `lsptrain-0.0.52/lsptrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.51/setup.py` & `lsptrain-0.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.51',
+      version='0.0.52',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

