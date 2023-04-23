# Comparing `tmp/zerocs-0.5.tar.gz` & `tmp/zerocs-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocs-0.5.tar", last modified: Sat Apr 22 03:23:29 2023, max compression
+gzip compressed data, was "zerocs-0.6.tar", last modified: Sun Apr 23 12:40:56 2023, max compression
```

## Comparing `zerocs-0.5.tar` & `zerocs-0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 03:23:29.649029 zerocs-0.5/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-22 03:23:29.649029 zerocs-0.5/setup.cfg
--rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-22 03:23:03.000000 zerocs-0.5/setup.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.645029 zerocs-0.5/zerocs/
--rw-r--r--   0 yanping   (1000) yanping   (1000)     4785 2023-04-22 02:58:49.000000 zerocs-0.5/zerocs/__init__.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.645029 zerocs-0.5/zerocs/base/
--rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/base/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/base/_base.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-20 05:50:35.000000 zerocs-0.5/zerocs/base/_default_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/base/_function.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/base/base_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/base/default_func_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/base/function_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.645029 zerocs-0.5/zerocs/fork/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/fork/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-0.5/zerocs/fork/_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/fork/fork_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/logger/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/logger/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/logger/_logger.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/logger/logger_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-20 03:18:43.000000 zerocs-0.5/zerocs/mate.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/network/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/network/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/network/_network.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/network/network_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/rabbitmq/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/rabbitmq/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/rabbitmq/_rabbitmq.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/rabbitmq/rabbitmq_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/script/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/script/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/script/_queue.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/script/queue_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/snowflakeId/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/snowflakeId/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/snowflakeId/_snowflakeId.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-0.5/zerocs/snowflakeId/snowflakeId.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.649029 zerocs-0.5/zerocs/sqlite/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/sqlite/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-0.5/zerocs/sqlite/_sqlite.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-0.5/zerocs/sqlite/sqlite3_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     8662 2023-04-20 05:52:13.000000 zerocs-0.5/zerocs/zerocs_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 03:23:29.645029 zerocs-0.5/zerocs.egg-info/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 03:23:29.000000 zerocs-0.5/zerocs.egg-info/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-22 03:23:29.000000 zerocs-0.5/zerocs.egg-info/SOURCES.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-22 03:23:29.000000 zerocs-0.5/zerocs.egg-info/dependency_links.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-22 03:23:29.000000 zerocs-0.5/zerocs.egg-info/requires.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-22 03:23:29.000000 zerocs-0.5/zerocs.egg-info/top_level.txt
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.490149 zerocs-0.6/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18120 2023-04-23 12:40:56.490149 zerocs-0.6/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-23 12:40:56.490149 zerocs-0.6/setup.cfg
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-23 12:40:55.000000 zerocs-0.6/setup.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     4785 2023-04-22 02:58:49.000000 zerocs-0.6/zerocs/__init__.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/base/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/base/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/base/_base.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-20 05:50:35.000000 zerocs-0.6/zerocs/base/_default_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/base/_function.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/base/base_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/base/default_func_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/base/function_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/fork/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/fork/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-0.6/zerocs/fork/_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/fork/fork_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/logger/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/logger/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/logger/_logger.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/logger/logger_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-20 03:18:43.000000 zerocs-0.6/zerocs/mate.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/network/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/network/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/network/_network.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/network/network_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/rabbitmq/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/rabbitmq/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/rabbitmq/_rabbitmq.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/rabbitmq/rabbitmq_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs/script/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/script/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/script/_queue.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/script/queue_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.490149 zerocs-0.6/zerocs/snowflakeId/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/snowflakeId/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/snowflakeId/_snowflakeId.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-0.6/zerocs/snowflakeId/snowflakeId.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.490149 zerocs-0.6/zerocs/sqlite/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/sqlite/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-0.6/zerocs/sqlite/_sqlite.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-0.6/zerocs/sqlite/sqlite3_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    11297 2023-04-23 12:08:29.000000 zerocs-0.6/zerocs/zerocs_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-23 12:40:56.486149 zerocs-0.6/zerocs.egg-info/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18120 2023-04-23 12:40:56.000000 zerocs-0.6/zerocs.egg-info/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-23 12:40:56.000000 zerocs-0.6/zerocs.egg-info/SOURCES.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-23 12:40:56.000000 zerocs-0.6/zerocs.egg-info/dependency_links.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-23 12:40:56.000000 zerocs-0.6/zerocs.egg-info/requires.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-23 12:40:56.000000 zerocs-0.6/zerocs.egg-info/top_level.txt
```

### Comparing `zerocs-0.5/PKG-INFO` & `zerocs-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.5
+Version: 0.6
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
@@ -32,28 +32,37 @@
 
     3. It is divided into Master node and Slave node.
     The Master node is a management node and can only have one.
     set up ZERO_FW_NODE_MASTER=True/False ，Change node type
 
 2. start using
 
