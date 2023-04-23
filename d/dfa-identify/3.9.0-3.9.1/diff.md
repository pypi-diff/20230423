# Comparing `tmp/dfa_identify-3.9.0.tar.gz` & `tmp/dfa_identify-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfa_identify-3.9.0.tar", max compression
+gzip compressed data, was "dfa_identify-3.9.1.tar", max compression
```

## Comparing `dfa_identify-3.9.0.tar` & `dfa_identify-3.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2021-04-24 20:56:37.141888 dfa_identify-3.9.0/LICENSE
--rw-r--r--   0        0        0     3794 2021-11-01 19:39:41.141847 dfa_identify-3.9.0/README.md
--rw-r--r--   0        0        0       74 2021-11-01 19:39:41.141847 dfa_identify-3.9.0/dfa_identify/__init__.py
--rw-r--r--   0        0        0    11955 2021-09-28 21:10:17.627019 dfa_identify-3.9.0/dfa_identify/encoding.py
--rw-r--r--   0        0        0     4565 2021-11-01 19:39:41.141847 dfa_identify-3.9.0/dfa_identify/graphs.py
--rw-r--r--   0        0        0     8861 2021-12-12 20:07:37.284147 dfa_identify-3.9.0/dfa_identify/identify.py
--rw-r--r--   0        0        0      666 2021-12-12 20:09:41.010869 dfa_identify-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     4787 2021-12-12 20:09:57.700629 dfa_identify-3.9.0/setup.py
--rw-r--r--   0        0        0     4683 2021-12-12 20:09:57.702604 dfa_identify-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-23 17:52:47.971187 dfa_identify-3.9.1/LICENSE
+-rw-r--r--   0        0        0     3794 2023-04-23 17:52:47.971187 dfa_identify-3.9.1/README.md
+-rw-r--r--   0        0        0       74 2023-04-23 17:52:47.971187 dfa_identify-3.9.1/dfa_identify/__init__.py
+-rw-r--r--   0        0        0    11955 2023-04-23 17:52:47.971187 dfa_identify-3.9.1/dfa_identify/encoding.py
+-rw-r--r--   0        0        0     4565 2023-04-23 17:52:47.972187 dfa_identify-3.9.1/dfa_identify/graphs.py
+-rw-r--r--   0        0        0     8861 2023-04-23 17:52:47.972187 dfa_identify-3.9.1/dfa_identify/identify.py
+-rw-r--r--   0        0        0      628 2023-04-23 18:07:10.636553 dfa_identify-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 dfa_identify-3.9.1/setup.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 dfa_identify-3.9.1/PKG-INFO
```

### Comparing `dfa_identify-3.9.0/LICENSE` & `dfa_identify-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfa_identify-3.9.0/README.md` & `dfa_identify-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dfa_identify-3.9.0/dfa_identify/encoding.py` & `dfa_identify-3.9.1/dfa_identify/encoding.py`

 * *Files identical despite different names*

### Comparing `dfa_identify-3.9.0/dfa_identify/graphs.py` & `dfa_identify-3.9.1/dfa_identify/graphs.py`

 * *Files identical despite different names*

### Comparing `dfa_identify-3.9.0/dfa_identify/identify.py` & `dfa_identify-3.9.1/dfa_identify/identify.py`

 * *Files identical despite different names*

### Comparing `dfa_identify-3.9.0/setup.py` & `dfa_identify-3.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['dfa_identify']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=21.0.0,<22.0.0',
- 'bidict>=0.21.2,<0.22.0',
+['attrs>=22.0.0,<23.0.0',
+ 'bidict>=0.22,<0.23',
  'dfa>=4,<5',
  'funcy>=1.15,<2.0',
- 'more-itertools>=8.12.0,<9.0.0',
- 'networkx>=2.6,<3.0',
+ 'more-itertools>=9,<10',
+ 'networkx>=3,<4',
  'python-sat>=0.1.7.dev11,<0.2.0']
 
 setup_kwargs = {
     'name': 'dfa-identify',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'Python library for identifying (learning) DFAs (automata) from labeled examples.',
     'long_description': '# dfa-identify\nPython library for identifying (learning) minimal DFAs from labeled examples\nby reduction to SAT.\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/dfa-identify/status.svg)](https://cloud.drone.io/mvcisback/dfa-identify)\n[![PyPI version](https://badge.fury.io/py/dfa-identify.svg)](https://badge.fury.io/py/dfa-identify)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n**Table of Contents**\n\n- [Installation](#installation)\n- [Usage](#usage)\n- [Encoding](#encoding)\n- [Goals and related libraries](#goals-and-related-libraries)\n\n# Installation\n\nIf you just need to use `dfa`, you can just run:\n\n`$ pip install dfa`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# Usage\n\n`dfa_identify` is centered around the `find_dfa` and `find_dfas` function. Both take in\nsequences of accepting and rejecting "words", where are word is a\nsequence of arbitrary python objects. \n\n1. `find_dfas` returns all minimally sized (no `DFA`s exist of size\nsmaller) consistent with the given labeled data.\n\n2. `find_dfa` returns an arbitrary (first) minimally sized `DFA`.\n\nThe returned `DFA` object is from the [dfa](https://github.com/mvcisback/dfa) library.\n\n\n```python\nfrom dfa_identify import find_dfa\n\n\naccepting = [\'a\', \'abaa\', \'bb\']\nrejecting = [\'abb\', \'b\']\n    \nmy_dfa = find_dfa(accepting=accepting, rejecting=rejecting)\n\nassert all(my_dfa.label(x) for x in accepting)\nassert all(not my_dfa.label(x) for x in rejecting)\n```\n\nBecause words are sequences of arbitrary python objects, the\nidentification problem, with `a` ↦ 0 and `b` ↦ 1, is given below:\n\n\n```python\naccepting = [[0], [0, \'z\', 0, 0], [\'z\', \'z\']]\nrejecting = [[0, \'z\', \'z\'], [\'z\']]\n\nmy_dfa = find_dfa(accepting=accepting, rejecting=rejecting)\n```\n\n# Minimality\n\nThere are two forms of "minimality" supported by `dfa-identify`.\n\n1. By default, dfa-identify returns DFAs that have the minimum\n   number of states required to seperate the accepting and\n   rejecting set.\n2. If the `order_by_stutter` flag is set to `True`, then the\n   `find_dfas` (lazily) orders the DFAs so that the number of\n   self loops (stuttering transitions) appearing the DFAs decreases.\n   `find_dfa` thus returns a DFA with the most number of self loops\n   given the minimal number of states.\n\n# Encoding\n\nThis library currently uses the encodings outlined in [Heule, Marijn JH, and Sicco Verwer. "Exact DFA identification using SAT solvers." International Colloquium on Grammatical Inference. Springer, Berlin, Heidelberg, 2010.](https://link.springer.com/chapter/10.1007/978-3-642-15488-1_7) and [Ulyantsev, Vladimir, Ilya Zakirzyanov, and Anatoly Shalyto. "Symmetry Breaking Predicates for SAT-based DFA Identification."](https://arxiv.org/abs/1602.05028).\n\nThe key difference is in the use of the symmetry breaking clauses. Two kinds are exposed.\n\n1. clique (Heule 2010): Partially breaks symmetries by analyzing\n   conflict graph.\n2. bfs (Ulyantsev 2016): Breaks all symmetries so that each model corresponds to a unique DFA.\n\n# Goals and related libraries\n\nThere are many other python libraries that \nperform DFA and other automata inference.\n\n1. [DFA-Inductor-py](https://github.com/ctlab/DFA-Inductor-py) - State of the art passive inference via reduction to SAT (as of 2019).\n2. [z3gi](https://gitlab.science.ru.nl/rick/z3gi): Uses SMT backed passive learning algorithm.\n3. [lstar](https://pypi.org/project/lstar/): Active learning algorithm based L* derivative.\n\nThe primary goal of this library is to loosely track the state of the art in passive SAT based inference while providing a simple implementation and API.\n',
     'author': 'Marcell Vazquez-Chanlatte',
     'author_email': 'mvc@linux.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mvcisback/dfa-identify',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `dfa_identify-3.9.0/PKG-INFO` & `dfa_identify-3.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dfa-identify
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python library for identifying (learning) DFAs (automata) from labeled examples.
 Home-page: https://github.com/mvcisback/dfa-identify
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: mvc@linux.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: attrs (>=21.0.0,<22.0.0)
-Requires-Dist: bidict (>=0.21.2,<0.22.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22.0.0,<23.0.0)
+Requires-Dist: bidict (>=0.22,<0.23)
 Requires-Dist: dfa (>=4,<5)
 Requires-Dist: funcy (>=1.15,<2.0)
-Requires-Dist: more-itertools (>=8.12.0,<9.0.0)
-Requires-Dist: networkx (>=2.6,<3.0)
+Requires-Dist: more-itertools (>=9,<10)
+Requires-Dist: networkx (>=3,<4)
 Requires-Dist: python-sat (>=0.1.7.dev11,<0.2.0)
 Project-URL: Repository, https://github.com/mvcisback/dfa-identify
 Description-Content-Type: text/markdown
 
 # dfa-identify
 Python library for identifying (learning) minimal DFAs from labeled examples
 by reduction to SAT.
```

