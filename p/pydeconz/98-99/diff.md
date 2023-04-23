# Comparing `tmp/pydeconz-98.tar.gz` & `tmp/pydeconz-99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeconz-98.tar", last modified: Sat Jul  9 14:16:33 2022, max compression
+gzip compressed data, was "pydeconz-99.tar", last modified: Thu Jul 14 06:51:03 2022, max compression
```

## Comparing `pydeconz-98.tar` & `pydeconz-99.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.015281 pydeconz-98/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-07-09 14:16:25.000000 pydeconz-98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-09 14:16:33.015281 pydeconz-98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-09 14:16:25.000000 pydeconz-98/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.007281 pydeconz-98/pydeconz/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10456 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.011281 pydeconz-98/pydeconz/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/alarm_systems.py
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     8402 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/lights.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/scenes.py
--rw-r--r--   0 runner    (1001) docker     (121)    19972 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/interfaces/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.011281 pydeconz-98/pydeconz/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/alarm_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/deconz_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     9022 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.011281 pydeconz-98/pydeconz/models/light/
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/configuration_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/cover.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/fan.py
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/light.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/lock.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/range_extender.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/light/siren.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.015281 pydeconz-98/pydeconz/models/sensor/
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/air_quality.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/alarm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/ancillary_control.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/battery.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/carbon_monoxide.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/consumption.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/daylight.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/door_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/fire.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/generic_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/generic_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/humidity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/light_level.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/open_close.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/power.py
--rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/presence.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/relative_rotary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/temperature.py
--rw-r--r--   0 runner    (1001) docker     (121)    10596 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/vibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/models/sensor/water.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-07-09 14:16:25.000000 pydeconz-98/pydeconz/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 14:16:33.011281 pydeconz-98/pydeconz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-09 14:16:32.000000 pydeconz-98/pydeconz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-07-09 14:16:32.000000 pydeconz-98/pydeconz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 14:16:32.000000 pydeconz-98/pydeconz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-09 14:16:32.000000 pydeconz-98/pydeconz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-09 14:16:32.000000 pydeconz-98/pydeconz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-09 14:16:25.000000 pydeconz-98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-09 14:16:33.015281 pydeconz-98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-07-09 14:16:25.000000 pydeconz-98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.830111 pydeconz-99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-07-14 06:50:55.000000 pydeconz-99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-14 06:51:03.830111 pydeconz-99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-14 06:50:55.000000 pydeconz-99/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.810110 pydeconz-99/pydeconz/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10456 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.814110 pydeconz-99/pydeconz/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/alarm_systems.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/lights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/scenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20319 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/interfaces/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.818111 pydeconz-99/pydeconz/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/alarm_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/deconz_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9022 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.818111 pydeconz-99/pydeconz/models/light/
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/configuration_tool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/cover.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10985 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/light.py
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/range_extender.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/light/siren.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.830111 pydeconz-99/pydeconz/models/sensor/
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/ancillary_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/battery.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/carbon_monoxide.py
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/door_lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/fire.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/generic_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/generic_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/humidity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/light_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/presence.py
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/relative_rotary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/switch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10596 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/vibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/models/sensor/water.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-07-14 06:50:55.000000 pydeconz-99/pydeconz/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:51:03.814110 pydeconz-99/pydeconz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-14 06:51:03.000000 pydeconz-99/pydeconz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-07-14 06:51:03.000000 pydeconz-99/pydeconz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 06:51:03.000000 pydeconz-99/pydeconz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-14 06:51:03.000000 pydeconz-99/pydeconz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-14 06:51:03.000000 pydeconz-99/pydeconz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-14 06:50:55.000000 pydeconz-99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-14 06:51:03.830111 pydeconz-99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-07-14 06:50:55.000000 pydeconz-99/setup.py
```

### Comparing `pydeconz-98/LICENSE` & `pydeconz-99/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeconz-98/PKG-INFO` & `pydeconz-99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydeconz
-Version: 98
+Version: 99
 Summary: A Python library for communicating with deCONZ REST-API from Dresden Elektronik
 Home-page: https://github.com/Kane610/deconz
 Author: Robert Svensson
 Author-email: Kane610@users.noreply.github.com
 License: MIT
-Download-URL: https://github.com/Kane610/deconz/archive/v98.tar.gz
+Download-URL: https://github.com/Kane610/deconz/archive/v99.tar.gz
 Keywords: deconz,zigbee,homeassistant
 Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `pydeconz-98/README.rst` & `pydeconz-99/README.rst`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/__main__.py` & `pydeconz-99/pydeconz/__main__.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/config.py` & `pydeconz-99/pydeconz/config.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/errors.py` & `pydeconz-99/pydeconz/errors.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/gateway.py` & `pydeconz-99/pydeconz/gateway.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/interfaces/alarm_systems.py` & `pydeconz-99/pydeconz/interfaces/alarm_systems.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/interfaces/api.py` & `pydeconz-99/pydeconz/interfaces/api.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/interfaces/events.py` & `pydeconz-99/pydeconz/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/interfaces/groups.py` & `pydeconz-99/pydeconz/interfaces/groups.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/interfaces/lights.py` & `pydeconz-99/pydeconz/interfaces/lights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
