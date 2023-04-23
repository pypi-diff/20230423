# Comparing `tmp/legion-utils-0.2.9.tar.gz` & `tmp/legion-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-utils-0.2.9.tar", max compression
+gzip compressed data, was "legion-utils-0.3.0.tar", last modified: Sun Apr 23 03:35:41 2023, max compression
```

## Comparing `legion-utils-0.2.9.tar` & `legion-utils-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0    34500 2021-07-04 19:28:00.000000 legion-utils-0.2.9/LICENSE
--rw-r--r--   0        0        0     2573 2021-07-04 19:28:00.000000 legion-utils-0.2.9/README.md
--rw-r--r--   0        0        0      671 2021-09-01 15:13:35.284697 legion-utils-0.2.9/legion_utils/__init__.py
--rw-r--r--   0        0        0    12427 2021-09-01 15:13:35.284697 legion-utils-0.2.9/legion_utils/core.py
--rw-r--r--   0        0        0     1054 2022-01-17 17:10:47.572775 legion-utils-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3372 2022-01-17 17:14:46.313467 legion-utils-0.2.9/setup.py
--rw-r--r--   0        0        0     3582 2022-01-17 17:14:46.313776 legion-utils-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:58.357856 legion-utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2573 2022-11-16 02:41:58.357856 legion-utils-0.3.0/README.md
+-rw-r--r--   0        0        0      671 2022-11-16 02:41:58.357856 legion-utils-0.3.0/legion_utils/__init__.py
+-rw-r--r--   0        0        0    12649 2023-04-10 23:53:37.883526 legion-utils-0.3.0/legion_utils/core.py
+-rw-r--r--   0        0        0      893 2023-04-23 03:31:02.035016 legion-utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-17 01:19:20.049718 legion-utils-0.3.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5565 2023-04-17 01:27:37.589477 legion-utils-0.3.0/tests/integration/test_alert.py
+-rw-r--r--   0        0        0     2104 2023-04-17 01:25:04.130604 legion-utils-0.3.0/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    18292 2023-04-17 01:01:57.259012 legion-utils-0.3.0/tests/unit/test_alert_data.py
+-rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 legion-utils-0.3.0/PKG-INFO
```

### Comparing `legion-utils-0.2.9/LICENSE` & `legion-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.9/README.md` & `legion-utils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.9/legion_utils/__init__.py` & `legion-utils-0.3.0/legion_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.9/legion_utils/core.py` & `legion-utils-0.3.0/legion_utils/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     INFO = 0
     ACTIVITY = 1
     WARNING = 2
     ERROR = 3
     CRITICAL = 4
 
 
-INFO = {'info', 'information', 'i'}
-ACTIVITY = {'activity', 'a'}
-WARNING = {'warning', 'warn', 'w'}
-ERROR = {'error', 'err', 'e'}
-CRITICAL = {'critical', 'crit', 'c'}
+INFO = {"info", "information", "i"}
+ACTIVITY = {"activity", "a"}
+WARNING = {"warning", "warn", "w"}
+ERROR = {"error", "err", "e"}
+CRITICAL = {"critical", "crit", "c"}
 
 
 @typechecked
 def valid_priority(candidate: Any) -> bool:
     if isinstance(candidate, Priority):
         return True
     if isinstance(candidate, str):
-        return any(candidate.lower() in P for P in [INFO, ACTIVITY, WARNING, ERROR, CRITICAL])
+        return any(
+            candidate.lower() in P for P in [INFO, ACTIVITY, WARNING, ERROR, CRITICAL]
+        )
     if isinstance(candidate, int):
         return any(candidate == i for i in Priority)
     return False
 
 
 @typechecked
 def priority_of(candidate: Union[str, int]) -> Priority:
@@ -50,50 +52,54 @@
     if isinstance(candidate, int):
         return Priority(candidate)
     raise ValueError(f'"{candidate}" cannot be mapped to a valid priority')
 
 
 class NotificationMsg:
     @typechecked
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 alert_key: Union[str, List[str], None] = None,
-                 desc: Optional[str] = None,
-                 ttl: Optional[int] = None,
-                 priority: Optional[Priority] = None):
+    def __init__(
+        self,
+        contents: Dict[str, Any],
+        alert_key: Union[str, List[str], None] = None,
+        desc: Optional[str] = None,
+        ttl: Optional[int] = None,
+        priority: Optional[Priority] = None,
+    ):
         self.contents = contents
