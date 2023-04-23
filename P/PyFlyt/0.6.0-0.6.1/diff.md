# Comparing `tmp/PyFlyt-0.6.0.tar.gz` & `tmp/PyFlyt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.6.0.tar", last modified: Wed Apr 12 14:05:24 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.1.tar", last modified: Sun Apr 23 21:26:28 2023, max compression
```

## Comparing `PyFlyt-0.6.0.tar` & `PyFlyt-0.6.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     8851 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.0/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.0/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7626 2023-04-12 13:36:46.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11784 2023-04-12 01:16:04.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4211 2023-04-12 01:15:08.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7686 2023-04-12 01:27:48.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6365 2023-04-11 23:16:18.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12428 2023-04-12 01:36:15.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4651 2023-04-11 23:13:32.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15163 2023-04-12 14:05:07.000000 PyFlyt-0.6.0/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.0/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9602 2023-04-12 13:37:24.000000 PyFlyt-0.6.0/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18116 2023-04-12 13:37:02.000000 PyFlyt-0.6.0/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11668 2023-04-12 13:37:20.000000 PyFlyt-0.6.0/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.0/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5510 2023-04-07 22:18:42.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3531 2023-03-13 17:50:16.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5733 2023-04-07 22:18:54.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     8772 2023-04-12 13:57:31.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.0/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.0/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-02 23:08:08.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8851 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       57 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1184 2023-04-12 14:05:16.000000 PyFlyt-0.6.0/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     7034 2023-04-08 01:06:54.000000 PyFlyt-0.6.0/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.0/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.0/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-12 01:51:05.000000 PyFlyt-0.6.0/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.1/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8847 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.1/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.1/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-23 00:11:20.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4277 2023-04-12 15:03:07.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7239 2023-04-23 20:15:04.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15014 2023-04-12 15:29:07.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.1/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15536 2023-04-23 00:13:01.000000 PyFlyt-0.6.1/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.1/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.1/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    17954 2023-04-12 14:34:19.000000 PyFlyt-0.6.1/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11506 2023-04-12 14:34:51.000000 PyFlyt-0.6.1/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.1/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.1/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.1/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.1/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.1/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.1/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.129101 PyFlyt-0.6.1/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8847 2023-04-23 21:26:28.000000 PyFlyt-0.6.1/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-23 21:26:28.000000 PyFlyt-0.6.1/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-23 21:26:28.000000 PyFlyt-0.6.1/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       57 2023-04-23 21:26:28.000000 PyFlyt-0.6.1/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-23 21:26:28.000000 PyFlyt-0.6.1/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1184 2023-04-23 21:26:14.000000 PyFlyt-0.6.1/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7030 2023-04-12 17:54:58.000000 PyFlyt-0.6.1/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.1/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-23 21:26:28.133101 PyFlyt-0.6.1/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.1/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.1/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.6.0/LICENSE.txt` & `PyFlyt-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PKG-INFO` & `PyFlyt-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.0
+Version: 0.6.1
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -204,15 +204,15 @@
 ```
 
 > `angle_representation` can be either `"quaternion"` or `"euler"`.
 >
 > `render_mode` can be either `"human"` or `rgb_array` or `None`.
 
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/fixedwing_waypoint.gif?raw=true" width="500px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/rocket_landing.gif?raw=true" width="500px"/>
 </p>
 
 ## Citation
 
 If you use our work in your research and would like to cite it, please use the following bibtex entry:
 
 ```
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/boosters.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.ratio_fuel_rate = self.max_fuel_rate / self.total_fuel_mass
         self.noise_ratio = noise_ratio
 
     def reset(self, starting_fuel_ratio: float | np.ndarray = 1.0):
         """Reset the boosters.
 
         Args:
-            starting_fuel_ratio (float | np.ndarray): ratio amount of fuel that the booster is reset to
+            starting_fuel_ratio (float | np.ndarray): ratio amount of fuel that the booster is reset to.
         """
         # deal with everything in percents
         self.ratio_fuel_remaining = (
             np.ones((self.num_boosters,), dtype=np.float64) * starting_fuel_ratio
         )
         self.throttle = np.zeros((self.num_boosters,), dtype=np.float64)
         self.ignition_state = np.zeros((self.num_boosters,), dtype=bool)
@@ -147,17 +147,17 @@
 
     def physics_update(
         self, ignition: np.ndarray, pwm: np.ndarray, rotation: None | np.ndarray = None
     ):
         """Converts booster settings into forces on the booster and inertia change on fuel tank.
 
         Args:
-            ignition (np.ndarray): (num_boosters,) array of booleans for engine on or off
-            pwm (np.ndarray): (num_boosters,) array of floats between [0, 1] for min or max thrust
-            rotation (np.ndarray): (num_boosters, 3, 3) rotation matrices to rotate each booster's thrust axis around
+            ignition (np.ndarray): (num_boosters,) array of booleans for engine on or off.
+            pwm (np.ndarray): (num_boosters,) array of floats between [0, 1] for min or max thrust.
+            rotation (np.ndarray): (num_boosters, 3, 3) rotation matrices to rotate each booster's thrust axis around, this is readily obtained from the `gimbals` component.
         """
         assert np.all(ignition >= 0.0) and np.all(
             ignition <= 1.0
         ), f"{ignition=} has values out of bounds of 0.0 and 1.0."
         assert np.all(pwm >= 0.0) and np.all(
             pwm <= 1.0
         ), f"{pwm=} has values out of bounds of 0.0 and 1.0."
@@ -200,16 +200,16 @@
                 localInertiaDiagonal=inertia[i],
             )
 
     def _compute_thrust_mass_inertia(self, ignition: np.ndarray, pwm: np.ndarray):
         """_compute_thrust_mass_inertia.
 
         Args:
-            ignition (np.ndarray): (num_boosters,) array of booleans for engine on or off
-            pwm (np.ndarray): (num_boosters,) array of floats between [0, 1] for min or max thrust
+            ignition (np.ndarray): (num_boosters,) array of booleans for engine on or off.
+            pwm (np.ndarray): (num_boosters,) array of floats between [0, 1] for min or max thrust.
         """
         # if not reignitable, logical or ignition_state with ignition
         # otherwise, just follow ignition
         self.ignition_state = ((not self.reignitable) & self.ignition_state) | (
             ignition > 0.5
         )
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A component to simulate bodies moving through the air."""
 from __future__ import annotations
 
-import warnings
+from typing import Sequence
 
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class BoringBodies:
     """Vectorized implementation of a series of plain bodies affected by aerodynamics.