-import enum
 import logging
 from typing import TYPE_CHECKING, Any, Union
 
 from ..models import ResourceGroup, ResourceType
 from ..models.light.configuration_tool import ConfigurationTool
 from ..models.light.cover import Cover, CoverAction
-from ..models.light.fan import Fan
-from ..models.light.light import Light, LightAlert, LightEffect
+from ..models.light.light import Light, LightAlert, LightEffect, LightFanSpeed
 from ..models.light.lock import Lock
 from ..models.light.range_extender import RangeExtender
 from ..models.light.siren import Siren
 from .api import APIItems, GroupedAPIItems
 
 if TYPE_CHECKING:
     from ..gateway import DeconzSession
 
 LOGGER = logging.getLogger(__name__)
 
 
-class FanSpeed(enum.Enum):
-    """Possible fan speeds."""
-
-    OFF = 0
-    PERCENT_25 = 1
-    PERCENT_50 = 2
-    PERCENT_75 = 3
-    PERCENT_100 = 4
-    AUTO = 5
-    COMFORT_BREEZE = 6
-
-
 class ConfigurationToolHandler(APIItems[ConfigurationTool]):
     """Handler for configuration tool."""
 
     resource_group = ResourceGroup.LIGHT
     resource_type = ResourceType.CONFIGURATION_TOOL
     item_cls = ConfigurationTool
 
@@ -85,45 +71,27 @@
         return await self.gateway.request_with_retry(
             "put",
             path=f"{self.path}/{id}/state",
             json=data,
         )
 
 
-class FanHandler(APIItems[Fan]):
-    """Handler for locks."""
-
-    resource_group = ResourceGroup.LIGHT
-    resource_type = ResourceType.FAN
-    item_cls = Fan
-
-    async def set_state(self, id: str, speed: FanSpeed) -> dict[str, Any]:
-        """Set speed of fans/ventilators.
-
-        Speed [FanSpeed] Off, 25%, 50%, 75%, 100%, Auto, ComfortBreeze.
-        """
-        return await self.gateway.request_with_retry(
-            "put",
-            path=f"{self.path}/{id}/state",
-            json={"speed": speed.value},
-        )
-
-
 class LightHandler(APIItems[Light]):
     """Handler for lights."""
 
     resource_group = ResourceGroup.LIGHT
     resource_types = {
         ResourceType.COLOR_DIMMABLE_LIGHT,
         ResourceType.COLOR_LIGHT,
         ResourceType.COLOR_TEMPERATURE_LIGHT,
         ResourceType.EXTENDED_COLOR_LIGHT,
         ResourceType.DIMMABLE_LIGHT,
         ResourceType.DIMMABLE_PLUGIN_UNIT,
         ResourceType.DIMMER_SWITCH,
+        ResourceType.FAN,
         ResourceType.ON_OFF_LIGHT,
         ResourceType.ON_OFF_OUTPUT,
         ResourceType.ON_OFF_PLUGIN_UNIT,
         ResourceType.SMART_PLUG,
         ResourceType.UNKNOWN,  # Legacy support
     }
     item_cls = Light
@@ -132,14 +100,15 @@
         self,
         id: str,
         alert: LightAlert | None = None,
         brightness: int | None = None,
         color_loop_speed: int | None = None,
         color_temperature: int | None = None,
         effect: LightEffect | None = None,
+        fan_speed: LightFanSpeed | None = None,
         hue: int | None = None,
         on: bool | None = None,
         on_time: int | None = None,
         saturation: int | None = None,
         transition_time: int | None = None,
         xy: tuple[float, float] | None = None,
     ) -> dict[str, Any]:
@@ -156,14 +125,15 @@
           - 15 is default
           - 255 very slow
         - color_temperature [int] between ctmin-ctmax
         - effect [str]
           - "none" no effect
           - "colorloop" the light will cycle continuously through all
                         colors with the speed specified by colorloopspeed
