# Comparing `tmp/rlaphoenix_pymp4-1.4.0.tar.gz` & `tmp/rlaphoenix_pymp4-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlaphoenix_pymp4-1.4.0.tar", max compression
+gzip compressed data, was "rlaphoenix_pymp4-1.5.0.tar", max compression
```

## Comparing `rlaphoenix_pymp4-1.4.0.tar` & `rlaphoenix_pymp4-1.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11339 2023-04-23 21:15:44.459232 rlaphoenix_pymp4-1.4.0/LICENSE
--rw-r--r--   0        0        0     1277 2023-04-23 21:18:07.584529 rlaphoenix_pymp4-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1839 2023-04-23 21:15:44.459232 rlaphoenix_pymp4-1.4.0/README.md
--rw-r--r--   0        0        0        1 2023-04-23 21:15:44.461745 rlaphoenix_pymp4-1.4.0/src/pymp4/__init__.py
--rw-r--r--   0        0        0      664 2023-04-23 21:15:44.462744 rlaphoenix_pymp4-1.4.0/src/pymp4/cli.py
--rw-r--r--   0        0        0      651 2023-04-23 21:15:44.462744 rlaphoenix_pymp4-1.4.0/src/pymp4/exceptions.py
--rw-r--r--   0        0        0    28245 2023-04-23 21:15:44.463744 rlaphoenix_pymp4-1.4.0/src/pymp4/parser.py
--rw-r--r--   0        0        0       74 2023-04-23 21:15:44.463744 rlaphoenix_pymp4-1.4.0/src/pymp4/tools/__init__.py
--rw-r--r--   0        0        0     2250 2023-04-23 21:15:44.464744 rlaphoenix_pymp4-1.4.0/src/pymp4/util.py
--rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 rlaphoenix_pymp4-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-03-27 17:24:03.021828 rlaphoenix_pymp4-1.5.0/LICENSE
+-rw-r--r--   0        0        0        1 2023-03-27 17:29:38.178583 rlaphoenix_pymp4-1.5.0/pymp4/__init__.py
+-rw-r--r--   0        0        0      664 2023-03-27 17:29:38.178583 rlaphoenix_pymp4-1.5.0/pymp4/cli.py
+-rw-r--r--   0        0        0      651 2023-03-27 17:29:38.178583 rlaphoenix_pymp4-1.5.0/pymp4/exceptions.py
+-rw-r--r--   0        0        0    28194 2023-03-27 17:29:38.459523 rlaphoenix_pymp4-1.5.0/pymp4/parser.py
+-rw-r--r--   0        0        0       74 2023-03-27 17:29:38.179584 rlaphoenix_pymp4-1.5.0/pymp4/tools/__init__.py
+-rw-r--r--   0        0        0     2250 2023-03-27 17:29:38.502892 rlaphoenix_pymp4-1.5.0/pymp4/util.py
+-rw-r--r--   0        0        0      885 2023-03-27 17:31:48.772385 rlaphoenix_pymp4-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      635 2023-03-27 17:24:03.021828 rlaphoenix_pymp4-1.5.0/README.md
+-rw-r--r--   0        0        0     1978 1970-01-01 00:00:00.000000 rlaphoenix_pymp4-1.5.0/PKG-INFO
```

### Comparing `rlaphoenix_pymp4-1.4.0/LICENSE` & `rlaphoenix_pymp4-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlaphoenix_pymp4-1.4.0/pyproject.toml` & `rlaphoenix_pymp4-1.5.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rlaphoenix.pymp4"
-version = "1.4.0"
-description = "Python parser for MP4 boxes"
+version = "1.5.0"
+description = "A Python parser for MP4 boxes"
 authors = ["beardypig <git@beardypig.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/beardypig/pymp4"
-repository = "https://github.com/beardypig/pymp4"
+homepage = "https://github.com/rlaphoenix/pymp4"
+repository = "https://github.com/rlaphoenix/pymp4"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
 ]
 packages = [
-    { include="pymp4", from="src" }
+    { include = "pymp4" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = "^2.7 || >=3.3,<4.0"
 construct = "2.8.8"
 
-[tool.poetry.group.dev.dependencies]
-coverage = { version="^7.2.3", extras=["toml"] }
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-
 [tool.poetry.scripts]
 mp4dump = "pymp4.cli:dump"
-
-[tool.coverage.run]
-source = ["src/pymp4"]
-omit = [".*", "*/site-packages/*", "*/python?.?/*"]
-
-[tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    "def __repr__",
-    "raise NotImplementedError",
-    "if __name__ == .__main__.:"
-]
```

### Comparing `rlaphoenix_pymp4-1.4.0/src/pymp4/cli.py` & `rlaphoenix_pymp4-1.5.0/pymp4/cli.py`

 * *Files identical despite different names*

### Comparing `rlaphoenix_pymp4-1.4.0/src/pymp4/exceptions.py` & `rlaphoenix_pymp4-1.5.0/pymp4/exceptions.py`

 * *Files identical despite different names*

### Comparing `rlaphoenix_pymp4-1.4.0/src/pymp4/parser.py` & `rlaphoenix_pymp4-1.5.0/pymp4/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
-import logging
+import io
 from uuid import UUID
 
 from construct import *
 import construct.core
 from construct.lib import *
 
-log = logging.getLogger(__name__)
-
 UNITY_MATRIX = [0x10000, 0, 0, 0, 0x10000, 0, 0, 0, 0x40000000]
 
 
 class PrefixedIncludingSize(Subconstruct):
     __slots__ = ["name", "lengthfield", "subcon"]
 
     def __init__(self, lengthfield, subcon):
@@ -38,14 +36,20 @@
             lengthfield_size = self.lengthfield.sizeof()
             length = self.lengthfield._parse(stream, context, path)
         except SizeofError:
             offset_start = stream.tell()
             length = self.lengthfield._parse(stream, context, path)
             lengthfield_size = stream.tell() - offset_start
 
+        if length == 0 or length == 1:
+            curr_pos = stream.tell()
+            stream.seek(0, io.SEEK_END)
+            eof = stream.tell()
+            stream.seek(curr_pos)
+            length = eof - curr_pos + lengthfield_size
         stream2 = BoundBytesIO(stream, length - lengthfield_size)
         obj = self.subcon._parse(stream2, context, path)
         return obj
 
     def _build(self, obj, stream, context, path):
         try:
             # needs to be both fixed size, seekable and tellable (third not checked)
@@ -263,15 +267,16 @@
 HandlerReferenceBox = Struct(
     "type" / Const(b"hdlr"),
     "version" / Const(Int8ub, 0),
     "flags" / Const(Int24ub, 0),
     Padding(4, pattern=b"\x00"),
     "handler_type" / String(4),
     Padding(12, pattern=b"\x00"),  # Int32ub[3]
-    "name" / CString(encoding="utf8")
+    "name" / CString(encoding="utf8"),
+    If(this.name == "", Padding(4, pattern=b"\x00"))
 )
 
 # Boxes contained by Media Info Box
 
 VideoMediaHeaderBox = Struct(
     "type" / Const(b"vmhd"),
     "version" / Default(Int8ub, 0),
@@ -691,34 +696,26 @@
                            PrefixedArray(Int32ub, UUIDBytes(Bytes(16)))),
                         None),
     "init_data" / Prefixed(Int32ub, GreedyBytes)
 )
 
 TrackEncryptionBox = Struct(
     "type" / If(this._.type != b"uuid", Const(b"tenc")),
-    "version" / Default(OneOf(Int8ub, (0, 1)), 0),
+    "version" / Default(Int8ub, 0),
     "flags" / Default(Int24ub, 0),
-    "_reserved" / Const(Int8ub, 0),
-    "default_byte_blocks" / Default(IfThenElse(
-        this.version > 0,
-        BitStruct(
-            # count of encrypted blocks in the protection pattern, where each block is 16-bytes
-            "crypt" / Nibble,
-            # count of unencrypted blocks in the protection pattern
-            "skip" / Nibble
-        ),
-        Const(Int8ub, 0)
-    ), 0),
-    "is_encrypted" / OneOf(Int8ub, (0, 1)),
-    "iv_size" / OneOf(Int8ub, (0, 8, 16)),
+    "_reserved0" / Const(Int8ub, 0),
+    "_reserved1" / Const(Int8ub, 0),
+    "is_encrypted" / Int8ub,
+    "iv_size" / Int8ub,
     "key_ID" / UUIDBytes(Bytes(16)),
-    "constant_iv" / Default(If(
-        this.is_encrypted and this.iv_size == 0,
-        PrefixedArray(Int8ub, Byte)
-    ), None)
+    "constant_iv" / Default(If(this.is_encrypted and this.iv_size == 0,
+                               PrefixedArray(Int8ub, Byte),
+                               ),
+                            None)
+
 )
 
 SampleEncryptionBox = Struct(
     "type" / If(this._.type != b"uuid", Const(b"senc")),
     "version" / Const(Int8ub, 0),
     "flags" / BitStruct(
         Padding(22),
```

### Comparing `rlaphoenix_pymp4-1.4.0/src/pymp4/util.py` & `rlaphoenix_pymp4-1.5.0/pymp4/util.py`

 * *Files identical despite different names*

