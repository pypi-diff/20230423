# Comparing `tmp/py-aiger-dfa-0.4.1.tar.gz` & `tmp/py_aiger_dfa-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aiger-dfa-0.4.1.tar", max compression
+gzip compressed data, was "py_aiger_dfa-0.4.2.tar", max compression
```

## Comparing `py-aiger-dfa-0.4.1.tar` & `py_aiger_dfa-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1082 2021-11-18 00:04:30.106323 py-aiger-dfa-0.4.1/LICENSE
--rw-r--r--   0        0        0     2927 2021-11-18 00:04:30.109656 py-aiger-dfa-0.4.1/README.md
--rw-r--r--   0        0        0       91 2021-11-18 00:04:30.109656 py-aiger-dfa-0.4.1/aiger_dfa/__init__.py
--rw-r--r--   0        0        0     2566 2021-11-23 06:45:55.384332 py-aiger-dfa-0.4.1/aiger_dfa/aig2dfa.py
--rw-r--r--   0        0        0     3670 2021-11-23 18:38:52.335060 py-aiger-dfa-0.4.1/aiger_dfa/dfa2aig.py
--rw-r--r--   0        0        0     1278 2021-11-23 06:48:41.241555 py-aiger-dfa-0.4.1/aiger_dfa/test_aig2dfa.py
--rw-r--r--   0        0        0     1288 2021-11-23 08:32:48.151509 py-aiger-dfa-0.4.1/aiger_dfa/test_dfa2aig.py
--rw-r--r--   0        0        0       65 2021-11-18 00:04:30.109656 py-aiger-dfa-0.4.1/aiger_dfa/utils.py
--rw-r--r--   0        0        0      742 2021-11-23 18:38:57.524786 py-aiger-dfa-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3897 2021-11-23 18:39:20.630586 py-aiger-dfa-0.4.1/setup.py
--rw-r--r--   0        0        0     3836 2021-11-23 18:39:20.631121 py-aiger-dfa-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-23 06:43:49.294579 py_aiger_dfa-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2927 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/README.md
+-rw-r--r--   0        0        0       91 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/__init__.py
+-rw-r--r--   0        0        0     2566 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/aig2dfa.py
+-rw-r--r--   0        0        0     3670 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/dfa2aig.py
+-rw-r--r--   0        0        0     1278 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/test_aig2dfa.py
+-rw-r--r--   0        0        0     1288 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/test_dfa2aig.py
+-rw-r--r--   0        0        0       65 2023-04-23 06:43:49.295579 py_aiger_dfa-0.4.2/aiger_dfa/utils.py
+-rw-r--r--   0        0        0      738 2023-04-23 06:57:49.951357 py_aiger_dfa-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 py_aiger_dfa-0.4.2/setup.py
+-rw-r--r--   0        0        0     3879 1970-01-01 00:00:00.000000 py_aiger_dfa-0.4.2/PKG-INFO
```

### Comparing `py-aiger-dfa-0.4.1/LICENSE` & `py_aiger_dfa-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/README.md` & `py_aiger_dfa-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/aiger_dfa/aig2dfa.py` & `py_aiger_dfa-0.4.2/aiger_dfa/aig2dfa.py`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/aiger_dfa/dfa2aig.py` & `py_aiger_dfa-0.4.2/aiger_dfa/dfa2aig.py`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/aiger_dfa/test_aig2dfa.py` & `py_aiger_dfa-0.4.2/aiger_dfa/test_aig2dfa.py`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/aiger_dfa/test_dfa2aig.py` & `py_aiger_dfa-0.4.2/aiger_dfa/test_dfa2aig.py`

 * *Files identical despite different names*

### Comparing `py-aiger-dfa-0.4.1/setup.py` & `py_aiger_dfa-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 packages = \
 ['aiger_dfa']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=21.0.0,<22.0.0',