-    1. To use the framework, it is very simple, just refer to zerocs
+    1. Please install RabbitMQ before use,
+    rabbitmq official website : https://www.rabbitmq.com,
+    It is recommended to use Docker installation during testing::
+
+            docker run -d --hostname my-rabbit --name rabbit \
+            -e RABBITMQ_DEFAULT_USER=user \
+            -e RABBITMQ_DEFAULT_PASS=password \
+            -p 15672:15672 -p 5672:5672 rabbitmq:management
+
+    2. To use the framework, it is very simple, just refer to zerocs
     in the first line of your startup script
     Please create the corresponding directory and files before starting::
 
           ├─zerocs_files //Temporary file directory
           ├─zerocs_logs //log directory
           ├─zerocs_service //Directory of microservice codes
           │  │─t_service //A folder with the same name as the microservice name
           │  │  ├─t_service.py //Microservice startup file with the same name as the service name
           ├─zerocs_demo_master.py  //Master node startup script
           └─zerocs_demo_slave.py //Slave node startup script
           └─zerocs_test.py //Test Script
 
-    2. zerocs_demo_master.py ::
+    3. zerocs_demo_master.py ::
 
         # Master startup file, please refer to zerocs first
         # Flask API is not mandatory and can be connected to other management systems
 
         from zerocs import Service
         import os
         from flask import Flask, request
@@ -201,15 +210,15 @@
                 RABBITMQ_CONFIG='amqp://admin:Rabbit*ads12@192.168.100.2',
                 RABBITMQ_CONFIG_URL='http://127.0.0.1/get_config',
                 ZERO_FW_DB_FILE="test.db",
                 ZERO_FW_NODE_MASTER="True"
             )
             app.run(host='0.0.0.0', port=5002)
 
-    3. zerocs_demo_slave.py ::
+    4. zerocs_demo_slave.py ::
 
         # Slave startup file, please refer to zerocs first
 
         from zerocs import Service
         import os
 
         OS_PATH = os.path.dirname(os.path.abspath(__file__))
@@ -229,15 +238,15 @@
                 RABBITMQ_PORT='5672',
                 RABBITMQ_CONFIG='amqp://admin:Rabbit*ads12@192.168.100.2',
                 RABBITMQ_CONFIG_URL='http://127.0.0.1/get_config',
                 ZERO_FW_DB_FILE="test.db",
                 ZERO_FW_NODE_MASTER="False"
             )
 
-    4. t_service.py ::
+    5. t_service.py ::
 
         import time
         from nameko.rpc import rpc
 
 
         class RpcFunction:
             """
@@ -272,15 +281,15 @@
                 which can be subdivided in the work code to complete all types of
                 tasks using one service, but it is not recommended to do so
                 """
                 print(service, config, task_data, '--work')
                 time.sleep(25)
                 print(service, config, task_data, '--end')
 
-    5. zerocs_test.py ::
+    6. zerocs_test.py ::
 
         import json
         import os
         import requests
         from nameko.standalone.rpc import ClusterRpcProxy
 
         OS_PATH = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `zerocs-0.5/setup.py` & `zerocs-0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zerocs',
-    version='0.5',
+    version='0.6',
     description="zerocs",
     long_description=open('zerocs/README.rst').read(),
     # long_description_content_type='text/plain',
     include_package_data=True,
     author='YanPing',
     author_email='zyphhxx@foxmail.com',
     maintainer='YanPing',
```

