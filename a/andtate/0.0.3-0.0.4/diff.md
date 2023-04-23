# Comparing `tmp/andtate-0.0.3.tar.gz` & `tmp/andtate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andtate-0.0.3.tar", last modified: Sun Apr 23 11:46:15 2023, max compression
+gzip compressed data, was "andtate-0.0.4.tar", last modified: Sun Apr 23 11:50:45 2023, max compression
```

## Comparing `andtate-0.0.3.tar` & `andtate-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 11:46:15.320219 andtate-0.0.3/
--rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      553 2023-04-23 11:46:15.318071 andtate-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 11:46:15.275954 andtate-0.0.3/andtate/
--rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.3/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
--rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.3/andtate/AMDL Linear Regression (Diabetes Dataset).py
--rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.3/andtate/AMDL Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.3/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
--rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.3/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.3/andtate/AMDL SVM classifier (Iris Dataset).py
--rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.3/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
--rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.3/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
--rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.3/andtate/AMDL.py
--rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.3/andtate/NLP Dependency parsing of a given text.py
--rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.3/andtate/NLP Implement a tri-gram model.py
--rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.3/andtate/NLP Lemmatization.py
--rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.3/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
--rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.3/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
--rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.3/andtate/NLP Stemming.py
--rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.3/andtate/NLP Syntactic parsing of a given text.py
--rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.3/andtate/NLP Text summarization using NLTK Library.py
--rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.3/andtate/NLP Text summarization using gensim Library.py
--rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.3/andtate/NLP Text summarization using spaCy Library.py
--rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.3/andtate/NLP Tokenization using Gensim.py
--rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.3/andtate/NLP Tokenization using NLTK.py
--rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.3/andtate/NLP Tokenization using Python’s split function.py
--rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.3/andtate/NLP Tokenization using Regular Expressions (RegEx).py
--rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.3/andtate/NLP Tokenization using the spaCy library.py
--rw-rw-rw-   0        0        0    17204 2023-04-23 10:19:53.000000 andtate-0.0.3/andtate/NLP.py
--rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.3/andtate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 11:46:15.309618 andtate-0.0.3/andtate.egg-info/
--rw-rw-rw-   0        0        0      553 2023-04-23 11:46:14.000000 andtate-0.0.3/andtate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-04-23 11:46:14.000000 andtate-0.0.3/andtate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 11:46:14.000000 andtate-0.0.3/andtate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 11:46:14.000000 andtate-0.0.3/andtate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 11:46:15.320321 andtate-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-23 11:45:59.000000 andtate-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.606596 andtate-0.0.4/
+-rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-04-23 11:50:45.605448 andtate-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.572346 andtate-0.0.4/andtate/
+-rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.4/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
+-rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.4/andtate/AMDL Linear Regression (Diabetes Dataset).py
+-rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.4/andtate/AMDL Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.4/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
+-rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.4/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.4/andtate/AMDL SVM classifier (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.4/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
+-rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.4/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
+-rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.4/andtate/AMDL.py
+-rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.4/andtate/NLP Dependency parsing of a given text.py
+-rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.4/andtate/NLP Implement a tri-gram model.py
+-rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.4/andtate/NLP Lemmatization.py
+-rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
+-rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
+-rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.4/andtate/NLP Stemming.py
+-rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.4/andtate/NLP Syntactic parsing of a given text.py
+-rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.4/andtate/NLP Text summarization using NLTK Library.py
+-rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.4/andtate/NLP Text summarization using gensim Library.py
+-rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.4/andtate/NLP Text summarization using spaCy Library.py
+-rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.4/andtate/NLP Tokenization using Gensim.py
+-rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.4/andtate/NLP Tokenization using NLTK.py
+-rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.4/andtate/NLP Tokenization using Python’s split function.py
+-rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.4/andtate/NLP Tokenization using Regular Expressions (RegEx).py
+-rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.4/andtate/NLP Tokenization using the spaCy library.py
+-rw-rw-rw-   0        0        0    17204 2023-04-23 10:19:53.000000 andtate-0.0.4/andtate/NLP.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.4/andtate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.599743 andtate-0.0.4/andtate.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 11:50:45.607595 andtate-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-23 11:50:24.000000 andtate-0.0.4/setup.py
```

### Comparing `andtate-0.0.3/LICENSE` & `andtate-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/PKG-INFO` & `andtate-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.3
+Version: 0.0.4
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.3/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py` & `andtate-0.0.4/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL Linear Regression (Diabetes Dataset).py` & `andtate-0.0.4/andtate/AMDL Linear Regression (Diabetes Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL Logistic Regression (Iris Dataset).py` & `andtate-0.0.4/andtate/AMDL Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py` & `andtate-0.0.4/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py` & `andtate-0.0.4/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL SVM classifier (Iris Dataset).py` & `andtate-0.0.4/andtate/AMDL SVM classifier (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py` & `andtate-0.0.4/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py` & `andtate-0.0.4/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/AMDL.py` & `andtate-0.0.4/andtate/AMDL.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Dependency parsing of a given text.py` & `andtate-0.0.4/andtate/NLP Dependency parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Implement a tri-gram model.py` & `andtate-0.0.4/andtate/NLP Implement a tri-gram model.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Lemmatization.py` & `andtate-0.0.4/andtate/NLP Lemmatization.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py` & `andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Stemming.py` & `andtate-0.0.4/andtate/NLP Stemming.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Syntactic parsing of a given text.py` & `andtate-0.0.4/andtate/NLP Syntactic parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Text summarization using NLTK Library.py` & `andtate-0.0.4/andtate/NLP Text summarization using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Text summarization using gensim Library.py` & `andtate-0.0.4/andtate/NLP Text summarization using gensim Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Text summarization using spaCy Library.py` & `andtate-0.0.4/andtate/NLP Text summarization using spaCy Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Tokenization using Gensim.py` & `andtate-0.0.4/andtate/NLP Tokenization using Gensim.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Tokenization using NLTK.py` & `andtate-0.0.4/andtate/NLP Tokenization using NLTK.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Tokenization using Python’s split function.py` & `andtate-0.0.4/andtate/NLP Tokenization using Python’s split function.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Tokenization using Regular Expressions (RegEx).py` & `andtate-0.0.4/andtate/NLP Tokenization using Regular Expressions (RegEx).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP Tokenization using the spaCy library.py` & `andtate-0.0.4/andtate/NLP Tokenization using the spaCy library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate/NLP.py` & `andtate-0.0.4/andtate/NLP.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/andtate.egg-info/PKG-INFO` & `andtate-0.0.4/andtate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.3
+Version: 0.0.4
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.3/andtate.egg-info/SOURCES.txt` & `andtate-0.0.4/andtate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `andtate-0.0.3/setup.py` & `andtate-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'andtate'
 LONG_DESCRIPTION = 'Finding Glitches And Loop Holes In Matrix And Trying To Break The System'
 
 # Setting up
 setup(
     name="andtate",
     version=VERSION,
```

