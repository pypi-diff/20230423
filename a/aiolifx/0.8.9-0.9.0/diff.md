# Comparing `tmp/aiolifx-0.8.9.tar.gz` & `tmp/aiolifx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolifx-0.8.9.tar", last modified: Thu Feb  9 13:37:03 2023, max compression
+gzip compressed data, was "aiolifx-0.9.0.tar", last modified: Sun Apr 23 10:55:01 2023, max compression
```

## Comparing `aiolifx-0.8.9.tar` & `aiolifx-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/
--rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-0.8.9/LICENSE.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-0.8.9/MANIFEST.in
--rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-09 13:37:03.513687 aiolifx-0.8.9/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)     3316 2022-09-29 07:38:39.000000 aiolifx-0.8.9/README.md
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/aiolifx/
--rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-0.8.9/aiolifx/__init__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    19095 2022-09-24 03:41:41.000000 aiolifx-0.8.9/aiolifx/__main__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    75045 2023-02-08 14:59:15.000000 aiolifx-0.8.9/aiolifx/aiolifx.py
--rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-0.8.9/aiolifx/connection.py
--rw-rw-r--   0 fw        (1000) fw        (1000)     6393 2021-05-03 10:41:06.000000 aiolifx-0.8.9/aiolifx/message.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    55837 2022-09-29 07:36:29.000000 aiolifx-0.8.9/aiolifx/msgtypes.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    30251 2023-02-09 13:33:52.000000 aiolifx-0.8.9/aiolifx/products.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    20159 2022-09-29 07:36:29.000000 aiolifx-0.8.9/aiolifx/unpack.py
--rwxrwxr-x   0 fw        (1000) fw        (1000)     1473 2022-04-26 14:59:59.000000 aiolifx-0.8.9/aiolifx/update-products.py
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/aiolifx.egg-info/
--rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)      455 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/SOURCES.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/dependency_links.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       50 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/entry_points.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/not-zip-safe
--rw-rw-r--   0 fw        (1000) fw        (1000)       17 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/requires.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        8 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/top_level.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       79 2023-02-09 13:37:03.513687 aiolifx-0.8.9/setup.cfg
--rw-rw-r--   0 fw        (1000) fw        (1000)     1205 2023-02-09 13:35:35.000000 aiolifx-0.8.9/setup.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-04-23 10:55:01.106212 aiolifx-0.9.0/
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-0.9.0/LICENSE.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-0.9.0/MANIFEST.in
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3945 2023-04-23 10:55:01.106212 aiolifx-0.9.0/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3476 2023-04-23 10:52:10.000000 aiolifx-0.9.0/README.md
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-04-23 10:55:01.106212 aiolifx-0.9.0/aiolifx/
+-rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-0.9.0/aiolifx/__init__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    25068 2023-04-23 10:52:10.000000 aiolifx-0.9.0/aiolifx/__main__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    85550 2023-04-23 10:52:01.000000 aiolifx-0.9.0/aiolifx/aiolifx.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-0.9.0/aiolifx/connection.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)     6392 2023-04-13 02:19:41.000000 aiolifx-0.9.0/aiolifx/message.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    66140 2023-04-23 10:52:01.000000 aiolifx-0.9.0/aiolifx/msgtypes.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    33282 2023-04-13 03:25:57.000000 aiolifx-0.9.0/aiolifx/products.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    25789 2023-04-23 10:52:01.000000 aiolifx-0.9.0/aiolifx/unpack.py
+-rwxrwxr-x   0 fw        (1000) fw        (1000)     1473 2022-04-26 14:59:59.000000 aiolifx-0.9.0/aiolifx/update-products.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-04-23 10:55:01.106212 aiolifx-0.9.0/aiolifx.egg-info/
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3945 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)      455 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       49 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/entry_points.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-04-23 10:55:00.000000 aiolifx-0.9.0/aiolifx.egg-info/not-zip-safe
+-rw-rw-r--   0 fw        (1000) fw        (1000)       83 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/requires.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        8 2023-04-23 10:55:01.000000 aiolifx-0.9.0/aiolifx.egg-info/top_level.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       79 2023-04-23 10:55:01.110212 aiolifx-0.9.0/setup.cfg
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1304 2023-04-23 10:52:10.000000 aiolifx-0.9.0/setup.py
```

### Comparing `aiolifx-0.8.9/LICENSE.txt` & `aiolifx-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.9/PKG-INFO` & `aiolifx-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 0.8.9
+Version: 0.9.0
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
@@ -117,10 +117,18 @@
 
     - I only have Original 1000, so I could not test with other types
       of bulbs
 
     - Unlike in lifxlan, set_waveform takes a dictionary with the right
       keys instead of all those parameters
 
+# Development
+## Running locally
+Run this command each time you make changes to the project. It enters at `__main__.py`
+
+```bash
+pip3 install . && aiolifx
+```
+
 # Thanks
 
 Thanks to Anders Melchiorsen and Avi Miller for their essential contributions
```

### Comparing `aiolifx-0.8.9/README.md` & `aiolifx-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,10 +102,18 @@
 
     - I only have Original 1000, so I could not test with other types
       of bulbs
 
     - Unlike in lifxlan, set_waveform takes a dictionary with the right
       keys instead of all those parameters
 
+# Development
+## Running locally
+Run this command each time you make changes to the project. It enters at `__main__.py`
+
+```bash
+pip3 install . && aiolifx
+```
+
 # Thanks
 
 Thanks to Anders Melchiorsen and Avi Miller for their essential contributions
```

### Comparing `aiolifx-0.8.9/aiolifx/aiolifx.py` & `aiolifx-0.9.0/aiolifx/aiolifx.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,50 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
 # IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE
 import asyncio as aio
