# Comparing `tmp/extr-0.0.8.tar.gz` & `tmp/extr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.8.tar", last modified: Tue Apr 18 09:55:54 2023, max compression
+gzip compressed data, was "extr-0.0.9.tar", last modified: Tue Apr 18 10:30:47 2023, max compression
```

## Comparing `extr-0.0.8.tar` & `extr-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.332029 extr-0.0.8/
--rw-rw-rw-   0        0        0     2522 2023-04-18 09:55:54.329917 extr-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1655 2023-04-18 09:54:04.000000 extr-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 09:55:54.338972 extr-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-04-18 09:55:24.000000 extr-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.123941 extr-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.195901 extr-0.0.8/src/extr/
--rw-rw-rw-   0        0        0      268 2023-04-18 09:50:37.000000 extr-0.0.8/src/extr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.276871 extr-0.0.8/src/extr/entities/
--rw-rw-rw-   0        0        0       80 2023-04-18 09:41:28.000000 extr-0.0.8/src/extr/entities/__init__.py
--rw-rw-rw-   0        0        0      612 2023-04-18 09:41:38.000000 extr-0.0.8/src/extr/entities/annotator.py
--rw-rw-rw-   0        0        0     1144 2023-04-18 09:45:57.000000 extr-0.0.8/src/extr/entities/extractor.py
--rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.8/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     2901 2023-04-18 09:42:52.000000 extr-0.0.8/src/extr/models.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.293671 extr-0.0.8/src/extr/regexes/
--rw-rw-rw-   0        0        0       38 2023-04-18 09:50:25.000000 extr-0.0.8/src/extr/regexes/__init__.py
--rw-rw-rw-   0        0        0      905 2023-04-18 09:47:44.000000 extr-0.0.8/src/extr/regexes/regex.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.311522 extr-0.0.8/src/extr/relations/
--rw-rw-rw-   0        0        0       96 2023-04-18 09:53:11.000000 extr-0.0.8/src/extr/relations/__init__.py
--rw-rw-rw-   0        0        0     1177 2023-04-18 09:46:03.000000 extr-0.0.8/src/extr/relations/extractor.py
--rw-rw-rw-   0        0        0     1676 2023-04-18 09:53:02.000000 extr-0.0.8/src/extr/relations/label_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.325156 extr-0.0.8/src/extr/tokenizers/
--rw-rw-rw-   0        0        0       34 2023-04-18 09:43:44.000000 extr-0.0.8/src/extr/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-04-18 09:43:53.000000 extr-0.0.8/src/extr/tokenizers/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.261625 extr-0.0.8/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2522 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.167752 extr-0.0.9/
+-rw-rw-rw-   0        0        0     2522 2023-04-18 10:30:47.159717 extr-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1655 2023-04-18 09:54:04.000000 extr-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:30:47.179153 extr-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-04-18 10:30:31.000000 extr-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:46.901196 extr-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:46.972872 extr-0.0.9/src/extr/
+-rw-rw-rw-   0        0        0      268 2023-04-18 09:50:37.000000 extr-0.0.9/src/extr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.080220 extr-0.0.9/src/extr/entities/
+-rw-rw-rw-   0        0        0       80 2023-04-18 09:41:28.000000 extr-0.0.9/src/extr/entities/__init__.py
+-rw-rw-rw-   0        0        0      612 2023-04-18 09:41:38.000000 extr-0.0.9/src/extr/entities/annotator.py
+-rw-rw-rw-   0        0        0     1140 2023-04-18 10:28:24.000000 extr-0.0.9/src/extr/entities/extractor.py
+-rw-rw-rw-   0        0        0     2901 2023-04-18 09:42:52.000000 extr-0.0.9/src/extr/models.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.090509 extr-0.0.9/src/extr/regexes/
+-rw-rw-rw-   0        0        0       38 2023-04-18 09:50:25.000000 extr-0.0.9/src/extr/regexes/__init__.py
+-rw-rw-rw-   0        0        0      911 2023-04-18 10:28:39.000000 extr-0.0.9/src/extr/regexes/regex.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.121475 extr-0.0.9/src/extr/relations/
+-rw-rw-rw-   0        0        0       96 2023-04-18 09:53:11.000000 extr-0.0.9/src/extr/relations/__init__.py
+-rw-rw-rw-   0        0        0     1173 2023-04-18 10:28:15.000000 extr-0.0.9/src/extr/relations/extractor.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 09:53:02.000000 extr-0.0.9/src/extr/relations/label_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.138207 extr-0.0.9/src/extr/tokenizers/
+-rw-rw-rw-   0        0        0       34 2023-04-18 09:43:44.000000 extr-0.0.9/src/extr/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-04-18 10:20:42.000000 extr-0.0.9/src/extr/tokenizers/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.158714 extr-0.0.9/src/extr/utils/
+-rw-rw-rw-   0        0        0       58 2023-04-18 10:27:55.000000 extr-0.0.9/src/extr/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.9/src/extr/utils/iterutils.py
+-rw-rw-rw-   0        0        0      564 2023-04-18 10:30:03.000000 extr-0.0.9/src/extr/utils/query.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:30:47.054851 extr-0.0.9/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-04-18 10:30:46.000000 extr-0.0.9/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-04-18 10:30:46.000000 extr-0.0.9/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:30:46.000000 extr-0.0.9/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 10:30:46.000000 extr-0.0.9/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.8/PKG-INFO` & `extr-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
```

### Comparing `extr-0.0.8/README.md` & `extr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `extr-0.0.8/setup.py` & `extr-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr',
-    version='0.0.8',
+    version='0.0.9',
     keywords='',
     description='Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[],
     url='https://github.com/dpasse/extr',
     long_description=long_description,
```

