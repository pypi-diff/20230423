# Comparing `tmp/sd-parsers-0.2.1.tar.gz` & `tmp/sd-parsers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-parsers-0.2.1.tar", last modified: Thu Apr 20 22:44:30 2023, max compression
+gzip compressed data, was "sd-parsers-0.2.2.tar", last modified: Sun Apr 23 14:51:29 2023, max compression
```

## Comparing `sd-parsers-0.2.1.tar` & `sd-parsers-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.082386 sd-parsers-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/.github/workflows/publish-to.pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.082386 sd-parsers-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sd_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sdparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sdparsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/invokeai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/novelai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/prompt_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.github/workflows/publish-to.pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/examples/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sd_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 14:51:29.000000 sd-parsers-0.2.2/src/sd_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sdparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/src/sdparsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111_stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/parsers/novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/src/sdparsers/prompt_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.102538 sd-parsers-0.2.2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/resources/automatic1111/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_cropped.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)   382368 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/automatic1111/automatic1111_stealth.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.106538 sd-parsers-0.2.2/tests/resources/bad_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/bad_images/empty_file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/bad_images/text_after_idat.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/img2img_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/night_evening_day_morning_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/noisy_latents_3_subjects_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/comfyui/unclip_2pass_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/invokeai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/invokeai/invokeai1_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/novelai/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/novelai/novelai1_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/resources/parser_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/resources/parser_manager/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/test_parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:51:29.110538 sd-parsers-0.2.2/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/crop_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-23 14:51:19.000000 sd-parsers-0.2.2/tests/tools/crop_image.sh
```

### Comparing `sd-parsers-0.2.1/.github/workflows/publish-to.pypi.yml` & `sd-parsers-0.2.2/.github/workflows/publish-to.pypi.yml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/LICENSE.txt` & `sd-parsers-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/PKG-INFO` & `sd-parsers-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.1
+Version: 0.2.2
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: repository, https://github.com/d3x-at/sd-parsers
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 ## Features
 
 Supports reading metadata from images generated with:
```

### Comparing `sd-parsers-0.2.1/README.md` & `sd-parsers-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/examples/cmdline.py` & `sd-parsers-0.2.2/examples/cmdline.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             logging.exception("error reading file: %s", filename)
 
 
 def display_info(prompt_info: parser.PromptInfo):
     # Models
     print(f"{len(prompt_info.models)} Model(s) used:")
     for model in prompt_info.models:
-        print(f"Model: {model.name}\nModel Hash:{model.model_hash}")
+        print(f"Model: {model.name}\nModel Hash: {model.model_hash}")
 
     # Samplers
     print(f"\n{len(prompt_info.samplers)} Sampler(s) used:")
     for sampler in prompt_info.samplers:
         sampler_parameters = ", ".join(
             f"{k}: {v}" for k, v in sampler.parameters.items())
         print(f"Sampler: {sampler.name}\nSampler Parameters: {sampler_parameters}")
@@ -40,22 +40,22 @@
             print(f"Negative Prompt: {negative_prompt.value}")
 
     # Remaining metadata
     print("\nOther Metadata:")
     for k, v in prompt_info.metadata.items():
         print(f"{k}: {v}")
 
-    # Raw parameters
-    if prompt_info.generator in (
-            parser.AUTOMATIC1111Parser.GENERATOR_ID,
-            parser.AUTOMATICStealthParser.GENERATOR_ID):
+    # Some (not all) raw parameters
+    if prompt_info.generator == parser.AUTOMATIC1111Parser.GENERATOR_ID:
         print(f"\nRaw Parameters: {prompt_info.raw_params.get('parameters')}")
 
     elif prompt_info.generator == parser.InvokeAIParser.GENERATOR_ID:
         print(f"\nRaw Parameters: {prompt_info.raw_params.get('sd-metadata')}")
 
     elif prompt_info.generator == parser.ComfyUIParser.GENERATOR_ID:
         print(f"\nRaw Parameters: {prompt_info.raw_params.get('prompt')}")
 
+    elif prompt_info.generator == parser.NovelAIParser.GENERATOR_ID:
+        print(f"\nRaw Parameters: {prompt_info.raw_params.get('Comment')}")
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `sd-parsers-0.2.1/examples/fast_api.py` & `sd-parsers-0.2.2/examples/fast_api.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/src/sd_parsers.egg-info/PKG-INFO` & `sd-parsers-0.2.2/src/sd_parsers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.1
+Version: 0.2.2
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: repository, https://github.com/d3x-at/sd-parsers
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 ## Features
 
 Supports reading metadata from images generated with:
```

