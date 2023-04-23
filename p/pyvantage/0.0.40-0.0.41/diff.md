# Comparing `tmp/pyvantage-0.0.40.tar.gz` & `tmp/pyvantage-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.40.tar", last modified: Tue Jul  5 22:06:37 2022, max compression
+gzip compressed data, was "pyvantage-0.0.41.tar", last modified: Sun Apr 23 18:11:38 2023, max compression
```

## Comparing `pyvantage-0.0.40.tar` & `pyvantage-0.0.41.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2022-07-05 22:06:37.916660 pyvantage-0.0.40/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.40/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2022-07-05 22:06:37.916776 pyvantage-0.0.40/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.40/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2022-07-05 22:06:37.915010 pyvantage-0.0.40/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)    99909 2022-07-05 22:04:50.000000 pyvantage-0.0.40/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2022-07-05 22:06:37.916455 pyvantage-0.0.40/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2022-07-05 22:06:37.000000 pyvantage-0.0.40/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2022-07-05 22:06:37.000000 pyvantage-0.0.40/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-05 22:06:37.000000 pyvantage-0.0.40/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2022-07-05 22:06:37.000000 pyvantage-0.0.40/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.40/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2022-07-05 22:06:37.917176 pyvantage-0.0.40/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2022-07-05 22:06:29.000000 pyvantage-0.0.40/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.019250 pyvantage-0.0.41/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2021-06-03 17:37:04.000000 pyvantage-0.0.41/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-23 18:11:38.019412 pyvantage-0.0.41/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2023-04-23 17:44:30.000000 pyvantage-0.0.41/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.015777 pyvantage-0.0.41/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)    99570 2023-04-23 18:09:02.000000 pyvantage-0.0.41/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.018688 pyvantage-0.0.41/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:37.000000 pyvantage-0.0.41/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-04-23 18:11:38.019945 pyvantage-0.0.41/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-04-23 17:49:39.000000 pyvantage-0.0.41/setup.py
```

### Comparing `pyvantage-0.0.40/LICENSE` & `pyvantage-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.40/PKG-INFO` & `pyvantage-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.40
+Version: 0.0.41
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.40/README.md` & `pyvantage-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.40/pyvantage/__init__.py` & `pyvantage-0.0.41/pyvantage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,31 +106,30 @@
 # - Control devices connected via serial/ethernet links, such as Elk alarms,
 #   stereo systems, etc.
 #
 #
 #  light.mh_m_great_room_big_ass_fan (load_type == Motor)
 
 import logging
-import telnetlib
 import socket
+import ssl
 import select
 import threading
 import time
 import base64
 import re
 import json
 import os
 import traceback
 
 from collections import deque
 from xml.sax.saxutils import escape
 
-from colormath.color_objects import sRGBColor, HSVColor
-from colormath.color_conversions import convert_color
-
+from colorsys import hsv_to_rgb, rgb_to_hsv
+from xml.etree import ElementTree as ET
 
 def kelvin_to_level(kelvin):
     """Convert kelvin temperature to a USAI level."""
     if kelvin < 2200:
         return 0
     if kelvin > 6000:
         return 100.0
@@ -168,32 +167,36 @@
     """Raised when a connection already exists (e.g. two connect() calls)."""
 
 
 class VantageConnection(threading.Thread):
     """Encapsulates the connection to the Vantage controller."""
 
     def __init__(self, host, user, password, cmd_port, recv_callback,
-                 commdebug=True, num_connections=2):
+                 commdebug=True, num_connections=2, use_ssl=False):
         """Initializes the vantage connection, doesn't actually connect."""
         threading.Thread.__init__(self, name="VantageConnection")
 
         self._host = host
         self._user = user
         self._password = password
         self._cmd_port = cmd_port
+        self._use_ssl = use_ssl
         self._num_connections = num_connections
-        self._telnet = [None] * num_connections
+        self._sockets = [None] * num_connections
         self._connected = [False] * num_connections
-        self._iconn = 0  # index into the _telnet array
+        self._iconn = 0  # index into the _sockets array
         self._lock = threading.RLock()
         self._connect_cond = threading.Condition(lock=self._lock)
         self._recv_cb = recv_callback
         self._done = False
         self._commdebug = commdebug
 
+        if use_ssl:
+            self._ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+
         self.setDaemon(True)
 
     def connect(self):
         """Connects to the vantage controller."""
         if all(self._connected) or self.is_alive():
             raise ConnectionExistsError("Already connected")
         # After starting the thread we wait for it to post us
@@ -213,64 +216,88 @@
             if cmd.startswith("LOGIN"):
                 pass
             elif cmd.startswith("GET") or cmd.startswith("ADDSTATUS"):
                 _LOGGER.debug("Vantage #%s send_ascii_nl: %s", i, cmd)
             else:
                 _LOGGER.info("Vantage #%s send_ascii_nl: %s", i, cmd)
         try:
-            self._telnet[i].write(cmd.encode('ascii') + b'\r\n')
+            self._sockets[i].send(cmd.encode('ascii') + b'\r\n')
         except BrokenPipeError:
             _LOGGER.warning("Vantage BrokenPipeError - disconnected but retrying")
             self._connected[i] = False
-            raise
 
     def send_ascii_nl(self, cmd):
         """Sends the specified command to the vantage controller.
 
         Must not hold self._lock"""
         with self._lock:
             self._send_ascii_nl_locked(cmd, self._iconn)
             if not cmd.startswith("GET"):
                 self._iconn = (self._iconn + 1) % self._num_connections
 
+    def _read_until(self, delimiter, i):
+        """Read data from a socket until a delimiter is found."""
+        data = b''
+        while True:
+            chunk = self._sockets[i].recv(1024)
+            if not chunk:
+                break
+            data += chunk
+            if delimiter in data:
+                break
+        return data
+
     def _do_login_locked(self, i):