+        - fan_speed [FanSpeed] Off, 25%, 50%, 75%, 100%, Auto, ComfortBreeze
         - hue [int] 0-65535
         - on [bool] True/False
         - on_time [int] 0-65535 1/10 seconds resolution
         - saturation [int] 0-255
         - transition_time [int] 0-65535 1/10 seconds resolution
         - xy [tuple] (0-1, 0-1)
         """
@@ -182,14 +152,16 @@
             }.items()
             if value is not None
         }
         if alert is not None:
             data["alert"] = alert.value
         if effect is not None:
             data["effect"] = effect.value
+        if fan_speed is not None:
+            data["speed"] = fan_speed.value
         return await self.gateway.request_with_retry(
             "put",
             path=f"{self.path}/{id}/state",
             json=data,
         )
 
 
@@ -252,15 +224,14 @@
             json=data,
         )
 
 
 LightResources = Union[
     ConfigurationTool,
     Cover,
-    Fan,
     Light,
     Lock,
     Siren,
 ]
 
 
 class LightResourceManager(GroupedAPIItems[LightResources]):
@@ -268,24 +239,22 @@
 
     resource_group = ResourceGroup.LIGHT
 
     def __init__(self, gateway: DeconzSession) -> None:
         """Initialize light manager."""
         self.configuration_tool = ConfigurationToolHandler(gateway, grouped=True)
         self.covers = CoverHandler(gateway, grouped=True)
-        self.fans = FanHandler(gateway, grouped=True)
         self.lights = LightHandler(gateway, grouped=True)
         self.locks = LockHandler(gateway, grouped=True)
         self.range_extender = RangeExtenderHandler(gateway, grouped=True)
         self.sirens = SirenHandler(gateway, grouped=True)
 
         handlers: list[APIItems[Any]] = [
             self.configuration_tool,
             self.covers,
-            self.fans,
             self.lights,
             self.locks,
             self.range_extender,
             self.sirens,
         ]
 
         super().__init__(gateway, handlers)
```

### Comparing `pydeconz-98/pydeconz/interfaces/scenes.py` & `pydeconz-99/pydeconz/interfaces/scenes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, cast
 
 from ..models import ResourceGroup
 from ..models.event import EventType
 from ..models.scene import Scene
 from .api import APIItems
 
 
@@ -82,11 +82,8 @@
         self.process_item(group_id, {})
 
     def process_item(self, id: str, raw: dict[str, Any]) -> None:
         """Pre-process scene data."""
         group = self.gateway.groups[id]
 
         for scene in group.raw["scenes"]:
-            super().process_item(
-                f'{id}_{scene["id"]}',
-                scene | {"group_id": id, "group_name": group.name},
-            )
+            super().process_item(f'{id}_{scene["id"]}', cast(dict[str, Any], scene))
```

### Comparing `pydeconz-98/pydeconz/interfaces/sensors.py` & `pydeconz-99/pydeconz/interfaces/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ..models.sensor.daylight import Daylight
 from ..models.sensor.door_lock import DoorLock
 from ..models.sensor.fire import Fire
 from ..models.sensor.generic_flag import GenericFlag
 from ..models.sensor.generic_status import GenericStatus
 from ..models.sensor.humidity import Humidity
 from ..models.sensor.light_level import LightLevel
+from ..models.sensor.moisture import Moisture
 from ..models.sensor.open_close import OpenClose
 from ..models.sensor.power import Power
 from ..models.sensor.presence import (
     Presence,
     PresenceConfigDeviceMode,
     PresenceConfigTriggerDistance,
 )
@@ -283,14 +284,22 @@
         return await self.gateway.request_with_retry(
             "put",
             path=f"{self.path}/{id}/config",
             json=data,
         )
 
 
+class MoistureHandler(APIItems[Moisture]):
+    """Handler for moisture sensor."""
+
+    resource_group = ResourceGroup.SENSOR
+    resource_type = ResourceType.ZHA_MOISTURE
+    item_cls = Moisture
+
+
 class OpenCloseHandler(APIItems[OpenClose]):
     """Handler for open/close sensor."""
 
     resource_group = ResourceGroup.SENSOR
     resource_types = {
         ResourceType.ZHA_OPEN_CLOSE,
         ResourceType.CLIP_OPEN_CLOSE,
@@ -590,14 +599,15 @@
     Daylight,
     DoorLock,
     Fire,
     GenericFlag,
     GenericStatus,
     Humidity,
     LightLevel,
+    Moisture,
     OpenClose,
     Power,
     Presence,
     Pressure,
     RelativeRotary,
     Switch,
     Temperature,
@@ -627,14 +637,15 @@
         self.door_lock = DoorLockHandler(gateway, grouped=True)
         self.fire = FireHandler(gateway, grouped=True)
         self.generic_flag = GenericFlagHandler(gateway, grouped=True)
         self.generic_status = GenericStatusHandler(gateway, grouped=True)
         self.humidity = HumidityHandler(gateway, grouped=True)
         self.light_level = LightLevelHandler(gateway, grouped=True)
         self.open_close = OpenCloseHandler(gateway, grouped=True)
+        self.moisture = MoistureHandler(gateway, grouped=True)
         self.power = PowerHandler(gateway, grouped=True)
         self.presence = PresenceHandler(gateway, grouped=True)
         self.pressure = PressureHandler(gateway, grouped=True)
         self.relative_rotary = RelativeRotaryHandler(gateway, grouped=True)
         self.switch = SwitchHandler(gateway, grouped=True)
         self.temperature = TemperatureHandler(gateway, grouped=True)
         self.thermostat = ThermostatHandler(gateway, grouped=True)
@@ -653,14 +664,15 @@
             self.daylight,
             self.door_lock,
             self.fire,
             self.generic_flag,
             self.generic_status,
             self.humidity,
             self.light_level,
+            self.moisture,
             self.open_close,
             self.power,
             self.presence,
             self.pressure,
             self.relative_rotary,
             self.switch,
             self.temperature,
```

### Comparing `pydeconz-98/pydeconz/models/__init__.py` & `pydeconz-99/pydeconz/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,23 @@
     CONFIGURATION_TOOL = "Configuration tool"
 
     # Cover
     LEVEL_CONTROLLABLE_OUTPUT = "Level controllable output"
     WINDOW_COVERING_CONTROLLER = "Window covering controller"
     WINDOW_COVERING_DEVICE = "Window covering device"
 
-    # Fan
-    FAN = "Fan"
-
     # Light
     COLOR_DIMMABLE_LIGHT = "Color dimmable light"
     COLOR_LIGHT = "Color light"
     COLOR_TEMPERATURE_LIGHT = "Color temperature light"
     EXTENDED_COLOR_LIGHT = "Extended color light"
     DIMMABLE_LIGHT = "Dimmable light"
     DIMMABLE_PLUGIN_UNIT = "Dimmable plug-in unit"
     DIMMER_SWITCH = "Dimmer switch"
+    FAN = "Fan"
     ON_OFF_LIGHT = "On/Off light"
     ON_OFF_OUTPUT = "On/Off output"
     ON_OFF_PLUGIN_UNIT = "On/Off plug-in unit"
     SMART_PLUG = "Smart plug"
 
     # Lock
     DOOR_LOCK = "Door Lock"
@@ -106,14 +104,17 @@
     ZHA_HUMIDITY = "ZHAHumidity"
     CLIP_HUMIDITY = "CLIPHumidity"
 
     # Light level
     ZHA_LIGHT_LEVEL = "ZHALightLevel"
     CLIP_LIGHT_LEVEL = "CLIPLightLevel"
 
+    # Moisture
+    ZHA_MOISTURE = "ZHAMoisture"
+
     # Open close
     ZHA_OPEN_CLOSE = "ZHAOpenClose"
     CLIP_OPEN_CLOSE = "CLIPOpenClose"
 
     # Power
     ZHA_POWER = "ZHAPower"
```

### Comparing `pydeconz-98/pydeconz/models/alarm_system.py` & `pydeconz-99/pydeconz/models/alarm_system.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/api.py` & `pydeconz-99/pydeconz/models/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,14 @@
         self._request = request
 
         self.changed_keys: set[str] = set()
 
         self._callbacks: list[SubscriptionType] = []
         self._subscribers: list[SubscriptionType] = []
 
-        self.post_init()
-
-    def post_init(self) -> None:
-        """Post init method used by subclasses."""
-
     @property
     def deconz_id(self) -> str:
         """Id to call device over API e.g. /sensors/1."""
         return f"/{self.resource_group.value}/{self.resource_id}"
 
     def register_callback(self, callback: SubscriptionType) -> None:
         """Register callback for signalling."""
```

### Comparing `pydeconz-98/pydeconz/models/deconz_device.py` & `pydeconz-99/pydeconz/models/deconz_device.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/event.py` & `pydeconz-99/pydeconz/models/event.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/group.py` & `pydeconz-99/pydeconz/models/group.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/light/__init__.py` & `pydeconz-99/pydeconz/models/light/__init__.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/light/cover.py` & `pydeconz-99/pydeconz/models/light/cover.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
 import enum
-from typing import Any, TypedDict
+from typing import TypedDict
 
 from . import LightBase
 
 
 class TypedCoverState(TypedDict):
     """Cover state type definition."""
 
@@ -29,92 +29,46 @@
 
     CLOSE = enum.auto()
     OPEN = enum.auto()
     STOP = enum.auto()
 
 
 class Cover(LightBase):
-    """Cover and Damper class.
-
-    Position 0 means open and 100 means closed.
-    """
+    """Cover and Damper class."""
 
     raw: TypedCover
 
     @property
     def is_open(self) -> bool:
         """Is cover open."""
         if "open" not in self.raw["state"]:  # Legacy support
             return self.state is False
         return self.raw["state"]["open"]
 
     @property
     def lift(self) -> int:
         """Amount of closed position.
 
