# Comparing `tmp/robotnikmq-0.6.1.tar.gz` & `tmp/robotnikmq-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotnikmq-0.6.1.tar", last modified: Tue Apr 18 03:04:26 2023, max compression
+gzip compressed data, was "robotnikmq-0.7.0.tar", last modified: Sun Apr 23 03:35:23 2023, max compression
```

## Comparing `robotnikmq-0.6.1.tar` & `robotnikmq-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/LICENSE
--rw-r--r--   0        0        0     6128 2023-04-16 21:48:51.582507 robotnikmq-0.6.1/README.md
--rw-r--r--   0        0        0     1256 2023-04-18 01:40:55.148760 robotnikmq-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0      337 2023-04-17 01:22:37.631810 robotnikmq-0.6.1/robotnikmq/__init__.py
--rwxr-xr-x   0        0        0     6280 2023-04-16 22:02:59.632874 robotnikmq-0.6.1/robotnikmq/config.py
--rw-r--r--   0        0        0     6278 2023-04-16 22:03:20.340835 robotnikmq-0.6.1/robotnikmq/core.py
--rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/error.py
--rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/log.py
--rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/rpc_client.py
--rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.6.1/robotnikmq/rpc_server.py
--rw-r--r--   0        0        0     3669 2023-04-18 02:34:34.875545 robotnikmq-0.6.1/robotnikmq/subscriber.py
--rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.6.1/robotnikmq/topic.py
--rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.6.1/robotnikmq/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.6.1/tests/integration/__init__.py
--rw-r--r--   0        0        0      454 2023-04-16 23:25:18.821810 robotnikmq-0.6.1/tests/integration/conftest.py
--rwxr-xr-x   0        0        0    16105 2023-04-18 02:39:58.179068 robotnikmq-0.6.1/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0    13569 2023-04-16 22:59:42.127250 robotnikmq-0.6.1/tests/integration/test_rpc.py
--rw-r--r--   0        0        0      622 2023-04-16 22:26:51.861392 robotnikmq-0.6.1/tests/integration/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.6.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     4105 2023-04-16 23:26:37.032343 robotnikmq-0.6.1/tests/unit/test_config.py
--rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_error.py
--rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_message.py
--rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_validation.py
--rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 robotnikmq-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6284 2023-04-23 03:34:39.968822 robotnikmq-0.7.0/README.md
+-rw-r--r--   0        0        0     1299 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/__init__.py
+-rwxr-xr-x   0        0        0     6280 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/config.py
+-rw-r--r--   0        0        0     6434 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/core.py
+-rwxr-xr-x   0        0        0      652 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/error.py
+-rw-r--r--   0        0        0      325 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/log.py
+-rw-r--r--   0        0        0     2543 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/rpc_client.py
+-rw-r--r--   0        0        0    11527 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/rpc_server.py
+-rw-r--r--   0        0        0     4397 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/subscriber.py
+-rwxr-xr-x   0        0        0     2055 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/topic.py
+-rw-r--r--   0        0        0      471 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/utils.py
+-rw-r--r--   0        0        0      364 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/conftest.py
+-rwxr-xr-x   0        0        0    14200 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0    13569 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/test_rpc.py
+-rw-r--r--   0        0        0      622 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.7.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4105 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_config.py
+-rw-r--r--   0        0        0      261 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_error.py
+-rw-r--r--   0        0        0     1818 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_message.py
+-rw-r--r--   0        0        0     1292 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 robotnikmq-0.7.0/PKG-INFO
```

### Comparing `robotnikmq-0.6.1/LICENSE` & `robotnikmq-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/README.md` & `robotnikmq-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,22 @@
 
 **Sublime Text 3**
 
 ```bash
 curl -sSL https://gitlab.com/-/snippets/2385805/raw/main/pdm.sublime-project.py | pdm run python > robotnikmq.sublime-project
 ```
 
