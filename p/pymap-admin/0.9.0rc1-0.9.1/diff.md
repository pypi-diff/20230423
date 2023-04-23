# Comparing `tmp/pymap-admin-0.9.0rc1.tar.gz` & `tmp/pymap_admin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymap-admin-0.9.0rc1.tar", last modified: Sun Oct 30 00:04:53 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pymap-admin-0.9.0rc1.tar` & `pymap_admin-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.672323 pymap-admin-0.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6815 2022-10-30 00:04:53.672323 pymap-admin-0.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.664323 pymap-admin-0.9.0rc1/pymap_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6815 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-30 00:04:53.000000 pymap-admin-0.9.0rc1/pymap_admin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.664323 pymap-admin-0.9.0rc1/pymapadmin/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.668323 pymap-admin-0.9.0rc1/pymapadmin/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/health.py
--rw-r--r--   0 runner    (1001) docker     (121)     4411 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     4144 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/commands/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.668323 pymap-admin-0.9.0rc1/pymapadmin/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    13072 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/health_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/grpc/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4877 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/main.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pymapadmin/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-30 00:04:53.672323 pymap-admin-0.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:04:53.672323 pymap-admin-0.9.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/test_health.py
--rw-r--r--   0 runner    (1001) docker     (121)     3286 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/test_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     4326 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-30 00:04:33.000000 pymap-admin-0.9.0rc1/test/test_version.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.flake8
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.gitattributes
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/__about__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/__init__.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/config.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/local.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/py.typed
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/typing.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/__init__.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/base.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/health.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/mailbox.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/system.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/__init__.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin.proto
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_grpc.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.py
+-rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.pyi
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/grpc_tools.protoc-args
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health.proto
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_grpc.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.pyi
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/handler.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_health.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_mailbox.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_system.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_user.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/README.md
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/PKG-INFO
```

### Comparing `pymap-admin-0.9.0rc1/LICENSE.md` & `pymap_admin-0.9.1/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## The MIT License (MIT)
 
-Copyright (c) 2021 Ian Good
+Copyright (c) 2022 Ian Good
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymap-admin-0.9.0rc1/PKG-INFO` & `pymap_admin-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,55 @@
 Metadata-Version: 2.1
 Name: pymap-admin
-Version: 0.9.0rc1
-Summary: Admin tool for running pymap instances.
-Home-page: https://github.com/icgood/pymap-admin/
-Author: Ian Good
-Author-email: ian@icgood.net
-License: MIT
+Version: 0.9.1
+Summary: Tool for administering running pymap instances.
+Project-URL: Homepage, https://github.com/icgood/pymap-admin/
+Project-URL: API Documentation, https://icgood.github.io/pymap-admin/
+Author-email: Ian Good <ian@icgood.net>
+License: ## The MIT License (MIT)
+        
+        Copyright (c) 2022 Ian Good
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Communications :: Email :: Post-Office
-Classifier: Topic :: Communications :: Email :: Post-Office :: IMAP
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications :: Email :: Post-Office
+Classifier: Topic :: Communications :: Email :: Post-Office :: IMAP
 Requires-Python: ~=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: optional
+Requires-Dist: grpclib
+Requires-Dist: protobuf
+Requires-Dist: typing-extensions
 Provides-Extra: build