@@ -13,39 +13,39 @@
     The `BoringBodies` component is used to represent a normal body moving through the air.
 
     Args:
         p (bullet_client.BulletClient): PyBullet physics client ID.
         physics_period (float): physics period of the simulation.
         np_random (np.random.RandomState): random number generator of the simulation.
         uav_id (int): ID of the drone.
-        body_ids (np.ndarray): (n,) array of IDs for the links representing the bodies
-        drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions
-        normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions
+        body_ids (np.ndarray | Sequence[int]): (n,) array of IDs for the links representing the bodies.
+        drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions.
+        normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions.
     """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         physics_period: float,
         np_random: np.random.RandomState,
         uav_id: int,
-        body_ids: np.ndarray,
+        body_ids: np.ndarray | Sequence[int],
         drag_coefs: np.ndarray,
         normal_areas: np.ndarray,
     ):
         """Used for simulating a body moving through the air.
 
         Args:
             p (bullet_client.BulletClient): PyBullet physics client ID.
             physics_period (float): physics period of the simulation.
             np_random (np.random.RandomState): random number generator of the simulation.
             uav_id (int): ID of the drone.
-            body_ids (np.ndarray): (n,) array of IDs for the links representing the bodies
-            drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions
-            normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions
+            body_ids (np.ndarray | Sequence[int]): (n,) array of IDs for the links representing the bodies.
+            drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions.
+            normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions.
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         # store IDs
         self.uav_id = uav_id
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     The camera itself can be gimballed to achieve a horizon lock effect.
     In addition, the field-of-view (FOV), tilt angle, resolution, and offset distance from the main link can be adjusted.
     On image capture, the camera returns an RGBA image, a depth map, and a segmentation map with pixel values representing the IDs of objects in the environment.
 
     Args:
         p (bullet_client.BulletClient): PyBullet physics client ID.
         uav_id (int): ID of the drone.
-        camera_id (int): integer representing the ID of the link that the camera is attached to
-        use_gimbal (bool): whether to lock the horizon of the camera
-        camera_FOV_degrees (float): the field-of-view of the camera in degrees
-        camera_angle_degrees (float): when gimballed, this is the angle of downtilt from horizon; when not gimballed, this is theh angle of uptile from horizon
-        camera_resolution (tuple[int, int]): the resolution of the camera in terms of [width, height]
-        camera_position_offset (np.ndarray = np.array([0.0, 0.0, 0.0])): an (3,) array representing an offset of where the camera is from the center of the link in `camera_id`
-        is_tracking_camera (bool = False): if the camera is a tracking camera, the focus point of the camera is adjusted to focus on the center body of the aircraft instead of at infinity
-        cinematic (bool = False): it's not a bug, it's a feature
+        camera_id (int): integer representing the ID of the link that the camera is attached to.
+        use_gimbal (bool): whether to lock the horizon of the camera.
+        camera_FOV_degrees (float): the field-of-view of the camera in degrees.
+        camera_angle_degrees (float): when gimballed, this is the angle of downtilt from horizon; when not gimballed, this is theh angle of uptile from horizon.
+        camera_resolution (tuple[int, int]): the resolution of the camera in terms of [width, height].
+        camera_position_offset (np.ndarray = np.array([0.0, 0.0, 0.0])): an (3,) array representing an offset of where the camera is from the center of the link in `camera_id`.
+        is_tracking_camera (bool = False): if the camera is a tracking camera, the focus point of the camera is adjusted to focus on the center body of the aircraft instead of at infinity.
+        cinematic (bool = False): it's not a bug, it's a feature.
     """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         uav_id: int,
         camera_id: int,
@@ -43,22 +43,22 @@
         cinematic: bool = False,
     ):
         """Used for implementing camera modules.
 
         Args:
             p (bullet_client.BulletClient): PyBullet physics client ID.
             uav_id (int): ID of the drone.
-            camera_id (int): integer representing the ID of the link that the camera is attached to
-            use_gimbal (bool): whether to lock the horizon of the camera
-            camera_FOV_degrees (float): the field-of-view of the camera in degrees
-            camera_angle_degrees (float): when gimballed, this is the angle of downtilt from horizon; when not gimballed, this is theh angle of uptile from horizon
-            camera_resolution (tuple[int, int]): the resolution of the camera in terms of [width, height]
-            camera_position_offset (np.ndarray = np.array([0.0, 0.0, 0.0])): an (3,) array representing an offset of where the camera is from the center of the link in `camera_id`
-            is_tracking_camera (bool = False): if the camera is a tracking camera, the focus point of the camera is adjusted to focus on the center body of the aircraft instead of at infinity
-            cinematic (bool = False): it's not a bug, it's a feature
+            camera_id (int): integer representing the ID of the link that the camera is attached to.
+            use_gimbal (bool): whether to lock the horizon of the camera.
+            camera_FOV_degrees (float): the field-of-view of the camera in degrees.
+            camera_angle_degrees (float): when gimballed, this is the angle of downtilt from horizon; when not gimballed, this is theh angle of uptile from horizon.
+            camera_resolution (tuple[int, int]): the resolution of the camera in terms of [width, height].
+            camera_position_offset (np.ndarray = np.array([0.0, 0.0, 0.0])): an (3,) array representing an offset of where the camera is from the center of the link in `camera_id`.
+            is_tracking_camera (bool = False): if the camera is a tracking camera, the focus point of the camera is adjusted to focus on the center body of the aircraft instead of at infinity.
+            cinematic (bool = False): it's not a bug, it's a feature.
         """
         if is_tracking_camera and use_gimbal:
             warnings.warn(
                 "Use_gimbal and is_tracking_camera are both enabled. This will lead to funky behaviour."
             )
 
         # grab the pybullet client instance and relevant IDs
@@ -87,15 +87,15 @@
         self.cinematic = cinematic
 
     @property
     def view_mat(self) -> np.ndarray:
         """Generates the view matrix for the camera depending on the current orientation and implicit parameters.
 
         Returns:
-            np.ndarray: view matrix
+            np.ndarray: view matrix.
         """
         # get the state of the camera on the robot
         camera_state = self.p.getLinkState(self.uav_id, self.camera_id)
 
         # pose and rot depends on offset if any
         position = np.array(camera_state[0])
         if self.has_camera_offset:
@@ -127,17 +127,17 @@
         return self.p.computeViewMatrix(
             cameraEyePosition=position,
             cameraTargetPosition=target,
             cameraUpVector=up_vector,
         )
 
     def get_states(self):
-        """This does not need to be called for camera. Call `capture_image()` instead within `update_avionics()`."""
+        """This does not need to be called for camera. Call `capture_image()` instead within `update_last()`."""
         warnings.warn(
-            "This does not need to be called for camera. Call `capture_image()` instead within `update_avionics()`."
+            "This does not need to be called for camera. Call `capture_image()` instead within `update_last()`."
         )
 
     def state_update(self):
         """This does not need to be called for camera."""
         warnings.warn("`state_update` does not need to be called for camera.")
 
     def physics_update(self):
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/gimbals.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,36 +4,49 @@
 import warnings
 
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class Gimbals:
-    """Gimbals."""
+    """A set of actuated gimbals.
+
+    The `Gimbals` component simulates a series of servo actuated gimbals.
+    Each gimbal can rotate about two arbitrary axis that may not be orthogonal to each other.
+
+    Args:
+        p (bullet_client.BulletClient): PyBullet physics client ID.
+        physics_period (float): physics period of the simulation.
+        np_random (np.random.RandomState): random number generator of the simulation.
+        gimbal_unit_1 (np.ndarray): first unit vector that the gimbal rotates around.
+        gimbal_unit_2 (np.ndarray): second unit vector that the gimbal rotates around.
+        gimbal_tau (np.ndarray): gimbal actuation time constant.
+        gimbal_range_degrees (np.ndarray): gimbal actuation range in degrees.
+    """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         physics_period: float,
         np_random: np.random.RandomState,
         gimbal_unit_1: np.ndarray,
         gimbal_unit_2: np.ndarray,
         gimbal_tau: np.ndarray,
         gimbal_range_degrees: np.ndarray,
     ):
         """Used for simulating an array of gimbals.
 
         Args:
-            p (bullet_client.BulletClient): p
-            physics_period (float): physics_period
-            np_random (np.random.RandomState): np_random
-            gimbal_unit_1 (np.ndarray): first unit vector that the gimbal rotates around
-            gimbal_unit_2 (np.ndarray): second unit vector that the gimbal rotates around
-            gimbal_tau (np.ndarray): gimbal ramp time constant
-            gimbal_range_degrees (np.ndarray): gimbal_range_degrees
+            p (bullet_client.BulletClient): PyBullet physics client ID.
+            physics_period (float): physics period of the simulation.
+            np_random (np.random.RandomState): random number generator of the simulation.
+            gimbal_unit_1 (np.ndarray): first unit vector that the gimbal rotates around.
+            gimbal_unit_2 (np.ndarray): second unit vector that the gimbal rotates around.
+            gimbal_tau (np.ndarray): gimbal actuation time constant.
+            gimbal_range_degrees (np.ndarray): gimbal actuation range in degrees.
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         assert (
             len(gimbal_unit_1.shape) == 2 and gimbal_unit_1.shape[-1] == 3
@@ -123,37 +136,38 @@
             "`state_update` does not need to be called for gimbals, call `compute_rotation` instead."
         )
 
     def compute_rotation(self, gimbal_command) -> np.ndarray:
         """Returns a rotation vector after the gimbal rotation.
 
         Args:
-            gimbal_command (np.ndarray): (num_gimbals, 2) array of floats between [-1, 1]
+            gimbal_command (np.ndarray): (num_gimbals, 2) array of floats between [-1, 1].
 
         Returns:
-            rotation_vector (np.ndarray): (num_gimbals, 3, 3) rotation matrices for all gimbals
+            rotation_vector (np.ndarray): (num_gimbals, 3, 3) rotation matrices for all gimbals.
         """
         assert np.all(gimbal_command >= -1.0) and np.all(
             gimbal_command <= 1.0
         ), f"`{gimbal_command=} has values out of bounds of -1.0 and 1.0.`"
 
         # model the gimbal using first order ODE, y' = T/tau * (setpoint - y)
         self.gimbal_state += (self.physics_period / self.gimbal_tau) * (
             gimbal_command - self.gimbal_state
         )
-        gimbal_angles = self.gimbal_state * self.gimbal_range_radians
-
         # start calculating rotation matrices
         # https://math.stackexchange.com/questions/142821/matrix-for-rotation-around-a-vector
+        sin_angles = np.expand_dims(
+            np.sin(self.gimbal_state * self.gimbal_range_radians), axis=(-1, -2)
+        )
         rotation1 = (
             np.eye(3)
-            + np.sin(gimbal_angles[:, 0]) * self.w1
-            + 2 * (np.sin(gimbal_angles[:, 0]) ** 2) * self.w1_squared
+            + sin_angles[:, 0, ...] * self.w1
+            + 2 * (sin_angles[:, 0, ...] ** 2) * self.w1_squared
         )
         rotation2 = (
             np.eye(3)
-            + np.sin(gimbal_angles[:, 1]) * self.w2
-            + 2 * (np.sin(gimbal_angles[:, 1]) ** 2) * self.w2_squared
+            + sin_angles[:, 1, ...] * self.w2
+            + 2 * (sin_angles[:, 1, ...] ** 2) * self.w2_squared
         )
 
         # get the final thrust vector
         return rotation1 @ rotation2
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,28 @@
 import warnings
 
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class LiftingSurfaces:
-    """Handler for multiple lifting surfaces."""
+    """Handler for multiple lifting surfaces.
+
+    This is a convenience class for handling multiple lifting surfaces as a single object.
+    Simply pass it a list of `LiftingSurface` objects.
+
+    Args:
+        lifting_surfaces (list[LiftingSurface]): a list of `LiftingSurface` objects.
+    """
 
     def __init__(self, lifting_surfaces: list[LiftingSurface]):
         """__init__.
 
         Args:
-            lifting_surfaces (list[LiftingSurface]): lifting_surfaces
+            lifting_surfaces (list[LiftingSurface]): a list of `LiftingSurface` objects.
         """
         # assert all is lifting surfaces
         assert all(
             [isinstance(surface, LiftingSurface) for surface in lifting_surfaces]
         )
 
         # store some stuff