+**VSCodium/VSCode**
+
+I recommend installing the [pdm-vscode](https://github.com/frostming/pdm-vscode) plug-in:
+
+```bash
+sudo pdm plugin add pdm-vscode
+```
+
 ## Testing
 
 All testing should be done with `pytest` which is installed with the `dev` requirements.
 
 To run all the unit tests, execute the following from the repo directory:
 
 ```bash
```

### Comparing `robotnikmq-0.6.1/pyproject.toml` & `robotnikmq-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "robotnikmq"
-version = "0.6.1"
+version = "0.7.0"
 description = "Utilities for safe, efficient, and scalable infrastructure using RabbitMQ"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "typeguard>=3.0.2",
     "pyyaml>=6.0",
     "pydantic>=1.0",
     "pika>=1.3.0",
     "funcy>=1.17",
     "arrow>=1.2.3",
-    "logzero>=1.7.0",
     "types-pika>=1.2.0b1",
     "types-pyyaml>=6.0.11",
     "typing-extensions>=4.5.0",
     "tenacity>=8.2.2",
+    "loguru>=0.7.0",
 ]
 requires-python = ">3.8.2,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
@@ -36,14 +36,16 @@
     "mkdocs>=1.0.0",
     "mkdocstrings[python]>=0.10.0",
     "mkdocs-cinder>=1.2.0",
     "pytest-rabbitmq>=2.2.1",
     "pudb>=2022.1.2",
     "types-retry>=0.9.9.3",
     "testcontainers[rabbitmq]>=3.7.1",
+    "autopep8>=1.6.0",
+    "bandit>=1.7.5",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
 [tool.pdm.scripts.publish-prod]
 cmd = "twine upload -r pypi dist/*"
```

### Comparing `robotnikmq-0.6.1/robotnikmq/config.py` & `robotnikmq-0.7.0/robotnikmq/config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/robotnikmq/core.py` & `robotnikmq-0.7.0/robotnikmq/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from contextlib import contextmanager
 from datetime import datetime
 from json import loads as _from_json
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from random import sample
-from ssl import SSLError
 from threading import current_thread
 from typing import Optional, Callable, Any, Dict, Union, Generator, List
 from uuid import uuid4 as uuid, UUID
 
 from arrow import Arrow, get as to_arrow, now
 from funcy import first
 from pika import BlockingConnection
@@ -21,14 +20,15 @@
     wait_random,
     Retrying,
 )
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig, config_of
 from robotnikmq.error import UnableToConnect, MalformedMessage
+from robotnikmq.log import log
 from robotnikmq.utils import to_json as _to_json
 
 AMQPErrorCallback = Optional[Callable[[AMQPError], None]]
 ConnErrorCallback = Optional[Callable[[AMQPConnectionError], None]]
 
 
 @contextmanager
@@ -121,43 +121,43 @@
 
 
 class Robotnik:
     @typechecked
     def __init__(
         self,
         config: Optional[RobotnikConfig] = None,
-        on_conn_error: ConnErrorCallback = None,
         config_paths: Optional[List[Path]] = None,
     ):
         config_paths = config_paths or [
             Path.cwd() / "robotnikmq.yaml",
             Path.home() / ".config" / "robotnikmq" / "robotnikmq.yaml",
             Path("/etc/robotnikmq/robotnikmq.yaml"),
         ]
         self.config = config or config_of(
             first(path for path in config_paths if path.exists())
         )
         self._connection = None
         self._channel: Optional[BlockingChannel] = None
-        self._on_conn_error = on_conn_error
+        self.log = log.bind(rmq_server="")
 
     @typechecked
     def _make_connection(self) -> BlockingConnection:
-        errors: Dict[str, str] = {}
+        self.log = log.bind(rmq_server="")
         for tier in self.config.tiers:
             for config in sample(tier, len(tier)):
                 try:
-                    return BlockingConnection(config.conn_params())
-                except (AMQPConnectionError, SSLError) as exc:
-                    errors[f"{config.user}@{config.host}:{config.port}"] = str(exc)
-                    if self._on_conn_error is not None:
-                        self._on_conn_error(exc)
-        raise UnableToConnect(
-            f"Cannot connect to any of the configured servers: {errors}"
-        )
+                    connection = BlockingConnection(config.conn_params())
+                    self.log = log.bind(rmq_server=f"{config.host}:{config.port}{config.vhost}")
+                    self.log.success("Connection to {}:{}{} is successful",
+                                     config.host, config.port, config.vhost)
+                    return connection
+                except AMQPConnectionError:
+                    log.exception("Unable to connect to {}:{}{}", config.host,
+                                  config.port, config.vhost)
+        raise UnableToConnect("Cannot connect to any of the configured servers")
 
     @property
     def connection(self) -> BlockingConnection:
         if self._connection is None or not self._connection.is_open:
             for attempt in Retrying(
                 retry=retry_if_exception_type((UnableToConnect, AMQPError, OSError)),
                 stop=stop_after_attempt(self.config.connection.attempts),
```

### Comparing `robotnikmq-0.6.1/robotnikmq/error.py` & `robotnikmq-0.7.0/robotnikmq/error.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/robotnikmq/rpc_client.py` & `robotnikmq-0.7.0/robotnikmq/rpc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from time import time
 from typing import Optional, Any, Dict, Union, List
 from uuid import uuid4 as uuid
 
 from pika import BasicProperties
 from typeguard import typechecked
 
-from robotnikmq.core import Robotnik, RobotnikConfig, ConnErrorCallback
+from robotnikmq.core import Robotnik, RobotnikConfig
 from robotnikmq.rpc_server import RpcError, RpcResponse
 from robotnikmq.utils import to_json
 
 
 class RpcClient(Robotnik):
     @typechecked
-    def __init__(self, config: Optional[RobotnikConfig] = None,
-                 on_conn_error: ConnErrorCallback = None):
-        super().__init__(config=config, on_conn_error=on_conn_error)
+    def __init__(self, config: Optional[RobotnikConfig] = None):
+        super().__init__(config=config)
         self.response: Optional[Any] = None
         self.callback_queue = None
         self.corr_id = str(uuid())
 
     @typechecked
     def _on_response(self, _, __, props: BasicProperties, body: bytes) -> None:
         self.response = body.decode() if self.corr_id == props.correlation_id else None
```

### Comparing `robotnikmq-0.6.1/robotnikmq/rpc_server.py` & `robotnikmq-0.7.0/robotnikmq/rpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from pika import BasicProperties
 from pika.exceptions import AMQPError, ChannelError, AMQPConnectionError
 from tenacity import retry, wait_exponential, retry_if_exception_type
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig
-from robotnikmq.core import Robotnik, ConnErrorCallback, thread_name, valid_json
-from robotnikmq.log import log
+from robotnikmq.core import Robotnik, thread_name, valid_json
 from robotnikmq.utils import to_json as _to_json
+from robotnikmq.log import log
 
 
 @typechecked
 def _type_hint_str(typ: Any) -> str:
     if get_origin(typ) is Union:
         return f"Union[{','.join([_type_hint_str(t) for t in get_args(typ)])}]"
     return str(typ.__name__)
@@ -82,30 +82,29 @@
 
     @staticmethod
     @typechecked
     def from_json(json_str: Union[str, bytes]) -> Optional["RpcResponse"]:
         json_str = json_str if isinstance(json_str, str) else json_str.decode()
         if valid_json(json_str):
             data = _from_json(json_str)
-            if all(k in data for k in {"request_id", "type", "data"}):
+            if all(k in data for k in ("request_id", "type", "data")):
                 return RpcResponse(request_id=data["request_id"], data=data["data"])
         return None
 
 
 class RpcServer(Robotnik):
     @typechecked
     def __init__(
         self,
         config: Optional[RobotnikConfig] = None,
-        on_conn_error: ConnErrorCallback = None,
         meta_queue_prefix: Optional[str] = None,
         docs_queue_suffix: Optional[str] = None,
         only_once: bool = False,
     ):
-        super().__init__(config=config, on_conn_error=on_conn_error)
+        super().__init__(config=config)
         self._callbacks: Dict[str, Callable] = {}
         self.meta_queue_prefix = meta_queue_prefix or gethostname()
         self.docs_queue_suffix = docs_queue_suffix or ".__doc__"
         # Typically used for testing, implies server should stop after 1 response
         self.only_once = only_once
 
     @typechecked
@@ -124,15 +123,15 @@
                     "inputs": self._get_input_type_strings(queue),
                     "returns": self._get_return_type_str(queue),
                     "description": callback.__doc__,
                 },
             )
             self.channel.basic_publish(
                 exchange="",
-                routing_key=props.reply_to,
+                routing_key=props.reply_to or "",
                 properties=BasicProperties(correlation_id=props.correlation_id),
                 body=response.to_json(),
             )
             self.channel.basic_ack(delivery_tag=method.delivery_tag)
 
         self.channel.basic_consume(
             queue=queue + self.docs_queue_suffix,
@@ -218,71 +217,71 @@
             self._register_docs(queue, callback)
         # TODO: servers should have an exclusive Queue for information about themselves
 
         @typechecked
         def meta_callback(_, method, props: BasicProperties, body: bytes):
             req_id = props.correlation_id or uuid()
             with thread_name(req_id):
-                log.debug("Request received")
+                self.log.debug("Request received")
                 try:
                     try:
                         if valid_json(body.decode()):
                             input_args: Dict[str, Any] = _from_json(body.decode())
-                            log.debug(f"Input JSON is valid: {input_args}")
+                            self.log.debug(f"Input JSON is valid: {input_args}")
                             valid_inputs, msg = self._valid_inputs(queue, input_args)
                             if not valid_inputs:
-                                log.debug("Invalid input")
+                                self.log.debug("Invalid input")
                                 response = RpcError(req_id, msg).to_json()
                             elif not input_args:
-                                log.debug(f"Executing: {callback}")
+                                self.log.debug(f"Executing: {callback}")
                                 response = RpcResponse(req_id, callback()).to_json()
                             else:
-                                log.debug(
+                                self.log.debug(
                                     f"Executing: {callback} with inputs: {input_args}"
                                 )
                                 response = RpcResponse(
                                     req_id, callback(**input_args)
                                 ).to_json()
                         else:
                             response = RpcError(
                                 req_id, "Input could not be decoded as JSON"
                             ).to_json()
                     except (AMQPError, ChannelError):
                         raise  # we want this kind of exception to be caught further down
                     except Exception:  # pylint: disable=W0703
-                        log.error(
+                        self.log.error(
                             "An error has occurred during the execution of the RPC method"
                         )
                         for line in format_exc().split("\n"):
-                            log.error(line)
+                            self.log.error(line)
                         response = RpcError(
                             request_id=req_id,
                             details=f"There was an error "
                             f"while processing the "
                             f"request, please refer "
                             f"to server log with "
                             f"request ID: "
                             f"{req_id}",
                         ).to_json()
-                    log.debug(f"Response: {response}")
+                    self.log.debug(f"Response: {response}")
                     self.channel.basic_publish(
                         exchange="",
-                        routing_key=props.reply_to,
+                        routing_key=props.reply_to or "",
                         properties=BasicProperties(correlation_id=props.correlation_id),
                         body=response,
                     )
                     self.channel.basic_ack(delivery_tag=method.delivery_tag)
-                    log.debug("Response sent and ack-ed")
+                    self.log.debug("Response sent and ack-ed")
                 except (AMQPError, ChannelError):
-                    log.error(
+                    self.log.error(
                         f"A RabbitMQ communication error has occurred while processing "
                         f"Request ID: {req_id}"
                     )
                     for line in format_exc().split("\n"):
-                        log.error(line)
+                        self.log.error(line)
             if self.only_once:
                 self.channel.stop_consuming()
 
         self.channel.basic_consume(
             queue=queue, on_message_callback=meta_callback, auto_ack=False
         )
 
@@ -292,8 +291,8 @@
     )
     @typechecked
     def run(self) -> None:
         try:
             self.channel.start_consuming()
         except KeyboardInterrupt:
             self.channel.stop_consuming()
-            log.info("Shutting down server")
+            self.log.info("Shutting down server")
```

### Comparing `robotnikmq-0.6.1/robotnikmq/topic.py` & `robotnikmq-0.7.0/robotnikmq/topic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import json
 from typing import Optional
 
 from pika.exceptions import AMQPError
+from pika.exchange_type import ExchangeType
 from tenacity import retry, retry_if_exception_type, wait_exponential
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig
-from robotnikmq.core import Robotnik, Message, ConnErrorCallback, AMQPErrorCallback
-from robotnikmq.log import log
+from robotnikmq.core import Robotnik, Message
 
 
 class Topic(Robotnik):
+    """The Topic is one of two key elements of the Publish/Subscribe workflow with RobotnikMQ.
+       Once configured, a topic is able to broadcast messages to any Subscribers on a given exchange
+       and routing key combination.
+    """
     @typechecked
     def __init__(
         self,
         exchange: str,
         config: Optional[RobotnikConfig] = None,
-        on_conn_error: ConnErrorCallback = None,
     ):
-        super().__init__(config=config, on_conn_error=on_conn_error)
+        super().__init__(config=config)
         self.exchange = exchange
         self.channel.exchange_declare(
-            exchange=self.exchange, exchange_type="topic", auto_delete=True
+            exchange=self.exchange, exchange_type=ExchangeType.topic, auto_delete=True
         )
 
     @retry(
         retry=retry_if_exception_type((AMQPError, OSError)),
         wait=wait_exponential(multiplier=1, min=3, max=30),
     )
     @typechecked
     def broadcast(
         self,
         msg: Message,
-        routing_key: Optional[str] = None,
-        on_msg_error: AMQPErrorCallback = None,
+        routing_key: Optional[str] = None
     ) -> None:
-        msg.routing_key = routing_key or msg.routing_key
+        """Broadcasts a message with an optional routing key.
+
+        Args:
+            msg (Message): The message to be broadcast.
+            routing_key (Optional[str], optional): Routing key used to broadcast the message.
+                                                   Defaults to an empty string.
+            on_msg_error (AMQPErrorCallback, optional): _description_. Defaults to None.
+        """
+        msg.routing_key = routing_key or msg.routing_key or ""
+        self.log.info("Broadcasting message (routing-key: [{}]):\n{}",
+                      msg.routing_key, json.dumps(msg.to_dict(), indent=4))
         self.channel.basic_publish(
             exchange=self.exchange,
-            routing_key=(routing_key or msg.routing_key or ""),
+            routing_key=msg.routing_key,
             body=json.dumps(msg.to_dict()),
         )
-        log.debug(f"Broadcast: \n{json.dumps(msg.to_dict(), indent=4)}")
+        self.log.success("Broadcast:\n{}", json.dumps(msg.to_dict(), indent=4))
```

### Comparing `robotnikmq-0.6.1/tests/integration/test_broadcast.py` & `robotnikmq-0.7.0/tests/integration/test_broadcast.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# pylint: disable=redefined-outer-name
 import json
 from multiprocessing import Process, Event
 from pprint import pprint
 from time import sleep
 
 from pytest import raises
 
+import robotnikmq
 from robotnikmq.config import server_config, RobotnikConfig, conn_config
 from robotnikmq.core import Message
 from robotnikmq.error import UnableToConnect
 from robotnikmq.log import log
 from robotnikmq.subscriber import Subscriber
 from robotnikmq.topic import Topic
 
@@ -21,42 +21,22 @@
 except ImportError:
     pass
 else:
     cleanup_on_sigterm()
 
 
 def test_basic_broadcast(robotnikmq_config):
-    topic = Topic(
-        META_QUEUE,
-        robotnikmq_config,
-        on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-    )
+    topic = Topic(META_QUEUE, robotnikmq_config)
     topic.broadcast(Message({"stuff": "Hello world!"}))
 
 
-def test_unable_to_connect():
-    config = RobotnikConfig(
-        connection=conn_config(1, 1, 2),
-        tiers=[
-            [
-                server_config("127.0.0.1", 1, "", "", ""),
-                server_config("127.0.0.2", 1, "1", "1", "1"),
-            ]
-        ],
-    )
-    with raises(UnableToConnect):
-        medium = Topic(
-            META_QUEUE,
-            config,
-            on_conn_error=lambda a: print(f"Could not connect (callback): {a.args}"),
-        )
-        medium.broadcast(Message({"stuff": "Hello world!"}))
+# TODO: Figure out how to turn testcontainer on and off to test failure modes and reconnecting
 
 
-def test_unable_to_connect_without_callback():
+def test_unable_to_connect():
     config = RobotnikConfig(
         connection=conn_config(1, 1, 2),
         tiers=[
             [
                 server_config("127.0.0.1", 1, "", "", ""),
                 server_config("127.0.0.2", 1, "1", "1", "1"),
             ]
@@ -79,15 +59,14 @@
             pprint(msg.to_dict())
             msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Hello world!"}))
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc = Process(target=pub)
@@ -95,34 +74,45 @@
     assert msg_received.wait(timeout=5)
     pub_proc.terminate()
     sub_proc.terminate()
     pub_proc.join()
     sub_proc.join()
 
 
+def test_subscriber_jitter(robotnikmq_config):
+    subscriber = Subscriber(config=robotnikmq_config).bind(exchange=META_QUEUE)
+    for _ in range(1000):
+        assert 5.0 <= subscriber._jitter(10, 5) <= 15  # pylint: disable=W0212
+
+
+def test_backoff_with_jitter(monkeypatch, robotnikmq_config):
+    with monkeypatch.context() as mock:
+        mock.setattr(robotnikmq.subscriber, 'sleep', lambda x: log.debug('sleep({})', x))
+        sub = Subscriber(config=robotnikmq_config).bind(exchange=META_QUEUE)
+        for _ in range(1000):
+            assert (10 + sub.TIMEOUT_STEP - sub.TIMEOUT_JITTER) <= \
+                   sub._backoff_with_jitter(10) \
+                   <= (10 + sub.TIMEOUT_STEP + sub.TIMEOUT_JITTER)  # pylint: disable=W0212
+
 def test_broadcast_malformed_message(robotnikmq_config):
     msg_received = Event()
 
     def sub():
         for msg in (
-            Subscriber(
-                config=robotnikmq_config,
-                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-            )
+            Subscriber(config=robotnikmq_config)
             .bind(exchange=META_QUEUE)
             .consume()
         ):
             pprint(msg.to_dict())
             msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.channel.basic_publish(
             exchange=META_QUEUE,
             routing_key="",
             body=json.dumps({"stuff": "Hello world!"}),
         )
@@ -140,53 +130,50 @@
 def test_subscriber_stop(robotnikmq_config):
     first_msg_received = Event()
     second_msg_received = Event()
 
     def sub():
         sub = Subscriber(
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         for msg in sub.bind(exchange=META_QUEUE).consume():
             pprint(msg.to_dict())
             if not first_msg_received.is_set():
                 first_msg_received.set()
                 break
             second_msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "first message"}))
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "second message"})
         )  # this message should not be received
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc = Process(target=pub)
     pub_proc.start()
     assert first_msg_received.wait(timeout=1)
     assert not second_msg_received.wait(timeout=1)
