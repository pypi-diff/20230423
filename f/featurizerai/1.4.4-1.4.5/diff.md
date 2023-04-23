# Comparing `tmp/featurizerai-1.4.4.tar.gz` & `tmp/featurizerai-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.4.tar", last modified: Sun Apr 23 00:11:27 2023, max compression
+gzip compressed data, was "featurizerai-1.4.5.tar", last modified: Sun Apr 23 14:46:38 2023, max compression
```

## Comparing `featurizerai-1.4.4.tar` & `featurizerai-1.4.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028838 featurizerai-1.4.4/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.4/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.4/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 00:11:27.028907 featurizerai-1.4.4/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.4/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-23 00:11:27.029128 featurizerai-1.4.4/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-23 00:07:53.000000 featurizerai-1.4.4/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.025307 featurizerai-1.4.4/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028097 featurizerai-1.4.4/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.4/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.4/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4098 2023-04-23 00:08:33.000000 featurizerai-1.4.4/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5603 2023-04-23 00:09:21.000000 featurizerai-1.4.4/src/features/materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      222 2023-04-22 23:38:13.000000 featurizerai-1.4.4/src/features/test_authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1086 2023-04-23 00:07:09.000000 featurizerai-1.4.4/src/features/test_create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      971 2023-04-23 00:10:38.000000 featurizerai-1.4.4/src/features/test_materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 00:11:27.028711 featurizerai-1.4.4/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      466 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-23 00:11:26.000000 featurizerai-1.4.4/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.832386 featurizerai-1.4.5/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.5/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.5/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 14:46:38.832450 featurizerai-1.4.5/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.5/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-23 14:46:38.832660 featurizerai-1.4.5/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-23 14:46:29.000000 featurizerai-1.4.5/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.829067 featurizerai-1.4.5/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.831570 featurizerai-1.4.5/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.5/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.5/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.5/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.5/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4128 2023-04-23 14:39:35.000000 featurizerai-1.4.5/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      222 2023-04-23 00:14:52.000000 featurizerai-1.4.5/src/features/test_authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1100 2023-04-23 11:25:26.000000 featurizerai-1.4.5/src/features/test_create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2627 2023-04-23 14:45:41.000000 featurizerai-1.4.5/src/features/test_materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.832275 featurizerai-1.4.5/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      496 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.4/LICENSE` & `featurizerai-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.4/PKG-INFO` & `featurizerai-1.4.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.4/setup.py` & `featurizerai-1.4.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.4',
+    version='1.4.5',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.4/src/features/authenticate.py` & `featurizerai-1.4.5/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.4/src/features/create_stream.py` & `featurizerai-1.4.5/src/features/create_stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,21 @@
 from confluent_kafka import Consumer, KafkaError
 import certifi
 import os
 import threading
 import jwt
 
 class create_stream:
-    def __init__(self, kafka_connection, mongo_connection=None, topicname=""):
+    def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
         self.topicname = topicname
         self.kafka_connection = kafka_connection
-        self.mongo_connection = mongo_connection or {
-            'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
-            'database': 'kafkastream',
-            'rawcollection': 'rawdata',
-            'collection': 'sparkaggregate'
-        }
+        self.mongo_connection = mongo_connection
+        self.timestamp_attr = timestamp_attr
         self._stop_event = threading.Event()
 
-    os.environ['HADOOP_OPTS'] = f"{os.environ.get('HADOOP_OPTS', '')} -Djava.library.path=/Library/hadoop/lib/native"
-
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
@@ -39,30 +33,39 @@
         raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
 
         consumer = Consumer(self.kafka_connection)
         print(self.topicname)
         consumer.subscribe([self.topicname])
 
         while not self._stop_event.is_set():
-            msg = consumer.poll(1.0)
-
+            msg = consumer.poll(10.0)
+            print("Poll executed")
+            print(msg)
             if msg is None:
                 continue
             if msg.error():
                 print("Consumer error: {}".format(msg.error()))
             else:
                 message_value = ast.literal_eval(msg.value().decode("utf-8"))
-                if self.is_epoch(message_value.get("timestamp")):
-                    if self.is_epoch(message_value.get("timestamp")):
-                        message_value["timestamp"] = int(message_value["timestamp"])
+                print(message_value)
+
+                # New lines added for validation
+                if self.timestamp_attr not in message_value:
+                    print(
+                        f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
+                    continue
+
+                if self.is_epoch(message_value.get(self.timestamp_attr)):
+                    if self.is_epoch(message_value.get(self.timestamp_attr)):
+                        message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
                     else:
-                        message_value["timestamp"] = datetime.now().timestamp()
+                        message_value[self.timestamp_attr] = datetime.now().timestamp()
 
-                    raw_data_collection.insert_one(message_value)
-                    print("Message received: {}".format(message_value))
+                raw_data_collection.insert_one(message_value)
+                print("Message received: {}".format(message_value))
         consumer.close()
 
     def start(self, token):
         # authenicate token
         mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
         mongo_db_featurizer = mongo_client['featurizer']
```

### Comparing `featurizerai-1.4.4/src/features/test_create_stream.py` & `featurizerai-1.4.5/src/features/test_create_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,21 @@
         'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
         'database': 'kafkastream',
         'rawcollection': 'rawdata',
         'collection': 'sparkaggregate'
     }
 
     # Create a new instance of the create_stream class
-    featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5")
+    featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5", "timestamp")
 
     # Start the Kafka consumer in a separate thread
-    jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIyMDkyNjR9.L8hxyGgyx0ksnRuYnyB-OvXmgjNn4ONixd2lvvUS_8Y"
+    jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIyNTE0MDB9.keOhdMFQhFwNp5VLHW4UrGHsRrglt7HIdOyJ7p9DdLg"
     featurizerai.start(jwt)
 
-    # Run the consumer for 30 seconds
-    time.sleep(5)
+    # Run the consumer for 60 seconds
+    time.sleep(60)
 
     # Stop the consumer and wait for the thread to finish
     featurizerai.stop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `featurizerai-1.4.4/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.5/src/featurizerai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