+import logging
+from typing import Any, Coroutine, Set
 from .message import BROADCAST_MAC, BROADCAST_SOURCE_ID
 from .msgtypes import *
 from .products import *
 from .unpack import unpack_lifx_message
 from functools import partial
 from math import floor
 import time, random, datetime, socket, ifaddr
 
+# prevent tasks from being garbage collected
+_BACKGROUND_TASKS: Set[aio.Task] = set()
+
+if sys.version_info[:2] < (3, 11):
+    from async_timeout import timeout as asyncio_timeout
+else:
+    from asyncio import timeout as asyncio_timeout
 
 # A couple of constants
 LISTEN_IP = "0.0.0.0"
 UDP_BROADCAST_IP = "255.255.255.255"
 UDP_BROADCAST_PORT = 56700
 DEFAULT_TIMEOUT = 0.5  # How long to wait for an ack or response
 DEFAULT_ATTEMPTS = 3  # How many time shou;d we try to send to the bulb`
 DISCOVERY_INTERVAL = 180
 DISCOVERY_STEP = 5
+MAX_UNSIGNED_16_BIT_INTEGER_VALUE = int("0xFFFF", 16)
+_LOGGER = logging.getLogger(__name__)
+
+
+def _create_background_task(coro: Coroutine) -> None:
+    """Create a background task that will not be garbage collected."""
+    global _BACKGROUND_TASKS
+    task = aio.create_task(coro)
+    _BACKGROUND_TASKS.add(task)
+    task.add_done_callback(_BACKGROUND_TASKS.discard)
 
 
 def mac_to_ipv6_linklocal(mac, prefix="fe80::"):
     """Translate a MAC address into an IPv6 address in the prefixed network.
 
     This function calculates the EUI (Extended Unique Identifier) from the given
     MAC address and prepend the needed prefix to come up with a valid IPv6 address.
@@ -112,15 +131,15 @@
         self.timeout = DEFAULT_TIMEOUT
         self.unregister_timeout = DEFAULT_TIMEOUT
         self.transport = None
         self.task = None
         self.seq = 0
         # Key is the message sequence, value is (Response, Event, callb )
         self.message = {}
-        self.source_id = random.randint(0, (2 ** 32) - 1)
+        self.source_id = random.randint(0, (2**32) - 1)
         # Default callback for unexpected messages
         self.default_callb = None
         # And the rest
         self.label = None
         self.location = None
         self.group = None
         self.power_level = None
@@ -147,14 +166,33 @@
     #
 
     def connection_made(self, transport):
         """Method run when the connection to the lamp is established"""
         self.transport = transport
         self.register()
 
+    def error_received(self, exc: Exception) -> None:
+        """Method run when an error is received from the device.
+
+        This method is called in rare conditions, when the transport (e.g. UDP)
+        detects that a datagram could not be delivered to its recipient.
+        In many conditions though, undeliverable datagrams will be silently dropped.
+        """
+        _LOGGER.debug("%s: Error received: %s", self.ip_addr, exc)
+        # Clear the message queue since we know they are not going to be answered
+        # and there is no point in waiting for them
+        for entry in self.message.values():
+            response_type, myevent, callb = entry
+            if response_type != Acknowledgement:
+                if callb:
+                    callb(self, None)
+                if myevent:
+                    myevent.set()
+        self.message.clear()
+
     def datagram_received(self, data, addr):
         """Method run when data is received from the device
 
         This method will unpack the data according to the LIFX protocol.
         If the message represents some state information, it will update
         the device state. Following that it will execute the callback corresponding
         to the message sequence number. If there is no sequence number, the
@@ -267,15 +305,15 @@
             self.mac_addr,
             self.source_id,
             seq_num=0,
             payload=payload,
             ack_requested=False,
             response_requested=False,
         )
-        xx = self.loop.create_task(self.fire_sending(msg, num_repeats))
+        _create_background_task(self.fire_sending(msg, num_repeats))
         return True
 
     async def try_sending(self, msg, timeout_secs, max_attempts):
         """Coroutine used to send message to the device when a response or ack is needed.
 
         This coroutine will try to send up to max_attempts time the message, waiting timeout_secs
         for an answer. If no answer is received, it will consider that the device is no longer
@@ -301,15 +339,16 @@
                 return
             event = aio.Event()
             self.message[msg.seq_num][1] = event
             attempts += 1
             if self.transport:
                 self.transport.sendto(msg.packed_message)
             try:
-                myresult = await aio.wait_for(event.wait(), timeout_secs)
+                async with asyncio_timeout(timeout_secs):
+                    await event.wait()
                 break
             except Exception as inst:
                 if attempts >= max_attempts:
                     if msg.seq_num in self.message:
                         callb = self.message[msg.seq_num][2]
                         if callb:
                             callb(self, None)
@@ -341,15 +380,15 @@
             self.source_id,
             seq_num=self.seq_next(),
             payload=payload,
             ack_requested=True,
             response_requested=False,
         )
         self.message[msg.seq_num] = [Acknowledgement, None, callb]
-        xx = self.loop.create_task(self.try_sending(msg, timeout_secs, max_attempts))
+        _create_background_task(self.try_sending(msg, timeout_secs, max_attempts))
         return True
 
     # Usually used for Get messages, or for state confirmation after Set (hence the optional payload)
     def req_with_resp(
         self,
         msg_type,
         response_type,
@@ -380,15 +419,15 @@
             self.source_id,
             seq_num=self.seq_next(),
             payload=payload,
             ack_requested=False,
             response_requested=True,
         )
         self.message[msg.seq_num] = [response_type, None, callb]
-        xx = self.loop.create_task(self.try_sending(msg, timeout_secs, max_attempts))
+        _create_background_task(self.try_sending(msg, timeout_secs, max_attempts))
         return True
 
     # Not currently implemented, although the LIFX LAN protocol supports this kind of workflow natively
     def req_with_ack_resp(
         self,
         msg_type,
         response_type,
@@ -417,15 +456,15 @@
             self.source_id,
             seq_num=self.seq_next(),
             payload=payload,
             ack_requested=True,
             response_requested=True,
         )
         self.message[msg.seq_num] = [response_type, None, callb]
-        xx = self.loop.create_task(self.try_sending(msg, timeout_secs, max_attempts))
+        _create_background_task(self.try_sending(msg, timeout_secs, max_attempts))
         return True
 
     #
     #                            Attribute Methods
     #
     def get_label(self, callb=None):
         """Convenience method to request the label from the device