-        0 is fully open.
-        100 is fully closed.
+        Supported values:
+          0-100 - 0 is open / 100 is closed
         """
         if "lift" not in self.raw["state"]:  # Legacy support
             return int(self.raw["state"]["bri"] / 2.54)
         return self.raw["state"]["lift"]
 
     @property
     def tilt(self) -> int | None:
         """Amount of tilt.
 
-        0 is fully open.
-        100 is fully closed.
+        Supported values:
+          0-100 - 0 is open / 100 is closed
         """
         if "tilt" in self.raw["state"]:
             return self.raw["state"]["tilt"]
         elif "sat" in self.raw["state"]:  # Legacy support
             return int(self.raw["state"]["sat"] / 2.54)
         return None
 
-    async def set_position(
-        self, *, lift: int | None = None, tilt: int | None = None
-    ) -> dict[str, Any]:
-        """Set amount of closed position and/or tilt of cover.
-
-        Lift [int] between 0-100.
-        Scale to brightness 0-254.
-        Tilt [int] between 0-100.
-        Scale to saturation 0-254.
-        """
-        data = {}
-
-        if lift is not None:
-            if "lift" in self.raw["state"]:
-                data["lift"] = lift
-            elif "bri" in self.raw["state"]:  # Legacy support
-                data["bri"] = int(lift * 2.54)
-
-        if tilt is not None:
-            if "tilt" in self.raw["state"]:
-                data["tilt"] = tilt
-            elif "sat" in self.raw["state"]:  # Legacy support
-                data["sat"] = int(tilt * 2.54)
-
-        return await self.request(field=f"{self.deconz_id}/state", data=data)
-
-    async def open(self) -> dict[str, Any]:
-        """Fully open cover."""
-        data = {"open": True}
-        if "open" not in self.raw["state"]:  # Legacy support
-            data = {"on": False}
-        return await self.request(field=f"{self.deconz_id}/state", data=data)
-
-    async def close(self) -> dict[str, Any]:
-        """Fully close cover."""
-        data = {"open": False}
-        if "open" not in self.raw["state"]:  # Legacy support
-            data = {"on": True}
-        return await self.request(field=f"{self.deconz_id}/state", data=data)
-
-    async def stop(self) -> dict[str, Any]:
-        """Stop cover motion."""
-        data: dict[str, bool | int]
-        data = {"stop": True}
-        if "lift" not in self.raw["state"]:  # Legacy support
-            data = {"bri_inc": 0}
-        return await self.request(field=f"{self.deconz_id}/state", data=data)
+    @property
+    def supports_tilt(self) -> bool:
+        """Supports tilt."""
+        return "tilt" in self.raw["state"]
```

### Comparing `pydeconz-98/pydeconz/models/light/light.py` & `pydeconz-99/pydeconz/models/light/light.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "updown",
         "vintage",
         "waves",
     ]
     hue: int
     on: bool
     sat: int
+    speed: Literal[0, 1, 2, 3, 4, 5, 6]
     xy: tuple[float, float]
 
 
 class TypedLight(TypedDict):
     """Light type definition."""
 
     colorcapabilities: int
@@ -191,14 +192,36 @@
     @classmethod
     def _missing_(cls, value: object) -> "LightEffect":
         """Set default enum member if an unknown value is provided."""
         LOGGER.warning("Unexpected light effect type %s", value)
         return LightEffect.UNKNOWN
 
 
+class LightFanSpeed(enum.IntEnum):
+    """Possible fan speeds.
+
+    Supported values:
+    - 0 - fan is off
+    - 1 - 25%
+    - 2 - 50%
+    - 3 - 75%
+    - 4 - 100%
+    - 5 - Auto
+    - 6 - "comfort-breeze"
+    """
+
+    OFF = 0
+    PERCENT_25 = 1
+    PERCENT_50 = 2
+    PERCENT_75 = 3
+    PERCENT_100 = 4
+    AUTO = 5
+    COMFORT_BREEZE = 6
+
+
 class Light(LightBase):
     """deCONZ light representation.
 
     Dresden Elektroniks documentation of lights in deCONZ
     http://dresden-elektronik.github.io/deconz-rest-doc/lights/
     """
 
@@ -338,14 +361,24 @@
 
         colorloop — the light will cycle continuously through all colors
                     with the speed specified by colorloopspeed.
         none — no effect.
         """
         return self.raw["state"].get("effect")
 
