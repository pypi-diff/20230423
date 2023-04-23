# Comparing `tmp/pymap_admin-0.9.1.tar.gz` & `tmp/pymap_admin-0.9.2.tar.gz`

## Comparing `pymap_admin-0.9.1.tar` & `pymap_admin-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.flake8
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.gitattributes
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/__about__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/__init__.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/config.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/local.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/py.typed
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/typing.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/__init__.py
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/base.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/health.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/mailbox.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/system.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/commands/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/__init__.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin.proto
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_grpc.py
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.py
--rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.pyi
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/grpc_tools.protoc-args
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health.proto
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_grpc.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.pyi
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/handler.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_health.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_mailbox.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_system.py
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_user.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/test/test_version.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/LICENSE.md
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/README.md
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 pymap_admin-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/.flake8
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/.gitattributes
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/__about__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/__init__.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/config.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/local.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/py.typed
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/typing.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/__init__.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/base.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/health.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/mailbox.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/system.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/commands/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/__init__.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/admin.proto
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/admin_grpc.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/admin_pb2.py
+-rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/admin_pb2.pyi
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/grpc_tools.protoc-args
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/health.proto
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/health_grpc.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/health_pb2.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pymapadmin/grpc/health_pb2.pyi
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/handler.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/test_health.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/test_mailbox.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/test_system.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/test_user.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/test/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/LICENSE.md
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/README.md
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 pymap_admin-0.9.2/PKG-INFO
```

### Comparing `pymap_admin-0.9.1/pymapadmin/config.py` & `pymap_admin-0.9.2/pymapadmin/config.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/local.py` & `pymap_admin-0.9.2/pymapadmin/local.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/main.py` & `pymap_admin-0.9.2/pymapadmin/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import asyncio
 from argparse import ArgumentParser, Namespace
 from ssl import create_default_context, CERT_NONE
 
 from grpclib.client import Channel
-from pymapadmin import __version__
+from pymapadmin.__about__ import __version__
 
 from .commands import load_commands
 from .commands.base import Command
 from .config import Config
 from .local import config_file, token_file, socket_file
```

### Comparing `pymap_admin-0.9.1/pymapadmin/typing.py` & `pymap_admin-0.9.2/pymapadmin/typing.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/__init__.py` & `pymap_admin-0.9.2/pymapadmin/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/base.py` & `pymap_admin-0.9.2/pymapadmin/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from abc import abstractmethod, ABCMeta
 from argparse import ArgumentParser, Namespace
 from collections.abc import Mapping
 from typing import Generic, Any, Final, TextIO
 
 from grpclib.client import Channel
 
-from .. import __version__ as client_version
+from ..__about__ import __version__ as client_version
 from ..local import token_file
 from ..typing import StubT, MethodProtocol, RequestT, ResponseT, \
     AdminRequestT, AdminResponseT
 from ..grpc.admin_pb2 import SUCCESS
 
 try:
     # This import ensures error details are displayed correctly
```

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/health.py` & `pymap_admin-0.9.2/pymapadmin/commands/health.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/mailbox.py` & `pymap_admin-0.9.2/pymapadmin/commands/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/system.py` & `pymap_admin-0.9.2/pymapadmin/commands/system.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/commands/user.py` & `pymap_admin-0.9.2/pymapadmin/commands/user.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/admin.proto` & `pymap_admin-0.9.2/pymapadmin/grpc/admin.proto`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/admin_grpc.py` & `pymap_admin-0.9.2/pymapadmin/grpc/admin_grpc.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.py` & `pymap_admin-0.9.2/pymapadmin/grpc/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/admin_pb2.pyi` & `pymap_admin-0.9.2/pymapadmin/grpc/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/health.proto` & `pymap_admin-0.9.2/pymapadmin/grpc/health.proto`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/health_grpc.py` & `pymap_admin-0.9.2/pymapadmin/grpc/health_grpc.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.py` & `pymap_admin-0.9.2/pymapadmin/grpc/health_pb2.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pymapadmin/grpc/health_pb2.pyi` & `pymap_admin-0.9.2/pymapadmin/grpc/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/handler.py` & `pymap_admin-0.9.2/test/handler.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/test_health.py` & `pymap_admin-0.9.2/test/test_health.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/test_mailbox.py` & `pymap_admin-0.9.2/test/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/test_system.py` & `pymap_admin-0.9.2/test/test_system.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/test_user.py` & `pymap_admin-0.9.2/test/test_user.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/test/test_version.py` & `pymap_admin-0.9.2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/.gitignore` & `pymap_admin-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/LICENSE.md` & `pymap_admin-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/README.md` & `pymap_admin-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/pyproject.toml` & `pymap_admin-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymap_admin-0.9.1/PKG-INFO` & `pymap_admin-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymap-admin
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tool for administering running pymap instances.
 Project-URL: Homepage, https://github.com/icgood/pymap-admin/
 Project-URL: API Documentation, https://icgood.github.io/pymap-admin/
 Author-email: Ian Good <ian@icgood.net>
 License: ## The MIT License (MIT)
         
         Copyright (c) 2022 Ian Good
```

