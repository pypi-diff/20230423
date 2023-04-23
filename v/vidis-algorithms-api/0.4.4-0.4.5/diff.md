# Comparing `tmp/vidis_algorithms_api-0.4.4.tar.gz` & `tmp/vidis_algorithms_api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidis_algorithms_api-0.4.4.tar", last modified: Fri Apr 21 13:43:53 2023, max compression
+gzip compressed data, was "vidis_algorithms_api-0.4.5.tar", last modified: Sun Apr 23 10:56:32 2023, max compression
```

## Comparing `vidis_algorithms_api-0.4.4.tar` & `vidis_algorithms_api-0.4.5.tar`

### file list

```diff
@@ -1,27 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.755903 vidis_algorithms_api-0.4.4/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 13:43:53.755903 vidis_algorithms_api-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.751903 vidis_algorithms_api-0.4.4/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.751903 vidis_algorithms_api-0.4.4/examples/dummy_example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.4.4/examples/dummy_example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.4/examples/dummy_example/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.751903 vidis_algorithms_api-0.4.4/examples/neural_network/
--rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.4/examples/neural_network/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.751903 vidis_algorithms_api-0.4.4/examples/neural_network/model/
--rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.4/examples/neural_network/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 13:43:53.755903 vidis_algorithms_api-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.751903 vidis_algorithms_api-0.4.4/vidis_algorithms_api/
--rw-rw-rw-   0 root         (0) root         (0)     1952 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api/Lifecycle.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api/Task.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.755903 vidis_algorithms_api-0.4.4/vidis_algorithms_api/core/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api/core/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:43:53.755903 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 13:43:53.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      571 2023-04-21 13:43:53.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:43:53.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 13:43:53.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-21 13:43:53.000000 vidis_algorithms_api-0.4.4/vidis_algorithms_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-23 10:45:55.000000 vidis_algorithms_api-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/Lifecycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-04-23 10:45:55.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/top_level.txt
```

### Comparing `vidis_algorithms_api-0.4.4/README.md` & `vidis_algorithms_api-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.4/setup.py` & `vidis_algorithms_api-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 
 def setup_package():
-    __version__ = '0.4.4'
+    __version__ = '0.4.5'
     url = 'https://github.com/Banayaki'
 
     setup(name='vidis_algorithms_api',
           description=description,
           version=__version__,
           url=url,
           license='MIT',
```

### Comparing `vidis_algorithms_api-0.4.4/vidis_algorithms_api/Lifecycle.py` & `vidis_algorithms_api-0.4.5/vidis_algorithms_api/Lifecycle.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.4/vidis_algorithms_api/Task.py` & `vidis_algorithms_api-0.4.5/vidis_algorithms_api/Task.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         path_to_save = os.path.join(settings.DATA_PATH, hypespecter_path,
                                     settings.CUSTOM_LAYER_FOLDER, f'{self.name}_{datetime.now()}.npy')
         os.makedirs(os.path.dirname(path_to_save), exist_ok=True)
         np.save(path_to_save, layer_data)
         return os.path.dirname(path_to_save)
         
 
-    def run(self, lname, hsi_id, _, hyperspecter_path, **kwargs):
+    def run(self, lname, hsi_id, hyperspecter_path, **kwargs):
         # Laye
         data = np.load(os.path.join(settings.DATA_PATH, hyperspecter_path, "hsi.npy"), mmap_mode="r")
         result = self.task(hyperspecter=data, **kwargs)
         assert result.ndim == 2, "Result should have two dimensions (height x width)"
         return self._save_task_result(result, hyperspecter_path)
     
     @abstractmethod
```

