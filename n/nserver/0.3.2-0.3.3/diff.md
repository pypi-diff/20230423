# Comparing `tmp/nserver-0.3.2-py3-none-any.whl.zip` & `tmp/nserver-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 19375 bytes, number of entries: 14
+Zip file size: 19972 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      180 b- defN 21-Feb-06 17:59 nserver/__init__.py
--rw-r--r--  2.0 unx     2033 b- defN 23-Jan-26 05:54 nserver/_version.py
--rw-r--r--  2.0 unx     3274 b- defN 22-May-01 09:55 nserver/models.py
+-rw-r--r--  2.0 unx     2032 b- defN 23-Apr-23 10:57 nserver/_version.py
+-rw-r--r--  2.0 unx     3275 b- defN 23-Apr-23 10:26 nserver/models.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-01 11:08 nserver/py.typed
--rw-r--r--  2.0 unx     6361 b- defN 23-Jan-26 05:29 nserver/records.py
+-rw-r--r--  2.0 unx     6362 b- defN 23-Apr-23 10:26 nserver/records.py
 -rw-r--r--  2.0 unx     5030 b- defN 21-Jul-17 15:59 nserver/rules.py
--rw-r--r--  2.0 unx    13759 b- defN 22-Oct-30 20:04 nserver/server.py
--rw-r--r--  2.0 unx    17985 b- defN 23-Jan-26 05:52 nserver/transport.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/LICENCE
--rw-r--r--  2.0 unx     6825 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx      220 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1067 b- defN 23-Jan-26 05:54 nserver-0.3.2.dist-info/RECORD
-14 files, 57905 bytes uncompressed, 17627 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx    13760 b- defN 23-Apr-23 10:26 nserver/server.py
+-rw-r--r--  2.0 unx    17989 b- defN 23-Apr-23 10:32 nserver/transport.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/LICENCE
+-rw-r--r--  2.0 unx     8029 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/RECORD
+14 files, 59115 bytes uncompressed, 18224 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: nserver/server.py
 Comment: 
 
 Filename: nserver/transport.py
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/LICENCE
+Filename: nserver-0.3.3.dist-info/LICENCE
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/METADATA
+Filename: nserver-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/NOTICE
+Filename: nserver-0.3.3.dist-info/NOTICE
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/WHEEL
+Filename: nserver-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/top_level.txt
+Filename: nserver-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: nserver-0.3.2.dist-info/RECORD
+Filename: nserver-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nserver/_version.py

```diff
@@ -8,21 +8,21 @@
 ## Application
 
 ### CONSTANTS
 ### ============================================================================
 ## Version Information - DO NOT EDIT
 ## -----------------------------------------------------------------------------
 # These variables will be set during the build process. Do not attempt to edit.
-PACKAGE_VERSION = "0.3.2"
-BUILD_VERSION = "0.3.2"
-BUILD_GIT_HASH = "be352b6fcc3b50c8c4f193b45fbd564c10584d23"
-BUILD_GIT_HASH_SHORT = "be352b6"
-BUILD_GIT_BRANCH = "master"
-BUILD_TIMESTAMP = 1674712436
-BUILD_DATETIME = datetime.datetime.utcfromtimestamp(1674712436)
+PACKAGE_VERSION = "0.3.3"
+BUILD_VERSION = "0.3.3"
+BUILD_GIT_HASH = "62bb4f9029e729045588e1545a8f0f2920905a86"
+BUILD_GIT_HASH_SHORT = "62bb4f9"
+BUILD_GIT_BRANCH = "main"
+BUILD_TIMESTAMP = 1682247461
+BUILD_DATETIME = datetime.datetime.utcfromtimestamp(1682247461)
 
 VERSION_VARS = vars()  # Don't have f-strings until py36
 
 ## Version Information Templates
 ## -----------------------------------------------------------------------------
 # You can customise the templates used for version information here.
 VERSION_INFO_TEMPLATE_SHORT = "{BUILD_VERSION}"
@@ -32,14 +32,15 @@
 )
 VERSION_INFO_TEMPLATE_FULL = (
     "{PACKAGE_VERSION} ({BUILD_VERSION})\n"
     "{BUILD_GIT_BRANCH}@{BUILD_GIT_HASH}\n"
     "Built: {BUILD_DATETIME}"
 )
 
+
 ### FUNCTIONS
 ### ============================================================================
 def get_version_info_short() -> str:  # pylint: disable=missing-function-docstring
     return VERSION_INFO_TEMPLATE_SHORT.format(**VERSION_VARS)
 
 
 def get_version_info() -> str:  # pylint: disable=missing-function-docstring
```