-        self.alert_key = '['+']['.join(alert_key)+']' if isinstance(alert_key, List) else alert_key
+        self.alert_key = (
+            "[" + "][".join(alert_key) + "]"
+            if isinstance(alert_key, List)
+            else alert_key
+        )
         self.desc = desc
         self.ttl = ttl
         self.priority = priority or Priority.INFO
 
     @typechecked
-    def broadcast(self, exchange: str, route: str, config: Optional[RobotnikConfig] = None) -> None:
+    def broadcast(
+        self, exchange: str, route: str, config: Optional[RobotnikConfig] = None
+    ) -> None:
         broadcast_msg(exchange, route, self, config)
 
 
 @typechecked
 class InfoMsg(NotificationMsg):
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 ttl: Optional[int] = None):
+    def __init__(self, contents: Dict[str, Any], ttl: Optional[int] = None):
         super().__init__(contents=contents, ttl=ttl, priority=Priority.INFO)
 
 
 @typechecked
 class ActivityMsg(NotificationMsg):
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 ttl: Optional[int] = None):
+    def __init__(self, contents: Dict[str, Any], ttl: Optional[int] = None):
         super().__init__(contents=contents, ttl=ttl, priority=Priority.ACTIVITY)
 
 
 class AlertComparison:
     @typechecked
-    def __init__(self, first: 'AlertMsg', second: 'AlertMsg'):
+    def __init__(self, first: "AlertMsg", second: "AlertMsg"):
         self.key = first.key, second.key
         self.desc = first.desc, second.desc
         self.ttl = first.ttl, second.ttl
         self.priority = first.priority, second.priority
         self.contents = first.contents, second.contents
 
     @property
@@ -117,207 +123,334 @@
         return bool(match(*self.key) or match(self.key[1], self.key[0]))
 
     @property
     def desc_match(self) -> bool:
         return bool(match(*self.desc) or match(self.desc[1], self.desc[0]))
 
 
-@typechecked
 class AlertMsg(NotificationMsg):
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 key: Union[str, List[str]],
-                 desc: str,
-                 ttl: Optional[int] = None,
-                 priority: Optional[Priority] = None,
-                 from_msg: Optional[Message] = None):
+    @typechecked
+    def __init__(
+        self,
+        contents: Dict[str, Any],
+        key: Union[str, List[str]],
+        desc: str,
+        ttl: Optional[int] = None,
+        priority: Optional[Priority] = None,
+        from_msg: Optional[Message] = None,
+    ):
         if priority is not None and priority < Priority.WARNING:
-            raise ValueError('Alerts can only have a priority of WARNING (2) or higher')
+            raise ValueError("Alerts can only have a priority of WARNING (2) or higher")
         if not desc:
-            raise ValueError('Alerts have to have a description')
+            raise ValueError("Alerts have to have a description")
         if not key:
-            raise ValueError('Alerts have to have a key')
-        super().__init__(desc=desc, priority=priority or Priority.WARNING,
-                         ttl=ttl or 30, contents=contents)
-        self.alert_key: str = '['+']['.join(key)+']' if isinstance(key, List) else key
+            raise ValueError("Alerts have to have a key")
+        super().__init__(
+            desc=desc,
+            priority=priority or Priority.WARNING,
+            ttl=ttl or 30,
+            contents=contents,
+        )
+        self.alert_key: str = (
+            "[" + "][".join(key) + "]" if isinstance(key, List) else key
+        )
         self.msg = from_msg
 
-    def compare(self, other: 'AlertMsg') -> AlertComparison:
+    @typechecked
+    def compare(self, other: "AlertMsg") -> AlertComparison:
         return AlertComparison(self, other)
 
     @property
     def key(self) -> str:
         return self.alert_key
 
     @property
     def description(self) -> Optional[str]:
         return self.desc
 
     @staticmethod
