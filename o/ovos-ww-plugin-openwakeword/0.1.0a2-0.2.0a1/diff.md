# Comparing `tmp/ovos_ww_plugin_openwakeword-0.1.0a2-py3-none-any.whl.zip` & `tmp/ovos_ww_plugin_openwakeword-0.2.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7735 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3230 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      377 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      101 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      804 b- defN 23-Mar-06 01:38 ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/RECORD
-8 files, 16158 bytes uncompressed, 6289 bytes compressed:  61.1%
+Zip file size: 7825 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3482 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      390 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      101 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/RECORD
+8 files, 16423 bytes uncompressed, 6379 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_ww_plugin_openwakeword/__init__.py
 Comment: 
 
 Filename: ovos_ww_plugin_openwakeword/version.py
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/LICENSE
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/METADATA
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/WHEEL
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/entry_points.txt
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/top_level.txt
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/RECORD
+Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_ww_plugin_openwakeword/__init__.py

```diff
@@ -42,31 +42,34 @@
     def update(self, chunk):
         """
         Predict on input audio using openWakeWord models.
         openWakeWord requires that audio be provided in chunks of 1280 samples,
         so a small buffer is used to ensure proper sizes.
         """
         audio_frame = np.frombuffer(chunk, dtype=np.int16).tolist()
-        self.audio_buffer.extend(audio_frame)
-        if len(self.audio_buffer) > 1280:
+        self.audio_buffer.extend(audio_frame)  # build up the buffer until it has enough samples
+
+        if len(self.audio_buffer) >= 1280:
             # Get prediction from openWakeWord
-            prediction = self.model.predict(list(self.audio_buffer[0:1280]))
+            prediction = self.model.predict(self.audio_buffer)
 
-            # Advance the buffer
-            self.audio_buffer = self.audio_buffer[1280:]
+            # Clear the buffer after each prediction
+            self.audio_buffer = []
 
             # Check for score above threshold
             for mdl_name in self.model_names:
                 if prediction[mdl_name] >= self.config.get("threshold"):
                     # Set flag indicating that a wakeword was detected
                     self.has_found = True
 
-                    # Flush recent history of openWakeWord feature buffer to avoid re-activations
+                    # Flush recent history of openWakeWord internal audio buffer to avoid re-activations
                     n_frames = self.model.model_inputs[mdl_name]
+                    self.model.preprocessor.raw_data_buffer.extend([0.0]*n_frames*1280)
                     self.model.preprocessor.feature_buffer[-n_frames:, :] = np.zeros((n_frames, 96)).astype(np.float32)
+                    self.model.preprocessor.melspectrogram_buffer[-250:, :] = np.zeros((250, 32)).astype(np.float32)
                     
                     break
                     
 
     def found_wake_word(self, frame_data):
         if self.has_found:
             self.has_found = False
```

## ovos_ww_plugin_openwakeword/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
-VERSION_MINOR = 1
+VERSION_MINOR = 2
 VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_ww_plugin_openwakeword-0.1.0a2.dist-info/LICENSE` & `ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE`

 * *Files identical despite different names*

