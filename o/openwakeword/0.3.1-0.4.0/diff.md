# Comparing `tmp/openwakeword-0.3.1.tar.gz` & `tmp/openwakeword-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwakeword-0.3.1.tar", last modified: Mon Mar  6 01:31:28 2023, max compression
+gzip compressed data, was "openwakeword-0.4.0.tar", last modified: Sat Apr 22 22:07:13 2023, max compression
```

## Comparing `openwakeword-0.3.1.tar` & `openwakeword-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.997745 openwakeword-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 01:31:19.000000 openwakeword-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-06 01:31:19.000000 openwakeword-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-03-06 01:31:27.997745 openwakeword-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-03-06 01:31:19.000000 openwakeword-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.981745 openwakeword-0.3.1/openwakeword/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/custom_verifier_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32108 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19077 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.977745 openwakeword-0.3.1/openwakeword/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.993745 openwakeword-0.3.1/openwakeword/resources/models/
--rw-r--r--   0 runner    (1001) docker     (123)   854246 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/alexa_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  1328103 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/embedding_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  1271370 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/hey_jarvis_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)   857691 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/hey_marvin_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)   503850 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/hey_mycroft_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  1087958 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/melspectrogram.onnx
--rwxr-xr-x   0 runner    (1001) docker     (123)  1807522 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  1742475 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/timer_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  1149158 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/resources/models/weather_v0.1.onnx
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-03-06 01:31:19.000000 openwakeword-0.3.1/openwakeword/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.985745 openwakeword-0.3.1/openwakeword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-03-06 01:31:27.000000 openwakeword-0.3.1/openwakeword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-06 01:31:27.000000 openwakeword-0.3.1/openwakeword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:31:27.000000 openwakeword-0.3.1/openwakeword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-06 01:31:27.000000 openwakeword-0.3.1/openwakeword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 01:31:27.000000 openwakeword-0.3.1/openwakeword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-06 01:31:19.000000 openwakeword-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 01:31:27.997745 openwakeword-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-06 01:31:19.000000 openwakeword-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:31:27.997745 openwakeword-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-06 01:31:19.000000 openwakeword-0.3.1/tests/test_custom_verifier_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-03-06 01:31:19.000000 openwakeword-0.3.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.917442 openwakeword-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-22 22:06:58.000000 openwakeword-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 22:06:58.000000 openwakeword-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-22 22:07:13.917442 openwakeword-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-04-22 22:06:58.000000 openwakeword-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.901442 openwakeword-0.4.0/openwakeword/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/custom_verifier_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32108 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19970 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.897442 openwakeword-0.4.0/openwakeword/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.913442 openwakeword-0.4.0/openwakeword/resources/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   854246 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/alexa_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)  1328103 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/embedding_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)  1271370 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/hey_jarvis_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)   857691 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/hey_marvin_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)   503850 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/hey_mycroft_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)  1087958 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/melspectrogram.onnx
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1807522 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)  1742475 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/timer_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)  1149158 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/resources/models/weather_v0.1.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-04-22 22:06:58.000000 openwakeword-0.4.0/openwakeword/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.901442 openwakeword-0.4.0/openwakeword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-22 22:07:13.000000 openwakeword-0.4.0/openwakeword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-22 22:07:13.000000 openwakeword-0.4.0/openwakeword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:07:13.000000 openwakeword-0.4.0/openwakeword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-22 22:07:13.000000 openwakeword-0.4.0/openwakeword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 22:07:13.000000 openwakeword-0.4.0/openwakeword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-22 22:06:58.000000 openwakeword-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:07:13.917442 openwakeword-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-22 22:06:58.000000 openwakeword-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:13.917442 openwakeword-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-22 22:06:58.000000 openwakeword-0.4.0/tests/test_custom_verifier_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-22 22:06:58.000000 openwakeword-0.4.0/tests/test_models.py
```

### Comparing `openwakeword-0.3.1/LICENSE` & `openwakeword-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/PKG-INFO` & `openwakeword-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwakeword
-Version: 0.3.1
+Version: 0.4.0
 Summary: An open-source audio wake word (or phrase) detection framework with a focus on performance and simplicity
 Home-page: https://pypi.org/project/openwakeword
 Author: David Scripka
 Author-email: David Scripka <david.scripka@gmail.com>
 Project-URL: Homepage, https://github.com/dscripka/openWakeWord
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -52,15 +52,17 @@
 from openwakeword.model import Model
 
 # Instantiate the model
 model = Model(
     wakeword_model_paths=["path/to/model.onnx"],  # can also leave this argument empty to load all of the included pre-trained models
 )
 
