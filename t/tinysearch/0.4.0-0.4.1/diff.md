# Comparing `tmp/tinysearch-0.4.0.tar.gz` & `tmp/tinysearch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinysearch-0.4.0.tar", last modified: Sun Apr 23 11:30:33 2023, max compression
+gzip compressed data, was "tinysearch-0.4.1.tar", last modified: Sun Apr 23 12:19:46 2023, max compression
```

## Comparing `tinysearch-0.4.0.tar` & `tinysearch-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-23 11:30:22.711030 tinysearch-0.4.0/LICENSE
--rw-r--r--   0        0        0     3189 2023-04-23 11:30:22.711030 tinysearch-0.4.0/README.md
--rw-r--r--   0        0        0     1044 2023-04-23 11:30:33.871198 tinysearch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/analyzer.py
--rw-r--r--   0        0        0        0 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/base/__init__.py
--rw-r--r--   0        0        0      775 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/base/analyzer.py
--rw-r--r--   0        0        0     1464 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/document.py
--rw-r--r--   0        0        0     1178 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/index.py
--rw-r--r--   0        0        0     3479 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/search.py
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 tinysearch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-23 12:19:29.850110 tinysearch-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3189 2023-04-23 12:19:29.850110 tinysearch-0.4.1/README.md
+-rw-r--r--   0        0        0     1044 2023-04-23 12:19:46.750129 tinysearch-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/__init__.py
+-rw-r--r--   0        0        0     1392 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/analyzer.py
+-rw-r--r--   0        0        0        0 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/base/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/base/analyzer.py
+-rw-r--r--   0        0        0     1464 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/document.py
+-rw-r--r--   0        0        0     1178 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/index.py
+-rw-r--r--   0        0        0     3479 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/search.py
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 tinysearch-0.4.1/PKG-INFO
```

### Comparing `tinysearch-0.4.0/LICENSE` & `tinysearch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.0/README.md` & `tinysearch-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tinysearch
+Version: 0.4.1
+Summary: Tiny one-phase search engine
+Keywords: search engine
+Author-Email: Domagoj Marsic <dmars@protonmail.com>
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/dmarsic/tinysearch
+Requires-Python: >=3.9
+Requires-Dist: pystemmer>=2.2.0.1
+Description-Content-Type: text/markdown
+
 # TinySearch
 
 TinySearch is a tiny one-phase search engine. It is extremely easy to
 use and works well with simple lists where the query may not match the
 document text exactly.
 
 This is a minimal search engine. You don't need to run separate, big
@@ -110,27 +125,27 @@
 
 section 100
 0.1, terms=1 : 0, 0.1s
 0.1, terms=2 : 0, 0.1s
 0.1, terms=3 : 0, 0.1s
 
 section 1000
-0.9, terms=1 : 0, 0.9s
-0.9, terms=2 : 0, 0.9s
-0.9, terms=3 : 0, 0.9s
+0.6, terms=1 : 0, 0.6s
+0.6, terms=2 : 0, 0.6s
+0.5, terms=3 : 0, 0.5s
 
 section 10000
-9.2, terms=1 : 0, 9.2s
-9.1, terms=2 : 0, 9.1s
-9.1, terms=3 : 0, 9.1s
+5.2, terms=1 : 0, 5.2s
+4.9, terms=2 : 0, 4.9s
+4.9, terms=3 : 0, 4.9s
 
 section 52478
-46.9, terms=1 : 0, 46.9s
-53.8, terms=2 : 0, 53.8s
-46.2, terms=3 : 0, 46.2s
+26.8, terms=1 : 0, 26.8s
+26.8, terms=2 : 0, 26.8s
+26.8, terms=3 : 0, 26.8s
 ```
 
 Datasets of around 1000 entries might generate reasonable search times,
 which is the intended use case for TinySearch. Still, there is probably
 room for improvement.
 
 ## License
```

