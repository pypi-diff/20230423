# Comparing `tmp/hti_index-0.1.2.tar.gz` & `tmp/hti_index-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hti_index-0.1.2.tar", last modified: Fri Apr 21 06:31:59 2023, max compression
+gzip compressed data, was "hti_index-0.1.3.tar", last modified: Sun Apr 23 13:00:25 2023, max compression
```

## Comparing `hti_index-0.1.2.tar` & `hti_index-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.180386 hti_index-0.1.2/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.2/LICENSE
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:31:59.180080 hti_index-0.1.2/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.2/README.md
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.178804 hti_index-0.1.2/hti_index/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      148 2023-04-21 06:22:58.000000 hti_index-0.1.2/hti_index/__init__.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3095 2023-04-20 00:12:09.000000 hti_index-0.1.2/hti_index/component.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2696 2023-04-20 00:20:10.000000 hti_index-0.1.2/hti_index/composite.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3041 2023-04-21 06:31:46.000000 hti_index-0.1.2/hti_index/flowfreq.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     5361 2023-04-21 05:32:49.000000 hti_index-0.1.2/hti_index/indexer.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-21 06:02:13.000000 hti_index-0.1.2/hti_index/utils.py
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.179839 hti_index-0.1.2/hti_index.egg-info/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      320 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/SOURCES.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/dependency_links.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/requires.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/top_level.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-21 06:31:59.180450 hti_index-0.1.2/setup.cfg
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-21 06:31:54.000000 hti_index-0.1.2/setup.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-23 13:00:25.738215 hti_index-0.1.3/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.3/LICENSE
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-23 13:00:25.737872 hti_index-0.1.3/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.3/README.md
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-23 13:00:25.736519 hti_index-0.1.3/hti_index/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      192 2023-04-23 13:00:03.000000 hti_index-0.1.3/hti_index/__init__.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     6456 2023-04-23 12:54:39.000000 hti_index-0.1.3/hti_index/chain_tree.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3087 2023-04-23 12:55:16.000000 hti_index-0.1.3/hti_index/component.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2796 2023-04-23 12:55:36.000000 hti_index-0.1.3/hti_index/composite.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     4744 2023-04-23 05:02:36.000000 hti_index-0.1.3/hti_index/flowfreq.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     8070 2023-04-21 13:41:18.000000 hti_index-0.1.3/hti_index/holonomic_index.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3855 2023-04-23 05:01:58.000000 hti_index-0.1.3/hti_index/indexer.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-21 06:02:13.000000 hti_index-0.1.3/hti_index/utils.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-23 13:00:25.737596 hti_index-0.1.3/hti_index.egg-info/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-23 13:00:25.000000 hti_index-0.1.3/hti_index.egg-info/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      373 2023-04-23 13:00:25.000000 hti_index-0.1.3/hti_index.egg-info/SOURCES.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-23 13:00:25.000000 hti_index-0.1.3/hti_index.egg-info/dependency_links.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-23 13:00:25.000000 hti_index-0.1.3/hti_index.egg-info/requires.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-23 13:00:25.000000 hti_index-0.1.3/hti_index.egg-info/top_level.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-23 13:00:25.738291 hti_index-0.1.3/setup.cfg
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-23 13:00:19.000000 hti_index-0.1.3/setup.py
```

### Comparing `hti_index-0.1.2/PKG-INFO` & `hti_index-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti_index
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.2/README.md` & `hti_index-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.2/hti_index/component.py` & `hti_index-0.1.3/hti_index/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 class Component(NodeComponent):
     def __init__(self):
         self.parent = None
         self.children = []
         
     def accept(self, visitor):
         visitor.visit_component(self)
-
-
-    
+        
     @abstractmethod
     def get_ancestors(self) -> List['NodeComponent']:
         pass
 
     @abstractmethod
     def get_descendants(self) -> List['NodeComponent']:
         pass
@@ -60,16 +58,14 @@
         self.children.remove(child)
         
     @abstractmethod
     def max_children(self) -> int:
         pass
     
     
-    
-    
 class Composite(Component):
     
     def __init__(self, key: str, value: str):
         super().__init__()
         self.key = key
         self.value = value
```

### Comparing `hti_index-0.1.2/hti_index/composite.py` & `hti_index-0.1.3/hti_index/composite.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,8 +64,9 @@
 
     def get_children(self) -> List[Component]:
         return {
             "children": self.children,
             "children_hashes": self.children_hashes
         }
 
-    
+    def __str__(self):
+        return f"NodeComposite(id={self.id}, key={self.key}, value={self.value})"
```

### Comparing `hti_index-0.1.2/hti_index/indexer.py` & `hti_index-0.1.3/hti_index/indexer.py`

 * *Files 24% similar despite different names*

```diff
@@ -101,43 +101,8 @@
     def range_search(self, start: str, end: str) -> List[Tuple[str, Any]]:
         results = []
         for bucket in self.hash_table:
             if bucket is not None:
                 for node in bucket:
                     results.extend(self._get_range(node, start, end))
         return results
-    
-
-    def _get_node_frequency(self, key: str) -> int:
-        return len(self.get_bucket(key))
-    
-    def _get_transition_frequency(self, prev_key: str, key: str) -> int:
-        return sum(1 for node in self.get_bucket(prev_key) if node.key == key)
-
-        
-    def _get_node_probability(self, key: str) -> float:
-        return self._get_node_frequency(key) / self.num_items
-            
-    def _get_transition_probability(self, prev_key: str, key: str) -> float:
-        return self._get_transition_frequency(prev_key, key) / self.num_items
-    
-    def _get_node_entropy(self, key: str) -> float:
-        prob = self._get_node_probability(key)
-        return -prob * np.log2(prob)
-    
-    def _get_transition_entropy(self, prev_key: str, key: str) -> float:
-        prob = self._get_transition_probability(prev_key, key)
-        return -prob * np.log2(prob)
-            
-    def _get_node_information(self, key: str) -> float:
-        return self._get_node_entropy(key) * self._get_node_frequency(key)
-    
-    def _get_transition_information(self, prev_key: str, key: str) -> float:
-        return self._get_transition_entropy(prev_key, key) * self._get_transition_frequency(prev_key, key)
-    
-    def _get_node_information_gain(self, key: str) -> float:
-        return self._get_node_information(key) / self.num_items
-    
-    def _get_transition_information_gain(self, prev_key: str, key: str) -> float:
-        return self._get_transition_information(prev_key, key) / self.num_items
-
```

### Comparing `hti_index-0.1.2/hti_index/utils.py` & `hti_index-0.1.3/hti_index/utils.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.2/hti_index.egg-info/PKG-INFO` & `hti_index-0.1.3/hti_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti-index
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.2/setup.py` & `hti_index-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Description: Setup script for the qbf_index package
 from setuptools import setup, find_packages
 
 setup(
     name='hti_index',
-    version='0.1.2',
+    version='0.1.3',
     author='Mohamed Diomande',
     author_email='gdiomande7907@gmail.com',
     description='Python package for implementing a HasH Table Index', 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/diomandeee/hti_index',
     packages=find_packages(),
```

