# Comparing `tmp/deepfos-ipc-1.2.3.tar.gz` & `tmp/deepfos-ipc-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfos-ipc-1.2.3.tar", last modified: Fri Mar 24 06:13:15 2023, max compression
+gzip compressed data, was "deepfos-ipc-1.2.4.tar", last modified: Sun Apr 23 06:33:12 2023, max compression
```

## Comparing `deepfos-ipc-1.2.3.tar` & `deepfos-ipc-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 06:13:14.995009 deepfos-ipc-1.2.3/
--rw-rw-rw-   0        0        0       48 2023-03-24 05:22:48.000000 deepfos-ipc-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3416 2023-03-24 06:13:14.996009 deepfos-ipc-1.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-24 06:13:14.993008 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/
--rw-rw-rw-   0        0        0     3416 2023-03-24 06:13:14.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-03-24 06:13:14.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 06:13:14.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-24 04:59:47.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-03-24 06:13:14.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-24 06:13:14.000000 deepfos-ipc-1.2.3/deepfos_ipc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-24 06:13:14.997009 deepfos-ipc-1.2.3/dip/
--rw-rw-rw-   0        0        0      129 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/dip/__init__.py
--rw-rw-rw-   0        0        0      518 2023-03-24 06:13:14.997009 deepfos-ipc-1.2.3/dip/_version.py
--rw-rw-rw-   0        0        0     2515 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/dip/client.py
--rw-rw-rw-   0        0        0     2820 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/dip/connection.py
--rw-rw-rw-   0        0        0      824 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/dip/errors.py
--rw-rw-rw-   0        0        0     2263 2023-03-24 04:14:52.000000 deepfos-ipc-1.2.3/dip/pool.py
--rw-rw-rw-   0        0        0     6092 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/dip/proto.py
--rw-rw-rw-   0        0        0     4120 2023-03-24 04:14:52.000000 deepfos-ipc-1.2.3/dip/server.py
--rw-rw-rw-   0        0        0      944 2023-03-24 06:13:14.997009 deepfos-ipc-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      144 2023-03-24 05:22:48.000000 deepfos-ipc-1.2.3/setup.py
--rw-rw-rw-   0        0        0    80318 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.3/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:33:12.538838 deepfos-ipc-1.2.4/
+-rw-rw-rw-   0        0        0       48 2023-03-24 05:22:48.000000 deepfos-ipc-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3474 2023-04-23 06:33:12.538838 deepfos-ipc-1.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 06:33:12.535838 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/
+-rw-rw-rw-   0        0        0     3474 2023-04-23 06:33:12.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-04-23 06:33:12.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:33:12.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-24 04:59:47.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-23 06:33:12.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-23 06:33:12.000000 deepfos-ipc-1.2.4/deepfos_ipc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 06:33:12.540839 deepfos-ipc-1.2.4/dip/
+-rw-rw-rw-   0        0        0      129 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.4/dip/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-23 06:33:12.540839 deepfos-ipc-1.2.4/dip/_version.py
+-rw-rw-rw-   0        0        0     2628 2023-04-17 10:23:11.000000 deepfos-ipc-1.2.4/dip/client.py
+-rw-rw-rw-   0        0        0     3079 2023-04-17 10:27:09.000000 deepfos-ipc-1.2.4/dip/connection.py
+-rw-rw-rw-   0        0        0      847 2023-04-14 08:29:55.000000 deepfos-ipc-1.2.4/dip/errors.py
+-rw-rw-rw-   0        0        0     2319 2023-04-23 06:28:24.000000 deepfos-ipc-1.2.4/dip/pool.py
+-rw-rw-rw-   0        0        0     6570 2023-04-18 02:11:47.000000 deepfos-ipc-1.2.4/dip/proto.py
+-rw-rw-rw-   0        0        0     3938 2023-04-23 06:24:46.000000 deepfos-ipc-1.2.4/dip/server.py
+-rw-rw-rw-   0        0        0      944 2023-04-23 06:33:12.540839 deepfos-ipc-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      144 2023-03-24 05:22:48.000000 deepfos-ipc-1.2.4/setup.py
+-rw-rw-rw-   0        0        0    80318 2023-03-24 03:46:34.000000 deepfos-ipc-1.2.4/versioneer.py
```

### Comparing `deepfos-ipc-1.2.3/PKG-INFO` & `deepfos-ipc-1.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos-ipc
-Version: 1.2.3
+Version: 1.2.4
 Summary: DeepFOS interprocess communication protocol
 Home-page: UNKNOWN
 Author: deepfos-python
 Author-email: 'python@deepfos.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,31 +61,31 @@
 
 ```python
 import typing
 from dip import Protocol
 
 class NewProtocol(Protocol, mtype=b'N'):
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
+    def decode_body(cls, buf: bytes) -> typing.Any:
         pass
     
     @classmethod
-    def _encode(cls, data: typing.Any) -> bytes:
+    def encode_body(cls, data: typing.Any) -> bytes:
         pass
 ```
 
