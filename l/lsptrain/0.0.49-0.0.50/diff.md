# Comparing `tmp/lsptrain-0.0.49.tar.gz` & `tmp/lsptrain-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.49.tar", last modified: Fri Apr 21 05:48:57 2023, max compression
+gzip compressed data, was "lsptrain-0.0.50.tar", last modified: Sun Apr 23 10:11:01 2023, max compression
```

## Comparing `lsptrain-0.0.49.tar` & `lsptrain-0.0.50.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.222717 lsptrain-0.0.49/
--rw-rw-rw-   0        0        0      492 2023-04-21 05:48:57.221716 lsptrain-0.0.49/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.49/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.209715 lsptrain-0.0.49/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.49/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.216717 lsptrain-0.0.49/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6974 2023-04-21 05:48:54.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/model.py
--rw-rw-rw-   0        0        0     1603 2023-04-21 05:47:19.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.220716 lsptrain-0.0.49/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.49/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2418 2023-04-21 05:40:42.000000 lsptrain-0.0.49/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.49/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.214717 lsptrain-0.0.49/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      492 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 05:48:57.222717 lsptrain-0.0.49/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-21 05:48:54.000000 lsptrain-0.0.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.766748 lsptrain-0.0.50/
+-rw-rw-rw-   0        0        0      492 2023-04-23 10:11:01.766748 lsptrain-0.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.50/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.747748 lsptrain-0.0.50/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.50/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.756748 lsptrain-0.0.50/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.50/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.50/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.50/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.760748 lsptrain-0.0.50/lsptrain/nlp_classification_server/
+-rw-rw-rw-   0        0        0       82 2023-04-23 08:34:51.000000 lsptrain-0.0.50/lsptrain/nlp_classification_server/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-04-23 09:53:04.000000 lsptrain-0.0.50/lsptrain/nlp_classification_server/fastapi_server.py
+-rw-rw-rw-   0        0        0     4721 2023-04-23 09:55:42.000000 lsptrain-0.0.50/lsptrain/nlp_classification_server/predictor.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.765747 lsptrain-0.0.50/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.50/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.50/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.50/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:11:01.752748 lsptrain-0.0.50/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      492 2023-04-23 10:11:01.000000 lsptrain-0.0.50/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-23 10:11:01.000000 lsptrain-0.0.50/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:11:01.000000 lsptrain-0.0.50/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-23 10:11:01.000000 lsptrain-0.0.50/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 10:11:01.000000 lsptrain-0.0.50/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:11:01.766748 lsptrain-0.0.50/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-23 10:10:56.000000 lsptrain-0.0.50/setup.py
```

### Comparing `lsptrain-0.0.49/setup.py` & `lsptrain-0.0.50/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.49',
+      version='0.0.50',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
-      install_requires=['torch>=1.11.0',
-                        'transformers>=4.20.1',
-                        'scikit-learn>=1.1.0',
+      install_requires=['torch',
+                        'transformers',
+                        'scikit-learn',
                         'tqdm'],
       python_requires='>=3.7',
       license='BSD License',
       packages=find_packages(),
       platforms=['all'],
       include_package_data=True
       )
```

