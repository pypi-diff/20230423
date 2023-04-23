# Comparing `tmp/stubborn-0.0.1.tar.gz` & `tmp/stubborn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stubborn-0.0.1.tar", last modified: Sun Apr 23 20:16:13 2023, max compression
+gzip compressed data, was "stubborn-0.0.2.tar", last modified: Sun Apr 23 20:21:30 2023, max compression
```

## Comparing `stubborn-0.0.1.tar` & `stubborn-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:16:13.669167 stubborn-0.0.1/
--rw-rw-rw-   0        0        0     1106 2023-04-23 20:10:28.000000 stubborn-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      150 2023-04-23 20:10:11.000000 stubborn-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4546 2023-04-23 20:16:13.668166 stubborn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-23 20:09:26.000000 stubborn-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     3855 2023-04-23 19:54:00.000000 stubborn-0.0.1/readme.md
--rw-rw-rw-   0        0        0      152 2023-04-22 19:18:27.000000 stubborn-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 20:16:13.669167 stubborn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-04-23 20:14:43.000000 stubborn-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:16:13.642166 stubborn-0.0.1/stubborn/
--rw-rw-rw-   0        0        0      418 2023-04-23 20:14:58.000000 stubborn-0.0.1/stubborn/__init__.py
--rw-rw-rw-   0        0        0      169 2023-04-23 20:11:49.000000 stubborn-0.0.1/stubborn/__main__.py
--rw-rw-rw-   0        0        0     1570 2023-04-23 20:11:19.000000 stubborn-0.0.1/stubborn/bootstrap.py
--rw-rw-rw-   0        0        0     7327 2023-04-23 20:11:21.000000 stubborn-0.0.1/stubborn/callbackino.py
--rw-rw-rw-   0        0        0      206 2023-04-23 20:11:24.000000 stubborn-0.0.1/stubborn/command_group.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:16:13.665169 stubborn-0.0.1/stubborn/county/
--rw-rw-rw-   0        0        0      396 2023-04-23 20:11:17.000000 stubborn-0.0.1/stubborn/county/__init__.py
--rw-rw-rw-   0        0        0     3161 2023-04-23 20:10:50.000000 stubborn-0.0.1/stubborn/county/base_env.py
--rw-rw-rw-   0        0        0      766 2023-04-23 20:10:55.000000 stubborn-0.0.1/stubborn/county/base_state.py
--rw-rw-rw-   0        0        0      258 2023-04-23 20:10:58.000000 stubborn-0.0.1/stubborn/county/constants.py
--rw-rw-rw-   0        0        0     1512 2023-04-23 20:11:00.000000 stubborn-0.0.1/stubborn/county/csv_tools.py
--rw-rw-rw-   0        0        0     2911 2023-04-23 20:11:02.000000 stubborn-0.0.1/stubborn/county/filtros.py
--rw-rw-rw-   0        0        0    12932 2023-04-23 20:11:06.000000 stubborn-0.0.1/stubborn/county/misc.py
--rw-rw-rw-   0        0        0     5425 2023-04-23 20:11:08.000000 stubborn-0.0.1/stubborn/county/policing.py
--rw-rw-rw-   0        0        0     1285 2023-04-23 20:11:12.000000 stubborn-0.0.1/stubborn/county/thready_krueger.py
--rw-rw-rw-   0        0        0      373 2023-04-23 20:11:14.000000 stubborn-0.0.1/stubborn/county/typing.py
--rw-rw-rw-   0        0        0      357 2023-04-23 20:11:26.000000 stubborn-0.0.1/stubborn/defaults.py
--rw-rw-rw-   0        0        0      322 2023-04-23 20:11:28.000000 stubborn-0.0.1/stubborn/exceptions.py
--rw-rw-rw-   0        0        0     7649 2023-04-23 20:11:30.000000 stubborn-0.0.1/stubborn/hand_coded_policies.py
--rw-rw-rw-   0        0        0     2406 2023-04-23 20:11:33.000000 stubborn-0.0.1/stubborn/plotting.py
--rw-rw-rw-   0        0        0    10219 2023-04-23 20:11:35.000000 stubborn-0.0.1/stubborn/running.py
--rw-rw-rw-   0        0        0     4727 2023-04-23 20:11:37.000000 stubborn-0.0.1/stubborn/stubborn_config.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 20:11:40.000000 stubborn-0.0.1/stubborn/stubborn_env.py
--rw-rw-rw-   0        0        0    25679 2023-04-23 20:11:42.000000 stubborn-0.0.1/stubborn/stubborn_state.py
--rw-rw-rw-   0        0        0     2943 2023-04-23 20:11:44.000000 stubborn-0.0.1/stubborn/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:16:13.651168 stubborn-0.0.1/stubborn.egg-info/
--rw-rw-rw-   0        0        0     4546 2023-04-23 20:16:13.000000 stubborn-0.0.1/stubborn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-04-23 20:16:13.000000 stubborn-0.0.1/stubborn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 20:16:13.000000 stubborn-0.0.1/stubborn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      161 2023-04-23 20:16:13.000000 stubborn-0.0.1/stubborn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 20:16:13.000000 stubborn-0.0.1/stubborn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:16:13.667169 stubborn-0.0.1/tests/
--rw-rw-rw-   0        0        0      102 2023-04-23 20:12:56.000000 stubborn-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-23 20:11:54.000000 stubborn-0.0.1/tests/test_stubborn_state.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:21:30.079485 stubborn-0.0.2/
+-rw-rw-rw-   0        0        0     1106 2023-04-23 20:10:28.000000 stubborn-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      150 2023-04-23 20:10:11.000000 stubborn-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4546 2023-04-23 20:21:30.078483 stubborn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-23 20:09:26.000000 stubborn-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     3855 2023-04-23 19:54:00.000000 stubborn-0.0.2/readme.md
+-rw-rw-rw-   0        0        0      152 2023-04-22 19:18:27.000000 stubborn-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:21:30.079485 stubborn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-04-23 20:14:43.000000 stubborn-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:21:30.024266 stubborn-0.0.2/stubborn/
+-rw-rw-rw-   0        0        0      418 2023-04-23 20:20:01.000000 stubborn-0.0.2/stubborn/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-04-23 20:11:49.000000 stubborn-0.0.2/stubborn/__main__.py
+-rw-rw-rw-   0        0        0     1570 2023-04-23 20:11:19.000000 stubborn-0.0.2/stubborn/bootstrap.py
+-rw-rw-rw-   0        0        0     7327 2023-04-23 20:11:21.000000 stubborn-0.0.2/stubborn/callbackino.py
+-rw-rw-rw-   0        0        0      206 2023-04-23 20:11:24.000000 stubborn-0.0.2/stubborn/command_group.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:21:30.075482 stubborn-0.0.2/stubborn/county/
+-rw-rw-rw-   0        0        0      396 2023-04-23 20:11:17.000000 stubborn-0.0.2/stubborn/county/__init__.py
+-rw-rw-rw-   0        0        0     3161 2023-04-23 20:10:50.000000 stubborn-0.0.2/stubborn/county/base_env.py
+-rw-rw-rw-   0        0        0      766 2023-04-23 20:10:55.000000 stubborn-0.0.2/stubborn/county/base_state.py
+-rw-rw-rw-   0        0        0      258 2023-04-23 20:10:58.000000 stubborn-0.0.2/stubborn/county/constants.py
+-rw-rw-rw-   0        0        0     1512 2023-04-23 20:11:00.000000 stubborn-0.0.2/stubborn/county/csv_tools.py
+-rw-rw-rw-   0        0        0     2911 2023-04-23 20:11:02.000000 stubborn-0.0.2/stubborn/county/filtros.py
+-rw-rw-rw-   0        0        0    12043 2023-04-23 20:21:05.000000 stubborn-0.0.2/stubborn/county/misc.py
+-rw-rw-rw-   0        0        0     5425 2023-04-23 20:11:08.000000 stubborn-0.0.2/stubborn/county/policing.py
+-rw-rw-rw-   0        0        0     1285 2023-04-23 20:11:12.000000 stubborn-0.0.2/stubborn/county/thready_krueger.py
+-rw-rw-rw-   0        0        0      373 2023-04-23 20:11:14.000000 stubborn-0.0.2/stubborn/county/typing.py
+-rw-rw-rw-   0        0        0      357 2023-04-23 20:11:26.000000 stubborn-0.0.2/stubborn/defaults.py
+-rw-rw-rw-   0        0        0      322 2023-04-23 20:11:28.000000 stubborn-0.0.2/stubborn/exceptions.py
+-rw-rw-rw-   0        0        0     7649 2023-04-23 20:11:30.000000 stubborn-0.0.2/stubborn/hand_coded_policies.py
+-rw-rw-rw-   0        0        0     2406 2023-04-23 20:11:33.000000 stubborn-0.0.2/stubborn/plotting.py
+-rw-rw-rw-   0        0        0    10129 2023-04-23 20:21:19.000000 stubborn-0.0.2/stubborn/running.py
+-rw-rw-rw-   0        0        0     4727 2023-04-23 20:11:37.000000 stubborn-0.0.2/stubborn/stubborn_config.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 20:11:40.000000 stubborn-0.0.2/stubborn/stubborn_env.py
+-rw-rw-rw-   0        0        0    25679 2023-04-23 20:11:42.000000 stubborn-0.0.2/stubborn/stubborn_state.py
+-rw-rw-rw-   0        0        0     2943 2023-04-23 20:11:44.000000 stubborn-0.0.2/stubborn/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:21:30.062486 stubborn-0.0.2/stubborn.egg-info/
+-rw-rw-rw-   0        0        0     4546 2023-04-23 20:21:29.000000 stubborn-0.0.2/stubborn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-04-23 20:21:29.000000 stubborn-0.0.2/stubborn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:21:29.000000 stubborn-0.0.2/stubborn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      161 2023-04-23 20:21:29.000000 stubborn-0.0.2/stubborn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 20:21:29.000000 stubborn-0.0.2/stubborn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:21:30.077482 stubborn-0.0.2/tests/
+-rw-rw-rw-   0        0        0      102 2023-04-23 20:12:56.000000 stubborn-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-23 20:11:54.000000 stubborn-0.0.2/tests/test_stubborn_state.py
```

### Comparing `stubborn-0.0.1/LICENSE` & `stubborn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/PKG-INFO` & `stubborn-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stubborn
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Environment for Evaluating Stubbornness between Agents with Aligned Incentives
 Home-page: https://github.com/cool-RR/stubborn
 Author: Ram Rachum
 Author-email: ram@rachum.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `stubborn-0.0.1/readme.md` & `stubborn-0.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/setup.py` & `stubborn-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/bootstrap.py` & `stubborn-0.0.2/stubborn/bootstrap.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/callbackino.py` & `stubborn-0.0.2/stubborn/callbackino.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/base_env.py` & `stubborn-0.0.2/stubborn/county/base_env.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/base_state.py` & `stubborn-0.0.2/stubborn/county/base_state.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/csv_tools.py` & `stubborn-0.0.2/stubborn/county/csv_tools.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/filtros.py` & `stubborn-0.0.2/stubborn/county/filtros.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/misc.py` & `stubborn-0.0.2/stubborn/county/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,41 +191,14 @@
 # def cool_windowed(iterable: Iterable[Any], n: int = 2) -> Iterable[tuple[Any, Any]]:
     # sentinel = object()
     # for left, right in more_itertools.windowed(iterable, n, fillvalue=sentinel):
         # if sentinel in (left, right):
             # return
         # yield (left, right)
 
-def get_stubborn_repo_commit() -> str:
-    result = subprocess.run(
-        ('/usr/bin/git', 'rev-parse', 'HEAD'),
-        check=True,
-        cwd=pathlib.Path(__file__).parent,
-        stderr=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        encoding='utf-8',
-    )
-    return result.stdout.strip()
-
-def get_stubborn_repo_is_clean() -> bool:
-    result = subprocess.run(
-        (cmd := ('/usr/bin/git', 'diff-index', '--quiet', 'HEAD')),
-        cwd=pathlib.Path(__file__).parent,
-        stderr=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        encoding='utf-8',
-    )
-    if result.returncode == 0:
-        return True
-    elif result.returncode == 1:
-        return False
-    else:
-        raise subprocess.CalledProcessError(result.returncode, cmd=cmd, output=result.stdout,
-                                            stderr=result.stderr)
-
 def clamp(number: RealNumber, low: RealNumber, high: RealNumber) -> RealNumber:
     if number < low:
         return low
     elif number > high:
         return high
     else:
         return number
```

