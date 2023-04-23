# Comparing `tmp/rembg-2.0.32.tar.gz` & `tmp/rembg-2.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.32.tar", last modified: Fri Mar 31 16:16:32 2023, max compression
+gzip compressed data, was "rembg-2.0.33.tar", last modified: Sun Apr 23 04:49:09 2023, max compression
```

## Comparing `rembg-2.0.32.tar` & `rembg-2.0.33.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:16:32.469142 rembg-2.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-31 16:16:09.000000 rembg-2.0.32/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-31 16:16:09.000000 rembg-2.0.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-03-31 16:16:32.469142 rembg-2.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-03-31 16:16:09.000000 rembg-2.0.32/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-31 16:16:10.000000 rembg-2.0.32/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:16:32.469142 rembg-2.0.32/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-31 16:16:32.469142 rembg-2.0.32/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/session_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/session_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/session_dis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/session_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-31 16:16:10.000000 rembg-2.0.32/rembg/session_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:16:32.469142 rembg-2.0.32/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 16:16:32.000000 rembg-2.0.32/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 16:16:10.000000 rembg-2.0.32/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-31 16:16:10.000000 rembg-2.0.32/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-31 16:16:32.469142 rembg-2.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-31 16:16:10.000000 rembg-2.0.32/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-03-31 16:16:10.000000 rembg-2.0.32/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 04:48:58.000000 rembg-2.0.33/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 04:48:58.000000 rembg-2.0.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-23 04:49:09.301674 rembg-2.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-23 04:48:58.000000 rembg-2.0.33/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-23 04:48:58.000000 rembg-2.0.33/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.297674 rembg-2.0.33/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/dis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.297674 rembg-2.0.33/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 04:48:58.000000 rembg-2.0.33/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-23 04:48:58.000000 rembg-2.0.33/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 04:49:09.301674 rembg-2.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-23 04:48:58.000000 rembg-2.0.33/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-23 04:48:58.000000 rembg-2.0.33/versioneer.py
```

### Comparing `rembg-2.0.32/LICENSE.txt` & `rembg-2.0.33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.32/PKG-INFO` & `rembg-2.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.32
+Version: 2.0.33
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -169,14 +169,20 @@
 
 Remove the background applying an alpha matting
 
 ```
 rembg i -a path/to/input.png path/to/output.png
 ```
 
+Passing extras parameters
+
+```
+rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -266,15 +272,15 @@
 
     with open(input_path, 'rb') as i:
         with open(output_path, 'wb') as o:
             input = i.read()
             output = remove(input, session=session)
             o.write(output)
 ```