-自定义通信协议需要使用一个byte作为标识（mtype），并且必须实现`_decode`和`_encode`两个方法。其中:
+自定义通信协议需要使用一个byte作为标识（mtype），并且必须实现`decode_body`和`encode_body`两个方法。其中:
 
-> 1. `_encode` 用于将python对象序列化为字节流
-> 2. `_decode` 用于将字节流反序列化为python对象
+> 1. `encode_body` 用于将python对象序列化为字节流
+> 2. `decode_body` 用于将字节流反序列化为python对象
 
 两者一般互为逆操作，即对于python对象`obj`：
 
 ```python
-obj == Protocol.decode(Protocol.encode(obj))
+obj == Protocol.decode_body(Protocol.encode_body(obj))
 ```
 *注: 这并不是硬性规定，只是一种通常做法*
 
 下述是一个非常粗糙的固定字符串压缩协议的实现
 
 ```python
 from dip import Protocol
@@ -96,23 +96,23 @@
         'Hello World': b'h',
     }
     MAP_REV = {
         v: k for k, v in MAP.items()
     }
     
     @classmethod
-    def _decode(cls, buf: bytes) -> str:
-        data = cls.MAP_REV.get(buf)
+    def decode_body(cls, buf: memoryview) -> str:
+        data = cls.MAP_REV.get(buf.tobytes())
         if data is not None:
             return data
         else:
             raise errors.ProtoDecodeError(f'Cannot decode byte: {buf!r}')
 
     @classmethod
-    def _encode(cls, data: str) -> bytes:
+    def encode_body(cls, data: str)  -> bytes:
         compressed = cls.MAP.get(data)
         if compressed is not None:
             return compressed
         else:
             raise errors.ProtoEncodeError(f'Cannot encode string: {data!r}')
 ```
```

### Comparing `deepfos-ipc-1.2.3/deepfos_ipc.egg-info/PKG-INFO` & `deepfos-ipc-1.2.4/deepfos_ipc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos-ipc
-Version: 1.2.3
+Version: 1.2.4
 Summary: DeepFOS interprocess communication protocol
 Home-page: UNKNOWN
 Author: deepfos-python
 Author-email: 'python@deepfos.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,31 +61,31 @@
 
 ```python
 import typing
 from dip import Protocol
 
 class NewProtocol(Protocol, mtype=b'N'):
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
+    def decode_body(cls, buf: bytes) -> typing.Any:
         pass
     
     @classmethod
-    def _encode(cls, data: typing.Any) -> bytes:
+    def encode_body(cls, data: typing.Any) -> bytes:
         pass
 ```
 
-自定义通信协议需要使用一个byte作为标识（mtype），并且必须实现`_decode`和`_encode`两个方法。其中:
+自定义通信协议需要使用一个byte作为标识（mtype），并且必须实现`decode_body`和`encode_body`两个方法。其中:
 