-        """Executes the login procedure (telnet) as well as setting up some
+        """Executes the login procedure as well as setting up some
         connection defaults like turning off the prompt, etc."""
         while True:
             try:
-                self._telnet[i] = telnetlib.Telnet(self._host, self._cmd_port)
+                self._sockets[i] = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                self._sockets[i].connect((self._host, self._cmd_port))
+
+                if self._use_ssl:
+                    self._sockets[i] = self._ssl_context.wrap_socket(self._sockets[i])
+
+                self._sockets[i].settimeout(2)
                 break
             except Exception as e:
                 _LOGGER.warning("Could not connect #%s to %s:%d, "
                                 "retrying after 3 sec (%s)", i,
                                 self._host, self._cmd_port,
                                 e)
                 time.sleep(3)
                 continue
         if not (self._user is None or self._password is None):
             _LOGGER.debug("Connection #%s is made, logging in", i)
             self._send_ascii_nl_locked("LOGIN " + self._user +
                                        " " + self._password, i)
             _LOGGER.debug("reading login response for #%s", i)
-            self._telnet[i].read_until(b'\r\n', 2)
+            self._read_until(b'\r\n', i)
         if i == 0:
             self._send_ascii_nl_locked("STATUS LOAD", i)
-            self._telnet[i].read_until(b'\r\n', 2)
+            self._read_until(b'\r\n', i)
+
             self._send_ascii_nl_locked("STATUS BLIND", i)
-            self._telnet[i].read_until(b'\r\n', 2)
+            self._read_until(b'\r\n', i)
+
             self._send_ascii_nl_locked("STATUS BTN", i)
-            self._telnet[i].read_until(b'\r\n', 2)
+            self._read_until(b'\r\n', i)
+
             self._send_ascii_nl_locked("STATUS VARIABLE", i)
-            self._telnet[i].read_until(b'\r\n', 2)
+            self._read_until(b'\r\n', i)
         return True
 
     def _disconnect_locked(self):
         self._connected = [False] * self._num_connections
         self._connect_cond.notify_all()
-        self._telnet = [None] * self._num_connections
+
+        for i in range(0, self._num_connections):
+            self._sockets[i].close()
+            self._sockets[i] = None
+
         _LOGGER.warning("Disconnected")
 
     def _maybe_reconnect(self):
         """Reconnects to controller if we have been previously disconnected."""
         need_notify = False
         with self._lock:
             for i in range(0, self._num_connections):
@@ -286,35 +313,33 @@
 
     def run(self):
         """Main thread to maintain connection and receive remote status."""
         _LOGGER.debug("VantageConnection run started")
         while True:
             self._maybe_reconnect()
             try:
-                sockets = [t.get_socket() for t in self._telnet]
-                readable, _, exceptional = select.select(sockets, [], [])
-                for i, t in enumerate(self._telnet):
-                    if t.get_socket() in exceptional:
+                readable, _, exceptional = select.select(self._sockets, [], [])
+                for i, sock in enumerate(self._sockets):
+                    if sock in exceptional:
                         _LOGGER.error("Exceptional socket #%s: %s", i, t)
                         raise EOFError()
-                    if t.get_socket() in readable:
-                        line = self._telnet[i].read_until(b"\n", 2)
+                    if sock in readable:
+                        line = self._read_until(b'\n', i)
                         self._recv_cb(line.decode('ascii').rstrip(), i)
             except EOFError:
                 _LOGGER.warning("run got EOFError")
                 with self._lock:
                     self._disconnect_locked()
                 continue
             except BrokenPipeError:
                 _LOGGER.warning("run got BrokenPipeError")
                 with self._lock:
                     self._disconnect_locked()
                 continue
 
-
 def _desc_from_t1t2(title1, title2):
     if not title2:
         desc = title1 or ''
     else:
         desc = title1 + ' ' + title2
     return desc.strip()
 
@@ -349,15 +374,15 @@
         self.variables = []
         self.tasks = []
         self.buttons = []
         self.keypads = []
         self.sensors = []
         self.load_groups = []
         self.last_area_vid = -1
-        self.vid_to_area = {}
+        self.vid_to_area = vantage._vid_to_area = {}
         self.vid_to_load = {}
         self.vid_to_keypad = {}
         self.vid_to_button = {}
         self.vid_to_variable = {}
         self.vid_to_task = {}
         self.vid_to_sensor = {}
         self.name_to_task = {}
@@ -369,16 +394,14 @@
     def parse(self):
         """Main entrypoint into the parser.
 
         It interprets and creates all the relevant Vantage objects and
         stuffs them into the appropriate hierarchy.
         """
 
-        import xml.etree.ElementTree as ET
-
         root = ET.fromstring(self._xml_db_str)
         # The structure of a Lutron config is something like this:
         # <Areas>
         #   <Area ...>
         #     <DeviceGroups ...>
         #     <Scenes ...>
         #     <ShadeGroups ...>
@@ -390,77 +413,77 @@
         # Load (with @VID and <Name> and <Area> (enclosing Area VID))
         # GMem (with @VID and <Name> [variables])
         # Task (with @VID and <Name> )
         # OmniSensor (with @VID and <Name> )
         # Timer (with @VID and <Name> )
         # Keypad (with @VID and <Name> )
 
-        areas = root.findall(".//Objects//Area[@VID]")
+        objects = root.find("Objects")
+        areas = objects.findall("Object/Area[@VID]")
         for area_xml in areas:
             if self.project_name is None:
-                self.project_name = area_xml.find('Name').text
+                self.project_name = area_xml.findtext('Name')
                 _LOGGER.debug("Set project name to %s", self.project_name)
             area = self._parse_area(area_xml)
             _LOGGER.debug("Area = %s", area)
             self.vid_to_area[area.vid] = area
             self.last_area_vid = area.vid
 
-        irzones = root.findall(".//Objects//IRZone[@VID]")
+        irzones = objects.findall("Object/IRZone[@VID]")
         for irzone_xml in irzones:
             area = self._parse_irzone(irzone_xml)
             _LOGGER.debug("IRZone = %s", area)
             self.vid_to_area[area.vid] = area
 
-        loads = root.findall(".//Objects//Load[@VID]")
-        loads = loads + root.findall(".//Objects//Vantage.DDGColorLoad[@VID]")
+        # note the extra '/' after 'Object/ -- the Vantage.DDGColorLoad elements aren't always direct descendents of Object
+        loads = objects.findall("Object/Load[@VID]") + objects.findall("Object//Vantage.DDGColorLoad[@VID]")
         other_loads = []
         color_loads = []
         open_loads = []
         for ld in loads:
-            t = ld.find('Name').text
+            t = ld.findtext('Name')
             if t.endswith(' COLOR'):
                 color_loads.append(ld)
             elif t.lower().endswith(' open'):
                 open_loads.append(ld)
             else:
                 other_loads.append(ld)
         ordered_loads = open_loads + other_loads + color_loads
         skip_load_vids = set()
         for load_xml in ordered_loads:
-            xml_name = load_xml.find('Name').text
+            xml_name = load_xml.findtext('Name')
             output = None
             if xml_name.lower().endswith(" open"):
                 close_name = replace_keep_case(' open', " close", xml_name)
                 stop_name = replace_keep_case(' open', " stop", xml_name)
                 isopen_name = replace_keep_case(' open', " is open", xml_name)
                 _LOGGER.debug("Looking for close_name = %s", close_name)
                 _LOGGER.debug("Looking for stop_name = %s", stop_name)
                 _LOGGER.debug("Looking for isopen_name = %s", isopen_name)
-                close_load_xml = root.findall(
-                    ".//Objects//Load[Name='" + close_name + "']")
+                close_load_xml = objects.findall(
+                    "Object/Load[Name='" + close_name + "']")
                 if len(close_load_xml) == 1:
                     close_load_xml = close_load_xml[0]
-                    isopen_contact_xml = root.findall(
-                        ".//Objects//DryContact[Name='" + isopen_name + "']")
+                    isopen_contact_xml = objects.findall(
+                        "Object/DryContact[Name='" + isopen_name + "']")
                     if len(isopen_contact_xml) == 1:
                         isopen_contact_xml = isopen_contact_xml[0]
                     else:
                         isopen_contact_xml = None
-                    stop_load_xml = root.findall(
-                        ".//Objects//Load[Name='" + stop_name + "']")
+                    stop_load_xml = objects.findall(
+                        "Object/Load[Name='" + stop_name + "']")
                     if len(stop_load_xml) == 1:
                         stop_load_xml = stop_load_xml[0]
                     else:
                         stop_load_xml = None
                     shade = self._parse_3_shade(isopen_contact_xml,
                                                 load_xml,
                                                 close_load_xml,
                                                 stop_load_xml)
-                    for v in shade.vids:
-                        skip_load_vids.add(v)
+                    skip_load_vids = { k for k in shade.vids if k is not None }
                     self.vid_to_shade[shade.vid] = shade
                     self.outputs.append(shade)
                     _LOGGER.debug("shade3 = %s", shade)
                     continue
 
             if int(load_xml.get("VID")) in skip_load_vids:
                 _LOGGER.debug("Skipping %s because used for blind3", load_xml)
@@ -469,214 +492,211 @@
             if output is None:
                 continue
             self.outputs.append(output)
             self.vid_to_load[output.vid] = output
             _LOGGER.debug("Output = %s", output)
             self.vid_to_area[output.area].add_output(output)
 
-        load_groups = root.findall(".//Objects//LoadGroup[@VID]")
+        load_groups = objects.findall("Object/LoadGroup[@VID]")
         for lg_xml in load_groups:
             lgroup = self._parse_load_group(lg_xml)
             if lgroup is None:
                 continue
             self.load_groups.append(lgroup)
             self.outputs.append(lgroup)
             self.vid_to_load[lgroup.vid] = lgroup
             _LOGGER.debug("load group = %s", lgroup)
             self.vid_to_area[lgroup.area].add_output(lgroup)
 
-        keypads = root.findall(".//Objects//Keypad[@VID]")
-        keypads = keypads + root.findall(".//Objects//DualRelayStation[@VID]")
-        keypads = keypads + root.findall(".//Objects//IRZone[@VID]")
-        keypads = keypads + root.findall(".//Objects//Dimmer[@VID]")
-        keypads = keypads + root.findall(".//Objects//EqCtrl[@VID]")
-        keypads = keypads + root.findall(".//Objects//EqUX[@VID]")
+        keypads = [obj for t in ["Keypad", "DualRelayStation", "IRZone", "Dimmer", "EqCtrl", "EqUX"]
+                       for obj in objects.findall(f"Object/{t}[@VID]")]
         for kp_xml in keypads:
             keypad = self._parse_keypad(kp_xml)
             _LOGGER.debug("keypad = %s", keypad)
             self.vid_to_keypad[keypad.vid] = keypad
             if keypad.area > 0:
                 self.vid_to_area[keypad.area].add_keypad(keypad)
             self.keypads.append(keypad)
 
-        buttons = root.findall(".//Objects//Button[@VID]")
+        buttons = objects.findall("Object/Button[@VID]")
         for button_xml in buttons:
             b = self._parse_button(button_xml)
             if not b:
                 continue
             _LOGGER.debug("b = %s", b)
             self.vid_to_button[b.vid] = b
             if b.area != -1:
                 self.vid_to_area[b.area].add_button(b)
                 self.buttons.append(b)
 
-        drycontacts = root.findall(".//Objects//DryContact[@VID]")
+        drycontacts = objects.findall("Object/DryContact[@VID]")
         for dc_xml in drycontacts:
             dc = self._parse_drycontact(dc_xml)
             if not dc:
                 continue
             _LOGGER.debug("dc = %s", dc)
             self.vid_to_button[dc.vid] = dc
             self.buttons.append(dc)
 
-        variables = root.findall(".//Objects//GMem[@VID]")
+        variables = objects.findall("Object/GMem[@VID]")
         for v in variables:
             var = self._parse_variable(v)
             _LOGGER.debug("var = %s", var)
             self.vid_to_variable[var.vid] = var
             # N.B. variables have categories, not areas, so no add to area
             self.variables.append(var)
 
-        omnisensors = root.findall(".//Objects//OmniSensor[@VID]")
+        omnisensors = objects.findall("Object/OmniSensor[@VID]")
         for s in omnisensors:
             sensor = self._parse_omnisensor(s)
             _LOGGER.debug("sensor = %s", sensor)
             self.vid_to_sensor[sensor.vid] = sensor
             # N.B. variables have categories, not areas, so no add to area
             self.sensors.append(sensor)
 
-        lightsensors = root.findall(".//Objects//LightSensor[@VID]")
+        lightsensors = objects.findall("Object/LightSensor[@VID]")
         for s in lightsensors:
             sensor = self._parse_lightsensor(s)
             _LOGGER.debug("sensor = %s", sensor)
             self.vid_to_sensor[sensor.vid] = sensor
             # N.B. variables have categories, not areas, so no add to area
             self.sensors.append(sensor)
 
-        tasks = root.findall(".//Objects//Task[@VID]")
+        tasks = objects.findall("Object/Task[@VID]")
         for t in tasks:
             task = self._parse_task(t)
             _LOGGER.debug("task = %s", task)
             self.vid_to_task[task.vid] = task
             self.name_to_task[task.name] = task
             # N.B. tasks have categories, not areas, so no add to area
             self.tasks.append(task)
 
         # Lots of different shade types, one xpath for each kind of shade
         # MechoShade driver shades
         shades = \
-            root.findall(".//Objects//MechoShade.IQ2_Shade_Node_CHILD[@VID]")
+            objects.findall("Object/MechoShade.IQ2_Shade_Node_CHILD[@VID]")
         shades = (shades +
-                  root.findall(".//Objects//MechoShade.IQ2_Group_CHILD[@VID]"))
+                  objects.findall("Object/MechoShade.IQ2_Group_CHILD[@VID]"))
         # Native QIS QMotion shades
-        shades = shades + root.findall(".//Objects//QISBlind[@VID]")
-        shades = shades + root.findall(".//Objects//BlindGroup[@VID]")
+        shades = shades + objects.findall("Object/QISBlind[@VID]")
+        shades = shades + objects.findall("Object/BlindGroup[@VID]")
         # Non-native QIS Driver QMotion shades (the old way)
         shades = (shades +
-                  root.findall(".//Objects//QMotion.QIS_Channel_CHILD[@VID]"))
+                  objects.findall("Object/QMotion.QIS_Channel_CHILD[@VID]"))
         # Somfy radio-controlled
         shades = (shades +
-                  root.findall(".//Objects//Somfy.URTSI_2_Shade_CHILD[@VID]"))
+                  objects.findall("Object/Somfy.URTSI_2_Shade_CHILD[@VID]"))
         # Somfy RS-485 SDN wired shades
         shades = (shades +
-                  root.findall(".//Objects//Somfy.RS-485_Shade_CHILD[@VID]"))
+                  objects.findall("Object/Somfy.RS-485_Shade_CHILD[@VID]"))
 
         for shade_xml in shades:
             shade = self._parse_shade(shade_xml)
             if shade is None:
                 continue
             self.vid_to_shade[shade.vid] = shade
             self.outputs.append(shade)
             _LOGGER.debug("shade = %s", shade)
 
         _LOGGER.debug("self._name_area_to_vid = %s", self._name_area_to_vid)
 
         return True
 
+    def _object_area_vid(self, obj):
+        """Parses an Area element which designates the VID of the Area that the
+        object is located in."""
+        if obj is None: return self.last_area_vid
+        area = obj.find('Area')
+        if area is None: return self.last_area_vid
+        return int(area.text)
+
     def _parse_area(self, area_xml):
         """Parses an Area tag, which is effectively a room, depending on how the
         Vantage controller programming was done."""
         try:
             vid = int(area_xml.get('VID'))
             area = Area(self._vantage,
-                        name=area_xml.find('Name').text,
-                        parent=int(area_xml.find('Area').text),
+                        name=area_xml.findtext('Name'),
+                        parent=self._object_area_vid(area_xml),
                         vid=vid,
-                        note=area_xml.find('Note').text)
+                        note=area_xml.findtext('Note'))
             return area
         except Exception as e:
             _LOGGER.warning("Error parsing Area vid = %d: %s", vid, e)
 
     def _parse_irzone(self, irzone_xml):
         """Parses an IRZone tag, which we treat like an area with no parent."""
         try:
             vid = int(irzone_xml.get('VID'))
             irzone = Area(self._vantage,
-                          name=irzone_xml.find('Name').text,
+                          name=irzone_xml.findtext('Name'),
                           parent=0,
                           vid=vid,
-                          note=irzone_xml.find('Note').text)
+                          note=irzone_xml.findtext('Note'))
             return irzone
         except Exception as e:
             _LOGGER.warning("Error parsing IRZone vid = %d: %s", vid, e)
 
     def _parse_variable(self, var_xml):
         """Parses a variable (GMem) tag."""
         try:
             vid = int(var_xml.get('VID'))
             subtype_node = var_xml.find('Tag')
             subtype = ''
             if subtype_node is not None:
                 subtype = subtype_node.text.lower()
             var = Variable(self._vantage,
-                           name=var_xml.find('Name').text,
+                           name=var_xml.findtext('Name'),
                            vid=vid, subtype=subtype)
             return var
         except Exception as e:
             _LOGGER.warning("Error parsing variable vid = %d: %s", vid, e)
 
     def _parse_omnisensor(self, sensor_xml):
         """Parses an OmniSensor tag."""
         try:
             vid = int(sensor_xml.get('VID'))
             kind = {
                 "Power": "power",
                 "Current": "current",
                 "Temperature": "sensor"
-            }[sensor_xml.find('Model').text]
+            }[sensor_xml.findtext('Model')]
             sensor = OmniSensor(self._vantage,
-                                name=sensor_xml.find('Name').text,
+                                name=sensor_xml.findtext('Name'),
                                 kind=kind,
                                 vid=int(sensor_xml.get('VID')))
             return sensor
         except Exception as e:
             _LOGGER.warning("Error parsing omnisensor vid = %d: %s", vid, e)
 
     def _parse_lightsensor(self, sensor_xml):
         """Parses a LightSensor object."""
         try:
             vid = int(sensor_xml.get('VID'))
-            area_xml = sensor_xml.find('Area')
-            area = (area_xml is not None and int(area_xml.text)) or -1
-            value_range = (float(sensor_xml.find('RangeLow').text),
-                           float(sensor_xml.find('RangeHigh').text))
+            value_range = (float(sensor_xml.findtext('RangeLow')),
+                           float(sensor_xml.findtext('RangeHigh')))
             return LightSensor(self._vantage,
-                               name=sensor_xml.find('Name').text,
-                               area=area,
+                               name=sensor_xml.findtext('Name'),
+                               area=self._object_area_vid(sensor_xml),
                                value_range=value_range,
                                vid=vid)
         except Exception as e:
             _LOGGER.warning("Error parsing lightsensor vid = %d: %s", vid, e)
 
     def _parse_shade(self, shade_xml):
         """Parses a shade node.
 
         Either a MechoShade.IQ2_Shade_Node_CHILD or
         QMotion.QIS_Channel_CHILD (shade) tag.
         """
         try:
             vid = int(shade_xml.get('VID'))
-            area_xml = shade_xml.find('Area')
-            area_vid = self.last_area_vid
-            if area_xml is not None:
-                area_vid = int(area_xml.text)
-
             shade = Shade(self._vantage,
-                          name=shade_xml.find('Name').text,
-                          area_vid=area_vid,
+                          name=shade_xml.findtext('Name'),
+                          area_vid=self._object_area_vid(shade_xml),
                           vid=vid)
             return shade
         except Exception as e:
             _LOGGER.warning("Error parsing shade vid = %d: %s", vid, e)
 
     def _parse_output(self, output_xml):
         """Parses a load.
