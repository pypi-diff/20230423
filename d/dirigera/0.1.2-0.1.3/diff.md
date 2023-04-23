# Comparing `tmp/dirigera-0.1.2.tar.gz` & `tmp/dirigera-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.2.tar", last modified: Fri Apr 21 14:19:17 2023, max compression
+gzip compressed data, was "dirigera-0.1.3.tar", last modified: Sun Apr 23 09:34:51 2023, max compression
```

## Comparing `dirigera-0.1.2.tar` & `dirigera-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-21 14:19:07.000000 dirigera-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:17.053646 dirigera-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-21 14:19:07.000000 dirigera-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 14:19:07.000000 dirigera-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:19:17.057646 dirigera-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:19:07.000000 dirigera-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-21 14:19:07.000000 dirigera-0.1.2/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-21 14:19:07.000000 dirigera-0.1.2/tests/test_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 09:34:39.000000 dirigera-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-23 09:34:51.228526 dirigera-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-23 09:34:39.000000 dirigera-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-23 09:34:39.000000 dirigera-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:34:51.228526 dirigera-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:34:39.000000 dirigera-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.224526 dirigera-0.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.224526 dirigera-0.1.3/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-23 09:34:39.000000 dirigera-0.1.3/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-23 09:34:39.000000 dirigera-0.1.3/tests/test_light.py
```

### Comparing `dirigera-0.1.2/LICENSE` & `dirigera-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/PKG-INFO` & `dirigera-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,19 @@
-Metadata-Version: 2.1
-Name: dirigera
-Version: 0.1.2
-Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
-Author-email: Leggin <legginsun@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Leggin
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Leggin/dirigera
-Keywords: python,iot,smarthome,hub,lighting,ikea,tradfri,dirigera
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+# Dirigera Python Client
+![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
+![Pypi](https://img.shields.io/pypi/v/dirigera)
+[![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 
-# Dirigera Python client
 
-This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Currently, only light control is supported, but support for other features will be added in the future.
+This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
+ - [light control](#controlling-lights)
+ - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
+ - [event listener](#event-listener) for hub events
+
+Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
 pip install dirigera
 ```
 
@@ -57,17 +29,17 @@
    ```
     Press the action button on Dirigera then hit ENTER ...
     Your Token:
     mgwB.aXqwpzV89N0aUwBhZMJjD8a.UBPyzy2InGtqgwo2MO5.xX4ug7.uBcVJquwYzLnAijF7SdYKvNxTo0uzQKahV10A-3ZQOz-UAubGP6sHWt1CJx3QmWZyE7ZcMZKgODXjSzWL1lumKgGz5dUIwFi3rhNxgK-IsBGeGVhNXPt8vGrYEcZePwPvNAIg8RqmlH27L-JZPnkAtP2wHoOdW72Djot3yJsohtEsb0p9mJvoZFSavTlTr4LDuf584vuH5fha5xoR9QhhIvvgbAP-s4EHFqENNi6vrYLHKR.sdqnv4sYw6UH-l6oiPnnRLxinoqBPOlWhlcL9doFviXQE.tZ9X8WVqyBrd0NYHlo9iorEvUbnZuD02BEJrg4NLwgh3rZtyF0Mi46HenynzBohbPn4RnuSYYCiHt5EZnWedxBtDqc7mSTm1ZtyD
    ```
 6. Done
 
-## Dirigera Hub
+## [Dirigera Hub](./src/dirigera/hub/hub.py)
 
-Setting up the client works by providing the token and ip address that is read from your .env file by the `config.py`
+Setting up the client works by providing the token and ip address.
 
 ```python
 import dirigera
 
 dirigera_hub = dirigera.Hub(
     token="mgwB.aXqwpzV89N0aUwBhZMJjD8a...",
     ip_address="192.1..."
@@ -81,51 +53,79 @@
 ```python
 lights = dirigera_hub.get_lights()
 ```
 
 The light object has the following attributes:
 
 ```python
-    device_id: str
-    is_reachable: bool
-    custom_name: str
-    is_on: bool
-    startup_on_off: StartupEnum | None
-    light_level: int | None  # not all lights have a light level
-    color_temp: int | None  # not all lights have a color temperature
-    color_temp_min: int | None
-    color_temp_max: int | None
-    color_hue: int | None  # not all lights have a color hue
-    color_saturation: float | None  # not all lights have a color saturation
-    room_id: str
-    room_name: str
-    can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+startup_on_off: StartupEnum | None
+light_level: int | None  # not all lights have a light level
+color_temp: int | None  # not all lights have a color temperature
+color_temp_min: int | None
+color_temp_max: int | None
+color_hue: int | None  # not all lights have a color hue
+color_saturation: float | None  # not all lights have a color saturation
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
 ```
 
 Available methods for light are:
 
 ```python
-    light.set_name(name="kitchen light 1")
+light.set_name(name="kitchen light 1")
+
+light.set_light(lamp_on=True)
+
+light.set_light_level(light_level=90)
+
+light.set_color_temperature(color_temp=3000)
+
+light.set_light_color(hue=128, saturation=0.5)
 
-    light.set_light(lamp_on=True)
+light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+```
 
-    light.set_light_level(light_level=90)
+## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
+Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
-    light.set_color_temperature(color_temp=3000)
 
-    light.set_light_color(hue=128, saturation=0.5)
+To get the environment sensors use:
+```python
+sensors = dirigera_hub.get_environment_sensors()
+```
 
-    light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+The environment sensor object has the following attributes:
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+current_temperature: str
+current_rh: int  # current humidity
+current_pm25: int  # current particulate matter 2.5
+max_measured_pm25: int  # maximum measurable particulate matter 2.5
+min_measured_pm25: int  # minimum measurable particulate matter 2.5
+voc_index: int  # current volatile organic compound
+room_id: str
+room_name: str
+can_receive: list[str]  # list of all available commands ["customName"]
 ```
 
 
 ## Event Listener
 The event listener allows you to listen to events that are published by your Dirigera hub. This is useful if you want to automate tasks based on events such as when a light is turned on or off, or when the color temperature of a light is changed.
 
 ```python
+import json
+from typing import Any
+
 
 def on_message(ws: Any, message: str):
     message_dict = json.loads(message)
     data = message_dict["data"]
     if data["id"] == bed_light.light_id:
         print(f"{message_dict['type']} event on {bed_light.custom_name}, attributes: {data['attributes']}")
 
@@ -144,14 +144,14 @@
 The primary motivation for this project was to provide users with the ability to control the startup behavior of their smart home lamps when there is a power outage.  
 The default behavior of the hub is to turn on all lights when power is restored, which can be problematic if the user is away from home or on vacation, and a small power fluctuation causes all lights to turn on and stay on. Unfortunately, the IKEA app does not offer a way to change this default behavior.  
 The `set_startup_behaviour()` function enables users to override the default behavior and choose the startup behavior that best suits their needs (START_ON = turn on light when power is back, START_OFF = light stays off when power is back).  
 I can not guarantee that all IKEA lamps offer this functionality.
 
 ## Contributing
 
-Contributions are welcome! If you have an idea for a new feature or a bug fix, please submit a pull request.
+Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ## License
 
 The MIT License (MIT)
 
-Copyright (c) 2023 Leggin
+Copyright (c) 2023 Leggin
```

### Comparing `dirigera-0.1.2/pyproject.toml` & `dirigera-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.2"
+version = "0.1.3"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.2/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.3/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/src/dirigera/devices/light.py` & `dirigera-0.1.3/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.3/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/src/dirigera/hub/auth.py` & `dirigera-0.1.3/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/src/dirigera/hub/hub.py` & `dirigera-0.1.3/src/dirigera/hub/hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.2
+Version: 0.1.3
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,17 +31,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Dirigera Python client
+# Dirigera Python Client
+![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
+![Pypi](https://img.shields.io/pypi/v/dirigera)
+[![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 
-This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Currently, only light control is supported, but support for other features will be added in the future.
+
+This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
+ - [light control](#controlling-lights)
+ - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
+ - [event listener](#event-listener) for hub events
+
+Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
 pip install dirigera
 ```
 
@@ -57,17 +66,17 @@
    ```
     Press the action button on Dirigera then hit ENTER ...
     Your Token:
     mgwB.aXqwpzV89N0aUwBhZMJjD8a.UBPyzy2InGtqgwo2MO5.xX4ug7.uBcVJquwYzLnAijF7SdYKvNxTo0uzQKahV10A-3ZQOz-UAubGP6sHWt1CJx3QmWZyE7ZcMZKgODXjSzWL1lumKgGz5dUIwFi3rhNxgK-IsBGeGVhNXPt8vGrYEcZePwPvNAIg8RqmlH27L-JZPnkAtP2wHoOdW72Djot3yJsohtEsb0p9mJvoZFSavTlTr4LDuf584vuH5fha5xoR9QhhIvvgbAP-s4EHFqENNi6vrYLHKR.sdqnv4sYw6UH-l6oiPnnRLxinoqBPOlWhlcL9doFviXQE.tZ9X8WVqyBrd0NYHlo9iorEvUbnZuD02BEJrg4NLwgh3rZtyF0Mi46HenynzBohbPn4RnuSYYCiHt5EZnWedxBtDqc7mSTm1ZtyD
    ```
 6. Done
 
-## Dirigera Hub
+## [Dirigera Hub](./src/dirigera/hub/hub.py)
 
-Setting up the client works by providing the token and ip address that is read from your .env file by the `config.py`
+Setting up the client works by providing the token and ip address.
 
 ```python
 import dirigera
 
 dirigera_hub = dirigera.Hub(
     token="mgwB.aXqwpzV89N0aUwBhZMJjD8a...",
     ip_address="192.1..."
@@ -81,51 +90,79 @@
 ```python
 lights = dirigera_hub.get_lights()
 ```
 
 The light object has the following attributes:
 
 ```python
-    device_id: str
-    is_reachable: bool
-    custom_name: str
-    is_on: bool
-    startup_on_off: StartupEnum | None
-    light_level: int | None  # not all lights have a light level
-    color_temp: int | None  # not all lights have a color temperature
-    color_temp_min: int | None
-    color_temp_max: int | None
-    color_hue: int | None  # not all lights have a color hue
-    color_saturation: float | None  # not all lights have a color saturation
-    room_id: str
-    room_name: str
-    can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+startup_on_off: StartupEnum | None
+light_level: int | None  # not all lights have a light level
+color_temp: int | None  # not all lights have a color temperature
+color_temp_min: int | None
+color_temp_max: int | None
+color_hue: int | None  # not all lights have a color hue
+color_saturation: float | None  # not all lights have a color saturation
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
 ```
 
 Available methods for light are:
 
 ```python
-    light.set_name(name="kitchen light 1")
+light.set_name(name="kitchen light 1")
 
-    light.set_light(lamp_on=True)
+light.set_light(lamp_on=True)
 
-    light.set_light_level(light_level=90)
+light.set_light_level(light_level=90)
 
-    light.set_color_temperature(color_temp=3000)
+light.set_color_temperature(color_temp=3000)
 
-    light.set_light_color(hue=128, saturation=0.5)
+light.set_light_color(hue=128, saturation=0.5)
 
-    light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+```
+
+## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
+Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
+
+
+To get the environment sensors use:
+```python
+sensors = dirigera_hub.get_environment_sensors()
+```
+
+The environment sensor object has the following attributes:
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+current_temperature: str
+current_rh: int  # current humidity
+current_pm25: int  # current particulate matter 2.5
+max_measured_pm25: int  # maximum measurable particulate matter 2.5
+min_measured_pm25: int  # minimum measurable particulate matter 2.5
+voc_index: int  # current volatile organic compound
+room_id: str
+room_name: str
+can_receive: list[str]  # list of all available commands ["customName"]
 ```
 
 
 ## Event Listener
 The event listener allows you to listen to events that are published by your Dirigera hub. This is useful if you want to automate tasks based on events such as when a light is turned on or off, or when the color temperature of a light is changed.
 
 ```python
+import json
+from typing import Any
+
 
 def on_message(ws: Any, message: str):
     message_dict = json.loads(message)
     data = message_dict["data"]
     if data["id"] == bed_light.light_id:
         print(f"{message_dict['type']} event on {bed_light.custom_name}, attributes: {data['attributes']}")
 
@@ -144,14 +181,14 @@
 The primary motivation for this project was to provide users with the ability to control the startup behavior of their smart home lamps when there is a power outage.  
 The default behavior of the hub is to turn on all lights when power is restored, which can be problematic if the user is away from home or on vacation, and a small power fluctuation causes all lights to turn on and stay on. Unfortunately, the IKEA app does not offer a way to change this default behavior.  
 The `set_startup_behaviour()` function enables users to override the default behavior and choose the startup behavior that best suits their needs (START_ON = turn on light when power is back, START_OFF = light stays off when power is back).  
 I can not guarantee that all IKEA lamps offer this functionality.
 
 ## Contributing
 
-Contributions are welcome! If you have an idea for a new feature or a bug fix, please submit a pull request.
+Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ## License
 
 The MIT License (MIT)
 
 Copyright (c) 2023 Leggin
```

### Comparing `dirigera-0.1.2/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.3/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/tests/test_environment_sensor.py` & `dirigera-0.1.3/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.2/tests/test_light.py` & `dirigera-0.1.3/tests/test_light.py`

 * *Files identical despite different names*