### Comparing `sd-parsers-0.2.1/src/sdparsers/config.json` & `sd-parsers-0.2.2/src/sdparsers/config.json`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/src/sdparsers/parser.py` & `sd-parsers-0.2.2/src/sdparsers/parser.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/src/sdparsers/parser_manager.py` & `sd-parsers-0.2.2/src/sdparsers/parser_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Type, Union
 
 if TYPE_CHECKING:
     from _typeshed import SupportsRead
 
@@ -38,15 +36,15 @@
 
         # initialize parsers
         self.parsers = sorted((parser(get_config(parser), process_items)
                                for parser in _get_parsers()),
                               key=lambda p: p.PRIORITY, reverse=True)
 
     def parse(self, image: Union[str, bytes, Path,
-                                 SupportsRead[bytes],
+                                 'SupportsRead[bytes]',
                                  Image.Image]) -> Optional[PromptInfo]:
         '''try available parsers to get image information
 
         The following exceptions can be thrown by the underlying `Image.open()`
         function:
         :exception FileNotFoundError: If the file cannot be found.
         :exception PIL.UnidentifiedImageError: If the image cannot be opened
```

### Comparing `sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111.py` & `sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import Tuple
+import json
+import re
+from typing import Optional, Tuple, Iterable
 
 from ..parser import Parser, get_exif_value
 from ..prompt_info import Model, Prompt, PromptInfo, Sampler
 
 SAMPLER_PARAMS_DEFAULT = ['CFG scale', 'Seed', 'Steps', 'ENSD']
 
+_RE_CIVITAI_HASHES = re.compile(r'(?:,\s*)?Hashes:\s*(\{[^\}]*\})\s*')
+
 
 class AUTOMATIC1111Parser(Parser):
     '''parse images created in AUTOMATIC1111's webui'''
     GENERATOR_ID = "AUTOMATIC1111"
 
     def __init__(self, config=None, process_items=True):
         super().__init__(config, process_items)
@@ -68,48 +72,46 @@
 
 
 def split_parameters(parameters: str) -> Tuple[str, str, dict]:
     '''
     split an A1111 parameters string into prompt, negative prompt and metadata
     :exception ValueError: If the metadata does not conform to the expected format.
     '''
+    def split_meta(last_line: str) -> Iterable[Tuple[str, str]]:
+        for item in last_line.split(','):
+            try:
+                key, value = map(str.strip, item.split(':'))
+                yield key, value
+            except ValueError:
+                pass
+
+    last_newline = parameters.rfind("\n")
+    if last_newline == -1:
+        raise ValueError("malformed parameters")
 
-    def split_meta(item: str) -> Tuple[str, str]:
-        '''
-        split metadata item into key:value pair
-        :exception ValueError: If the item has more or less than two components.
-        '''
-        components = item.split(':')
-        if len(components) != 2:
-            raise ValueError("metadata malformed")
-        key, value = map(str.strip, components)
-        return key, value
-
-    lines = parameters.split('\n')
-    metadata = dict(split_meta(item) for item in lines[-1].split(','))
-
+    last_line, hashes = get_civitai_hashes(parameters[last_newline:])
+    metadata = dict(split_meta(last_line))
     if len(metadata) < 3:
         # actually a bit stricter than in the webui itself
         # grants some protection against "non-a1111" parameters
         raise ValueError("metadata too short")
 
-    prompt_lines = lines[:-1]
-
-    # prompt
-    prompt = []
-    i = 0
-    for line in prompt_lines:
-        line = line.strip()
-        if line.startswith("Negative prompt:"):
-            prompt_lines[i] = line[16:]
-            break
-        prompt.append(line)
-        i += 1
-
-    # negative prompt
-    negative_prompt = [line.strip() for line in prompt_lines[i:]]
+    prompts = parameters[:last_newline].split('Negative prompt:')
+    prompt, negative_prompt = prompts + ['']*(2-len(prompts))
+    if hashes:
+        metadata["hashes"] = hashes
 
     return (
-        "\n".join(prompt),
-        "\n".join(negative_prompt),
+        prompt.strip("\n "),
+        negative_prompt.strip("\n "),
         metadata
     )
+
+
+def get_civitai_hashes(line: str) -> Tuple[str, Optional[dict]]:
+    hashes = None
+    match = _RE_CIVITAI_HASHES.search(line)
+    if match:
+        hashes = json.loads(match.group(1))
+        start, end = match.span(0)
+        line = line[:start] + line[end:]
+    return line, hashes
```

### Comparing `sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111_stealth.py` & `sd-parsers-0.2.2/src/sdparsers/parsers/automatic1111_stealth.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         metadata = self._prepare_metadata(geninfo)
         if metadata is None:
             return None
 
         return PromptInfo(self.GENERATOR_ID, *metadata, {"parameters": geninfo})
 