@@ -688,26 +708,23 @@
         try:
             vid = int(output_xml.get('VID'))
             dname_xml = output_xml.find('DName')
             out_name = dname_xml is not None and dname_xml.text
             if out_name:
                 out_name = out_name.strip()
             if not out_name or out_name.isspace():
-                out_name = output_xml.find('Name').text.strip()
-            area_xml = output_xml.find('Area')
-            area_vid = self.last_area_vid
-            if area_xml is not None:
-                area_vid = int(area_xml.text)
+                out_name = output_xml.findtext('Name').strip()
+            area_vid = self._object_area_vid(output_xml)
 
             area_name = self.vid_to_area[area_vid].name.strip()
             lt_xml = output_xml.find('LoadType')
             if lt_xml is not None:
                 load_type = lt_xml.text.strip()
             else:
-                load_type = output_xml.find('ColorType').text.strip()
+                load_type = output_xml.findtext('ColorType').strip()
 
             output_type = 'LIGHT'
 
             # TODO: find a better heuristic so that on/off lights still show up
             if (load_type == 'High Voltage Relay' or
                 load_type == 'Low Voltage Relay'):
                 output_type = 'RELAY'
@@ -792,34 +809,19 @@
         _LOGGER.debug("_parse_3_shade io,o,c,s=%s, %s, %s, %s",
                       isopen_xml, open_xml, close_xml, stop_xml)
         vids = [int(isopen_xml.get('VID')) if isopen_xml else None,
                 int(open_xml.get('VID')),
                 int(close_xml.get('VID')),
                 int(stop_xml.get('VID')) if stop_xml else None]
 