### Comparing `extr-0.0.8/src/extr/entities/annotator.py` & `extr-0.0.9/src/extr/entities/annotator.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.8/src/extr/entities/extractor.py` & `extr-0.0.9/src/extr/entities/extractor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, cast
 
 from ..regexes import RegExLabel
-from ..iterutils import flatten
+from ..utils import flatten
 from ..models import Location, Entity
 
 
 class EntityExtractor:
     def __init__(self, regex_labels: List[RegExLabel]) -> None:
         self._regex_labels = regex_labels
```

### Comparing `extr-0.0.8/src/extr/models.py` & `extr-0.0.9/src/extr/models.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.8/src/extr/regexes/regex.py` & `extr-0.0.9/src/extr/regexes/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple
 import re
 
-from ..iterutils import flatten
+from ..utils.iterutils import flatten
 
 
 class RegEx:
     def __init__(self, expressions: List[str], flags: int = 0) -> None:
         self._expressions = expressions
         self._flags = flags
```

### Comparing `extr-0.0.8/src/extr/relations/extractor.py` & `extr-0.0.9/src/extr/relations/extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Generator, cast
 
 import re
 from ..regexes import RegExLabel
 from ..models import EntityAnnotationResults, Relation
-from ..iterutils import flatten
+from ..utils import flatten
 
 
 class RelationExtractor:
     def __init__(self, relation_labels: List[RegExLabel]) -> None:
         self._relation_labels = relation_labels
 
     def extract(self, entity_annotation_results: EntityAnnotationResults) -> List[Relation]:
```

### Comparing `extr-0.0.8/src/extr/relations/label_builder.py` & `extr-0.0.9/src/extr/relations/label_builder.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.8/src/extr/tokenizers/tokenizer.py` & `extr-0.0.9/src/extr/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.8/src/extr.egg-info/PKG-INFO` & `extr-0.0.9/src/extr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
```

### Comparing `extr-0.0.8/src/extr.egg-info/SOURCES.txt` & `extr-0.0.9/src/extr.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.md
 setup.py
 src/extr/__init__.py
-src/extr/iterutils.py
 src/extr/models.py
 src/extr.egg-info/PKG-INFO
 src/extr.egg-info/SOURCES.txt
 src/extr.egg-info/dependency_links.txt
 src/extr.egg-info/top_level.txt
 src/extr/entities/__init__.py
 src/extr/entities/annotator.py
 src/extr/entities/extractor.py
 src/extr/regexes/__init__.py
 src/extr/regexes/regex.py
 src/extr/relations/__init__.py
 src/extr/relations/extractor.py
 src/extr/relations/label_builder.py
 src/extr/tokenizers/__init__.py
-src/extr/tokenizers/tokenizer.py
+src/extr/tokenizers/tokenizer.py
+src/extr/utils/__init__.py
+src/extr/utils/iterutils.py
+src/extr/utils/query.py
```

