# Comparing `tmp/UC2 REST-0.2.0.9.tar.gz` & `tmp/UC2 REST-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UC2 REST-0.2.0.9.tar", last modified: Fri Mar 24 08:35:41 2023, max compression
+gzip compressed data, was "UC2 REST-2.1.0.tar", last modified: Sun Apr 23 18:32:41 2023, max compression
```

## Comparing `UC2 REST-0.2.0.9.tar` & `UC2 REST-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.873601 UC2 REST-0.2.0.9/UC2_REST.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/uc2rest/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5682 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/UC2Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-24 08:35:27.000000 UC2 REST-0.2.0.9/uc2rest/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/analog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/config_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/digitalout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/galvo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/laser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/ledmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/motor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/mserial.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/slm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:41.236843 UC2 REST-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-04-23 18:32:41.236843 UC2 REST-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:41.232843 UC2 REST-2.1.0/UC2_REST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:32:41.000000 UC2 REST-2.1.0/UC2_REST.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:32:41.236843 UC2 REST-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:41.236843 UC2 REST-2.1.0/uc2rest/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6305 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/UC2Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 18:32:25.000000 UC2 REST-2.1.0/uc2rest/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/analog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/config_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/digitalout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/galvo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/ledmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/mserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/slm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-23 18:32:24.000000 UC2 REST-2.1.0/uc2rest/wifi.py
```

### Comparing `UC2 REST-0.2.0.9/PKG-INFO` & `UC2 REST-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UC2 REST
-Version: 0.2.0.9
+Version: 2.1.0
 Summary: This pacage will help you to drive the ESP32-driven microscopy control modules from UC2
 Home-page: https://github.com/openUC2/UC2-REST
 Author: Benedict Diederich
 Author-email: benedictdied@gmail.com
 License: GPL v3
 Keywords: UC2REST API to control ESP32-driven microscopy control boards
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: UC2 REST Version: 0.2.0.9 Summary: This pacage will
+Metadata-Version: 2.1 Name: UC2 REST Version: 2.1.0 Summary: This pacage will
 help you to drive the ESP32-driven microscopy control modules from UC2 Home-
 page: https://github.com/openUC2/UC2-REST Author: Benedict Diederich Author-
 email: benedictdied@gmail.com License: GPL v3 Keywords: UC2REST API to control
 ESP32-driven microscopy control boards Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `UC2 REST-0.2.0.9/README.md` & `UC2 REST-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/UC2_REST.egg-info/PKG-INFO` & `UC2 REST-2.1.0/UC2_REST.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UC2-REST
-Version: 0.2.0.9
+Version: 2.1.0
 Summary: This pacage will help you to drive the ESP32-driven microscopy control modules from UC2
 Home-page: https://github.com/openUC2/UC2-REST
 Author: Benedict Diederich
 Author-email: benedictdied@gmail.com
 License: GPL v3
 Keywords: UC2REST API to control ESP32-driven microscopy control boards
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: UC2-REST Version: 0.2.0.9 Summary: This pacage will
+Metadata-Version: 2.1 Name: UC2-REST Version: 2.1.0 Summary: This pacage will
 help you to drive the ESP32-driven microscopy control modules from UC2 Home-
 page: https://github.com/openUC2/UC2-REST Author: Benedict Diederich Author-
 email: benedictdied@gmail.com License: GPL v3 Keywords: UC2REST API to control
 ESP32-driven microscopy control boards Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `UC2 REST-0.2.0.9/UC2_REST.egg-info/SOURCES.txt` & `UC2 REST-2.1.0/UC2_REST.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 uc2rest/modules.py
 uc2rest/motor.py
 uc2rest/mserial.py
 uc2rest/pid.py
 uc2rest/slm.py
 uc2rest/state.py
 uc2rest/updater.py
+uc2rest/utils.py
 uc2rest/wifi.py
