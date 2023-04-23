# Comparing `tmp/imbrium-1.2.0.tar.gz` & `tmp/imbrium-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbrium-1.2.0.tar", last modified: Tue Apr 11 21:05:07 2023, max compression
+gzip compressed data, was "imbrium-1.3.0.tar", last modified: Sun Apr 23 00:39:43 2023, max compression
```

## Comparing `imbrium-1.2.0.tar` & `imbrium-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.321368 imbrium-1.2.0/
--rw-rw-rw-   0        0        0     1732 2023-03-26 19:06:20.000000 imbrium-1.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    48846 2023-04-11 21:05:07.321368 imbrium-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    48093 2023-04-11 20:47:03.000000 imbrium-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.164635 imbrium-1.2.0/imbrium/
--rw-rw-rw-   0        0        0       91 2023-03-12 18:31:01.000000 imbrium-1.2.0/imbrium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.211564 imbrium-1.2.0/imbrium/architectures/
--rw-rw-rw-   0        0        0       44 2022-10-31 01:25:26.000000 imbrium-1.2.0/imbrium/architectures/__init__.py
--rw-rw-rw-   0        0        0    36327 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/architectures/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.227151 imbrium-1.2.0/imbrium/blueprints/
--rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-1.2.0/imbrium/blueprints/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-02-18 02:25:36.000000 imbrium-1.2.0/imbrium/blueprints/abstract_multivariate.py
--rw-rw-rw-   0        0        0     1702 2023-02-18 02:25:36.000000 imbrium-1.2.0/imbrium/blueprints/abstract_univariate.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.274491 imbrium-1.2.0/imbrium/predictors/
--rw-rw-rw-   0        0        0      296 2023-02-26 18:46:56.000000 imbrium-1.2.0/imbrium/predictors/__init__.py
--rw-rw-rw-   0        0        0    26529 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/multivarhybrid.py
--rw-rw-rw-   0        0        0    44845 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/multivarpure.py
--rw-rw-rw-   0        0        0    25879 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/univarhybrid.py
--rw-rw-rw-   0        0        0    44457 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/univarpure.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.305818 imbrium-1.2.0/imbrium/utils/
--rw-rw-rw-   0        0        0      129 2023-02-21 00:14:08.000000 imbrium-1.2.0/imbrium/utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-02-21 00:14:08.000000 imbrium-1.2.0/imbrium/utils/optimization.py
--rw-rw-rw-   0        0        0      426 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/utils/scaler.py
--rw-rw-rw-   0        0        0    10584 2023-01-09 01:24:32.000000 imbrium-1.2.0/imbrium/utils/transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.195940 imbrium-1.2.0/imbrium.egg-info/
--rw-rw-rw-   0        0        0    48846 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:05:07.321368 imbrium-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-03-12 18:30:22.000000 imbrium-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.178804 imbrium-1.3.0/
+-rw-rw-rw-   0        0        0     1942 2023-04-21 22:48:49.000000 imbrium-1.3.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    58424 2023-04-23 00:39:43.178804 imbrium-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    57671 2023-04-22 23:52:00.000000 imbrium-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:42.974774 imbrium-1.3.0/imbrium/
+-rw-rw-rw-   0        0        0       91 2023-04-15 00:42:37.000000 imbrium-1.3.0/imbrium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.021667 imbrium-1.3.0/imbrium/architectures/
+-rw-rw-rw-   0        0        0       44 2022-10-31 01:25:26.000000 imbrium-1.3.0/imbrium/architectures/__init__.py
+-rw-rw-rw-   0        0        0    61240 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/architectures/models.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.052934 imbrium-1.3.0/imbrium/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-1.3.0/imbrium/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-02-18 02:25:36.000000 imbrium-1.3.0/imbrium/blueprints/abstract_multivariate.py
+-rw-rw-rw-   0        0        0     1702 2023-02-18 02:25:36.000000 imbrium-1.3.0/imbrium/blueprints/abstract_univariate.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.100280 imbrium-1.3.0/imbrium/predictors/
+-rw-rw-rw-   0        0        0      296 2023-02-26 18:46:56.000000 imbrium-1.3.0/imbrium/predictors/__init__.py
+-rw-rw-rw-   0        0        0    31296 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/predictors/multivarhybrid.py
+-rw-rw-rw-   0        0        0    53344 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/predictors/multivarpure.py
+-rw-rw-rw-   0        0        0    30646 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/predictors/univarhybrid.py
+-rw-rw-rw-   0        0        0    52913 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/predictors/univarpure.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.147146 imbrium-1.3.0/imbrium/utils/
+-rw-rw-rw-   0        0        0      180 2023-04-17 22:16:55.000000 imbrium-1.3.0/imbrium/utils/__init__.py
+-rw-rw-rw-   0        0        0     1879 2023-04-21 22:56:36.000000 imbrium-1.3.0/imbrium/utils/optimization.py
+-rw-rw-rw-   0        0        0      742 2023-04-19 19:15:36.000000 imbrium-1.3.0/imbrium/utils/optimizer.py
+-rw-rw-rw-   0        0        0      426 2023-04-23 00:00:25.000000 imbrium-1.3.0/imbrium/utils/scaler.py
+-rw-rw-rw-   0        0        0    10584 2023-01-09 01:24:32.000000 imbrium-1.3.0/imbrium/utils/transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:39:43.006045 imbrium-1.3.0/imbrium.egg-info/
+-rw-rw-rw-   0        0        0    58424 2023-04-23 00:39:42.000000 imbrium-1.3.0/imbrium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-04-23 00:39:42.000000 imbrium-1.3.0/imbrium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 00:39:42.000000 imbrium-1.3.0/imbrium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-04-23 00:39:42.000000 imbrium-1.3.0/imbrium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 00:39:42.000000 imbrium-1.3.0/imbrium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 00:39:43.178804 imbrium-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-04-15 00:48:30.000000 imbrium-1.3.0/setup.py
```

### Comparing `imbrium-1.2.0/CHANGELOG.md` & `imbrium-1.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -69,8 +69,15 @@
 - removed batch_size parameter from fit_model method
 - hyperparameter optimization added via the Optuna library
 
 
 ### 1.2.0
 
 - added Tensorboard support