-    def of(msg: Message) -> 'AlertMsg':  # pylint: disable=C0103
-        if 'ttl' not in msg.contents:
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have a TTL: {pformat(msg.to_dict())}')
-        if 'priority' not in msg.contents:
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have a priority: {pformat(msg.to_dict())}')
-        if not valid_priority(msg.contents['priority']):
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have a valid priority: {pformat(msg.to_dict())}')
-        if not isinstance(msg.contents['ttl'], int) or msg.contents['ttl'] < 0:
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have a valid TTL: {pformat(msg.to_dict())}')
-        if 'alert_key' not in msg.contents:
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have an alert key: {pformat(msg.to_dict())}')
-        if 'description' not in msg.contents:
-            raise ValueError(f'Message id {msg.msg_id} cannot be interpreted as an alert '
-                             f'as it does not have a description: {pformat(msg.to_dict())}')
-        return AlertMsg(msg.contents, key=msg.contents['alert_key'],
-                        desc=msg.contents['description'], ttl=msg.contents['ttl'],
-                        priority=priority_of(msg.contents['priority']), from_msg=msg)
+    def of(msg: Message) -> "AlertMsg":  # pylint: disable=C0103
+        if "ttl" not in msg.contents:
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have a TTL: {pformat(msg.to_dict())}"
+            )
+        if "priority" not in msg.contents:
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have a priority: {pformat(msg.to_dict())}"
+            )
+        if not valid_priority(msg.contents["priority"]):
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have a valid priority: {pformat(msg.to_dict())}"
+            )
+        if not isinstance(msg.contents["ttl"], int) or msg.contents["ttl"] < 0:
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have a valid TTL: {pformat(msg.to_dict())}"
+            )
+        if "alert_key" not in msg.contents:
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have an alert key: {pformat(msg.to_dict())}"
+            )
+        if "description" not in msg.contents:
+            raise ValueError(
+                f"Message id {msg.msg_id} cannot be interpreted as an alert "
+                f"as it does not have a description: {pformat(msg.to_dict())}"
+            )
+        return AlertMsg(
+            msg.contents,
+            key=msg.contents["alert_key"],
+            desc=msg.contents["description"],
+            ttl=msg.contents["ttl"],
+            priority=priority_of(msg.contents["priority"]),
+            from_msg=msg,
+        )
 
 
 class WarningMsg(AlertMsg):
     @typechecked
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 key: Union[str, List[str]],
-                 desc: str,
-                 ttl: Optional[int] = None):
+    def __init__(
+        self,
+        contents: Dict[str, Any],
+        key: Union[str, List[str]],
+        desc: str,
+        ttl: Optional[int] = None,
+    ):
         if not desc:
-            raise ValueError('Warnings (alerts) have to have a description')
+            raise ValueError("Warnings (alerts) have to have a description")
         if not key:
-            raise ValueError('Warnings (alerts) have to have a key')
-        super().__init__(key=key, desc=desc, priority=Priority.WARNING,
-                         ttl=ttl or 30, contents=contents)
+            raise ValueError("Warnings (alerts) have to have a key")
+        super().__init__(
+            key=key,
+            desc=desc,
+            priority=Priority.WARNING,
+            ttl=ttl or 30,
+            contents=contents,
+        )
 
 
 class ErrorMsg(AlertMsg):
     @typechecked
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 key: Union[str, List[str]],
-                 desc: str,
-                 ttl: Optional[int] = None):
+    def __init__(
+        self,
+        contents: Dict[str, Any],
+        key: Union[str, List[str]],
+        desc: str,
+        ttl: Optional[int] = None,
+    ):
         if not desc:
-            raise ValueError('Errors (alerts) have to have a description')
+            raise ValueError("Errors (alerts) have to have a description")
         if not key:
-            raise ValueError('Errors (alerts) have to have a key')
-        super().__init__(key=key, desc=desc, priority=Priority.ERROR,
-                         ttl=ttl or 30, contents=contents)
+            raise ValueError("Errors (alerts) have to have a key")
+        super().__init__(
+            key=key,
+            desc=desc,
+            priority=Priority.ERROR,
+            ttl=ttl or 30,
+            contents=contents,
+        )
 
 
 class CriticalMsg(AlertMsg):
     @typechecked
-    def __init__(self,
-                 contents: Dict[str, Any],
-                 key: Union[str, List[str]],
-                 desc: str,
-                 ttl: Optional[int] = None):
+    def __init__(
+        self,
+        contents: Dict[str, Any],
+        key: Union[str, List[str]],
+        desc: str,
+        ttl: Optional[int] = None,
+    ):
         if not desc:
-            raise ValueError('Critical Alerts have to have a description')
+            raise ValueError("Critical Alerts have to have a description")
         if not key:
-            raise ValueError('Critical Alerts have to have a key')
-        super().__init__(key=key, desc=desc, priority=Priority.CRITICAL,
-                         ttl=ttl or 30, contents=contents)
+            raise ValueError("Critical Alerts have to have a key")
+        super().__init__(
+            key=key,
+            desc=desc,
+            priority=Priority.CRITICAL,
+            ttl=ttl or 30,
+            contents=contents,
+        )
 
 
 @typechecked
