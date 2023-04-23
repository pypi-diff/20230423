# Comparing `tmp/py_aiger-6.2.0.tar.gz` & `tmp/py_aiger-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_aiger-6.2.0.tar", max compression
+gzip compressed data, was "py_aiger-6.2.1.tar", max compression
```

## Comparing `py_aiger-6.2.0.tar` & `py_aiger-6.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1082 2023-01-14 22:42:34.194862 py_aiger-6.2.0/LICENSE
--rw-r--r--   0        0        0     8426 2023-01-14 22:42:34.194862 py_aiger-6.2.0/README.md
--rw-r--r--   0        0        0      287 2023-01-14 22:42:34.194862 py_aiger-6.2.0/aiger/__init__.py
--rw-r--r--   0        0        0     8110 2023-01-14 22:58:49.477589 py_aiger-6.2.0/aiger/aig.py
--rw-r--r--   0        0        0     4951 2023-01-14 22:42:34.194862 py_aiger-6.2.0/aiger/common.py
--rw-r--r--   0        0        0     2253 2023-01-14 22:42:34.194862 py_aiger-6.2.0/aiger/expr.py
--rw-r--r--   0        0        0      148 2023-01-14 22:42:34.194862 py_aiger-6.2.0/aiger/hypothesis.py
--rw-r--r--   0        0        0    15682 2023-01-14 22:42:34.194862 py_aiger-6.2.0/aiger/lazy.py
--rwxr-xr-x   0        0        0    10626 2023-01-14 23:16:35.217171 py_aiger-6.2.0/aiger/parser.py
--rw-r--r--   0        0        0     2735 2023-01-14 22:42:34.195861 py_aiger-6.2.0/aiger/writer.py
--rw-r--r--   0        0        0      770 2023-01-14 23:27:05.498436 py_aiger-6.2.0/pyproject.toml
--rw-r--r--   0        0        0     9622 1970-01-01 00:00:00.000000 py_aiger-6.2.0/setup.py
--rw-r--r--   0        0        0     9414 1970-01-01 00:00:00.000000 py_aiger-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-24 19:21:50.121815 py_aiger-6.2.1/LICENSE
+-rw-r--r--   0        0        0     8426 2022-10-24 19:21:50.121815 py_aiger-6.2.1/README.md
+-rw-r--r--   0        0        0      287 2022-10-24 19:21:50.121815 py_aiger-6.2.1/aiger/__init__.py
+-rw-r--r--   0        0        0     8110 2023-04-23 06:31:21.206553 py_aiger-6.2.1/aiger/aig.py
+-rw-r--r--   0        0        0     4951 2022-10-24 19:21:50.122815 py_aiger-6.2.1/aiger/common.py
+-rw-r--r--   0        0        0     2253 2022-10-24 19:21:50.122815 py_aiger-6.2.1/aiger/expr.py
+-rw-r--r--   0        0        0      148 2022-10-24 19:21:50.122815 py_aiger-6.2.1/aiger/hypothesis.py
+-rw-r--r--   0        0        0    15682 2022-10-24 19:21:50.122815 py_aiger-6.2.1/aiger/lazy.py
+-rwxr-xr-x   0        0        0    10626 2023-04-23 06:31:21.206553 py_aiger-6.2.1/aiger/parser.py
+-rw-r--r--   0        0        0     2735 2022-10-24 19:21:50.122815 py_aiger-6.2.1/aiger/writer.py
+-rw-r--r--   0        0        0      769 2023-04-23 06:33:46.703158 py_aiger-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9622 1970-01-01 00:00:00.000000 py_aiger-6.2.1/setup.py
+-rw-r--r--   0        0        0     9414 1970-01-01 00:00:00.000000 py_aiger-6.2.1/PKG-INFO
```

### Comparing `py_aiger-6.2.0/LICENSE` & `py_aiger-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/README.md` & `py_aiger-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/aig.py` & `py_aiger-6.2.1/aiger/aig.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/common.py` & `py_aiger-6.2.1/aiger/common.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/expr.py` & `py_aiger-6.2.1/aiger/expr.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/lazy.py` & `py_aiger-6.2.1/aiger/lazy.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/parser.py` & `py_aiger-6.2.1/aiger/parser.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/aiger/writer.py` & `py_aiger-6.2.1/aiger/writer.py`

 * *Files identical despite different names*

### Comparing `py_aiger-6.2.0/pyproject.toml` & `py_aiger-6.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "py-aiger"
 readme="README.md"
