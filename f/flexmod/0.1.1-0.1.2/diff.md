# Comparing `tmp/flexmod-0.1.1.tar.gz` & `tmp/flexmod-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmod-0.1.1.tar", last modified: Mon Jan 16 18:12:49 2023, max compression
+gzip compressed data, was "flexmod-0.1.2.tar", last modified: Sat Apr 22 23:43:36 2023, max compression
```

## Comparing `flexmod-0.1.1.tar` & `flexmod-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-16 18:12:49.975248 flexmod-0.1.1/
--rw-r--r--   0 harry      (501) staff       (20)     1066 2023-01-15 00:52:21.000000 flexmod-0.1.1/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)     3920 2023-01-16 18:12:49.974973 flexmod-0.1.1/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)     3398 2023-01-15 18:22:32.000000 flexmod-0.1.1/README.md
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-16 18:12:49.973441 flexmod-0.1.1/flexmod/
--rw-r--r--   0 harry      (501) staff       (20)     4474 2023-01-16 16:15:01.000000 flexmod-0.1.1/flexmod/__init__.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-16 18:12:49.974611 flexmod-0.1.1/flexmod.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)     3920 2023-01-16 18:12:49.000000 flexmod-0.1.1/flexmod.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)      170 2023-01-16 18:12:49.000000 flexmod-0.1.1/flexmod.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-01-16 18:12:49.000000 flexmod-0.1.1/flexmod.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)        8 2023-01-16 18:12:49.000000 flexmod-0.1.1/flexmod.egg-info/top_level.txt
--rw-r--r--   0 harry      (501) staff       (20)       38 2023-01-16 18:12:49.975329 flexmod-0.1.1/setup.cfg
--rw-r--r--   0 harry      (501) staff       (20)      907 2023-01-16 16:15:56.000000 flexmod-0.1.1/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-22 23:43:36.869859 flexmod-0.1.2/
+-rw-r--r--   0 harry      (501) staff       (20)     1066 2023-01-15 00:52:21.000000 flexmod-0.1.2/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)     3893 2023-04-22 23:43:36.869583 flexmod-0.1.2/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     3371 2023-01-20 15:14:39.000000 flexmod-0.1.2/README.md
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-22 23:43:36.868070 flexmod-0.1.2/flexmod/
+-rw-r--r--   0 harry      (501) staff       (20)     4894 2023-04-22 21:01:01.000000 flexmod-0.1.2/flexmod/__init__.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-22 23:43:36.869203 flexmod-0.1.2/flexmod.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)     3893 2023-04-22 23:43:36.000000 flexmod-0.1.2/flexmod.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      170 2023-04-22 23:43:36.000000 flexmod-0.1.2/flexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-04-22 23:43:36.000000 flexmod-0.1.2/flexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)        8 2023-04-22 23:43:36.000000 flexmod-0.1.2/flexmod.egg-info/top_level.txt
+-rw-r--r--   0 harry      (501) staff       (20)       38 2023-04-22 23:43:36.869958 flexmod-0.1.2/setup.cfg
+-rw-r--r--   0 harry      (501) staff       (20)      907 2023-04-22 23:19:31.000000 flexmod-0.1.2/setup.py
```

### Comparing `flexmod-0.1.1/LICENSE` & `flexmod-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flexmod-0.1.1/PKG-INFO` & `flexmod-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module for other modules to allow flexible (yet not error-prone) configuration.
 Home-page: https://github.com/haochuanwei/flexmod
 Author: Haochuan Wei
 Author-email: pepsimixt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flexmod
 A python module for other modules to allow flexible (yet not error-prone) configuration.
 
-## Example
+## Story
 