-    @staticmethod
+    @staticmethod  # noqa: C901
     def _read_info_from_image_stealth(image):
         # read_info_from_image_stealth method (image.mode check is done in parse()) from:
         # https://github.com/ashen-sensored/sd_webui_stealth_pnginfo/blob/main/scripts/stealth_pnginfo.py
 
         width, height = image.size
         pixels = image.load()
```

### Comparing `sd-parsers-0.2.1/src/sdparsers/parsers/comfyui.py` & `sd-parsers-0.2.2/src/sdparsers/parsers/comfyui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-import typing
 from collections import defaultdict
+from typing import Any, Iterable, Optional, Set, Tuple
 
 from ..parser import Parser
 from ..prompt_info import Model, Prompt, PromptInfo, Sampler
 
 SAMPLER_TYPES_DEFAULT = ["KSampler", "KSamplerAdvanced"]
 TEXT_TYPES_DEFAULT = []  # by default, don't filter text nodes by class_type
 TEXT_POSITIVE_KEYS_DEFAULT = ['text']
@@ -36,108 +36,134 @@
             return None
 
         params_prompt = image.text.get('prompt')
         params_workflow = image.text.get('workflow')
         if not params_prompt or not params_workflow:
             return None
 
-        prompts, samplers, models = self._prepare_metadata(params_prompt, params_workflow)
+        image_data = {
+            'prompt': json.loads(params_prompt),
+            'workflow': json.loads(params_workflow),
+            'links': defaultdict(list),
+            'inputs_cache': {'uniq': set()}
+        }
 
-        return PromptInfo(self.GENERATOR_ID, prompts, samplers, models, {}, {
-            "prompt": params_prompt,
-            "workflow": params_workflow
-        })
-
-    def _prepare_metadata(self, params_prompt: str, params_workflow: str):
-        prompt_data = json.loads(params_prompt)
-        workflow_data = json.loads(params_workflow)
-
-        links = defaultdict(list)
+        # build list of links of the allowed traverse types
+        # (start at a sampler, go backwards to reach all available model and text nodes)
         try:
-            for _, output_id, _, input_id, _, link_type in workflow_data["links"]:
+            for _, output_id, _, input_id, _, link_type in image_data['workflow']["links"]:
                 if link_type in self.traverse_types:
-                    links[input_id].append(output_id)
+                    image_data['links'][input_id].append(output_id)
         except ValueError:
             pass
 
-        def get_prompts(node_id: int, text_tags: typing.Set[str], depth: int = 0) -> typing.Iterable[str]:
-            '''recursively search for a text prompt, starting from the given node id'''
-            if self.traverse_limit != -1 and depth >= self.traverse_limit:
-                return
-            try:
-                # test if the current node has prompt text
-                node = prompt_data[str(node_id)]
-                if not self.text_types or node['class_type'] in self.text_types:
-                    for text_key in text_tags & set(node['inputs'].keys()):
-                        yield node['inputs'][text_key].strip()
-            except KeyError:
-                pass
-
-            # explore other inputs fed into this node
-            for output_id in links.get(node_id, []):
-                yield from get_prompts(output_id, text_tags, depth + 1)
-
-        # check all sampler types
-        samplers = []
-        models = []
-        prompt_ids = []
-        for sampler, positive_id, negative_id, model in self._get_samplers(prompt_data):
-            samplers.append(sampler)
-            if model:
-                models.append(model)
-            prompt_ids.append((positive_id, negative_id))
+        metadata = self._prepare_metadata(image_data)
 
-        # ignore multiple uses
-        prompts = []
-        for positive_id, negative_id in set(prompt_ids):
-            positive_prompts = list(get_prompts(positive_id, self.text_positive_keys)) \
-                if positive_id else None
-            negative_prompts = list(get_prompts(negative_id, self.text_negative_keys)) \
-                if negative_id else None
-
-            if negative_prompts or positive_prompts:
-                prompts.append((
-                    Prompt(value=",\n".join(positive_prompts), parts=positive_prompts)
-                    if positive_prompts else None,
-                    Prompt(value=",\n".join(negative_prompts), parts=negative_prompts)
-                    if negative_prompts else None
-                ))
+        return PromptInfo(self.GENERATOR_ID, **metadata, raw_params={
+            "prompt": params_prompt,
+            "workflow": params_workflow
+        })
 
-        return prompts, samplers, models
+    def _prepare_metadata(self, image_data: dict):
 