@@ -39,15 +46,15 @@
         """
         return np.array([surface.actuation for surface in self.surfaces])
 
     def physics_update(self, cmd: np.ndarray):
         """Converts actuation commands into forces on the lifting surfaces.
 
         Args:
-            cmd (np.ndarray): the full command array, command mapping is handled through `command_id` and `command_sign` on each surface.
+            cmd (np.ndarray): the full command array, command mapping is handled through `command_id` and `command_sign` on each surface, normalized in [-1, 1].
         """
         assert np.all(cmd >= -1.0) and np.all(
             cmd <= 1.0
         ), f"`{cmd=} has values out of bounds of -1.0 and 1.0.`"
 
         for surface in self.surfaces:
             actuation = (
@@ -77,15 +84,40 @@
 
         # update the velocities of all surfaces
         for surface, velocity in zip(self.surfaces, surface_velocities):
             surface.state_update(velocity)
 
 
 class LiftingSurface:
-    """LiftingSurface."""
+    """Used to represent a single lifting surface.
+
+    The `Lifting Surface` component is used to simulate a single lifting surface based on "Real-time modeling of agile fixed-wing uav aerodynamics, Khan et. al.".
+
+    Args:
+        p (bullet_client.BulletClient): PyBullet physics client ID.
+        physics_period (float): physics period of the simulation.
+        np_random (np.random.RandomState): random number generator of the simulation.
+        uav_id (int): ID of the drone.
+        surface_id (int): an integer for the link ID for this lifting surface.
+        command_id (None | int): the index of the command array that corresponds to an actuation of this lifting surface.
+        command_sign (float): the sign of the command to actuate this lifting surface.
+        lifting_unit (np.ndarray): (3,) unit vector representing the direction of lift.
+        forward_unit (np.ndarray): (3,) unit vector representing the direction of travel.
+        Cl_alpha_2D (float): lift coefficient slope under a no-stall condition.
+        chord (float): chord of the lifting surface.
+        span (float): span of the lifting surface.
+        flap_to_chord (float): ratio of the wing that is an actuated flap, can be in [0, 1].
+        eta (float): correction factor for viscosity effects, usually 0.65.
+        alpha_0_base (float): zero lift angle-of-attack.
+        alpha_stall_P_base (float): positive stall angle in degrees.
+        alpha_stall_N_base (float): negative stall angle in degrees.
+        Cd_0 (float): drag coefficient at zero angle-of-attack.
+        deflection_limit (float): maximum deflection limit of the actuated flap in degrees.
+        tau (float): actuation ramp time constant.
+    """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         physics_period: float,
         np_random: np.random.RandomState,
         uav_id: int,
@@ -105,34 +137,34 @@
         Cd_0: float,
         deflection_limit: float,
         tau: float,
     ):
         """Used for simulating a single lifting surface.
 
         Args:
-            p (bullet_client.BulletClient): p
-            physics_period (float): physics_period
-            np_random (np.random.RandomState): np_random
-            uav_id (int): uav_id
-            surface_id (int): surface_id
-            command_id (None | int): command_id, for convenience
-            command_sign (float): command_sign, for convenience
-            lifting_unit (np.ndarray): (3,) unit vector representing the direction of lift
-            forward_unit (np.ndarray): (3,) unit vector representing the direction of travel
-            Cl_alpha_2D (float): float
-            chord (float): float
-            span (float): float
-            flap_to_chord (float): float
-            eta (float): float
-            alpha_0_base (float): float
-            alpha_stall_P_base (float): float
-            alpha_stall_N_base (float): float
-            Cd_0 (float): float
-            deflection_limit (float): float
-            tau (float): float
+            p (bullet_client.BulletClient): PyBullet physics client ID.
+            physics_period (float): physics period of the simulation.
+            np_random (np.random.RandomState): random number generator of the simulation.
+            uav_id (int): ID of the drone.
+            surface_id (int): an integer for the link ID for this lifting surface.
+            command_id (None | int): the index of the command array that corresponds to an actuation of this lifting surface.
+            command_sign (float): the sign of the command to actuate this lifting surface.
+            lifting_unit (np.ndarray): (3,) unit vector representing the direction of lift.
+            forward_unit (np.ndarray): (3,) unit vector representing the direction of travel.
+            Cl_alpha_2D (float): lift coefficient slope under a no-stall condition.
+            chord (float): chord of the lifting surface.
+            span (float): span of the lifting surface.
+            flap_to_chord (float): ratio of the wing that is an actuated flap, can be in [0, 1].
+            eta (float): correction factor for viscosity effects, usually 0.65.
+            alpha_0_base (float): zero lift angle-of-attack.
+            alpha_stall_P_base (float): positive stall angle in degrees.
+            alpha_stall_N_base (float): negative stall angle in degrees.
+            Cd_0 (float): drag coefficient at zero angle-of-attack.
+            deflection_limit (float): maximum deflection limit of the actuated flap in degrees.
+            tau (float): actuation ramp time constant.
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         # store IDs
         self.uav_id = uav_id
@@ -206,23 +238,23 @@
         """
         return self.actuation
 
     def state_update(self, surface_velocity: np.ndarray):
         """Updates the local surface velocity of the lifting surface.
 
         Args:
-            surface_velocity (np.ndarray): surface_velocity
+            surface_velocity (np.ndarray): surface_velocity.
         """
         self.local_surface_velocity = surface_velocity
 
     def physics_update(self, cmd: float):
         """Converts a commanded actuation state into forces on the lifting surface.
 
         Args:
-            cmd (float): normalized actuation in [-1, 1]
+            cmd (float): normalized actuation in [-1, 1].
 
         Returns:
             tuple[np.ndarray, np.ndarray]: vec3 force, vec3 torque
         """
         freestream_speed = np.linalg.norm(self.local_surface_velocity)
         lifting_airspeed = np.dot(self.local_surface_velocity, self.lift_unit)
         forward_airspeed = np.dot(self.local_surface_velocity, self.drag_unit)
@@ -256,16 +288,16 @@
             self.uav_id, self.surface_id, torque, self.p.LINK_FRAME
         )
 
     def _compute_aero_data(self, alpha: float) -> tuple[float, float, float]:
         """Computes the relevant aerodynamic data depending on the current state of the lifting surface.
 
         Args:
-            deflection (float): deflection of the lifting surface in degrees
-            alpha (float): angle of attack in degrees
+            deflection (float): deflection of the lifting surface in degrees.
+            alpha (float): angle of attack in degrees.
 
         Returns:
             tuple[float, float, float]: Cl, Cd, CM
         """
         # deflection must be in degrees because engineering uses degrees
         deflection_radians = np.deg2rad(self.actuation * self.deflection_limit)
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.1/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/core/aviary.py` & `PyFlyt-0.6.1/PyFlyt/core/aviary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
 from __future__ import annotations
 
 import time
 from itertools import repeat
 from typing import Any, Sequence
+from warnings import warn
 
 import numpy as np
 import pybullet as p
 import pybullet_data
 from pybullet_utils import bullet_client
 
 from .abstractions import DroneClass
@@ -25,29 +26,27 @@
     Args:
         start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
         start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
         drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
         drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
         drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
         render (bool): a boolean whether to render the simulation.
-        render_FPS (int): the FPS for rendering, this helps the scheduler.
         physics_hz (int): physics looprate (not recommended to be changed).
         worldScale (float): how big to spawn the floor.
         seed (None | int): optional int for seeding the simulation RNG.
     """
 
     def __init__(
         self,
         start_pos: np.ndarray,
         start_orn: np.ndarray,
         drone_type: str | Sequence[str],
         drone_type_mappings: None | dict[str, DroneClass] = None,
         drone_options: dict[str, Any] | Sequence[dict[str, Any]] = {},
         render: bool = False,
-        render_FPS: int = 60,
         physics_hz: int = 240,
         worldScale: float = 1.0,
         seed: None | int = None,
     ):
         """Initializes a PyBullet environment that hosts UAVs and other entities.
 
         The Aviary class itself inherits from a BulletClient, so any function that a PyBullet client has, this class will have.
@@ -56,15 +55,14 @@
         Args:
             start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
             start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
             drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
             drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
             drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
             render (bool): a boolean whether to render the simulation.
-            render_FPS (int): the FPS for rendering, this helps the scheduler.
             physics_hz (int): physics looprate (not recommended to be changed).
             worldScale (float): how big to spawn the floor.
             seed (None | int): optional int for seeding the simulation RNG.
         """
         super().__init__(p.GUI if render else p.DIRECT)
         print("\033[A                             \033[A")
 
@@ -75,14 +73,20 @@
         assert (
             start_pos.shape[-1] == 3
         ), f"start_pos must be shape (n, 3), currently {start_pos.shape}."
         assert (
             start_orn.shape == start_pos.shape
         ), f"start_orn must be same shape as start_pos, currently {start_orn.shape}."
 
+        # check the physics hz
+        if physics_hz != 240.0:
+            warn(
+                f"Physics_hz is currently {physics_hz}, not the 240.0 that is recommended by pybullet. There may be physics errors."
+            )
+
         # check to ensure drone type has same number as drones if is list/tuple
         if isinstance(drone_type, (tuple, list)):
             assert (
                 len(drone_type) == start_pos.shape[0]
             ), f"If multiple `drone_types` are used, must have same number of `drone_types` ({len(drone_type)}) as number of drones ({start_pos.shape[0]})."
         # check to ensure drone type has same number as drones if is list/tuple
         if isinstance(drone_options, (tuple, list)):
@@ -204,14 +208,19 @@
         self.frame_time_elapsed = 0.0
         self.sim_time_elapsed = 0.0
 
         # arm everything
         self.register_all_new_bodies()
         self.set_armed(True)
 
+        # reset all drones and initialize required states
+        [drone.reset() for drone in self.drones]
+        [drone.update_state() for drone in self.drones]
+        [drone.update_last() for drone in self.drones]
+
     def register_all_new_bodies(self):
         """Registers all new bodies in the environment to be able to handle collisions later.
 
         Call this when there is an update in the number of bodies in the environment.
         """
         # collision array
         self.contact_array = np.zeros(
@@ -336,14 +345,16 @@
         if self.render:
             elapsed = time.time() - self.now
             self.now = time.time()
 
             self.sim_time_elapsed += self.update_period * self.updates_per_step
             self.frame_time_elapsed += elapsed
 
+            time.sleep(max(self.sim_time_elapsed - self.frame_time_elapsed, 0.0))
+
             # print RTF every 0.5 seconds, this actually adds considerable overhead
             if self.frame_time_elapsed >= 0.5:
                 # calculate real time factor based on realtime/simtime
                 RTF = self.sim_time_elapsed / (self.frame_time_elapsed + 1e-6)
                 self.sim_time_elapsed = 0.0
                 self.frame_time_elapsed = 0.0
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.1/PyFlyt/core/drones/fixedwing.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,31 +179,25 @@
                 camera_FOV_degrees=camera_FOV_degrees,
                 camera_angle_degrees=camera_angle_degrees,
                 camera_resolution=camera_resolution,
                 camera_position_offset=camera_position_offset,
                 is_tracking_camera=True,
             )
 
-        self.reset()
-
     def reset(self):
         """Resets the vehicle to the initial state."""
         self.set_mode(0)
         self.setpoint = np.zeros(4)
         self.cmd = np.zeros(4)
 
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.p.resetBaseVelocity(self.Id, self.starting_velocity, [0, 0, 0])
         self.disable_artificial_damping()
         self.lifting_surfaces.reset()
         self.motors.reset()