### Comparing `tinysearch-0.4.0/pyproject.toml` & `tinysearch-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "search",
     "engine",
 ]
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://github.com/dmarsic/tinysearch"
```

### Comparing `tinysearch-0.4.0/tinysearch/analyzer.py` & `tinysearch-0.4.1/tinysearch/analyzer.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,30 +17,33 @@
 import Stemmer
 from typing import List
 
 from tinysearch.base.analyzer import Analyzer
 
 
 class SimpleEnglishAnalyzer(Analyzer):
-    @classmethod
-    def remove_nonchars(cls, token: str) -> str:
-        m = re.search(r"[\w\-]+", token)
-        if m:
-            token = m.group(0)
-        return token
+    def __init__(self):
+        super().__init__()
+        self.stemmer = Stemmer.Stemmer("english")
 
     @classmethod
-    def stem(cls, token: str) -> str:
-        stemmer = Stemmer.Stemmer("english")
-        return stemmer.stemWord(token)
+    def remove_nonchars(cls, token: str) -> str:
+        new_chars = []
+        for c in token:
+            if c.isalnum() or c == "-":
+                new_chars.append(c)
+        return ''.join(new_chars)
 
     @classmethod
     def lower(cls, token: str) -> str:
         return token.lower()
 
+    def stem(self, token: str) -> str:
+        return self.stemmer.stemWord(token)
+
     def analyze(self, text: str) -> List[str]:
         """Transforms input text to a list of tokens."""
 
         # Split on whitespace.
         tokens = re.split(r"\s+", text)
 
         # Apply transformations on each token.
```

### Comparing `tinysearch-0.4.0/tinysearch/base/analyzer.py` & `tinysearch-0.4.1/tinysearch/base/analyzer.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.0/tinysearch/document.py` & `tinysearch-0.4.1/tinysearch/document.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.0/tinysearch/index.py` & `tinysearch-0.4.1/tinysearch/index.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.0/tinysearch/search.py` & `tinysearch-0.4.1/tinysearch/search.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.0/PKG-INFO` & `tinysearch-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tinysearch
-Version: 0.4.0
-Summary: Tiny one-phase search engine
-Keywords: search engine
-Author-Email: Domagoj Marsic <dmars@protonmail.com>
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Project-URL: Homepage, https://github.com/dmarsic/tinysearch
-Requires-Python: >=3.9
-Requires-Dist: pystemmer>=2.2.0.1
-Description-Content-Type: text/markdown
-
 # TinySearch
 
 TinySearch is a tiny one-phase search engine. It is extremely easy to
 use and works well with simple lists where the query may not match the
 document text exactly.
 
 This is a minimal search engine. You don't need to run separate, big
@@ -125,27 +110,27 @@
 
 section 100
 0.1, terms=1 : 0, 0.1s
 0.1, terms=2 : 0, 0.1s
 0.1, terms=3 : 0, 0.1s
 
 section 1000
-0.9, terms=1 : 0, 0.9s
-0.9, terms=2 : 0, 0.9s
-0.9, terms=3 : 0, 0.9s
+0.6, terms=1 : 0, 0.6s
+0.6, terms=2 : 0, 0.6s
+0.5, terms=3 : 0, 0.5s
 
 section 10000
-9.2, terms=1 : 0, 9.2s
-9.1, terms=2 : 0, 9.1s
-9.1, terms=3 : 0, 9.1s
+5.2, terms=1 : 0, 5.2s
+4.9, terms=2 : 0, 4.9s
+4.9, terms=3 : 0, 4.9s
 
 section 52478
-46.9, terms=1 : 0, 46.9s
-53.8, terms=2 : 0, 53.8s
-46.2, terms=3 : 0, 46.2s
+26.8, terms=1 : 0, 26.8s
+26.8, terms=2 : 0, 26.8s
+26.8, terms=3 : 0, 26.8s
 ```
 
 Datasets of around 1000 entries might generate reasonable search times,
 which is the intended use case for TinySearch. Still, there is probably
 room for improvement.
 
 ## License
```

