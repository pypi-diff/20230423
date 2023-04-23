# Comparing `tmp/plttbc-0.2.3.tar.gz` & `tmp/plttbc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plttbc-0.2.3.tar", last modified: Sun Apr 23 14:57:48 2023, max compression
+gzip compressed data, was "plttbc-0.2.4.tar", last modified: Sun Apr 23 16:40:15 2023, max compression
```

## Comparing `plttbc-0.2.3.tar` & `plttbc-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 14:57:48.418230 plttbc-0.2.3/
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 14:57:48.402875 plttbc-0.2.3/.github/
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 14:57:48.410868 plttbc-0.2.3/.github/workflows/
--rw-r--r--   0 pavel      (501) staff       (20)      863 2023-04-23 12:41:43.000000 plttbc-0.2.3/.github/workflows/python-app.yml
--rw-r--r--   0 pavel      (501) staff       (20)      368 2023-04-23 11:36:14.000000 plttbc-0.2.3/.gitignore
--rw-r--r--   0 pavel      (501) staff       (20)     1091 2023-04-23 11:36:14.000000 plttbc-0.2.3/LICENSE.txt
--rw-r--r--   0 pavel      (501) staff       (20)     2551 2023-04-23 14:57:48.417217 plttbc-0.2.3/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     2335 2023-04-23 14:14:51.000000 plttbc-0.2.3/README.md
--rw-r--r--   0 pavel      (501) staff       (20)     1609 2023-04-23 11:36:14.000000 plttbc-0.2.3/README.txt
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 14:57:48.411538 plttbc-0.2.3/images/
--rw-r--r--   0 pavel      (501) staff       (20)    91844 2023-04-23 11:36:14.000000 plttbc-0.2.3/images/demo.png
--rw-r--r--   0 pavel      (501) staff       (20)     6276 2023-04-23 11:36:14.000000 plttbc-0.2.3/lttbc.c
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 14:57:48.415323 plttbc-0.2.3/plttbc.egg-info/
--rw-r--r--   0 pavel      (501) staff       (20)     2551 2023-04-23 14:57:48.000000 plttbc-0.2.3/plttbc.egg-info/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)      302 2023-04-23 14:57:48.000000 plttbc-0.2.3/plttbc.egg-info/SOURCES.txt
--rw-r--r--   0 pavel      (501) staff       (20)        1 2023-04-23 14:57:48.000000 plttbc-0.2.3/plttbc.egg-info/dependency_links.txt
--rw-r--r--   0 pavel      (501) staff       (20)        6 2023-04-23 14:57:48.000000 plttbc-0.2.3/plttbc.egg-info/requires.txt
--rw-r--r--   0 pavel      (501) staff       (20)        6 2023-04-23 14:57:48.000000 plttbc-0.2.3/plttbc.egg-info/top_level.txt
--rw-r--r--   0 pavel      (501) staff       (20)       14 2023-04-23 11:54:01.000000 plttbc-0.2.3/requirements.txt
--rw-r--r--   0 pavel      (501) staff       (20)       38 2023-04-23 14:57:48.418429 plttbc-0.2.3/setup.cfg
--rw-r--r--   0 pavel      (501) staff       (20)     1804 2023-04-23 14:50:31.000000 plttbc-0.2.3/setup.py
--rw-r--r--   0 pavel      (501) staff       (20)    10978 2023-04-23 11:36:14.000000 plttbc-0.2.3/test_downsample.py
--rw-r--r--   0 pavel      (501) staff       (20)      157 2023-04-23 11:36:14.000000 plttbc-0.2.3/tox.ini
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 16:40:15.170054 plttbc-0.2.4/
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 16:40:15.146744 plttbc-0.2.4/.github/
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 16:40:15.158858 plttbc-0.2.4/.github/workflows/
+-rw-r--r--   0 pavel      (501) staff       (20)      863 2023-04-23 12:41:43.000000 plttbc-0.2.4/.github/workflows/python-app.yml
+-rw-r--r--   0 pavel      (501) staff       (20)      368 2023-04-23 11:36:14.000000 plttbc-0.2.4/.gitignore
+-rw-r--r--   0 pavel      (501) staff       (20)     1091 2023-04-23 11:36:14.000000 plttbc-0.2.4/LICENSE.txt
+-rw-r--r--   0 pavel      (501) staff       (20)      941 2023-04-23 16:40:15.168221 plttbc-0.2.4/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     2335 2023-04-23 14:14:51.000000 plttbc-0.2.4/README.md
+-rw-r--r--   0 pavel      (501) staff       (20)     1609 2023-04-23 11:36:14.000000 plttbc-0.2.4/README.txt
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 16:40:15.160180 plttbc-0.2.4/images/
+-rw-r--r--   0 pavel      (501) staff       (20)    91844 2023-04-23 11:36:14.000000 plttbc-0.2.4/images/demo.png
+-rw-r--r--   0 pavel      (501) staff       (20)     6276 2023-04-23 11:36:14.000000 plttbc-0.2.4/lttbc.c
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-04-23 16:40:15.166707 plttbc-0.2.4/plttbc.egg-info/
+-rw-r--r--   0 pavel      (501) staff       (20)      941 2023-04-23 16:40:15.000000 plttbc-0.2.4/plttbc.egg-info/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)      317 2023-04-23 16:40:15.000000 plttbc-0.2.4/plttbc.egg-info/SOURCES.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        1 2023-04-23 16:40:15.000000 plttbc-0.2.4/plttbc.egg-info/dependency_links.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        6 2023-04-23 16:40:15.000000 plttbc-0.2.4/plttbc.egg-info/requires.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        6 2023-04-23 16:40:15.000000 plttbc-0.2.4/plttbc.egg-info/top_level.txt
+-rw-r--r--   0 pavel      (501) staff       (20)      137 2023-04-23 16:26:40.000000 plttbc-0.2.4/pyproject.toml
+-rw-r--r--   0 pavel      (501) staff       (20)       14 2023-04-23 11:54:01.000000 plttbc-0.2.4/requirements.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       38 2023-04-23 16:40:15.170373 plttbc-0.2.4/setup.cfg
+-rw-r--r--   0 pavel      (501) staff       (20)     1809 2023-04-23 16:39:43.000000 plttbc-0.2.4/setup.py
+-rw-r--r--   0 pavel      (501) staff       (20)    10978 2023-04-23 11:36:14.000000 plttbc-0.2.4/test_downsample.py
+-rw-r--r--   0 pavel      (501) staff       (20)      157 2023-04-23 11:36:14.000000 plttbc-0.2.4/tox.ini
```

### Comparing `plttbc-0.2.3/.github/workflows/python-app.yml` & `plttbc-0.2.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/LICENSE.txt` & `plttbc-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/README.md` & `plttbc-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/README.txt` & `plttbc-0.2.4/README.txt`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/images/demo.png` & `plttbc-0.2.4/images/demo.png`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/lttbc.c` & `plttbc-0.2.4/lttbc.c`

 * *Files identical despite different names*

### Comparing `plttbc-0.2.3/setup.py` & `plttbc-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from setuptools import Extension, setup
 
 
 def get_script_path():
     return osp.dirname(osp.realpath(sys.argv[0]))
 
 
-def read(*parts):
-    return open(osp.join(get_script_path(), *parts)).read()
+# def read(*parts):
+#     return open(osp.join(get_script_path(), *parts)).read()
 
 
 class numpy_get_include:
     def __str__(self):
         import numpy
         return numpy.get_include()
 
@@ -25,22 +25,22 @@
                      include_dirs=[numpy_get_include(),
                                    get_script_path()],
                      )
 
 setup(
     name="plttbc",
     author="Pavel Rabetski",
-    version="0.2.3",
+    version="0.2.4",
     #use_scm_version=True,
     ext_modules=[lttbc_py],
     author_email="rabeckijps@gmail.com",
     maintainer="Pavel Rabetski",
     url="https://github.com/pavradev/lttbc/",
     description="Largest triangle three buckets module for Python written in C",
-    long_description=read("README.txt"),
+    #long_description=read("README.txt"),
     long_description_content_type="text/markdown",
     license="MIT",
     install_requires=["numpy"],
     setup_requires=["setuptools_scm"],
     python_requires=">=3.5",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `plttbc-0.2.3/test_downsample.py` & `plttbc-0.2.4/test_downsample.py`

 * *Files identical despite different names*

