# Comparing `tmp/featurizerai-1.4.3.tar.gz` & `tmp/featurizerai-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.3.tar", last modified: Sat Apr 22 22:42:41 2023, max compression
+gzip compressed data, was "featurizerai-1.4.4.tar", last modified: Sun Apr 23 00:11:27 2023, max compression
```

## Comparing `featurizerai-1.4.3.tar` & `featurizerai-1.4.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518757 featurizerai-1.4.3/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.3/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.3/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-22 22:42:41.518821 featurizerai-1.4.3/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.3/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 22:42:41.519193 featurizerai-1.4.3/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-22 22:41:27.000000 featurizerai-1.4.3/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.516549 featurizerai-1.4.3/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518009 featurizerai-1.4.3/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.3/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     3010 2023-04-22 21:36:06.000000 featurizerai-1.4.3/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4533 2023-04-22 22:30:15.000000 featurizerai-1.4.3/src/features/materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      941 2023-04-22 21:36:37.000000 featurizerai-1.4.3/src/features/test_create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      822 2023-04-22 22:30:00.000000 featurizerai-1.4.3/src/features/test_materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518650 featurizerai-1.4.3/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      403 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028838 featurizerai-1.4.4/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.4/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.4/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 00:11:27.028907 featurizerai-1.4.4/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.4/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-23 00:11:27.029128 featurizerai-1.4.4/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-23 00:07:53.000000 featurizerai-1.4.4/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.025307 featurizerai-1.4.4/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028097 featurizerai-1.4.4/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.4/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.4/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4098 2023-04-23 00:08:33.000000 featurizerai-1.4.4/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5603 2023-04-23 00:09:21.000000 featurizerai-1.4.4/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      222 2023-04-22 23:38:13.000000 featurizerai-1.4.4/src/features/test_authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1086 2023-04-23 00:07:09.000000 featurizerai-1.4.4/src/features/test_create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      971 2023-04-23 00:10:38.000000 featurizerai-1.4.4/src/features/test_materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028711 featurizerai-1.4.4/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      466 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.3/LICENSE` & `featurizerai-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.3/PKG-INFO` & `featurizerai-1.4.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.3/setup.py` & `featurizerai-1.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.3',
+    version='1.4.4',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.3/src/features/create_stream.py` & `featurizerai-1.4.4/src/features/create_stream.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 import ast
 import logging
 from datetime import datetime
+from http.client import HTTPException
+
 from pymongo import MongoClient
 from pymongo.server_api import ServerApi
 from confluent_kafka import Consumer, KafkaError
 import certifi
 import os
 import threading
+import jwt
 
 class create_stream:
     def __init__(self, kafka_connection, mongo_connection=None, topicname=""):
         self.topicname = topicname
         self.kafka_connection = kafka_connection
         self.mongo_connection = mongo_connection or {
             'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
@@ -26,15 +29,15 @@
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
-    def _run(self):
+    def _run(self, token):
         mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
         raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
 
         consumer = Consumer(self.kafka_connection)
         print(self.topicname)
         consumer.subscribe([self.topicname])
@@ -54,18 +57,42 @@
                     else:
                         message_value["timestamp"] = datetime.now().timestamp()
 
                     raw_data_collection.insert_one(message_value)
                     print("Message received: {}".format(message_value))
         consumer.close()
 
-    def start(self):
+    def start(self, token):
+        # authenicate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print(user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+
         if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
             self._stop_event.clear()
-            self._consumer_thread = threading.Thread(target=self._run)
+            self._consumer_thread = threading.Thread(target=self._run(self))
             self._consumer_thread.start()
             print('featurizerai: Started consumer thread.')
         else:
             print("Thread is already running. Cannot start it again.")
 
     def stop(self):
         if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
```

### Comparing `featurizerai-1.4.3/src/features/materialize.py` & `featurizerai-1.4.4/src/features/materialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import json
 import logging
 from datetime import datetime, timedelta
+
+import jwt
 from pymongo import MongoClient
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import col, count
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 from pyspark.sql import functions as F
 from pyspark.sql.window import Window
 import certifi
 from pymongo.server_api import ServerApi
 
 class materialize:
-    def __init__(self, mongo_connection, aggregation_date, device_id, hours, days):
+    def __init__(self, mongo_connection, aggregation_date, device_id, hours, days, token):
         self.mongo_connection = mongo_connection
         self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
         self.device_id = device_id
+        self.token = token
         self.hours = hours
         self.days = days
         self.schema = StructType([
             StructField("timestamp", IntegerType(), True),
             StructField("name", StringType(), True),
             StructField("email", StringType(), True),
             StructField("deviceid", IntegerType(), True)
@@ -26,14 +29,39 @@
 
         self.spark = SparkSession.builder \
             .appName("IncrementalAggregation") \
             .master("local[*]") \
             .getOrCreate()
 
     def read_data_and_aggregate(self, raw_data_collection):
+
+        # authenicate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(self.token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print(user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+
         mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
         aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
 
         raw_data = raw_data_collection.find()
         raw_data_list = [doc for doc in raw_data]
         df = self.spark.createDataFrame(raw_data_list, self.schema)
```

### Comparing `featurizerai-1.4.3/src/features/test_create_stream.py` & `featurizerai-1.4.4/src/features/test_create_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         'collection': 'sparkaggregate'
     }
 
     # Create a new instance of the create_stream class
     featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5")
 
     # Start the Kafka consumer in a separate thread
-    featurizerai.start()
+    jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIyMDkyNjR9.L8hxyGgyx0ksnRuYnyB-OvXmgjNn4ONixd2lvvUS_8Y"
+    featurizerai.start(jwt)
 
     # Run the consumer for 30 seconds
     time.sleep(5)
 
     # Stop the consumer and wait for the thread to finish
     featurizerai.stop()
```

### Comparing `featurizerai-1.4.3/src/features/test_materialize.py` & `featurizerai-1.4.4/src/features/test_materialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     'rawdata': 'rawdata',
     'collection': 'sparkaggregate'
 }
 
 mongo_client = MongoClient(mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
 
 aggregation_date = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-device_id = 56
+device_id = 84
 hours = []
-days = [1, 5, 7, 10, 15]
+days = [15, 45, 90, 180, 365]
 
-m = materialize(mongo_connection, aggregation_date, device_id, hours, days)
+jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIyMDkyNjR9.L8hxyGgyx0ksnRuYnyB-OvXmgjNn4ONixd2lvvUS_8Y"
+
+m = materialize(mongo_connection, aggregation_date, device_id, hours, days, jwt)
 raw_data_collection = mongo_client[mongo_connection['database']][mongo_connection['rawdata']]
 m.read_data_and_aggregate(raw_data_collection)
```

### Comparing `featurizerai-1.4.3/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.4/src/featurizerai.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