@@ -595,21 +634,25 @@
         mypartial = partial(self.resp_set_power, power_level=value)
         if callb:
             mycallb = lambda x, y: (mypartial(y), callb(x, y))
         else:
             mycallb = lambda x, y: mypartial(y)
         if value in on and not rapid:
             response = self.req_with_ack(
-                SetPower, {"power_level": 65535}, callb=mycallb
+                SetPower,
+                {"power_level": MAX_UNSIGNED_16_BIT_INTEGER_VALUE},
+                callb=mycallb,
             )
         elif value in off and not rapid:
             response = self.req_with_ack(SetPower, {"power_level": 0}, callb=mycallb)
         elif value in on and rapid:
-            response = self.fire_and_forget(SetPower, {"power_level": 65535})
-            self.power_level = 65535
+            response = self.fire_and_forget(
+                SetPower, {"power_level": MAX_UNSIGNED_16_BIT_INTEGER_VALUE}
+            )
+            self.power_level = MAX_UNSIGNED_16_BIT_INTEGER_VALUE
         elif value in off and rapid:
             response = self.fire_and_forget(SetPower, {"power_level": 0})
             self.power_level = 0
 
     def resp_set_power(self, resp, power_level=None):
         """Default callback for get_power/set_power"""
         if power_level is not None:
@@ -800,15 +843,15 @@
         )
         return s
 
     def device_product_str(self, indent):
         """Convenience to string method."""
         s = "Vendor: {}\n".format(self.vendor)
         s += indent + "Product: {}\n".format(
-            (self.product and product_map[self.product]) or "Unknown"
+            (self.product and products_dict[self.product]) or "Unknown"
         )
         s += indent + "Version: {}\n".format(self.version)
         return s
 
     def device_time_str(self, resp, indent="  "):
         """Convenience to string method."""
         time = resp.time
@@ -872,14 +915,22 @@
         self.color_zones = None
         self.zones_count = 1
         self.infrared_brightness = None
         self.hev_cycle = None
         self.hev_cycle_configuration = None
         self.last_hev_cycle_result = None
         self.effect = {"effect": None}
+        # Only used by a Lifx Switch. Will be populated with either True or False for each relay index if `get_rpower` called.
+        # At the moment we assume the switch to be 4 relays. This will likely work with the 2 relays switch as well, but only the first two values
+        # in this array will contain useful data.
+        self.relays_power = [None, None, None, None]
+        # Only used by a Lifx switch. Will be populated with an object containing the `haptic_duration_ms`, `backlight_on_color` and `backlight_off_color`
+        self.button_config = None
+        # Only used by a Lifx switch. Will be populated with an object containing `count`, `index`, `buttons_count` and `buttons`
+        self.button = None
 
     def get_power(self, callb=None):
         """Convenience method to request the power status from the device
 
         This method will check whether the value has already been retrieved from the device,
         if so, it will simply return it. If no, it will request the information from the device
         and request that callb be executed when a response is received. The default callback
@@ -912,15 +963,15 @@
             :type rapid: bool
             :returns: None
             :rtype: None
         """
         on = [True, 1, "on"]
         off = [False, 0, "off"]
         if value in on:
-            myvalue = 65535
+            myvalue = MAX_UNSIGNED_16_BIT_INTEGER_VALUE
         else:
             myvalue = 0
         mypartial = partial(self.resp_set_lightpower, power_level=myvalue)
         if callb:
             mycallb = lambda x, y: (mypartial(y), callb(x, y))
         else:
             mycallb = lambda x, y: mypartial(y)
@@ -1139,15 +1190,15 @@
 
     def set_multizone_effect(
         self, effect=0, speed=3, direction=0, callb=None, rapid=False
     ):
         """Convenience method to start or stop the Move firmware effect on multizone devices.
 
         Compatible devices include LIFX Z, Lightstrip and Beam and can be identified by
-        checking if features_map[device.product]['multizone'] is True. Multizone devices
+        checking if products_dict[device.product].multizone is True. Multizone devices
         only have one firmware effect named "MOVE". The effect can be started and stopped
         without the device being powered on. The effect will not be visible if the
         device is a single uniform color.
 
         Sending a set_power(0) to the device while the effect is running does not stop the effect.
         Physically powering off the device will stop the effect. And the device.
 
@@ -1424,15 +1475,15 @@
         This method will do nothing unless a call back is passed to it.
 
         :param callb: Callable to be used when the response is received.
         :type callb: callable
         :returns: None
         :rtype: None
         """
