# Comparing `tmp/nobus-0.1.2.tar.gz` & `tmp/nobus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobus-0.1.2.tar", max compression
+gzip compressed data, was "nobus-0.1.3.tar", max compression
```

## Comparing `nobus-0.1.2.tar` & `nobus-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.2/LICENSE
--rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.2/nobus/__init__.py
--rw-r--r--   0        0        0    11307 2023-04-22 17:04:49.898539 nobus-0.1.2/nobus/safeattr.py
--rw-r--r--   0        0        0      256 2023-04-22 17:05:33.468640 nobus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.2/setup.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.3/nobus/__init__.py
+-rw-r--r--   0        0        0    11312 2023-04-23 06:24:15.348935 nobus-0.1.3/nobus/safeattr.py
+-rw-r--r--   0        0        0      256 2023-04-23 06:25:00.203805 nobus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.3/setup.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.3/PKG-INFO
```

### Comparing `nobus-0.1.2/LICENSE` & `nobus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nobus-0.1.2/README.md` & `nobus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nobus-0.1.2/nobus/safeattr.py` & `nobus-0.1.3/nobus/safeattr.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     
     @property
     def is_safeattr_derived_class(self):
         if not hasattr(self, '_is_safeattr_derived_class'):
             return False
         return self._is_safeattr_derived_class
     
-    def __getattr__(self, name):
+    def __getattribute__(self, name):
         if not name.startswith('_') or name.startswith('_safeattr_'):
             # 隠蔽されたメンバに対するアクセスではないか、
             # 隠蔽されたメンバの実体に対する直アクセス
             return super().__getattribute__(name)
         
         # ユーザが隠蔽されたメンバ '_x' にアクセスするときは '_safeattr_x' が実体になる
         try:
```

### Comparing `nobus-0.1.2/setup.py` & `nobus-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['nobus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'nobus',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# nobus\n"Nobody But Us" modules for Python\n\n## What is nobus\n[NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。\n\n`nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。\n\n現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。\n\nそのうち関数型プログラミングモジュールの `kette` を統合する予定です。\n\n本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。\n\n* Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)\n* Twitter: [@wsuzume](https://twitter.com/wsuzume)\n\n## Usage\n```\n$ pip install nobus\n```\n',
     'author': 'Josh Nobus',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nobus-0.1.2/PKG-INFO` & `nobus-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobus
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Josh Nobus
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