## nserver/models.py

```diff
@@ -5,14 +5,15 @@
 
 ## Installed
 import dnslib
 
 ## Application
 from .records import RecordBase
 
+
 ### CLASSES
 ### ============================================================================
 class Query:  # pylint: disable=too-few-public-methods
     """Simplified version of a DNS query.
 
     This class acts as an adaptor for dnslib classes.
     """
```

## nserver/records.py

```diff
@@ -12,14 +12,15 @@
 
 ## Application
 
 ### CONSTANTS
 ### ============================================================================
 DEFAULT_TTL = 300
 
+
 ### CLASSES
 ### ============================================================================
 class RecordBase:
     """Base class for all DNS records.
 
     NOT to be used directly.
```

## nserver/server.py

```diff
@@ -10,14 +10,15 @@
 
 ## Application
 from .rules import RuleBase, WildcardStringRule, RegexRule
 from .models import Query, Response
 from .transport import UDPv4Transport, TCPv4Transport, TransportBase, InvalidMessageError
 from .records import RecordBase
 
+
 ### NAME SERVER
 ### ============================================================================
 class NameServer:
     """NameServer for responding to requests."""
 
     # pylint: disable=too-many-instance-attributes
```

## nserver/transport.py

```diff
@@ -12,14 +12,15 @@
 from typing import Tuple, Optional, Dict, List, Deque, NewType, cast
 
 ## Installed
 import dnslib
 
 ## Application
 
+
 ### CONSTANTS
 ### ============================================================================
 class TcpState(IntEnum):
     """State of a TCP connection.
 
     General usage:
     `TcpState(get_tcp_info(connection)[0])`
@@ -68,15 +69,15 @@
     data_remaining = data_length - len(data)
     start_time = time.time()
     while data_remaining > 0:
         data += connection.recv(data_remaining)
         data_remaining = data_length - len(data)
         if data_remaining and time.time() - start_time > timeout:
             msg = f"timeout reading data from {connection.getpeername()}"
-            raise Exception(msg)
+            raise TimeoutError(msg)
     return data
 
 
 ### CLASSES
 ### ============================================================================
 class MessageContainer:  # pylint: disable=too-few-public-methods
     """Class for holding DNS messages and the socket they originated from.
```

## Comparing `nserver-0.3.2.dist-info/LICENCE` & `nserver-0.3.3.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `nserver-0.3.2.dist-info/METADATA` & `nserver-0.3.3.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 Metadata-Version: 2.1
 Name: nserver
-Version: 0.3.2
+Version: 0.3.3
 Summary: DNS Name Server Framework
-Home-page: https://github.com/nhairs/nserver
-Author: Nicholas Hairs
-Author-email: info+nserver@nicholashairs.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Nicholas Hairs <info+nserver@nicholashairs.com>
+License: MIT License
+        
+        Copyright (c) 2020 Nicholas Hairs
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
+Project-URL: homepage, https://github.com/nhairs/nserver
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Name Service (DNS)
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 License-File: NOTICE
 Requires-Dist: dnslib
 Requires-Dist: tldextract
 Provides-Extra: dev
 Requires-Dist: setuptools ; extra == 'dev'
@@ -31,14 +49,15 @@
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: mkdocs ; extra == 'dev'
 Requires-Dist: mkdocs-material (>=8.5) ; extra == 'dev'
 Requires-Dist: mkdocs-awesome-pages-plugin ; extra == 'dev'
 Requires-Dist: mdx-truly-sane-lists ; extra == 'dev'
