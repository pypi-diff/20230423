# Comparing `tmp/lecture-automator-0.1.1.tar.gz` & `tmp/lecture-automator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture-automator-0.1.1.tar", max compression
+gzip compressed data, was "lecture-automator-0.2.0.tar", max compression
```

## Comparing `lecture-automator-0.1.1.tar` & `lecture-automator-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1140 2023-04-13 20:31:53.497325 lecture-automator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.1.1/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0      831 2023-04-11 18:02:48.539135 lecture-automator-0.1.1/src/lecture_automator/cli.py
--rw-r--r--   0        0        0     1934 2023-04-11 16:44:42.058381 lecture-automator-0.1.1/src/lecture_automator/gen_speech.py
--rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.1.1/src/lecture_automator/gen_video.py
--rw-r--r--   0        0        0     1051 2023-04-13 20:31:53.497573 lecture-automator-0.1.1/src/lecture_automator/marp_api.py
--rw-r--r--   0        0        0     2430 2023-04-11 18:00:24.487850 lecture-automator-0.1.1/src/lecture_automator/parser.py
--rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.1.1/src/lecture_automator/settings.py
--rw-r--r--   0        0        0      904 2023-04-13 20:36:27.090350 lecture-automator-0.1.1/setup.py
--rw-r--r--   0        0        0      534 2023-04-13 20:36:27.090498 lecture-automator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2209 2023-04-23 14:22:41.590194 lecture-automator-0.2.0/README.md
+-rw-r--r--   0        0        0     1224 2023-04-23 14:22:41.590664 lecture-automator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.2.0/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0     1273 2023-04-23 14:22:41.590863 lecture-automator-0.2.0/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0     1393 2023-04-23 14:22:41.591129 lecture-automator-0.2.0/src/lecture_automator/command_handler.py
+-rw-r--r--   0        0        0     1934 2023-04-11 16:44:42.058381 lecture-automator-0.2.0/src/lecture_automator/gen_speech.py
+-rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.2.0/src/lecture_automator/gen_video.py
+-rw-r--r--   0        0        0     1089 2023-04-23 14:22:41.591679 lecture-automator-0.2.0/src/lecture_automator/marp_api.py
+-rw-r--r--   0        0        0     4492 2023-04-23 14:22:41.591888 lecture-automator-0.2.0/src/lecture_automator/parser.py
+-rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.2.0/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0     3209 2023-04-23 14:22:57.699255 lecture-automator-0.2.0/setup.py
+-rw-r--r--   0        0        0     2846 2023-04-23 14:22:57.699481 lecture-automator-0.2.0/PKG-INFO
```

### Comparing `lecture-automator-0.1.1/pyproject.toml` & `lecture-automator-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "lecture-automator"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["CapBlood <stalker.anonim@mail.ru>"]
+readme = "README.md"
+homepage = "https://github.com/CapBlood/lecture-automator.git"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ffmpeg-python = "^0.2.0"
 torch = "^2.0.0"
 numpy = "^1.24.2"
 click = "^8.1.3"
```

### Comparing `lecture-automator-0.1.1/src/lecture_automator/gen_speech.py` & `lecture-automator-0.2.0/src/lecture_automator/gen_speech.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.1.1/src/lecture_automator/gen_video.py` & `lecture-automator-0.2.0/src/lecture_automator/gen_video.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.1.1/src/lecture_automator/marp_api.py` & `lecture-automator-0.2.0/src/lecture_automator/marp_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import subprocess
 import tempfile
 import os
 
 
-def generate_marp_slides(outdir: str, md_text: str, type_images: str = 'png') -> None:
+def generate_marp_slides(outdir: str, md_text: str, type_images: str = 'png', scale: float = 2.0) -> None:
     """Генерация слайдов презентации Marp в виде набора изображений.
 
     Args:
         outdir (str): директория для сохранения изображений.
         md_text (str): текст файла Markdown презентации Marp.
         type_images (str, optional): Формат изображений (png или jpeg). Defaults to 'png'.
     """
 
     with tempfile.TemporaryDirectory() as tmpdirname:
         path_to_md = os.path.join(tmpdirname, "input.md")
         with open(path_to_md, "w") as file:
             file.write(md_text)
 
         subprocess.run(
-            ['marp', '--images', type_images, '--image-scale', '2', '-o', 'Slide.png', path_to_md],
+            ['marp', '--images', type_images, '--image-scale', str(scale), '-o', 'Slide.png', path_to_md],
             cwd=outdir
         )
 
 
 if __name__ == '__main__':
     with open('examples/Example.md') as file:
         text = file.read()
 
-    generate_marp_slides('examples', text)
+    generate_marp_slides('examples', text, scale=1.5)
```