+    @property
+    def fan_speed(self) -> LightFanSpeed:
+        """Speed of the fan."""
+        return LightFanSpeed(self.raw["state"]["speed"])
+
+    @property
+    def supports_fan_speed(self) -> bool:
+        """Speed of the fan."""
+        return True if "speed" in self.raw["state"] else False
+
     async def set_attributes(self, name: str) -> dict[str, Any]:
         """Change attributes of a light.
 
         Supported values:
         - name [str] The name of the light
         """
         data = {"name": name}
```

### Comparing `pydeconz-98/pydeconz/models/light/lock.py` & `pydeconz-99/pydeconz/models/light/lock.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/light/siren.py` & `pydeconz-99/pydeconz/models/light/siren.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/scene.py` & `pydeconz-99/pydeconz/models/sensor/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,60 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
-from collections.abc import Awaitable, Callable
-from typing import Any, TypedDict
+from .. import ResourceGroup
+from ..deconz_device import DeconzDevice
 
-from . import ResourceGroup
-from .api import APIItem
 
+class SensorBase(DeconzDevice):
+    """deCONZ sensor representation.
 
-class TypedScene(TypedDict):
-    """Scene type definition."""
-
-    id: str
-    lightcount: int
-    transitiontime: int
-    name: str
-
-
-class Scene(APIItem):
-    """deCONZ scene representation.
-
-    Dresden Elektroniks documentation of scenes in deCONZ
-    http://dresden-elektronik.github.io/deconz-rest-doc/scenes/
+    Dresden Elektroniks documentation of sensors in deCONZ
+    http://dresden-elektronik.github.io/deconz-rest-doc/sensors/
     """
 
-    raw: TypedScene
-    resource_group = ResourceGroup.SCENE
+    resource_group = ResourceGroup.SENSOR
 
-    def __init__(
-        self,
-        resource_id: str,
-        raw: Any,
-        request: Callable[..., Awaitable[dict[str, Any]]],
-    ) -> None:
-        """Set initial information about scene."""
-        super().__init__(resource_id, raw, request)
-
-        self.group_id: str = raw["group_id"]
-        self.group_deconz_id: str = f"/groups/{self.group_id}"
-        self.group_name: str = raw["group_name"]
-
-    async def store(self) -> dict[str, Any]:
-        """Store current group state in scene.
-
-        The actual state of each light in the group will become the lights scene state.
-        """
-        return await self.request(field=f"{self.deconz_id}/store", data={})
+    @property
+    def battery(self) -> int | None:
+        """Battery status of sensor."""
+        raw: dict[str, int] = self.raw["config"]
+        return raw.get("battery")
 
     @property
-    def deconz_id(self) -> str:
-        """Id to call scene over API e.g. /groups/1/scenes/1."""
-        return f"{self.group_deconz_id}/{self.resource_group.value}/{self.id}"
+    def ep(self) -> int | None:
+        """Endpoint of sensor."""
+        raw: dict[str, int] = self.raw
+        return raw.get("ep")
 
     @property
-    def id(self) -> str:
-        """Scene ID."""
-        return self.raw["id"]
+    def low_battery(self) -> bool | None:
+        """Low battery."""
+        raw: dict[str, bool] = self.raw["state"]
+        return raw.get("lowbattery")
 
     @property
-    def light_count(self) -> int:
-        """Lights in group."""
-        return self.raw["lightcount"]
+    def on(self) -> bool | None:
+        """Declare if the sensor is on or off."""
+        raw: dict[str, bool] = self.raw["config"]
+        return raw.get("on")
 
     @property
-    def transition_time(self) -> int:
-        """Transition time for scene."""
-        return self.raw["transitiontime"]
+    def reachable(self) -> bool:
+        """Declare if the sensor is reachable."""
+        raw: dict[str, bool] = self.raw["config"]
+        return raw.get("reachable", True)
 
     @property
-    def name(self) -> str:
-        """Scene name."""
-        return self.raw["name"]
+    def tampered(self) -> bool | None:
+        """Tampered."""
+        raw: dict[str, bool] = self.raw["state"]
+        return raw.get("tampered")
 
     @property
-    def full_name(self) -> str:
-        """Full name."""
-        return f"{self.group_name} {self.name}"
+    def secondary_temperature(self) -> float | None:
+        """Extra temperature available on some Xiaomi devices."""
+        raw: dict[str, int] = self.raw["config"]
+        if temperature := raw.get("temperature"):
+            return round(temperature / 100, 1)
+        return None
```

### Comparing `pydeconz-98/pydeconz/models/sensor/__init__.py` & `pydeconz-99/pydeconz/models/sensor/air_quality.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,91 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
-from .. import ResourceGroup
-from ..deconz_device import DeconzDevice
+import enum
+import logging
+from typing import Literal, TypedDict
 
+from . import SensorBase
 
-class SensorBase(DeconzDevice):
-    """deCONZ sensor representation.
+LOGGER = logging.getLogger(__name__)
 