-- changed show_performance plot to show loss and metric values
+- changed show_performance plot to show loss and metric values
+- added optional dropout and regularization layers to architectures
+
+### 1.3.0
+
+- added depth parameter to architectures
+- added optimizer configuration support
+- added optimizer configuration to seeker
```

### Comparing `imbrium-1.2.0/LICENSE` & `imbrium-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imbrium-1.2.0/imbrium/blueprints/abstract_multivariate.py` & `imbrium-1.3.0/imbrium/blueprints/abstract_multivariate.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.2.0/imbrium/blueprints/abstract_univariate.py` & `imbrium-1.3.0/imbrium/blueprints/abstract_univariate.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.2.0/imbrium/predictors/multivarhybrid.py` & `imbrium-1.3.0/imbrium/predictors/univarhybrid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import datetime
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
-from numpy import array, empty, reshape
+from numpy import array, reshape
 from pandas import DataFrame
 from tensorflow import keras
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
                                      Dropout, Flatten, MaxPooling1D, SimpleRNN,
                                      TimeDistributed)
 
 from imbrium.architectures.models import *
-from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
+from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
+from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.scaler import SCALER
-from imbrium.utils.transformer import data_prep_multi, multistep_prep_hybrid
+from imbrium.utils.transformer import data_prep_uni, sequence_prep_hybrid_uni
 
 
-class HybridMulti(MultiVariateMultiStep):
-    """Implements neural network based multivariate multipstep hybrid predictors.
+class HybridUni(UniVariateMultiStep):
+    """Implements neural network based univariate multipstep hybrid predictors.
 
     Methods
     -------
     set_model_id(self, name: str):
         Setter method to change model id name.
     get_model_id(self) -> array:
         Getter method to retrieve model id used.