-# Get an 80 ms audio frame containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc. 
+# Get audio data containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc.
+# For the best efficiency and latency, audio frames should be multiples of 80 ms, with longer frames
+# increasing overall efficiency at the cost of detection latency
 frame = my_function_to_get_audio_frame()
 
 # Get predictions for the frame
 prediction = model.predict(frame)
 ```
 
 # Recommendations for Usage
@@ -75,15 +77,15 @@
 
 ## Threshold Scores for Activation
 
 All of the included openWakeWord models were trained to work well with a default threshold of `0.5` for a positive prediction, but you are encouraged to determine the best threshold for your environment and use-case through testing. For certain deployments, using a lower or higher threshold in practice may result in significantly better performance.
 
 ## User-specific models
 
-If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to voices new voices.
+If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to new voices.
 
 # Project Goals
 
 openWakeWord has four high-level goals, which combine to (hopefully!) produce a framework that is simple to use *and* extend.
 
 1) Be fast *enough* for real-world usage, while maintaining ease of use and development. For example, a single core of a Raspberry Pi 3 can run 15-20 openWakeWord models simultaneously in real-time. However, the models are likely still too large for less powerful systems or micro-controllers. Commercial options like [Picovoice Porcupine](https://picovoice.ai/platform/porcupine/) or [Fluent Wakeword](https://fluent.ai/products/wakeword/) are likely better suited for highly constrained hardware environments.
```

### Comparing `openwakeword-0.3.1/README.md` & `openwakeword-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 from openwakeword.model import Model
 
 # Instantiate the model
 model = Model(
     wakeword_model_paths=["path/to/model.onnx"],  # can also leave this argument empty to load all of the included pre-trained models
 )
 
-# Get an 80 ms audio frame containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc. 
+# Get audio data containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc.
+# For the best efficiency and latency, audio frames should be multiples of 80 ms, with longer frames
+# increasing overall efficiency at the cost of detection latency
 frame = my_function_to_get_audio_frame()
 
 # Get predictions for the frame
 prediction = model.predict(frame)
 ```
 
 # Recommendations for Usage
@@ -58,15 +60,15 @@
 
 ## Threshold Scores for Activation
 
 All of the included openWakeWord models were trained to work well with a default threshold of `0.5` for a positive prediction, but you are encouraged to determine the best threshold for your environment and use-case through testing. For certain deployments, using a lower or higher threshold in practice may result in significantly better performance.
 
 ## User-specific models
 
-If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to voices new voices.
+If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to new voices.
 
 # Project Goals
 
 openWakeWord has four high-level goals, which combine to (hopefully!) produce a framework that is simple to use *and* extend.
 
 1) Be fast *enough* for real-world usage, while maintaining ease of use and development. For example, a single core of a Raspberry Pi 3 can run 15-20 openWakeWord models simultaneously in real-time. However, the models are likely still too large for less powerful systems or micro-controllers. Commercial options like [Picovoice Porcupine](https://picovoice.ai/platform/porcupine/) or [Fluent Wakeword](https://fluent.ai/products/wakeword/) are likely better suited for highly constrained hardware environments.
 
@@ -180,8 +182,8 @@
 
 Currently, openWakeWord only supports English, primarily because the pre-trained text-to-speech models used to generate training data are all based on english datasets. It's likely that speech-to-text models trained on other languages would also work well, but non-english models & datasets are less commonly available.
 
 Future release road maps may have non-english support. In particular, [Mycroft.AIs Mimic 3](https://github.com/MycroftAI/mimic3-voices) TTS engine may work well to help extend some support to other languages.
 
 # License
 
-All of the code in openWakeWord is licensed under the **Apache 2.0** license. All of the included pre-trained models are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license due to the inclusion of datasets with unknown or restrictive licensing as part of the training data. If you are interested in pre-trained models with more permissive licensing, please raise an issue and we will try to add them to a future release.
+All of the code in openWakeWord is licensed under the **Apache 2.0** license. All of the included pre-trained models are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license due to the inclusion of datasets with unknown or restrictive licensing as part of the training data. If you are interested in pre-trained models with more permissive licensing, please raise an issue and we will try to add them to a future release.
```