-    Dresden Elektroniks documentation of sensors in deCONZ
-    http://dresden-elektronik.github.io/deconz-rest-doc/sensors/
+
+class TypedAirQualityState(TypedDict):
+    """Air quality state type definition."""
+
+    airquality: Literal[
+        "excellent",
+        "good",
+        "moderate",
+        "poor",
+        "unhealthy",
+        "out of scale",
+    ]
+    airqualityppb: int
+    pm2_5: int
+
+
+class TypedAirQuality(TypedDict):
+    """Air quality type definition."""
+
+    state: TypedAirQualityState
+
+
+class AirQualityValue(enum.Enum):
+    """Air quality.
+
+    Supported values:
+    - "excellent"
+    - "good"
+    - "moderate"
+    - "poor"
+    - "unhealthy"
+    - "out of scale"
     """
 
-    resource_group = ResourceGroup.SENSOR
+    EXCELLENT = "excellent"
+    GOOD = "good"
+    MODERATE = "moderate"
+    POOR = "poor"
+    UNHEALTHY = "unhealthy"
+    OUT_OF_SCALE = "out of scale"
 
-    @property
-    def battery(self) -> int | None:
-        """Battery status of sensor."""
-        raw: dict[str, int] = self.raw["config"]
-        return raw.get("battery")
+    UNKNOWN = "unknown"
 