@@ -90,48 +91,46 @@
 
     def __init__(
         self,
         sub_seq: int,
         steps_past: int,
         steps_future: int,
         data=DataFrame(),
-        features: list = [],
         scale: str = "",
     ) -> object:
         """
         Parameters:
-            sub_seq (int): Divide data into further subsequences.
+            sub_seq (int): Further division of given steps a predictor will
+            look backward.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
-            data (DataFrame): Input data for model training.
-            features (list): List of features. First feature in list will be
-            set to the target variable.
+            data (array): Input data for model training. Default is empty to
+            enable loading pre-trained models.
             scale (str): How to scale the data before making predictions.
         """
         self.sub_seq = sub_seq
         self.steps_past = steps_past
         self.steps_future = steps_future
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
         self.scaler = SCALER[scale]
 
-        self.model_id = ""
-        self.sub_seq = sub_seq
-
         if len(data) > 0:
-            self.data = data_prep_multi(data, features, self.scaler)
-            self.input_x, self.input_y, self.modified_back = multistep_prep_hybrid(
+            self.data = array(data)
+            self.data = data_prep_uni(data, self.scaler)
+            self.input_x, self.input_y, self.modified_back = sequence_prep_hybrid_uni(
                 self.data, sub_seq, steps_past, steps_future
             )
-
         else:
             self.data = data
 
+        self.model_id = ""
+
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
@@ -174,16 +173,21 @@
     def get_metrics(self) -> str:
         """Get metrics."""
         return self.metrics
 
     def create_cnnrnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        rnn_block_one=1,
+        rnn_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -196,32 +200,39 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnrnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnlstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        lstm_block_one=1,
+        lstm_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -234,32 +245,39 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnlstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnngru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        gru_block_one=1,
+        gru_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -272,32 +290,39 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnngru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbirnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        birnn_block_one=1,
+        rnn_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -310,32 +335,39 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbirnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        bilstm_block_one=1,
+        lstm_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -348,32 +380,39 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbilstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        bigru_block_one=1,
+        gru_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -386,24 +425,26 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbigru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
-            input_shape=(
-                self.input_x.shape[1],
-                self.input_x.shape[2],
-                self.input_x.shape[3],
-            ),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
@@ -412,15 +453,15 @@
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             validation_split (float): Determines size of Validation data.
-            board (bool): Creates TensorBoard.
+            board (bool): Create TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = tf.keras.callbacks.TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -524,14 +565,17 @@
     def predict(self, data: array) -> DataFrame:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (DataFrame): Forecast for sequence provided.
         """
+        data = array(data)
+        data = data.reshape(-1, 1)
+
         self.scaler.fit(data)
         data = self.scaler.transform(data)
 
         shape_ = int((data.shape[1] * self.steps_past) / self.sub_seq)
         data = data.reshape(1, self.sub_seq, shape_, 1)
 
         y_pred = self.model.predict(data, verbose=0)
@@ -551,20 +595,25 @@
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = keras.models.load_model(location)
 
 
-class OptimizeHybridMulti(HybridMulti):
+class OptimizeHybridUni(HybridUni):
     def create_fit_cnnrnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -573,32 +622,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -607,32 +666,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -641,32 +710,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -675,32 +754,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -709,32 +798,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -743,16 +842,21 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
```

### Comparing `imbrium-1.2.0/imbrium/predictors/multivarpure.py` & `imbrium-1.3.0/imbrium/predictors/multivarpure.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tensorflow import keras
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
                                      Dropout, Flatten, MaxPooling1D, SimpleRNN)
 
 from imbrium.architectures.models import *
 from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
+from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.scaler import SCALER
 from imbrium.utils.transformer import data_prep_multi, multistep_prep_standard
 
 
 class PureMulti(MultiVariateMultiStep):
     """Implements deep neural networks based on multivariate multipstep
     standard predictors.
@@ -192,16 +193,20 @@
     def get_metrics(self) -> str:
         """Get metrics."""
         return self.metrics
 
     def create_mlp(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        dense_block_one: int = 1,
+        dense_block_two: int = 1,
+        dense_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 50,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -222,38 +227,47 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("MLP")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         # necessary to account for hyperparameter optimization
         try:
             self.input_x = self.backup_input_x
         except:
             self.backup_input_x = self.input_x.copy()
 
         self.dimension = self.input_x.shape[1] * self.input_x.shape[2]
 
         self.input_x = self.input_x.reshape((self.input_x.shape[0], self.dimension))
 
         self.model = mlp(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            dense_block_one=dense_block_one,
+            dense_block_two=dense_block_two,
+            dense_block_three=dense_block_three,
             layer_config=layer_config,
             input_shape=self.input_x.shape[1],
             output_shape=self.input_y.shape[1],
         )
 
     def create_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
+        rnn_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -274,28 +288,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = rnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
+            rnn_block_three=rnn_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
+        lstm_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -316,28 +339,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = lstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
+            lstm_block_three=lstm_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        dense_block_one: int = 1,
         layer_config: dict = {
             "layer0": (
                 64,
                 1,
                 "relu",
                 0.0,
                 0.0,
@@ -361,28 +393,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            dense_block_one=dense_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
+        gru_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -403,28 +444,36 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = gru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
+            gru_block_three=gru_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_birnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },  # (neurons, activation, regularization, dropout)
     ):
         """Creates BI-RNN model.
         Parameters:
@@ -434,28 +483,35 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = birnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_bilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
     ):
         """Creates BI-LSTM model.
         Parameters:
@@ -465,28 +521,35 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = bilstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_bigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
     ):
         """Creates BI-GRU model.
         Parameters:
@@ -496,28 +559,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = bigru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_y.shape[1],
         )
 
     def create_encdec_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_rnn_block_one: int = 1,
+        enc_rnn_block_two: int = 1,
+        dec_rnn_block_one: int = 1,
+        dec_rnn_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -544,29 +616,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_rnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_rnn_block_one=enc_rnn_block_one,
+            enc_rnn_block_two=enc_rnn_block_two,
+            dec_rnn_block_one=dec_rnn_block_one,
+            dec_rnn_block_two=dec_rnn_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=1,
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_lstm_block_one: int = 1,
+        enc_lstm_block_two: int = 1,
+        dec_lstm_block_one: int = 1,
+        dec_lstm_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -593,29 +676,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_lstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_lstm_block_one=enc_lstm_block_one,
+            enc_lstm_block_two=enc_lstm_block_two,
+            dec_lstm_block_one=dec_lstm_block_one,
+            dec_lstm_block_two=dec_lstm_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=1,
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_gru_block_one: int = 1,
+        enc_gru_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (100, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0, 0.0),
             "layer2": (50, "relu", 0.0, 0.0),
             "layer3": (100, "relu", 0.0),
         },
     ):
@@ -627,29 +721,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_gru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_gru_block_one=enc_gru_block_one,
+            enc_gru_block_two=enc_gru_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=1,
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_conv_block_one: int = 1,
+        enc_conv_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (100, "relu", 0.0),
         },
@@ -663,18 +768,24 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder(CNN)-Decoder(GRU)")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_cnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_conv_block_one=enc_conv_block_one,
+            enc_conv_block_two=enc_conv_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=1,
             repeat=self.input_y.shape[1],
         )
 
     def fit_model(
@@ -834,16 +945,20 @@
         self.model = keras.models.load_model(location)
 
 
 class OptimizePureMulti(PureMulti):
     def create_fit_mlp(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        dense_block_one: int = 1,
+        dense_block_two: int = 1,
+        dense_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 50,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -860,32 +975,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            dense_block_one=dense_block_one,
+            dense_block_two=dense_block_two,
+            dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
+        rnn_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -902,32 +1025,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a RNN model."""
         self.create_rnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
+            rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
+        lstm_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -944,32 +1075,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
+            lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        dense_block_one: int = 1,
         layer_config: dict = {
             "layer0": (
                 64,
                 1,
                 "relu",
                 0.0,
                 0.0,
@@ -989,32 +1128,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a CNN model."""
         self.create_cnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
+        gru_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1031,125 +1178,152 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
+            gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },  # (neurons, activation, regularization, dropout)
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-RNN model."""
         self.create_birnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-LSTM model."""
         self.create_bilstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-GRU model."""
         self.create_bigru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_rnn_block_one: int = 1,
+        enc_rnn_block_two: int = 1,
+        dec_rnn_block_one: int = 1,
+        dec_rnn_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1172,32 +1346,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains an encoder-decoder RNN model."""
         self.create_encdec_rnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_rnn_block_one=enc_rnn_block_one,
+            enc_rnn_block_two=enc_rnn_block_two,
+            dec_rnn_block_one=dec_rnn_block_one,
+            dec_rnn_block_two=dec_rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_lstm_block_one: int = 1,
+        enc_lstm_block_two: int = 1,
+        dec_lstm_block_one: int = 1,
+        dec_lstm_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1220,32 +1404,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains an encoder-decoder LSTM model."""
         self.create_encdec_lstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_lstm_block_one=enc_lstm_block_one,
+            enc_lstm_block_two=enc_lstm_block_two,
+            dec_lstm_block_one=dec_lstm_block_one,
+            dec_lstm_block_two=dec_lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_gru_block_one: int = 1,
+        enc_gru_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (100, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0, 0.0),
             "layer2": (50, "relu", 0.0, 0.0),
             "layer3": (100, "relu", 0.0),
         },
         epochs: int = 100,
@@ -1253,32 +1447,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains an encoder-decoder GRU model."""
         self.create_encdec_gru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_gru_block_one=enc_gru_block_one,
+            enc_gru_block_two=enc_gru_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_conv_block_one: int = 1,
+        enc_conv_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (100, "relu", 0.0),
         },
@@ -1287,16 +1491,21 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains an encoder-decoder CNN model."""
         self.create_encdec_cnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_conv_block_one=enc_conv_block_one,
+            enc_conv_block_two=enc_conv_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
```

### Comparing `imbrium-1.2.0/imbrium/predictors/univarhybrid.py` & `imbrium-1.3.0/imbrium/predictors/multivarhybrid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import datetime
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
-from numpy import array, reshape
+from numpy import array, empty, reshape
 from pandas import DataFrame
 from tensorflow import keras
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
                                      Dropout, Flatten, MaxPooling1D, SimpleRNN,
                                      TimeDistributed)
 
 from imbrium.architectures.models import *
-from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
+from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
+from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.scaler import SCALER
-from imbrium.utils.transformer import data_prep_uni, sequence_prep_hybrid_uni
+from imbrium.utils.transformer import data_prep_multi, multistep_prep_hybrid
 
 
-class HybridUni(UniVariateMultiStep):
-    """Implements neural network based univariate multipstep hybrid predictors.
+class HybridMulti(MultiVariateMultiStep):
+    """Implements neural network based multivariate multipstep hybrid predictors.
 
     Methods
     -------
     set_model_id(self, name: str):
         Setter method to change model id name.
     get_model_id(self) -> array:
         Getter method to retrieve model id used.
@@ -90,46 +91,48 @@
 
     def __init__(
         self,
         sub_seq: int,
         steps_past: int,
         steps_future: int,
         data=DataFrame(),
+        features: list = [],
         scale: str = "",
     ) -> object:
         """
         Parameters:
-            sub_seq (int): Further division of given steps a predictor will
-            look backward.
+            sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
-            data (array): Input data for model training. Default is empty to
-            enable loading pre-trained models.
+            data (DataFrame): Input data for model training.
+            features (list): List of features. First feature in list will be
+            set to the target variable.
             scale (str): How to scale the data before making predictions.
         """
         self.sub_seq = sub_seq
         self.steps_past = steps_past
         self.steps_future = steps_future
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
         self.scaler = SCALER[scale]
 
+        self.model_id = ""
+        self.sub_seq = sub_seq
+
         if len(data) > 0:
-            self.data = array(data)
-            self.data = data_prep_uni(data, self.scaler)
-            self.input_x, self.input_y, self.modified_back = sequence_prep_hybrid_uni(
+            self.data = data_prep_multi(data, features, self.scaler)
+            self.input_x, self.input_y, self.modified_back = multistep_prep_hybrid(
                 self.data, sub_seq, steps_past, steps_future
             )
+
         else:
             self.data = data
 
-        self.model_id = ""
-
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
@@ -172,16 +175,21 @@
     def get_metrics(self) -> str:
         """Get metrics."""
         return self.metrics
 
     def create_cnnrnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        rnn_block_one=1,
+        rnn_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -194,28 +202,43 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnrnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnlstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        lstm_block_one=1,
+        lstm_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -228,28 +251,43 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnlstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnngru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        gru_block_one=1,
+        gru_block_two=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -262,28 +300,43 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnngru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbirnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        birnn_block_one=1,
+        rnn_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -296,28 +349,43 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbirnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        bilstm_block_one=1,
+        lstm_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -330,28 +398,43 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbilstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnnbigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one=1,
+        conv_block_two=1,
+        bigru_block_one=1,
+        gru_block_one=1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -364,20 +447,30 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN-BI-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnnbigru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(None, self.modified_back, 1),
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
+            layer_config=layer_config,
+            input_shape=(
+                self.input_x.shape[1],
+                self.input_x.shape[2],
+                self.input_x.shape[3],
+            ),
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
@@ -386,15 +479,15 @@
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             validation_split (float): Determines size of Validation data.
-            board (bool): Create TensorBoard.
+            board (bool): Creates TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = tf.keras.callbacks.TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -498,17 +591,14 @@
     def predict(self, data: array) -> DataFrame:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (DataFrame): Forecast for sequence provided.
         """
-        data = array(data)
-        data = data.reshape(-1, 1)
-
         self.scaler.fit(data)
         data = self.scaler.transform(data)
 
         shape_ = int((data.shape[1] * self.steps_past) / self.sub_seq)
         data = data.reshape(1, self.sub_seq, shape_, 1)
 
         y_pred = self.model.predict(data, verbose=0)
@@ -528,20 +618,25 @@
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = keras.models.load_model(location)
 
 
-class OptimizeHybridUni(HybridUni):
+class OptimizeHybridMulti(HybridMulti):
     def create_fit_cnnrnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -550,32 +645,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -584,32 +689,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -618,32 +733,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -652,32 +777,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -686,32 +821,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config={
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (25, "relu", 0.0),
         },
@@ -720,16 +865,21 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
```

### Comparing `imbrium-1.2.0/imbrium/predictors/univarpure.py` & `imbrium-1.3.0/imbrium/predictors/univarpure.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
 from numpy import array, empty, reshape
 from pandas import DataFrame
 from tensorflow import keras
+from tensorflow.keras import optimizers
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
                                      Dropout, Flatten, MaxPooling1D,
                                      RepeatVector, SimpleRNN, TimeDistributed)
 
 from imbrium.architectures.models import *
 from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
+from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.scaler import SCALER
 from imbrium.utils.transformer import data_prep_uni, sequence_prep_standard_uni
 
 
 class PureUni(UniVariateMultiStep):
     """Implements neural network based univariate multipstep predictors.
 
@@ -186,16 +188,20 @@
     def get_metrics(self) -> str:
         """Get metrics."""
         return self.metrics
 
     def create_mlp(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        dense_block_one: int = 1,
+        dense_block_two: int = 1,
+        dense_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 50,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -220,28 +226,37 @@
         self.loss = loss
         self.metrics = metrics
 
         self.input_x = self.input_x.reshape(
             (self.input_x.shape[0], self.input_x.shape[1])
         )
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = mlp(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            dense_block_one=dense_block_one,
+            dense_block_two=dense_block_two,
+            dense_block_three=dense_block_three,
             layer_config=layer_config,
             input_shape=self.input_x.shape[1],
             output_shape=self.input_y.shape[1],
         )
 
     def create_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
+        rnn_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -262,28 +277,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = rnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
+            rnn_block_three=rnn_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
+        lstm_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -304,28 +328,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = lstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
+            lstm_block_three=lstm_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        dense_block_one: int = 1,
         layer_config: dict = {
             "layer0": (
                 64,
                 1,
                 "relu",
                 0.0,
                 0.0,
@@ -349,28 +382,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("CNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = cnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            dense_block_one=dense_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
+        gru_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -391,28 +433,36 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = gru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
+            gru_block_three=gru_block_three,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_birnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },  # (neurons, activation, regularization, dropout)
     ):
         """Creates BI-RNN model.
         Parameters:
@@ -422,28 +472,35 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = birnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_bilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
     ):
         """Creates BI-LSTM model.
         Parameters:
@@ -453,28 +510,35 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = bilstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_bigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
     ):
         """Creates BI-GRU model.
         Parameters:
@@ -484,28 +548,37 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("BI-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = bigru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], 1),
             output_shape=self.input_y.shape[1],
         )
 
     def create_encdec_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_rnn_block_one: int = 1,
+        enc_rnn_block_two: int = 1,
+        dec_rnn_block_one: int = 1,
+        dec_rnn_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -532,29 +605,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_rnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
+            enc_rnn_block_one=enc_rnn_block_one,
+            enc_rnn_block_two=enc_rnn_block_two,
+            dec_rnn_block_one=dec_rnn_block_one,
+            dec_rnn_block_two=dec_rnn_block_two,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_x.shape[2],
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_lstm_block_one=1,
+        enc_lstm_block_two=1,
+        dec_lstm_block_one=1,
+        dec_lstm_block_two=1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -581,29 +665,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_lstm(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_lstm_block_one=enc_lstm_block_one,
+            enc_lstm_block_two=enc_lstm_block_two,
+            dec_lstm_block_one=dec_lstm_block_one,
+            dec_lstm_block_two=dec_lstm_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_x.shape[2],
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_gru_block_one=1,
+        enc_gru_block_two=1,
+        dec_gru_block_one=1,
+        dec_gru_block_two=1,
         layer_config: dict = {
             "layer0": (100, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0, 0.0),
             "layer2": (50, "relu", 0.0, 0.0),
             "layer3": (100, "relu", 0.0),
         },
     ):
@@ -615,29 +710,40 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder-Decoder-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_gru(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_gru_block_one=enc_gru_block_one,
+            enc_gru_block_two=enc_gru_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_x.shape[2],
             repeat=self.input_y.shape[1],
         )
 
     def create_encdec_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_conv_block_one=1,
+        enc_conv_block_two=1,
+        dec_gru_block_one=1,
+        dec_gru_block_two=1,
         layer_config: dict = {
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (100, "relu", 0.0),
         },
@@ -651,18 +757,24 @@
             layer_config (dict): Adjust neurons and acitivation functions.
         """
         self.set_model_id("Encoder(CNN)-Decoder(GRU)")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
+        optimizer_obj = get_optimizer(optimizer, optimizer_args)
+
         self.model = encdec_cnn(
-            optimizer=optimizer,
+            optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
+            enc_conv_block_one=enc_conv_block_one,
+            enc_conv_block_two=enc_conv_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
             input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
             output_shape=self.input_x.shape[2],
             repeat=self.input_y.shape[1],
         )
 
     def fit_model(
@@ -825,16 +937,20 @@
         self.model = keras.models.load_model(location)
 
 
 class OptimizePureUni(PureUni):
     def create_fit_mlp(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        dense_block_one: int = 1,
+        dense_block_two: int = 1,
+        dense_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 50,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -851,31 +967,39 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            dense_block_one=dense_block_one,
+            dense_block_two=dense_block_two,
+            dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
+        rnn_block_one: int = 1,
+        rnn_block_two: int = 1,
+        rnn_block_three: int = 1,
         metrics: str = "mean_squared_error",
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
@@ -893,32 +1017,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Recurrent Neural Network model."""
         self.create_rnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            rnn_block_one=rnn_block_one,
+            rnn_block_two=rnn_block_two,
+            rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        lstm_block_one: int = 1,
+        lstm_block_two: int = 1,
+        lstm_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -935,32 +1067,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            lstm_block_one=lstm_block_one,
+            lstm_block_two=lstm_block_two,
+            lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        conv_block_one: int = 1,
+        conv_block_two: int = 1,
+        dense_block_one: int = 1,
         layer_config: dict = {
             "layer0": (
                 64,
                 1,
                 "relu",
                 0.0,
                 0.0,
@@ -980,32 +1120,40 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Convolutional Neural Network model."""
         self.create_cnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            conv_block_one=conv_block_one,
+            conv_block_two=conv_block_two,
+            dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        gru_block_one: int = 1,
+        gru_block_two: int = 1,
+        gru_block_three: int = 1,
         layer_config: dict = {
             "layer0": (
                 40,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1022,125 +1170,152 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            gru_block_one=gru_block_one,
+            gru_block_two=gru_block_two,
+            gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        birnn_block_one: int = 1,
+        rnn_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },  # (neurons, activation, regularization, dropout)
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional RNN model."""
         self.create_birnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            birnn_block_one=birnn_block_one,
+            rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bilstm_block_one: int = 1,
+        lstm_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional LSTM model."""
         self.create_bilstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            bilstm_block_one=bilstm_block_one,
+            lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        bigru_block_one: int = 1,
+        gru_block_one: int = 1,
         layer_config: dict = {
             "layer0": (50, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional GRU model."""
         self.create_bigru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            bigru_block_one=bigru_block_one,
+            gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_rnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_rnn_block_one: int = 1,
+        enc_rnn_block_two: int = 1,
+        dec_rnn_block_one: int = 1,
+        dec_rnn_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1163,32 +1338,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder RNN model."""
         self.create_encdec_rnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_rnn_block_one=enc_rnn_block_one,
+            enc_rnn_block_two=enc_rnn_block_two,
+            dec_rnn_block_one=dec_rnn_block_one,
+            dec_rnn_block_two=dec_rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_lstm(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_lstm_block_one: int = 1,
+        enc_lstm_block_two: int = 1,
+        dec_lstm_block_one: int = 1,
+        dec_lstm_block_two: int = 1,
         layer_config: dict = {
             "layer0": (
                 100,
                 "relu",
                 0.0,
                 0.0,
             ),  # (neurons, activation, regularization, dropout)
@@ -1211,32 +1396,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder LSTM model."""
         self.create_encdec_lstm(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_lstm_block_one=enc_lstm_block_one,
+            enc_lstm_block_two=enc_lstm_block_two,
+            dec_lstm_block_one=dec_lstm_block_one,
+            dec_lstm_block_two=dec_lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_gru(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_gru_block_one: int = 1,
+        enc_gru_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (100, "relu", 0.0, 0.0),
             "layer1": (50, "relu", 0.0, 0.0),
             "layer2": (50, "relu", 0.0, 0.0),
             "layer3": (100, "relu", 0.0),
         },
         epochs: int = 100,
@@ -1244,32 +1439,42 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder GRU model."""
         self.create_encdec_gru(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_gru_block_one=enc_gru_block_one,
+            enc_gru_block_two=enc_gru_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_cnn(
         self,
         optimizer: str = "adam",
+        optimizer_args: dict = None,
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
+        enc_conv_block_one: int = 1,
+        enc_conv_block_two: int = 1,
+        dec_gru_block_one: int = 1,
+        dec_gru_block_two: int = 1,
         layer_config: dict = {
             "layer0": (64, 1, "relu", 0.0, 0.0),
             "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
             "layer3": (50, "relu", 0.0, 0.0),
             "layer4": (100, "relu", 0.0),
         },
@@ -1278,16 +1483,21 @@
         validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder CNN model."""
         self.create_encdec_cnn(
             optimizer=optimizer,
+            optimizer_args=optimizer_args,
             loss=loss,
             metrics=metrics,
+            enc_conv_block_one=enc_conv_block_one,
+            enc_conv_block_two=enc_conv_block_two,
+            dec_gru_block_one=dec_gru_block_one,
+            dec_gru_block_two=dec_gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
             board=board,
```

### Comparing `imbrium-1.2.0/imbrium/utils/transformer.py` & `imbrium-1.3.0/imbrium/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.2.0/imbrium.egg-info/SOURCES.txt` & `imbrium-1.3.0/imbrium.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 imbrium/predictors/__init__.py
 imbrium/predictors/multivarhybrid.py
 imbrium/predictors/multivarpure.py
 imbrium/predictors/univarhybrid.py
 imbrium/predictors/univarpure.py
 imbrium/utils/__init__.py
 imbrium/utils/optimization.py
+imbrium/utils/optimizer.py
 imbrium/utils/scaler.py
 imbrium/utils/transformer.py
```

### Comparing `imbrium-1.2.0/setup.py` & `imbrium-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/Imbrium",
     description="Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="imbrium",
-    version="1.2.0",
+    version="1.3.0",
     packages=find_packages(include=["imbrium", "imbrium.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "tensorflow >= 2.11.0, < 2.12.0",
         "matplotlib >= 3.5.0, < 3.7.0",
         "pandas >= 1.3.3, < 1.6.0",
         "scikit-learn >= 1.0, < 1.3.0",
```