-Suppose you wrote a package and you want to allow users to set package-level configs.
-
-Something like this:
+Suppose you wrote a package and you want to allow users to set package-level configs:
 
 ```python
 import awesomepackage
 from awesomepackage.foo import bar
 
 # user can change module param on the fly
 awesomepackage.config["logging"]["verbose"] = True
@@ -35,19 +33,19 @@
 
 This is simple, but maybe not any parameter can be changed at any time. For example:
 
 ```python
 awesomepackage.config["metric"]["length"] = "foot"
 ```
 
-Having flexible units may be helpful for different locales, but Changing metric units in the middle of a program can lead to consistency issues.
+Having flexible units may be helpful for different locales, but changing metric units in the middle of a program can lead to consistency issues.
 
 `flexmod` lets you:
 -   specify configs that are auto-locked (i.e. no further changes) when used
--   add custom preprocessing functions to entered config values
+-   add custom preprocessor functions to entered config values
     -   this is useful when reading config from a text file
 -   add validation functions to check user-supplied config values
 
 ## Usage
 
 ### Define configurations in your module using `flexmod` classes
 
@@ -72,16 +70,16 @@
 		    validation=lambda x: x in ["en-us", "fr-fr"],
 		),
 	        # example of a config that can change dynamically
 	    	ConfigValue(
 		    "verbosity",
 		    "The granularity to which the module reports / complains",
 		    1,
-		    # specify a preprocessing function if needed
-		    preprocessing=int,
+		    # specify a preprocessor function if needed
+		    preprocessor=int,
 		),
 	    ],
 	),
         Config(
 	    "foo",
 	    [
 	    	AutolockedConfigValue(
```

### Comparing `flexmod-0.1.1/README.md` & `flexmod-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # flexmod
 A python module for other modules to allow flexible (yet not error-prone) configuration.
 
-## Example
+## Story
 
-Suppose you wrote a package and you want to allow users to set package-level configs.
-
-Something like this:
+Suppose you wrote a package and you want to allow users to set package-level configs:
 
 ```python
 import awesomepackage
 from awesomepackage.foo import bar
 
 # user can change module param on the fly
 awesomepackage.config["logging"]["verbose"] = True
@@ -20,19 +18,19 @@
 
 This is simple, but maybe not any parameter can be changed at any time. For example:
 
 ```python
 awesomepackage.config["metric"]["length"] = "foot"
 ```
 
-Having flexible units may be helpful for different locales, but Changing metric units in the middle of a program can lead to consistency issues.
+Having flexible units may be helpful for different locales, but changing metric units in the middle of a program can lead to consistency issues.
 
 `flexmod` lets you:
 -   specify configs that are auto-locked (i.e. no further changes) when used
--   add custom preprocessing functions to entered config values
+-   add custom preprocessor functions to entered config values
     -   this is useful when reading config from a text file
 -   add validation functions to check user-supplied config values
 
 ## Usage
 
 ### Define configurations in your module using `flexmod` classes
 
@@ -57,16 +55,16 @@
 		    validation=lambda x: x in ["en-us", "fr-fr"],
 		),
 	        # example of a config that can change dynamically
 	    	ConfigValue(
 		    "verbosity",
 		    "The granularity to which the module reports / complains",
 		    1,
-		    # specify a preprocessing function if needed
-		    preprocessing=int,
+		    # specify a preprocessor function if needed
+		    preprocessor=int,
 		),
 	    ],
 	),
         Config(
 	    "foo",
 	    [
 	    	AutolockedConfigValue(
```