### Comparing `openwakeword-0.3.1/openwakeword/__init__.py` & `openwakeword-0.4.0/openwakeword/__init__.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/custom_verifier_model.py` & `openwakeword-0.4.0/openwakeword/custom_verifier_model.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/data.py` & `openwakeword-0.4.0/openwakeword/data.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/metrics.py` & `openwakeword-0.4.0/openwakeword/metrics.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/model.py` & `openwakeword-0.4.0/openwakeword/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,16 +153,17 @@
         """Reset the prediction buffer"""
         self.prediction_buffer = defaultdict(partial(deque, maxlen=30))
 
     def predict(self, x: np.ndarray, patience: dict = {}, threshold: dict = {}, timing: bool = False):
         """Predict with all of the wakeword models on the input audio frames
 
         Args:
-            x (Union[ndarray]): The input audio data to predict on with the models. Must be 1280
-                                      samples of 16khz, 16-bit audio data.
+            x (Union[ndarray]): The input audio data to predict on with the models. Should be multiples of 80 ms
+                                (1280 samples), with longer lengths reducing overall CPU usage
+                                but decreasing detection latency.
             patience (dict): How many consecutive frames (of 1280 samples or 80 ms) above the threshold that must
                              be observed before the current frame will be returned as non-zero.
                              Must be provided as an a dictionary where the keys are the
                              model names and the values are the number of frames. Can reduce false-positive
                              detections at the cost of a lower true-positive rate.
                              By default, this behavior is disabled.
             threshold (dict): The threshold values to use when the `patience` behavior is enabled.
@@ -196,19 +197,34 @@
         predictions = {}
         for mdl in self.models.keys():
             input_name = self.model_input_names[mdl]
 
             if timing:
                 model_start = time.time()
 
-            # Run model
-            prediction = self.models[mdl].run(
-                                    None,
-                                    {input_name: self.preprocessor.get_features(self.model_inputs[mdl])}
-                                )
+            # Run model to get predictions
+            if len(x) > 1280:
+                group_predictions = []
+                for i in np.arange(len(x)//1280-1, -1, -1):
+                    group_predictions.extend(
+                        self.models[mdl].run(
+                            None,
+                            {input_name: self.preprocessor.get_features(
+                                    self.model_inputs[mdl],
+                                    start_ndx=-self.model_inputs[mdl] - i
+                            )}
+                        )
+                    )
+                prediction = np.array(group_predictions).max(axis=0)[None, ]
+            else:
+                prediction = self.models[mdl].run(
+                                        None,
+                                        {input_name: self.preprocessor.get_features(self.model_inputs[mdl])}
+                                    )
+
             if self.model_outputs[mdl] == 1:
                 predictions[mdl] = prediction[0][0][0]
             else:
                 for int_label, cls in self.class_mapping[mdl].items():
                     predictions[cls] = prediction[0][0][int(int_label)]
 
             # Update scores based on custom verifier model
@@ -263,23 +279,24 @@
                     predictions[mdl] = 0.0
 
         if timing:
             return predictions, timing_dict
         else:
             return predictions
 
-    def predict_clip(self, clip: Union[str, np.ndarray], padding: int = 1, **kwargs):
+    def predict_clip(self, clip: Union[str, np.ndarray], padding: int = 1, chunk_size=1280, **kwargs):
         """Predict on an full audio clip, simulating streaming prediction.
         The input clip must bit a 16-bit, 16 khz, single-channel WAV file.
 
         Args:
             clip (Union[str, np.ndarray]): The path to a 16-bit PCM, 16 khz, single-channel WAV file,
                                            or an 1D array containing the same type of data
             padding (int): How many seconds of silence to pad the start/end of the clip with
                             to make sure that short clips can be processed correctly (default: 1)