-    pub_proc.terminate()  # note that the subscriber should NOT need to be terminated after stop was called
+    pub_proc.terminate()  # note that the subscriber should NOT need to be terminated
     pub_proc.join()
     sub_proc.join()
 
 
 def test_basic_broadcast_consume(robotnikmq_config):
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Hello world!"}))
 
     pub_proc = Process(target=pub)
     pub_proc.start()
     stream = (
@@ -204,15 +191,14 @@
 
 
 def test_consume_malformed_message(robotnikmq_config):
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.channel.basic_publish(
             exchange=META_QUEUE, routing_key="", body=json.dumps({"stuff": "MALFORMED"})
         )
         medium.broadcast(Message({"stuff": "Hello world!"}))
 
@@ -231,53 +217,47 @@
 
 
 def test_multiple_broadcast_single_receive(robotnikmq_config):
     msg_received = Event()
 
     def sub():
         for msg in (
-            Subscriber(
-                config=robotnikmq_config,
-                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-            )
+            Subscriber(config=robotnikmq_config)
             .bind(exchange="stuff", binding_key="stuff.*")
             .consume()
         ):
             pprint(msg.to_dict())
             assert msg.contents["stuff"] != "Bad"
             assert msg.routing_key in {"stuff.something", "stuff.nothing"}
             msg_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (1)"}), routing_key="stuff.something"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (2)"}), routing_key="stuff.nothing"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
