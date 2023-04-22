# Comparing `tmp/ringneck-0.0.1.tar.gz` & `tmp/ringneck-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringneck-0.0.1.tar", last modified: Sun Apr  9 15:25:23 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ringneck-0.0.1.tar` & `ringneck-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-04-09 15:25:23.288231 ringneck-0.0.1/
--rw-r--r--   0 greger    (1000) greger    (1000)      550 2023-04-09 15:25:23.288231 ringneck-0.0.1/PKG-INFO
--rw-r--r--   0 greger    (1000) greger    (1000)      156 2023-04-09 14:27:35.000000 ringneck-0.0.1/README.md
--rw-r--r--   0 greger    (1000) greger    (1000)     1078 2023-04-07 17:59:44.000000 ringneck-0.0.1/pyproject.toml
--rw-r--r--   0 greger    (1000) greger    (1000)       38 2023-04-09 15:25:23.288231 ringneck-0.0.1/setup.cfg
--rw-r--r--   0 greger    (1000) greger    (1000)       38 2023-04-07 17:58:54.000000 ringneck-0.0.1/setup.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-04-09 15:25:23.285231 ringneck-0.0.1/src/
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-04-09 15:25:23.286231 ringneck-0.0.1/src/ringneck/
--rw-r--r--   0 greger    (1000) greger    (1000)      600 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/__init__.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-04-09 15:25:23.288231 ringneck-0.0.1/src/ringneck/ast/
--rw-r--r--   0 greger    (1000) greger    (1000)        0 2023-04-07 20:35:02.000000 ringneck-0.0.1/src/ringneck/ast/__init__.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1016 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/ast/base.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1016 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/ast/expression.py
--rw-r--r--   0 greger    (1000) greger    (1000)     1695 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/ast/printer.py
--rw-r--r--   0 greger    (1000) greger    (1000)      302 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/ast/statement.py
--rw-r--r--   0 greger    (1000) greger    (1000)      703 2023-04-08 08:30:47.000000 ringneck-0.0.1/src/ringneck/error_handler.py
--rw-r--r--   0 greger    (1000) greger    (1000)     4033 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/interpreter.py
--rw-r--r--   0 greger    (1000) greger    (1000)     6841 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/parser.py
--rw-r--r--   0 greger    (1000) greger    (1000)     4481 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/scanner.py
--rw-r--r--   0 greger    (1000) greger    (1000)      920 2023-04-09 14:27:35.000000 ringneck-0.0.1/src/ringneck/tokens.py
-drwxr-xr-x   0 greger    (1000) greger    (1000)        0 2023-04-09 15:25:23.287231 ringneck-0.0.1/src/ringneck.egg-info/
--rw-r--r--   0 greger    (1000) greger    (1000)      550 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/PKG-INFO
--rw-r--r--   0 greger    (1000) greger    (1000)      547 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/SOURCES.txt
--rw-r--r--   0 greger    (1000) greger    (1000)        1 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/dependency_links.txt
--rw-r--r--   0 greger    (1000) greger    (1000)       47 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/entry_points.txt
--rw-r--r--   0 greger    (1000) greger    (1000)       13 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/requires.txt
--rw-r--r--   0 greger    (1000) greger    (1000)        9 2023-04-09 15:25:23.000000 ringneck-0.0.1/src/ringneck.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 ringneck-0.0.2/Makefile
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ringneck-0.0.2/_version.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ringneck-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ringneck-0.0.2/setup.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ringneck-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ringneck-0.0.2/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ringneck-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ringneck-0.0.2/examples/generator.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/error_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/grammar.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/interpreter.py
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/parser.py
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/scanner.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tokens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/base.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/expression.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/printer.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/statement.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/__init__.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/cases.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_embedded.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_interpreter.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_parser.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_scanner.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 ringneck-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ringneck-0.0.2/LICENSE
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ringneck-0.0.2/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 ringneck-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 ringneck-0.0.2/PKG-INFO
```

### Comparing `ringneck-0.0.1/pyproject.toml` & `ringneck-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,24 @@
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
 name = "ringneck"