-License-File: LICENSE.md
+Requires-Dist: grpcio-tools; extra == 'build'
+Requires-Dist: mypy-protobuf; extra == 'build'
+Provides-Extra: optional
+Requires-Dist: googleapis-common-protos; extra == 'optional'
+Description-Content-Type: text/markdown
 
 pymap-admin
 ===========
 
 [![build](https://github.com/icgood/pymap-admin/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/pymap-admin/actions/workflows/python-package.yml)
 [![Coverage Status](https://coveralls.io/repos/icgood/pymap-admin/badge.svg)](https://coveralls.io/r/icgood/pymap-admin)
 [![PyPI](https://img.shields.io/pypi/v/pymap-admin.svg)](https://pypi.python.org/pypi/pymap-admin)
@@ -170,29 +197,7 @@
 
 [1]: https://github.com/icgood/pymap
 [2]: https://grpc.io/
 [3]: https://github.com/vmagamedov/grpclib
 [4]: https://github.com/slimta/slimta-docker
 [5]: https://github.com/slimta/slimta-docker#address-management
 [6]: https://github.com/ecordell/pymacaroons
-## The MIT License (MIT)
-
-Copyright (c) 2021 Ian Good
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
```

### Comparing `pymap-admin-0.9.0rc1/README.md` & `pymap_admin-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/__init__.py` & `pymap_admin-0.9.1/pymapadmin/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Contains the package version string.
 
 See Also:
     `PEP 396 <https://www.python.org/dev/peps/pep-0396/>`_
 
 """
 
-import pkg_resources
+from importlib.metadata import distribution
 
 __all__ = ['__version__', 'is_compatible']
 
 #: The package version string.
-__version__: str = pkg_resources.require('pymap-admin')[0].version
+__version__: str = distribution('pymap-admin').version
 
 
 def is_compatible(client_version: str, server_version: str) -> bool:
     """Check if the given client version is backwards- and forwards-compatible
     with the server version.
 
     Args:
```

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/__init__.py` & `pymap_admin-0.9.1/pymapadmin/commands/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 
 from __future__ import annotations
 
 from collections.abc import Mapping
-
-from pkg_resources import iter_entry_points, DistributionNotFound
+from importlib.metadata import entry_points
 
 from .base import Command
 
 __all__ = ['load_commands']
 
 
 def load_commands(group: str = 'pymapadmin.commands') \
         -> Mapping[str, type[Command]]:  # pragma: no cover
     """Load and return a map of command name to implementation class.
 
     Args:
-        group: The setuptools entry point used to register commands.
+        group: The entry point group used to register commands.
 
     """
     ret = {}
-    for entry_point in iter_entry_points(group):
-        try:
-            cls = entry_point.load()
-        except DistributionNotFound:
-            pass  # optional dependencies not installed
-        else:
-            ret[entry_point.name] = cls
+    for entry_point in entry_points(group=group):
+        cls = entry_point.load()
+        ret[entry_point.name] = cls
     return ret
```

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/base.py` & `pymap_admin-0.9.1/pymapadmin/commands/base.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/health.py` & `pymap_admin-0.9.1/pymapadmin/commands/health.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/mailbox.py` & `pymap_admin-0.9.1/pymapadmin/commands/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/system.py` & `pymap_admin-0.9.1/pymapadmin/commands/system.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/commands/user.py` & `pymap_admin-0.9.1/pymapadmin/commands/user.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/config.py` & `pymap_admin-0.9.1/pymapadmin/config.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_grpc.py` & `pymap_admin-0.9.1/pymapadmin/grpc/admin_grpc.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_pb2.py` & `pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/admin_pb2.pyi` & `pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/health_grpc.py` & `pymap_admin-0.9.1/pymapadmin/grpc/health_grpc.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/health_pb2.py` & `pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/grpc/health_pb2.pyi` & `pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/local.py` & `pymap_admin-0.9.1/pymapadmin/local.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/main.py` & `pymap_admin-0.9.1/pymapadmin/main.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/pymapadmin/typing.py` & `pymap_admin-0.9.1/pymapadmin/typing.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/handler.py` & `pymap_admin-0.9.1/test/handler.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/test_health.py` & `pymap_admin-0.9.1/test/test_health.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/test_mailbox.py` & `pymap_admin-0.9.1/test/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/test_system.py` & `pymap_admin-0.9.1/test/test_system.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/test_user.py` & `pymap_admin-0.9.1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `pymap-admin-0.9.0rc1/test/test_version.py` & `pymap_admin-0.9.1/test/test_version.py`

 * *Files identical despite different names*