-    @property
-    def ep(self) -> int | None:
-        """Endpoint of sensor."""
-        raw: dict[str, int] = self.raw
-        return raw.get("ep")
+    @classmethod
+    def _missing_(cls, value: object) -> "AirQualityValue":
+        """Set default enum member if an unknown value is provided."""
+        LOGGER.warning("Unexpected panel mode %s", value)
+        return AirQualityValue.UNKNOWN
+
+
+class AirQuality(SensorBase):
+    """Air quality sensor."""
+
+    raw: TypedAirQuality
 
     @property
-    def low_battery(self) -> bool | None:
-        """Low battery."""
-        raw: dict[str, bool] = self.raw["state"]
-        return raw.get("lowbattery")
+    def air_quality(self) -> str:  # AirQualityValue:
+        """Air quality."""
+        return AirQualityValue(self.raw["state"]["airquality"]).value
 
     @property
-    def on(self) -> bool | None:
-        """Declare if the sensor is on or off."""
-        raw: dict[str, bool] = self.raw["config"]
-        return raw.get("on")
+    def air_quality_ppb(self) -> int | None:
+        """Air quality PPB TVOC."""
+        return self.raw["state"].get("airqualityppb")
 
     @property
-    def reachable(self) -> bool:
-        """Declare if the sensor is reachable."""
-        raw: dict[str, bool] = self.raw["config"]
-        return raw.get("reachable", True)
+    def pm_2_5(self) -> int | None:
+        """Air quality PM2.5 (µg/m³)."""
+        return self.raw["state"].get("pm2_5")
 
     @property
-    def tampered(self) -> bool | None:
-        """Tampered."""
-        raw: dict[str, bool] = self.raw["state"]
-        return raw.get("tampered")
+    def supports_air_quality_ppb(self) -> bool:
+        """Support Air quality PPB reporting."""
+        return "airqualityppb" in self.raw["state"]
 
     @property
