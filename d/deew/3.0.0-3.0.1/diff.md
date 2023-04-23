# Comparing `tmp/deew-3.0.0.tar.gz` & `tmp/deew-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deew-3.0.0.tar", max compression
+gzip compressed data, was "deew-3.0.1.tar", max compression
```

## Comparing `deew-3.0.0.tar` & `deew-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    46890 2023-04-22 13:55:31.689447 deew-3.0.0/deew/__main__.py
--rw-r--r--   0        0        0     1125 2023-04-22 13:55:31.689447 deew-3.0.0/deew/bitrates.py
--rw-r--r--   0        0        0     9112 2023-04-22 13:55:31.689447 deew-3.0.0/deew/logos.py
--rw-r--r--   0        0        0     2450 2023-04-22 13:55:31.689447 deew-3.0.0/deew/messages.py
--rw-r--r--   0        0        0    11603 2023-04-22 13:55:31.689447 deew-3.0.0/deew/xml_base.py
--rw-r--r--   0        0        0     1086 2023-04-22 13:55:31.673805 deew-3.0.0/LICENSE
--rw-r--r--   0        0        0      593 2023-04-22 13:55:31.689447 deew-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    10120 2023-04-22 13:55:31.673805 deew-3.0.0/README.md
--rw-r--r--   0        0        0    10814 1970-01-01 00:00:00.000000 deew-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    46890 2023-04-23 10:37:02.845011 deew-3.0.1/deew/__main__.py
+-rw-r--r--   0        0        0     1125 2023-04-23 10:37:02.845011 deew-3.0.1/deew/bitrates.py
+-rw-r--r--   0        0        0     9112 2023-04-23 10:37:02.845011 deew-3.0.1/deew/logos.py
+-rw-r--r--   0        0        0     2482 2023-04-23 10:37:02.845011 deew-3.0.1/deew/messages.py
+-rw-r--r--   0        0        0    11603 2023-04-23 10:37:02.845011 deew-3.0.1/deew/xml_base.py
+-rw-r--r--   0        0        0     1086 2023-04-23 10:37:02.845011 deew-3.0.1/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-23 10:37:02.845011 deew-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10120 2023-04-23 10:37:02.845011 deew-3.0.1/README.md
+-rw-r--r--   0        0        0    10814 1970-01-01 00:00:00.000000 deew-3.0.1/PKG-INFO
```

### Comparing `deew-3.0.0/deew/__main__.py` & `deew-3.0.1/deew/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 from deew.bitrates import allowed_bitrates
 from deew.logos import logos
 from deew.messages import error_messages
 from deew.xml_base import xml_dd_ddp_base, xml_thd_base, xml_ac4_base
 
 prog_name = 'deew'
-prog_version = '3.0.0'
+prog_version = '3.0.1'
 
 simplens = SimpleNamespace()
 
 
 class RParse(argparse.ArgumentParser):
     def _print_message(self, message, file=None):
         if message:
```

### Comparing `deew-3.0.0/deew/bitrates.py` & `deew-3.0.1/deew/bitrates.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,9 +4,9 @@
     'dd_51': [224, 256, 320, 384, 448, 512, 576, 640],
     'ddp_10': [32, 40, 48, 56, 64, 72, 80, 88, 96, 104, 112, 120, 128, 144, 160, 176, 192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_20': [96, 104, 112, 120, 128, 144, 160, 176, 192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_51': [192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_71_standard': [384, 448, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_71_bluray': [768, 1024, 1280, 1536, 1664],
     'ddp_71_combined': [384, 448, 576, 640, 704, 768, 832, 896, 960, 1008, 1024, 1280, 1536, 1664],
-    'ac4_20': [64, 72, 114, 144, 256, 320],
+    'ac4_20': [64, 72, 112, 144, 256, 320],
 }
```

### Comparing `deew-3.0.0/deew/logos.py` & `deew-3.0.1/deew/logos.py`

 * *Files identical despite different names*

### Comparing `deew-3.0.0/deew/messages.py` & `deew-3.0.1/deew/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 error_messages = {
     'changelog'         : 'couldn\'t fetch changelog from GitHub.',
     'delay'             : 'unsupported delay value.',
     'wsl_path'          : 'WSL path conversion doesn\'t work with [bold yellow]🤠[/bold yellow].',
     'create_dir'        : 'failed to create [bold yellow]🤠[/bold yellow].',
-    'format'            : '[bold yellow]-f[/bold yellow]/[bold yellow]--format[/bold yellow] can only be [bold yellow]dd[/bold yellow], [bold yellow]ddp[/bold yellow] or [bold yellow]thd[/bold yellow].',
+    'format'            : '[bold yellow]-f[/bold yellow]/[bold yellow]--format[/bold yellow] can only be [bold yellow]dd[/bold yellow], [bold yellow]ddp[/bold yellow], [bold yellow]ac4[/bold yellow] or [bold yellow]thd[/bold yellow].',
     'downmix'           : '[bold yellow]-dm[/bold yellow]/[bold yellow]--downmix[/bold yellow] can only be [bold yellow]1[/bold yellow], [bold yellow]2[/bold yellow] or [bold yellow]6[/bold yellow].',
     'downmix_mismatch'  : 'downmix value has to be lower than the number of input channels.',
     'thd_downmix'       : '[bold yellow]-m[/bold yellow]/[bold yellow]--mix[/bold yellow] can only be used for [bold yellow]DD[/bold yellow]/[bold yellow]DDP[/bold yellow] encoding.',
     'thd_mono_input'    : 'input channels for TrueHD encoding can only be [bold yellow]2[/bold yellow]/[bold yellow]6[/bold yellow]/[bold yellow]8[/bold yellow]. ',
     'drc'               : 'allowed DRC values: [bold yellow]film_light[/bold yellow], [bold yellow]film_standard[/bold yellow], [bold yellow]music_light[/bold yellow], [bold yellow]music_standard[/bold yellow], [bold yellow]speech[/bold yellow].',
     'linux_thd'         : 'Linux version of DEE does not support TrueHD encoding.',
     'path'              : 'path [bold yellow]🤠[/bold yellow] does not exist.',
```

### Comparing `deew-3.0.0/deew/xml_base.py` & `deew-3.0.1/deew/xml_base.py`

 * *Files identical despite different names*

### Comparing `deew-3.0.0/LICENSE` & `deew-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deew-3.0.0/pyproject.toml` & `deew-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "deew"
-version = "3.0.0"
+version = "3.0.1"
 readme = 'README.md'
 description = "Dolby Encoding Engine Wrapper"
 authors = ["pcroland <pcroland@protonmail.ch>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
```

### Comparing `deew-3.0.0/README.md` & `deew-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 PATH="/usr/local/bin/dee:$PATH"
 PATH="/usr/local/bin/ffmpeg:$PATH"
 ```
 
 # Usage
 ```
 ❯ deew -h
-deew 3.0.0
+deew 3.0.1
 
 USAGE: deew [-h] [-v] [-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT]
             [-b BITRATE] [-dm CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM]
             [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-np] [-pl]
             [-cl] [-c] [-gc]
 
 FLAGS:
```

#### html2text {}

```diff
@@ -76,15 +76,15 @@
 variables ### Windows: - open `cmd.exe` as administrator - run a `setx /m PATH
 "%PATH%;[location]"` command for each path that contains binaries\ *(replace* `
 [location]` *with the path)* - for example: ```bat setx /m PATH "%PATH%;C:
 \bin\dee" setx /m PATH "%PATH%;C:\bin\ffmpeg" ``` ### Linux/macOS: - add a
 `PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each
 path that contains a binary\ *(replace* `[location]` *with the path)* - for
 example: ```sh PATH="/usr/local/bin/dee:$PATH" PATH="/usr/local/bin/ffmpeg:
-$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.0 USAGE: deew [-h] [-v] [-i [INPUT
+$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.1 USAGE: deew [-h] [-v] [-i [INPUT
 ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT] [-b BITRATE] [-dm CHANNELS] [-
 d DELAY] [-r DRC] [-dn DIALNORM] [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb]
 [-la] [-np] [-pl] [-cl] [-c] [-gc] FLAGS: -h, --help show this help message. -
 v, --version show version. -i, --input [INPUT ...] audio file(s) or folder(s) -
 ti, --track-index INDEX default: 0 select audio track index of input(s) -o, --
 output DIRECTORY default: current directory specifies output directory -f, --
 format FORMAT options: dd / ddp / ac4 / thd default: ddp -b, --bitrate BITRATE
```

### Comparing `deew-3.0.0/PKG-INFO` & `deew-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deew
-Version: 3.0.0
+Version: 3.0.1
 Summary: Dolby Encoding Engine Wrapper
 License: MIT
 Author: pcroland
 Author-email: pcroland@protonmail.ch
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -117,15 +117,15 @@
 PATH="/usr/local/bin/dee:$PATH"
 PATH="/usr/local/bin/ffmpeg:$PATH"
 ```
 
 # Usage
 ```
 ❯ deew -h
-deew 3.0.0
+deew 3.0.1
 
 USAGE: deew [-h] [-v] [-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT]
             [-b BITRATE] [-dm CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM]
             [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-np] [-pl]
             [-cl] [-c] [-gc]
 
 FLAGS:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deew Version: 3.0.0 Summary: Dolby Encoding Engine
+Metadata-Version: 2.1 Name: deew Version: 3.0.1 Summary: Dolby Encoding Engine
 Wrapper License: MIT Author: pcroland Author-email: pcroland@protonmail.ch
 Requires-Python: >=3.7,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Unidecode (>=1.3.4,<2.0.0) Requires-Dist: packaging
@@ -87,15 +87,15 @@
 variables ### Windows: - open `cmd.exe` as administrator - run a `setx /m PATH
 "%PATH%;[location]"` command for each path that contains binaries\ *(replace* `
 [location]` *with the path)* - for example: ```bat setx /m PATH "%PATH%;C:
 \bin\dee" setx /m PATH "%PATH%;C:\bin\ffmpeg" ``` ### Linux/macOS: - add a
 `PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each
 path that contains a binary\ *(replace* `[location]` *with the path)* - for
 example: ```sh PATH="/usr/local/bin/dee:$PATH" PATH="/usr/local/bin/ffmpeg:
-$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.0 USAGE: deew [-h] [-v] [-i [INPUT
+$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.1 USAGE: deew [-h] [-v] [-i [INPUT
 ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT] [-b BITRATE] [-dm CHANNELS] [-
 d DELAY] [-r DRC] [-dn DIALNORM] [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb]
 [-la] [-np] [-pl] [-cl] [-c] [-gc] FLAGS: -h, --help show this help message. -
 v, --version show version. -i, --input [INPUT ...] audio file(s) or folder(s) -
 ti, --track-index INDEX default: 0 select audio track index of input(s) -o, --
 output DIRECTORY default: current directory specifies output directory -f, --
 format FORMAT options: dd / ddp / ac4 / thd default: ddp -b, --bitrate BITRATE
```