-        if features_map[self.product]["hev"] is True:
+        if products_dict[self.product].hev is True:
             self.req_with_resp(GetHevCycle, StateHevCycle, callb=callb)
 
     def resp_set_hevcycle(self, resp):
         """Default callback for get_hev_cycle/set_hev_cycle"""
         if resp:
             self.hev_cycle = {
                 "duration": resp.duration,
@@ -1456,15 +1507,15 @@
         :param callb: Callable to be used when the response is received.
         :type callb: callable
         :param rapid: Whether to ask for ack (False) or not (True). Default False
         :type rapid: bool
         :returns: None
         :rtype: None
         """
-        if features_map[self.product]["hev"] is True:
+        if products_dict[self.product].hev is True:
             if rapid:
                 self.fire_and_forget(
                     SetHevCycle,
                     {"enable": int(enable), "duration": duration},
                     num_repeats=1,
                 )
                 if callb:
@@ -1485,15 +1536,15 @@
         This method will do nothing unless a call back is passed to it.
 
         :param callb: Callable to be used when the response is received.
         :type callb: callable
         :returns: None
         :rtype: None
         """
-        if features_map[self.product]["hev"] is True:
+        if products_dict[self.product].hev is True:
             self.req_with_resp(
                 GetHevCycleConfiguration, StateHevCycleConfiguration, callb=callb
             )
 
     def resp_set_hevcycleconfiguration(self, resp):
         """Default callback for get_hev_cycle_configuration/set_hev_cycle_configuration"""
         if resp:
@@ -1518,15 +1569,15 @@
         :param callb: Callable to be used when the response is received.
         :type callb: callable
         :param rapid: Whether to ask for ack (False) or not (True). Default False
         :type rapid: bool
         :returns: None
         :rtype: None
         """
-        if features_map[self.product]["hev"] is True:
+        if products_dict[self.product].hev is True:
             if rapid:
                 self.fire_and_forget(
                     SetHevCycleConfiguration,
                     {"indication": int(indication), "duration": duration},
                     num_repeats=1,
                 )
                 if callb:
@@ -1548,15 +1599,15 @@
         This method will do nothing unless a call back is passed to it.
 
         :param callb: Callable to be used when the response is received.
         :type callb: callable
         :returns: None
         :rtype: None
         """
-        if features_map[self.product]["hev"] is True:
+        if products_dict[self.product].hev is True:
             self.req_with_resp(
                 GetLastHevCycleResult, StateLastHevCycleResult, callb=callb
             )
 
     def resp_set_lasthevcycleresult(self, resp):
         if resp:
             self.last_hev_cycle_result = LAST_HEV_CYCLE_RESULT.get(resp.result)
@@ -1645,14 +1696,227 @@
                     0.0
                     if resp.duration == 0
                     else float(f"{self.effect['duration']/1000000000:4f}")
                 )
                 self.effect["palette_count"] = resp.palette_count
                 self.effect["palette"] = resp.palette
 