-        self.update_state()
-
-        if self.use_camera:
-            self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
 
     def update_control(self):
         """Runs through controllers."""
         # the default mode
         if self.mode == 0:
             self.cmd = self.setpoint
             return
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.1/PyFlyt/core/drones/quadx.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,29 +182,23 @@
                 camera_id=0,
                 use_gimbal=use_gimbal,
                 camera_FOV_degrees=camera_FOV_degrees,
                 camera_angle_degrees=camera_angle_degrees,
                 camera_resolution=camera_resolution,
             )
 
-        self.reset()
-
     def reset(self):
         """Resets the vehicle to the initial state."""
         self.set_mode(0)
         self.setpoint = np.zeros(4)
         self.pwm = np.zeros(4)
 
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.disable_artificial_damping()
         self.motors.reset()
-        self.update_state()
-
-        if self.use_camera:
-            self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
 
     def set_mode(self, mode: int):
         """Sets the current flight mode of the vehicle.
 
         sets the flight mode:
            -1 - m1, m2, m3, m4
             0 - vp, vq, vr, T
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.1/PyFlyt/core/drones/rocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,32 +202,26 @@
                 camera_FOV_degrees=camera_FOV_degrees,
                 camera_angle_degrees=camera_angle_degrees,
                 camera_resolution=camera_resolution,
                 camera_position_offset=camera_position_offset,
                 is_tracking_camera=True,
             )
 
-        self.reset()
-
     def reset(self):
         """Resets the vehicle to the initial state."""
         self.set_mode(0)
         self.setpoint = np.zeros(7)
         self.cmd = np.zeros(8)
 
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.disable_artificial_damping()
         self.bodies.reset()
         self.lifting_surfaces.reset()
         self.booster_gimbal.reset()
         self.boosters.reset(starting_fuel_ratio=self.starting_fuel_ratio)
-        self.update_state()
-
-        if self.use_camera:
-            self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
 
     def update_control(self):
         """Runs through controllers."""
         # the default mode
         if self.mode == 0:
             # finlet mapping
             finlet_cmd = self.finlet_map @ np.expand_dims(self.setpoint[:3], axis=-1)
```

### Comparing `PyFlyt-0.6.0/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.1/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 from ..waypoint_handler import WaypointHandler
 from .fixedwing_base_env import FixedwingBaseEnv
 
 
 class FixedwingWaypointsEnv(FixedwingBaseEnv):
     """Fixedwing Waypoints Environment.
 
-    Actions are vp, vq, vr, T, ie: angular rates and thrust
+    Actions are roll, pitch, yaw, thrust commands.
+    The target is a set of `[x, y, z]` targets in space
 
-    The target is a set of `[x, y, z, yaw]` targets in space
-
-    Reward:
-        200.0 for reaching target,
-        -100 for collisions or out of bounds,
-        -0.1 otherwise
+    Args:
+        sparse_reward (bool): whether to use sparse rewards or not.
+        num_targets (int): number of waypoints in the environment.
+        goal_reach_distance (float): distance to the waypoints for it to be considered reached.
+        flight_dome_size (float): size of the allowable flying area.
+        max_duration_seconds (float): maximum simulation time of the environment.
+        angle_representation (str): can be "euler" or "quaternion".
+        agent_hz (int): looprate of the agent to environment interaction.
+        render_mode (None | str): can be "human" or None
+        render_resolution (tuple[int, int]): render_resolution
     """
 
     def __init__(
         self,
         sparse_reward: bool = False,
         num_targets: int = 4,
         goal_reach_distance: float = 2.0,
@@ -32,22 +37,22 @@
         agent_hz: int = 30,
         render_mode: None | str = None,
         render_resolution: tuple[int, int] = (480, 480),
     ):
         """__init__.
 
         Args:
-            sparse_reward (bool): sparse_reward
-            num_targets (int): num_targets
-            goal_reach_distance (float): goal_reach_distance
-            flight_dome_size (float): flight_dome_size
-            max_duration_seconds (float): max_duration_seconds
-            angle_representation (str): angle_representation
-            agent_hz (int): agent_hz
-            render_mode (None | str): render_mode
+            sparse_reward (bool): whether to use sparse rewards or not.
+            num_targets (int): number of waypoints in the environment.
+            goal_reach_distance (float): distance to the waypoints for it to be considered reached.
+            flight_dome_size (float): size of the allowable flying area.
+            max_duration_seconds (float): maximum simulation time of the environment.
+            angle_representation (str): can be "euler" or "quaternion".
+            agent_hz (int): looprate of the agent to environment interaction.
+            render_mode (None | str): can be "human" or None
             render_resolution (tuple[int, int]): render_resolution
         """
         super().__init__(
             start_pos=np.array([[0.0, 0.0, 10.0]]),
             flight_dome_size=flight_dome_size,
             max_duration_seconds=max_duration_seconds,
             angle_representation=angle_representation,
```

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
 from .quadx_base_env import QuadXBaseEnv
 
 
 class QuadXHoverEnv(QuadXBaseEnv):
     """Simple Hover Environment.
 
-    Actions are vp, vq, vr, T, ie: angular rates and thrust
+    Actions are vp, vq, vr, T, ie: angular rates and thrust.
+    The target is to not crash for the longest time possible.
 
-    The target is to not crash for the longest time possible
-
-    Reward:
-        -100 for collisions or out of bounds,
-        -0.1 otherwise
+    Args:
+        sparse_reward (bool): whether to use sparse rewards or not.
+        flight_dome_size (float): size of the allowable flying area.
+        max_duration_seconds (float): maximum simulation time of the environment.
+        angle_representation (str): can be "euler" or "quaternion".
+        agent_hz (int): looprate of the agent to environment interaction.
+        render_mode (None | str): can be "human" or None.
+        render_resolution (tuple[int, int]): render_resolution.
     """
 
     def __init__(
         self,
         sparse_reward: bool = False,
         flight_dome_size: float = 3.0,
         max_duration_seconds: float = 10.0,
@@ -27,21 +31,21 @@
         agent_hz: int = 40,
         render_mode: None | str = None,
         render_resolution: tuple[int, int] = (480, 480),
     ):
         """__init__.
 
         Args:
-            sparse_reward (bool): sparse_reward
-            flight_dome_size (float): size of the allowable flying area
-            max_duration_seconds (float): maximum simulatiaon time of the environment
-            angle_representation (str): can be "euler" or "quaternion"
-            agent_hz (int): looprate of the agent to environment interaction
-            render_mode (None | str): can be "human" or None
-            render_resolution (tuple[int, int]): render_resolution
+            sparse_reward (bool): whether to use sparse rewards or not.
+            flight_dome_size (float): size of the allowable flying area.
+            max_duration_seconds (float): maximum simulation time of the environment.
+            angle_representation (str): can be "euler" or "quaternion".
+            agent_hz (int): looprate of the agent to environment interaction.
+            render_mode (None | str): can be "human" or None.
+            render_resolution (tuple[int, int]): render_resolution.
         """
         super().__init__(
             flight_dome_size=flight_dome_size,
             max_duration_seconds=max_duration_seconds,
             angle_representation=angle_representation,
             agent_hz=agent_hz,
             render_mode=render_mode,
```

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 from ..waypoint_handler import WaypointHandler
 from .quadx_base_env import QuadXBaseEnv
 
 
 class QuadXWaypointsEnv(QuadXBaseEnv):
     """QuadX Waypoints Environment.
 
-    Actions are vp, vq, vr, T, ie: angular rates and thrust
+    Actions are vp, vq, vr, T, ie: angular rates and thrust.
+    The target is a set of `[x, y, z, (optional) yaw]` waypoints in space.
 
-    The target is a set of `[x, y, z, yaw]` targets in space
-
-    Reward:
-        200.0 for reaching target,
-        -100 for collisions or out of bounds,
-        -0.1 otherwise
+    Args:
+        sparse_reward (bool): whether to use sparse rewards or not.
+        num_targets (int): number of waypoints in the environment.
+        use_yaw_targets (bool): whether to match yaw targets before a waypoint is considered reached.
+        goal_reach_distance (float): distance to the waypoints for it to be considered reached.
+        goal_reach_angle (float): angle in radians to the waypoints for it to be considered reached, only in effect if `use_yaw_targets` is used.
+        flight_dome_size (float): size of the allowable flying area.
+        max_duration_seconds (float): maximum simulation time of the environment.
+        angle_representation (str): can be "euler" or "quaternion".
+        agent_hz (int): looprate of the agent to environment interaction.
+        render_mode (None | str): can be "human" or None
+        render_resolution (tuple[int, int]): render_resolution
     """
 
     def __init__(
         self,
         sparse_reward: bool = False,
         num_targets: int = 4,
         use_yaw_targets: bool = False,
@@ -34,24 +41,24 @@
         agent_hz: int = 30,
         render_mode: None | str = None,
         render_resolution: tuple[int, int] = (480, 480),
     ):
         """__init__.
 
         Args:
-            sparse_reward (bool): sparse_reward
-            num_targets (int): num_targets
-            use_yaw_targets (bool): use_yaw_targets
-            goal_reach_distance (float): goal_reach_distance
-            goal_reach_angle (float): goal_reach_angle
-            flight_dome_size (float): flight_dome_size
-            max_duration_seconds (float): max_duration_seconds
-            angle_representation (str): angle_representation
-            agent_hz (int): agent_hz
-            render_mode (None | str): render_mode
+            sparse_reward (bool): whether to use sparse rewards or not.
+            num_targets (int): number of waypoints in the environment.
+            use_yaw_targets (bool): whether to match yaw targets before a waypoint is considered reached.
+            goal_reach_distance (float): distance to the waypoints for it to be considered reached.
+            goal_reach_angle (float): angle in radians to the waypoints for it to be considered reached, only in effect if `use_yaw_targets` is used.
+            flight_dome_size (float): size of the allowable flying area.
+            max_duration_seconds (float): maximum simulation time of the environment.
+            angle_representation (str): can be "euler" or "quaternion".
+            agent_hz (int): looprate of the agent to environment interaction.
+            render_mode (None | str): can be "human" or None
             render_resolution (tuple[int, int]): render_resolution
         """
         super().__init__(
             start_pos=np.array([[0.0, 0.0, 1.0]]),
             flight_dome_size=flight_dome_size,
             max_duration_seconds=max_duration_seconds,
             angle_representation=angle_representation,
```

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 
 from .rocket_base_env import RocketBaseEnv
 
 
 class RocketLandingEnv(RocketBaseEnv):
     """Rocket Landing Environment.
 
-    Actions are finlet_x, finlet_z, roll, booster ignition, throttle, booster gimbal x, booster gimbal z
+    Actions are finlet_x, finlet_y, finlet_roll, booster ignition, throttle, booster gimbal x, booster gimbal y
+    The goal is to land the rocket on the landing pad.
 
-    The goal is to land the rocket on the landing pad
-
-    Reward:
-        -100 for collisions or out of bounds,
-        -0.1 otherwise
+    Args:
+        sparse_reward (bool): whether to use sparse rewards or not.
+        ceiling (float): the absolute ceiling of the flying area.
+        max_displacement (float): the maximum horizontal distance the rocket can go.
+        max_duration_seconds (float): maximum simulation time of the environment.
+        angle_representation (str): can be "euler" or "quaternion".
+        agent_hz (int): looprate of the agent to environment interaction..
+        render_mode (None | str): can be "human" or None.
+        render_resolution (tuple[int, int]): render_resolution.
     """
 
     def __init__(
         self,
         sparse_reward: bool = False,
         ceiling: float = 500.0,
         max_displacement: float = 200.0,
@@ -32,22 +37,22 @@
         agent_hz: int = 40,
         render_mode: None | str = None,
         render_resolution: tuple[int, int] = (480, 480),
     ):
         """__init__.
 
         Args:
-            sparse_reward (bool): sparse_reward
-            ceiling (float): the absolute ceiling of the flying area
-            max_displacement (float): the maximum horizontal distance the rocket can go
-            max_duration_seconds (float): maximum simulatiaon time of the environment
-            angle_representation (str): can be "euler" or "quaternion"
-            agent_hz (int): looprate of the agent to environment interaction
-            render_mode (None | str): can be "human" or None
-            render_resolution (tuple[int, int]): render_resolution
+            sparse_reward (bool): whether to use sparse rewards or not.
+            ceiling (float): the absolute ceiling of the flying area.
+            max_displacement (float): the maximum horizontal distance the rocket can go.
+            max_duration_seconds (float): maximum simulation time of the environment.
+            angle_representation (str): can be "euler" or "quaternion".
+            agent_hz (int): looprate of the agent to environment interaction..
+            render_mode (None | str): can be "human" or None.
+            render_resolution (tuple[int, int]): render_resolution.
         """
         super().__init__(
             start_pos=np.array([[0.0, 0.0, ceiling * 0.9]]),
             start_orn=np.array([[0.0, 0.0, 0.0]]),
             ceiling=ceiling,
             max_displacement=max_displacement,
             max_duration_seconds=max_duration_seconds,
@@ -80,15 +85,15 @@
     def reset(self, seed=None, options=dict()):
         """Resets the environment.
 
         Args:
             seed: int
             options: None
         """
-        options = dict(randomize_drop=False, accelerate_drop=True)
+        options = dict(randomize_drop=True, accelerate_drop=True)
         drone_options = dict(starting_fuel_ratio=0.01)
 
         super().begin_reset(seed, options, drone_options)
 
         # reset the tracked parameters
         self.landing_pad_contact = 0.0
         self.ang_vel = np.zeros((3,))
@@ -137,43 +142,43 @@
             self.lin_vel,
             lin_pos,
             quarternion,
         ) = super().compute_attitude()
         aux_state = super().compute_auxiliary()
 
         # drone to landing pad
-        # rotation = np.array(p.getMatrixFromQuaternion(quarternion)).reshape(3, 3)
-        # self.distance = np.matmul((lin_pos - self.landing_pad_position), rotation)
+        rotation = np.array(p.getMatrixFromQuaternion(quarternion)).reshape(3, 3)
         self.distance = lin_pos - self.landing_pad_position
+        rotated_distance = np.matmul(self.distance, rotation)
 
         # combine everything
         if self.angle_representation == 0:
             self.state = np.array(
                 [
                     *self.ang_vel,
                     *self.ang_pos,
                     *self.lin_vel,
                     *lin_pos,
                     *self.action,
                     *aux_state,
                     self.landing_pad_contact,
-                    *self.distance,
+                    *rotated_distance,
                 ]
             )
         elif self.angle_representation == 1:
             self.state = np.array(
                 [
                     *self.ang_vel,
                     *quarternion,
                     *self.lin_vel,
                     *lin_pos,
                     *self.action,
                     *aux_state,
                     self.landing_pad_contact,
-                    *self.distance,
+                    *rotated_distance,
                 ]
             )
 
     def compute_term_trunc_reward(self):
         """Computes the termination, truncation, and reward of the current timestep."""
         super().compute_base_term_trunc_reward(
             collision_ignore_mask=[self.env.drones[0].Id, self.landing_pad_id]
@@ -196,22 +201,29 @@
                     0.0,
                 )
                 / self.distance[-1]
             )
 
             # composite reward together
             self.reward += (
-                # -5.0  # negative offset to discourage staying in the air
-                # + (1.0 / offset_to_pad)  # encourage being near the pad
-                # + (500.0 * progress_to_pad)  # encourage progress to landing pad
-                -(1.0 * abs(self.ang_vel[-1]))  # minimize spinning
-                - (1.0 * np.linalg.norm(self.ang_pos[:2]))  # penalize aggressive angles
+                -5.0  # negative offset to discourage staying in the air
+                + (2.0 / offset_to_pad)  # encourage being near the pad
+                + (100.0 * progress_to_pad)  # encourage progress to landing pad
+                - (1.0 * abs(self.ang_vel[-1]))  # minimize spinning
+                - (3.0 * np.linalg.norm(self.ang_pos[:2]))  # penalize aggressive angles
                 # + (5.0 * deceleration_bonus)  # reward deceleration when near pad
             )
 
+            # -5.0  # negative offset to discourage staying in the air
+            # + (2.0 / offset_to_pad)  # encourage being near the pad
+            # + (100.0 * progress_to_pad)  # encourage progress to landing pad
+            # -(1.0 * abs(self.ang_vel[-1]))  # minimize spinning
+            # - (1.0 * np.linalg.norm(self.ang_pos[:2]))  # penalize aggressive angles
+            # # + (5.0 * deceleration_bonus)  # reward deceleration when near pad
+
         # check if we touched the landing pad
         if self.env.contact_array[self.env.drones[0].Id, self.landing_pad_id]:
             self.landing_pad_contact = 1.0
             self.reward += 20
         else:
             self.landing_pad_contact = 0.0
             return
```

### Comparing `PyFlyt-0.6.0/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.1/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.1/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.1/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.6.1/PyFlyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.0
+Version: 0.6.1
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -204,15 +204,15 @@
 ```
 
 > `angle_representation` can be either `"quaternion"` or `"euler"`.
 >
 > `render_mode` can be either `"human"` or `rgb_array` or `None`.
 
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/fixedwing_waypoint.gif?raw=true" width="500px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/rocket_landing.gif?raw=true" width="500px"/>
 </p>
 
 ## Citation
 
 If you use our work in your research and would like to cite it, please use the following bibtex entry:
 
 ```
```

### Comparing `PyFlyt-0.6.0/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.1/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/pyproject.toml` & `PyFlyt-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.6.0/readme.md` & `PyFlyt-0.6.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 ```
 
 > `angle_representation` can be either `"quaternion"` or `"euler"`.
 >
 > `render_mode` can be either `"human"` or `rgb_array` or `None`.
 
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/fixedwing_waypoint.gif?raw=true" width="500px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/rocket_landing.gif?raw=true" width="500px"/>
 </p>
 
 ## Citation
 
 If you use our work in your research and would like to cite it, please use the following bibtex entry:
 
 ```
```

### Comparing `PyFlyt-0.6.0/tests/test_core.py` & `PyFlyt-0.6.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.0/tests/test_gym_envs.py` & `PyFlyt-0.6.1/tests/test_gym_envs.py`

 * *Files identical despite different names*