### Comparing `stubborn-0.0.1/stubborn/county/policing.py` & `stubborn-0.0.2/stubborn/county/policing.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/county/thready_krueger.py` & `stubborn-0.0.2/stubborn/county/thready_krueger.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/hand_coded_policies.py` & `stubborn-0.0.2/stubborn/hand_coded_policies.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/plotting.py` & `stubborn-0.0.2/stubborn/plotting.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/running.py` & `stubborn-0.0.2/stubborn/running.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import ray.rllib.env.multi_agent_env
 import ray.rllib.algorithms.callbacks
 from ray.rllib import algorithms
 import ray.tune
 import ray.rllib.algorithms.ppo
 
+import stubborn
 from stubborn import county
 from stubborn.county import misc
 from .stubborn_config import StubbornConfig
 from .stubborn_env import StubbornEnv
 from . import defaults
 from .callbackino import Callbackino
 
@@ -132,16 +133,15 @@
         'insistence_on_stubbornness_4',
     )
 
     with (trial_folder / 'metadata.yaml').open('w') as yaml_file:
         yaml.dump(
             {
                 'stubborn_config': stubborn_config.get_nice_dict(),
-                'stubborn_repo_commit': county.misc.get_stubborn_repo_commit(),
-                'stubborn_repo_is_clean': county.misc.get_stubborn_repo_is_clean(),
+                'stubborn_version': stubborn.__version__,
                 'observation_fields': list(stubborn_env.observation_space.keys()),
                 'algorithm_class': type(algorithm).__name__,
                 'argv': sys.argv if argv is None else argv,
             },
             yaml_file,
         )
```

### Comparing `stubborn-0.0.1/stubborn/stubborn_config.py` & `stubborn-0.0.2/stubborn/stubborn_config.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/stubborn_env.py` & `stubborn-0.0.2/stubborn/stubborn_env.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/stubborn_state.py` & `stubborn-0.0.2/stubborn/stubborn_state.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn/utils.py` & `stubborn-0.0.2/stubborn/utils.py`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/stubborn.egg-info/PKG-INFO` & `stubborn-0.0.2/stubborn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stubborn
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Environment for Evaluating Stubbornness between Agents with Aligned Incentives
 Home-page: https://github.com/cool-RR/stubborn
 Author: Ram Rachum
 Author-email: ram@rachum.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `stubborn-0.0.1/stubborn.egg-info/SOURCES.txt` & `stubborn-0.0.2/stubborn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stubborn-0.0.1/tests/test_stubborn_state.py` & `stubborn-0.0.2/tests/test_stubborn_state.py`

 * *Files identical despite different names*

