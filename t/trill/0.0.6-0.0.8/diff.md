# Comparing `tmp/trill-0.0.6.tar.gz` & `tmp/trill-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trill-0.0.6.tar", last modified: Sat Mar 18 21:46:16 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `trill-0.0.6.tar` & `trill-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-03-18 21:46:16.137287 trill-0.0.6/
--rw-r--r--   0 greger    (1000) greger    (1000)     1069 2023-02-24 08:08:36.000000 trill-0.0.6/LICENSE
--rw-r--r--   0 greger    (1000) greger    (1000)     3870 2023-03-18 21:46:16.137287 trill-0.0.6/PKG-INFO
--rw-r--r--   0 greger    (1000) greger    (1000)     2316 2023-03-18 21:45:08.000000 trill-0.0.6/README.md
--rw-r--r--   0 greger    (1000) greger    (1000)     1080 2023-03-18 21:45:53.000000 trill-0.0.6/pyproject.toml
--rw-r--r--   0 greger    (1000) greger    (1000)       38 2023-03-18 21:46:16.137287 trill-0.0.6/setup.cfg
--rw-r--r--   0 greger    (1000) greger    (1000)       38 2023-02-24 08:08:36.000000 trill-0.0.6/setup.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-03-18 21:46:16.127287 trill-0.0.6/src/
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-03-18 21:46:16.136287 trill-0.0.6/src/trill/
--rw-r--r--   0 greger    (1000) greger    (1000)      539 2023-03-04 08:40:07.000000 trill-0.0.6/src/trill/__init__.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-03-18 21:46:16.137287 trill-0.0.6/src/trill/ast/
--rw-r--r--   0 greger    (1000) greger    (1000)        0 2022-08-09 09:08:09.000000 trill-0.0.6/src/trill/ast/__init__.py
--rw-r--r--   0 greger    (1000) greger    (1000)      792 2023-03-04 15:16:22.000000 trill-0.0.6/src/trill/ast/base.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1562 2023-03-15 22:26:04.000000 trill-0.0.6/src/trill/ast/expression.py
--rw-r--r--   0 greger    (1000) greger    (1000)     3358 2023-03-15 22:26:04.000000 trill-0.0.6/src/trill/ast/printer.py
--rw-r--r--   0 greger    (1000) greger    (1000)      486 2023-03-04 15:16:22.000000 trill-0.0.6/src/trill/ast/statement.py
--rw-r--r--   0 greger    (1000) greger    (1000)      885 2022-08-20 09:10:30.000000 trill-0.0.6/src/trill/error.py
--rw-r--r--   0 greger    (1000) greger    (1000)    17650 2023-03-18 21:45:08.000000 trill-0.0.6/src/trill/interpreter.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1445 2023-03-18 21:45:08.000000 trill-0.0.6/src/trill/main.py
--rw-r--r--   0 greger    (1000) greger    (1000)    18932 2023-03-18 21:45:08.000000 trill-0.0.6/src/trill/parser.py
--rw-r--r--   0 greger    (1000) greger    (1000)      917 2022-08-20 21:38:04.000000 trill-0.0.6/src/trill/reserved.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1884 2023-03-15 22:26:04.000000 trill-0.0.6/src/trill/string.py
--rw-r--r--   0 greger    (1000) greger    (1000)     7438 2023-03-15 22:26:04.000000 trill-0.0.6/src/trill/tokenizer.py
--rw-r--r--   0 greger    (1000) greger    (1000)     2757 2023-03-15 22:26:04.000000 trill-0.0.6/src/trill/tokens.py
--rw-r--r--   0 greger    (1000) greger    (1000)      124 2023-03-04 16:10:56.000000 trill-0.0.6/src/trill/types.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-03-18 21:46:16.136287 trill-0.0.6/src/trill.egg-info/
--rw-r--r--   0 greger    (1000) greger    (1000)     3870 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/PKG-INFO
--rw-r--r--   0 greger    (1000) greger    (1000)      577 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/SOURCES.txt
--rw-r--r--   0 greger    (1000) greger    (1000)        1 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/dependency_links.txt
--rw-r--r--   0 greger    (1000) greger    (1000)       41 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/entry_points.txt
--rw-r--r--   0 greger    (1000) greger    (1000)       13 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/requires.txt
--rw-r--r--   0 greger    (1000) greger    (1000)        6 2023-03-18 21:46:16.000000 trill-0.0.6/src/trill.egg-info/top_level.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 trill-0.0.8/.env
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 trill-0.0.8/Makefile
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 trill-0.0.8/_version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 trill-0.0.8/requirements-dev.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 trill-0.0.8/rolls.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trill-0.0.8/setup.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 trill-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 trill-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 trill-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 trill-0.0.8/examples/rolls.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/error.py
+-rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/interpreter.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/main.py
+-rw-r--r--   0        0        0    19895 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/parser.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/reserved.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/string.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tokenizer.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tokens.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/base.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/expression.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/printer.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/statement.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/__init__.py
+-rw-r--r--   0        0        0    10634 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/cases.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_errors.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_interpreter.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_parser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_string.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_syntax_tree.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_tokenizer.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 trill-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 trill-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 trill-0.0.8/README.md
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 trill-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 trill-0.0.8/PKG-INFO
```

### Comparing `trill-0.0.6/LICENSE` & `trill-0.0.8/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Greger Stolt Nilsen
+Copyright © 2022-2023 Greger Stolt Nilsen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `trill-0.0.6/PKG-INFO` & `trill-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: trill
-Version: 0.0.6
+Version: 0.0.8
 Summary: Troll language parser and interpreter.
+Project-URL: Homepage, https://github.com/gregersn/Trill
 Author-email: Greger Stolt Nilsen <gregersn@gmail.com>
-License: Copyright © 2022 Greger Stolt Nilsen
+License: Copyright © 2022-2023 Greger Stolt Nilsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://github.com/gregersn/Trill
-Keywords: troll,dice,interpreter
-Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Keywords: dice,interpreter,troll
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: typer>=0.6.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Trill is a Troll interpreter
 
 Implemented in Python both as a package and for command line use.
 
 Troll is a dice roll language made by Torben Mogensen  
 http://hjemmesider.diku.dk/~torbenm/Troll/
@@ -90,15 +91,15 @@
 - [x] logical and ( & )
 - [x] logical not ( ! )
 - [x] bind x to value of e1 in e2 ( _x := e1; e2_ )
 - [x] _foreach x in e1 do e2_
 - [x] _repeat x := e1 while/until e2_
 - [x] _accumulate x := e1 while/until e2_
 - [x] _function_
-- [ ] _compositional_
+- [x] _compositional_
 - [x] _call_
 - [x] text box of single sample ( ' )
 - [x] text box of n samples ( n ' )
 - [x] combine text boxes horisontally ( || )
 - [x] combine text boxes vertically, left-aligned ( |> )
 - [x] combine text boxes vertically, right-aligned ( <| )
 - [x] combine text boxes, centre-aligned ( <> )
```

