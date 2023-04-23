# Comparing `tmp/yolink-api-0.2.8.tar.gz` & `tmp/yolink-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolink-api-0.2.8.tar", last modified: Tue Jan 31 13:02:55 2023, max compression
+gzip compressed data, was "yolink-api-0.2.9.tar", last modified: Sun Apr 23 07:05:46 2023, max compression
```

## Comparing `yolink-api-0.2.8.tar` & `yolink-api-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:02:55.607196 yolink-api-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-31 13:02:52.000000 yolink-api-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-31 13:02:55.607196 yolink-api-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-31 13:02:52.000000 yolink-api-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-31 13:02:52.000000 yolink-api-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 13:02:55.607196 yolink-api-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-31 13:02:52.000000 yolink-api-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:02:55.607196 yolink-api-0.2.8/yolink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/auth_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/client_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/home_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/message_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/message_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/outlet_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-31 13:02:52.000000 yolink-api-0.2.8/yolink/thermostat_request_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:02:55.607196 yolink-api-0.2.8/yolink_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-31 13:02:55.000000 yolink-api-0.2.8/yolink_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 07:05:40.000000 yolink-api-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 07:05:46.460615 yolink-api-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-23 07:05:40.000000 yolink-api-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 07:05:40.000000 yolink-api-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:05:46.460615 yolink-api-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-23 07:05:40.000000 yolink-api-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/yolink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/home_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/message_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/outlet_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/thermostat_request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/yolink_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/top_level.txt
```

### Comparing `yolink-api-0.2.8/LICENSE` & `yolink-api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/setup.py` & `yolink-api-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="yolink-api",
-    version="0.2.8",
+    version="0.2.9",
     author="YoSmart",
     description="A library to authenticate with yolink device",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YoSmart-Inc/yolink-api",
     project_urls={
         "Bug Tracker": "https://github.com/YoSmart-Inc/yolink-api/issues",
```

### Comparing `yolink-api-0.2.8/yolink/auth_mgr.py` & `yolink-api-0.2.9/yolink/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/client.py` & `yolink-api-0.2.9/yolink/client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/const.py` & `yolink-api-0.2.9/yolink/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,7 +25,10 @@
 ATTR_DEVICE_MANIPULATOR = "Manipulator"
 ATTR_DEVICE_CO_SMOKE_SENSOR = "COSmokeSensor"
 ATTR_DEVICE_SWITCH = "Switch"
 ATTR_DEVICE_THERMOSTAT = "Thermostat"
 ATTR_DEVICE_DIMMER = "Dimmer"
 ATTR_GARAGE_DOOR_CONTROLLER = "GarageDoor"
 ATTR_DEVICE_SMART_REMOTER = "SmartRemoter"
+ATTR_DEVICE_POWER_FAILURE_ALARM = "PowerFailureAlarm"
+ATTR_DEVICE_HUB = "Hub"
+ATTR_DEVICE_SPEAKER_HUB = "SpeakerHub"
```

### Comparing `yolink-api-0.2.8/yolink/device.py` & `yolink-api-0.2.9/yolink/device.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/home_manager.py` & `yolink-api-0.2.9/yolink/home_manager.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/model.py` & `yolink-api-0.2.9/yolink/model.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/mqtt_client.py` & `yolink-api-0.2.9/yolink/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/outlet_request_builder.py` & `yolink-api-0.2.9/yolink/outlet_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink/thermostat_request_builder.py` & `yolink-api-0.2.9/yolink/thermostat_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.8/yolink_api.egg-info/SOURCES.txt` & `yolink-api-0.2.9/yolink_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

