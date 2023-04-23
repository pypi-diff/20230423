# Comparing `tmp/nobus-0.1.3.tar.gz` & `tmp/nobus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobus-0.1.3.tar", max compression
+gzip compressed data, was "nobus-0.1.4.tar", max compression
```

## Comparing `nobus-0.1.3.tar` & `nobus-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.3/LICENSE
--rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.3/nobus/__init__.py
--rw-r--r--   0        0        0    11312 2023-04-23 06:24:15.348935 nobus-0.1.3/nobus/safeattr.py
--rw-r--r--   0        0        0      256 2023-04-23 06:25:00.203805 nobus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.3/setup.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.4/nobus/__init__.py
+-rw-r--r--   0        0        0    11566 2023-04-23 09:14:45.535948 nobus-0.1.4/nobus/safeattr.py
+-rw-r--r--   0        0        0      256 2023-04-23 09:17:34.713283 nobus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.4/setup.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.4/PKG-INFO
```

### Comparing `nobus-0.1.3/LICENSE` & `nobus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobus-0.1.3/README.md` & `nobus-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nobus-0.1.3/nobus/safeattr.py` & `nobus-0.1.4/nobus/safeattr.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return self._function(x)
 
 def typechecker(function):
     return TypeChecker(function)
 
 class Typed:
     @staticmethod
-    def typecheck(value, type_, optional):
+    def _typecheck(value, type_, optional):
         if value is None:
             if optional:
                 # optional で None なら OK
                 return
             # optional じゃないのに value が None である 
             raise TypeError(f"value is None even though it is not optional.")
         
@@ -33,22 +33,25 @@
                 raise TypeError(f"typechecking by '{type_}' returned False.")
 
             if isinstance(value, type_):
                 return True
             raise TypeError(f"value must be instance of {type_} but actual type {type(value)}.")
 
         return
+    
+    def typecheck(self, value):
+        self._typecheck(value, self.type, self.optional)
+        return value
 
     def __init__(self, value, type_=None, optional=False):
-        self.typecheck(value, type_, optional)
-
-        self._value = value
         self._type = type_
         self._optional = optional
 
+        self._value = self.typecheck(value)
+
     def __repr__(self):
         xs = f"{self.__class__.__name__}(value={self.value.__repr__()}"
         if self.type is not None:
             xs += f", type_={self.type}"
         xs += f", optional={self.optional.__repr__()}"
         xs += ")"
         return xs
@@ -72,17 +75,15 @@
             if (self.type is not None) and (self.type != value.type):
                 raise TypeError(f"value must be instance of {self.type} but actual type {value.type}.")
         
         if isinstance(value, Typed):
             value = value.value
 
         # value に対して型チェック
-        self.typecheck(value, self.type, self.optional)
-
-        self._value = value
+        self._value = self.typecheck(value)
     
 class Immutable(Typed):
     def __init__(self, value, type_=None, optional=False):
         super().__init__(value, type_, optional)
 
     @property
     def value(self):
@@ -256,17 +257,24 @@
             return setter
         
         # getter と setter をセットする
         setattr(self.__class__, name, property(getter_of(name), setter_of(name)))
         
         # メソッドの引数を優先して返す
         def selector_of(name):
-            def arg_override(self, x=None, f=None):
-                if x is not None:
-                    if f is not None:
-                        return f(x)
-                    return x
-                return getattr(self, name)
+            def arg_override(self, x=None, f=None, typecheck=True):
+                if x is None:
+                    return getattr(self, name)
+                
+                if f is not None:
+                    x = f(x)
+                
+                if typecheck:
+                    attr = getattr(self, '_safeattr_' + name)
+                    return attr.typecheck(x)
+                    
+                return x
+                
             return arg_override
         
         # arg_override を追加する
         super().__setattr__('arg_' + name, MethodType(selector_of(name), self))
```

### Comparing `nobus-0.1.3/setup.py` & `nobus-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['nobus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'nobus',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# nobus\n"Nobody But Us" modules for Python\n\n## What is nobus\n[NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。\n\n`nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。\n\n現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。\n\nそのうち関数型プログラミングモジュールの `kette` を統合する予定です。\n\n本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。\n\n* Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)\n* Twitter: [@wsuzume](https://twitter.com/wsuzume)\n\n## Usage\n```\n$ pip install nobus\n```\n',
     'author': 'Josh Nobus',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nobus-0.1.3/PKG-INFO` & `nobus-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobus
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Josh Nobus
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