-        shade_name = open_xml.find('Name').text.strip()[:-5]
-        area_xml = open_xml.find('Area')
-        area_vid = self.last_area_vid
-        if area_xml is not None:
-            area_vid = int(area_xml.text)
-
-        close_area_xml = close_xml and close_xml.find('Area')
-        close_area_vid = self.last_area_vid
-        if close_area_xml is not None:
-            close_area_vid = int(close_area_xml.text)
-
-        isopen_area_xml = isopen_xml and isopen_xml.find('Area')
-        isopen_area_vid = self.last_area_vid
-        if isopen_area_xml is not None:
-            isopen_area_vid = int(isopen_area_xml.text)
-
-        stop_area_xml = stop_xml and stop_xml.find('Area')
-        stop_area_vid = self.last_area_vid
-        if stop_area_xml is not None:
-            stop_area_vid = int(stop_area_xml.text)
+        shade_name = open_xml.findtext('Name').strip()[:-5]
+        area_vid = self._object_area_vid(open_xml)
+        close_area_vid = self._object_area_vid(close_xml)
+        isopen_area_vid = self._object_area_vid(isopen_xml)
+        stop_area_vid = self._object_area_vid(stop_xml)
 
         if ((area_vid != close_area_vid) or
              (isopen_xml and area_vid != isopen_area_vid) or
              (stop_xml and area_vid != stop_area_vid)):
             _LOGGER.warning("open/close/stop/isopen device "
                             "areas do not match: %s", shade_name)
             return None