+            chunk_size (int): The size (in samples) of each chunk of audio to pass to the model
             kwargs: Any keyword arguments to pass to the class `predict` method
 
         Returns:
             list: A list containing the frame-level prediction dictionaries for the audio clip
         """
         if isinstance(clip, str):
             # Load audio clip as 16-bit PCM data
@@ -296,15 +313,15 @@
                     data,
                     np.zeros(16000*padding).astype(np.int16)
                 )
             )
 
         # Iterate through clip, getting predictions
         predictions = []
-        step_size = 1280
+        step_size = chunk_size
         for i in range(0, data.shape[0]-step_size, step_size):
             predictions.append(self.predict(data[i:i+step_size], **kwargs))
 
         return predictions
 
     def _get_positive_prediction_frames(
             self,
```

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/alexa_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/alexa_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/embedding_model.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/embedding_model.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/hey_jarvis_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/hey_jarvis_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/hey_marvin_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/hey_marvin_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/hey_mycroft_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/hey_mycroft_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/melspectrogram.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/melspectrogram.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/silero_vad.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/timer_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/timer_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/resources/models/weather_v0.1.onnx` & `openwakeword-0.4.0/openwakeword/resources/models/weather_v0.1.onnx`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword/utils.py` & `openwakeword-0.4.0/openwakeword/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                                                     providers=["CUDAExecutionProvider", "CPUExecutionProvider"])
         self.onnx_execution_provider = self.melspec_model.get_providers()[0]
 
         # Create databuffers
         self.raw_data_buffer: Deque = deque(maxlen=sr*10)
         self.melspectrogram_buffer = np.ones((76, 32))  # n_frames x num_features
         self.melspectrogram_max_len = 10*97  # 97 is the number of frames in 1 second of 16hz audio
+        self.accumulated_samples = 0  # the samples added to the buffer since the audio preprocessor was last called
         self.feature_buffer = self._get_embeddings(np.zeros(160000).astype(np.int16))  # fill with blank data to start
         self.feature_buffer_max_len = 120  # ~10 seconds of feature buffer history
 
     def _get_melspectrogram(self, x: Union[np.ndarray, List], melspec_transform: Callable = lambda x: x/10 + 2):
         """
         Function to compute the mel-spectrogram of the provided audio samples.
 
@@ -206,15 +207,15 @@
             raise ValueError("Embedding model requires the input melspectrograms to have at least 76 frames")
 
         # Prepare ThreadPool object, if needed for multithreading
         pool = None
         if "CPU" in self.onnx_execution_provider:
             pool = ThreadPool(processes=ncpu)
 
-        # Calcuate array sizes and make batches
+        # Calculate array sizes and make batches
         n_frames = (x.shape[1] - 76)//8 + 1
         embedding_dim = 96  # fixed by embedding model
         embeddings = np.empty((x.shape[0], n_frames, embedding_dim), dtype=np.float32)
 
         batch = []
         ndcs = []
         for ndx, melspec in enumerate(x):
@@ -271,45 +272,70 @@
         melspecs = self._get_melspectrogram_batch(x, batch_size=batch_size, ncpu=ncpu)
 
         # Compute embeddings from melspectrograms
         embeddings = self._get_embeddings_batch(melspecs[:, :, :, None], batch_size=batch_size, ncpu=ncpu)
 
         return embeddings
 
-    def _streaming_melspectrogram(self, x):
+    def _streaming_melspectrogram(self, n_samples):
         """Note! There seem to be some slight numerical issues depending on the underlying audio data
         such that the streaming method is not exactly the same as when the melspectrogram of the entire
         clip is calculated. It's unclear if this difference is significant and will impact model performance.
         In particular padding with 0 or very small values seems to demonstrate the differences well.
         """
-        if len(x) < 400:
-            raise ValueError("The number of input frames must be at least 400 samples @ 16khz (25 ms)!")
-        self.raw_data_buffer.extend(x.tolist() if isinstance(x, np.ndarray) else x)
         self.melspectrogram_buffer = np.vstack(
-            (self.melspectrogram_buffer, self._get_melspectrogram(list(self.raw_data_buffer)[-len(x)-160*3:]))
+            (self.melspectrogram_buffer, self._get_melspectrogram(list(self.raw_data_buffer)[-n_samples-160*3:]))
         )
 
         if self.melspectrogram_buffer.shape[0] > self.melspectrogram_max_len:
             self.melspectrogram_buffer = self.melspectrogram_buffer[-self.melspectrogram_max_len:, :]
 