-
+To see a full list of examples on how to use rembg, go to the [examples](USAGE.md) page.
 ## Usage as a docker
 
 Just replace the `rembg` command for `docker run danielgatis/rembg`.
 
 Try this:
 
 ```
@@ -289,43 +295,47 @@
 
 -   u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
 -   u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
 -   u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
 -   u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
+-   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### Some differences between the models result
 
 <table>
     <tr>
         <th>original</th>
         <th>u2net</th>
         <th>u2netp</th>
         <th>u2net_human_seg</th>
         <th>u2net_cloth_seg</th>
         <th>silueta</th>
         <th>isnet-general-use</th>
+        <th>sam</th>
     </tr>
     <tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/car-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.sam.png" width="100" /></th>
     </tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/cloth-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.sam.png" width="100" /></th>
     </tr>
 </table>
 
 
 ### How to train your own model
 
 If You need more fine tunned models try this:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.32 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.33 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -61,21 +61,23 @@
 using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
 files. Remove the background from a remote image ``` curl -s http://input.png |
 rembg i > output.png ``` Remove the background from a local file ``` rembg i
 path/to/input.png path/to/output.png ``` Remove the background specifying a
 model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
 background returning only the mask ``` rembg i -om path/to/input.png path/to/
 output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` ### rembg `p` Used when input and
-output are folders. Remove the background from all images in a folder ``` rembg
-p path/to/input path/to/output ``` Same as before, but watching for new/changed
-files to process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s`
-Used to start http server. To see the complete endpoints documentation, go to:
-`http://localhost:5000/docs`. Remove the background from an image url ``` curl
--s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
+a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
+i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
+input.png path/to/output.png ``` ### rembg `p` Used when input and output are
+folders. Remove the background from all images in a folder ``` rembg p path/to/
+input path/to/output ``` Same as before, but watching for new/changed files to
+process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
+start http server. To see the complete endpoints documentation, go to: `http://
+localhost:5000/docs`. Remove the background from an image url ``` curl -
+s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
 background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
 "http://localhost:5000" -o output.png ``` ## Usage as a library Input and
 output as bytes ```python from rembg import remove input_path = 'input.png'
 output_path = 'output.png' with open(input_path, 'rb') as i: with open
 (output_path, 'wb') as o: input = i.read() output = remove(input) o.write
 (output) ``` Input and output as a PIL image ```python from rembg import remove
 from PIL import Image input_path = 'input.png' output_path = 'output.png' input
@@ -84,43 +86,49 @@
 input_path = 'input.png' output_path = 'output.png' input = cv2.imread
 (input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
 iterate over files in a performatic way ```python from pathlib import Path from
 rembg import remove, new_session session = new_session() for file in Path
 ('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
 (file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
 open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` ## Usage as a docker Just replace the
-`rembg` command for `docker run danielgatis/rembg`. Try this: ``` docker run
-danielgatis/rembg i path/to/input.png path/to/output.png ``` ## Models All
-models are downloaded and saved in the user home folder in the `.u2net`
-directory. The available models are: - u2net ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://
-github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases. -
-u2netp ([download](https://github.com/danielgatis/rembg/releases/download/
-v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
-lightweight version of u2net model. - u2net_human_seg ([download](https://
+session=session) o.write(output) ``` To see a full list of examples on how to
+use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
+replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
+docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
+Models All models are downloaded and saved in the user home folder in the
+`.u2net` directory. The available models are: - u2net ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
+cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
+A lightweight version of u2net model. - u2net_human_seg ([download](https://
 github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
 [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
 segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
 rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
 github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
 Parsing from human portrait. Here clothes are parsed into 3 category: Upper
 body, Lower body and Full body. - silueta ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
 github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
 reduced to 43Mb. - isnet-general-use ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
 (https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. ### Some differences between the models result
-original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use
-[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
-raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
-danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
-tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet-
-                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]
+cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
+quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
+pre-trained model for any use cases. ### Some differences between the models
+result
+original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
+[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
+raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
+danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
+tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
+                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289 ## Some
 video tutorials - https://www.youtube.com/watch?v=3xqwpXjxyMQ - https://
 www.youtube.com/watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=Ai-
 BS_T7yjE - https://www.youtube.com/watch?v=dFKRGXdkGJU - https://
 www.youtube.com/watch?v=D7W-C0urVcQ ## References - https://arxiv.org/pdf/
 2005.09007.pdf - https://github.com/NathanUA/U-2-Net - https://github.com/
```

### Comparing `rembg-2.0.32/README.md` & `rembg-2.0.33/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,20 @@
 
 Remove the background applying an alpha matting
 
 ```
 rembg i -a path/to/input.png path/to/output.png
 ```
 
+Passing extras parameters
+
+```
+rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -239,15 +245,15 @@
 
     with open(input_path, 'rb') as i:
         with open(output_path, 'wb') as o:
             input = i.read()
             output = remove(input, session=session)
             o.write(output)
 ```
-
+To see a full list of examples on how to use rembg, go to the [examples](USAGE.md) page.
 ## Usage as a docker
 
 Just replace the `rembg` command for `docker run danielgatis/rembg`.
 
 Try this:
 
 ```
@@ -262,43 +268,47 @@
 
 -   u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
 -   u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
 -   u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
 -   u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
+-   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### Some differences between the models result
 
 <table>
     <tr>
         <th>original</th>
         <th>u2net</th>
         <th>u2netp</th>
         <th>u2net_human_seg</th>
         <th>u2net_cloth_seg</th>
         <th>silueta</th>
         <th>isnet-general-use</th>
+        <th>sam</th>
     </tr>
     <tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/car-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.sam.png" width="100" /></th>
     </tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/cloth-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.sam.png" width="100" /></th>
     </tr>
 </table>
 
 
 ### How to train your own model
 
 If You need more fine tunned models try this:
```

#### html2text {}

```diff
@@ -47,21 +47,23 @@
 using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
 files. Remove the background from a remote image ``` curl -s http://input.png |
 rembg i > output.png ``` Remove the background from a local file ``` rembg i
 path/to/input.png path/to/output.png ``` Remove the background specifying a
 model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
 background returning only the mask ``` rembg i -om path/to/input.png path/to/
 output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` ### rembg `p` Used when input and
-output are folders. Remove the background from all images in a folder ``` rembg
-p path/to/input path/to/output ``` Same as before, but watching for new/changed
-files to process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s`
-Used to start http server. To see the complete endpoints documentation, go to:
-`http://localhost:5000/docs`. Remove the background from an image url ``` curl
--s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
+a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
+i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
+input.png path/to/output.png ``` ### rembg `p` Used when input and output are
+folders. Remove the background from all images in a folder ``` rembg p path/to/
+input path/to/output ``` Same as before, but watching for new/changed files to
+process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
+start http server. To see the complete endpoints documentation, go to: `http://
+localhost:5000/docs`. Remove the background from an image url ``` curl -
+s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
 background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
 "http://localhost:5000" -o output.png ``` ## Usage as a library Input and
 output as bytes ```python from rembg import remove input_path = 'input.png'
 output_path = 'output.png' with open(input_path, 'rb') as i: with open
 (output_path, 'wb') as o: input = i.read() output = remove(input) o.write
 (output) ``` Input and output as a PIL image ```python from rembg import remove
 from PIL import Image input_path = 'input.png' output_path = 'output.png' input
@@ -70,43 +72,49 @@
 input_path = 'input.png' output_path = 'output.png' input = cv2.imread
 (input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
 iterate over files in a performatic way ```python from pathlib import Path from
 rembg import remove, new_session session = new_session() for file in Path
 ('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
 (file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
 open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` ## Usage as a docker Just replace the
-`rembg` command for `docker run danielgatis/rembg`. Try this: ``` docker run
-danielgatis/rembg i path/to/input.png path/to/output.png ``` ## Models All
-models are downloaded and saved in the user home folder in the `.u2net`
-directory. The available models are: - u2net ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://
-github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases. -
-u2netp ([download](https://github.com/danielgatis/rembg/releases/download/
-v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
-lightweight version of u2net model. - u2net_human_seg ([download](https://
+session=session) o.write(output) ``` To see a full list of examples on how to
+use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
+replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
+docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
+Models All models are downloaded and saved in the user home folder in the
+`.u2net` directory. The available models are: - u2net ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
+cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
+A lightweight version of u2net model. - u2net_human_seg ([download](https://
 github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
 [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
 segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
 rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
 github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
 Parsing from human portrait. Here clothes are parsed into 3 category: Upper
 body, Lower body and Full body. - silueta ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
 github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
 reduced to 43Mb. - isnet-general-use ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
 (https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. ### Some differences between the models result
-original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use
-[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
-raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
-danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
-tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet-
-                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]
+cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
+quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
+pre-trained model for any use cases. ### Some differences between the models
+result
+original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
+[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
+raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
+danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
+tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
+                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289 ## Some
 video tutorials - https://www.youtube.com/watch?v=3xqwpXjxyMQ - https://
 www.youtube.com/watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=Ai-
 BS_T7yjE - https://www.youtube.com/watch?v=dFKRGXdkGJU - https://
 www.youtube.com/watch?v=D7W-C0urVcQ ## References - https://arxiv.org/pdf/
 2005.09007.pdf - https://github.com/NathanUA/U-2-Net - https://github.com/
```

### Comparing `rembg-2.0.32/rembg/bg.py` & `rembg-2.0.33/rembg/bg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 from enum import Enum
-from typing import List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
 from cv2 import (
     BORDER_DEFAULT,
     MORPH_ELLIPSE,
     MORPH_OPEN,
     GaussianBlur,
@@ -14,16 +14,16 @@
 from PIL import Image
 from PIL.Image import Image as PILImage
 from pymatting.alpha.estimate_alpha_cf import estimate_alpha_cf
 from pymatting.foreground.estimate_foreground_ml import estimate_foreground_ml
 from pymatting.util.util import stack_images
 from scipy.ndimage import binary_erosion
 
-from .session_base import BaseSession
 from .session_factory import new_session
+from .sessions.base import BaseSession
 
 kernel = getStructuringElement(MORPH_ELLIPSE, (3, 3))
 
 
 class ReturnType(Enum):
     BYTES = 0
     PILLOW = 1
@@ -119,31 +119,33 @@
     alpha_matting_foreground_threshold: int = 240,
     alpha_matting_background_threshold: int = 10,
     alpha_matting_erode_size: int = 10,
     session: Optional[BaseSession] = None,
     only_mask: bool = False,
     post_process_mask: bool = False,
     bgcolor: Optional[Tuple[int, int, int, int]] = None,
+    *args: Optional[Any],
+    **kwargs: Optional[Any]
 ) -> Union[bytes, PILImage, np.ndarray]:
     if isinstance(data, PILImage):
         return_type = ReturnType.PILLOW
         img = data
     elif isinstance(data, bytes):
         return_type = ReturnType.BYTES
         img = Image.open(io.BytesIO(data))
     elif isinstance(data, np.ndarray):
         return_type = ReturnType.NDARRAY
         img = Image.fromarray(data)
     else:
         raise ValueError("Input type {} is not supported.".format(type(data)))
 
     if session is None:
-        session = new_session("u2net")
+        session = new_session("u2net", *args, **kwargs)
 
-    masks = session.predict(img)
+    masks = session.predict(img, *args, **kwargs)
     cutouts = []
 
     for mask in masks:
         if post_process_mask:
             mask = Image.fromarray(post_process(np.array(mask)))
 
         if only_mask:
```

### Comparing `rembg-2.0.32/rembg/session_simple.py` & `rembg-2.0.33/rembg/sessions/dis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,47 @@
+import os
 from typing import List
 
 import numpy as np
+import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
-from .session_base import BaseSession
+from .base import BaseSession
 
 
-class SimpleSession(BaseSession):
-    def predict(self, img: PILImage) -> List[PILImage]:
+class DisSession(BaseSession):
+    def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
-            self.normalize(
-                img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
-            ),
+            self.normalize(img, (0.485, 0.456, 0.406), (1.0, 1.0, 1.0), (1024, 1024)),
         )
 
         pred = ort_outs[0][:, 0, :, :]
 
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
+
+    @classmethod
+    def download_models(cls, *args, **kwargs):
+        fname = f"{cls.name()}.onnx"
+        pooch.retrieve(
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx",
+            "md5:fc16ebd8b0c10d971d3513d564d01e29",
+            fname=fname,
+            path=cls.u2net_home(),
+            progressbar=True,
+        )
+
+        return os.path.join(cls.u2net_home(), fname)
+
+    @classmethod
+    def name(cls, *args, **kwargs):
+        return "isnet-general-use"
```

### Comparing `rembg-2.0.32/rembg.egg-info/PKG-INFO` & `rembg-2.0.33/rembg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.32
+Version: 2.0.33
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -169,14 +169,20 @@
 
 Remove the background applying an alpha matting
 
 ```
 rembg i -a path/to/input.png path/to/output.png
 ```
 
+Passing extras parameters
+
+```
+rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -266,15 +272,15 @@
 
     with open(input_path, 'rb') as i:
         with open(output_path, 'wb') as o:
             input = i.read()
             output = remove(input, session=session)
             o.write(output)
 ```
-
+To see a full list of examples on how to use rembg, go to the [examples](USAGE.md) page.
 ## Usage as a docker
 
 Just replace the `rembg` command for `docker run danielgatis/rembg`.
 
 Try this:
 
 ```
@@ -289,43 +295,47 @@
 
 -   u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
 -   u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
 -   u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
 -   u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
+-   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### Some differences between the models result
 
 <table>
     <tr>
         <th>original</th>
         <th>u2net</th>
         <th>u2netp</th>
         <th>u2net_human_seg</th>
         <th>u2net_cloth_seg</th>
         <th>silueta</th>
         <th>isnet-general-use</th>
+        <th>sam</th>
     </tr>
     <tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/car-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/car-1.sam.png" width="100" /></th>
     </tr>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/fixtures/cloth-1.jpg" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2netp.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_human_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.u2net_cloth_seg.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.silueta.png" width="100" /></th>
         <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.isnet-general-use.png" width="100" /></th>
+        <th><img src="https://raw.githubusercontent.com/danielgatis/rembg/master/tests/results/cloth-1.sam.png" width="100" /></th>
     </tr>
 </table>
 
 
 ### How to train your own model
 
 If You need more fine tunned models try this:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.32 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.33 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -61,21 +61,23 @@
 using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
 files. Remove the background from a remote image ``` curl -s http://input.png |
 rembg i > output.png ``` Remove the background from a local file ``` rembg i
 path/to/input.png path/to/output.png ``` Remove the background specifying a
 model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
 background returning only the mask ``` rembg i -om path/to/input.png path/to/
 output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` ### rembg `p` Used when input and
-output are folders. Remove the background from all images in a folder ``` rembg
-p path/to/input path/to/output ``` Same as before, but watching for new/changed
-files to process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s`
-Used to start http server. To see the complete endpoints documentation, go to:
-`http://localhost:5000/docs`. Remove the background from an image url ``` curl
--s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
+a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
+i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
+input.png path/to/output.png ``` ### rembg `p` Used when input and output are
+folders. Remove the background from all images in a folder ``` rembg p path/to/
+input path/to/output ``` Same as before, but watching for new/changed files to
+process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
+start http server. To see the complete endpoints documentation, go to: `http://
+localhost:5000/docs`. Remove the background from an image url ``` curl -
+s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
 background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
 "http://localhost:5000" -o output.png ``` ## Usage as a library Input and
 output as bytes ```python from rembg import remove input_path = 'input.png'
 output_path = 'output.png' with open(input_path, 'rb') as i: with open
 (output_path, 'wb') as o: input = i.read() output = remove(input) o.write
 (output) ``` Input and output as a PIL image ```python from rembg import remove
 from PIL import Image input_path = 'input.png' output_path = 'output.png' input
@@ -84,43 +86,49 @@
 input_path = 'input.png' output_path = 'output.png' input = cv2.imread
 (input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
 iterate over files in a performatic way ```python from pathlib import Path from
 rembg import remove, new_session session = new_session() for file in Path
 ('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
 (file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
 open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` ## Usage as a docker Just replace the
-`rembg` command for `docker run danielgatis/rembg`. Try this: ``` docker run
-danielgatis/rembg i path/to/input.png path/to/output.png ``` ## Models All
-models are downloaded and saved in the user home folder in the `.u2net`
-directory. The available models are: - u2net ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://
-github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases. -
-u2netp ([download](https://github.com/danielgatis/rembg/releases/download/
-v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
-lightweight version of u2net model. - u2net_human_seg ([download](https://
+session=session) o.write(output) ``` To see a full list of examples on how to
+use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
+replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
+docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
+Models All models are downloaded and saved in the user home folder in the
+`.u2net` directory. The available models are: - u2net ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
+cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
+A lightweight version of u2net model. - u2net_human_seg ([download](https://
 github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
 [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
 segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
 rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
 github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
 Parsing from human portrait. Here clothes are parsed into 3 category: Upper
 body, Lower body and Full body. - silueta ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
 github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
 reduced to 43Mb. - isnet-general-use ([download](https://github.com/
 danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
 (https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. ### Some differences between the models result
-original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use
-[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
-raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
-danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
-tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet-
-                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]
+cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
+quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
+pre-trained model for any use cases. ### Some differences between the models
+result
+original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
+[https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
+raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
+danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
+tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
+                           1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289 ## Some
 video tutorials - https://www.youtube.com/watch?v=3xqwpXjxyMQ - https://
 www.youtube.com/watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=Ai-
 BS_T7yjE - https://www.youtube.com/watch?v=dFKRGXdkGJU - https://
 www.youtube.com/watch?v=D7W-C0urVcQ ## References - https://arxiv.org/pdf/
 2005.09007.pdf - https://github.com/NathanUA/U-2-Net - https://github.com/
```

### Comparing `rembg-2.0.32/setup.py` & `rembg-2.0.33/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,40 +30,40 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="remove, background, u2net",
-    packages=["rembg"],
+    packages=["rembg", "rembg.sessions", "rembg.commands"],
     python_requires=">3.7, <3.11",
     install_requires=[
         "aiohttp>=3.8.1",
         "asyncer>=0.0.2",
         "click>=8.1.3",
         "fastapi>=0.92.0",
         "filetype>=1.2.0",
-        "pooch>=1.6.0",
         "imagehash>=4.3.1",
         "numpy>=1.23.5",
-        "onnxruntime>=1.13.1",
+        "onnxruntime>=1.14.1",
         "opencv-python-headless>=4.6.0.66",
         "pillow>=9.3.0",
+        "pooch>=1.6.0",
         "pymatting>=1.1.8",
         "python-multipart>=0.0.5",
         "scikit-image>=0.19.3",
         "scipy>=1.9.3",
         "tqdm>=4.64.1",
         "uvicorn>=0.20.0",
         "watchdog>=2.1.9",
     ],
     entry_points={
         "console_scripts": [
             "rembg=rembg.cli:main",
         ],
     },
     extras_require={
-        "gpu": ["onnxruntime-gpu>=1.13.1"],
+        "gpu": ["onnxruntime-gpu>=1.14.1"],
     },
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `rembg-2.0.32/versioneer.py` & `rembg-2.0.33/versioneer.py`

 * *Files identical despite different names*