@@ -300,18 +280,15 @@
 def test_multiple_route_receive(robotnikmq_config):
     msg1_received = Event()
     msg2_received = Event()
     msg3_received = Event()
 
     def sub():
         for msg in (
-            Subscriber(
-                config=robotnikmq_config,
-                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-            )
+            Subscriber(config=robotnikmq_config)
             .bind("stuff", "message.1")
             .bind("stuff", "message.2")
             .bind("stuff", "message.3")
             .consume()
         ):
             pprint(msg.to_dict())
             assert msg.contents["stuff"] != "Bad"
@@ -322,48 +299,44 @@
             if msg.route == "message.3":
                 msg3_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (1)"}), routing_key="message.1"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (2)"}), routing_key="message.2"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (3)"}), routing_key="message.3"
         )
 
     def pub_bad():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
@@ -392,18 +365,15 @@
 def test_multiple_queue_receive(robotnikmq_config):
     msg1_received = Event()
     msg2_received = Event()
     msg3_received = Event()
 
     def sub():
         for msg in (
-            Subscriber(
-                config=robotnikmq_config,
-                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-            )
+            Subscriber(config=robotnikmq_config)
             .bind("stuff.1", "message.1")
             .bind("stuff.2", "message.2")
             .bind("stuff.3", "message.3")
             .consume()
         ):
             pprint(msg.to_dict())
             assert msg.contents["stuff"] != "Bad"