+    def _buffer_raw_data(self, x):
+        """
+        Adds raw audio data to the input buffer
+        """
+        if len(x) < 400:
+            raise ValueError("The number of input frames must be at least 400 samples @ 16khz (25 ms)!")
+        self.raw_data_buffer.extend(x.tolist() if isinstance(x, np.ndarray) else x)
+
     def _streaming_features(self, x):
-        if len(x) != 1280:
-            raise ValueError("You must provide input samples in frames of 1280 samples @ 1600khz."
-                             f"Received a frame of {len(x)} samples.")
-        self._streaming_melspectrogram(x)
-        x = self.melspectrogram_buffer[-76:].astype(np.float32)[None, :, :, None]
-        if x.shape[1] == 76:
-            self.feature_buffer = np.vstack((self.feature_buffer,
-                                             self.embedding_model.run(None, {'input_1': x})[0].squeeze()))
+        # if len(x) != 1280:
+        #     raise ValueError("You must provide input samples in frames of 1280 samples @ 1600khz."
+        #                      f"Received a frame of {len(x)} samples.")
+
+        # Add raw audio data to buffer
+        self._buffer_raw_data(x)
+        self.accumulated_samples += len(x)
+
+        # Only calculate melspectrogram every ~0.5 seconds to significantly increase efficiency
+        if self.accumulated_samples >= 1280:
+            self._streaming_melspectrogram(self.accumulated_samples)
+
+            # Calculate new audio embeddings/features based on update melspectrograms
+            for i in np.arange(self.accumulated_samples//1280-1, -1, -1):
+                ndx = -8*i
+                ndx = ndx if ndx != 0 else len(self.melspectrogram_buffer)
+                x = self.melspectrogram_buffer[-76 + ndx:ndx].astype(np.float32)[None, :, :, None]
+                if x.shape[1] == 76:
+                    self.feature_buffer = np.vstack((self.feature_buffer,
+                                                    self.embedding_model.run(None, {'input_1': x})[0].squeeze()))
+
+            # Reset raw data buffer counter
+            self.accumulated_samples = 0
 
         if self.feature_buffer.shape[0] > self.feature_buffer_max_len:
             self.feature_buffer = self.feature_buffer[-self.feature_buffer_max_len:, :]
 
-    def get_features(self, n_feature_frames: int = 16):
-        return self.feature_buffer[int(-1*n_feature_frames):, :][None, ].astype(np.float32)
+    def get_features(self, n_feature_frames: int = 16, start_ndx: int = -1):
+        if start_ndx != -1:
+            end_ndx = start_ndx + int(n_feature_frames) \
+                if start_ndx + n_feature_frames != 0 else len(self.feature_buffer)
+            return self.feature_buffer[start_ndx:end_ndx, :][None, ].astype(np.float32)
+        else:
+            return self.feature_buffer[int(-1*n_feature_frames):, :][None, ].astype(np.float32)
 
     def __call__(self, x):
         self._streaming_features(x)
 
 
 # Bulk prediction function
 def bulk_predict(
@@ -324,15 +350,16 @@
 
     Args:
         input_paths (List[str]): The list of input file to predict
         wakeword_model_path (List[str])): The paths to the wakeword ONNX model files
         prediction_function (str): The name of the method used to predict on the input audio files
                                    (default is the `predict_clip` method)
         ncpu (int): How many processes to create (up to max of available CPUs)
-        kwargs (dict): Any other keyword arguments to pass to the model initialization
+        kwargs (dict): Any other keyword arguments to pass to the model initialization or
+                       specified prediction function
 
     Returns:
         dict: A dictionary containing the predictions for each file, with the filepath as the key
     """
 
     # Create openWakeWord model objects
     n_batches = max(1, len(file_paths)//ncpu)
```

### Comparing `openwakeword-0.3.1/openwakeword/vad.py` & `openwakeword-0.4.0/openwakeword/vad.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/openwakeword.egg-info/PKG-INFO` & `openwakeword-0.4.0/openwakeword.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwakeword
-Version: 0.3.1
+Version: 0.4.0
 Summary: An open-source audio wake word (or phrase) detection framework with a focus on performance and simplicity
 Home-page: https://pypi.org/project/openwakeword
 Author: David Scripka
 Author-email: David Scripka <david.scripka@gmail.com>
 Project-URL: Homepage, https://github.com/dscripka/openWakeWord
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -52,15 +52,17 @@
 from openwakeword.model import Model
 
 # Instantiate the model
 model = Model(
     wakeword_model_paths=["path/to/model.onnx"],  # can also leave this argument empty to load all of the included pre-trained models
 )
 
-# Get an 80 ms audio frame containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc. 
+# Get audio data containing 16-bit 16khz PCM audio data from a file, microphone, network stream, etc.
+# For the best efficiency and latency, audio frames should be multiples of 80 ms, with longer frames
+# increasing overall efficiency at the cost of detection latency
 frame = my_function_to_get_audio_frame()
 
 # Get predictions for the frame
 prediction = model.predict(frame)
 ```
 
 # Recommendations for Usage
@@ -75,15 +77,15 @@
 
 ## Threshold Scores for Activation
 
 All of the included openWakeWord models were trained to work well with a default threshold of `0.5` for a positive prediction, but you are encouraged to determine the best threshold for your environment and use-case through testing. For certain deployments, using a lower or higher threshold in practice may result in significantly better performance.
 
 ## User-specific models
 
-If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to voices new voices.
+If the baseline performance of openWakeWord models is not sufficient for a given application (specifically, if the false activation rate is unacceptably high), it is possible to train [custom verifier models](docs/custom_verifier_models.md) for specific voices that act as a second-stage filter on predictions (i.e., only allow activations through that were likely spoken by a known set of voices). This can greatly improve performance, at the cost of making the openWakeWord system less likely to respond to new voices.
 
 # Project Goals
 
 openWakeWord has four high-level goals, which combine to (hopefully!) produce a framework that is simple to use *and* extend.
 
 1) Be fast *enough* for real-world usage, while maintaining ease of use and development. For example, a single core of a Raspberry Pi 3 can run 15-20 openWakeWord models simultaneously in real-time. However, the models are likely still too large for less powerful systems or micro-controllers. Commercial options like [Picovoice Porcupine](https://picovoice.ai/platform/porcupine/) or [Fluent Wakeword](https://fluent.ai/products/wakeword/) are likely better suited for highly constrained hardware environments.
```

### Comparing `openwakeword-0.3.1/openwakeword.egg-info/SOURCES.txt` & `openwakeword-0.4.0/openwakeword.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/pyproject.toml` & `openwakeword-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 testpaths = [
     "tests",
     "openwakeword"
 ]
 
 [project]
 name = "openwakeword"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="David Scripka", email="david.scripka@gmail.com" },
 ]
 description = "An open-source audio wake word (or phrase) detection framework with a focus on performance and simplicity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `openwakeword-0.3.1/setup.py` & `openwakeword-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     else:
         additional_requires = []
 
     return additional_requires
 
 setuptools.setup(
     name="openwakeword",
-    version="0.3.1",
+    version="0.4.0",
     install_requires=['onnxruntime>=1.10.0,<2', 'tqdm>=4.0,<5.0', 'scipy>=1.3,<2', 'scikit-learn>=1,<2'],
     extras_require={
         'test': [
                     'pytest>=7.2.0,<8',
                     'pytest-cov>=2.10.1,<3',
                     'pytest-flake8>=1.1.1,<2',
                     'flake8>=4.0,<4.1',
```

### Comparing `openwakeword-0.3.1/tests/test_custom_verifier_model.py` & `openwakeword-0.4.0/tests/test_custom_verifier_model.py`

 * *Files identical despite different names*

### Comparing `openwakeword-0.3.1/tests/test_models.py` & `openwakeword-0.4.0/tests/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         owwModel = openwakeword.Model(wakeword_model_paths=[
                                         os.path.join("openwakeword", "resources", "models", "alexa_v0.1.onnx")
                                       ])
 
         # Prediction on random data
         owwModel.predict(np.random.randint(-1000, 1000, 1280).astype(np.int16))
 
+        # Prediction on random data with different chunk size
+        owwModel.predict(np.random.randint(-1000, 1000, 1280*2).astype(np.int16))
+
     def test_custom_model_label_mapping_dict(self):
         # Load model with model path
         owwModel = openwakeword.Model(wakeword_model_paths=[
                                         os.path.join("openwakeword", "resources", "models", "alexa_v0.1.onnx")
                                       ],
                                       class_mapping_dicts=[{"alexa_v0.1": {"0": "positive"}}]
                                       )
```