+    def get_rpower(self, relay_index=None, callb=None):
+        """Method will get the power state of all relays; or a single relay if value provided.
+
+        :param relay_index: The index of the relay to check power state for. If not provided, will loop through 4 relays
+        :type relay_index: int
+        :param callb: Callable to be used when the response is received.
+        :type callb: callable
+        :returns: The cached value
+        :rtype: int
+        """
+        mypartial = partial(self.resp_set_rpower)
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        if relay_index is not None:
+            payload = {"relay_index": relay_index}
+            response = self.req_with_resp(
+                GetRPower, StateRPower, payload, callb=mycallb
+            )
+        else:
+            for relay_index in range(4):
+                payload = {"relay_index": relay_index}
+                response = self.req_with_resp(
+                    GetRPower, StateRPower, payload, callb=mycallb
+                )
+        return self.relays_power
+
+    def set_rpower(self, relay_index, is_on, callb=None, rapid=False):
+        """Sets relay power for a given relay index
+
+        :param relay_index: The relay on the switch starting from 0.
+        :type relay_index: int
+        :param on: Whether the relay is on or not
+        :type is_on: bool
+        :param callb: Callable to be used when the response is received.
+        :type callb: callable
+        :param rapid: Whether to ask for ack (False) or not (True). Default False
+        :type rapid: bool
+        :returns: None
+        :rtype: None
+        """
+        level = 0
+        if is_on:
+            level = MAX_UNSIGNED_16_BIT_INTEGER_VALUE
+
+        payload = {"relay_index": relay_index, "level": level}
+        mypartial = partial(self.resp_set_rpower, relay_index=relay_index, level=level)
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        if not rapid:
+            self.req_with_resp(SetRPower, StateRPower, payload, callb=mycallb)
+        else:
+            self.fire_and_forget(SetRPower, payload)
+
+    def resp_set_rpower(self, resp, relay_index=None, level=None):
+        """Default callback for get_rpower/set_rpower"""
+        if relay_index != None and level != None:
+            self.relays_power[relay_index] = level == MAX_UNSIGNED_16_BIT_INTEGER_VALUE
+        elif resp:
+            # Current models of the LIFX switch do not have dimming capability, so the two valid values are 0 for off (False) and 65535 for on (True).
+            self.relays_power[resp.relay_index] = (
+                resp.level == MAX_UNSIGNED_16_BIT_INTEGER_VALUE
+            )
+
+    def get_button(self, callb=None):
+        """Method will get the state of all buttons
+
+        :param relay_index: The index of the relay to check power state for. If not provided, will loop through 4 relays
+        :type relay_index: int
+        :param callb: Callable to be used when the response is received.
+        :type callb: callable
+        :returns: The cached value
+        :rtype: int
+        """
+        mypartial = partial(self.resp_get_button)
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        payload = {}
+        response = self.req_with_resp(GetButton, StateButton, payload, callb=mycallb)
+
+    def set_button(self, callb=None, rapid=False):
+        raise Exception(
+            "SetButton isn't yet implemented as you can only set button actions to the same values as the LIFX app (ie you can't add custom callbacks), making it not that useful. Feel free to implement if you need this :)"
+        )
+        """ Sets button
+
+            :param callb: Callable to be used when the response is received.
+            :type callb: callable
+            :param rapid: Whether to ask for ack (False) or not (True). Default False
+            :type rapid: bool
+            :returns: None
+            :rtype: None
+        """
+
+        payload = {}
+        mypartial = partial(self.resp_get_button)
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        if not rapid:
+            self.req_with_resp(SetButton, StateButton, payload, callb=mycallb)
+        else:
+            self.fire_and_forget(SetButton, payload)
+
+    def resp_get_button(self, resp):
+        """Default callback for get_button/set_button"""
+        self.button = {
+            "count": resp.count,
+            "index": resp.index,
+            "buttons_count": resp.buttons_count,
+            "buttons": resp.buttons,
+        }
+
+    def get_button_config(self, callb=None):
+        """Method will get the button config
+
+        :param callb: Callable to be used when the response is received.
+        :type callb: callable
+        :returns: The cached value
+        :rtype: int
+        """
+        mypartial = partial(self.resp_get_button_config)
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        response = self.req_with_resp(
+            GetButtonConfig, StateButtonConfig, {}, callb=mycallb
+        )
+
+    def set_button_config(
+        self,
+        haptic_duration_ms: int,
+        backlight_on_color,
+        backlight_off_color,
+        callb=None,
+        rapid=False,
+    ):
+        """Sets button config
+
+        :param haptic_duration_ms: How many milliseconds the haptic vibration when the button is pressed should last
+        :type haptic_duration_ms: int
+        :param backlight_on_color: The color the backlight should be when a button is on
+        :type backlight_on_color: { "hue": int, "saturation": int, "brightness": int, "kelvin": int }
+        :param backlight_off_color: The color the backlight should be when a button is off
+        :type backlight_off_color: { "hue": int, "saturation": int, "brightness": int, "kelvin": int }
+        :param callb: Callable to be used when the response is received.
+        :type callb: callable
+        :param rapid: Whether to ask for ack (False) or not (True). Default False
+        :type rapid: bool
+        :returns: None
+        :rtype: None
+        """
+
+        payload = {
+            "haptic_duration_ms": haptic_duration_ms,
+            "backlight_on_color": backlight_on_color,
+            "backlight_off_color": backlight_off_color,
+        }
+        mypartial = partial(
+            self.resp_get_button_config,
+            haptic_duration_ms=haptic_duration_ms,
+            backlight_on_color=backlight_on_color,
+            backlight_off_color=backlight_off_color,
+        )
+        if callb:
+            mycallb = lambda x, y: (mypartial(y), callb(x, y))
+        else:
+            mycallb = lambda x, y: mypartial(y)
+
+        if not rapid:
+            self.req_with_resp(
+                SetButtonConfig, StateButtonConfig, payload, callb=mycallb
+            )
+        else:
+            self.fire_and_forget(SetButtonConfig, payload)
+
+    def resp_get_button_config(
+        self,
+        resp,
+        haptic_duration_ms=None,
+        backlight_on_color=None,
+        backlight_off_color=None,
+    ):
+        """Default callback for get_button_config/set_button_config"""
+        if (
+            haptic_duration_ms != None
+            and backlight_on_color != None
+            and backlight_off_color != None
+        ):
+            self.button_config = {
+                "haptic_duration_ms": haptic_duration_ms,
+                "backlight_on_color": backlight_on_color,
+                "backlight_off_color": backlight_off_color,
+            }
+        elif resp:
+            self.button_config = {
+                "haptic_duration_ms": resp.haptic_duration_ms,
+                "backlight_on_color": resp.backlight_on_color,
+                "backlight_off_color": resp.backlight_off_color,
+            }
+
     def get_accesspoint(self, callb=None):
         """Convenience method to request the access point available
 
         This method will do nothing unless a call back is passed to it.
 
         :param callb: Callable to be used when the response is received. If not set,
                       self.resp_set_label will be used.
@@ -1707,28 +1971,28 @@
         broadcast_ip=UDP_BROADCAST_IP,
     ):
         self.lights = {}  # Known devices indexed by mac addresses
         self.parent = parent  # Where to register new devices
         self.transport = None
         self.loop = loop
         self.task = None
-        self.source_id = random.randint(0, (2 ** 32) - 1)
+        self.source_id = random.randint(0, (2**32) - 1)
         self.ipv6prefix = ipv6prefix
         self.discovery_interval = discovery_interval
         self.discovery_step = discovery_step
         self.discovery_countdown = 0
         self.broadcast_ip = broadcast_ip
 
     def start(self, listen_ip=LISTEN_IP, listen_port=0):
         """Start discovery task."""
         coro = self.loop.create_datagram_endpoint(
             lambda: self, local_addr=(listen_ip, listen_port)
         )
 
-        self.task = self.loop.create_task(coro)
+        self.task = aio.create_task(coro)
         return self.task
 
     def connection_made(self, transport):
         """Method run when the UDP broadcast server is started"""
         # print('started')
         self.transport = transport
         sock = self.transport.get_extra_info("socket")
@@ -1789,15 +2053,15 @@
             light = Light(self.loop, mac_addr, remote_ip, remote_port, parent=self)
             self.lights[mac_addr] = light
 
         coro = self.loop.create_datagram_endpoint(
             lambda: light, family=family, remote_addr=(remote_ip, remote_port)
         )
 
-        light.task = self.loop.create_task(coro)
+        light.task = aio.create_task(coro)
 
     def discover(self):
         """Method to send a discovery message"""
         if self.transport:
             if self.discovery_countdown <= 0:
                 self.discovery_countdown = self.discovery_interval
                 msg = GetService(
@@ -1862,15 +2126,15 @@
         tasks = []
         discoveries = []
         for ip in ips:
             manager = ScanManager(ip)
             lifx_discovery = LifxDiscovery(self.loop, manager)
             discoveries.append(lifx_discovery)
             lifx_discovery.start(listen_ip=ip)
-            tasks.append(self.loop.create_task(manager.lifx_ip()))
+            tasks.append(aio.create_task(manager.lifx_ip()))
 
         (done, pending) = await aio.wait(tasks, timeout=timeout)
 
         for discovery in discoveries:
             discovery.cleanup()
 
         for task in pending:
```

### Comparing `aiolifx-0.8.9/aiolifx/connection.py` & `aiolifx-0.9.0/aiolifx/connection.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.9/aiolifx/message.py` & `aiolifx-0.9.0/aiolifx/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         msg_type,
         target_addr,
         source_id,
         seq_num,
         ack_requested=False,
         response_requested=False,
     ):
-
         # Frame
         self.frame_format = ["<H", "<H", "<L"]
         self.size = None  # 16 bits/uint16
         self.origin = 0  # 2 bits/uint8, must be zero
         self.tagged = (
             1 if target_addr == BROADCAST_MAC else 0
         )  # 1 bit/bool, also must be one if getservice
```

### Comparing `aiolifx-0.8.9/aiolifx/msgtypes.py` & `aiolifx-0.9.0/aiolifx/msgtypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1829,14 +1829,278 @@
         for color in self.palette:
             payload += b"".join(
                 little_endian(bitstring.pack("uint:16", field)) for field in color
             )
         return payload
 
 
+##### RELAY (SWITCH) MESSAGES #####
+##### https://lan.developer.lifx.com/docs/the-lifx-switch #####
+
+
+class GetRPower(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload={},
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.relay_index = payload["relay_index"]
+        super(GetRPower, self).__init__(
+            MSG_IDS[GetRPower],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+    def get_payload(self):
+        self.payload_fields.append(("Relay Index", self.relay_index))
+        relay_index = little_endian(bitstring.pack("uint:8", self.relay_index))
+        payload = relay_index
+        return payload
+
+
+class SetRPower(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.relay_index = payload["relay_index"]
+        self.level = payload["level"]
+        super(SetRPower, self).__init__(
+            MSG_IDS[SetRPower],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+    def get_payload(self):
+        self.payload_fields.append(("Relay Index", self.relay_index))
+        self.payload_fields.append(("Level", self.level))
+        relay_index = little_endian(bitstring.pack("uint:8", self.relay_index))
+        level = little_endian(bitstring.pack("uint:16", self.level))
+        payload = relay_index + level
+        return payload
+
+
+class StateRPower(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.relay_index = payload["relay_index"]
+        self.level = payload["level"]
+        super(StateRPower, self).__init__(
+            MSG_IDS[StateRPower],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+    def get_payload(self):
+        self.payload_fields.append(("Relay Index", self.relay_index))
+        self.payload_fields.append(("Level", self.level))
+        relay_index = little_endian(bitstring.pack("uint:8", self.relay_index))
+        level = little_endian(bitstring.pack("uint:32", self.level))
+        payload = relay_index + level
+        return payload
+
+
+##### SWITCH BUTTON MESSAGES #####
+##### https://github.com/LIFX/public-protocol/blob/main/protocol.yml#L472-L541 #####
+
+
+class GetButton(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload={},
+        ack_requested=False,
+        response_requested=False,
+    ):
+        super(GetButton, self).__init__(
+            MSG_IDS[GetButton],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+
+class SetButton(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        super(SetButton, self).__init__(
+            MSG_IDS[SetButton],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+        raise Exception("Not implemented")
+
+    def get_payload(self):
+        raise Exception("Not implemented")
+
+
+class StateButton(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.count = payload["count"]
+        self.index = payload["index"]
+        self.buttons_count = payload["buttons_count"]
+        self.buttons = payload["buttons"]
+        super(StateButton, self).__init__(
+            MSG_IDS[StateButton],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+
+class GetButtonConfig(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload={},
+        ack_requested=False,
+        response_requested=False,
+    ):
+        super(GetButtonConfig, self).__init__(
+            MSG_IDS[GetButtonConfig],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+
+class SetButtonConfig(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.haptic_duration_ms = payload["haptic_duration_ms"]
+        self.backlight_on_color = payload["backlight_on_color"]
+        self.backlight_off_color = payload["backlight_off_color"]
+        super(SetButtonConfig, self).__init__(
+            MSG_IDS[SetButtonConfig],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+    def get_payload(self):
+        self.payload_fields.append(("haptic_duration_ms", self.haptic_duration_ms))
+        self.payload_fields.append(("backlight_on_color", self.backlight_on_color))
+        self.payload_fields.append(("backlight_off_color", self.backlight_off_color))
+        haptic_duration_ms = little_endian(
+            bitstring.pack("uint:16", self.haptic_duration_ms)
+        )
+
+        hue = self.backlight_on_color["hue"]
+        saturation = self.backlight_on_color["saturation"]
+        brightness = self.backlight_on_color["brightness"]
+        kelvin = self.backlight_on_color["kelvin"]
+
+        backlight_on_color = (
+            little_endian(bitstring.pack("uint:16", hue))
+            + little_endian(bitstring.pack("uint:16", saturation))
+            + little_endian(bitstring.pack("uint:16", brightness))
+            + little_endian(bitstring.pack("uint:16", kelvin))
+        )
+
+        hue = self.backlight_off_color["hue"]
+        saturation = self.backlight_off_color["saturation"]
+        brightness = self.backlight_off_color["brightness"]
+        kelvin = self.backlight_off_color["kelvin"]
+
+        backlight_off_color = (
+            little_endian(bitstring.pack("uint:16", hue))
+            + little_endian(bitstring.pack("uint:16", saturation))
+            + little_endian(bitstring.pack("uint:16", brightness))
+            + little_endian(bitstring.pack("uint:16", kelvin))
+        )
+
+        payload = haptic_duration_ms + backlight_on_color + backlight_off_color
+        return payload
+
+
+class StateButtonConfig(Message):
+    def __init__(
+        self,
+        target_addr,
+        source_id,
+        seq_num,
+        payload,
+        ack_requested=False,
+        response_requested=False,
+    ):
+        self.haptic_duration_ms = payload["haptic_duration_ms"]
+        self.backlight_on_color = payload["backlight_on_color"]
+        self.backlight_off_color = payload["backlight_off_color"]
+        super(StateButtonConfig, self).__init__(
+            MSG_IDS[StateButtonConfig],
+            target_addr,
+            source_id,
+            seq_num,
+            ack_requested,
+            response_requested,
+        )
+
+
 MSG_IDS = {
     GetService: 2,
     StateService: 3,
     GetHostInfo: 12,
     StateHostInfo: 13,
     GetHostFirmware: 14,
     StateHostFirmware: 15,
@@ -1890,14 +2154,23 @@
     MultiZoneStateMultiZoneEffect: 509,
     MultiZoneSetExtendedColorZones: 510,
     MultiZoneGetExtendedColorZones: 511,
     MultiZoneStateExtendedColorZones: 512,
     TileGetTileEffect: 718,
     TileSetTileEffect: 719,
     TileStateTileEffect: 720,
+    GetRPower: 816,
+    SetRPower: 817,
+    StateRPower: 818,
+    GetButton: 905,
+    SetButton: 906,
+    StateButton: 907,
+    GetButtonConfig: 909,
+    SetButtonConfig: 910,
+    StateButtonConfig: 911,
 }
 
 SERVICE_IDS = {1: "UDP", 2: "reserved", 3: "reserved", 4: "reserved"}
 
 STR_MAP = {65535: "On", 0: "Off", None: "Unknown"}
 
 ZONE_MAP = {0: "NO_APPLY", 1: "APPLY", 2: "APPLY_ONLY"}
@@ -1909,14 +2182,95 @@
     3: "INTERRUPTED_BY_HOMEKIT",
     4: "INTERRUPTED_BY_LAN",
     5: "INTERRUPTED_BY_CLOUD",
     255: "NONE",
 }
 
 
+class Button:
+    def __init__(self, data):
+        self.actions = []
+        self.actions_count = data[0]
+        for i in range(0, self.actions_count):
+            self.actions.append(ButtonAction(data[1 + i * 20 : 1 + (i + 1) * 20]))
+
+    def get_payload(self):
+        payload = little_endian(bitstring.pack("uint:8", self.actions_count))
+        for action in self.actions:
+            payload += action.get_payload()
+        return payload
+
+
+class ButtonAction:
+    def __init__(self, data):
+        self.gesture = ButtonGesture(data[0] + data[1] * 256)
+        self.target_type = ButtonTargetType(data[2] + data[3] * 256)
+        if self.target_type == ButtonTargetType.RELAYS:
+            self.target = ButtonTargetRelays(data[4:])
+        elif self.target_type == ButtonTargetType.DEVICE:
+            self.target = ButtonTargetDevice(data[4:])
+        elif self.target_type == ButtonTargetType.DEVICE_RELAYS:
+            self.target = ButtonTargetDeviceRelays(data[4:])
+        else:
+            self.target = None
+
+    def get_payload(self):
+        payload = little_endian(bitstring.pack("uint:16", self.gesture.value))
+        payload += little_endian(bitstring.pack("uint:16", self.target_type.value))
+        if self.target_type == ButtonTargetType.RELAYS:
+            payload += little_endian(bitstring.pack("uint:8", self.target.relays_count))
+            for relay in self.target.relays:
+                payload += little_endian(bitstring.pack("uint:8", relay))
+        elif self.target_type == ButtonTargetType.DEVICE:
+            payload += self.target.serial
+            payload += self.target.reserved
+        elif self.target_type == ButtonTargetType.DEVICE_RELAYS:
+            payload += self.target.serial
+            payload += little_endian(bitstring.pack("uint:8", self.target.relays_count))
+            for relay in self.target.relays:
+                payload += little_endian(bitstring.pack("uint:8", relay))
+        return payload
+
+
+class ButtonTargetRelays:
+    def __init__(self, data):
+        self.relays_count = data[0]
+        self.relays = data[1 : 1 + self.relays_count]
+
+
+class ButtonTargetDevice:
+    def __init__(self, data):
+        self.serial = data[0:6]
+        self.reserved = data[6:16]
+
+
+class ButtonTargetDeviceRelays:
+    def __init__(self, data):
+        self.serial = data[0:6]
+        self.relays_count = data[6]
+        self.relays = data[7 : 7 + self.relays_count]
+
+
+class ButtonGesture(Enum):
+    PRESS = 1
+    HOLD = 2
+    PRESS_PRESS = 3
+    PRESS_HOLD = 4
+    HOLD_HOLD = 5
+
+
+class ButtonTargetType(Enum):
+    RELAYS = 2
+    DEVICE = 3
+    LOCATION = 4
+    GROUP = 5
+    SCENE = 6
+    DEVICE_RELAYS = 7
+
+
 class MultiZoneEffectType(Enum):
     OFF = 0
     MOVE = 1
     RESERVED1 = 2
     RESERVED2 = 3
```

### Comparing `aiolifx-0.8.9/aiolifx/products.py` & `aiolifx-0.9.0/aiolifx/products.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 product_map = {
     1: "LIFX Original 1000",
     3: "LIFX Color 650",
     10: "LIFX White 800 (Low Voltage)",
     11: "LIFX White 800 (High Voltage)",
     15: "LIFX Color 1000",
     18: "LIFX White 900 BR30 (Low Voltage)",
@@ -1244,7 +1246,95 @@
         "matrix": True,
         "max_kelvin": 9000,
         "min_kelvin": 1500,
         "multizone": False,
         "relays": False,
     },
 }
+
+
+class Product:
+    def __init__(
+        self,
+        id: int,
+        name: str,
+        buttons: bool,
+        chain: bool,
+        color: bool,
+        extended_multizone: bool,
+        hev: bool,
+        infrared: bool,
+        matrix: bool,
+        multizone: bool,
+        relays: bool,
+        max_kelvin: int,
+        min_kelvin: int,
+        min_ext_mz_firmware: int,
+        min_ext_mz_firmware_components: List[int],
+        temperature_range: None,
+    ):
+        self.id = id
+        self.name = name
+        self.buttons = buttons
+        self.chain = chain
+        self.color = color
+        self.extended_multizone = extended_multizone
+        self.hev = hev
+        self.infrared = infrared
+        self.matrix = matrix
+        self.multizone = multizone
+        self.relays = relays
+        self.max_kelvin = max_kelvin
+        self.min_kelvin = min_kelvin
+        self.min_ext_mz_firmware = min_ext_mz_firmware
+        self.min_ext_mz_firmware_components = min_ext_mz_firmware_components
+        self.temperature_range = temperature_range
+
+    def __str__(self):
+        return (
+            f"Product(id={self.id}, "
+            f"name='{self.name}', "
+            f"buttons={self.buttons}, "
+            f"chain={self.chain}, "
+            f"color={self.color}, "
+            f"extended_multizone={self.extended_multizone}, "
+            f"hev={self.hev}, "
+            f"infrared={self.infrared}, "
+            f"matrix={self.matrix}, "
+            f"multizone={self.multizone}, "
+            f"relays={self.relays}, "
+            f"max_kelvin={self.max_kelvin}, "
+            f"min_kelvin={self.min_kelvin}, "
+            f"min_ext_mz_firmware={self.min_ext_mz_firmware}, "
+            f"min_ext_mz_firmware_components={self.min_ext_mz_firmware_components}, "
+            f"temperature_range={self.temperature_range})"
+        )
+
+
+def create_product_dict(product_map, features_map):
+    products_dict = {}
+    for product_id, product_name in product_map.items():
+        features = features_map[product_id]
+        products_dict[product_id] = Product(
+            id=product_id,
+            name=product_name,
+            buttons=features.get("buttons"),
+            chain=features.get("chain"),
+            color=features.get("color"),
+            extended_multizone=features.get("extended_multizone"),
+            hev=features.get("hev"),
+            infrared=features.get("infrared"),
+            matrix=features.get("matrix"),
+            multizone=features.get("multizone"),
+            relays=features.get("relays"),
+            max_kelvin=features.get("max_kelvin"),
+            min_kelvin=features.get("min_kelvin"),
+            min_ext_mz_firmware=features.get("min_ext_mz_firmware"),
+            min_ext_mz_firmware_components=features.get(
+                "min_ext_mz_firmware_components"
+            ),
+            temperature_range=features.get("temperature_range"),
+        )
+    return products_dict
+
+
+products_dict = create_product_dict(product_map, features_map)
```

### Comparing `aiolifx-0.8.9/aiolifx/update-products.py` & `aiolifx-0.9.0/aiolifx/update-products.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.9/aiolifx.egg-info/PKG-INFO` & `aiolifx-0.9.0/aiolifx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 0.8.9
+Version: 0.9.0
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
@@ -117,10 +117,18 @@
 
     - I only have Original 1000, so I could not test with other types
       of bulbs
 
     - Unlike in lifxlan, set_waveform takes a dictionary with the right
       keys instead of all those parameters
 
+# Development
+## Running locally
+Run this command each time you make changes to the project. It enters at `__main__.py`
+
+```bash
+pip3 install . && aiolifx
+```
+
 # Thanks
 
 Thanks to Anders Melchiorsen and Avi Miller for their essential contributions
```

### Comparing `aiolifx-0.8.9/setup.py` & `aiolifx-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 import setuptools
 
-version = "0.8.9"
+version = "0.9.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiolifx",
     packages=["aiolifx"],
@@ -16,22 +16,25 @@
     description="API for local communication with LIFX devices over a LAN with asyncio.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/frawau/aiolifx",
     keywords=["lifx", "light", "automation"],
     license="MIT",
     install_requires=[
+        "async_timeout>=3.0.1",
         "bitstring",
         "ifaddr",
+        'click>=8.1.0,<8.2.0',
+        'InquirerPy>=0.3.0,<0.4.0'
     ],
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3",
     ],
-    entry_points={"console_scripts": ["aiolifx=aiolifx.__main__:main"]},
+    entry_points={"console_scripts": ["aiolifx = aiolifx.__main__:cli"]},
     python_requires=">=3.4",
     zip_safe=False,
 )
```