-version = "0.0.1"
+dynamic = ["version"]
+
 description = "A Python-ish script interpreter."
 readme = "README.md"
+
 authors = [
   { name = "Greger Stolt Nilsen", email = "gregersn@gmail.com" },
 ]
 license = { file ="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ringneck-0.0.1/src/ringneck/__init__.py` & `ringneck-0.0.2/src/ringneck/__init__.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.1/src/ringneck/ast/base.py` & `ringneck-0.0.2/src/ringneck/ast/base.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.1/src/ringneck/ast/expression.py` & `ringneck-0.0.2/src/ringneck/ast/expression.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from typing import Any, List as TList
+import operator
+from typing import Any, List as TList, Optional, Union
 
 from ringneck.ast.base import Node, Visitor, VisitorType
 from ..tokens import Token
 
 
 class ExpressionVisitor(Visitor[VisitorType]):
     ...
@@ -11,14 +12,19 @@
 
 @dataclass
 class Expression(Node):
     ...
 
 
 @dataclass
+class ExpressionList(Expression):
+    expressions: TList['Expression']
+
+
+@dataclass
 class Binary(Expression):
     left: Expression
     operator: Token
     right: Expression
 
 
 @dataclass
@@ -39,16 +45,43 @@
 
 @dataclass
 class Variable(Expression):
     name: Token
 
 
 @dataclass
+class VariableIterator(Expression):
+    prefix: Expression
+    iterator: 'List'
+
+
+@dataclass
 class Assign(Expression):
     name: Token
+    operator: Token
+    value: Any
+
+
+@dataclass
+class MultiAssign(Expression):
+    identifiers: Union['Tuple', 'List']
+    operator: Token
+    values: Union['Tuple', 'List']
+
+
+@dataclass
+class AssignIterator(Expression):
+    iterator: VariableIterator
+    operator: Token
+    value: Any
+
+
+@dataclass
+class Starred(Expression):
+    operator: Token
     value: Any
 
 
 @dataclass
 class KeyDatum(Expression):
     key: Expression
     datum: Expression
@@ -56,16 +89,33 @@
 
 @dataclass
 class Dict(Expression):
     values: TList[KeyDatum]
 
 
 @dataclass
+class Tuple(Expression):
+    values: TList[Expression] | ExpressionList | Starred
+
+
+@dataclass
 class List(Expression):
-    values: TList[Expression]
+    values: TList[Expression] | ExpressionList | Starred
 
 
 @dataclass
 class Call(Expression):
     callee: Expression
     paren: Token
-    arguments: TList[Expression]
+    arguments: Optional[ExpressionList]
+
+
+@dataclass
+class Conditional(Expression):
+    left: Expression
+    condition: Expression
+    right: Expression
+
+
+@dataclass
+class IteratorValue(Expression):
+    token: Token
```

### Comparing `ringneck-0.0.1/src/ringneck/ast/printer.py` & `ringneck-0.0.2/src/ringneck/ast/printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,15 +34,48 @@
 
     def visit_Expression_Statement(self, stmt: statement.Expression):
         return str(stmt.expr.accept(self))
 
     def visit_Assign_Expression(self, expr: expression.Assign):
         return self.parenthesize(f'assign {expr.name.literal}', expr.value)
 
+    def visit_AssignIterator_Expression(self, expr: expression.AssignIterator):
+        return self.parenthesize(f'assign {expr.iterator.accept(self)}', expr.value)
+
     def visit_KeyDatum_Expression(self, expr: expression.KeyDatum):
         return f"{expr.key.accept(self)}: {expr.datum.accept(self)}"
 
     def visit_Dict_Expression(self, expr: expression.Dict):
         return f"(dict {', '.join([v.accept(self) for v in expr.values])})"
 
+    def visit_List_Expression(self, expr: expression.List):
+        if isinstance(expr.values, expression.Starred):
+            return expr.values.accept(self)
+
+        if isinstance(expr.values, expression.ExpressionList):
+            return f"(list {', '.join([str(v.accept(self)) for v in expr.values.expressions])})"
+
+        return f"(list {', '.join([str(v.accept(self)) for v in expr.values])})"
+
     def visit_Variable_Expression(self, expr: expression.Variable):
         return f"{expr.name.literal}"
+
+    def visit_VariableIterator_Expression(self, expr: expression.VariableIterator):
+        return f"{expr.prefix.literal}{expr.iterator.accept(self)}"
+
+    def visit_Conditional_Expression(self, expr: expression.Conditional):
+        return f"(if {expr.left.accept(self)} {expr.condition.accept(self)} {expr.right.accept(self)})"
+
+    def visit_Call_Expression(self, expr: expression.Call):
+        return f"(call {expr.callee.accept(self)} {' '.join([str(arg.accept(self)) for arg in expr.arguments.expressions])})"
+
+    def visit_MultiAssign_Expression(self, expr: expression.MultiAssign):
+        return (f'(assign {expr.identifiers.accept(self)} {expr.values.accept(self)})')
+
+    def visit_Tuple_Expression(self, expr: expression.Tuple):
+        return f"(tuple {', '.join(str(v.accept(self)) for v in expr.values)})"
+
+    def visit_ExpressionList_Expression(self, expr: expression.ExpressionList):
+        return f"(expressionlist {', '.join(str(v.accept(self)) for v in expr.expressions)})"
+
+    def visit_Starred_Expression(self, expr: expression.Starred):
+        return self.parenthesize("starred", expr.value)
```

### Comparing `ringneck-0.0.1/src/ringneck/error_handler.py` & `ringneck-0.0.2/src/ringneck/error_handler.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.1/src/ringneck/parser.py` & `ringneck-0.0.2/src/ringneck/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,22 @@
+"""Ringneck parser."""
 from typing import List
 from ringneck.ast import expression, statement
 from ringneck.error_handler import ErrorHandler
 
 from ringneck.tokens import Token, TokenType
 
 
 class Parser:
     tokens: List[Token]
     current: int = 0
 
     def __init__(self, tokens: List[Token]):
         self.tokens = tokens
 
-    def parse(self):
-        statements: List[statement.Statement] = []
-        while not self.is_at_end():
-            statements.append(self.statement())
-            while self.match(TokenType.EOL):
-                self.advance()
-
-        return statements
-
     def match(self, *args: TokenType) -> bool:
         for tokentype in args:
             if self.check(tokentype):
                 self.advance()
                 return True
 
         return False
@@ -46,52 +38,105 @@
 
     def peek(self):
         return self.tokens[self.current]
 
     def previous(self):
         return self.tokens[self.current - 1]
 
+    def parse(self):
+        statements: List[statement.Statement] = []
+        while not self.is_at_end():
+            statements.append(self.statement())
+            while self.match(TokenType.EOL):
+                pass
+
+        return statements
+
     def statement(self):
         return self.expression_statement()
 
     def expression_statement(self):
         expr = self.parse_expression()
+
         if not self.is_at_end():
-            self.consume(TokenType.EOL, "Expect newline after expression")
+            self.consume(
+                TokenType.EOL, f"Expect newline after expression, got {self.peek().tokentype}")
         return statement.Expression(expr)
 
+    def expression_list(self):
+        expr = self.equality()
+        if self.peek().tokentype == TokenType.COMMA:
+            expr_list = [expr]
+            while self.match(TokenType.COMMA):
+                expr_list.append(self.equality())
+
+            if self.peek().tokentype != TokenType.RIGHT_PAREN:
+                return expression.Tuple(expr_list)
+            expr = expression.ExpressionList(expr_list)
+        return expr
+
     def parse_expression(self):
         return self.assignment()
 
     def assignment(self) -> expression.Expression:
-        expr = self.equality()
-        if self.match(TokenType.EQUAL):
+        expr = self.expression_list()
+
+        if self.match(TokenType.EQUAL, TokenType.MAYBE_EQUAL):
             equals = self.previous()
             value = self.assignment()
 
+            if isinstance(expr, (expression.Tuple, expression.List)):
+                assert isinstance(value, expression.Tuple)
+                assert len(expr.values) == len(value.values)
+                return expression.MultiAssign(expr, equals, value)
             if isinstance(expr, expression.Variable):
                 name = expr.name
-                return expression.Assign(name, value)
-            self.error(equals,  "Invalid assignment target.")
+                return expression.Assign(name, equals, value)
+            if isinstance(expr, expression.VariableIterator):
+                return expression.AssignIterator(expr, equals, value)
+            self.error(equals, "Invalid assignment target.")
         return expr
 
     def equality(self):
+        expr = self.logical()
+
+        if self.peek().tokentype == TokenType.IF:
+            self.consume(TokenType.IF, "Expected conditional")
+            condition = self.equality()
+            other = None
+
+            if self.peek().tokentype == TokenType.ELSE:
+                self.consume(TokenType.ELSE,
+                             f"Expected else, got {self.peek().tokentype}")
+                other = self.parse_expression()
+
+            return expression.Conditional(expr, condition, other)
+
+        while self.match(TokenType.BANG_EQUAL, TokenType.EQUAL_EQUAL):
+            operator = self.previous()
+            right = self.logical()
+            expr = expression.Binary(expr, operator, right)
+
+        return expr
+
+    def logical(self):
         expr = self.comparison()
 
-        while (self.match(TokenType.BANG_EQUAL, TokenType.EQUAL_EQUAL)):
+        while (self.match(TokenType.AND, TokenType.OR)):
             operator = self.previous()
             right = self.comparison()
             expr = expression.Binary(expr, operator, right)
 
         return expr
 
     def comparison(self):
         expr = self.term()
 
-        while (self.match(TokenType.GREATER, TokenType.GREATER_EQUAL, TokenType.LESS, TokenType.LESS_EQUAL)):
+        while (self.match(TokenType.GREATER, TokenType.GREATER_EQUAL,
+                          TokenType.LESS, TokenType.LESS_EQUAL)):
             operator = self.previous()
             right = self.term()
             expr = expression.Binary(expr, operator, right)
 
         return expr
 
     def term(self):
@@ -114,107 +159,126 @@
         return expr
 
     def unary(self) -> expression.Expression:
         if self.match(TokenType.MINUS):
             operator = self.previous()
             right = self.unary()
             return expression.Unary(operator, right)
-
+        if self.match(TokenType.STAR):
+            operator = self.previous()
+            right = self.unary()
+            return expression.Starred(operator, right)
         return self.call()
 
     def call(self):
         expr = self.primary()
 
         while True:
             if self.match(TokenType.LEFT_PAREN):
                 expr = self.finish_call(expr)
             else:
                 break
 
         return expr
 
     def finish_call(self, callee: expression.Expression):
-        arguments: List[expression.Expression] = []
-
+        arguments = []
         if not self.check(TokenType.RIGHT_PAREN):
-            arguments.append(self.parse_expression())
+            arguments.append(self.equality())
             while self.match(TokenType.COMMA):
-                arguments.append(self.parse_expression())
+                arguments.append(self.equality())
 
         paren = self.consume(TokenType.RIGHT_PAREN,
                              "Expected ')' after arguments")
 
-        return expression.Call(callee, paren, arguments)
+        return expression.Call(callee, paren, expression.ExpressionList(arguments))
 
     def primary(self):
+        if self.match(TokenType.FALSE):
+            return expression.Literal(False)
+
+        if self.match(TokenType.TRUE):
+            return expression.Literal(True)
+
+        if self.match(TokenType.NOT):
+            return expression.Literal('not')
+
         if self.match(TokenType.IDENTIFIER):
+            if self.peek().tokentype == TokenType.LEFT_BRACKET:
+                prefix = self.previous()
+                iterator = self.primary()
+                return expression.VariableIterator(prefix, iterator)
+
             return expression.Variable(self.previous())
 
         if self.match(TokenType.NUMBER, TokenType.STRING):
             return expression.Literal(self.previous().literal)
 
         if self.match(TokenType.LEFT_PAREN):
-            expr = self.parse_expression()
+            expr = self.expression_list()
             self.consume(TokenType.RIGHT_PAREN, "Expect ')' after expression")
+            if isinstance(expr, expression.ExpressionList):
+                return expression.Tuple(expr.expressions)
             return expression.Grouping(expr)
 
         if self.match(TokenType.LEFT_BRACKET):
             return self.list()
 
         if self.match(TokenType.LEFT_BRACE):
             return self.dictionary()
 
+        if self.match(TokenType.PERCENT):
+            return expression.IteratorValue(self.previous())
+
         raise self.error(self.peek(), "Expect expression")
 
     def dictionary(self):
         data_pairs: List[expression.KeyDatum] = []
         while not self.peek().tokentype == TokenType.RIGHT_BRACE:
 
             while self.check(TokenType.EOL):
                 self.advance()
 
             key = self.parse_expression()
             self.consume(TokenType.COLON, "Expect colon")
-            value = self.parse_expression()
+            value = self.equality()
             data_pairs.append(expression.KeyDatum(key, value))
             if self.peek().tokentype == TokenType.COMMA:
                 self.consume(TokenType.COMMA, "Expected comma")
 
             while self.check(TokenType.EOL):
                 self.advance()
 
         self.consume(TokenType.RIGHT_BRACE, "Expect '}' to close dict")
         return expression.Dict(data_pairs)
 
     def list(self):
-        data: List[expression.Expression] = []
-        while not self.peek().tokentype == TokenType.RIGHT_BRACKET:
-            while self.check(TokenType.EOL):
-                self.advance()
-            value = self.parse_expression()
-            data.append(value)
-            if self.peek().tokentype == TokenType.COMMA:
-                self.consume(TokenType.COMMA, "Expected comma")
-            while self.check(TokenType.EOL):
-                self.advance()
+        if self.peek().tokentype == TokenType.RIGHT_BRACKET:
+            self.consume(TokenType.RIGHT_BRACKET,
+                         "Expected ']' to close an empty list.")
+            return expression.List(expression.ExpressionList([]))
+        expr = self.expression_list()
         self.consume(TokenType.RIGHT_BRACKET, "Expect ']' to close list")
-        return expression.List(data)
+        if isinstance(expr, expression.Starred):
+            return expression.List(expr)
+        return expression.List(expr.values)
 
     def consume(self, tokentype: TokenType, message: str):
         if self.check(tokentype):
             return self.advance()
 
         raise self.error(self.peek(), message)
 
     def error(self, token: Token, message: str):
         ErrorHandler.error(token, message)
         return ParserError(token, message)
 
     def synchronize(self):
-        # TODO: This is where we should try to find the start of a new statement.
+        # TODO: This is where we should try to
+        # find the start of a new statement.
         self.advance()
 
         while not self.is_at_end():
             if self.previous().tokentype == TokenType.EOL:
                 return
 
             if self.peek().tokentype in []:
```

### Comparing `ringneck-0.0.1/src/ringneck/scanner.py` & `ringneck-0.0.2/src/ringneck/scanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, List
-from ringneck.tokens import Token, TokenType
+from ringneck.tokens import Token, TokenType, keywords
 from ringneck.error_handler import ErrorHandler
 
 
 class Scanner:
     source: str
     tokens: List[Token]
 
@@ -31,38 +31,64 @@
 
         return self.tokens
 
     def scan_token(self):
         char = self.advance()
         if char == '+':
             return self.add_token(TokenType.PLUS, '+')
+        if char == '-':
+            return self.add_token(TokenType.MINUS, '-')
         if char == '*':
             return self.add_token(TokenType.STAR, '*')
+        if char == '/':
+            return self.add_token(TokenType.SLASH, '/')
+
+        if char == '%':
+            return self.add_token(TokenType.PERCENT, '%')
+
+        if char == '<':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.LESS_EQUAL, '<=')
+            return self.add_token(TokenType.LESS, '<')
+        if char == '>':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.GREATER_EQUAL, '>=')
+            return self.add_token(TokenType.GREATER, '>')
 
         if char == '(':
             return self.add_token(TokenType.LEFT_PAREN, '(')