### Comparing `trill-0.0.6/README.md` & `trill-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 - [x] logical and ( & )
 - [x] logical not ( ! )
 - [x] bind x to value of e1 in e2 ( _x := e1; e2_ )
 - [x] _foreach x in e1 do e2_
 - [x] _repeat x := e1 while/until e2_
 - [x] _accumulate x := e1 while/until e2_
 - [x] _function_
-- [ ] _compositional_
+- [x] _compositional_
 - [x] _call_
 - [x] text box of single sample ( ' )
 - [x] text box of n samples ( n ' )
 - [x] combine text boxes horisontally ( || )
 - [x] combine text boxes vertically, left-aligned ( |> )
 - [x] combine text boxes vertically, right-aligned ( <| )
 - [x] combine text boxes, centre-aligned ( <> )
```

### Comparing `trill-0.0.6/pyproject.toml` & `trill-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-requirements-txt", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "_version.py"
 
 [project]
 name = "trill"
-version = "0.0.6"
+dynamic = ["version"]
+
 description = "Troll language parser and interpreter."
 readme = "README.md"
 authors = [
   { name = "Greger Stolt Nilsen", email = "gregersn@gmail.com" },
 ]
 license = { file ="LICENSE" }
 classifiers = [
```

### Comparing `trill-0.0.6/src/trill/ast/base.py` & `trill-0.0.8/src/trill/ast/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 """Base AST classes and types."""
+import sys
 from dataclasses import dataclass
-from typing import Any, TypeVar, Generic
+import random
+from typing import Any, Optional, TypeVar, Generic
 
 T = TypeVar('T')
 
+
 class UnknownNodeType(Exception):
     """Unknown node type."""
 
 
 class Visitor(Generic[T]):
     """Visitor base class."""
 
+    def __init__(self, seed: Optional[int] = None):
+        if seed is None:
+            seed = random.randrange(sys.maxsize)
+        random.seed(seed)
+
     def visit_generic(self, node: 'Node'):
         """Visit a generic node."""
         raise UnknownNodeType(f"No visit_{type(node).__name__} method")
 
 
 @dataclass
 class Node:
```

### Comparing `trill-0.0.6/src/trill/ast/expression.py` & `trill-0.0.8/src/trill/ast/expression.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.6/src/trill/ast/printer.py` & `trill-0.0.8/src/trill/ast/printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,15 +73,23 @@
     def visit_Function_Statement(self, stmt: statement.Function):
         name = stmt.name
         parameters = stmt.parameters
         expr = stmt.expression
 
         return self.parenthesize(f"function {name.literal} ({','.join(p.literal for p in parameters)})", expr)
 
+    def visit_Compositional_Statement(self, stmt: statement.Compositional):
+        name = stmt.name
+        empty = stmt.empty
+        singleton = stmt.singleton
+        union = stmt.union
+
+        return self.parenthesize(f"compositional {name.literal} {empty.value} {singleton.literal} {union.literal}")
+
     def visit_Print_Statement(self, stmt: statement.Print):
         repeats = stmt.repeats
         expr = stmt.expression
 
         return self.parenthesize(f"textbox {repeats}", expr)
-    
+
     def visit_TextAlign_Expression(self, expr: expression.TextAlign):
         return self.parenthesize('textalign', expr.left, expr.right)
```

### Comparing `trill-0.0.6/src/trill/error.py` & `trill-0.0.8/src/trill/error.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.6/src/trill/interpreter.py` & `trill-0.0.8/src/trill/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import ChainMap, Dict, Iterable, Sequence, TypeVar, List, Any, Union, cast
 import random
 from trill.string import process_string
 
 from trill.types import Number, NumberList
 from .ast import expression
 from .ast import statement
-from .tokens import TokenType
+from .tokens import Token, TokenType
 
 T = TypeVar('T')
 
 
 class UnknownOperator(Exception):
     """Unknown operator."""
 
@@ -20,15 +20,15 @@
 
 
 class Interpreter(expression.ExpressionVisitor[T], statement.StatementVisitor[T]):
     average: bool = False
 
     # variables: Dict[str, Union[int, str]] = {}
     variables: ChainMap[str, Union[Number, NumberList, str]] = ChainMap({})
-    functions: Dict[str, statement.Function] = {}
+    functions: Dict[str, Union[statement.Function, statement.Compositional]] = {}
 
     def __repr__(self):
         return "<Interpreter >"
 
     def push(self):
         self.variables = self.variables.new_child()
 
@@ -320,15 +320,15 @@
                 return [v for v in right if left > v]
 
             if token_type == TokenType.EQUAL:
                 return [v for v in right if left == v]
 
             if token_type == TokenType.NOT_EQUAL:
                 return [v for v in right if left != v]
-        
+
         if isinstance(left, list):
             assert len(left) == 1
             left = left[0]
 
         if isinstance(right, list):
             assert len(right) == 1
             right = right[0]
@@ -451,17 +451,52 @@
 
         return result
 
     def visit_Function_Statement(self, stmt: statement.Function):
         assert isinstance(stmt.name.literal, str)
         self.functions[stmt.name.literal] = stmt
 
+    def visit_Compositional_Statement(self, stmt: statement.Compositional):
+        assert isinstance(stmt.name.literal, str)
+        self.functions[stmt.name.literal] = stmt
+
     def visit_Call_Expression(self, expr: expression.Call):
         assert expr.name.literal in self.functions
         stmt = self.functions[expr.name.literal]
+
+        if isinstance(stmt, statement.Compositional):
+            return self.call_compositional(expr, stmt)
+
+        return self.call_function(expr, stmt)
+
+    def call_compositional(self, expr: expression.Call, stmt: statement.Compositional):
+        self.push()
+
+        res = stmt.empty.value
+
+        parameter = expr.parameters[0]
+
+        if isinstance(parameter, expression.List):
+            operator = stmt.union
+            for next_val in parameter.value:
+                if isinstance(operator, Token) and operator.token_type == TokenType.IDENTIFIER:
+                    res = self.visit_Call_Expression(expression.Call(name=operator, parameters=[expression.Literal(res), next_val]))
+                else:
+                    res = self.visit_Binary_Expression(expression.Binary(expression.Literal(res), operator=operator, right=next_val))
+        else:
+            operator = stmt.singleton
+            if isinstance(operator, Token) and operator.token_type == TokenType.IDENTIFIER:
+                res = self.visit_Call_Expression(expression.Call(name=operator, parameters=[expression.Literal(res)]))
+            else:
+                res = self.visit_Unary_Expression(expression.Unary(operator=operator, right=parameter))
+
+        self.pop()
+        return res
+
+    def call_function(self, expr: expression.Call, stmt: statement.Function):
         self.push()
         for name, value in zip(stmt.parameters, expr.parameters):
             assert isinstance(name.literal, str)
             self.variables[name.literal] = self.evaluate(value)
 
         assert isinstance(
             stmt.expression, (statement.Expression, statement.Statement))
@@ -482,50 +517,48 @@
         return [str(self.evaluate(expr)) for _ in range(repeats)]
 
     def visit_TextAlign_Expression(self, expr: expression.TextAlign):
         operator = expr.operator
         left = self.evaluate(expr.left)
         right = self.evaluate(expr.right)
 
-
         if isinstance(left, str):
             left = left.split('\n')
-        
+
         if isinstance(right, str):
             right = right.split('\n')
 
         if not isinstance(left, list):
             left = [left]
         if not isinstance(right, list):
-            right  = [right]
+            right = [right]
 
         assert isinstance(left, list), f"{left}, {type(left)}"
         assert isinstance(right, list), f"{right}, {type(right)}"
 
         max_length_left = len(str(max(left, key=lambda x: len(str(x)))))
         max_length_right = len(str(max(right, key=lambda x: len(str(x)))))
-        max_length = max(max_length_left, max_length_right )
+        max_length = max(max_length_left, max_length_right)
 
         if operator.lexeme == '|>':
-            output =  [f'{t:<{max_length}}' for t in left] + [f'{t:<{max_length}}' for t in right]
+            output = [f'{t:<{max_length}}' for t in left] + [f'{t:<{max_length}}' for t in right]
             return "\n".join(output)
 
         if operator.lexeme == '<|':
-            output =  [f'{t:>{max_length}}' for t in left] + [f'{t:>{max_length}}' for t in right]
+            output = [f'{t:>{max_length}}' for t in left] + [f'{t:>{max_length}}' for t in right]
             return "\n".join(output)
 
         if operator.lexeme == '<>':
-            output =  [f'{t:^{max_length}}' for t in left] + [f'{t:^{max_length}}' for t in right]
+            output = [f'{t:^{max_length}}' for t in left] + [f'{t:^{max_length}}' for t in right]
             return "\n".join(output)
 
         if operator.lexeme == '||':
             max_height = max(len(left), len(right))
 
             left += [' ' * max_length_left] * (max_height - len(left))
             right += [' ' * max_length_right] * (max_height - len(right))
 
             assert len(left) == len(right)
 
             preliminary = list(zip(left, right))
 
             return "\n".join(["".join([str(v) for v in t]) for t in preliminary])
-
```

### Comparing `trill-0.0.6/src/trill/main.py` & `trill-0.0.8/src/trill/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Run Trill dice roller."""
 from pathlib import Path
+from typing import Optional
 import typer
 from .tokens import TokenType
 from .tokenizer import Token, Tokenizer
 from .interpreter import Interpreter
 from .parser import Parser
 from .ast.printer import ASTPrinter
 from .ast.expression import Binary, Grouping, Literal, Unary
@@ -23,26 +24,27 @@
     ASTPrinter().print([expression])
 
 
 @app.command()
 def run(
         source: str = typer.Argument(..., help="Source of dice rolls."),
         average: bool = typer.Option(False, help="Use average dice values."),
+        seed: Optional[int] = typer.Option(None, help="Set random seed.")
 ):
     """
     Use SOURCE to roll dice according to the Troll language.
     If SOURCE resolves to an existing file, it will be read and used.
     """
     if Path(source).exists():
         with open(Path(source), 'r', encoding="utf-8") as f:
             source = f.read()
 
     tokens = Tokenizer(source).scan_tokens()
     parsed = Parser(tokens).parse()
-    result = Interpreter().interpret(parsed, average=average)
+    result = Interpreter(seed).interpret(parsed, average=average)
 
     if error_handler.had_error:
         for error in error_handler.error_report:
             print(error)
         return
 
     for line in result:
```

### Comparing `trill-0.0.6/src/trill/parser.py` & `trill-0.0.8/src/trill/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
             self.error(f"Type error: expected int, got {type(repeats)}")
             return None
 
         return statement.Print(self.parse_expression(), repeats)
 
     def declaration(self) -> Optional[Union[statement.Statement, expression.Expression]]:
         # statement -> exprStatement | printStatement;
+
+        if self.match(TokenType.COMPOSITIONAL):
+            return self.compositional_declaration()
+
         if self.match(TokenType.FUNCTION):
             return self.function_declaration()
 
         if (self.check(TokenType.INTEGER) and self.peek(1).token_type == TokenType.TEXTBOX) or self.check(TokenType.TEXTBOX):
             return self.print_statement()
 
         expr = self.parse_expression()
@@ -229,14 +233,15 @@
         while not self.match(TokenType.RPAREN):
             token = self.consume(TokenType.IDENTIFIER, "Expect variable name")
             if not token:
                 self.error(f"Expected token, got {token}")
                 err = True
             else:
                 parameters.append(token)
+            self.match(TokenType.COMMA)
 
         self.consume(TokenType.EQUAL, "Expect '=' before function body.")
         expr = self.declaration()
 
         if not identifier:
             self.error("Missing expected identifier")
             return None
@@ -246,14 +251,30 @@
             return None
 
         if err:
             return None
 
         return statement.Function(identifier, parameters, expr)
 
+    def compositional_declaration(self) -> Optional[statement.Compositional]:
+        identifier = self.consume(
+            TokenType.IDENTIFIER, "Expected compositional identifier.")
+
+        self.consume(TokenType.LPAREN, "Expect '(' after compositional name.")
+        empty = self.primary()
+        self.consume(TokenType.COMMA, "Expected comma")
+        singleton = self.tokens[self.current]
+        self.consume(singleton.token_type, "Found one")
+        self.consume(TokenType.COMMA, "Expected comma")
+        union = self.tokens[self.current]
+        self.consume(union.token_type, "Expected identifier")
+        self.consume(TokenType.RPAREN, "Expect ')' after last compositional parameter.")
+
+        return statement.Compositional(identifier, empty, singleton, union)
+
     def parse_expression(self) -> Optional[expression.Expression]:
         if self.match(TokenType.IF):
             return self.if_expression()
         if self.match(TokenType.ACCUMULATE):
             return self.accumulate_expression()
         if self.match(TokenType.REPEAT):
             return self.repeat_expression()
@@ -288,14 +309,15 @@
         parameters: List[expression.Expression] = []
         self.consume(TokenType.LPAREN, "Expect parenthesis for function call")
         while not self.match(TokenType.RPAREN):
             expr = self.parse_expression()
             if expr is None:
                 break
             parameters.append(expr)
+            self.match(TokenType.COMMA)
 
         if not name:
             self.error("Missing function name")
             return None
 
         return expression.Call(name, parameters)
```

### Comparing `trill-0.0.6/src/trill/reserved.py` & `trill-0.0.8/src/trill/reserved.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,9 +25,10 @@
     'in': TokenType.IN,
     'do': TokenType.DO,
     'repeat': TokenType.REPEAT,
     'until': TokenType.UNTIL,
     'while': TokenType.WHILE,
     'accumulate': TokenType.ACCUMULATE,
     'function': TokenType.FUNCTION,
+    'compositional': TokenType.COMPOSITIONAL,
     'call': TokenType.CALL,
 }
```

### Comparing `trill-0.0.6/src/trill/string.py` & `trill-0.0.8/src/trill/string.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.6/src/trill/tokenizer.py` & `trill-0.0.8/src/trill/tokenizer.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.6/src/trill/tokens.py` & `trill-0.0.8/src/trill/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     IN = 'in'
     DO = 'do'
     REPEAT = 'repeat'
     WHILE = 'while'
     UNTIL = 'until'
     ACCUMULATE = 'accumulate'
 
+    COMPOSITIONAL = 'compositional'
     FUNCTION = 'function'
     CALL = 'call'
 
     TEXTBOX = "'"
     TEXTALIGN = "textalign"
 
     EOF = 'eof'
```