-version = "6.2.0"
+version = "6.2.1"
 repository = "https://github.com/mvcisback/py-aiger"
 description = "A python library for manipulating sequential and-inverter gates."
 authors = ["Marcell Vazquez-Chanlatte <marcell.vc@eecs.berkeley.edu>"]
 license = "MIT"
 packages = [
     { include = "aiger" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-attrs = "^22"
+attrs = "^23"
 bidict = "^0.22.0"
 funcy = "^1.12"
 toposort = "^1.5"
 pyrsistent = "^0.19.0"
 sortedcontainers = "^2.3.0"
 
 [tool.poetry.dev-dependencies]
 hypothesis_cfg = {git = "https://github.com/mvcisback/hypothesis-cfg.git"}
 hypothesis = "^6"
 pytest-xdist = "^3"
 py-aiger-ptltl = "^3.1.0"
-parsimonious = "^0.8.1"
+parsimonious = "^0.10"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `py_aiger-6.2.0/setup.py` & `py_aiger-6.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['aiger']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=22,<23',
+['attrs>=23,<24',
  'bidict>=0.22.0,<0.23.0',
  'funcy>=1.12,<2.0',
  'pyrsistent>=0.19.0,<0.20.0',
  'sortedcontainers>=2.3.0,<3.0.0',
  'toposort>=1.5,<2.0']
 
 setup_kwargs = {
     'name': 'py-aiger',
-    'version': '6.2.0',
+    'version': '6.2.1',
     'description': 'A python library for manipulating sequential and-inverter gates.',
     'long_description': '<figure>\n  <img src="assets/logo_text.svg" alt="py-aiger logo" width=300px>\n  <figcaption>\n      pyAiger: A python library for manipulating sequential and\n      combinatorial circuits.\n  </figcaption>\n\n</figure>\n\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger/status.svg)](https://cloud.drone.io/mvcisback/py-aiger)\n[![codecov](https://codecov.io/gh/mvcisback/py-aiger/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger)\n[![PyPI version](https://badge.fury.io/py/py-aiger.svg)](https://badge.fury.io/py/py-aiger)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1405781.svg)](https://doi.org/10.5281/zenodo.1405781)\n\n<!-- markdown-toc start - Don\'t edit this section. Run M-x markdown-toc-generate-toc again -->\n**Table of Contents**\n\n- [About PyAiger](#about-pyaiger)\n- [Installation](#installation)\n- [Boolean Expression DSL](#boolean-expression-dsl)\n- [Sequential Circuit DSL](#sequential-circuit-dsl)\n    - [Sequential composition](#sequential-composition)\n    - [Parallel composition](#parallel-composition)\n    - [Circuits with Latches/Feedback/Delay](#circuits-with-latchesfeedbackdelay)\n    - [Relabeling](#relabeling)\n    - [Evaluation](#evaluation)\n    - [Useful circuits](#useful-circuits)\n- [Extra](#extra)\n- [Ecosystem](#ecosystem)\n- [Related Projects](#related-projects)\n- [Citing](#citing)\n\n<!-- markdown-toc end -->\n\n\n# About PyAiger\n\n1. Q: How is Py-Aiger pronounced? A: Like "pie" + "grrr".\n2. Q: Why python? Aren\'t you worried about performance?! A: No. The goals of this library are ease of use and hackability. \n3. Q: No, I\'m really concerned about performance! A: This library is not suited to implement logic solvers. For everything else, such as the creation and manipulation of circuits with many thousands of gates in between solver calls, the library is really fast enough.\n4. Q: Where does the name come from? A: <a href="http://fmv.jku.at/aiger/">Aiger</a> is a popular circuit format. The format is used in <a href="http://fmv.jku.at/hwmcc17/">hardware model checking</a>, <a href="http://www.syntcomp.org/">synthesis</a>, and is supported by <a href="https://github.com/berkeley-abc/abc">ABC</a>. The name is a combination of AIG (standing for <a href="https://en.wikipedia.org/wiki/And-inverter_graph">And-Inverter-Graph</a>) and the mountain <a href="https://en.wikipedia.org/wiki/Eiger">Eiger</a>.\n\n# Installation\n\nIf you just need to use `aiger`, you can just run:\n\n`$ pip install py-aiger`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# Usage\n\n```\nimport aiger\n\nx, y, z, w = aiger.atoms(\'x\', \'y\', \'z\', \'w\')\n\nexpr1 = z.implies(x & y)\nexpr2 = z & w\n\ncirc1 = expr1.with_output(\'z\') \\      # Get AIG for expr1 with output \'z\'.\n             .aig\ncirc2 = circ1 >> circ2                # Feed outputs of circ1 into circ2.\n```\n\n# Boolean Expression DSL\nWhile powerful, when writing combinatorial circuits, the Sequential\nCircuit DSL can be somewhat clumsy. For this common usecase, we have\ndeveloped the Boolean Expression DSL. All circuits generated this way\nhave a single output.\n\n```python\nimport aiger\nx, y, z = aiger.atoms(\'x\', \'y\', \'z\')\nexpr1 = x & y  # circuit with inputs \'x\', \'y\' and 1 output computing x AND y.\nexpr2 = x | y  # logical or.\nexpr3 = x ^ y  # logical xor.\nexpr4 = x == y  # logical ==, xnor.\nexpr5 = x.implies(y)\nexpr6 = ~x  # logical negation.\nexpr7 = aiger.ite(x, y, z)  # if x then y else z.\n\n# Atoms can be constants.\nexpr8 = x & True  # Equivalent to just x.\nexpr9 = x & False # Equivalent to const False.\n\n# Specifying output name of boolean expression.\n# - Output is a long uuid otherwise.\nexpr10 = expr5.with_output(\'x_implies_y\')\nassert expr10.output == \'x_implies_y\'\n\n# And you can inspect the AIG if needed.\ncirc = x.aig\n\n# And of course, you can get a BoolExpr from a single output aig.\nexpr10 = aiger.BoolExpr(circ)\n```\n\n\n# Sequential Circuit DSL\n\n```python\nimport aiger\nfrom aiger import utils\n\n# Parser for ascii AIGER format.\naig1 = aiger.load(path_to_aig1_file.aag)\naig2 = aiger.load(path_to_aig2_file.aag)\n```\n\n## Sequential composition\n```python\naig3 = aig1 >> aig2\n```\n\n## Parallel composition\n```python\naig4 = aig1 | aig2\n```\n\n## Circuits with Latches and Delayed Feedback\nSometimes one requires some outputs to be feed back into the circuits\nas time delayed inputs. This can be accomplished using the `loopback`\nmethod. This method takes in a variable number of dictionaries\nencoding how to wire an input to an output. The wiring dictionaries\nwith the following keys and default values:\n\n| Key         | Default | Meaning                          |\n| ----------- | ------- | -------------------------------- |\n| input       |         | Input port                       |\n| output      |         | Output port                      |\n| latch       | input   | Latch name                       |\n| init        | True    | Initial latch value              |\n| keep_output | True    | Keep loopbacked output as output |\n\n\n```python\n# Connect output y to input x with delay, initialized to True.\n# (Default initialization is False.)\naig5 = aig1.loopback({\n  "input": "x", "output": "y",\n})\n\naig6 = aig1.loopback({\n  "input": "x", "output": "y",\n}, {\n  "input": "z", "output": "z", "latch": "z_latch",\n  "init": False, "keep_outputs": False\n})\n\n```\n\n## Relabeling\n\nThere are two syntaxes for relabeling. The first uses indexing\nsyntax in a nod to [notation often used variable substition in math](https://mathoverflow.net/questions/243084/history-of-the-notation-for-substitution).\n\nThe syntax is the relabel method, which is preferable when one wants\nto be explicit, even for those not familar with `py-aiger`.\n\n```python\n# Relabel input \'x\' to \'z\'.\naig1[\'i\', {\'x\': \'z\'}]\naig1.relabel(\'input\', {\'x\': \'z\'})\n\n# Relabel output \'y\' to \'w\'.\naig1[\'o\', {\'y\': \'w\'}]\naig1.relabel(\'output\', {\'y\': \'w\'})\n\n# Relabel latches \'l1\' to \'l2\'.\naig1[\'l\', {\'l1\': \'l2\'}]\naig1.relabel(\'latch\', {\'l1\': \'l2\'})\n```\n\n## Evaluation\n```python\n# Combinatoric evaluation.\naig3(inputs={\'x\':True, \'y\':False})\n\n# Sequential evaluation.\nsim = aig3.simulate([{\'x\': 0, \'y\': 0}, \n                    {\'x\': 1, \'y\': 2},\n                    {\'x\': 3, \'y\': 4}])\n\n# Simulation Coroutine\nsim = aig3.simulator()  # Coroutine\nnext(sim)  # Initialize\nprint(sim.send({\'x\': 0, \'y\': 0}))\nprint(sim.send({\'x\': 1, \'y\': 2}))\nprint(sim.send({\'x\': 3, \'y\': 4}))\n\n\n# Unroll\naig4 = aig3.unroll(steps=10, init=True)\n```\n\n## Useful circuits\n```python\n# Fix input x to be False.\naig4 = aiger.source({\'x\': False}) >> aig3\n\n# Remove output y. \naig4 = aig3 >> aiger.sink([\'y\'])\n\n# Create duplicate w of output y.\naig4 = aig3 >> aiger.tee({\'y\': [\'y\', \'w\']})\n```\n\n# Extra\n```python\naiger.common.eval_order(aig1)  # Returns topological ordering of circuit gates.\n\n# Convert object into an AIG from multiple formats including BoolExpr, AIG, str, and filepaths.\naiger.to_aig(aig1)\n```\n\n# Ecosystem\n\n### Stable\n- [py-aiger-bv](https://github.com/mvcisback/py-aiger-bv): Extension of pyAiger for manipulating sequential bitvector circuits.\n- [py-aiger-cnf](https://github.com/mvcisback/py-aiger-cnf): BoolExpr to Object representing CNF. Mostly used for interfacing with py-aiger-sat.\n- [py-aiger-past-ltl](https://github.com/mvcisback/py-aiger-past-ltl): Converts Past Linear Temporal Logic to aiger circuits.\n- [py-aiger-coins](https://github.com/mvcisback/py-aiger-coins): Library for creating circuits that encode discrete distributions.\n- [py-aiger-sat](https://github.com/mvcisback/py-aiger-sat): Bridge between py-aiger and py-sat.\n- [py-aiger-bdd](https://github.com/mvcisback/py-aiger-bdd): Aiger <-> BDD bridge.\n- [py-aiger-gridworld](https://github.com/mvcisback/py-aiger-gridworld): Create aiger circuits representing gridworlds.\n- [py-aiger-dfa](https://pypi.org/project/py-aiger-dfa/): Convert between finite automata and sequential circuits.\n\n\n### Underdevelopment\n\n\n- [py-aiger-spectral](https://github.com/mvcisback/py-aiger-spectral): A tool for performing (Fourier) Analysis of Boolean Functions.\n- [py-aiger-abc](https://pypi.org/project/py-aiger-abc/): Aiger and abc bridge.\n\n# Related Projects\n- [pyAig](https://github.com/sterin/pyaig): Another python library\n  for working with AIGER circuits.\n',
     'author': 'Marcell Vazquez-Chanlatte',
     'author_email': 'marcell.vc@eecs.berkeley.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mvcisback/py-aiger',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['aiger']
-package_data = \ {'': ['*']} install_requires = \ ['attrs>=22,<23',
+package_data = \ {'': ['*']} install_requires = \ ['attrs>=23,<24',
 'bidict>=0.22.0,<0.23.0', 'funcy>=1.12,<2.0', 'pyrsistent>=0.19.0,<0.20.0',
 'sortedcontainers>=2.3.0,<3.0.0', 'toposort>=1.5,<2.0'] setup_kwargs =
-{ 'name': 'py-aiger', 'version': '6.2.0', 'description': 'A python library for
+{ 'name': 'py-aiger', 'version': '6.2.1', 'description': 'A python library for
 manipulating sequential and-inverter gates.', 'long_description': '\n [py-aiger
 logo]\n \n pyAiger: A python library for manipulating sequential and\n
 combinatorial circuits.\n \n\n\n\n\n[![Build Status](https://cloud.drone.io/
 api/badges/mvcisback/py-aiger/status.svg)](https://cloud.drone.io/mvcisback/py-
 aiger)\n[![codecov](https://codecov.io/gh/mvcisback/py-aiger/branch/master/
 graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger)\n[![PyPI version]
 (https://badge.fury.io/py/py-aiger.svg)](https://badge.fury.io/py/py-aiger)\n[!
```

### Comparing `py_aiger-6.2.0/PKG-INFO` & `py_aiger-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py-aiger
-Version: 6.2.0
+Version: 6.2.1
 Summary: A python library for manipulating sequential and-inverter gates.
 Home-page: https://github.com/mvcisback/py-aiger
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: marcell.vc@eecs.berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22,<23)
+Requires-Dist: attrs (>=23,<24)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
 Requires-Dist: funcy (>=1.12,<2.0)
 Requires-Dist: pyrsistent (>=0.19.0,<0.20.0)
 Requires-Dist: sortedcontainers (>=2.3.0,<3.0.0)
 Requires-Dist: toposort (>=1.5,<2.0)
 Project-URL: Repository, https://github.com/mvcisback/py-aiger
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: py-aiger Version: 6.2.0 Summary: A python library
+Metadata-Version: 2.1 Name: py-aiger Version: 6.2.1 Summary: A python library
 for manipulating sequential and-inverter gates. Home-page: https://github.com/
 mvcisback/py-aiger License: MIT Author: Marcell Vazquez-Chanlatte Author-email:
 marcell.vc@eecs.berkeley.edu Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: attrs (>=22,<23) Requires-Dist:
+Language :: Python :: 3.11 Requires-Dist: attrs (>=23,<24) Requires-Dist:
 bidict (>=0.22.0,<0.23.0) Requires-Dist: funcy (>=1.12,<2.0) Requires-Dist:
 pyrsistent (>=0.19.0,<0.20.0) Requires-Dist: sortedcontainers (>=2.3.0,<3.0.0)
 Requires-Dist: toposort (>=1.5,<2.0) Project-URL: Repository, https://
 github.com/mvcisback/py-aiger Description-Content-Type: text/markdown  [py-
 aiger logo]  pyAiger: A python library for manipulating sequential and
 combinatorial circuits.   [![Build Status](https://cloud.drone.io/api/badges/
 mvcisback/py-aiger/status.svg)](https://cloud.drone.io/mvcisback/py-aiger) [!
```