### Comparing `zerocs-0.5/zerocs/__init__.py` & `zerocs-0.6/zerocs/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/base/_base.py` & `zerocs-0.6/zerocs/base/_base.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/base/_default_func.py` & `zerocs-0.6/zerocs/base/_default_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/base/base_.py` & `zerocs-0.6/zerocs/base/base_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/base/default_func_.py` & `zerocs-0.6/zerocs/base/default_func_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/base/function_.py` & `zerocs-0.6/zerocs/base/function_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/fork/_func.py` & `zerocs-0.6/zerocs/fork/_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/fork/fork_.py` & `zerocs-0.6/zerocs/fork/fork_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/logger/_logger.py` & `zerocs-0.6/zerocs/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/mate.py` & `zerocs-0.6/zerocs/mate.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/rabbitmq/_rabbitmq.py` & `zerocs-0.6/zerocs/rabbitmq/_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/rabbitmq/rabbitmq_.py` & `zerocs-0.6/zerocs/rabbitmq/rabbitmq_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/script/_queue.py` & `zerocs-0.6/zerocs/script/_queue.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/script/queue_.py` & `zerocs-0.6/zerocs/script/queue_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/snowflakeId/_snowflakeId.py` & `zerocs-0.6/zerocs/snowflakeId/_snowflakeId.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/sqlite/_sqlite.py` & `zerocs-0.6/zerocs/sqlite/_sqlite.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs/sqlite/sqlite3_.py` & `zerocs-0.6/zerocs/sqlite/sqlite3_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.5/zerocs.egg-info/PKG-INFO` & `zerocs-0.6/zerocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.5
+Version: 0.6
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
@@ -32,28 +32,37 @@
 
     3. It is divided into Master node and Slave node.
     The Master node is a management node and can only have one.
     set up ZERO_FW_NODE_MASTER=True/False ，Change node type
 
 2. start using
 
-    1. To use the framework, it is very simple, just refer to zerocs
+    1. Please install RabbitMQ before use,
+    rabbitmq official website : https://www.rabbitmq.com,
+    It is recommended to use Docker installation during testing::
+
+            docker run -d --hostname my-rabbit --name rabbit \
+            -e RABBITMQ_DEFAULT_USER=user \
+            -e RABBITMQ_DEFAULT_PASS=password \
+            -p 15672:15672 -p 5672:5672 rabbitmq:management
+
+    2. To use the framework, it is very simple, just refer to zerocs
     in the first line of your startup script
     Please create the corresponding directory and files before starting::
 
           ├─zerocs_files //Temporary file directory
           ├─zerocs_logs //log directory
           ├─zerocs_service //Directory of microservice codes
           │  │─t_service //A folder with the same name as the microservice name
           │  │  ├─t_service.py //Microservice startup file with the same name as the service name
           ├─zerocs_demo_master.py  //Master node startup script
           └─zerocs_demo_slave.py //Slave node startup script
           └─zerocs_test.py //Test Script
 
-    2. zerocs_demo_master.py ::
+    3. zerocs_demo_master.py ::
 
         # Master startup file, please refer to zerocs first
         # Flask API is not mandatory and can be connected to other management systems
 
         from zerocs import Service
         import os
         from flask import Flask, request
@@ -201,15 +210,15 @@
                 RABBITMQ_CONFIG='amqp://admin:Rabbit*ads12@192.168.100.2',
                 RABBITMQ_CONFIG_URL='http://127.0.0.1/get_config',
                 ZERO_FW_DB_FILE="test.db",
                 ZERO_FW_NODE_MASTER="True"
             )
             app.run(host='0.0.0.0', port=5002)
 
-    3. zerocs_demo_slave.py ::
+    4. zerocs_demo_slave.py ::
 
         # Slave startup file, please refer to zerocs first
 
         from zerocs import Service
         import os
 
         OS_PATH = os.path.dirname(os.path.abspath(__file__))
@@ -229,15 +238,15 @@
                 RABBITMQ_PORT='5672',
                 RABBITMQ_CONFIG='amqp://admin:Rabbit*ads12@192.168.100.2',
                 RABBITMQ_CONFIG_URL='http://127.0.0.1/get_config',
                 ZERO_FW_DB_FILE="test.db",
                 ZERO_FW_NODE_MASTER="False"
             )
 
-    4. t_service.py ::
+    5. t_service.py ::
 
         import time
         from nameko.rpc import rpc
 
 
         class RpcFunction:
             """
@@ -272,15 +281,15 @@
                 which can be subdivided in the work code to complete all types of
                 tasks using one service, but it is not recommended to do so
                 """
                 print(service, config, task_data, '--work')
                 time.sleep(25)
                 print(service, config, task_data, '--end')
 
-    5. zerocs_test.py ::
+    6. zerocs_test.py ::
 
         import json
         import os
         import requests
         from nameko.standalone.rpc import ClusterRpcProxy
 
         OS_PATH = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `zerocs-0.5/zerocs.egg-info/SOURCES.txt` & `zerocs-0.6/zerocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