@@ -827,30 +829,25 @@
                        name=shade_name,
                        area_vid=area_vid,
                        vids=vids)
         return shade
 
     def _parse_load_group(self, output_xml):
         """Parses a load group, which is a set of loads"""
-        out_name = output_xml.find('DName').text
+        out_name = output_xml.findtext('DName')
         if out_name:
             out_name = out_name.strip()
         if not out_name or out_name.isspace():
-            out_name = output_xml.find('Name').text
+            out_name = output_xml.findtext('Name')
         else:
             _LOGGER.debug("Using dname = %s", out_name)
-        area_xml = output_xml.find('Area')
-        area_vid = self.last_area_vid
-        if area_xml is not None:
-            area_vid = int(area_xml.text)
+        area_vid = self._object_area_vid(output_xml)
 
-#        area_name = self.vid_to_area[area_vid].name
         loads = output_xml.findall('./LoadTable/Load')
-        vid = output_xml.get('VID')
-        vid = int(vid)
+        vid = int(output_xml.get('VID'))
 
         load_vids = []
         color_vids = []
         dmx_color = False
         support_color_temp = False
         for load in loads:
             v = int(load.text)
@@ -875,26 +872,24 @@
                            dmx_color=dmx_color,
                            support_color_temp=support_color_temp,
                            vid=vid)
         return output
 
     def _parse_keypad(self, keypad_xml):
         """Parses a keypad device."""