-def broadcast_msg(exchange: str, route: str, notification: NotificationMsg,
-                  config: Optional[RobotnikConfig] = None) -> None:
-    broadcast(exchange=exchange,
-              route=route,
-              priority=notification.priority,
-              contents=notification.contents,
-              ttl=notification.ttl,
-              description=notification.desc,
-              alert_key=notification.alert_key,
-              config=config)
+def broadcast_msg(
+    exchange: str,
+    route: str,
+    notification: NotificationMsg,
+    config: Optional[RobotnikConfig] = None,
+) -> None:
+    broadcast(
+        exchange=exchange,
+        route=route,
+        priority=notification.priority,
+        contents=notification.contents,
+        ttl=notification.ttl,
+        description=notification.desc,
+        alert_key=notification.alert_key,
+        config=config,
+    )
 
 
 @typechecked
-def broadcast_alert_msg(exchange: str, route: str, alert: AlertMsg,
-                        config: Optional[RobotnikConfig] = None) -> None:
-    broadcast(exchange=exchange,
-              route=route,
-              priority=alert.priority,
-              contents=alert.contents,
-              ttl=alert.ttl,
-              description=alert.desc,
-              alert_key=alert.alert_key,
-              config=config)
+def broadcast_alert_msg(
+    exchange: str, route: str, alert: AlertMsg, config: Optional[RobotnikConfig] = None
+) -> None:
+    broadcast(
+        exchange=exchange,
+        route=route,
+        priority=alert.priority,
+        contents=alert.contents,
+        ttl=alert.ttl,
+        description=alert.desc,
+        alert_key=alert.alert_key,
+        config=config,
+    )
 
 
 @typechecked
-def broadcast(exchange: str,
-              route: str,
-              priority: Priority,
-              contents: Dict[str, Any],
-              ttl: Optional[int] = None,
-              description: Optional[str] = None,
-              alert_key: Optional[str] = None,
-              config: Optional[RobotnikConfig] = None):
-    _contents: Dict[str, Any] = {'priority': priority.value}
+def broadcast(
+    exchange: str,
+    route: str,
+    priority: Priority,
+    contents: Dict[str, Any],
+    ttl: Optional[int] = None,
+    description: Optional[str] = None,
+    alert_key: Optional[str] = None,
+    config: Optional[RobotnikConfig] = None,
+):
+    _contents: Dict[str, Any] = {"priority": priority.value}
     if priority.value >= 2:
-        assert description is not None, 'Alerts (e.g. WARNING, ERROR, CRITICAL) must have a description'
-        assert ttl is not None, 'Alerts (e.g. WARNING, ERROR, CRITICAL) must have a ttl (to clear an alert, set the ttl to 0)'
-        assert alert_key is not None, 'Alerts (e.g. WARNING, ERROR, CRITICAL) must have an alert_key'
+        assert (
+            description is not None
+        ), "Alerts (e.g. WARNING, ERROR, CRITICAL) must have a description"
+        assert (
+            ttl is not None
+        ), "Alerts (e.g. WARNING, ERROR, CRITICAL) must have a ttl (to clear an alert, set the ttl to 0)"
+        assert (
+            alert_key is not None
+        ), "Alerts (e.g. WARNING, ERROR, CRITICAL) must have an alert_key"
     if ttl is not None:
-        _contents['ttl'] = ttl
+        _contents["ttl"] = ttl
     if description is not None:
-        _contents['description'] = description
+        _contents["description"] = description
     if alert_key is not None:
-        _contents['alert_key'] = alert_key
+        _contents["alert_key"] = alert_key
     _contents.update(contents)
-    route += f'.{priority.name.lower()}'
-    Topic(exchange=exchange, config=config).broadcast(Message(contents=_contents),
-                                                      routing_key=route)
+    route += f".{priority.name.lower()}"
+    Topic(exchange=exchange, config=config).broadcast(
+        Message(contents=_contents), routing_key=route
+    )
 
 
 @typechecked
-def broadcast_info(exchange: str, route: str, contents: Dict[str, Any],
-                   config: Optional[RobotnikConfig] = None):
+def broadcast_info(
+    exchange: str,
+    route: str,
+    contents: Dict[str, Any],
+    config: Optional[RobotnikConfig] = None,
+):
     broadcast(exchange, route, priority=Priority.INFO, contents=contents, config=config)
 
 
 @typechecked