-
         if char == ')':
             return self.add_token(TokenType.RIGHT_PAREN, ')')
-
         if char == '{':
             return self.add_token(TokenType.LEFT_BRACE, '{')
-
         if char == '}':
             return self.add_token(TokenType.RIGHT_BRACE, '}')
-
         if char == '[':
             return self.add_token(TokenType.LEFT_BRACKET, '[')
-
         if char == ']':
             return self.add_token(TokenType.RIGHT_BRACKET, ']')
 
         if char == '=':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.EQUAL_EQUAL, '==')
             return self.add_token(TokenType.EQUAL, char)
 
+        if char == '!':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.BANG_EQUAL, '!=')
+
+        if char == '?':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.MAYBE_EQUAL, '?=')
+
         if char == '.':
             return self.add_token(TokenType.DOT, char)
 
         if char == ':':
             return self.add_token(TokenType.COLON, char)
 
         if char == ',':
@@ -80,27 +106,30 @@
         if char.isalpha() or char == '$':
             return self.identifier()
 
         if char in [' ', '\t']:
             return
 
         if char == '\n':
-            while self.peek() == '\n':
-                self.advance()
             if self._column > 1:
                 self.add_token(TokenType.EOL)
+            while self.peek() == '\n':
+                self.advance()
+                self.advance_line()
             self.advance_line()
             return
 
         ErrorHandler.report(self._line, self._column,
                             f"Unexepected character: {char}")
 
     def comment(self):
         while self.peek() != '\n':
             self.advance()