-        area_xml = keypad_xml.find('Area')
-        area_vid = int(area_xml.text) if area_xml else -1
         keypad = Keypad(self._vantage,
-                        name=keypad_xml.find('Name').text + ' [K]',
-                        area=area_vid,
+                        name=keypad_xml.findtext('Name') + ' [K]',
+                        area=self._object_area_vid(keypad_xml),
                         vid=int(keypad_xml.get('VID')))
         return keypad
 
     def _parse_task(self, task_xml):
         """Parses a task object."""
         task = Task(self._vantage,
-                    name=task_xml.find('Name').text,
+                    name=task_xml.findtext('Name'),
                     vid=int(task_xml.get('VID')))
         return task
 
     def _parse_drycontact(self, dc_xml):
         """Parses a dry contact switch."""
         # A dry contact switch *may* be plugged into the back of a keypad (and
         # hence has a keypad like a button does), but nobody cares if it does.
@@ -902,19 +897,18 @@
         # one.
         try:
             vid = int(dc_xml.get('VID'))
             if self.vid_to_shade.get(vid):
                 _LOGGER.debug("Skipping vid=%d as drycontact "
                               "because already part of a BLIND3", vid)
                 return None
-            name = dc_xml.find('Name').text + ' [C]'
+            name = dc_xml.findtext('Name') + ' [C]'
             parent = dc_xml.find('Parent')
             parent_vid = int(parent.text)
-            area_xml = dc_xml.find('Area')
-            area_vid = int(area_xml.text) if area_xml else -1
+            area_vid = self._object_area_vid(dc_xml)
             num = 0
             keypad = None
             _LOGGER.debug("Found DryContact with vid = %d", vid)
             # Ugh, awful -- three different ways of representing bad-value
             button = Button(self._vantage, name, area_vid, vid, num,
                             parent_vid, keypad, False)
             return button
@@ -949,16 +943,16 @@
                 text1 = xml_name.text or ""
                 text2 = xml_text2.text or ""
                 name = text1.strip() + ' ' + text2.strip()
             name += ' [B]'
             # no Text1 sub-element on DryContact
             parent = button_xml.find('Parent')
             parent_vid = int(parent.text)
-            text1 = button_xml.find('Text1').text
-            text2 = button_xml.find('Text2').text
+            text1 = button_xml.findtext('Text1')
+            text2 = button_xml.findtext('Text2')
             desc = _desc_from_t1t2(text1, text2)
             num = int(parent.get('Position'))
             keypad = self.vid_to_keypad.get(parent_vid)
             if keypad is None:
                 irzone = self.vid_to_area.get(parent_vid)
                 if irzone is None:
                     _LOGGER.debug("No parent vid = %d for button vid = %d "
@@ -1007,36 +1001,40 @@
     # Status report lines come back from Vantage with this prefix
     OP_STATUS = 'S:'
 
     def __init__(self, host, user, password,
                  only_areas=None, exclude_areas=None,
                  cmd_port=3001, file_port=2001,
                  name_mappings=None, filename=None,
-                 commdebug=True, num_connections=1):
+                 commdebug=True, num_connections=1,
+                 hierarchical_names=True,
+                 use_ssl=False):
         """Initializes the Vantage object. No connection is made to the remote
         device."""
         self._host = host
         self._user = user
         self._password = password
         self._name = None
         if self._host is not None:
             self._conn = VantageConnection(host, user, password, cmd_port,
                                            self._recv, commdebug,
-                                           num_connections)
+                                           num_connections, use_ssl)
         else:
             self._conn = None
             if filename is None:
                 raise Exception("Need host or filename to be specified")
         self._cmds = deque([])
         self._name_mappings = name_mappings
         self._file_port = file_port
+        self._use_ssl = use_ssl
         self._only_areas = only_areas
         self._exclude_areas = exclude_areas
-        self._ids = {}
+        self._hierarchical_names = hierarchical_names
         self._names = {}   # maps from unique name to id
+        self._ids = {}
         self._subscribers = {}
         self._vid_to_area = {}  # copied out from the parser
         self._vid_to_load = {}  # copied out from the parser
         self._vid_to_variable = {}  # copied out from the parser
         self._vid_to_task = {}  # copied out from the parser
         self._vid_to_shade = {}  # copied out from the parser
         self._vid_to_sensor = {}  # copied out from the parser
@@ -1053,14 +1051,17 @@
         self.outputs = None
         self.variables = None
         self.tasks = None
         self.buttons = None
         self.keypads = None
         self.sensors = None
 