- 'bidict>=0.21.0,<0.22.0',
+['attrs>=22,<23',
+ 'bidict>=0.22.0,<0.23.0',
  'dfa>=4,<5',
  'funcy>=1.12,<2.0',
- 'py-aiger-bv>=4.7.4,<5.0.0',
+ 'py-aiger-bv>=4.7.6,<5.0.0',
  'py-aiger-ptltl>=3.0.0,<4.0.0',
  'py-aiger>=6.0.0,<7.0.0',
- 'pyrsistent>=0.18,<0.19']
+ 'pyrsistent>=0.19,<0.20']
 
 setup_kwargs = {
     'name': 'py-aiger-dfa',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Library for moving between sequential circuits AIGs and DFAs.',
     'long_description': "# py-aiger-dfa\nPython library for converting between AIG circuits and DFAs.\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-dfa/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-dfa)\n[![Docs](https://img.shields.io/badge/API-link-color)](https://mvcisback.github.io/py-aiger-dfa)\n[![codecov](https://codecov.io/gh/mvcisback/py-aiger-dfa/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-dfa)\n[![PyPI version](https://badge.fury.io/py/py-aiger-dfa.svg)](https://badge.fury.io/py/py-aiger-dfa)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->\n**Table of Contents**\n\n- [Installation](#installation)\n- [Usage](#usage)\n    - [DFA to AIG](#dfa-to-aig)\n    - [AIG to DFA](#aig-to-dfa)\n\n<!-- markdown-toc end -->\n\n\n# Installation\n\nIf you just need to use `aiger_dfa`, you can just run:\n\n`$ pip install py-aiger-dfa`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# Usage\n\nThe main entry points for using this library are the `dfa2aig` and\n`aig2dfa` functions. DFAs are represented using the\n[dfa](https://github.com/mvcisback/dfa) package. Familiarity with the\n`dfa`, `py-aiger`, and `py-aiger-bv` packages is assumed.\n\n\n## DFA to AIG\n\nAn example of going from a `DFA` to an `AIG` object\nis shown below.\n\n```python\nfrom dfa import DFA\nfrom aiger_dfa import dfa2aig\n\nmy_dfa = DFA(\n    start=0,\n    inputs={0, 1},\n    label=lambda s: (s % 4) == 3,\n    transition=lambda s, c: (s + c) % 4,\n)\nmy_aig, relabels, valid = dfa2aig(my_dfa)\n```\n\nNow `circ` is an `AIG` and `relabels` is a mapping from the inputs,\nstates, and outputs of `my_dfa` to their **1-hot** encoded\ncounterparts in `my_aig`.\n\n`relabels` has the following schema:\n\n```python\nrelabels = {\n    'inputs': .. , #  Mapping from input alphabet -> py-aiger input.\n    'outputs': .. , # Mapping from py-aiger output -> output alphabet.\n    'states': .. , # Mapping from state space -> py-aiger latches.\n}\n```\n\nFinally, `valid` is another aiger circuit which tests if all inputs\nare 1-hot encoded.\n\n## AIG to DFA\n\nWe also support converting a sequential circuit (AIG) to a [Moore\nMachine](https://en.wikipedia.org/wiki/Moore_machine) (DFA) using\n`aig2dfa`. Using the same example:\n\n```python\nfrom aiger_dfa import aig2dfa\n\nmy_dfa2 = aig2dfa(my_aig, relabels=relabels)\n```\n\nNote that the output of a sequential circuit (AIG) is dependent on the\nstate **AND** the action (a [Mealy\nMachine](https://en.wikipedia.org/wiki/Mealy_machine)). \n\nWe use the standard Mealy ↦ Moore reduction where one introduces a\n1-step delay on the output. The default initial output is `None`, but\ncan be set using the `initial_label` argument.\n",
     'author': 'Marcell Vazquez-Chanlatte',
     'author_email': 'mvc@linux.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mvcisback/py-aiger-dfa',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `py-aiger-dfa-0.4.1/PKG-INFO` & `py_aiger_dfa-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: py-aiger-dfa
-Version: 0.4.1
+Version: 0.4.2
 Summary: Library for moving between sequential circuits AIGs and DFAs.
 Home-page: https://github.com/mvcisback/py-aiger-dfa
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: mvc@linux.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: attrs (>=21.0.0,<22.0.0)
-Requires-Dist: bidict (>=0.21.0,<0.22.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22,<23)
+Requires-Dist: bidict (>=0.22.0,<0.23.0)
 Requires-Dist: dfa (>=4,<5)
 Requires-Dist: funcy (>=1.12,<2.0)
 Requires-Dist: py-aiger (>=6.0.0,<7.0.0)
-Requires-Dist: py-aiger-bv (>=4.7.4,<5.0.0)
+Requires-Dist: py-aiger-bv (>=4.7.6,<5.0.0)
 Requires-Dist: py-aiger-ptltl (>=3.0.0,<4.0.0)
-Requires-Dist: pyrsistent (>=0.18,<0.19)
+Requires-Dist: pyrsistent (>=0.19,<0.20)
 Project-URL: Repository, https://github.com/mvcisback/py-aiger-dfa
 Description-Content-Type: text/markdown
 
 # py-aiger-dfa
 Python library for converting between AIG circuits and DFAs.
 
 [![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-dfa/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-dfa)
```