-    def secondary_temperature(self) -> float | None:
-        """Extra temperature available on some Xiaomi devices."""
-        raw: dict[str, int] = self.raw["config"]
-        if temperature := raw.get("temperature"):
-            return round(temperature / 100, 1)
-        return None
+    def supports_pm_2_5(self) -> bool:
+        """Support Air quality PM2.5 reporting."""
+        return "pm2_5" in self.raw["state"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydeconz-98/pydeconz/models/sensor/air_purifier.py` & `pydeconz-99/pydeconz/models/sensor/air_purifier.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/ancillary_control.py` & `pydeconz-99/pydeconz/models/sensor/ancillary_control.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/battery.py` & `pydeconz-99/pydeconz/models/sensor/battery.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/carbon_monoxide.py` & `pydeconz-99/pydeconz/models/sensor/carbon_monoxide.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/consumption.py` & `pydeconz-99/pydeconz/models/sensor/consumption.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/daylight.py` & `pydeconz-99/pydeconz/models/sensor/daylight.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/door_lock.py` & `pydeconz-99/pydeconz/models/sensor/door_lock.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/fire.py` & `pydeconz-99/pydeconz/models/sensor/fire.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/generic_flag.py` & `pydeconz-99/pydeconz/models/sensor/generic_flag.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/generic_status.py` & `pydeconz-99/pydeconz/models/sensor/generic_status.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/humidity.py` & `pydeconz-99/pydeconz/models/sensor/humidity.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/light_level.py` & `pydeconz-99/pydeconz/models/sensor/light_level.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/open_close.py` & `pydeconz-99/pydeconz/models/sensor/open_close.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/power.py` & `pydeconz-99/pydeconz/models/sensor/power.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/presence.py` & `pydeconz-99/pydeconz/models/sensor/presence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Python library to connect deCONZ and Home Assistant to work together."""
 
 from __future__ import annotations
 
 import enum
-from typing import Any, Final, Literal, TypedDict
+from typing import Final, Literal, TypedDict
 
 from . import SensorBase
 
 PRESENCE_DELAY: Final = "delay"
 PRESENCE_DURATION: Final = "duration"
 PRESENCE_SENSITIVITY: Final = "sensitivity"
 PRESENCE_SENSITIVITY_MAX: Final = "sensitivitymax"
@@ -177,31 +177,7 @@
 
     @property
     def trigger_distance(self) -> PresenceConfigTriggerDistance | None:
         """Device specific distance setting."""
         if "triggerdistance" in self.raw["config"]:
             return PresenceConfigTriggerDistance(self.raw["config"]["triggerdistance"])
         return None
-
-    async def set_config(
-        self,
-        delay: int | None = None,
-        duration: int | None = None,
-        sensitivity: int | None = None,
-    ) -> dict[str, Any]:
-        """Change config of presence sensor.
-
-        Supported values:
-        - delay [int] 0-65535 (in seconds)
-        - duration [int] 0-65535 (in seconds)
-        - sensitivity [int] 0-[sensitivitymax]
-        """
-        data = {
-            key: value
-            for key, value in {
-                "delay": delay,
-                "duration": duration,
-                "sensitivity": sensitivity,
-            }.items()
-            if value is not None
-        }
-        return await self.request(field=f"{self.deconz_id}/config", data=data)
```

### Comparing `pydeconz-98/pydeconz/models/sensor/pressure.py` & `pydeconz-99/pydeconz/models/sensor/pressure.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/relative_rotary.py` & `pydeconz-99/pydeconz/models/sensor/relative_rotary.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/switch.py` & `pydeconz-99/pydeconz/models/sensor/switch.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/temperature.py` & `pydeconz-99/pydeconz/models/sensor/temperature.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/thermostat.py` & `pydeconz-99/pydeconz/models/sensor/thermostat.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/models/sensor/vibration.py` & `pydeconz-99/pydeconz/models/sensor/vibration.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/utils.py` & `pydeconz-99/pydeconz/utils.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz/websocket.py` & `pydeconz-99/pydeconz/websocket.py`

 * *Files identical despite different names*

### Comparing `pydeconz-98/pydeconz.egg-info/PKG-INFO` & `pydeconz-99/pydeconz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydeconz
-Version: 98
+Version: 99
 Summary: A Python library for communicating with deCONZ REST-API from Dresden Elektronik
 Home-page: https://github.com/Kane610/deconz
 Author: Robert Svensson
 Author-email: Kane610@users.noreply.github.com
 License: MIT
-Download-URL: https://github.com/Kane610/deconz/archive/v98.tar.gz
+Download-URL: https://github.com/Kane610/deconz/archive/v99.tar.gz
 Keywords: deconz,zigbee,homeassistant
 Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `pydeconz-98/pydeconz.egg-info/SOURCES.txt` & `pydeconz-99/pydeconz.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 pydeconz/models/deconz_device.py
 pydeconz/models/event.py
 pydeconz/models/group.py
 pydeconz/models/scene.py
 pydeconz/models/light/__init__.py
 pydeconz/models/light/configuration_tool.py
 pydeconz/models/light/cover.py
-pydeconz/models/light/fan.py
 pydeconz/models/light/light.py
 pydeconz/models/light/lock.py
 pydeconz/models/light/range_extender.py
 pydeconz/models/light/siren.py
 pydeconz/models/sensor/__init__.py
 pydeconz/models/sensor/air_purifier.py
 pydeconz/models/sensor/air_quality.py
@@ -50,14 +49,15 @@
 pydeconz/models/sensor/daylight.py
 pydeconz/models/sensor/door_lock.py
 pydeconz/models/sensor/fire.py
 pydeconz/models/sensor/generic_flag.py
 pydeconz/models/sensor/generic_status.py
 pydeconz/models/sensor/humidity.py
 pydeconz/models/sensor/light_level.py
+pydeconz/models/sensor/moisture.py
 pydeconz/models/sensor/open_close.py
 pydeconz/models/sensor/power.py
 pydeconz/models/sensor/presence.py
 pydeconz/models/sensor/pressure.py
 pydeconz/models/sensor/relative_rotary.py
 pydeconz/models/sensor/switch.py
 pydeconz/models/sensor/temperature.py
```

### Comparing `pydeconz-98/setup.py` & `pydeconz-99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup for pydeCONZ."""
 
 from setuptools import find_packages, setup
 
 MIN_PY_VERSION = "3.9"
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
-VERSION = "98"
+VERSION = "99"
 
 setup(
     name="pydeconz",
     packages=PACKAGES,
     package_data={"pydeconz": ["py.typed"]},
     version=VERSION,
     description="A Python library for communicating with deCONZ REST-API from Dresden Elektronik",
```

