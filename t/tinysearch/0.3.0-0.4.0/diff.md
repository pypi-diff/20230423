# Comparing `tmp/tinysearch-0.3.0.tar.gz` & `tmp/tinysearch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinysearch-0.3.0.tar", last modified: Fri Apr 21 23:20:29 2023, max compression
+gzip compressed data, was "tinysearch-0.4.0.tar", last modified: Sun Apr 23 11:30:33 2023, max compression
```

## Comparing `tinysearch-0.3.0.tar` & `tinysearch-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-21 23:20:18.871505 tinysearch-0.3.0/LICENSE
--rw-r--r--   0        0        0     2292 2023-04-21 23:20:18.871505 tinysearch-0.3.0/README.md
--rw-r--r--   0        0        0      999 2023-04-21 23:20:29.983475 tinysearch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/analyzer.py
--rw-r--r--   0        0        0        0 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/base/__init__.py
--rw-r--r--   0        0        0      775 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/base/analyzer.py
--rw-r--r--   0        0        0     1464 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/document.py
--rw-r--r--   0        0        0     1178 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/index.py
--rw-r--r--   0        0        0     3357 2023-04-21 23:20:18.871505 tinysearch-0.3.0/tinysearch/search.py
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 tinysearch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-23 11:30:22.711030 tinysearch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3189 2023-04-23 11:30:22.711030 tinysearch-0.4.0/README.md
+-rw-r--r--   0        0        0     1044 2023-04-23 11:30:33.871198 tinysearch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/analyzer.py
+-rw-r--r--   0        0        0        0 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/base/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/base/analyzer.py
+-rw-r--r--   0        0        0     1464 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/document.py
+-rw-r--r--   0        0        0     1178 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/index.py
+-rw-r--r--   0        0        0     3479 2023-04-23 11:30:22.711030 tinysearch-0.4.0/tinysearch/search.py
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 tinysearch-0.4.0/PKG-INFO
```

### Comparing `tinysearch-0.3.0/LICENSE` & `tinysearch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinysearch-0.3.0/pyproject.toml` & `tinysearch-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
     "pytest-cov>=4.0.0",
     "black>=23.3.0",
+    "pyflame>=0.3.0",
+    "ipython>=8.12.0",
 ]
 lint = [
     "flake8",
     "black",
 ]
 test = [
     "pytest",
@@ -40,15 +42,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "search",
     "engine",
 ]
-version = "0.3.0"
+version = "0.4.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://github.com/dmarsic/tinysearch"
```

### Comparing `tinysearch-0.3.0/tinysearch/analyzer.py` & `tinysearch-0.4.0/tinysearch/analyzer.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.3.0/tinysearch/base/analyzer.py` & `tinysearch-0.4.0/tinysearch/base/analyzer.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.3.0/tinysearch/document.py` & `tinysearch-0.4.0/tinysearch/document.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.3.0/tinysearch/index.py` & `tinysearch-0.4.0/tinysearch/index.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.3.0/tinysearch/search.py` & `tinysearch-0.4.0/tinysearch/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     print(s.results.count)
     # 4
 
     print(s.results.matches[0])
     # Result(doc=..., score=0.20)
 """
 
+from collections import defaultdict
 from dataclasses import dataclass
 from math import log
 from typing import List
 
 from tinysearch.index import Index
 from tinysearch.document import Document
 from tinysearch.base.analyzer import Analyzer
@@ -87,37 +88,36 @@
     def __str__(self):
         return f"Search[query='{self.query}', matches={self.results.count}]"
 
     def __repr__(self):
         return self.__str__()
 
     def search(self) -> Results:
-        self.score_docs(self.query)
+        """Search builds a result set of matched documents.
 
-    def score_docs(self, query: str):
-        for doc in self.index.docs:
-            score = self.score_doc(doc, query)
-            self.results.append(Result(doc, score))
-
-    def score_doc(self, doc: Document, query: str) -> float:
-        tfidf_sum = 0.0
-        query_tokens = self.analyzer.analyze(query)
-        for t in query_tokens:
-            tfidf_sum += self.calculate_tfidf(doc, t)
-        return tfidf_sum
+        It takes the query and splits it into tokens, and then
+        calculates TF-IDF score for each document for each query
+        token. A final TF-IDF score is the sum of TF-IDF scores
+        for each query token.
+        """
+        query_tokens = self.analyzer.analyze(self.query)
 
-    def calculate_tfidf(self, doc: Document, query_token: str) -> float:
-        tf = doc.tokens[query_token] / sum(doc.tokens.values())
+        # Store the number of documents each query token appears in.
+        occurs = defaultdict(int)
+        for doc in self.index.docs:
+            for token in query_tokens:
+                occurs[token] += int(token in doc.tokens)
 
-        doc_count = len(self.index.docs)
-        contains_word_count = 0
+        # Calculate TF-IDF for each document.
         for doc in self.index.docs:
-            if query_token in doc.tokens:
-                contains_word_count += 1
-        if contains_word_count == 0:
-            return 0.0
+            tfidf_sum = 0.0
+
+            for token in query_tokens:
+                if occurs[token] == 0:
+                    continue
 
-        idf = log(doc_count / contains_word_count)
+                tf = doc.tokens[token] / sum(doc.tokens.values())
+                idf = log(len(self.index.docs) / occurs[token])
 
-        tfidf = tf * idf
+                tfidf_sum += tf * idf
 
-        return tfidf
+            self.results.append(Result(doc, tfidf_sum))
```

### Comparing `tinysearch-0.3.0/PKG-INFO` & `tinysearch-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tinysearch
-Version: 0.3.0
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
@@ -104,10 +89,50 @@
 tokenized and transformed for easier search. The same process is
 applied to the query.
 
 Then each document is scored using the TF-IDF algorithm to find the
 best match, and matches are returned sorted to the user. The best match
 is at the top.
 
+## Performance
+
+Performance is important since search engines typically respond to
+user queries, so it should generate results in a few seconds at most.
+More than that would appear as a significant delay.
+
+The numbers below are dependent on the running machine, so they are
+just indicative.
+
+```mermaid
+gantt
+title Search time for different dataset sizes [s]
+dateFormat X
+axisFormat %s
+
+section 100
+0.1, terms=1 : 0, 0.1s
+0.1, terms=2 : 0, 0.1s
+0.1, terms=3 : 0, 0.1s
+
+section 1000
+0.9, terms=1 : 0, 0.9s
+0.9, terms=2 : 0, 0.9s
+0.9, terms=3 : 0, 0.9s
+
+section 10000
+9.2, terms=1 : 0, 9.2s
+9.1, terms=2 : 0, 9.1s
+9.1, terms=3 : 0, 9.1s
+
+section 52478
+46.9, terms=1 : 0, 46.9s
+53.8, terms=2 : 0, 53.8s
+46.2, terms=3 : 0, 46.2s
+```
+
+Datasets of around 1000 entries might generate reasonable search times,
+which is the intended use case for TinySearch. Still, there is probably
+room for improvement.
+
 ## License
 
 See LICENSE.
```

