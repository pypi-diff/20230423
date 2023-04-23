# Comparing `tmp/jsbgym-0.1.7.tar.gz` & `tmp/jsbgym-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsbgym-0.1.7.tar", last modified: Thu Apr  6 06:55:26 2023, max compression
+gzip compressed data, was "jsbgym-0.1.8.tar", last modified: Sun Apr 23 06:28:06 2023, max compression
```

## Comparing `jsbgym-0.1.7.tar` & `jsbgym-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 06:55:26.889910 jsbgym-0.1.7/
--rw-rw-rw-   0        0        0     1083 2023-02-19 04:39:50.000000 jsbgym-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       39 2023-02-19 04:58:34.000000 jsbgym-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7288 2023-04-06 06:55:26.888909 jsbgym-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6495 2023-04-04 01:00:39.000000 jsbgym-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 06:55:26.852571 jsbgym-0.1.7/jsbgym/
--rw-rw-rw-   0        0        0     1030 2023-04-03 12:20:23.000000 jsbgym-0.1.7/jsbgym/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:55:26.872572 jsbgym-0.1.7/jsbgym/agents/
--rw-rw-rw-   0        0        0       68 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/agents/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-03-30 20:35:40.000000 jsbgym-0.1.7/jsbgym/agents/agents.py
--rw-rw-rw-   0        0        0      939 2023-04-04 00:54:34.000000 jsbgym-0.1.7/jsbgym/aircraft.py
--rw-rw-rw-   0        0        0     8691 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/assessors.py
--rw-rw-rw-   0        0        0      753 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/basic_ic.xml
--rw-rw-rw-   0        0        0     9268 2023-04-03 12:18:45.000000 jsbgym-0.1.7/jsbgym/environment.py
--rw-rw-rw-   0        0        0      593 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/flightgear.xml
--rw-rw-rw-   0        0        0      118 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/minimal_ic.xml
--rw-rw-rw-   0        0        0     6882 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/properties.py
--rw-rw-rw-   0        0        0    11941 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/rewards.py
--rw-rw-rw-   0        0        0     9598 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/simulation.py
--rw-rw-rw-   0        0        0    19494 2023-03-30 20:35:39.000000 jsbgym-0.1.7/jsbgym/tasks.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:55:26.887910 jsbgym-0.1.7/jsbgym/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/__init__.py
--rw-rw-rw-   0        0        0     6748 2023-03-30 20:35:41.000000 jsbgym-0.1.7/jsbgym/tests/manual_tests.py
--rw-rw-rw-   0        0        0     8547 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/stubs.py
--rw-rw-rw-   0        0        0     1346 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_agents.py
--rw-rw-rw-   0        0        0    12703 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_assessors.py
--rw-rw-rw-   0        0        0     8789 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_environment.py
--rw-rw-rw-   0        0        0     3112 2023-03-30 20:35:43.000000 jsbgym-0.1.7/jsbgym/tests/test_functional.py
--rw-rw-rw-   0        0        0     2345 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_geodetic_position.py
--rw-rw-rw-   0        0        0    17121 2023-02-21 09:27:05.000000 jsbgym-0.1.7/jsbgym/tests/test_rewards.py
--rw-rw-rw-   0        0        0     6350 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_simulation.py
--rw-rw-rw-   0        0        0    25499 2023-03-30 21:26:25.000000 jsbgym-0.1.7/jsbgym/tests/test_tasks.py
--rw-rw-rw-   0        0        0     4051 2023-02-19 04:39:50.000000 jsbgym-0.1.7/jsbgym/tests/test_visualiser.py
--rw-rw-rw-   0        0        0     2756 2023-04-04 00:41:50.000000 jsbgym-0.1.7/jsbgym/utils.py
--rw-rw-rw-   0        0        0    13723 2023-04-06 06:54:35.000000 jsbgym-0.1.7/jsbgym/visualiser.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:55:26.870572 jsbgym-0.1.7/jsbgym.egg-info/
--rw-rw-rw-   0        0        0     7288 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 06:55:26.000000 jsbgym-0.1.7/jsbgym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-04-06 06:41:16.000000 jsbgym-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 06:55:26.889910 jsbgym-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-23 06:27:52.000000 jsbgym-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:27:52.000000 jsbgym-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-23 06:28:06.816856 jsbgym-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-23 06:27:52.000000 jsbgym-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/basic_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/flightgear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/minimal_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/manual_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_geodetic_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/tests/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-23 06:27:52.000000 jsbgym-0.1.8/jsbgym/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:28:06.816856 jsbgym-0.1.8/jsbgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 06:28:06.000000 jsbgym-0.1.8/jsbgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-23 06:27:52.000000 jsbgym-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:28:06.816856 jsbgym-0.1.8/setup.cfg
```

### Comparing `jsbgym-0.1.7/LICENSE` & `jsbgym-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/PKG-INFO` & `jsbgym-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: jsbgym
-Version: 0.1.7
-Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
-Author: sryu1
-License: MIT
-Project-URL: Homepage, https://github.com/sryu1/jsbgym
-Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JSBGym
 
 [![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
 [![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -28,15 +9,15 @@
 
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
 ## Setup
 
 Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
 
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
+If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
 3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
 
 ```console
 fgfs --version
 ```
 
 Open the console and install jsbgym:
@@ -54,51 +35,57 @@
 env = gym.make(ENV_ID)
 env.reset()
 observation, reward, terminated, truncated, info = env.step(action)
 ```
 
 ## Environments
 
-### Task
-
-JSBGym implements two tasks for controlling the altitude and heading of aircraft:
+Environment ID strings are constructed as follows:
 
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+```python
+f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
+```
 
 ### Aircraft
 
 The environment can be configured to use one of Six aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
-* **F-16** General Dynamics F-16CJ Block 52
+* **F16** General Dynamics F-16CJ Block 52
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
 
 Some aircraft will not work until the next update of JSBSim.
 
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
+### Task
+
+JSBGym implements two tasks for controlling the altitude and heading of aircraft:
+
+* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+
 ### Shaping
 
 The environment can use three different shaping types:
 
 * **Shaping.STANDARD**
 * **Shaping.EXTRA**
 * **Shaping.EXTRA_SEQUENTIAL**
 
-Environment ID strings are constructed as follows:
+### FlightGear
 
-```python
-f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
-```
+If using FlightGear as a render mode, use "FG", if not, use "NoFG"
 
-For example, to fly a Cessna on the Heading Control task,
+### Environment ID
+
+To fly a Cessna on the Heading Control task withoug using FlightGear,
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
 ```
 
 ## Visualisation
 
@@ -150,13 +137,10 @@
 
  ```python
  (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
  ```
 
- Throttle will be 0.8 by default.
-
 ## Known Issues
 
-* Some aircraft when rendering with FlightGear will not start on the ground, but in the ground (A320 does not work completely with render).
-* Human render mode will not work due to Attribute error when calling render with matplotlib>=3.7.0
+* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.7/README.md` & `jsbgym-0.1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,165 @@
-# JSBGym
-
-[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
-[![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
-[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-> **Note**: This library will only work with Windows.
-
-JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
-
-## Setup
-
-Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
-
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
-
-```console
-fgfs --version
-```
-
-Open the console and install jsbgym:
-
-```console
-pip install jsbgym
-```
-
-## Getting Started
-
-```python
-import jsbgym
-import gymnasium as gym
-
-env = gym.make(ENV_ID)
-env.reset()
-observation, reward, terminated, truncated, info = env.step(action)
-```
-
-## Environments
-
-### Task
-
-JSBGym implements two tasks for controlling the altitude and heading of aircraft:
-
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
-
-### Aircraft
-
-The environment can be configured to use one of Six aircraft:
-
-* **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
-* **PA28** Piper PA-28-161 Warrior II
-* **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
-* **F-16** General Dynamics F-16CJ Block 52
-* **A320** Airbus A320 (A320 Familiy in Flightgear)
-* **B747** Boeing 747-400
-
-Some aircraft will not work until the next update of JSBSim.
-
-All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
-
-### Shaping
-
-The environment can use three different shaping types:
-
-* **Shaping.STANDARD**
-* **Shaping.EXTRA**
-* **Shaping.EXTRA_SEQUENTIAL**
-
-Environment ID strings are constructed as follows:
-
-```python
-f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
-```
-
-For example, to fly a Cessna on the Heading Control task,
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
-```
-
-## Visualisation
-
-### 2D
-
-A basic plot of agent actions and current state information can be using `human` render mode by calling `env.render()` after specifying the render mode in `gym.make()`.
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
-env.reset()
-env.render()
-```
-
-### 3D
-
-Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
-env.reset()
-env.render()
-```
-
-## State and Action Space
-
-JSBGym's environments have a continuous state and action space. The state is a 17-tuple:
-
-```python
-(name='position/h-sl-ft', description='altitude above mean sea level [ft]', min=-1400, max=85000)
-(name='attitude/pitch-rad', description='pitch [rad]', min=-1.5707963267948966, max=1.5707963267948966)
-(name='attitude/roll-rad', description='roll [rad]', min=-3.141592653589793, max=3.141592653589793)
-(name='velocities/u-fps', description='body frame x-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/v-fps', description='body frame y-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/w-fps', description='body frame z-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/p-rad_sec', description='roll rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='velocities/q-rad_sec', description='pitch rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='velocities/r-rad_sec', description='yaw rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='fcs/left-aileron-pos-norm', description='left aileron position, normalised', min=-1, max=1)
-(name='fcs/right-aileron-pos-norm', description='right aileron position, normalised', min=-1, max=1)
-(name='fcs/elevator-pos-norm', description='elevator position, normalised', min=-1, max=1)
-(name='fcs/rudder-pos-norm', description='rudder position, normalised', min=-1, max=1)
-(name='error/altitude-error-ft', description='error to desired altitude [ft]', min=-1400, max=85000)
-(name='aero/beta-deg', description='sideslip [deg]', min=-180, max=180)
-(name='error/track-error-deg', description='error to desired track [deg]', min=-180, max=180)
-(name='info/steps_left', description='steps remaining in episode', min=0, max=300)
- ```
-
- Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
-
- ```python
- (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
- (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
- (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
- ```
-
- Throttle will be 0.8 by default.
-
-## Known Issues
-
-* Some aircraft when rendering with FlightGear will not start on the ground, but in the ground (A320 does not work completely with render).
-* Human render mode will not work due to Attribute error when calling render with matplotlib>=3.7.0
+Metadata-Version: 2.1
+Name: jsbgym
+Version: 0.1.8
+Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
+Author: sryu1
+License: MIT
+Project-URL: Homepage, https://github.com/sryu1/jsbgym
+Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# JSBGym
+
+[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
+[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+> **Note**: This library will only work with Windows.
+
+JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
+
+## Setup
+
+Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
+
+If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+
+```console
+fgfs --version
+```
+
+Open the console and install jsbgym:
+
+```console
+pip install jsbgym
+```
+
+## Getting Started
+
+```python
+import jsbgym
+import gymnasium as gym
+
+env = gym.make(ENV_ID)
+env.reset()
+observation, reward, terminated, truncated, info = env.step(action)
+```
+
+## Environments
+
+Environment ID strings are constructed as follows:
+
+```python
+f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
+```
+
+### Aircraft
+
+The environment can be configured to use one of Six aircraft:
+
+* **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
+* **PA28** Piper PA-28-161 Warrior II
+* **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
+* **F16** General Dynamics F-16CJ Block 52
+* **A320** Airbus A320 (A320 Familiy in Flightgear)
+* **B747** Boeing 747-400
+
+Some aircraft will not work until the next update of JSBSim.
+
+All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
+
+### Task
+
+JSBGym implements two tasks for controlling the altitude and heading of aircraft:
+
+* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+
+### Shaping
+
+The environment can use three different shaping types:
+
+* **Shaping.STANDARD**
+* **Shaping.EXTRA**
+* **Shaping.EXTRA_SEQUENTIAL**
+
+### FlightGear
+
+If using FlightGear as a render mode, use "FG", if not, use "NoFG"
+
+### Environment ID
+
+To fly a Cessna on the Heading Control task withoug using FlightGear,
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
+```
+
+## Visualisation
+
+### 2D
+
+A basic plot of agent actions and current state information can be using `human` render mode by calling `env.render()` after specifying the render mode in `gym.make()`.
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
+env.reset()
+env.render()
+```
+
+### 3D
+
+Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
+env.reset()
+env.render()
+```
+
+## State and Action Space
+
+JSBGym's environments have a continuous state and action space. The state is a 17-tuple:
+
+```python
+(name='position/h-sl-ft', description='altitude above mean sea level [ft]', min=-1400, max=85000)
+(name='attitude/pitch-rad', description='pitch [rad]', min=-1.5707963267948966, max=1.5707963267948966)
+(name='attitude/roll-rad', description='roll [rad]', min=-3.141592653589793, max=3.141592653589793)
+(name='velocities/u-fps', description='body frame x-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/v-fps', description='body frame y-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/w-fps', description='body frame z-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/p-rad_sec', description='roll rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='velocities/q-rad_sec', description='pitch rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='velocities/r-rad_sec', description='yaw rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='fcs/left-aileron-pos-norm', description='left aileron position, normalised', min=-1, max=1)
+(name='fcs/right-aileron-pos-norm', description='right aileron position, normalised', min=-1, max=1)
+(name='fcs/elevator-pos-norm', description='elevator position, normalised', min=-1, max=1)
+(name='fcs/rudder-pos-norm', description='rudder position, normalised', min=-1, max=1)
+(name='error/altitude-error-ft', description='error to desired altitude [ft]', min=-1400, max=85000)
+(name='aero/beta-deg', description='sideslip [deg]', min=-180, max=180)
+(name='error/track-error-deg', description='error to desired track [deg]', min=-180, max=180)
+(name='info/steps_left', description='steps remaining in episode', min=0, max=300)
+ ```
+
+ Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
+
+ ```python
+ (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
+ (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
+ (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
+ ```
+
+## Known Issues
+
+* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.7/jsbgym/__init__.py` & `jsbgym-0.1.8/jsbgym/__init__.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/agents/agents.py` & `jsbgym-0.1.8/jsbgym/agents/agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/aircraft.py` & `jsbgym-0.1.8/jsbgym/aircraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
 
 cessna172P = Aircraft("c172p", "c172p", "Cessna172P", 120)
 pa28 = Aircraft("pa28", "PA28-161-180", "PA28", 130)
 f15 = Aircraft("f15", "f15c", "F15", 500)
 f16 = Aircraft("f16", "f16-block-52", "F16", 550)
 a320 = Aircraft("A320", "A320-200-CFM", "A320", 480)
-b747 = Aircraft("B747", "787-400", "B747", 490)
+b747 = Aircraft("B747", "747-400", "B747", 490)
```

### Comparing `jsbgym-0.1.7/jsbgym/assessors.py` & `jsbgym-0.1.8/jsbgym/assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/basic_ic.xml` & `jsbgym-0.1.8/jsbgym/basic_ic.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/environment.py` & `jsbgym-0.1.8/jsbgym/environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/flightgear.xml` & `jsbgym-0.1.8/jsbgym/flightgear.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/properties.py` & `jsbgym-0.1.8/jsbgym/properties.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/rewards.py` & `jsbgym-0.1.8/jsbgym/rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/simulation.py` & `jsbgym-0.1.8/jsbgym/simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tasks.py` & `jsbgym-0.1.8/jsbgym/tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/manual_tests.py` & `jsbgym-0.1.8/jsbgym/tests/manual_tests.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/stubs.py` & `jsbgym-0.1.8/jsbgym/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_agents.py` & `jsbgym-0.1.8/jsbgym/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_assessors.py` & `jsbgym-0.1.8/jsbgym/tests/test_assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_environment.py` & `jsbgym-0.1.8/jsbgym/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_functional.py` & `jsbgym-0.1.8/jsbgym/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_geodetic_position.py` & `jsbgym-0.1.8/jsbgym/tests/test_geodetic_position.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_rewards.py` & `jsbgym-0.1.8/jsbgym/tests/test_rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_simulation.py` & `jsbgym-0.1.8/jsbgym/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_tasks.py` & `jsbgym-0.1.8/jsbgym/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/tests/test_visualiser.py` & `jsbgym-0.1.8/jsbgym/tests/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/utils.py` & `jsbgym-0.1.8/jsbgym/utils.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/jsbgym/visualiser.py` & `jsbgym-0.1.8/jsbgym/visualiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,14 +348,15 @@
             time_of_day_arg,
         )
 
     def _block_until_flightgear_loaded(self):
         while True:
             msg_out = self.flightgear_process.stdout.readline().decode()
             if self.LOADED_MESSAGE in msg_out:
+                time.sleep(5)
                 print("FlightGear loading complete")
                 break
             else:
                 time.sleep(0.1)
 
     def close(self):
         if self.flightgear_process:
```

### Comparing `jsbgym-0.1.7/jsbgym.egg-info/PKG-INFO` & `jsbgym-0.1.8/jsbgym.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,165 @@
-Metadata-Version: 2.1
-Name: jsbgym
-Version: 0.1.7
-Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
-Author: sryu1
-License: MIT
-Project-URL: Homepage, https://github.com/sryu1/jsbgym
-Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# JSBGym
-
-[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
-[![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
-[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-> **Note**: This library will only work with Windows.
-
-JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
-
-## Setup
-
-Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
-
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
-
-```console
-fgfs --version
-```
-
-Open the console and install jsbgym:
-
-```console
-pip install jsbgym
-```
-
-## Getting Started
-
-```python
-import jsbgym
-import gymnasium as gym
-
-env = gym.make(ENV_ID)
-env.reset()
-observation, reward, terminated, truncated, info = env.step(action)
-```
-
-## Environments
-
-### Task
-
-JSBGym implements two tasks for controlling the altitude and heading of aircraft:
-
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
-
-### Aircraft
-
-The environment can be configured to use one of Six aircraft:
-
-* **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
-* **PA28** Piper PA-28-161 Warrior II
-* **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
-* **F-16** General Dynamics F-16CJ Block 52
-* **A320** Airbus A320 (A320 Familiy in Flightgear)
-* **B747** Boeing 747-400
-
-Some aircraft will not work until the next update of JSBSim.
-
-All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
-
-### Shaping
-
-The environment can use three different shaping types:
-
-* **Shaping.STANDARD**
-* **Shaping.EXTRA**
-* **Shaping.EXTRA_SEQUENTIAL**
-
-Environment ID strings are constructed as follows:
-
-```python
-f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
-```
-
-For example, to fly a Cessna on the Heading Control task,
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
-```
-
-## Visualisation
-
-### 2D
-
-A basic plot of agent actions and current state information can be using `human` render mode by calling `env.render()` after specifying the render mode in `gym.make()`.
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
-env.reset()
-env.render()
-```
-
-### 3D
-
-Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
-
-```python
-env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
-env.reset()
-env.render()
-```
-
-## State and Action Space
-
-JSBGym's environments have a continuous state and action space. The state is a 17-tuple:
-
-```python
-(name='position/h-sl-ft', description='altitude above mean sea level [ft]', min=-1400, max=85000)
-(name='attitude/pitch-rad', description='pitch [rad]', min=-1.5707963267948966, max=1.5707963267948966)
-(name='attitude/roll-rad', description='roll [rad]', min=-3.141592653589793, max=3.141592653589793)
-(name='velocities/u-fps', description='body frame x-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/v-fps', description='body frame y-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/w-fps', description='body frame z-axis velocity [ft/s]', min=-2200, max=2200)
-(name='velocities/p-rad_sec', description='roll rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='velocities/q-rad_sec', description='pitch rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='velocities/r-rad_sec', description='yaw rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
-(name='fcs/left-aileron-pos-norm', description='left aileron position, normalised', min=-1, max=1)
-(name='fcs/right-aileron-pos-norm', description='right aileron position, normalised', min=-1, max=1)
-(name='fcs/elevator-pos-norm', description='elevator position, normalised', min=-1, max=1)
-(name='fcs/rudder-pos-norm', description='rudder position, normalised', min=-1, max=1)
-(name='error/altitude-error-ft', description='error to desired altitude [ft]', min=-1400, max=85000)
-(name='aero/beta-deg', description='sideslip [deg]', min=-180, max=180)
-(name='error/track-error-deg', description='error to desired track [deg]', min=-180, max=180)
-(name='info/steps_left', description='steps remaining in episode', min=0, max=300)
- ```
-
- Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
-
- ```python
- (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
- (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
- (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
- ```
-
- Throttle will be 0.8 by default.
-
-## Known Issues
-
-* Some aircraft when rendering with FlightGear will not start on the ground, but in the ground (A320 does not work completely with render).
-* Human render mode will not work due to Attribute error when calling render with matplotlib>=3.7.0
+Metadata-Version: 2.1
+Name: jsbgym
+Version: 0.1.8
+Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
+Author: sryu1
+License: MIT
+Project-URL: Homepage, https://github.com/sryu1/jsbgym
+Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# JSBGym
+
+[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
+[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+> **Note**: This library will only work with Windows.
+
+JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
+
+## Setup
+
+Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
+
+If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+
+```console
+fgfs --version
+```
+
+Open the console and install jsbgym:
+
+```console
+pip install jsbgym
+```
+
+## Getting Started
+
+```python
+import jsbgym
+import gymnasium as gym
+
+env = gym.make(ENV_ID)
+env.reset()
+observation, reward, terminated, truncated, info = env.step(action)
+```
+
+## Environments
+
+Environment ID strings are constructed as follows:
+
+```python
+f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
+```
+
+### Aircraft
+
+The environment can be configured to use one of Six aircraft:
+
+* **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
+* **PA28** Piper PA-28-161 Warrior II
+* **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
+* **F16** General Dynamics F-16CJ Block 52
+* **A320** Airbus A320 (A320 Familiy in Flightgear)
+* **B747** Boeing 747-400
+
+Some aircraft will not work until the next update of JSBSim.
+
+All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
+
+### Task
+
+JSBGym implements two tasks for controlling the altitude and heading of aircraft:
+
+* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+
+### Shaping
+
+The environment can use three different shaping types:
+
+* **Shaping.STANDARD**
+* **Shaping.EXTRA**
+* **Shaping.EXTRA_SEQUENTIAL**
+
+### FlightGear
+
+If using FlightGear as a render mode, use "FG", if not, use "NoFG"
+
+### Environment ID
+
+To fly a Cessna on the Heading Control task withoug using FlightGear,
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
+```
+
+## Visualisation
+
+### 2D
+
+A basic plot of agent actions and current state information can be using `human` render mode by calling `env.render()` after specifying the render mode in `gym.make()`.
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
+env.reset()
+env.render()
+```
+
+### 3D
+
+Visualising with FlightGear requires the Gymnasium environment to be created with a FlightGear-enabled environment ID by specifying the render_mode in `gym.make()` and changing the value after `shaping` to `FG`. Using this render mode while training is strongly discouraged due to an error occuring midway through the training (`Could not connect to socket for output!`).
+
+```python
+env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-FG-v0", render_mode="flightgear")
+env.reset()
+env.render()
+```
+
+## State and Action Space
+
+JSBGym's environments have a continuous state and action space. The state is a 17-tuple:
+
+```python
+(name='position/h-sl-ft', description='altitude above mean sea level [ft]', min=-1400, max=85000)
+(name='attitude/pitch-rad', description='pitch [rad]', min=-1.5707963267948966, max=1.5707963267948966)
+(name='attitude/roll-rad', description='roll [rad]', min=-3.141592653589793, max=3.141592653589793)
+(name='velocities/u-fps', description='body frame x-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/v-fps', description='body frame y-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/w-fps', description='body frame z-axis velocity [ft/s]', min=-2200, max=2200)
+(name='velocities/p-rad_sec', description='roll rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='velocities/q-rad_sec', description='pitch rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='velocities/r-rad_sec', description='yaw rate [rad/s]', min=-6.283185307179586, max=6.283185307179586)
+(name='fcs/left-aileron-pos-norm', description='left aileron position, normalised', min=-1, max=1)
+(name='fcs/right-aileron-pos-norm', description='right aileron position, normalised', min=-1, max=1)
+(name='fcs/elevator-pos-norm', description='elevator position, normalised', min=-1, max=1)
+(name='fcs/rudder-pos-norm', description='rudder position, normalised', min=-1, max=1)
+(name='error/altitude-error-ft', description='error to desired altitude [ft]', min=-1400, max=85000)
+(name='aero/beta-deg', description='sideslip [deg]', min=-180, max=180)
+(name='error/track-error-deg', description='error to desired track [deg]', min=-180, max=180)
+(name='info/steps_left', description='steps remaining in episode', min=0, max=300)
+ ```
+
+ Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
+
+ ```python
+ (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
+ (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
+ (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
+ ```
+
+## Known Issues
+
+* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.7/jsbgym.egg-info/SOURCES.txt` & `jsbgym-0.1.8/jsbgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.7/pyproject.toml` & `jsbgym-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "jsbgym"
-version = "0.1.7"
-authors = [{ name = "sryu1" }]
-readme = "README.md"
-license = { text = "MIT" }
-description = "A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model."
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-]
-
-requires-python = ">=3.7"
-dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib<=3.6.3"]
-
-[project.urls]
-Homepage = "https://github.com/sryu1/jsbgym"
-"Bug Tracker" = "https://github.com/sryu1/jsbgym/issues"
-
-
-[tool.setuptools]
-zip-safe = false
-include-package-data = true
-
-[tool.setuptools.packages]
-find = { namespaces = false }
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "jsbgym"
+version = "0.1.8"
+authors = [{ name = "sryu1" }]
+readme = "README.md"
+license = { text = "MIT" }
+description = "A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model."
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+
+requires-python = ">=3.7"
+dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib<=3.6.3"]
+
+[project.urls]
+Homepage = "https://github.com/sryu1/jsbgym"
+"Bug Tracker" = "https://github.com/sryu1/jsbgym/issues"
+
+
+[tool.setuptools]
+zip-safe = false
+include-package-data = true
+
+[tool.setuptools.packages]
+find = { namespaces = false }
```