### Comparing `flexmod-0.1.1/flexmod/__init__.py` & `flexmod-0.1.2/flexmod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """
 Toolbox for your library to be dynamically configured by the user.
 Add defaults, hints, locks, preprocessors and validations for robustness.
 """
 import re
+import json
 import configparser
 from typing import Any, Callable, List
 from collections import defaultdict
 
 DUMMY_PREPROCESSOR = lambda x: x
 DUMMY_VALIDATION = lambda x: True
 
 def auto_interpret(text):
     """
     Automatic interpretation of a string.
     """
     if not isinstance(text, str):
         return text
 
+    # detect JSON body
+    try:
+        data = json.loads(text)
+        return data
+    except ValueError:
+        pass
+
+    # detect numbers and booleans
     if re.search(r"^\-?\d+$", text):
         return int(text)
     if re.search(r"^\-?\d+\.\d+$", text):
         return float(text)
     if re.search(r"(?i)^(yes|on|true)$", text):
         return True
     if re.search(r"(?i)^(no|off|false)$", text):
@@ -107,15 +116,16 @@
         self,
         name: str,
         values: List[ConfigValue],
     ):
         self.name = name
         self._data = dict()
         for _value in values:
-            assert isinstance(_value, ConfigValue)
+            assert isinstance(_value, ConfigValue), f"Expected ConfigValue, got {type(_value)}"
+            assert _value.name not in self._data, f"Duplicate key {_value.name}"
             self._data[_value.name] = _value
 
     def __getitem__(self, key):
         return self._data[key].value
 
     def __setitem__(self, key, value):
         self._data[key].value = value
@@ -147,15 +157,16 @@
         self,
         configs: List[Config],
     ):
         self._configs = dict()
         self._value_name_to_config_names = defaultdict(list)
         for _config in configs:
             # assign configs
-            assert isinstance(_config, Config)
+            assert isinstance(_config, Config), f"Expected Config, got {type(_config)}"
+            assert _config.name not in self._configs, f"Duplicate key {_config.name}"
             self._configs[_config.name] = _config
 
     def __getitem__(self, key):
         return self._configs[key]
 
     def load_override(self, ini_path):
         parser = configparser.ConfigParser()
```

### Comparing `flexmod-0.1.1/flexmod.egg-info/PKG-INFO` & `flexmod-0.1.2/flexmod.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module for other modules to allow flexible (yet not error-prone) configuration.
 Home-page: https://github.com/haochuanwei/flexmod
 Author: Haochuan Wei
 Author-email: pepsimixt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flexmod
 A python module for other modules to allow flexible (yet not error-prone) configuration.
 
-## Example
+## Story
 
-Suppose you wrote a package and you want to allow users to set package-level configs.
-
-Something like this:
+Suppose you wrote a package and you want to allow users to set package-level configs:
 
 ```python
 import awesomepackage
 from awesomepackage.foo import bar
 
 # user can change module param on the fly
 awesomepackage.config["logging"]["verbose"] = True
@@ -35,19 +33,19 @@
 
 This is simple, but maybe not any parameter can be changed at any time. For example:
 
 ```python
 awesomepackage.config["metric"]["length"] = "foot"
 ```
 
-Having flexible units may be helpful for different locales, but Changing metric units in the middle of a program can lead to consistency issues.
+Having flexible units may be helpful for different locales, but changing metric units in the middle of a program can lead to consistency issues.
 
 `flexmod` lets you:
 -   specify configs that are auto-locked (i.e. no further changes) when used
--   add custom preprocessing functions to entered config values
+-   add custom preprocessor functions to entered config values
     -   this is useful when reading config from a text file
 -   add validation functions to check user-supplied config values
 
 ## Usage
 
 ### Define configurations in your module using `flexmod` classes
 
@@ -72,16 +70,16 @@
 		    validation=lambda x: x in ["en-us", "fr-fr"],
 		),
 	        # example of a config that can change dynamically
 	    	ConfigValue(
 		    "verbosity",
 		    "The granularity to which the module reports / complains",
 		    1,
-		    # specify a preprocessing function if needed
-		    preprocessing=int,
+		    # specify a preprocessor function if needed
+		    preprocessor=int,
 		),
 	    ],
 	),
         Config(
 	    "foo",
 	    [
 	    	AutolockedConfigValue(
```

### Comparing `flexmod-0.1.1/setup.py` & `flexmod-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     else:
         desc = ""
     return desc
 
 
 setuptools.setup(
     name="flexmod",
-    version="0.1.1",
+    version="0.1.2",
     description="A module for other modules to allow flexible (yet not error-prone) configuration.",
     long_description=get_description(),
     long_description_content_type="text/markdown",
     author="Haochuan Wei",
     author_email="pepsimixt@gmail.com",
     url="https://github.com/haochuanwei/flexmod",
     packages=setuptools.find_packages(include=["flexmod*"]),
```