-> 1. `_encode` 用于将python对象序列化为字节流
-> 2. `_decode` 用于将字节流反序列化为python对象
+> 1. `encode_body` 用于将python对象序列化为字节流
+> 2. `decode_body` 用于将字节流反序列化为python对象
 
 两者一般互为逆操作，即对于python对象`obj`：
 
 ```python
-obj == Protocol.decode(Protocol.encode(obj))
+obj == Protocol.decode_body(Protocol.encode_body(obj))
 ```
 *注: 这并不是硬性规定，只是一种通常做法*
 
 下述是一个非常粗糙的固定字符串压缩协议的实现
 
 ```python
 from dip import Protocol
@@ -96,23 +96,23 @@
         'Hello World': b'h',
     }
     MAP_REV = {
         v: k for k, v in MAP.items()
     }
     
     @classmethod
-    def _decode(cls, buf: bytes) -> str:
-        data = cls.MAP_REV.get(buf)
+    def decode_body(cls, buf: memoryview) -> str:
+        data = cls.MAP_REV.get(buf.tobytes())
         if data is not None:
             return data
         else:
             raise errors.ProtoDecodeError(f'Cannot decode byte: {buf!r}')
 
     @classmethod
-    def _encode(cls, data: str) -> bytes:
+    def encode_body(cls, data: str)  -> bytes:
         compressed = cls.MAP.get(data)
         if compressed is not None:
             return compressed
         else:
             raise errors.ProtoEncodeError(f'Cannot encode string: {data!r}')
 ```
```

### Comparing `deepfos-ipc-1.2.3/dip/client.py` & `deepfos-ipc-1.2.4/dip/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 import uuid
 
 from dip.pool import ConnectionPool
 from dip import errors
 
 
 DEFAULT_UUID = uuid.UUID('00000000-0000-0000-0000-00000dee9f03')
+T_PoolCacheKey = typing.Tuple[uuid.UUID, int]
+T_PoolCache = typing.Dict[T_PoolCacheKey, ConnectionPool]
 
 
 class Client:
-    shared_pool: typing.Dict[int, ConnectionPool] = {}
+    shared_pool: T_PoolCache = {}
 
     def __init__(
         self,
         sockname: str,
-        id: typing.Union[str, uuid.UUID] = DEFAULT_UUID,
-        loop: asyncio.BaseEventLoop = None,
+        id: typing.Union[str, uuid.UUID] = DEFAULT_UUID,  # noqa
+        loop: asyncio.AbstractEventLoop = None,
         use_shared_pool: bool = True,
         pool_size: int = 16,
         **conn_options,
     ):
         if isinstance(id, str):
             self._id = uuid.UUID(id)
         else:
@@ -30,16 +32,16 @@
         self._loop = loop or asyncio.get_running_loop()
         self._use_shared_pool = use_shared_pool
         self._pool_size = pool_size
         self._conn_opts = conn_options
         self._inited = False
 
     @cached_property
-    def _pool_key(self):
-        return (self._id, id(self._loop))
+    def _pool_key(self) -> T_PoolCacheKey:
+        return self._id, id(self._loop)
 
     @cached_property
     def pool(self) -> ConnectionPool:
         self._inited = True
         if self._use_shared_pool:
             shared_pool = self.__class__.shared_pool
             if (pool := shared_pool.get(self._pool_key)) is None:
```

### Comparing `deepfos-ipc-1.2.3/dip/connection.py` & `deepfos-ipc-1.2.4/dip/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import typing
+import uuid
 
 from loguru import logger
 from dip.proto import Protocol
 from dip import errors
 
 
 class ClientProtocol(asyncio.Protocol):
@@ -15,38 +16,46 @@
 
     def connection_made(self, transport):
         self.transport = transport
 
     def data_received(self, data):
         if data and not self.conn.future.done():
             self.conn.future.set_result(data)
-        logger.opt(lazy=True).debug("Data received: {!r}".format(data.decode()))
+        logger.opt(lazy=True).debug(
+            "Data received: {dd!r}", dd=lambda: data.decode())
 
     def connection_lost(self, error):
         self._closed = True
         if error:
             self.conn.future.set_exception(error)
 
     @property
     def closed(self):
         return self._closed
 
 
 class Connection:
+    if typing.TYPE_CHECKING:
+        transport: typing.Optional[asyncio.Transport]
+        proto: typing.Optional[ClientProtocol]
+        future: typing.Optional[asyncio.Future]
+        id: typing.Optional[uuid.UUID]
+        timeout: typing.Optional[int]
+
     def __init__(
         self,
         sockname: str,
-        loop: asyncio.BaseEventLoop,
+        loop: asyncio.AbstractEventLoop,
         **options,
     ):
         self.sockname = sockname
         self._loop = loop