+        if use_ssl:
+            self._ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+
     def subscribe(self, obj, handler):
         """Subscribes to status updates of the requested object.
 
         The handler will be invoked when the controller sends a
         notification regarding changed state. The user can then
         further query the object for the state itself.
 
@@ -1104,62 +1105,61 @@
         ids = self._ids.setdefault(cmd_type2, {})
         if vid in ids:
             raise VIDExistsError("VID exists %s" % vid)
         self._ids[cmd_type][vid] = obj
         if cmd_type2:
             self._ids[cmd_type2][vid] = obj
 
-        # Now give the object a unique name.  We prefix in reverse order the
-        # areas the object is contained in.  So an object may be called "Main
-        # Floor-Kitchen-Ceiling Can Lights".  Every object must have a unique
-        # name, if there is a duplicate then (VID) is attached to the end.
-
-        lineage = self.get_lineage_from_obj(obj)
-        name = ""
-        # reverse all but the last element in list
-        for n in reversed(lineage[:-1]):
-            ns = n.strip()
-            if ns.startswith('Station Load '):
-                continue
-            if ns.startswith('Color Load '):
-                continue
-            if self._name_mappings:
-                mapped_name = self._name_mappings.get(ns.lower())
-                if mapped_name is not None:
-                    if mapped_name is True:
-                        continue
-                    ns = mapped_name
-            name += ns + "-"
-
-        # TODO: this may be a little too hacky
-        # Greg Badros has a convention of naming areas using 2-letter codes.
-        # This makes sure that we use "GH-Bedroom High East"
-        # instead of "GH-GH Bedroom High East"
-        # since it's sometimes convenient to have the short area
-        # at the start of the device name in vantage
-        if obj.name.startswith(name[0:-1]):
-            obj.name = name + obj.name[len(name):]
-        else:
-            obj.name = name + obj.name
+        # If configured, generate hierarchical object names.
+        # We prefix in reverse order the areas the object is contained in, eg:
+        # "Main Floor-Kitchen-Ceiling Can Lights"
+        if self._hierarchical_names:
+            lineage = self.get_lineage_from_obj(obj)
+            name = ""
+            # reverse all but the last element in list
+            for n in reversed(lineage[:-1]):
+                ns = n.strip()
+                if ns.startswith('Station Load '):
+                    continue
+                if ns.startswith('Color Load '):
+                    continue
+                if self._name_mappings:
+                    mapped_name = self._name_mappings.get(ns.lower())
+                    if mapped_name is not None:
+                        if mapped_name is True:
+                            continue
+                        ns = mapped_name
+                name += ns + "-"
+
+            # TODO: this may be a little too hacky
+            # Greg Badros has a convention of naming areas using 2-letter codes.
+            # This makes sure that we use "GH-Bedroom High East"
+            # instead of "GH-GH Bedroom High East"
+            # since it's sometimes convenient to have the short area
+            # at the start of the device name in vantage
+            if obj.name.startswith(name[0:-1]):
+                obj.name = name + obj.name[len(name):]
+            else:
+                obj.name = name + obj.name
 
         if obj.name in self._names:
             oldname = obj.name
-            obj.name += " (%s)" % (str(obj.vid))
+            obj.name += f" ({obj.vid})"
             if ('0-10V RELAYS' in oldname or
                 'NOT USED' in oldname or cmd_type == 'BTN'):
                 pass
             else:
-                _LOGGER.debug("Repeated name `%s' - adding vid to get %s",
-                              oldname, obj.name)
+                _LOGGER.debug(f"Repeated name `{oldname}' - adding vid to get {obj.name}")
         self._names[obj.name] = obj.vid
 
+
     # Note: invoked on VantageConnection thread.
     def _recv(self, line, i=0):
         """Invoked by the connection manager to process incoming data."""
-        _LOGGER.debug("#%s _recv got line: %s", i, line)
+        _LOGGER.debug(f"#{i} _recv got line: {line}")
         if line == '':
             return
         typ = None
         # Only handle query response messages, which are also sent on remote
         # status updates (e.g. user manually pressed a keypad button)
         if line[0] == 'R':
             cmds = self._r_cmds
@@ -1183,28 +1183,28 @@
             return
         if cmd_type == 'LOGIN':
             _LOGGER.info("#%s login successful", i)
             return
         # TODO: is it okay to ignore R:RAMPLOAD responses?
         # or do we need to handle_update_and_notify like with "LOAD",
         # below
-        if line[0] == 'R' and cmd_type in ('STATUS', 'ADDSTATUS',
+        if line[0] == 'R' and cmd_type in {'STATUS', 'ADDSTATUS',
                                            'DELSTATUS', 'INVOKE',
-                                           'GETCUSTOM', 'RAMPLOAD'):
+                                           'GETCUSTOM', 'RAMPLOAD'}:
             return
         if line[0] == 'R' and cmd_type == "ERROR":
             _LOGGER.warning("#%s Got %s on command: %s", i, line,
                             this_cmd)
             return
         # is there ever an S:ERROR line? that's all the below covers
         if cmd_type == 'ERROR':
             _LOGGER.error(" #%s _recv got ERROR line: %s", i, line)
             return
-        if cmd_type in ('GETLOAD', 'GETPOWER', 'GETCURRENT',
-                        'GETVARIABLE', 'GETSENSOR', 'GETLIGHT'):
+        if cmd_type in {'GETLOAD', 'GETPOWER', 'GETCURRENT',
+                        'GETVARIABLE', 'GETSENSOR', 'GETLIGHT'}:
             cmd_type = cmd_type[3:]  # strip "GET" from front
         elif cmd_type == 'GETBLIND':
             return
         elif cmd_type == 'TASK':
             return
         elif cmd_type == 'VARIABLE':
             _LOGGER.debug("#%s variable set response: %s", i, line)
@@ -1323,14 +1323,18 @@
                                 e)
         if not success:
             _LOGGER.info("doing request for vantage configuration file")
             if disable_cache:
                 _LOGGER.info("Vantage config cache is disabled.")
             ts = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             ts.connect((self._host, self._file_port))
+
+            if self._use_ssl:
+                ts = self._ssl_context.wrap_socket(ts)
+
             if self._user:
                 ts.send(("<ILogin><Login><call><User>%s</User>"
                          "<Password>%s</Password>"
                          "</call></Login></ILogin>\n"
                          % (escape(self._user),
                             escape(self._password))).encode("ascii"))
                 response = ""
@@ -1365,20 +1369,21 @@
                               " check username and password")
                 exit(-1)
             except socket.timeout:
                 ts.close()
             _LOGGER.debug("done reading, size = %s", len(response))
 
             response = response.decode('ascii')
-            response = response[response.find("</Result>\n")+10:]
-            response = response.replace('<?File Encode="Base64" /', '')
-            response = response.replace('?>', '')
-            response = response[:response.find('</return>')]
-            dbytes = base64.b64decode(response)
-            xml_db = dbytes.decode('utf-8')
+
+            # read XML preserving processing instructions
+            response = ET.fromstring(response, parser=ET.XMLParser(target=ET.TreeBuilder(insert_pis=True)))
+            response = response.find("GetFile/return")
+            response = next(response.iter(tag=ET.ProcessingInstruction))
+            response = response.text.split()[2][1:]
+            xml_db = base64.b64decode(response).decode('utf-8')
             if len(xml_db) < 1000:
                 _LOGGER.warning("Downloaded short .dc file; "
                                 " check saved cache file on disk")
             try:
                 f = open(filename, "w")
                 f.write(xml_db)
                 f.close()
@@ -1390,30 +1395,23 @@
         _LOGGER.info("Loaded xml db")
         # print(xml_db[0:10000])
         self.do_parse(xml_db)
 
     def do_parse(self, xml_db):
         """Call the parser and copy its output here."""
         parser = VantageXmlDbParser(vantage=self, xml_db_str=xml_db)
-        self._vid_to_load = parser.vid_to_load
-        self._vid_to_variable = parser.vid_to_variable
-        self._vid_to_area = parser.vid_to_area
-        self._vid_to_shade = parser.vid_to_shade
-        self._name = parser.project_name
-
         parser.parse()
         self.outputs = parser.outputs
         self.variables = parser.variables
         self.tasks = parser.tasks
         self.buttons = parser.buttons
         self.keypads = parser.keypads
         self.sensors = parser.sensors
         self._vid_to_load = parser.vid_to_load
         self._vid_to_variable = parser.vid_to_variable
-        self._vid_to_area = parser.vid_to_area
         self._vid_to_shade = parser.vid_to_shade
         self._vid_to_task = parser.vid_to_task
         self._vid_to_sensor = parser.vid_to_sensor
         self._name_to_task = parser.name_to_task
         self._name = parser.project_name
 
         _LOGGER.info("Found Vantage project: %s, %d areas, %d loads, "
@@ -1846,17 +1844,16 @@
             if self._rgb_is_dirty:
                 self._invoke_rgb()
             return
         # we need to adjust the rgb values to take into account the level
         _LOGGER.debug("%s: rgb = %s", self,
                       json.dumps(new_rgb))
         # INVOKE [vid] RGBLoad.SetRGBW [val0], [val1], [val2], [val3]
-        srgb = sRGBColor(*new_rgb)
-        hs_color = convert_color(srgb, HSVColor)
-        self._hs = [hs_color.hsv_h, hs_color.hsv_s * 100.0]
+        hs_color = rgb_to_hsv(*new_rgb)
+        self._hs = [hs_color[0] * 360.0, hs_color[1] * 100.0]
         self._rgb = new_rgb
         self._rgb_is_dirty = True
         if self._level > 0:
             self._invoke_rgb()
         else:
             self._invoke_hs()
 
@@ -1880,17 +1877,15 @@
     def hs(self, new_hs):
         """Sets new Hue/Saturation levels."""
         if self._hs == new_hs:
             return
         _LOGGER.debug("%s: hs = %s", self,
                       json.dumps(new_hs))
         self._hs = new_hs
-        hs_color = HSVColor(new_hs[0], new_hs[1]/100.0, 1.0)
-        rgb = convert_color(hs_color, sRGBColor)
-        self._rgb = [rgb.rgb_r, rgb.rgb_g, rgb.rgb_b]
+        self._rgb = list(hsv_to_rgb(new_hs[0]/360.0, new_hs[1]/100.0, 1.0))
         self._invoke_hs()
 
     def _invoke_hs(self):
         """Update the HS of the light to self._hsv
         It's worth noting that HS still specifies a color even when the light is off."""
         (h, s) = self._hs
         self._vantage.send("INVOKE", self._vid,
@@ -2217,15 +2212,18 @@
             else:
                 self._brightness_vid = self._load_vids[0]
         if self._brightness_vid:
             self._vantage._brightnessvid_to_group_vid[
                 self._brightness_vid] = self._vid
 
         for v in load_vids:
-            if self._vantage._vid_to_load[v]._is_dimmable:
+            load = self._vantage._vid_to_load.get(v)
+            if not load:
+                _LOGGER.warning("LoadGroup %s has unknown load vid %d", self, v)
+            if load and load._is_dimmable:
                 self._is_dimmable = True
                 break
 
     def support_color_temp(self):
         """Returns true iff this load can be set to a color temperature."""
         return self._support_color_temp
```

### Comparing `pyvantage-0.0.40/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.41/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.40
+Version: 0.0.41
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.40/setup.py` & `pyvantage-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.40',
+    version='0.0.41',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```