-def broadcast_activity(exchange: str, route: str, contents: Dict[str, Any],
-                       config: Optional[RobotnikConfig] = None):
-    broadcast(exchange, route, priority=Priority.ACTIVITY, contents=contents, config=config)
-
-
-@typechecked
-def broadcast_alert(exchange: str,
-                    route: str,
-                    description: str,
-                    alert_key: str,
-                    contents: Dict[str, Any],
-                    ttl: int = 30,
-                    priority: Priority = Priority.WARNING,
-                    config: Optional[RobotnikConfig] = None) -> None:
-    broadcast(exchange, route, ttl=ttl, priority=priority, contents=contents,
-              config=config, description=description, alert_key=alert_key)
-
-
-@typechecked
-def broadcast_warning(exchange: str, route: str, desc: str, alert_key: str,
-                      contents: Dict[str, Any], ttl: int = 30,
-                      config: Optional[RobotnikConfig] = None):
-    broadcast_alert(exchange, route, description=desc, alert_key=alert_key, contents=contents,
-                    ttl=ttl, priority=Priority.WARNING, config=config)
-
-
-@typechecked
-def broadcast_error(exchange: str, route: str, desc: str, alert_key: str,
-                    contents: Dict[str, Any], ttl: int = 30,
-                    config: Optional[RobotnikConfig] = None):
-    broadcast_alert(exchange, route, description=desc, alert_key=alert_key, contents=contents,
-                    ttl=ttl, priority=Priority.ERROR, config=config)
-
-
-@typechecked
-def broadcast_critical(exchange: str, route: str, desc: str, alert_key: str,
-                       contents: Dict[str, Any], ttl: int = 30,
-                       config: Optional[RobotnikConfig] = None):
-    broadcast_alert(exchange, route, description=desc, alert_key=alert_key, contents=contents,
-                    ttl=ttl, priority=Priority.CRITICAL, config=config)
+def broadcast_activity(
+    exchange: str,
+    route: str,
+    contents: Dict[str, Any],
+    config: Optional[RobotnikConfig] = None,
+):
+    broadcast(
+        exchange, route, priority=Priority.ACTIVITY, contents=contents, config=config
+    )
+
+
+@typechecked
+def broadcast_alert(
+    exchange: str,
+    route: str,
+    description: str,
+    alert_key: str,
+    contents: Dict[str, Any],
+    ttl: int = 30,
+    priority: Priority = Priority.WARNING,
+    config: Optional[RobotnikConfig] = None,
+) -> None:
+    broadcast(
+        exchange,
+        route,
+        ttl=ttl,
+        priority=priority,
+        contents=contents,
+        config=config,
+        description=description,
+        alert_key=alert_key,
+    )
+
+
+@typechecked
+def broadcast_warning(
+    exchange: str,
+    route: str,
+    desc: str,
+    alert_key: str,
+    contents: Dict[str, Any],
+    ttl: int = 30,
+    config: Optional[RobotnikConfig] = None,
+):
+    broadcast_alert(
+        exchange,
+        route,
+        description=desc,
+        alert_key=alert_key,
+        contents=contents,
+        ttl=ttl,
+        priority=Priority.WARNING,
+        config=config,
+    )
+
+
+@typechecked
+def broadcast_error(
+    exchange: str,
+    route: str,
+    desc: str,
+    alert_key: str,
+    contents: Dict[str, Any],
+    ttl: int = 30,
+    config: Optional[RobotnikConfig] = None,
+):
+    broadcast_alert(
+        exchange,
+        route,
+        description=desc,
+        alert_key=alert_key,
+        contents=contents,
+        ttl=ttl,
+        priority=Priority.ERROR,
+        config=config,
+    )
+
+
+@typechecked
+def broadcast_critical(
+    exchange: str,
+    route: str,
+    desc: str,
+    alert_key: str,
+    contents: Dict[str, Any],
+    ttl: int = 30,
+    config: Optional[RobotnikConfig] = None,
+):
+    broadcast_alert(
+        exchange,
+        route,
+        description=desc,
+        alert_key=alert_key,
+        contents=contents,
+        ttl=ttl,
+        priority=Priority.CRITICAL,
+        config=config,
+    )
```

### Comparing `legion-utils-0.2.9/PKG-INFO` & `legion-utils-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 Metadata-Version: 2.1
 Name: legion-utils
-Version: 0.2.9
+Version: 0.3.0
 Summary: Utilities for Legion Reporters and Monitors
-Home-page: https://gitlab.com/legion-robotnik/legion-utils
-License: GPL-3.0-only
-Author: Eugene Kovalev
-Author-email: eugene@kovalev.systems
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: robotnikmq (>=0.3.3,<0.4.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0)
-Project-URL: Documentation, https://gitlab.com/legion-robotnik/legion-utils
-Project-URL: Repository, https://gitlab.com/legion-robotnik/legion-utils
+License: GPL-3.0-or-later
+Author-email: Eugene Kovalev <eugene@kovalev.systems>
+Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Legion Utils
 
 Utilities for Legion Reporters and Monitors
 
 ## Usage
```