+        self.advance_line()
+        self.advance()
         return
 
     def advance_line(self):
         self._line += 1
         self._column = 0
 
     def string(self, quotation: str):
@@ -132,16 +161,18 @@
         else:
             self.add_token(TokenType.NUMBER, int(
                 self.source[self._start:self._current], 10))
 
     def identifier(self):
         while self.peek().isalnum() or self.peek() in ['_', '.']:
             self.advance()
-        self.add_token(TokenType.IDENTIFIER,
-                       (self.source[self._start:self._current]))
+
+        identifier = self.source[self._start:self._current]
+        identifier_type = keywords.get(identifier, TokenType.IDENTIFIER)
+        self.add_token(identifier_type, identifier)
 
     def peek(self):
         if self.is_at_end():
             return '\0'
         return self.source[self._current]
 
     def peek_next(self):
```

### Comparing `ringneck-0.0.1/src/ringneck/tokens.py` & `ringneck-0.0.2/src/ringneck/tokens.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     # Operators
     PLUS = '+'
     MINUS = '-'
     SLASH = '/'
     STAR = '*'
 
     EQUAL = '='
+    MAYBE_EQUAL = '?='
 
     DOLLAR = '$'
     DOT = '.'
     COLON = ':'
     COMMA = ','
     HASH = '#'
+    PERCENT = '%'
 
     GREATER = '>'
     GREATER_EQUAL = '>='
 
     LESS = '<'
     LESS_EQUAL = '<='
 
@@ -41,14 +43,36 @@
     NUMBER = 'number'
     STRING = 'string'
     IDENTIFIER = 'identifier'
 
     EOL = 'EOL'
     EOF = 'EOF'
 
+    # Keywords
+    IF = 'if'
+    ELSE = 'else'
+
+    AND = 'and'
+    OR = 'or'
+    NOT = 'not'
+
+    TRUE = 'True'
+    FALSE = 'False'
+
+
+keywords = {
+    'if': TokenType.IF,
+    'else': TokenType.ELSE,
+    'and': TokenType.AND,
+    'or': TokenType.OR,
+    'not': TokenType.NOT,
+    'True': TokenType.TRUE,
+    'False': TokenType.FALSE
+}
+
 
 @dataclass
 class Token:
     tokentype: TokenType
     lexeme: str
     literal: Any
     line: int
```

