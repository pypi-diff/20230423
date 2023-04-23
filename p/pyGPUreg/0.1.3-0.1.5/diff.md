# Comparing `tmp/pyGPUreg-0.1.3.tar.gz` & `tmp/pyGPUreg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGPUreg-0.1.3.tar", last modified: Thu Apr 20 15:04:29 2023, max compression
+gzip compressed data, was "dist\pyGPUreg-0.1.5.tar", last modified: Sun Apr 23 09:35:05 2023, max compression
```

## Comparing `pyGPUreg-0.1.3.tar` & `pyGPUreg-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/
--rw-rw-rw-   0        0        0    17099 2023-03-23 08:54:10.000000 pyGPUreg-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       73 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4777 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.180385 pyGPUreg-0.1.3/pyGPUreg/
--rw-rw-rw-   0        0        0      114 2023-04-20 15:04:22.000000 pyGPUreg-0.1.3/pyGPUreg/__init__.py
--rw-rw-rw-   0        0        0     5995 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/opengl_classes.py
--rw-rw-rw-   0        0        0    28476 2023-04-20 15:04:19.000000 pyGPUreg-0.1.3/pyGPUreg/pyGPUreg.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/pyGPUreg/shaders/
--rw-rw-rw-   0        0        0     1477 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/butterflytexture.glsl
--rw-rw-rw-   0        0        0      398 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/copy_r_to_rg.glsl
--rw-rw-rw-   0        0        0      392 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/cos_filter.glsl
--rw-rw-rw-   0        0        0      404 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/cos_filter_r.glsl
--rw-rw-rw-   0        0        0     3377 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft.glsl
--rw-rw-rw-   0        0        0      746 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation.glsl
--rw-rw-rw-   0        0        0      458 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
--rw-rw-rw-   0        0        0      532 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation.glsl
--rw-rw-rw-   0        0        0      582 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation_single.glsl
--rw-rw-rw-   0        0        0     2802 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_single.glsl
--rw-rw-rw-   0        0        0      805 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/resample_image.glsl
-drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.196013 pyGPUreg-0.1.3/pyGPUreg.egg-info/
--rw-rw-rw-   0        0        0      274 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-04-20 15:04:24.000000 pyGPUreg-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:35:05.650521 pyGPUreg-0.1.5/
+-rw-rw-rw-   0        0        0    17099 2023-03-23 17:28:06.000000 pyGPUreg-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       73 2023-03-21 07:44:45.000000 pyGPUreg-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      292 2023-04-23 09:35:05.650521 pyGPUreg-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4777 2023-04-23 09:15:41.000000 pyGPUreg-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 09:35:05.618521 pyGPUreg-0.1.5/pyGPUreg/
+-rw-rw-rw-   0        0        0      114 2023-04-23 09:35:02.000000 pyGPUreg-0.1.5/pyGPUreg/__init__.py
+-rw-rw-rw-   0        0        0     5995 2023-03-18 12:08:18.000000 pyGPUreg-0.1.5/pyGPUreg/opengl_classes.py
+-rw-rw-rw-   0        0        0    28490 2023-04-23 09:33:38.000000 pyGPUreg-0.1.5/pyGPUreg/pyGPUreg.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:35:05.646520 pyGPUreg-0.1.5/pyGPUreg/shaders/
+-rw-rw-rw-   0        0        0     1477 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/butterflytexture.glsl
+-rw-rw-rw-   0        0        0      398 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/copy_r_to_rg.glsl
+-rw-rw-rw-   0        0        0      392 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/cos_filter.glsl
+-rw-rw-rw-   0        0        0      404 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/cos_filter_r.glsl
+-rw-rw-rw-   0        0        0     3377 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft.glsl
+-rw-rw-rw-   0        0        0      746 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft_inversion_permutation.glsl
+-rw-rw-rw-   0        0        0      458 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
+-rw-rw-rw-   0        0        0      532 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft_phase_correlation.glsl
+-rw-rw-rw-   0        0        0      582 2023-04-23 09:15:41.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft_phase_correlation_single.glsl
+-rw-rw-rw-   0        0        0     2802 2023-03-22 20:19:01.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/fft_single.glsl
+-rw-rw-rw-   0        0        0      805 2023-04-23 09:15:41.000000 pyGPUreg-0.1.5/pyGPUreg/shaders/resample_image.glsl
+drwxrwxrwx   0        0        0        0 2023-04-23 09:35:05.626521 pyGPUreg-0.1.5/pyGPUreg.egg-info/
+-rw-rw-rw-   0        0        0      292 2023-04-23 09:35:05.000000 pyGPUreg-0.1.5/pyGPUreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-23 09:35:05.000000 pyGPUreg-0.1.5/pyGPUreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:35:05.000000 pyGPUreg-0.1.5/pyGPUreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-23 09:35:05.000000 pyGPUreg-0.1.5/pyGPUreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 09:35:05.000000 pyGPUreg-0.1.5/pyGPUreg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 09:35:05.650521 pyGPUreg-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-04-23 09:35:02.000000 pyGPUreg-0.1.5/setup.py
```

### Comparing `pyGPUreg-0.1.3/LICENSE.txt` & `pyGPUreg-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/README.md` & `pyGPUreg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/opengl_classes.py` & `pyGPUreg-0.1.5/pyGPUreg/opengl_classes.py`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/pyGPUreg.py` & `pyGPUreg-0.1.5/pyGPUreg/pyGPUreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     glfw.window_hint(glfw.CONTEXT_VERSION_MINOR, GLFW_CONTEXT_VERSION_MINOR)
     glfw.window_hint(glfw.OPENGL_PROFILE, glfw.OPENGL_CORE_PROFILE)
     glfw.window_hint(glfw.OPENGL_FORWARD_COMPAT, GL_TRUE)
     window = glfw.create_window(2, 2, "pyGPUreg hidden window", None, None)
     glfw.make_context_current(window)
 
     # compile shaders
-    shader_dir = os.path.join(os.path.dirname(__file__), "shaders")
+    shader_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)),"shaders")
     cs_butterfly = Shader(os.path.join(shader_dir, "butterflytexture.glsl"))
     cs_cosft = Shader(os.path.join(shader_dir, "cos_filter.glsl"))
     cs_fft = Shader(os.path.join(shader_dir, "fft.glsl"))
     cs_fft_pi = Shader(os.path.join(shader_dir, "fft_inversion_permutation.glsl"))
     cs_multiply = Shader(os.path.join(shader_dir, "fft_phase_correlation.glsl"))
     cs_resample = Shader(os.path.join(shader_dir, "resample_image.glsl"))
     cs_fft_single = Shader(os.path.join(shader_dir, "fft_single.glsl"))
@@ -575,8 +575,7 @@
             glfw.make_context_current(previous_context)
         return dx, dy
 
     resampled = sample_texture_with_shift(texture_r_i, (dx, dy), edge_mode, interpolation_mode)
     if window is not None:
         glfw.make_context_current(previous_context)
     return resampled, (dx, dy)
-
```

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/butterflytexture.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/butterflytexture.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/fft.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/fft.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/fft_inversion_permutation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/fft_phase_correlation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation_single.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/fft_phase_correlation_single.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_single.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/fft_single.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg/shaders/resample_image.glsl` & `pyGPUreg-0.1.5/pyGPUreg/shaders/resample_image.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/pyGPUreg.egg-info/SOURCES.txt` & `pyGPUreg-0.1.5/pyGPUreg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.3/setup.py` & `pyGPUreg-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyGPUreg',
-    version='0.1.3',
+    version='0.1.5',
     license='GPLv3',
     author="Mart G.F. Last",
     author_email='m.g.f.last@lumc.nl',
     description='GPU-accelerated image registration.\ngithub.com/bionanopatterning/pyGPUreg',
     packages=find_packages(),
     package_data={'pyGPUreg': ['*.glsl', 'shaders/*glsl']},
     include_package_data=True,
```

