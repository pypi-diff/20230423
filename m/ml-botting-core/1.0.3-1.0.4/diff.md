# Comparing `tmp/ml_botting_core-1.0.3.tar.gz` & `tmp/ml_botting_core-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.3.tar", last modified: Sat Apr 22 00:54:35 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.4.tar", last modified: Sun Apr 23 02:05:08 2023, max compression
```

## Comparing `ml_botting_core-1.0.3.tar` & `ml_botting_core-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.609975 ml_botting_core-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.136195 ml_botting_core-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 02:05:08.000000 ml_botting_core-1.0.4/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-23 02:05:08.000000 ml_botting_core-1.0.4/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:05:08.000000 ml_botting_core-1.0.4/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 02:05:08.000000 ml_botting_core-1.0.4/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:05:08.140195 ml_botting_core-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 02:03:51.000000 ml_botting_core-1.0.4/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.3/LICENSE` & `ml_botting_core-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.3/PKG-INFO` & `ml_botting_core-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 1.0.3
+Version: 1.0.4
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,16 @@
 │   │   ├── image_3.png  
 │   ├── in_hanger  
 │   │   ├── image_1.png  
 │   │   ├── image_2.png  
 │   │   ├── image_3.png  
   
 # Usage:
+Check out the samples [Here](https://github.com/darkmatter2222/ml_botting_core/tree/main/samples).  
+
 ### ml_botting_core_config.json
 ```json
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
```

### Comparing `ml_botting_core-1.0.3/README.md` & `ml_botting_core-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 │   │   ├── image_3.png  
 │   ├── in_hanger  
 │   │   ├── image_1.png  
 │   │   ├── image_2.png  
 │   │   ├── image_3.png  
   
 # Usage:
+Check out the samples [Here](https://github.com/darkmatter2222/ml_botting_core/tree/main/samples).  
+
 ### ml_botting_core_config.json
 ```json
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
```

### Comparing `ml_botting_core-1.0.3/setup.cfg` & `ml_botting_core-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.3
+version = 1.0.4
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core/base.py` & `ml_botting_core-1.0.4/src/ml_botting_core/base.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.4/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import pathlib
 
 from PIL import Image, ImageDraw
 
 from tensorflow.keras import layers
 from tensorflow.keras.models import Sequential
 from sklearn.metrics import confusion_matrix
+from sklearn.utils.class_weight import compute_class_weight
 
 def build_and_train(root_image_directory, model_location,
                     model_name, epochs=10,
-                    resize_ratio=0.2):
+                    resize_ratio=0.2, auto_balance_data=True):
     data_dir = pathlib.Path(root_image_directory)
 
     image_list = list(data_dir.glob('*/*.png'))
     image_count = len(image_list)
     print(image_count)
 
     img = Image.open(image_list[0])
@@ -36,15 +37,27 @@
         validation_split=0.2,
         subset="validation",
         seed=123,
         image_size=(img_height, img_width),
         batch_size=batch_size)
 
     class_names = train_ds.class_names
-    print(class_names)
+    print(f"Class Names: {class_names}")
+
+    class_weights = None
+    if auto_balance_data:
+        y_train = np.concatenate([y for x, y in train_ds], axis=0)
+
+        class_weights = compute_class_weight(class_weight="balanced", classes=np.unique(y_train), y=y_train)
+        class_weights = {i: w for i, w in enumerate(class_weights)}
+
+        print(f"Class Weights: {class_weights}")
+
+
+
 
     AUTOTUNE = tf.data.AUTOTUNE
 
     train_ds = train_ds.cache().shuffle(1000).prefetch(buffer_size=AUTOTUNE)
     val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)
 
     num_classes = len(class_names)
@@ -66,15 +79,16 @@
     model.compile(optimizer='adam',
                   loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
                   metrics=['accuracy'])
 
     history = model.fit(
         train_ds,
         validation_data=val_ds,
-        epochs=epochs
+        epochs=epochs,
+        class_weight=class_weights
     )
     train_data = list(train_ds)
     features = np.concatenate([train_data[n][0] for n in range(0, len(train_data))])
     targets = np.concatenate([train_data[n][1] for n in range(0, len(train_data))])
     print(targets)
     predictions = model.predict(features)
     print(predictions.argmax(1))
```

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.4/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.4/src/ml_botting_core/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core/prediction/prediction.py` & `ml_botting_core-1.0.4/src/ml_botting_core/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-1.0.4/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 1.0.3
+Version: 1.0.4
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,16 @@
 │   │   ├── image_3.png  
 │   ├── in_hanger  
 │   │   ├── image_1.png  
 │   │   ├── image_2.png  
 │   │   ├── image_3.png  
   
 # Usage:
+Check out the samples [Here](https://github.com/darkmatter2222/ml_botting_core/tree/main/samples).  
+
 ### ml_botting_core_config.json
 ```json
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
```

### Comparing `ml_botting_core-1.0.3/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.4/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