-        self.transport: asyncio.Transport = None
-        self.proto: ClientProtocol = None
-        self.future: asyncio.Future = None
+        self.transport = None
+        self.proto = None
+        self.future = None
         self.timeout = options.get('timeout', 5)
         self.id = options.get('connection_id')
 
     @property
     def closed(self) -> bool:
         return (
             self.transport is None
@@ -70,16 +79,16 @@
 
     async def request(self, mtype: str, message: typing.Any):
         """向服务端发送数据"""
         if self.closed:
             raise errors.ConnectionClosed("Cannot issue request after connection close.")
 
         self.future = self._loop.create_future()
-        data = Protocol.dispatch(ord(mtype)).encode(message)
-        self.transport.write(data)
+        for data in Protocol.dispatch(ord(mtype)).encode(message):
+            self.transport.write(data)
         try:
             return await asyncio.wait_for(self.future, self.timeout)
         except asyncio.TimeoutError:
             raise errors.ReadTimeout(
                 f'Server failed to respond after '
                 f'{self.timeout} seconds.') from None
```

### Comparing `deepfos-ipc-1.2.3/dip/errors.py` & `deepfos-ipc-1.2.4/dip/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,21 @@
     pass
 
 
 class ReadTimeout(DeepFOSIOError):
     pass
 
 
-class ConnectionError(DeepFOSIOError):
+class DeepFOSConnectionError(DeepFOSIOError):
     pass
 
 
-class ConnectionClosed(DeepFOSIOError):
+class ConnectionClosed(DeepFOSConnectionError):
     pass
 
 
-class ConnectionAquireTimeout(DeepFOSIOError):
+class ConnectionAquireTimeout(DeepFOSConnectionError):
     pass
 
 
 class ResponseError(DeepFOSIOError):
     pass
```

### Comparing `deepfos-ipc-1.2.3/dip/pool.py` & `deepfos-ipc-1.2.4/dip/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from loguru import logger
 
 from dip import errors
 from dip.connection import Connection
 
 
 class ConnectionPool:
-    def __init__(self,
+    def __init__(
+        self,
         sockname: str,
-        loop: asyncio.BaseEventLoop = None,
+        loop: asyncio.AbstractEventLoop = None,
         maxsize: int = 16,
         **conn_options,
     ):
         self._sockname = sockname
         self._loop = loop or asyncio.get_running_loop()
         self._conn_opts = conn_options
         self.maxsize = maxsize
         self.queue: asyncio.Queue = asyncio.Queue(maxsize=maxsize)
         self.lock = asyncio.Lock()
         self._conns: typing.Set[Connection] = set()
 
-    async def _new_connection(self):
+    async def _new_connection(self) -> Connection:
         logger.debug(f'Create new connection to {self._sockname}')
         conn = Connection(self._sockname, self._loop, **self._conn_opts)
         await conn.connect()
         self._conns.add(conn)
         return conn
 
     async def aquire(self, timeout: int = 10) -> Connection:
@@ -50,15 +51,15 @@
     async def release(self, conn: Connection):
         if conn.closed:
             self._conns.discard(conn)
         else:
             await self.queue.put(conn)
 
     @contextlib.asynccontextmanager
-    async def __call__(self) -> Connection:
+    async def __call__(self) -> typing.AsyncContextManager[Connection]:
         conn = await self.aquire()
         try:
             yield conn
         finally:
             await self.release(conn)
 
     def dispose(self):
```

### Comparing `deepfos-ipc-1.2.3/dip/proto.py` & `deepfos-ipc-1.2.4/dip/proto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import json
 import pickle
 import struct
 import typing
 import uuid
-from io import BytesIO
 
 from dip import errors
 
 read_uint32 = struct.Struct('!I').unpack
 to_uint32 = struct.Struct('!I').pack
 read_uint16 = struct.Struct('!H').unpack
 to_uint16 = struct.Struct('!H').pack
 read_uint8 = struct.Struct('!B').unpack
 
 U32 = 0xFFFFFFFF
 
 
+class MemoryStream:
+    def __init__(self, view: memoryview):
+        self.view = view
+        self.ptr = 0
+
+    def read(self, nbytes: int):
+        start = self.ptr
+        self.ptr += nbytes
+        return self.view[start: self.ptr]
+
+
 class Protocol:
     registry: typing.Dict[int, typing.Type['Protocol']] = {}
 
     if typing.TYPE_CHECKING:
         MSG_TYPE = b''
 
     @classmethod
-    def decode(cls, buf: bytes) -> typing.Any:
-        return cls._decode(buf[5:])
+    def decode_body(cls, buf: memoryview) -> typing.Any:
+        raise NotImplementedError()
 
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
-        raise NotImplemented
+    def encode_body(cls, data: typing.Any) -> bytes:
+        raise NotImplementedError()
 
     @classmethod
-    def _encode(cls, data: typing.Any) -> bytes:
-        raise NotImplemented
+    def decode(cls, buf: memoryview) -> typing.Any:
+        return cls.decode_body(buf[5:])
 
     @classmethod
-    def encode(cls, data: typing.Any) -> bytes:
-        buf = cls._encode(data)
+    def encode(cls, data: typing.Any) -> typing.Tuple[bytes, bytes, memoryview]:
+        buf = cls.encode_body(data)
         if (buf_len := len(buf)) > U32:
             raise errors.ProtoEncodeError(
                 f'Message ({buf_len}) exceeds max length ({U32}).')
-        return cls.MSG_TYPE + to_uint32(len(buf)) + buf
+        return cls.MSG_TYPE, to_uint32(len(buf)), memoryview(buf)
 
     def __init_subclass__(cls, mtype: bytes = None, **kwargs):
         if mtype is not None:
             m_ord = read_uint8(mtype)[0]
             if m_ord in cls.registry:
                 raise errors.DuplicateProtoError(
                     f'Cannot set mtype {mtype} for {cls} because '
@@ -63,120 +73,120 @@
 
         raise errors.UnsupportedProtoError(
             f'No protocol found in registry for message type: {mtype}')
 
 
 class _StringProtocol(Protocol):
     @classmethod
-    def _decode(cls, buf: bytes) -> str:
-        return buf.decode('utf8')
+    def decode_body(cls, buf: memoryview) -> str:
+        return str(buf, 'utf8')  # noqa
 
     @classmethod
-    def _encode(cls, data: str) -> bytes:
+    def encode_body(cls, data: str) -> bytes:
         return data.encode('utf8')
 
 
 class StdoutProtocol(_StringProtocol, mtype=b'O'):
     pass
 
 
 class StderrProtocol(_StringProtocol, mtype=b'E'):
     pass
 
 
 class PickleProtocl(Protocol, mtype=b'P'):
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
-        return pickle.loads(buf)
+    def decode_body(cls, buf: memoryview) -> typing.Any:
+        return pickle.loads(buf)  # noqa
 
     @classmethod
-    def _encode(cls, data: typing.Any) -> bytes:
+    def encode_body(cls, data: typing.Any) -> bytes:
         return pickle.dumps(data, protocol=-1)
 
 
 class JsonProtocol(Protocol, mtype=b'J'):
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
-        return json.load(BytesIO(buf))
+    def decode_body(cls, buf: memoryview) -> typing.Any:
+        return json.loads(str(buf, 'utf8'))  # noqa
 
     @classmethod
-    def _encode(cls, data: typing.Any) -> bytes:
+    def encode_body(cls, data: typing.Any) -> bytes:
         return json.dumps(data, ensure_ascii=False).encode('utf8')
 
 
 class DictProtocol(Protocol, mtype=b'D'):
     VALID_KEYS = ()
 
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.Any:
+    def decode_body(cls, buf: memoryview) -> typing.Any:
         return dict(cls._iter_record(buf))  # noqa
 
     @classmethod
-    def _iter_record(cls, buf: bytes) -> typing.Tuple[str, str]:
-        stream = BytesIO(buf)
+    def _iter_record(cls, buf: memoryview) -> typing.Tuple[str, str]:
+        stream = MemoryStream(buf)
         key_len = len(cls.VALID_KEYS)
 
         while key := stream.read(2):
             idx = read_uint16(key)[0]
             if idx >= key_len:
                 raise errors.ProtoDecodeError(
                     f'Field index {idx} exceeds max length ({key_len}).')
             val_len = read_uint32(stream.read(4))[0]
             val_bytes = stream.read(val_len)
             if len(val_bytes) < val_len:
                 raise errors.ProtoDecodeError(
                     f'Not enough bytes to read, '
                     f'expect: {val_len}, got: {len(val_bytes)}')
 
-            yield cls.VALID_KEYS[idx], val_bytes.decode('utf8')
+            yield cls.VALID_KEYS[idx], str(val_bytes, 'utf8')  # noqa
 
     @classmethod
     def _iter_buf(cls, data: typing.Dict[str, str]):
         try:
             for k, v in data.items():
                 yield to_uint16(cls.VALID_KEYS.index(k))
                 str_encode = v.encode('utf8')
                 yield to_uint32(len(str_encode))
                 yield str_encode
         except ValueError:
             raise errors.ProtoEncodeError(
                 f'Field {k!r} has not been registered, '  # noqa
-                f'valid fields are {cls.VALID_KEYS}')
+                f'valid fields are {cls.VALID_KEYS}') from None
 
     @classmethod
-    def _encode(cls, data: typing.Dict[str, str]) -> bytes:
+    def encode_body(cls, data: typing.Dict[str, str]) -> bytes:
         return b''.join(cls._iter_buf(data))
 
 
 class ListProtocol(Protocol):
     element_proto: typing.Type[Protocol]
 
     @classmethod
-    def _decode(cls, buf: bytes) -> typing.List[typing.Any]:
+    def decode_body(cls, buf: memoryview) -> typing.List[typing.Any]:
         return list(cls._iter_item(buf))
 
     @classmethod
-    def _iter_item(cls, buf: bytes) -> typing.Any:
-        stream = BytesIO(buf)
+    def _iter_item(cls, buf: memoryview) -> typing.Any:
+        stream = MemoryStream(buf)
         ele_mtype = cls.element_proto.MSG_TYPE
 
         while mtype := stream.read(1):
             if mtype != ele_mtype:
                 raise errors.ProtoDecodeError(
                     f'Invalid element for {mtype}, expect {ele_mtype}')
 
             val_len = read_uint32(stream.read(4))[0]
             val_bytes = stream.read(val_len)
-            yield cls.element_proto._decode(val_bytes)
+            yield cls.element_proto.decode_body(val_bytes)
 
     @classmethod
-    def _encode(cls, data: typing.List[typing.Any]) -> bytes:
+    def encode_body(cls, data: typing.List[typing.Any]) -> bytes:
         return b''.join(
+            ele for item in data for ele in
             cls.element_proto.encode(item)
-            for item in data
         )
 
 
 class HeaderProto(DictProtocol, mtype=b'H'):
     VALID_KEYS = ('header', )
 
 
@@ -194,13 +204,13 @@
 
 class TaskUpdateProtoV2(ListProtocol, mtype=b'I'):
     element_proto = JsonProtocol
 
 
 class SetConnectionIdProto(Protocol, mtype=b'\x1d'):
     @classmethod
-    def _decode(cls, buf: bytes) -> uuid.UUID:
-        return uuid.UUID(bytes=buf)
+    def decode_body(cls, buf: memoryview) -> uuid.UUID:
+        return uuid.UUID(bytes=buf.tobytes())
 
     @classmethod
-    def _encode(cls, data: uuid.UUID) -> bytes:
+    def encode_body(cls, data: uuid.UUID) -> bytes:
         return data.bytes
```

### Comparing `deepfos-ipc-1.2.3/dip/server.py` & `deepfos-ipc-1.2.4/dip/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,95 +2,90 @@
 import typing
 from uuid import UUID
 
 from loguru import logger
 
 from dip.proto import Protocol, SetConnectionIdProto, read_uint32
 
-
-class Stream:
-    def __init__(self):
-        self._pending = None
-        self._ready = []
-
-    def new_segmant(self, buf):
-        buf_len = len(buf)
-        expect_len = read_uint32(buf[1:5])[0] + 5
-        if expect_len == buf_len:
-            self._ready.append(buf)
-            self._pending = None
-        elif expect_len > buf_len:
-            self._pending = buf
-        else:
-            self._ready.append(buf[:expect_len])
-            self._pending = buf[expect_len:]
-
-    def amend_pending(self, buf):
-        new_buf = self._pending + buf
-        self.new_segmant(new_buf)
-
-    def feed_data(self, buf: bytes):
-        if not self._pending:
-            self.new_segmant(buf)
-        else:
-            self.amend_pending(buf)
-
-    def iter_data(self):
-        while self._ready:
-            yield self._ready.pop(0)
-
-
 # -----------------------------------------------------------------------------
 # typing
 
 T = typing.TypeVar('T', bound='DeepfosIPCProtocol')
 Callback_T = typing.Callable[
     [UUID, str, typing.Any],
     typing.Any
 ]
 
 
-class DeepfosIPCProtocol(asyncio.Protocol):
-    def __init__(self: T, callback: Callback_T = None, **kwargs) -> None:
+class DeepfosIPCProtocol(asyncio.BufferedProtocol):
+    if typing.TYPE_CHECKING:
+        _payload_feeded: bool = False
+
+    def __init__(self: T, callback: Callback_T = None) -> None:
         self.callback = callback
         self.transport = None
         self.id = None
-        self._stream = Stream()
+        self._new_playload()
 
-    def abort(self):
-        self._stream = Stream()
+    def _new_playload(self):
+        self._new_buffer(5)
 
-    def connection_made(self, transport):
-        self.transport = transport
+    def _new_buffer(
+        self,
+        size: int,
+        is_payload: bool = True,
+        mtype: int = None
+    ):
+        self._mtype = mtype
+        self._buf_idx = 0
+        self._buf = memoryview(bytearray(size))
+        self._is_payload = is_payload
+        self._expect_len = size
 
-    def data_received(self, data):
-        self._stream.feed_data(data)
+    def abort(self):
+        self._new_playload()
 
-        errors = []
-        data_processed = False
+    def get_buffer(self, sizehint: int):
+        return self._buf[self._buf_idx:]
 
-        for buf in self._stream.iter_data():
-            data_processed = True
+    def buffer_updated(self, nbytes: int) -> None:
+        self._buf_idx += nbytes
+
+        if self._buf_idx != self._expect_len:
+            return
+
+        if self._is_payload:
+            self._new_buffer(
+                size=read_uint32(memoryview(self._buf[1:5]))[0],
+                is_payload=False,
+                mtype=self._buf[0]
+            )
+        else:
             try:
-                self.process_message(buf)
+                self.process_message(self._buf)
+                errors = None
             except Exception as e:
                 self.abort()
                 logger.error(e)
-                errors.append(repr(e).encode("utf8"))
+                errors = repr(e).encode("utf8")
 
-        if data_processed:
             if errors:
-                self.transport.write(b''.join(errors))
+                self.transport.write(errors)
             else:
                 self.transport.write(b"ok")
 
-    def process_message(self, data):
-        mtype = data[0]
+            self._new_playload()
+
+    def connection_made(self, transport):
+        self.transport = transport
+
+    def process_message(self, data: memoryview):
+        mtype = self._mtype
         proto = Protocol.dispatch(mtype)
-        decoded = proto.decode(data)
+        decoded = proto.decode_body(data)
         logger.opt(lazy=True).debug("Receive data: {data!r}", data=lambda: decoded)
         if proto is SetConnectionIdProto:
             self.id = decoded
         elif self.callback is not None:
             self.callback(self.id, chr(mtype), decoded)
 
     def connection_lost(self, error):
@@ -99,34 +94,31 @@
         else:
             logger.debug('connection closed.')
         super().connection_lost(error)
         self.transport = None
 
 
 class Server:
-    """
-    启动Server服务.
-    """
     def __init__(
         self,
         sockname: str,
         callback: Callback_T = None,
-        loop: asyncio.BaseEventLoop = None,
-        **kwrags
+        loop: asyncio.AbstractEventLoop = None,
+        **kwargs
     ) -> None:
         self.sockname = sockname
         self.callback = callback
         self.waiter = None
         self.server = None
-        self.kwargs = kwrags
+        self.kwargs = kwargs
         self._loop = loop or asyncio.get_running_loop()
 
     async def _create_server(self):
         srv = await self._loop.create_unix_server(
-            lambda: DeepfosIPCProtocol(self.callback, **self.kwargs),
+            lambda: DeepfosIPCProtocol(self.callback),
             self.sockname,
         )
         return srv
 
     async def start(self):
         self.server = await self._create_server()
         return self.server
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deepfos-ipc-1.2.3/setup.cfg` & `deepfos-ipc-1.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepfos-ipc-1.2.3/versioneer.py` & `deepfos-ipc-1.2.4/versioneer.py`

 * *Files identical despite different names*