-    def _get_samplers(self, prompt_data):
         def might_be_sampler(node):
             try:
                 if self.sampler_types:
                     return node['class_type'] in self.sampler_types
                 return all(key in node['inputs'].keys() for key in _SAMPLER_EXCLUDES)
             except KeyError:
                 return False
 
-        for node in prompt_data.values():
+        samplers, models, prompts = [], [], []
+        for node in image_data['prompt'].values():
             if not might_be_sampler(node):
                 continue
 
             inputs = node.get('inputs')
             if not inputs:
                 continue
 
-            sampler_params = ((key, value) for key, value in inputs.items()
-                              if key not in _SAMPLER_EXCLUDES)
+            sampler, model, prompt = self._get_sampler_data(image_data, inputs)
+            samplers.append(sampler)
+            if model:
+                models.append(model)
+            if prompt:
+                prompts.append(prompt)
 
-            sampler = Sampler(
-                name=inputs.get('sampler_name'),
-                parameters=self._process_metadata(sampler_params))
+        return {
+            'samplers': samplers,
+            'models': models,
+            'prompts': prompts,
+            'metadata': {}
+        }
+
+    def _get_sampler_data(self, image_data: dict, inputs: dict):
+        # sampler
+        sampler_params = ((key, value) for key, value in inputs.items()
+                          if key not in _SAMPLER_EXCLUDES)
+        sampler = Sampler(
+            name=inputs.get('sampler_name'),
+            parameters=self._process_metadata(sampler_params))
 
-            positive_input = inputs.get("positive")
-            positive_id = int(positive_input[0]) if positive_input else None
+        # model
+        try:
+            model_node = image_data['prompt'][inputs['model'][0]]
+            model = Model(name=model_node['inputs']['ckpt_name'])
+        except (KeyError, ValueError):
+            model = None
+
+        # prompt
+        prompt = self._get_prompt(image_data, inputs)
+
+        return sampler, model, prompt
+
+    def _get_prompt(self, image_data: dict, inputs: dict):
+        inputs_cache = image_data['inputs_cache']
+
+        def get_prompt(input, text_keys) -> Tuple[Optional[Any], Optional[Prompt]]:
+            if not input:
+                return None, None
+            source_id = input[0]
+            # get cached prompt
+            prompt = inputs_cache.get(source_id)
+            if prompt:
+                return source_id, prompt
+            # collect reachable prompt parts
+            parts = list(self._get_parts(image_data, source_id, text_keys))
+            if not parts:
+                return None, None
+            # assemble prompt
+            prompt = Prompt(value=",\n".join(parts), parts=parts)
+            inputs_cache[source_id] = prompt
+            return source_id, prompt
+
+        positive_id, positive_prompt = get_prompt(
+            inputs.get("positive"), self.text_positive_keys)
+        negative_id, negative_prompt = get_prompt(
+            inputs.get("negative"), self.text_negative_keys)
 
-            negative_input = inputs.get("negative")
-            negative_id = int(negative_input[0]) if negative_input else None
+        if positive_id is None and negative_id is None:
+            return None
 
-            try:
-                model_node = prompt_data[inputs['model'][0]]
-                model = Model(name=model_node['inputs']['ckpt_name'])
-            except (KeyError, ValueError):
-                model = None
+        if (positive_id, negative_id) not in inputs_cache['uniq']:
+            inputs_cache['uniq'].add((positive_id, negative_id))
+            return positive_prompt, negative_prompt
+
+        return None
+
+    def _get_parts(self, image_data: dict, node_id, text_tags: Set[str], depth: int = 0
+                   ) -> Iterable[str]:
+        '''recursively search for all parts of a text prompt, starting from the given node id'''
+        if self.traverse_limit != -1 and depth >= self.traverse_limit:
+            return
+        try:
+            # test if the current node has prompt text
+            node = image_data['prompt'][node_id]
+            if not self.text_types or node['class_type'] in self.text_types:
+                for text_key in text_tags & set(node['inputs'].keys()):
+                    yield node['inputs'][text_key].strip()
+        except KeyError:
+            pass
 
-            yield sampler, positive_id, negative_id, model
+        # explore other inputs fed into this node
+        for output_id in image_data['links'].get(node_id, []):
+            yield from self._get_parts(output_id, text_tags, depth + 1)
```

### Comparing `sd-parsers-0.2.1/src/sdparsers/parsers/invokeai.py` & `sd-parsers-0.2.2/src/sdparsers/parsers/invokeai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/src/sdparsers/parsers/novelai.py` & `sd-parsers-0.2.2/src/sdparsers/parsers/novelai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.1/src/sdparsers/prompt_info.py` & `sd-parsers-0.2.2/src/sdparsers/prompt_info.py`

 * *Files identical despite different names*

