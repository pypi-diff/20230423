# Comparing `tmp/Timeseries-Preprocess-0.0.0.tar.gz` & `tmp/Timeseries-Preprocess-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Timeseries-Preprocess-0.0.0.tar", last modified: Sun Apr 23 15:35:15 2023, max compression
+gzip compressed data, was "Timeseries-Preprocess-0.0.1.tar", last modified: Sun Apr 23 15:47:29 2023, max compression
```

## Comparing `Timeseries-Preprocess-0.0.0.tar` & `Timeseries-Preprocess-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:35:15.768760 Timeseries-Preprocess-0.0.0/
--rw-r--r--   0 ruiwan     (501) staff       (20)      342 2023-04-23 15:35:15.768575 Timeseries-Preprocess-0.0.0/PKG-INFO
--rw-r--r--   0 ruiwan     (501) staff       (20)       24 2023-04-23 12:25:00.000000 Timeseries-Preprocess-0.0.0/README.md
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:35:15.768074 Timeseries-Preprocess-0.0.0/Timeseries_Preprocess.egg-info/
--rw-r--r--   0 ruiwan     (501) staff       (20)      342 2023-04-23 15:35:15.000000 Timeseries-Preprocess-0.0.0/Timeseries_Preprocess.egg-info/PKG-INFO
--rw-r--r--   0 ruiwan     (501) staff       (20)      232 2023-04-23 15:35:15.000000 Timeseries-Preprocess-0.0.0/Timeseries_Preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)        1 2023-04-23 15:35:15.000000 Timeseries-Preprocess-0.0.0/Timeseries_Preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)       22 2023-04-23 15:35:15.000000 Timeseries-Preprocess-0.0.0/Timeseries_Preprocess.egg-info/top_level.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)       38 2023-04-23 15:35:15.768822 Timeseries-Preprocess-0.0.0/setup.cfg
--rw-r--r--   0 ruiwan     (501) staff       (20)      501 2023-04-23 15:33:28.000000 Timeseries-Preprocess-0.0.0/setup.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:35:15.768204 Timeseries-Preprocess-0.0.0/timeseries_preprocess/
--rw-r--r--   0 ruiwan     (501) staff       (20)      152 2023-04-23 15:33:16.000000 Timeseries-Preprocess-0.0.0/timeseries_preprocess/__init__.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:47:29.399252 Timeseries-Preprocess-0.0.1/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      342 2023-04-23 15:47:29.399093 Timeseries-Preprocess-0.0.1/PKG-INFO
+-rw-r--r--   0 ruiwan     (501) staff       (20)       24 2023-04-23 12:25:00.000000 Timeseries-Preprocess-0.0.1/README.md
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:47:29.397825 Timeseries-Preprocess-0.0.1/Timeseries_Preprocess.egg-info/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      342 2023-04-23 15:47:29.000000 Timeseries-Preprocess-0.0.1/Timeseries_Preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 ruiwan     (501) staff       (20)      397 2023-04-23 15:47:29.000000 Timeseries-Preprocess-0.0.1/Timeseries_Preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)        1 2023-04-23 15:47:29.000000 Timeseries-Preprocess-0.0.1/Timeseries_Preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)       22 2023-04-23 15:47:29.000000 Timeseries-Preprocess-0.0.1/Timeseries_Preprocess.egg-info/top_level.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)       38 2023-04-23 15:47:29.399311 Timeseries-Preprocess-0.0.1/setup.cfg
+-rw-r--r--   0 ruiwan     (501) staff       (20)      506 2023-04-23 15:46:32.000000 Timeseries-Preprocess-0.0.1/setup.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:47:29.397967 Timeseries-Preprocess-0.0.1/timeseries_preprocess/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      152 2023-04-23 15:46:28.000000 Timeseries-Preprocess-0.0.1/timeseries_preprocess/__init__.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-04-23 15:47:29.398754 Timeseries-Preprocess-0.0.1/timeseries_preprocess/imputation/
+-rw-r--r--   0 ruiwan     (501) staff       (20)       78 2023-04-23 15:01:58.000000 Timeseries-Preprocess-0.0.1/timeseries_preprocess/imputation/__init__.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      547 2023-04-23 15:08:25.000000 Timeseries-Preprocess-0.0.1/timeseries_preprocess/imputation/multivariable_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      539 2023-04-23 15:01:52.000000 Timeseries-Preprocess-0.0.1/timeseries_preprocess/imputation/univariable_imputation.py
```