```

### Comparing `UC2 REST-0.2.0.9/setup.py` & `UC2 REST-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/UC2Client.py` & `UC2 REST-2.1.0/uc2rest/UC2Client.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 # coding: utf-8
 #%%
 """
 Simple client code for the ESP32 in Python
 Copyright 2021 Benedict Diederich, released under LGPL 3.0 or later
 """
 from .mserial import Serial
+from .mserial import SerialManagerWrapper
+
 try:
-    from imswitch.imcommon.model import initLogger
+    from .imswitch.imcommon.model import initLogger
     IS_IMSWITCH = True
 except:
     print("No imswitch available")
     from .logger import Logger
     IS_IMSWITCH = False
 
-import requests
+try:
+    import requests
+except:
+    print("No requests available - running on pyscript?")
 
 class UC2Client(object):
     # headers = {'ESP32-version': '*'}
     headers={"Content-Type":"application/json"}
     getmessage = ""
     is_connected = False
 
     is_wifi = False
     is_serial = False
 
     # BAUDRATE = 500000
     BAUDRATE = 115200
 
-    def __init__(self, host=None, port=31950, serialport=None, identity="UC2_Feather", baudrate=BAUDRATE, NLeds=64, DEBUG=False):
+    def __init__(self, host=None, port=31950, serialport=None, identity="UC2_Feather", baudrate=BAUDRATE, NLeds=64, SerialManager=None, DEBUG=False):
         '''
         This client connects to the UC2-REST microcontroller that can be found here
         https://github.com/openUC2/UC2-REST
 
         generally speaking you send/receive JSON documents that will cause an:
         1. action => "/XXX_act"
         2. getting => "/XXX_get"
@@ -44,14 +49,15 @@
         if IS_IMSWITCH:
             self.logger = initLogger(self, tryInheritParent=True)
         else:
             from .logger import Logger
             self.logger = Logger()
         # set default APIVersion
         self.APIVersion = 2
+        self.isPyScript = False
 
         # initialize communication channel (# connect to wifi or usb)
         if serialport is not None:
             # use USB connection
             self.serial = Serial(serialport, baudrate, parent=self, identity=identity, DEBUG=DEBUG)
             self.is_serial = True
             self.is_connected = True
@@ -61,17 +67,21 @@
             self.is_wifi = True
             self.host = host
             self.port = port
 
             # check if host is up
             self.logger.debug(f"Connecting to microscope {self.host}:{self.port}")
             self.is_connected = self.isConnected()
+        elif SerialManager is not None:
+            # we are trying to access the controller from .a web browser
+            self.serial = SerialManagerWrapper(SerialManager, parent=self)
+            self.isPyScript = True
         else:
             self.logger.error("No ESP32 device is connected - check IP or Serial port!")
-
+        
         # import libraries depending on API version
         if self.APIVersion == 1:
             self.logger.debug("Using API version 1")
             from .v1.galvo import Galvo
             from .v1.config import config
             from .v1.logger import Logger
             from .v1.ledmatrix import LedMatrix
@@ -89,28 +99,30 @@
             from .motor import Motor
             from .home import Home
             from .state import State
             from .laser import Laser
             from .wifi import Wifi
             from .camera import Camera
             from .analog import Analog
-            from .updater import updater
+            if not self.isPyScript: from .updater import updater
             from .modules import Modules
             from .digitalout import DigitalOut
 
 
         #FIXME
         #self.set_state(debug=False)
 
         # initialize state
         self.state = State(self)
-        self.state.get_state()
-
+        if not self.isPyScript: 
+            self.state.get_state()
+       
         # initialize config
-        self.config = config(self)
+        if not self.isPyScript: 
+            self.config = config(self)
 
         # initialize LED matrix
         self.led = LedMatrix(self, NLeds=NLeds)
 
         # initilize motor
         self.motor = Motor(self)
         
@@ -135,42 +147,44 @@
         # initialize analog
         self.analog = Analog(self)
         
         # initialize digital out
         self.digitalout = DigitalOut(self)
         
         # initialize config
-        self.config = config(self)
-        self.pinConfig = self.config.loadConfigDevice()
+        if not self.isPyScript: 
+            self.config = config(self)
+            self.pinConfig = self.config.loadConfigDevice()
         
         # initialize updater 
-        self.updater = updater(parent=self)
+        if not self.isPyScript: 
+            self.updater = updater(parent=self)
         
         # initialize module controller
         self.modules = Modules(parent=self)
    
     def post_json(self, path, payload, getReturn=True, timeout=1):
         if self.is_wifi:
             # FIXME: this is not working
             url = f"http://{self.host}:{self.port}{path}"
             r = requests.post(url, json=payload, headers=self.headers)
             return r.json()
-        elif self.is_serial:
+        elif self.is_serial or self.isPyScript:
             return self.serial.post_json(path, payload, getReturn=getReturn, timeout=timeout)
         else:
             self.logger.error("No ESP32 device is connected - check IP or Serial port!")
             return None
 
     def get_json(self, path, timeout=1):
         if self.is_wifi:
             # FIXME: this is not working
             url = f"http://{self.host}:{self.port}{path}"
             r = requests.get(url, headers=self.headers)
             return r.json()
-        elif self.is_serial:
+        elif self.is_serial or self.isPyScript:
             self.serial.get_json(path)
             return self.serial.read_json()
         else:
             self.logger.error("No ESP32 device is connected - check IP or Serial port!")
             return None
 
     def setDebugging(self, debug=False):
```

### Comparing `UC2 REST-0.2.0.9/uc2rest/analog.py` & `UC2 REST-2.1.0/uc2rest/analog.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/camera.py` & `UC2 REST-2.1.0/uc2rest/camera.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/config.py` & `UC2 REST-2.1.0/uc2rest/config.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/config_.py` & `UC2 REST-2.1.0/uc2rest/config_.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/digitalout.py` & `UC2 REST-2.1.0/uc2rest/digitalout.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/galvo.py` & `UC2 REST-2.1.0/uc2rest/galvo.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/home.py` & `UC2 REST-2.1.0/uc2rest/home.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/laser.py` & `UC2 REST-2.1.0/uc2rest/laser.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/ledmatrix.py` & `UC2 REST-2.1.0/uc2rest/ledmatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         self.send_LEDMatrix_single(indexled=indexled, intensity=np.array(state)*np.array(self.intensity), timeout=self.timeout)
 
         return self.ledpattern
     
     def setAll(self, state, intensity=None):
         # fast addressing
         # turns on all LEDs at a certain intensity
+        state = bool(state)
         if intensity is not None:
             self.intensity = intensity
         intensity2display = np.array(self.intensity)*np.array(state)
         self.send_LEDMatrix_full(intensity = intensity2display, timeout=self.timeout)
         self.ledpattern = state*np.ones((self.NLeds, 3))
         return self.ledpattern
```

### Comparing `UC2 REST-0.2.0.9/uc2rest/modules.py` & `UC2 REST-2.1.0/uc2rest/modules.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/motor.py` & `UC2 REST-2.1.0/uc2rest/motor.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,16 +274,16 @@
         '''
 
         # only consider those actions that are necessary
         motorPropList = []
         for iMotor in range(4):
             if isAbsoluteArray[iMotor] or abs(steps[iMotor])>0:
                 motorProp = { "stepperid": self.motorAxisOrder[iMotor],
-                             "position": np.int(steps[iMotor]),
-                             "speed": speed[iMotor],
+                             "position": int(steps[iMotor]),
+                             "speed": int(speed[iMotor]),
                              "isabs": isAbsoluteArray[iMotor],
                              "isaccel":0, 
                              "isen": is_enabled}
                 motorPropList.append(motorProp)
 
         path = "/motor_act"
         payload = {
```

### Comparing `UC2 REST-0.2.0.9/uc2rest/mserial.py` & `UC2 REST-2.1.0/uc2rest/mserial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import serial
-import serial.tools.list_ports
+try:
+    import serial
+    import serial.tools.list_ports
+except:
+    print("No serial available - running on pyscript?")
 import time
 import json
 
-T_SERIAL_WARMUP = 2 # the time to wait for the serial to warm up
+T_SERIAL_WARMUP = 3 # the time to wait for the serial to warm up
 
 class Serial(object):
     
     def __init__(self, port, baudrate, timeout=1, identity="UC2_Feather", parent=None, DEBUG=False):
         self.serialport = port
         self.baudrate = baudrate
         self.timeout = timeout
@@ -204,14 +207,83 @@
                 if self.DEBUG: self._parent.logger.debug(returnmessage)
                 _returnmessage = json.loads(_returnmessage)
             except Exception as e:
                 if self.DEBUG: self._parent.logger.debug("Casting json string from serial to Python dict failed")
             self.isSafetyBreak = False
         return _returnmessage
         
+class SerialManagerWrapper(object):
+    
+    def __init__(self, SerialManager, DEBUG = True, parent=None) -> None:
+        self._parent=parent
+        self._parent.logger.debug("SerialManagerWrapper init")
+        self.SerialManager = SerialManager
+        self.isSafetyBreak = False
+        self.DEBUG = DEBUG
+        
+    async def post_json(self, path, payload={}, getReturn=True, timeout=1):
+        if "task" not in payload:
+            payload["task"] = path
+        
+        if "isblock" in payload:
+            is_blocking = payload["isblock"]
+        else:
+            is_blocking = True
+
+        # write message to the serial
+        await self.writeSerial(payload)
+        return ''
+        print(3)
+        if getReturn:
+            # we read the return message
+            #self._parent.logger.debug(payload)
+            returnmessage = self.readSerial(is_blocking=is_blocking, timeout=timeout)
+        else:
+            returnmessage = False
+        return returnmessage
+    
+    async def writeSerial(self, payload):
+        """Write JSON document to serial device"""
+        if type(payload)==dict:
+            payload = json.dumps(payload)
+        try:
+            if self.DEBUG: self._parent.logger.debug(payload)
+            await self.SerialManager.write(payload)
+        except Exception as e:
+            self._parent.logger.error(e)
+
+    async def readSerial(self, is_blocking=True, timeout = 1): # TODO: hardcoded timeout - not code
+        """Receive and decode return message"""
+        returnmessage = ''
+        _returnmessage = ''
+        rmessage = ''
+        _time0 = time.time()
+        print("Reading serial")
+        if is_blocking:
+            while is_blocking and not self.isSafetyBreak:
+                try:
+                    rmessage = await self.SerialManager.read().decode()
+                    if self.DEBUG: self._parent.logger.debug(rmessage)
+                    returnmessage += rmessage
+                    if rmessage.find("--")==0:
+                        break
+                except:
+                    pass
+                if (time.time()-_time0)>timeout:
+                    break
+            # casting to dict
+            try:
+                # TODO: check if this is a valid JSON
+                _returnmessage = returnmessage.split("\n--")[0].split("\n++")[-1].replace("\r","").replace("\n", "").replace("'", '"')
+                if self.DEBUG: self._parent.logger.debug(returnmessage)
+                _returnmessage = json.loads(_returnmessage)
+            except Exception as e:
+                if self.DEBUG: self._parent.logger.debug("Casting json string from serial to Python dict failed")
+            self.isSafetyBreak = False
+        return _returnmessage
 class SerialDummy(object):
         
     def __init__(self, port, baudrate, timeout=1, parent=None):
         self.port = port
         self.baudrate = baudrate
         self.timeout = timeout
         self._parent = parent
```

### Comparing `UC2 REST-0.2.0.9/uc2rest/pid.py` & `UC2 REST-2.1.0/uc2rest/pid.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/slm.py` & `UC2 REST-2.1.0/uc2rest/slm.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/state.py` & `UC2 REST-2.1.0/uc2rest/state.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/updater.py` & `UC2 REST-2.1.0/uc2rest/updater.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.9/uc2rest/wifi.py` & `UC2 REST-2.1.0/uc2rest/wifi.py`

 * *Files identical despite different names*

