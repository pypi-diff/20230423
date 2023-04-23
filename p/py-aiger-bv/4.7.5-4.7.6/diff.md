# Comparing `tmp/py-aiger-bv-4.7.5.tar.gz` & `tmp/py_aiger_bv-4.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aiger-bv-4.7.5.tar", max compression
+gzip compressed data, was "py_aiger_bv-4.7.6.tar", max compression
```

## Comparing `py-aiger-bv-4.7.5.tar` & `py_aiger_bv-4.7.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/LICENSE
--rw-r--r--   0        0        0     8310 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/README.md
--rw-r--r--   0        0        0     1263 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/aiger_bv/__init__.py
--rw-r--r--   0        0        0     8455 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/aiger_bv/aigbv.py
--rw-r--r--   0        0        0     3219 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/aiger_bv/bundle.py
--rw-r--r--   0        0        0    13972 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/aiger_bv/common.py
--rw-r--r--   0        0        0     9013 2022-10-24 19:24:16.653280 py-aiger-bv-4.7.5/aiger_bv/expr.py
--rw-r--r--   0        0        0      632 2022-11-03 03:36:46.771600 py-aiger-bv-4.7.5/pyproject.toml
--rw-r--r--   0        0        0     9580 2022-11-03 03:37:23.773116 py-aiger-bv-4.7.5/setup.py
--rw-r--r--   0        0        0     9034 2022-11-03 03:37:23.774261 py-aiger-bv-4.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/LICENSE
+-rw-r--r--   0        0        0     8177 2022-11-03 04:14:43.656917 py_aiger_bv-4.7.6/README.md
+-rw-r--r--   0        0        0     1263 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/aiger_bv/__init__.py
+-rw-r--r--   0        0        0     8455 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/aiger_bv/aigbv.py
+-rw-r--r--   0        0        0     3219 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/aiger_bv/bundle.py
+-rw-r--r--   0        0        0    13972 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/aiger_bv/common.py
+-rw-r--r--   0        0        0     9013 2022-10-24 19:24:16.653280 py_aiger_bv-4.7.6/aiger_bv/expr.py
+-rw-r--r--   0        0        0      636 2023-04-23 06:45:39.670359 py_aiger_bv-4.7.6/pyproject.toml
+-rw-r--r--   0        0        0     9452 1970-01-01 00:00:00.000000 py_aiger_bv-4.7.6/setup.py
+-rw-r--r--   0        0        0     8952 1970-01-01 00:00:00.000000 py_aiger_bv-4.7.6/PKG-INFO
```

### Comparing `py-aiger-bv-4.7.5/LICENSE` & `py_aiger_bv-4.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/README.md` & `py_aiger_bv-4.7.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
   <img src="logo_text.svg" alt="py-aiger-bv logo" width=300px>
   <figcaption>pyAiger-BV: Extension of pyAiger for manipulating
     sequential bitvector circuits.</figcaption>
 </figure>
 
 
 [![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-bv/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-bv)
-[![codecov](https://codecov.io/gh/mvcisback/py-aiger-bv/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-bv)
 [![Docs](https://img.shields.io/badge/API-link-color)](https://mvcisback.github.io/py-aiger-bv)
 [![PyPI version](https://badge.fury.io/py/py-aiger-bv.svg)](https://badge.fury.io/py/py-aiger-bv)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  
 # Table of Contents
 - [About](#about-py-aiger-bv)
 - [Installation](#installation)
```

### Comparing `py-aiger-bv-4.7.5/aiger_bv/__init__.py` & `py_aiger_bv-4.7.6/aiger_bv/__init__.py`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/aiger_bv/aigbv.py` & `py_aiger_bv-4.7.6/aiger_bv/aigbv.py`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/aiger_bv/bundle.py` & `py_aiger_bv-4.7.6/aiger_bv/bundle.py`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/aiger_bv/common.py` & `py_aiger_bv-4.7.6/aiger_bv/common.py`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/aiger_bv/expr.py` & `py_aiger_bv-4.7.6/aiger_bv/expr.py`

 * *Files identical despite different names*

### Comparing `py-aiger-bv-4.7.5/pyproject.toml` & `py_aiger_bv-4.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "py-aiger-bv"
 readme="README.md"
-version = "4.7.5"
+version = "4.7.6"
 description = "A python library for manipulating sequential and-inverter gates."
 authors = ["Marcell Vazquez-Chanlatte <mvc@linux.com>"]
 license = "MIT"
 packages = [
     { include = "aiger_bv" },
 ]
 
@@ -13,15 +13,15 @@
 python = "^3.7"
 attrs = "^22"
 funcy = "^1.12"
 py-aiger = "^6.1.16"
 pyrsistent = "^0.19"
 
 [tool.poetry.dev-dependencies]
-hypothesis_cfg = {git = "git@github.com:mvcisback/hypothesis-cfg.git"}
+hypothesis_cfg = {git = "https://github.com/mvcisback/hypothesis-cfg.git"}
 hypothesis = "^6.0.0"
 pytest-xdist = "^3.0.0"
 pdoc3 = "^0.10"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `py-aiger-bv-4.7.5/setup.py` & `py_aiger_bv-4.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['attrs>=22,<23',
  'funcy>=1.12,<2.0',
  'py-aiger>=6.1.16,<7.0.0',
  'pyrsistent>=0.19,<0.20']
 
 setup_kwargs = {
     'name': 'py-aiger-bv',
-    'version': '4.7.5',
+    'version': '4.7.6',
     'description': 'A python library for manipulating sequential and-inverter gates.',
-    'long_description': '<figure>\n  <img src="logo_text.svg" alt="py-aiger-bv logo" width=300px>\n  <figcaption>pyAiger-BV: Extension of pyAiger for manipulating\n    sequential bitvector circuits.</figcaption>\n</figure>\n\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-bv/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-bv)\n[![codecov](https://codecov.io/gh/mvcisback/py-aiger-bv/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-bv)\n[![Docs](https://img.shields.io/badge/API-link-color)](https://mvcisback.github.io/py-aiger-bv)\n[![PyPI version](https://badge.fury.io/py/py-aiger-bv.svg)](https://badge.fury.io/py/py-aiger-bv)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n \n# Table of Contents\n- [About](#about-py-aiger-bv)\n- [Installation](#installation)\n- [BitVector Expr DSL](#bitvector-expression-dsl)\n- [Sequential Circuit DSL](#sequential-circuit-dsl)\n\n# About Py-Aiger-BV\n\nThis library provides word level abstractions on top of\n[py-aiger](https://github.com/mvcisback/py-aiger). This is done by the\n`AIGBV` which groups inputs, outputs, and latches into named\n**ordered** sequences, e.g. bitvectors.\n\nThe resulting objects can be turned into `AIG`s where each input,\noutput, or latches name has its index appended to its name. For example,\nan bitvector input, `\'x\'` with 3 bits becomes inputs `\'x[0]\', \'x[1]\', \'x[3]\'`\n\n\n# Installation\n\nIf you just need to use `aiger_bv`, you can just run:\n\n`$ pip install py-aiger-bv`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# BitVector Expression DSL\n\nAs in py-aiger, when writing combinatorial circuits, the Sequential\nCircuit DSL can be somewhat clumsy. For this common usecase, we have\ndeveloped the BitVector Expression DSL. This DSL actually consists of\ntwo DSLs for signed and unsigned BitVectors.  All circuits generated\nthis way have a single output word. We use a **big-endian** encoding\nwhere the most significant digit is the first element of the tuple\nrepresenting the word. For signed numbers, two\'s complement is used.\n\n```python\nimport aiger_bv\n\n# Create 16 bit variables.\nx = aiger_bv.atom(16, \'x\')\ny = aiger_bv.atom(16, \'y\', signed=True)  # Signed by default.\nz = aiger_bv.uatom(16, \'z\')              # Equiv to signed=False.\n\n# bitwise ops.\nexpr1 = x & y  # Bitwise and.\nexpr2 = x | y  # Bitwise or.\nexpr3 = x ^ y  # Bitwise xor.\nexpr4 = ~x  # Bitwise negation.\n\n# arithmetic\nexpr5 = x + y\nexpr6 = x - y\nexpr7 = x << y\nexpr8 = x >> y  # logical if unsigned, arithmetic if signed.\nexpr9 = -x  # Arithmetic negation. Only defined for signed expr.\nexpr10 = abs(x)\nexpr11 = x @ y  # inner product of bitvectors mod 2 (+ is xor).\n\n# comparison\nexpr12 = x == y\nexpr13 = x != y\nexpr14 = x < y\nexpr15 = x <= y\nexpr16 = x > y\nexpr17 = x >= y\n\n# Atoms can be constants.\nexpr18 = x & aiger_bv.atom(16, 3)\nexpr19 = x & aiger_bv.atom(16, 0xff)\n\n# BitVector expressions can be concatenated.\nexpr20 = x.concat(y)\n\n# Particular bits can be indexed to create new expressions.\nexpr21 = x[1]\n\n# Single bit expressions can be repeated.\nexpr22 = x[1].repeat(10)\n\n# And you can inspect the AIGBV if needed.\ncirc = x.aigbv\n\n# And you can inspect the AIG if needed.\ncirc = x.aigbv.aig\n\n# And of course, you can get a BoolExpr from a single output aig.\nexpr = aiger_bv.UnsignedBVExpr(circ)\n```\n\n# Sequential Circuit DSL\n\npy-aiger-bv\'s Sequential Circuit DSL implements the same basic api as\npy-aiger\'s Sequential Circuit DSL, but operates at the (variable\nlength) word level rather than the bit level.\n\n```python\nimport aiger\nimport aiger_bv\n\n\ncirc = ... # Create a circuit (see below).\n\n# We assume this circuit has word level\n# inputs: x,y, outputs: z, w, q, latches: a, b\nassert circ.inputs == {\'x\', \'y\'}\nassert circ.outputs == {\'z\', \'w\', \'q\'}\nassert circ.latches == {\'a\', \'b\'}\n```\n\n## Sequential composition\n```python\ncirc3 = circ1 >> circ2\n```\n\n## Parallel composition\n```python\ncirc3 = circ1 | circ2\n```\n\n## Adding Feedback (inserts a delay)\n```python\n# Connect output y to input x with delay (initialized to True).\n# (Default initialization is False.)\ncir2 = circ.feedback(\n    inputs=[\'x\'],\n    outputs=[\'y\'],\n    initials=[True],\n    keep_outputs=True\n)\n```\n\n## Relabeling\n```python\n# Relabel input \'x\' to \'z\'.\ncirc2 = circ[\'i\', {\'x\': \'z\'}]\n\n# Relabel output \'y\' to \'w\'.\ncirc2 = circ[\'o\', {\'y\': \'w\'}]\n\n# Relabel latches \'l1\' to \'l2\'.\ncirc2 = circ[\'l\', {\'l1\': \'l2\'}]\n```\n\n## Evaluation\n```python\n# Combinatoric evaluation.\ncirc(inputs={\'x\':(True, False, True), \'y\': (True, False)})\n\n# Sequential evaluation.\ncirc.simulate([\n        {\'x\': (True, False, True), \'y\': (True, False)},\n        {\'x\': (False, False, True), \'y\': (False, False)},\n    ])\n\n# Simulation Coroutine.\nsim = circ.simulator()  # Coroutine\nnext(sim)  # Initialize\nprint(sim.send({\'x\': (True, False, True), \'y\': (True, False)}))\nprint(sim.send({\'x\': (False, False, True), \'y\': (False, False)}))\n\n\n# Unroll\ncirc2 = circ.unroll(steps=10, init=True)\n```\n\n## aiger.AIG to aiger.AIGBV\n\nThere are two main ways to take an object `AIG` from `aiger` and\nconvert it into an `AIGBV` object. The first is the `aig2aigbv`\ncommand which simply makes all inputs words of size 1.\n\n\n```python\n# Create aiger_bv.AIGERBV object from aiger.AIG object.\ncirc  = ... # Some aiger.AIG object\nword_circ = aiger_bv.aig2aigbv(circ)  # aiger_bv.AIGBV object\n\n\n```\n\n## Gadget Library\n\n### General Manipulation\n\n```python\n# Copy outputs \'x\' and \'y\' to \'w1, w2\' and \'z1, z2\'.\ncirc1 = circ >> aiger_bv.tee(wordlen=3, iomap={\n        \'x\': (\'w1\', \'w2\'),\n        \'y\': (\'z1\', \'z2\')\n    })\n\n# Take 1 bit output, \'x\', duplicate it 5 times, and group into\n# a single 5-length word output, \'y\'.\ncirc2 = circ >> aiger_bv.repeat(wordlen=5, input=\'x\', output=\'z\')\n\n# Reverse order of a word.\ncirc3 = circ >> aiger_bv.reverse_gate(wordlen=5, input=\'x\', output=\'z\')\n\n# Sink and Source circuits (see encoding section for encoding details).\n## Always output binary encoding for 15. \ncirc4 = aiger_bv.source(wordlen=4, value=15, name=\'x\', signed=False)\n\n## Absorb output \'y\'\ncirc5 = circ >> aiger_bv.sink(wordlen=4, inputs=[\'y\'])\n\n# Identity Gate\ncirc6 = circ >> aiger_bv.identity_gate(wordlen=3, input=\'x\')\n\n# Combine/Concatenate words\ncirc7 = circ >> aiger_bv.combine_gate(\n    left_wordlen=3, left=\'x\',\n    right_wordlen=3, right=\'y\',\n    output=\'z\'\n)\n\n# Split words\ncirc8 = circ >> aiger_bv.split_gate(\n    input=\'x\',\n    left_wordlen=1, left=\'z\',\n    right_wordlen=2, right=\'w\'\n)\n\n# Select single index of circuit and make it a wordlen=1 output.\ncirc9 = circ >> aiger_bv.index_gate(wordlen=3, idx=1, input=\'x\', output=\'x1\')\n```\n\n## Bitwise Operations\n\n- `aiger_bv.bitwise_and(3, left=\'x\', right=\'y\', output=\'x&y\')`\n- `aiger_bv.bitwise_or(3, left=\'x\', right=\'y\', output=\'x|y\')`\n- `aiger_bv.bitwise_xor(3, left=\'x\', right=\'y\', output=\'x^y\')`\n- `aiger_bv.bitwise_negate(3, left=\'x\', output=\'~x\')`\n\n## Arithmetic\n\n- `aiger_bv.add_gate(3, left=\'x\', right=\'y\', output=\'x+y\')`\n- `aiger_bv.subtract_gate_gate(3, left=\'x\', right=\'y\', output=\'x-y\')`\n- `aiger_bv.inc_gate(3, left=\'x\', output=\'x+1\')`\n- `aiger_bv.dec_gate(3, left=\'x\', output=\'x+1\')`\n- `aiger_bv.negate_gate(3, left=\'x\', output=\'-x\')`\n- `aiger_bv.logical_right_shift(3, shift=1, input=\'x\', output=\'x>>1\')`\n- `aiger_bv.arithmetic_right_shift(3, shift=1, input=\'x\', output=\'x>>1\')`\n- `aiger_bv.left_shift(3, shift=1, input=\'x\', output=\'x<<1\')`\n\n## Comparison\n\n- `aiger_bv.is_nonzero_gate(3, input=\'x\', output=\'is_nonzero\')`\n- `aiger_bv.is_zero_gate(3, input=\'x\', output=\'is_zero\')`\n- `aiger_bv.eq_gate(3, left=\'x\', right=\'y\', output=\'x=y\')`\n- `aiger_bv.ne_gate(3, left=\'x\', right=\'y\', output=\'x!=y\')`\n- `aiger_bv.unsigned_lt_gate(3, left=\'x\', right=\'y\', output=\'x<y\')`\n- `aiger_bv.unsigned_gt_gate(3, left=\'x\', right=\'y\', output=\'x>y\')`\n- `aiger_bv.unsigned_le_gate(3, left=\'x\', right=\'y\', output=\'x<=y\')`\n- `aiger_bv.unsigned_ge_gate(3, left=\'x\', right=\'y\', output=\'x>=y\')`\n- `aiger_bv.signed_lt_gate(3, left=\'x\', right=\'y\', output=\'x<y\')`\n- `aiger_bv.signed_gt_gate(3, left=\'x\', right=\'y\', output=\'x>y\')`\n- `aiger_bv.signed_le_gate(3, left=\'x\', right=\'y\', output=\'x<=y\')`\n- `aiger_bv.signed_ge_gate(3, left=\'x\', right=\'y\', output=\'x>=y\')`\n',
+    'long_description': '<figure>\n  <img src="logo_text.svg" alt="py-aiger-bv logo" width=300px>\n  <figcaption>pyAiger-BV: Extension of pyAiger for manipulating\n    sequential bitvector circuits.</figcaption>\n</figure>\n\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-bv/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-bv)\n[![Docs](https://img.shields.io/badge/API-link-color)](https://mvcisback.github.io/py-aiger-bv)\n[![PyPI version](https://badge.fury.io/py/py-aiger-bv.svg)](https://badge.fury.io/py/py-aiger-bv)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n \n# Table of Contents\n- [About](#about-py-aiger-bv)\n- [Installation](#installation)\n- [BitVector Expr DSL](#bitvector-expression-dsl)\n- [Sequential Circuit DSL](#sequential-circuit-dsl)\n\n# About Py-Aiger-BV\n\nThis library provides word level abstractions on top of\n[py-aiger](https://github.com/mvcisback/py-aiger). This is done by the\n`AIGBV` which groups inputs, outputs, and latches into named\n**ordered** sequences, e.g. bitvectors.\n\nThe resulting objects can be turned into `AIG`s where each input,\noutput, or latches name has its index appended to its name. For example,\nan bitvector input, `\'x\'` with 3 bits becomes inputs `\'x[0]\', \'x[1]\', \'x[3]\'`\n\n\n# Installation\n\nIf you just need to use `aiger_bv`, you can just run:\n\n`$ pip install py-aiger-bv`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# BitVector Expression DSL\n\nAs in py-aiger, when writing combinatorial circuits, the Sequential\nCircuit DSL can be somewhat clumsy. For this common usecase, we have\ndeveloped the BitVector Expression DSL. This DSL actually consists of\ntwo DSLs for signed and unsigned BitVectors.  All circuits generated\nthis way have a single output word. We use a **big-endian** encoding\nwhere the most significant digit is the first element of the tuple\nrepresenting the word. For signed numbers, two\'s complement is used.\n\n```python\nimport aiger_bv\n\n# Create 16 bit variables.\nx = aiger_bv.atom(16, \'x\')\ny = aiger_bv.atom(16, \'y\', signed=True)  # Signed by default.\nz = aiger_bv.uatom(16, \'z\')              # Equiv to signed=False.\n\n# bitwise ops.\nexpr1 = x & y  # Bitwise and.\nexpr2 = x | y  # Bitwise or.\nexpr3 = x ^ y  # Bitwise xor.\nexpr4 = ~x  # Bitwise negation.\n\n# arithmetic\nexpr5 = x + y\nexpr6 = x - y\nexpr7 = x << y\nexpr8 = x >> y  # logical if unsigned, arithmetic if signed.\nexpr9 = -x  # Arithmetic negation. Only defined for signed expr.\nexpr10 = abs(x)\nexpr11 = x @ y  # inner product of bitvectors mod 2 (+ is xor).\n\n# comparison\nexpr12 = x == y\nexpr13 = x != y\nexpr14 = x < y\nexpr15 = x <= y\nexpr16 = x > y\nexpr17 = x >= y\n\n# Atoms can be constants.\nexpr18 = x & aiger_bv.atom(16, 3)\nexpr19 = x & aiger_bv.atom(16, 0xff)\n\n# BitVector expressions can be concatenated.\nexpr20 = x.concat(y)\n\n# Particular bits can be indexed to create new expressions.\nexpr21 = x[1]\n\n# Single bit expressions can be repeated.\nexpr22 = x[1].repeat(10)\n\n# And you can inspect the AIGBV if needed.\ncirc = x.aigbv\n\n# And you can inspect the AIG if needed.\ncirc = x.aigbv.aig\n\n# And of course, you can get a BoolExpr from a single output aig.\nexpr = aiger_bv.UnsignedBVExpr(circ)\n```\n\n# Sequential Circuit DSL\n\npy-aiger-bv\'s Sequential Circuit DSL implements the same basic api as\npy-aiger\'s Sequential Circuit DSL, but operates at the (variable\nlength) word level rather than the bit level.\n\n```python\nimport aiger\nimport aiger_bv\n\n\ncirc = ... # Create a circuit (see below).\n\n# We assume this circuit has word level\n# inputs: x,y, outputs: z, w, q, latches: a, b\nassert circ.inputs == {\'x\', \'y\'}\nassert circ.outputs == {\'z\', \'w\', \'q\'}\nassert circ.latches == {\'a\', \'b\'}\n```\n\n## Sequential composition\n```python\ncirc3 = circ1 >> circ2\n```\n\n## Parallel composition\n```python\ncirc3 = circ1 | circ2\n```\n\n## Adding Feedback (inserts a delay)\n```python\n# Connect output y to input x with delay (initialized to True).\n# (Default initialization is False.)\ncir2 = circ.feedback(\n    inputs=[\'x\'],\n    outputs=[\'y\'],\n    initials=[True],\n    keep_outputs=True\n)\n```\n\n## Relabeling\n```python\n# Relabel input \'x\' to \'z\'.\ncirc2 = circ[\'i\', {\'x\': \'z\'}]\n\n# Relabel output \'y\' to \'w\'.\ncirc2 = circ[\'o\', {\'y\': \'w\'}]\n\n# Relabel latches \'l1\' to \'l2\'.\ncirc2 = circ[\'l\', {\'l1\': \'l2\'}]\n```\n\n## Evaluation\n```python\n# Combinatoric evaluation.\ncirc(inputs={\'x\':(True, False, True), \'y\': (True, False)})\n\n# Sequential evaluation.\ncirc.simulate([\n        {\'x\': (True, False, True), \'y\': (True, False)},\n        {\'x\': (False, False, True), \'y\': (False, False)},\n    ])\n\n# Simulation Coroutine.\nsim = circ.simulator()  # Coroutine\nnext(sim)  # Initialize\nprint(sim.send({\'x\': (True, False, True), \'y\': (True, False)}))\nprint(sim.send({\'x\': (False, False, True), \'y\': (False, False)}))\n\n\n# Unroll\ncirc2 = circ.unroll(steps=10, init=True)\n```\n\n## aiger.AIG to aiger.AIGBV\n\nThere are two main ways to take an object `AIG` from `aiger` and\nconvert it into an `AIGBV` object. The first is the `aig2aigbv`\ncommand which simply makes all inputs words of size 1.\n\n\n```python\n# Create aiger_bv.AIGERBV object from aiger.AIG object.\ncirc  = ... # Some aiger.AIG object\nword_circ = aiger_bv.aig2aigbv(circ)  # aiger_bv.AIGBV object\n\n\n```\n\n## Gadget Library\n\n### General Manipulation\n\n```python\n# Copy outputs \'x\' and \'y\' to \'w1, w2\' and \'z1, z2\'.\ncirc1 = circ >> aiger_bv.tee(wordlen=3, iomap={\n        \'x\': (\'w1\', \'w2\'),\n        \'y\': (\'z1\', \'z2\')\n    })\n\n# Take 1 bit output, \'x\', duplicate it 5 times, and group into\n# a single 5-length word output, \'y\'.\ncirc2 = circ >> aiger_bv.repeat(wordlen=5, input=\'x\', output=\'z\')\n\n# Reverse order of a word.\ncirc3 = circ >> aiger_bv.reverse_gate(wordlen=5, input=\'x\', output=\'z\')\n\n# Sink and Source circuits (see encoding section for encoding details).\n## Always output binary encoding for 15. \ncirc4 = aiger_bv.source(wordlen=4, value=15, name=\'x\', signed=False)\n\n## Absorb output \'y\'\ncirc5 = circ >> aiger_bv.sink(wordlen=4, inputs=[\'y\'])\n\n# Identity Gate\ncirc6 = circ >> aiger_bv.identity_gate(wordlen=3, input=\'x\')\n\n# Combine/Concatenate words\ncirc7 = circ >> aiger_bv.combine_gate(\n    left_wordlen=3, left=\'x\',\n    right_wordlen=3, right=\'y\',\n    output=\'z\'\n)\n\n# Split words\ncirc8 = circ >> aiger_bv.split_gate(\n    input=\'x\',\n    left_wordlen=1, left=\'z\',\n    right_wordlen=2, right=\'w\'\n)\n\n# Select single index of circuit and make it a wordlen=1 output.\ncirc9 = circ >> aiger_bv.index_gate(wordlen=3, idx=1, input=\'x\', output=\'x1\')\n```\n\n## Bitwise Operations\n\n- `aiger_bv.bitwise_and(3, left=\'x\', right=\'y\', output=\'x&y\')`\n- `aiger_bv.bitwise_or(3, left=\'x\', right=\'y\', output=\'x|y\')`\n- `aiger_bv.bitwise_xor(3, left=\'x\', right=\'y\', output=\'x^y\')`\n- `aiger_bv.bitwise_negate(3, left=\'x\', output=\'~x\')`\n\n## Arithmetic\n\n- `aiger_bv.add_gate(3, left=\'x\', right=\'y\', output=\'x+y\')`\n- `aiger_bv.subtract_gate_gate(3, left=\'x\', right=\'y\', output=\'x-y\')`\n- `aiger_bv.inc_gate(3, left=\'x\', output=\'x+1\')`\n- `aiger_bv.dec_gate(3, left=\'x\', output=\'x+1\')`\n- `aiger_bv.negate_gate(3, left=\'x\', output=\'-x\')`\n- `aiger_bv.logical_right_shift(3, shift=1, input=\'x\', output=\'x>>1\')`\n- `aiger_bv.arithmetic_right_shift(3, shift=1, input=\'x\', output=\'x>>1\')`\n- `aiger_bv.left_shift(3, shift=1, input=\'x\', output=\'x<<1\')`\n\n## Comparison\n\n- `aiger_bv.is_nonzero_gate(3, input=\'x\', output=\'is_nonzero\')`\n- `aiger_bv.is_zero_gate(3, input=\'x\', output=\'is_zero\')`\n- `aiger_bv.eq_gate(3, left=\'x\', right=\'y\', output=\'x=y\')`\n- `aiger_bv.ne_gate(3, left=\'x\', right=\'y\', output=\'x!=y\')`\n- `aiger_bv.unsigned_lt_gate(3, left=\'x\', right=\'y\', output=\'x<y\')`\n- `aiger_bv.unsigned_gt_gate(3, left=\'x\', right=\'y\', output=\'x>y\')`\n- `aiger_bv.unsigned_le_gate(3, left=\'x\', right=\'y\', output=\'x<=y\')`\n- `aiger_bv.unsigned_ge_gate(3, left=\'x\', right=\'y\', output=\'x>=y\')`\n- `aiger_bv.signed_lt_gate(3, left=\'x\', right=\'y\', output=\'x<y\')`\n- `aiger_bv.signed_gt_gate(3, left=\'x\', right=\'y\', output=\'x>y\')`\n- `aiger_bv.signed_le_gate(3, left=\'x\', right=\'y\', output=\'x<=y\')`\n- `aiger_bv.signed_ge_gate(3, left=\'x\', right=\'y\', output=\'x>=y\')`\n',
     'author': 'Marcell Vazquez-Chanlatte',
     'author_email': 'mvc@linux.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `py-aiger-bv-4.7.5/PKG-INFO` & `py_aiger_bv-4.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: py-aiger-bv
-Version: 4.7.5
+Version: 4.7.6
 Summary: A python library for manipulating sequential and-inverter gates.
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: mvc@linux.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22,<23)
 Requires-Dist: funcy (>=1.12,<2.0)
 Requires-Dist: py-aiger (>=6.1.16,<7.0.0)
 Requires-Dist: pyrsistent (>=0.19,<0.20)
 Description-Content-Type: text/markdown
 
 <figure>
   <img src="logo_text.svg" alt="py-aiger-bv logo" width=300px>
   <figcaption>pyAiger-BV: Extension of pyAiger for manipulating
     sequential bitvector circuits.</figcaption>
 </figure>
 
 
 [![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-bv/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-bv)
-[![codecov](https://codecov.io/gh/mvcisback/py-aiger-bv/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-bv)
 [![Docs](https://img.shields.io/badge/API-link-color)](https://mvcisback.github.io/py-aiger-bv)
 [![PyPI version](https://badge.fury.io/py/py-aiger-bv.svg)](https://badge.fury.io/py/py-aiger-bv)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  
 # Table of Contents
 - [About](#about-py-aiger-bv)
 - [Installation](#installation)
```

