# Comparing `tmp/xjm-0.0.4.tar.gz` & `tmp/xjm-0.0.5.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xjm-0.0.4.tar", last modified: Sun Apr 23 08:17:48 2023, max compression
+gzip compressed data, was "/home/xjm/xjm/xjm_pycharm/xjm/dist/xjm-0.0.5.linux-x86_64.tar", last modified: Sun Apr 23 08:51:54 2023, max compression
```

## Comparing `xjm-0.0.4.tar` & `xjm-0.0.5.linux-x86_64.tar`

### file list

```diff
@@ -1,31 +1,54 @@
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/visualization/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     2445 2022-03-24 02:44:22.000000 xjm-0.0.4/visualization/heatmap.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:43.000000 xjm-0.0.4/visualization/__init__.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     4159 2023-01-05 01:16:29.000000 xjm-0.0.4/visualization/aug_image.py
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/data_augmentation/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     2566 2022-03-04 14:02:07.000000 xjm-0.0.4/data_augmentation/pic_aug.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:54.000000 xjm-0.0.4/data_augmentation/__init__.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)       38 2023-04-23 08:17:48.000000 xjm-0.0.4/setup.cfg
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/model/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     2515 2023-04-05 13:49:52.000000 xjm-0.0.4/model/model_init.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:36.000000 xjm-0.0.4/model/__init__.py
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/xjm.egg-info/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)      534 2023-04-23 08:17:48.000000 xjm-0.0.4/xjm.egg-info/SOURCES.txt
--rw-rw-r--   0 xjm       (1000) xjm       (1000)      258 2023-04-23 08:17:48.000000 xjm-0.0.4/xjm.egg-info/PKG-INFO
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        1 2023-04-23 08:17:48.000000 xjm-0.0.4/xjm.egg-info/dependency_links.txt
--rw-rw-r--   0 xjm       (1000) xjm       (1000)       59 2023-04-23 08:17:48.000000 xjm-0.0.4/xjm.egg-info/top_level.txt
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/logger/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)      757 2022-07-11 13:28:33.000000 xjm-0.0.4/logger/log_sample.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:27.000000 xjm-0.0.4/logger/__init__.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     2201 2023-03-09 08:53:14.000000 xjm-0.0.4/logger/cuda_monitor.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     1029 2022-07-12 03:13:45.000000 xjm-0.0.4/logger/set_logger.py
-drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:17:48.000000 xjm-0.0.4/data_processe/
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     4340 2023-04-22 08:29:35.000000 xjm-0.0.4/data_processe/pachong.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     1985 2023-03-17 17:27:58.000000 xjm-0.0.4/data_processe/pachong_google.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:13.000000 xjm-0.0.4/data_processe/__init__.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     4300 2023-04-18 03:26:12.000000 xjm-0.0.4/data_processe/compute_mean.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)     2009 2023-04-16 13:50:26.000000 xjm-0.0.4/data_processe/divide_train_test.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)      509 2023-04-23 08:17:32.000000 xjm-0.0.4/setup.py
--rw-rw-r--   0 xjm       (1000) xjm       (1000)      258 2023-04-23 08:17:48.000000 xjm-0.0.4/PKG-INFO
--rw-rw-r--   0 xjm       (1000) xjm       (1000)       51 2023-03-06 15:35:48.000000 xjm-0.0.4/README.txt
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2445 2022-03-24 02:44:22.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/heatmap.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/__pycache__/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      156 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1745 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/__pycache__/heatmap.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2311 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/__pycache__/aug_image.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:43.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/__init__.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     4159 2023-01-05 01:16:29.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/aug_image.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/__pycache__/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      160 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1112 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/__pycache__/pic_aug.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2566 2022-03-04 14:02:07.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/pic_aug.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/__init__.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      534 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/SOURCES.txt
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      258 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/PKG-INFO
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        1 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/dependency_links.txt
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)       59 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/top_level.txt
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2515 2023-04-05 13:49:52.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/model_init.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/__pycache__/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      148 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2365 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/__pycache__/model_init.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:36.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/model/__init__.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      757 2022-07-11 13:28:33.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/log_sample.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__pycache__/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      149 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      873 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__pycache__/set_logger.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1827 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__pycache__/cuda_monitor.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      881 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__pycache__/log_sample.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:27.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/__init__.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2201 2023-03-09 08:53:14.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/cuda_monitor.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1029 2022-07-12 03:13:45.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/logger/set_logger.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     4340 2023-04-22 08:29:35.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/pachong.py
+drwxrwxr-x   0 xjm       (1000) xjm       (1000)        0 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      156 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1872 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/pachong_google.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1775 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/pachong.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2305 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/compute_mean.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)      847 2023-04-23 08:51:54.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__pycache__/divide_train_test.cpython-36.pyc
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     1985 2023-03-17 17:27:58.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/pachong_google.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)        0 2023-04-22 08:48:13.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/__init__.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     4300 2023-04-18 03:26:12.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/compute_mean.py
+-rw-rw-r--   0 xjm       (1000) xjm       (1000)     2009 2023-04-16 13:50:26.000000 ./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/divide_train_test.py
```

### Comparing `xjm-0.0.4/visualization/heatmap.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/heatmap.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/visualization/aug_image.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/visualization/aug_image.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/data_augmentation/pic_aug.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/data_augmentation/pic_aug.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/model/model_init.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/model/model_init.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/xjm.egg-info/SOURCES.txt` & `./home/xjm/anaconda3/lib/python3.6/site-packages/xjm-0.0.5-py3.6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/logger/log_sample.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/logger/log_sample.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/logger/cuda_monitor.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/logger/cuda_monitor.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/logger/set_logger.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/logger/set_logger.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/data_processe/pachong.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/pachong.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/data_processe/pachong_google.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/pachong_google.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/data_processe/compute_mean.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/compute_mean.py`

 * *Files identical despite different names*

### Comparing `xjm-0.0.4/data_processe/divide_train_test.py` & `./home/xjm/anaconda3/lib/python3.6/site-packages/data_processe/divide_train_test.py`

 * *Files identical despite different names*