+Requires-Dist: bpython ; extra == 'dev'
 
 # NServer: a high-level Python DNS Name Server Framework.
 
 [![PyPi](https://img.shields.io/pypi/v/nserver.svg)](https://pypi.python.org/pypi/nserver/)
 [![PyPI - Status](https://img.shields.io/pypi/status/nserver)](https://pypi.python.org/pypi/nserver/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/nserver.svg)](https://github.com/nhairs/nserver)
 [![License](https://img.shields.io/github/license/nhairs/nserver.svg)](https://github.com/nhairs/nserver)
@@ -157,9 +176,7 @@
 ## Licence
 This project is licenced under the MIT Licence - see [`LICENCE`](https://github.com/nahirs/nserver/blob/master/LICENCE).
 
 This project may include other open source licenced software - see [`NOTICE`](https://github.com/nhairs/nserver/blob/master/NOTICE).
 
 ## Authors
 A project by Nicholas Hairs - [www.nicholashairs.com](https://www.nicholashairs.com).
-
-
```

## Comparing `nserver-0.3.2.dist-info/RECORD` & `nserver-0.3.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 nserver/__init__.py,sha256=MajwZ4WrYaWvsA8_lrOFWgZnsAJ-lpdG3BsmDlDA4NU,180
-nserver/_version.py,sha256=es8_WUQf4y7q4kBSlL8FeQUfjI_ZtVm01BZZCF3XYgQ,2033
-nserver/models.py,sha256=xz_jH0QkKvyRwUjBtMe_rjoqEJwvNNdF-i0TE22PK7w,3274
+nserver/_version.py,sha256=vRb8BYhmHsSGPl9aZIkth1iDd7tvhRCTE7o1ybtrTLI,2032
+nserver/models.py,sha256=acuUUF_I_mH8H7e8gGzKTsRnU0RE68e8lzIuTG2K7dw,3275
 nserver/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nserver/records.py,sha256=tZYHv0BhR6EGuRT6RwPbpAdqcyPq1_s9nJBI1RpVw8k,6361
+nserver/records.py,sha256=ZZY-_vN-1B0gcyohHTdhtkGqebemEmdVK6vAHVOzXeM,6362
 nserver/rules.py,sha256=j6XbD8kVcfiAtzbkNWlKpsm45Gc22WYVa8HLGfhpL_w,5030
-nserver/server.py,sha256=etMUlNzJ5_8tmlC7ofElzQvmG493V2EdSUXfg-Kqc2g,13759
-nserver/transport.py,sha256=5nQKC6fQHyoC6_ginxFLB3XC6ZJMa72IBv3O24pTmA8,17985
-nserver-0.3.2.dist-info/LICENCE,sha256=W1bDNCHGJddUmYNElLUEbbOlBPQmFISUR8uja44sOWs,1071
-nserver-0.3.2.dist-info/METADATA,sha256=v7VFjOmvRa1929OJy9INRImf_wjGf1GvkQkIPWwLiUg,6825
-nserver-0.3.2.dist-info/NOTICE,sha256=Qq6ErnuPr87l7y6-8UDasbfi5d7AWFHnWmz1-1N5b2M,220
-nserver-0.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-nserver-0.3.2.dist-info/top_level.txt,sha256=C11DUdis7SN6wOzDVcD08kmX7CQMRY03bxhZaEYX8ZQ,8
-nserver-0.3.2.dist-info/RECORD,,
+nserver/server.py,sha256=wFP14f44wenIrBZ4LaS4dHDzwWCW7v4p626MsSgvgwg,13760
+nserver/transport.py,sha256=YrP5BeZ2yWVULdKh-MwFpHD4ndnywa6fgZk7xkUBxKg,17989
+nserver-0.3.3.dist-info/LICENCE,sha256=W1bDNCHGJddUmYNElLUEbbOlBPQmFISUR8uja44sOWs,1071
+nserver-0.3.3.dist-info/METADATA,sha256=gRB1tvosJop9Wcho-3NMbGd3j9Yy-WBJYrPpXs7yV_M,8029
+nserver-0.3.3.dist-info/NOTICE,sha256=Qq6ErnuPr87l7y6-8UDasbfi5d7AWFHnWmz1-1N5b2M,220
+nserver-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nserver-0.3.3.dist-info/top_level.txt,sha256=C11DUdis7SN6wOzDVcD08kmX7CQMRY03bxhZaEYX8ZQ,8
+nserver-0.3.3.dist-info/RECORD,,
```