@@ -414,48 +384,44 @@
             if msg.route == "message.3":
                 msg3_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff.1",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (1)"}), routing_key="message.1"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.2",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (2)"}), routing_key="message.2"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.3",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (3)"}), routing_key="message.3"
         )
 
     def pub_bad():
         medium = Topic(
             exchange="stuff.1",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
@@ -482,53 +448,47 @@
 
 
 def test_multiple_broadcast_single_receive_msg_routing(robotnikmq_config):
     msg_received = Event()
 
     def sub():
         for msg in (
-            Subscriber(
-                config=robotnikmq_config,
-                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-            )
+            Subscriber(config=robotnikmq_config)
             .bind(exchange="stuff", binding_key="stuff.*")
             .consume()
         ):
             pprint(msg.to_dict())
             assert msg.contents["stuff"] != "Bad"
             assert msg.routing_key in {"stuff.something", "stuff.nothing"}
             msg_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (1)"}, routing_key="stuff.something")
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(
             Message({"stuff": "Hello world! (2)"}, routing_key="stuff.nothing")
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
         sleep(0.2)
         medium.broadcast(Message({"stuff": "Bad"}, routing_key="bad.stuff.nothing"))
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
```

### Comparing `robotnikmq-0.6.1/tests/integration/test_rpc.py` & `robotnikmq-0.7.0/tests/integration/test_rpc.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/tests/integration/utils.py` & `robotnikmq-0.7.0/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/tests/unit/test_config.py` & `robotnikmq-0.7.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/tests/unit/test_message.py` & `robotnikmq-0.7.0/tests/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/tests/unit/test_validation.py` & `robotnikmq-0.7.0/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.6.1/PKG-INFO` & `robotnikmq-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotnikmq
-Version: 0.6.1
+Version: 0.7.0
 Summary: Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >3.8.2,<4.0
 Description-Content-Type: text/markdown
 
 # RobotnikMQ
@@ -92,14 +92,22 @@
 
 **Sublime Text 3**
 
 ```bash
 curl -sSL https://gitlab.com/-/snippets/2385805/raw/main/pdm.sublime-project.py | pdm run python > robotnikmq.sublime-project
 ```
 
+**VSCodium/VSCode**
+
+I recommend installing the [pdm-vscode](https://github.com/frostming/pdm-vscode) plug-in:
+
+```bash
+sudo pdm plugin add pdm-vscode
+```
+
 ## Testing
 
 All testing should be done with `pytest` which is installed with the `dev` requirements.
 
 To run all the unit tests, execute the following from the repo directory:
 
 ```bash
```

