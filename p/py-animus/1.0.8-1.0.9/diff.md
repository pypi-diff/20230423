# Comparing `tmp/py_animus-1.0.8.tar.gz` & `tmp/py_animus-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_animus-1.0.8.tar", last modified: Sat Apr  1 10:10:34 2023, max compression
+gzip compressed data, was "py_animus-1.0.9.tar", last modified: Thu Apr 20 18:02:40 2023, max compression
```

## Comparing `py_animus-1.0.8.tar` & `py_animus-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-01 10:10:34.106710 py_animus-1.0.8/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    35149 2023-02-23 07:18:01.000000 py_animus-1.0.8/LICENSE
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     8370 2023-04-01 10:10:34.106710 py_animus-1.0.8/PKG-INFO
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     7419 2023-03-18 13:34:38.000000 py_animus-1.0.8/README.md
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       80 2023-01-15 13:20:17.000000 py_animus-1.0.8/pyproject.toml
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1096 2023-04-01 10:10:34.106710 py_animus-1.0.8/setup.cfg
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-01 10:10:34.106710 py_animus-1.0.8/src/
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-01 10:10:34.106710 py_animus-1.0.8/src/py_animus/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     2598 2023-03-06 06:58:46.000000 py_animus-1.0.8/src/py_animus/__init__.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    52219 2023-03-26 07:05:34.000000 py_animus-1.0.8/src/py_animus/manifest_management.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     4716 2023-03-18 13:34:38.000000 py_animus-1.0.8/src/py_animus/py_animus.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1076 2023-04-01 10:08:32.000000 py_animus-1.0.8/src/py_animus/utils.py
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-01 10:10:34.106710 py_animus-1.0.8/src/py_animus.egg-info/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     8370 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/PKG-INFO
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      434 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/SOURCES.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)        1 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/dependency_links.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       56 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/entry_points.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       16 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/requires.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       10 2023-04-01 10:10:34.000000 py_animus-1.0.8/src/py_animus.egg-info/top_level.txt
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-01 10:10:34.106710 py_animus-1.0.8/tests/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    45930 2023-03-19 10:55:21.000000 py_animus-1.0.8/tests/test_manifest_management.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     7114 2023-04-01 10:08:32.000000 py_animus-1.0.8/tests/test_utiles.py
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-20 18:02:40.904814 py_animus-1.0.9/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    35149 2023-02-23 07:18:01.000000 py_animus-1.0.9/LICENSE
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     8370 2023-04-20 18:02:40.904814 py_animus-1.0.9/PKG-INFO
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     7419 2023-03-18 13:34:38.000000 py_animus-1.0.9/README.md
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       80 2023-04-01 12:01:33.000000 py_animus-1.0.9/pyproject.toml
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1096 2023-04-20 18:02:40.908814 py_animus-1.0.9/setup.cfg
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-20 18:02:40.904814 py_animus-1.0.9/src/
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-20 18:02:40.904814 py_animus-1.0.9/src/py_animus/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     2598 2023-04-19 18:08:23.000000 py_animus-1.0.9/src/py_animus/__init__.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    67023 2023-04-20 18:01:40.000000 py_animus-1.0.9/src/py_animus/manifest_management.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     6252 2023-04-20 18:01:40.000000 py_animus-1.0.9/src/py_animus/py_animus.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1076 2023-04-01 10:12:57.000000 py_animus-1.0.9/src/py_animus/utils.py
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-20 18:02:40.904814 py_animus-1.0.9/src/py_animus.egg-info/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     8370 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/PKG-INFO
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      434 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)        1 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       56 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/entry_points.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       16 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/requires.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       10 2023-04-20 18:02:40.000000 py_animus-1.0.9/src/py_animus.egg-info/top_level.txt
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-20 18:02:40.904814 py_animus-1.0.9/tests/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    64666 2023-04-20 18:01:40.000000 py_animus-1.0.9/tests/test_manifest_management.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     7114 2023-04-01 10:12:57.000000 py_animus-1.0.9/tests/test_utiles.py
```

### Comparing `py_animus-1.0.8/LICENSE` & `py_animus-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_animus-1.0.8/PKG-INFO` & `py_animus-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_animus
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python based plugable and extensible manifest processing system
 Home-page: https://github.com/nicc777/py-animus
 Author: Nico Coetzee
 Author-email: nicc777@gmail.com
 Project-URL: Bug Tracker, https://github.com/nicc777/py-animus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py_animus-1.0.8/README.md` & `py_animus-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py_animus-1.0.8/setup.cfg` & `py_animus-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_animus
-version = 1.0.8
+version = 1.0.9
 author = Nico Coetzee
 author_email = nicc777@gmail.com
 description = A python based plugable and extensible manifest processing system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicc777/py-animus
 project_urls =
```

### Comparing `py_animus-1.0.8/src/py_animus/__init__.py` & `py_animus-1.0.9/src/py_animus/__init__.py`

 * *Files identical despite different names*

### Comparing `py_animus-1.0.8/src/py_animus/manifest_management.py` & `py_animus-1.0.9/src/py_animus/manifest_management.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
-    Copyright (c) 2023. All rights reserved. NS Coetzee <nicc777@gmail.com>
+    Copyright (c) 2023. All rights reserved. NS Coetzee <nicc777`@`gmail.com>
 
     This file is licensed under GPLv3 and a copy of the license should be included in the project (look for the file 
     called LICENSE), or alternatively view the license text at 
     https://raw.githubusercontent.com/nicc777/verbacratis/main/LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt
 """
 
 import copy
 import traceback
 import hashlib
 import json
 import yaml
 import importlib, os, inspect
 import sys
-from py_animus import get_logger, get_utc_timestamp, is_debug_set_in_environment
+import re
+from py_animus import get_logger, get_utc_timestamp, is_debug_set_in_environment, parse_raw_yaml_data
 
 
 def get_modules_in_package(target_dir: str, logger=get_logger()):
     files = os.listdir(target_dir)
     sys.path.insert(0,target_dir)
     for file in files:
         if file not in ['__init__.py', '__pycache__']:
@@ -32,14 +33,104 @@
                     yield (clazz, name)
 
 
 def dummy_manifest_lookup_function(name: str):  # pragma: no cover
     return
 
 
+class ValuePlaceholder:
+
+    def __init__(self, placeholder_name: str):
+        self.placeholder_name = placeholder_name
+        self.per_environment_values = dict()
+
+    def add_environment_value(self, environment_name: str, value: object):
+        self.per_environment_values[environment_name] = value
+
+    def get_environment_value(self, environment_name: str, default_value_when_not_found: object=None, raise_exception_when_not_found: bool=True):
+        if environment_name not in self.per_environment_values:
+            if raise_exception_when_not_found is True:
+                raise Exception('No value for environment "{}" for value placeholder "{}" found'.format(environment_name, self.placeholder_name))
+            return default_value_when_not_found
+        return copy.deepcopy(self.per_environment_values[environment_name])
+    
+    def to_dict(self):
+        data = dict()
+        data['name'] = self.placeholder_name
+        data['environments'] = list()
+        for env_name, env_val in self.per_environment_values.items():
+            pev = dict()
+            pev['environmentName'] = env_name
+            pev['value'] = env_val
+            data['environments'].append(copy.deepcopy(pev))
+        return data
+
+
+class ValuePlaceHolders:
+
+    def __init__(self, logger=get_logger()):
+        self.value_placeholder_names = dict()
+        self.logger = logger
+
+    def value_placeholder_exists(self, placeholder_name: str)->bool:
+        if placeholder_name in self.value_placeholder_names:
+            return True
+        return False
+
+    def get_value_placeholder(self, placeholder_name: str, create_in_not_exists: bool=True)->ValuePlaceholder:
+        if self.value_placeholder_exists(placeholder_name=placeholder_name) is False and create_in_not_exists is True:
+            return self.create_new_value_placeholder(placeholder_name=placeholder_name)
+        elif self.value_placeholder_exists(placeholder_name=placeholder_name) is False and create_in_not_exists is False:
+            raise Exception('ValuePlaceholder named "{}" not found'.format(placeholder_name))
+        return copy.deepcopy(self.value_placeholder_names[placeholder_name])
+
+    def create_new_value_placeholder(self, placeholder_name: str)->ValuePlaceholder:
+        vp = ValuePlaceholder(placeholder_name=placeholder_name)
+        self.value_placeholder_names[placeholder_name] = copy.deepcopy(vp)
+        return copy.deepcopy(vp)
+    
+    def add_environment_value(self, placeholder_name: str, environment_name: str, value: object):
+        vp = self.get_value_placeholder(placeholder_name=placeholder_name, create_in_not_exists=True)
+        vp.add_environment_value(environment_name=environment_name, value=value)
+        self.value_placeholder_names[placeholder_name] = copy.deepcopy(vp)
+
+    def to_dict(self):
+        data = dict()
+        data['values'] = list()
+        for vp_name in list(self.value_placeholder_names.keys()):
+            vp = self.get_value_placeholder(placeholder_name=vp_name)
+            data['values'].append(vp.to_dict())
+        return data
+
+    def parse_and_replace_placeholders_in_string(
+            self,
+            input_str: str,
+            environment_name: str,
+            default_value_when_not_found: object='',
+            raise_exception_when_not_found: bool=False
+        ):
+        self.logger.debug('Parsing for placeholders. input_str="{}'.format(input_str))
+        return_str = copy.deepcopy(input_str)
+        if input_str.find('{}{} .Values.'.format('{', '{')) >= 0:
+            for matched_placeholder in re.findall('\{\{\s+\.Values\.([\w|\s|\-|\_|\.]+)\s+\}\}', input_str):
+                return_str = return_str.replace(
+                    '{}{} .Values.{} {}{}'.format('{', '{', matched_placeholder, '}', '}'),
+                    self.get_value_placeholder(
+                        placeholder_name=matched_placeholder,
+                        create_in_not_exists=True
+                    ).get_environment_value(
+                        environment_name=environment_name,
+                        default_value_when_not_found=default_value_when_not_found,
+                        raise_exception_when_not_found=raise_exception_when_not_found
+                    )
+                )
+        self.logger.debug('   return_str="{}'.format(return_str))
+        return return_str
+
+
 class Variable:
     """A Variable is a runtime value generated by some operation that will be stored in a VariableCache in the 
     ManifestManager. Any other operation launched from the ManifestManager will have access to the current runtime 
     sVariable values.
 
     Within the user implementation of some class that extends ManifestBase, a method called apply_manifest() can update
     the VariableCache with a new Variable or change the value of an existing Variable.
@@ -347,14 +438,16 @@
         self.supported_versions = supported_versions
         self.debug = is_debug_set_in_environment()
         self.logger = logger
         self.initialized = False
         self.post_parsing_method = post_parsing_method
         self.checksum = None
         self.dependency_processing_counter = dict()
+        self.target_environments = ['default',]
+        self.original_manifest = dict()
 
     def log(self, message: str, level: str='info'): # pragma: no cover
         """During implementation, calls to `self.log()` can be made to log messages using the configure logger.
 
         The log level is supplied as an argument, with the default level being 'info'
 
         Args:
@@ -370,22 +463,48 @@
         elif level.lower().startswith('i'):
             self.logger.info('[{}:{}:{}] {}'.format(self.kind, name, self.version, message))
         elif level.lower().startswith('w'):
             self.logger.warning('[{}:{}:{}] {}'.format(self.kind, name, self.version, message))
         elif level.lower().startswith('e'):
             self.logger.error('[{}:{}:{}] {}'.format(self.kind, name, self.version, message))
 
-    def parse_manifest(self, manifest_data: dict):
+    def _process_dict_for_value_placeholders(self, d: dict, value_placeholders: ValuePlaceHolders, environment_name: str)->dict:
+        final_d = dict()
+        for k,v in d.items():
+            if isinstance(v, dict):
+                final_d[k] = copy.deepcopy(self._process_dict_for_value_placeholders(d=v, value_placeholders=value_placeholders, environment_name=environment_name))
+            elif isinstance(v, str):
+                final_d[k] = copy.deepcopy(
+                    value_placeholders.parse_and_replace_placeholders_in_string(
+                        input_str=v,
+                        environment_name=environment_name,
+                        default_value_when_not_found=v,
+                        raise_exception_when_not_found=False
+                    )
+                )
+            else:
+                final_d[k] = copy.deepcopy(v)
+        return final_d
+
+    def process_value_placeholders(self, value_placeholders: ValuePlaceHolders, environment_name: str):
+        manifest_data_with_parsed_value_placeholder_values = self._process_dict_for_value_placeholders(d=copy.deepcopy(self.original_manifest), value_placeholders=value_placeholders, environment_name=environment_name)
+        self.log(message='manifest_data_with_parsed_value_placeholder_values={}'.format(manifest_data_with_parsed_value_placeholder_values), level='debug')
+        self.metadata = copy.deepcopy(manifest_data_with_parsed_value_placeholder_values['metadata'])
+        self.spec = copy.deepcopy(manifest_data_with_parsed_value_placeholder_values['spec'])
+
+    def parse_manifest(self, manifest_data: dict, target_environments: list=['default',]):
         """Called via the ManifestManager when manifests files are parsed and one is found to belong to a class of this implementation.
 
         The user does not have to override this implementation.
 
         Args:
           manifest_data: A Dictionary of data from teh parsed Manifest file
         """
+        self.target_environments = target_environments
+        self.original_manifest = copy.deepcopy(manifest_data)
         converted_data = dict((k.lower(),v) for k,v in manifest_data.items()) # Convert keys to lowercase
         if 'kind' in converted_data:
             if converted_data['kind'] != self.kind:
                 self.log(message='Kind mismatch. Got "{}" and expected "{}"'.format(converted_data['kind'], self.kind), level='error')
                 return
         else:
             self.log(message='Kind property not present in data. Data={}'.format(manifest_data), level='error')
@@ -426,25 +545,35 @@
         self,
         action: str,
         process_dependency_if_already_applied: bool,
         process_dependency_if_not_already_applied: bool,
         manifest_lookup_function: object=dummy_manifest_lookup_function,
         variable_cache: VariableCache=VariableCache(),
         process_self_post_dependency_processing: bool=True,
-        dependency_processing_rounds: dict=dict()
+        dependency_processing_rounds: dict=dict(),
+        target_environment: str='default', 
+        value_placeholders: ValuePlaceHolders=ValuePlaceHolders()
     ):
         """Called via the ManifestManager just before calling the `apply_manifest()` or `delete_manifest()`
 
         Looks at `metadata.dependencies.*` to determine which other manifests has to be processed before the main action for this manifest is processed
 
         Args:
           action: String with the appropriate command by which the lookup in `metadata.dependencies.*` will be done
+          process_dependency_if_already_applied: bool, If set to True, will process dependencies again, even if it was previously processed (as determined by the implemented_manifest_differ_from_this_manifest() method)
+          process_dependency_if_not_already_applied: bool, If set to true, process dependencies
           manifest_lookup_function: A function passed in by the ManifestManager. Called with `manifest_lookup_function(name='...')`. Implemented in ManifestManager.get_manifest_instance_by_name()
           variable_cache: A reference to the current instance of the VariableCache
+          process_self_post_dependency_processing: bool=True, If set to True, run own apply/delete actions
+          dependency_processing_rounds: dict that tracks how many times processing happened in order to limit endless processing loops.
+          target_environment: string with the target environment
+          value_placeholders: ValuePlaceHolders instance that contains the per environment placeholder values that will be passed on during processing in order for final field values to be determined.
         """
+        if target_environment not in self.metadata['environments']:
+            return
         if 'dependencies' in self.metadata:
 
             if self.metadata['name'] not in dependency_processing_rounds:
                 dependency_processing_rounds[self.metadata['name']] = 1
             else:
                 dependency_processing_rounds[self.metadata['name']] += 1
             if dependency_processing_rounds[self.metadata['name']] > 2:
@@ -452,15 +581,15 @@
                 raise Exception('Possible recursion detected')
             
             if action in self.metadata['dependencies']:
                 for dependant_manifest_name in self.metadata['dependencies'][action]:
                     self.log(message='Processing dependency named "{}" for manifest "{}" while processing action "{}"'.format(dependant_manifest_name, self.metadata['name'], action), level='debug')
                     
                     dependency_manifest_implementation = manifest_lookup_function(name=dependant_manifest_name)
-                    dependency_manifest_applied_previously = not dependency_manifest_implementation.implemented_manifest_differ_from_this_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache)
+                    dependency_manifest_applied_previously = not dependency_manifest_implementation.implemented_manifest_differ_from_this_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache, target_environment=target_environment, value_placeholders=value_placeholders)
                     self.log(
                         message='Dependency named "{}" previously applied: {}'.format(
                             dependency_manifest_implementation.metadata['name'],
                             dependency_manifest_applied_previously
                         ),
                         level='debug'
                     )
@@ -469,42 +598,48 @@
                         dependency_manifest_implementation.process_dependencies(
                             action=action,
                             manifest_lookup_function=manifest_lookup_function,
                             variable_cache=variable_cache,
                             process_self_post_dependency_processing=process_self_post_dependency_processing,
                             process_dependency_if_already_applied=process_dependency_if_already_applied,
                             process_dependency_if_not_already_applied=process_dependency_if_not_already_applied,
-                            dependency_processing_rounds=dependency_processing_rounds
+                            dependency_processing_rounds=dependency_processing_rounds,
+                            target_environment=target_environment,
+                            value_placeholders=value_placeholders
                         )
                     else:
                         self.log(message='Dependency named "{}" will NOT be applied because process_dependency_if_already_applied is FALSE'.format(dependency_manifest_implementation.metadata['name']),level='debug')   
                     if dependency_manifest_applied_previously == process_dependency_if_not_already_applied:
                         self.log(message='Dependency named "{}" will be applied because process_dependency_if_not_already_applied is TRUE'.format(dependency_manifest_implementation.metadata['name']),level='debug')   
                         dependency_manifest_implementation.process_dependencies(
                             action=action,
                             manifest_lookup_function=manifest_lookup_function,
                             variable_cache=variable_cache,
                             process_self_post_dependency_processing=process_self_post_dependency_processing,
                             process_dependency_if_already_applied=process_dependency_if_already_applied,
                             process_dependency_if_not_already_applied=process_dependency_if_not_already_applied,
-                            dependency_processing_rounds=dependency_processing_rounds
+                            dependency_processing_rounds=dependency_processing_rounds,
+                            target_environment=target_environment,
+                            value_placeholders=value_placeholders
                         )
                     else:
                         self.log(message='Dependency named "{}" will be applied because process_dependency_if_not_already_applied is FALSE'.format(dependency_manifest_implementation.metadata['name']),level='debug')   
 
             else:
                 self.log(message='No dependencies for action "{}" for manifest "{}"'.format(action, self.metadata['name']), level='warning')
         else:
             self.log(message='No dependencies for manifest "{}" while processing action "{}"'.format(self.metadata['name'], action), level='debug')
 
         if process_self_post_dependency_processing is True:
             if action == 'apply':
-                self.apply_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache)
+                self.process_value_placeholders(value_placeholders=value_placeholders, environment_name=target_environment)
+                self.apply_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache, target_environment=target_environment, value_placeholders=value_placeholders)
             if action == 'delete':
-                self.delete_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache)
+                self.process_value_placeholders(value_placeholders=value_placeholders, environment_name=target_environment)
+                self.delete_manifest(manifest_lookup_function=manifest_lookup_function, variable_cache=variable_cache, target_environment=target_environment, value_placeholders=value_placeholders)
         else:
             self.log(message='SELF was NOT YET PROCESSED for manifest "{}" while processing action "{}"'.format(self.metadata['name'], action), level='debug')
 
     def to_dict(self):
         """When the user or some other part of the systems required the data as a Dict, for example when to produce a
         YAML file.
 
@@ -525,15 +660,15 @@
         """Produces a YAML representation of the class attributes
 
         Returns:
             A String in YAML format
         """
         return yaml.dump(self.to_dict())
 
-    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache())->bool:    # pragma: no cover
+    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders())->bool:    # pragma: no cover
         """A helper method to determine if the current manifest is different from a potentially previously implemented
         version
 
         The exact logic to derive the checksum of any previous implementation is left to the user. Ideally, calls
         should be made to determine some prior implementation that can reconstruct the original manifest from where the
         checksum can be calculated and compared to the current checksum.
 
@@ -548,28 +683,41 @@
         previous_implementation_data['spec'] = dict()
         // add data to previous_implementation_data['spec'] from a prior implementation as required
         if  hashlib.sha256(json.dumps(previous_implementation_data, sort_keys=True, ensure_ascii=True).encode('utf-8')).hexdigest() != self.checksum:
             return True
         return False
         ```
 
+        **IMPORTANT** It is up to the implementation to parse the per target placeholder values. Consider the following example:
+
+        ```python
+        # Assuming we have a spec field called "name" (self.spec['name']), we can ensure the final value is set with:
+        final_name = value_placeholders.parse_and_replace_placeholders_in_string(
+            input_str=self.spec['name'],
+            environment_name=target_environment,
+            default_value_when_not_found='what_ever_is_appropriate'
+        )
+        ```
+
         Args:
           manifest_lookup_function: A function passed in by the ManifestManager. Called with `manifest_lookup_function(name='...')`. Implemented in ManifestManager.get_manifest_instance_by_name()
           variable_cache: A reference to the current instance of the VariableCache
+          target_environment: string with the name of the target environment (default="default") (New since version 1.0.9)
+          value_placeholders: ValuePlaceHolders instance containing all the per environment replacement values (New since version 1.0.9)
 
         Returns:
-            Boolean True if the previous implementation checksum is different from the current manifest checksum.
+            Boolean True if the previous implementation is different from the current implementation
 
         Raises:
             Exception: When the method was not implemented by th user
             Exception: As determined by the user
         """
         raise Exception('To be implemented by user')
 
-    def apply_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False):  # pragma: no cover
+    def apply_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False, target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders()):  # pragma: no cover
         """A  method to Implement the state as defined in a manifest.
 
         The ManifestManager will typically call this method to apply the manifest. The ManifestManager will NOT make a
         prior call to implemented_manifest_differ_from_this_manifest() and it is up to the user implementation of this
         method to determine if prior changes need to be taken into consideration. A common pattern during
         implementation is therefore:
 
@@ -593,29 +741,42 @@
         ```python
         // Assuming we define our parent/dependency in the manifest as "spec.parent"
         parent_manifest = manifest_lookup_function(name=self.spec['parent'])    // Get an instance of ManifestBase implementation with teh provided name
         parent_manifest.apply_manifest(variable_cache=variable_cache)           // Ensure it is applied
         // Consume output from parent_manifest as stored in the variable_cache as needed...
         ```
 
+        **IMPORTANT** It is up to the implementation to parse the per target placeholder values. Consider the following example:
+
+        ```python
+        # Assuming we have a spec field called "name" (self.spec['name']), we can ensure the final value is set with:
+        final_name = value_placeholders.parse_and_replace_placeholders_in_string(
+            input_str=self.spec['name'],
+            environment_name=target_environment,
+            default_value_when_not_found='what_ever_is_appropriate'
+        )
+        ```
+
         Args:
           manifest_lookup_function: A function passed in by the ManifestManager. Called with `manifest_lookup_function(name='...')`. Implemented in ManifestManager.get_manifest_instance_by_name()
           variable_cache: A reference to the current instance of the VariableCache
           increment_exec_counter: If set to true, the implementation should make the following call: `self.apply_execute_count += 1`
+          target_environment: string with the name of the target environment (default="default") (New since version 1.0.9)
+          value_placeholders: ValuePlaceHolders instance containing all the per environment replacement values (New since version 1.0.9)
 
         Returns:
             Any returned value will be ignored by the ManifestManager
 
         Raises:
             Exception: When the method was not implemented by th user
             Exception: As determined by the user
         """
         raise Exception('To be implemented by user')
     
-    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False):  # pragma: no cover
+    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False, target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders()):  # pragma: no cover
         """A  method to DELETE the current state as defined in a manifest.
 
         The ManifestManager will typically call this method to delete the manifest. The ManifestManager will NOT make a
         prior call to implemented_manifest_differ_from_this_manifest() and it is up to the user implementation of this
         method to determine if prior changes need to be taken into consideration. A common pattern during
         implementation is therefore:
 
@@ -639,18 +800,31 @@
         ```python
         // Assuming we define our parent/dependency in the manifest as "spec.parent"
         parent_manifest = manifest_lookup_function(name=self.spec['parent'])    // Get an instance of ManifestBase implementation with teh provided name
         parent_manifest.apply_manifest(variable_cache=variable_cache)           // Ensure it is applied (or deleted, as required in this specific context)
         // Consume output from parent_manifest as stored in the variable_cache as needed...
         ```
 
+        **IMPORTANT** It is up to the implementation to parse the per target placeholder values. Consider the following example:
+
+        ```python
+        # Assuming we have a spec field called "name" (self.spec['name']), we can ensure the final value is set with:
+        final_name = value_placeholders.parse_and_replace_placeholders_in_string(
+            input_str=self.spec['name'],
+            environment_name=target_environment,
+            default_value_when_not_found='what_ever_is_appropriate'
+        )
+        ```
+
         Args:
           manifest_lookup_function: A function passed in by the ManifestManager. Called with `manifest_lookup_function(name='...')`. Implemented in ManifestManager.get_manifest_instance_by_name()
           variable_cache: A reference to the current instance of the VariableCache
           increment_exec_counter: If set to true, the implementation should make the following call: `self.delete_execute_count += 1`
+          target_environment: string with the name of the target environment (default="default") (New since version 1.0.9)
+          value_placeholders: ValuePlaceHolders instance containing all the per environment replacement values (New since version 1.0.9)
 
         Returns:
             Any returned value will be ignored by the ManifestManager
 
         Raises:
             Exception: When the method was not implemented by th user
             Exception: As determined by the user
@@ -815,36 +989,68 @@
             if dr.src in dst_deps:
                 return True
         return False
 
 
 class ManifestManager:
 
-    def __init__(self, variable_cache: VariableCache, logger=get_logger(), max_calls_to_manifest: int=int(os.getenv('MAX_CALLS_TO_MANIFEST', '10'))):
+    def __init__(
+            self,
+            variable_cache: VariableCache,
+            logger=get_logger(),
+            max_calls_to_manifest: int=int(os.getenv('MAX_CALLS_TO_MANIFEST', '10')),
+            environments: list=['default',],
+            values_files: list=['values.yaml',]
+        ):
         self.versioned_class_register = VersionedClassRegister(logger=logger)
         self.manifest_instances = dict()
         self.manifest_data_by_manifest_name = dict()
         self.variable_cache = variable_cache
         self.logger = logger
         self.apply_drs = DependencyReferences()
         self.delete_drs = DependencyReferences()
         self.max_calls_to_manifest = max_calls_to_manifest
         self.executions_per_manifest_instance = dict()
+        self.environments = environments
+        self.environment_values = ValuePlaceHolders(logger=logger)
+        self._load_values(files=values_files)
+
+    def _load_values_from_file(self, file: str):
+        try:
+            self.logger.info('Attempting to load values from file "{}"'.format(file))
+            with open(file, 'r') as f:
+                data = parse_raw_yaml_data(yaml_data=f.read(), logger=self.logger)
+            if 'values' in  data:
+                for value in data['values']:
+                    if 'name' in value and 'environments' in value:
+                        for env_name, env_val in value['environments'].items():
+                            self.environment_values.add_environment_value(placeholder_name=value['name'], environment_name=env_name, value=env_val)
+            self.logger.info('   Loaded values from file "{}"'.format(file))
+        except:
+            self.logger.error('Failed to load values from file "{}"'.format(file))
+
+    def _load_values(self, files: list):
+        try:
+            for file in files:
+                self._load_values_from_file(file=file)
+        except:
+            self.logger.error('Failed to load values from files. files: {}'.format(files))
+        self.logger.debug('LOADED environment_values: {}'.format(json.dumps(self.environment_values.to_dict())))
 
     def register_manifest_class(self, manifest_base: ManifestBase):
         if isinstance(manifest_base, ManifestBase) is False:
             raise Exception('Incorrect Base Class')
         self.versioned_class_register.add_class(clazz=manifest_base)
 
     def load_manifest_class_definition_from_file(self, plugin_file_path: str):
         for returned_class, kind in get_modules_in_package(target_dir=plugin_file_path, logger=self.logger):
              self.register_manifest_class(manifest_base=returned_class(logger=self.logger))
         self.logger.info('Registered classes: {}'.format(str(self.versioned_class_register)))
 
-    def get_manifest_instance_by_name(self, name: str):
+    def get_manifest_instance_by_name(self, name: str)->ManifestBase:
         for key, manifest_instance in self.manifest_instances.items():
             if manifest_instance.metadata['name'] == name or '{}:{}:{}'.format(manifest_instance.metadata['name'],manifest_instance.version,manifest_instance.checksum) == name:
                 return manifest_instance
         raise Exception('No manifest instance for "{}" found'.format(name))
     
     def _record_manifest_instance_call(self, name: str):
         if name in self.executions_per_manifest_instance:
@@ -859,25 +1065,39 @@
         else:
             self.executions_per_manifest_instance[manifest_instance.metadata['name']] = 0
         return False
     
     def _can_execute_again(self, manifest_instance: ManifestBase)->bool:
         return not self._max_execution_count_reached(manifest_instance=manifest_instance)
 
-    def apply_manifest(self, name: str, skip_dependency_processing: bool=False):
+    def apply_manifest(self, name: str, skip_dependency_processing: bool=False, target_environment: str='default'):
         manifest_instance = self.get_manifest_instance_by_name(name=name)
-        self.logger.debug('ManifestManager.apply_manifest(): manifest_instance named "{}" loaded.'.format(manifest_instance.metadata['name']))
+        if target_environment not in manifest_instance.metadata['environments']:
+            return
+        self.logger.debug('ManifestManager.apply_manifest(): manifest_instance named "{}" loaded. Target environment set to "{}"'.format(manifest_instance.metadata['name'], target_environment))
+
+        do_apply_in_environment = False
+        for te in self.environments:
+            self.logger.debug('* EVAL: te="{}" == target_environment="{}"'.format(te, target_environment))
+            if te == target_environment:
+                if te in manifest_instance.metadata['environments']:
+                    self.logger.info('ManifestManager.apply_manifest(): manifest_instance named "{}" targeted for environment "{}"'.format(manifest_instance.metadata['name'], te))    
+                    do_apply_in_environment = True
+        if do_apply_in_environment is False:
+            self.logger.warning('ManifestManager.apply_manifest(): manifest_instance named "{}" loaded not selected for target environment "{}". Skipping.'.format(manifest_instance.metadata['name'], target_environment))
+            return
 
         if 'skipApplyAll' in manifest_instance.metadata:
             if manifest_instance.metadata['skipApplyAll'] is True:
                 self.logger.warning('ManifestManager:apply_manifest(): Manifest named "{}" skipped because of skipApplyAll setting'.format(manifest_instance.metadata['name']))
                 return
 
         if skip_dependency_processing is True:
-            manifest_instance.apply_manifest(manifest_lookup_function=self.get_manifest_instance_by_name, variable_cache=self.variable_cache)
+            manifest_instance.process_value_placeholders(value_placeholders=self.environment_values, environment_name=target_environment)
+            manifest_instance.apply_manifest(manifest_lookup_function=self.get_manifest_instance_by_name, variable_cache=self.variable_cache, target_environment=target_environment, value_placeholders=self.environment_values)
             return
         
         if 'executeOnlyOnceOnApply' in manifest_instance.metadata:
             if manifest_instance.metadata['executeOnlyOnceOnApply'] is True and self.executions_per_manifest_instance[manifest_instance.metadata['name']] > 0:
                 self.logger.warning('ManifestManager:apply_manifest(): Manifest named "{}" skipped because executeOnlyOnceOnApply is TRUE and it was already executed before'.format(manifest_instance.metadata['name']))
                 return
 
@@ -889,28 +1109,43 @@
 
         manifest_instance.process_dependencies(
             action='apply',
             process_dependency_if_already_applied=False,
             process_dependency_if_not_already_applied=True,
             manifest_lookup_function=self.get_manifest_instance_by_name,
             variable_cache=self.variable_cache,
-            process_self_post_dependency_processing=True
+            process_self_post_dependency_processing=True,
+            target_environment=target_environment
         )
 
-    def delete_manifest(self, name: str, skip_dependency_processing: bool=False):
+    def delete_manifest(self, name: str, skip_dependency_processing: bool=False, target_environment: str='default'):
         manifest_instance = self.get_manifest_instance_by_name(name=name)
-        self.logger.debug('ManifestManager.delete_manifest(): manifest_instance named "{}" loaded.'.format(manifest_instance.metadata['name']))
+        if target_environment not in manifest_instance.metadata['environments']:
+            return
+        self.logger.debug('ManifestManager.delete_manifest(): manifest_instance named "{}" loaded.. Target environment set to "{}"'.format(manifest_instance.metadata['name'], target_environment))
+
+        do_delete_in_environment = False
+        for te in self.environments:
+            self.logger.debug('* EVAL: te="{}" == target_environment="{}"'.format(te, target_environment))
+            if te == target_environment:
+                if te in manifest_instance.metadata['environments']:
+                    self.logger.info('ManifestManager.delete_manifest(): manifest_instance named "{}" targeted for environment "{}"'.format(manifest_instance.metadata['name'], te))    
+                    do_delete_in_environment = True
+        if do_delete_in_environment is False:
+            self.logger.warning('ManifestManager.delete_manifest(): manifest_instance named "{}" loaded not selected for target environment "{}". Skipping.'.format(manifest_instance.metadata['name'], target_environment))
+            return
 
         if 'skipDeleteAll' in manifest_instance.metadata:
             if manifest_instance.metadata['skipDeleteAll'] is True:
                 self.logger.warning('ManifestManager:delete_manifest(): Manifest named "{}" skipped because of skipDeleteAll setting'.format(manifest_instance.metadata['name']))
                 return
 
         if skip_dependency_processing is True:
-            manifest_instance.delete_manifest(manifest_lookup_function=self.get_manifest_instance_by_name, variable_cache=self.variable_cache)
+            manifest_instance.process_value_placeholders(value_placeholders=self.environment_values, environment_name=target_environment)
+            manifest_instance.delete_manifest(manifest_lookup_function=self.get_manifest_instance_by_name, variable_cache=self.variable_cache, target_environment=target_environment, value_placeholders=self.environment_values)
             return
         
         if 'executeOnlyOnceOnDelete' in manifest_instance.metadata:
             if manifest_instance.metadata['executeOnlyOnceOnDelete'] is True and self.executions_per_manifest_instance[manifest_instance.metadata['name']] > 0:
                 self.logger.warning('ManifestManager:delete_manifest(): Manifest named "{}" skipped because executeOnlyOnceOnDelete is TRUE and it was already executed before'.format(manifest_instance.metadata['name']))
                 return
         
@@ -922,30 +1157,33 @@
         
         manifest_instance.process_dependencies(
             action='delete',
             process_dependency_if_already_applied=True,
             process_dependency_if_not_already_applied=False,
             manifest_lookup_function=self.get_manifest_instance_by_name,
             variable_cache=self.variable_cache,
-            process_self_post_dependency_processing=True
+            process_self_post_dependency_processing=True,
+            target_environment=target_environment
         )
 
     def get_manifest_class_by_kind(self, kind: str, version: str=None):
         if version is None:
             raise Exception('Version is required')
         return self.versioned_class_register.get_version_of_class(kind=kind, version=version)
     
     def parse_manifest(self, manifest_data: dict):
         manifest_data = dict((k.lower(), v) for k,v in manifest_data.items())   # Convert first level keys to lower case
         version = None
         if 'version' in manifest_data:
             version = manifest_data['version']
         class_instance_copy = copy.deepcopy(self.get_manifest_class_by_kind(kind=manifest_data['kind'], version=version))
+        if 'environments' not in manifest_data['metadata']:
+            manifest_data['metadata']['environments'] = ['default',]
 
-        class_instance_copy.parse_manifest(manifest_data=manifest_data)
+        class_instance_copy.parse_manifest(manifest_data=manifest_data, target_environments=self.environments)
         idx = '{}:{}:{}'.format(
             class_instance_copy.metadata['name'],
             class_instance_copy.version,
             class_instance_copy.checksum
         )
 
         if class_instance_copy.metadata['name'] not in self.executions_per_manifest_instance:
```

### Comparing `py_animus-1.0.8/src/py_animus/py_animus.py` & `py_animus-1.0.9/src/py_animus/py_animus.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,32 +35,58 @@
         nargs='*',
         dest='src_locations',
         metavar='LOCATION',
         type=str, 
         required=True,
         help='[REQUIRED] One or more Python files that implement the logic to handle the manifest files.'
     )
+    parser.add_argument(
+        '-e', '--env',
+        action='append',
+        nargs='*',
+        dest='environments',
+        metavar='ENVIRONMENT',
+        type=str, 
+        required=False,
+        default='default',
+        help='[OPTIONAL] One or more environments to target. Environment will be synchronized one at a time.'
+    )
+    parser.add_argument(
+        '-f', '--file',
+        action='append',
+        nargs='*',
+        dest='values_files',
+        metavar='VALUES_FILE',
+        type=str, 
+        required=False,
+        default='/tmp/values/values.yaml',
+        help='[OPTIONAL] One or more values files to use for environment variable substitution.'
+    )
     logger.info('Returning CLI Argument Parser')
     return parser
 
 
-def apply_command(vc: VariableCache, mm: ManifestManager, logger):
-    for name in tuple(mm.manifest_instances.keys()):
-        logger.info('Applying manifest named "{}"'.format(name))
-        mm.apply_manifest(name=name)
-    for name in tuple(vc.values.keys()):
-        logger.info('RESULT: {}={}'.format(name, vc.get_value(variable_name=name, for_logging=True)))
-
-
-def delete_command(vc: VariableCache, mm: ManifestManager, logger):
-    for name in tuple(mm.manifest_instances.keys()):
-        logger.info('Deleting manifest named "{}"'.format(name))
-        mm.delete_manifest(name=name)
-    for name in tuple(vc.values.keys()):
-        logger.info('RESULT: {}={}'.format(name, vc.get_value(variable_name=name, for_logging=True)))
+def apply_command(vc: VariableCache, mm: ManifestManager, logger, target_environments: list=['default',]):
+    for target_environment in target_environments:
+        logger.info('TARGET ENVIRONMENT: {}'.format(target_environment))
+        for name in tuple(mm.manifest_instances.keys()):
+            logger.info('Applying manifest named "{}"'.format(name))
+            mm.apply_manifest(name=name, target_environment=target_environment)
+        for name in tuple(vc.values.keys()):
+            logger.info('RESULT: {}={}'.format(name, vc.get_value(variable_name=name, for_logging=True)))
+
+
+def delete_command(vc: VariableCache, mm: ManifestManager, logger, target_environments: list=['default',]):
+    for target_environment in target_environments:
+        logger.info('TARGET ENVIRONMENT: {}'.format(target_environment))
+        for name in tuple(mm.manifest_instances.keys()):
+            logger.info('Deleting manifest named "{}"'.format(name))
+            mm.delete_manifest(name=name, target_environment=target_environment)
+        for name in tuple(vc.values.keys()):
+            logger.info('RESULT: {}={}'.format(name, vc.get_value(variable_name=name, for_logging=True)))
 
 
 def main(command: str, cli_args: list, logger=get_logger()):
     logger.info('ok')
     if command.lower().startswith('--h') or command.lower().startswith('-h'):
         cli_args=['-h', ]
     args = dict()
@@ -69,19 +95,24 @@
     parsed_args, unknown_args = parser.parse_known_args(cli_args)
     
     if not command:
         raise Exception('Expected command "apply" or "delete"')
     if command not in ('apply', 'delete'):
         raise Exception('Command must be one of "apply" or "delete"')
     
+    target_environments = parsed_args.environments
+    values_files = parsed_args.values_files
+    
     logger.debug('Command line arguments parsed...')
-    logger.debug('   parsed_args: {}'.format(parsed_args))
-    logger.debug('   unknown_args: {}'.format(unknown_args))
+    logger.debug('   parsed_args         : {}'.format(parsed_args))
+    logger.debug('   unknown_args        : {}'.format(unknown_args))
+    logger.debug('   target_environments : {}'.format(target_environments))
+    logger.debug('   values_files        : {}'.format(values_files))
     vc = VariableCache()
-    mm = ManifestManager(variable_cache=vc)
+    mm = ManifestManager(variable_cache=vc, environments=target_environments, values_files=values_files)
     for src_file_list in parsed_args.src_locations:
         for src_file in src_file_list:
             logger.debug('Ingesting source file {}'.format(src_file))
             mm.load_manifest_class_definition_from_file(plugin_file_path=src_file)
     for manifest_file_list in parsed_args.manifest_locations:
         for manifest_file in manifest_file_list:
             try:
@@ -91,18 +122,19 @@
                 parsed_data = parse_raw_yaml_data(yaml_data=data, logger=logger)
                 for part_id, data_as_dict in parsed_data.items():
                     if 'version' in data_as_dict and 'kind' in data_as_dict and 'metadata' in data_as_dict:
                         mm.parse_manifest(manifest_data=data_as_dict)
             except:
                 logger.error('Failed to read file "{}" due to exception'.format(manifest_file))
                 logger.error(traceback.format_exc())
+    
     if command == 'apply':
-        apply_command(vc, mm, logger)
+        apply_command(vc, mm, logger, target_environments=target_environments)
     elif command == 'delete':
-        delete_command(vc, mm, logger)
+        delete_command(vc, mm, logger, target_environments=target_environments)
     else:
         raise Exception('Unknown command. Command must be one of "apply" or "delete"')
 
 
 def run_main():
     command = '-h'
     cli_args = list()
```

### Comparing `py_animus-1.0.8/src/py_animus/utils.py` & `py_animus-1.0.9/src/py_animus/utils.py`

 * *Files identical despite different names*

### Comparing `py_animus-1.0.8/src/py_animus.egg-info/PKG-INFO` & `py_animus-1.0.9/src/py_animus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-animus
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python based plugable and extensible manifest processing system
 Home-page: https://github.com/nicc777/py-animus
 Author: Nico Coetzee
 Author-email: nicc777@gmail.com
 Project-URL: Bug Tracker, https://github.com/nicc777/py-animus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py_animus-1.0.8/tests/test_manifest_management.py` & `py_animus-1.0.9/tests/test_manifest_management.py`

 * *Files 18% similar despite different names*

```diff
@@ -199,25 +199,25 @@
     return
 
 class MyManifest1(ManifestBase):
 
     def __init__(self, logger=get_logger(), post_parsing_method: object = my_post_parsing_method, version: str='v0.1', supported_versions: tuple=('v0.1',)):
         super().__init__(logger=logger, post_parsing_method=post_parsing_method, version=version, supported_versions=supported_versions)
 
-    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function)->bool:
+    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, target_environment: str='default')->bool:
         return True # We are always different
 
-    def apply_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False):
+    def apply_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False, target_environment: str='default'):
         variable_cache.store_variable(variable=Variable(name='{}:{}'.format(self.kind, self.metadata['name']), initial_value='Some Result Worth Saving'))
         variable_cache.store_variable(variable=Variable(name='{}:{}-val'.format(self.kind, self.metadata['name']), initial_value=self.spec['val']), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-applied'.format(self.kind, self.metadata['name']), initial_value=True), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-deleted'.format(self.kind, self.metadata['name']), initial_value=False), overwrite_existing=True)
         return  # Assume some implementation
     
-    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False):
+    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False, target_environment: str='default'):
         variable_cache.store_variable(variable=Variable(name='{}:{}'.format(self.kind, self.metadata['name']), initial_value='Some Result Worth Saving'))
         variable_cache.store_variable(variable=Variable(name='{}:{}-val'.format(self.kind, self.metadata['name']), initial_value=None), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-applied'.format(self.kind, self.metadata['name']), initial_value=False), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-deleted'.format(self.kind, self.metadata['name']), initial_value=True), overwrite_existing=True)
         return  
     
 
@@ -243,28 +243,28 @@
 
 
 class MyManifest2(ManifestBase):
 
     def __init__(self, logger=get_logger(), post_parsing_method: object = my_post_parsing_method, version: str='v0.2', supported_versions: tuple=('v0.2',)):
         super().__init__(logger=logger, post_parsing_method=post_parsing_method, version=version, supported_versions=supported_versions)
 
-    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function)->bool:
+    def implemented_manifest_differ_from_this_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders())->bool:
         return True # We are always different
 
-    def apply_manifest(self, manifest_lookup_function: object=manifest_lookup_that_always_returns_MyManifest1, variable_cache: VariableCache=VariableCache()):
+    def apply_manifest(self, manifest_lookup_function: object=manifest_lookup_that_always_returns_MyManifest1, variable_cache: VariableCache=VariableCache(), target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders()):
         if 'parent' in self.spec:
             m1 = manifest_lookup_function(name=self.spec['parent'])
             m1.apply_manifest(variable_cache=variable_cache)
         variable_cache.store_variable(variable=Variable(name='{}:{}'.format(self.kind, self.metadata['name']), initial_value='Another value worth storing'))
         variable_cache.store_variable(variable=Variable(name='{}:{}-val'.format(self.kind, self.metadata['name']), initial_value=self.spec['val']), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-applied'.format(self.kind, self.metadata['name']), initial_value=True), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-deleted'.format(self.kind, self.metadata['name']), initial_value=False), overwrite_existing=True)
         return  # Assume some implementation
     
-    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False):
+    def delete_manifest(self, manifest_lookup_function: object=dummy_manifest_lookup_function, variable_cache: VariableCache=VariableCache(), increment_exec_counter: bool=False, target_environment: str='default', value_placeholders: ValuePlaceHolders=ValuePlaceHolders()):
         variable_cache.store_variable(variable=Variable(name='{}:{}'.format(self.kind, self.metadata['name']), initial_value='Some Result Worth Saving'))
         variable_cache.store_variable(variable=Variable(name='{}:{}-val'.format(self.kind, self.metadata['name']), initial_value=None), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-applied'.format(self.kind, self.metadata['name']), initial_value=False), overwrite_existing=True)
         variable_cache.store_variable(variable=Variable(name='{}:{}-deleted'.format(self.kind, self.metadata['name']), initial_value=True), overwrite_existing=True)
         return
 
 
@@ -1154,14 +1154,126 @@
         ###
         ### Mimic the main() function delete all call
         ###
         for name in tuple(mm.manifest_instances.keys()):
             print('Deleting manifest named "{}"'.format(name))
             mm.delete_manifest(name=name, skip_dependency_processing=True)
 
+    @mock.patch.dict(os.environ, {"DEBUG": "1"})        
+    def test_manifests_with_multiple_environments_and_only_one_environment_selected(self):
+        ###
+        ### Manifest Setup
+        ###
+
+        manifest_1_v01_a_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-1
+    environments:
+    - env1
+    - env2
+    - env3
+spec:
+    val: 1
+"""
+
+        # THIS ONE SHOULD NOT BE APPLIED... MISSING env3
+        manifest_1_v01_b_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-2
+    environments:
+    - env1
+    - env2
+spec:
+    val: 1
+"""
+
+        manifest_1_v01_c_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-3
+    environments:
+    - env2
+    - env3
+spec:
+    val: 1
+"""
+
+        ###
+        ### Init VariableCache and ManifestManager
+        ###
+        vc = VariableCache()
+        mm = ManifestManager(variable_cache=vc, max_calls_to_manifest=1, environments=['env3',])
+
+        ###
+        ### Consume classes that extend ManifestBase and register with ManifestManager
+        ###
+        mm.load_manifest_class_definition_from_file(plugin_file_path='/tmp/test_manifest_classes/test1')
+        mm.load_manifest_class_definition_from_file(plugin_file_path='/tmp/test_manifest_classes/test2')
+        self.assertEqual(len(mm.versioned_class_register.classes), 6)
+
+        ###
+        ### Consume Manifests and link with class implementations registered in ManifestManager
+        ###
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=manifest_1_v01_a_data)['part_1'])
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=manifest_1_v01_b_data)['part_1'])
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=manifest_1_v01_c_data)['part_1'])
+
+        ###
+        ### Mimic the main() function apply all call
+        ###
+        print()
+        print('#################### APPLY ####################')
+        for target_environment in ('env3',):
+            print('   >>> Target Environment: {}'.format(target_environment))
+            for name in tuple(mm.manifest_instances.keys()):
+                print('---------- Applying manifest named "{}"'.format(name))
+                mm.apply_manifest(name=name, skip_dependency_processing=True, target_environment=target_environment)
+        mm.executions_per_manifest_instance = dict()
+        
+        ###
+        ### Mimic the main() function delete all call
+        ###
+        print()
+        print('#################### DELETE ####################')
+        for target_environment in ('env3',):
+            print('   >>> Target Environment: {}'.format(target_environment))
+            for name in tuple(mm.manifest_instances.keys()):
+                print('---------- Deleting manifest named "{}"'.format(name))
+                mm.delete_manifest(name=name, skip_dependency_processing=True, target_environment=target_environment)
+
+        vc_dict = vc.to_dict()
+
+        print()
+        print('#################### RESULTS ####################')
+        print('   vc_dict={}'.format(json.dumps(vc_dict)))
+
+        ### Validate Target Environments - test1-2 should not be applied or deleted
+        manifest_names = ('test1-1', 'test1-2', 'test1-3', )
+        target_environments = {
+            'applied': ('test1-1', 'test1-3', ),
+            'deleted': ('test1-1', 'test1-3', ),
+        }
+        for action in tuple(target_environments.keys()):
+            for manifest_name in manifest_names:
+                variable_name = 'MyManifest1:{}-{}'.format(manifest_name, action)
+                print('> Testing variable "{}" for action "{}"'.format(variable_name, action))
+                if manifest_name not in target_environments[action]:
+                    print('>   Manifest "{}" NOT targeted for action "{}"'.format(manifest_name, action))
+                    self.assertEqual(manifest_name, 'test1-2', 'Expected manifest named test1-2')
+                else:
+                    print('>   Manifest "{}" targeted for action "{}"'.format(manifest_name, action))
+                    variable_value = vc.get_value(variable_name=variable_name, value_if_expired=None, default_value_if_not_found=None, raise_exception_on_expired=False, raise_exception_on_not_found=False)
+                    self.assertIsNotNone(variable_value, 'Not expecting a None for variable name "{}" for action "{}"'.format(variable_name, action))
+                    self.assertTrue(variable_value)
+
 
 class TestVersionedClassRegister(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print('-'*80)
 
     def test_init_with_defaults(self):
@@ -1199,14 +1311,306 @@
         v1 = registry.get_version_of_class(kind='Test', version='v1')
         self.assertEqual(c2, v1)
         self.assertNotEqual(c1, v1)
         self.assertNotEqual(c3, v1)
         self.assertEqual(c2.version, 'v3')
 
 
+class TestValuePlaceholder(unittest.TestCase):    # pragma: no cover
+
+    def setUp(self):
+        print('-'*80)
+
+    def test_init_with_defaults(self):
+        vp = ValuePlaceholder(placeholder_name='test1')
+        self.assertIsNotNone(vp)
+        self.assertIsInstance(vp, ValuePlaceholder)
+        self.assertEqual(vp.placeholder_name, 'test1')
+
+    def test_two_environments(self):
+        vp = ValuePlaceholder(placeholder_name='test1')
+        vp.add_environment_value(environment_name='e1', value='v1')
+        vp.add_environment_value(environment_name='e2', value='v2')
+        self.assertIsNotNone(vp.per_environment_values)
+        self.assertTrue('e1' in vp.per_environment_values)
+        self.assertTrue('e2' in vp.per_environment_values)
+        self.assertEqual(vp.per_environment_values['e1'], 'v1')
+        self.assertEqual(vp.per_environment_values['e2'], 'v2')
+
+        print('vp={}'.format(json.dumps(vp.to_dict())))
+
+    def test_get_value(self):
+        vp = ValuePlaceholder(placeholder_name='test1')
+        vp.add_environment_value(environment_name='e1', value='v1')
+        vp.add_environment_value(environment_name='e2', value='v2')
+        v1 = vp.get_environment_value(environment_name='e1')
+        v2 = vp.get_environment_value(environment_name='e2')
+        self.assertEqual(v1, 'v1')
+        self.assertEqual(v2, 'v2')
+
+    def test_to_dict(self):
+        """
+            Expecting {"name": "test1", "environments": [{"environmentName": "e1", "value": "v1"}, {"environmentName": "e2", "value": "v2"}]}
+        """
+        vp = ValuePlaceholder(placeholder_name='test1')
+        vp.add_environment_value(environment_name='e1', value='v1')
+        vp.add_environment_value(environment_name='e2', value='v2')
+        d = vp.to_dict()
+        self.assertIsNotNone(d)
+        self.assertIsInstance(d, dict)
+        self.assertTrue('name' in d)
+        self.assertTrue('environments' in d)
+        self.assertEqual(d['name'], 'test1')
+        self.assertIsInstance(d['environments'], list)
+        self.assertEqual(len(d['environments']), 2)
+        for envs in d['environments']:
+            self.assertTrue('environmentName' in envs)
+            self.assertTrue('value' in envs)
+
+
+class TestValuePlaceHolders(unittest.TestCase):    # pragma: no cover
+
+    def setUp(self):
+        print('-'*80)
+
+    def test_init_with_defaults(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        self.assertIsNotNone(vps)
+        self.assertIsInstance(vps, ValuePlaceHolders)
+
+    def test_init_set_two_place_holders_each_with_two_same_environments(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val3')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val4')
+
+        d = vps.to_dict()
+        self.assertIsNotNone(d)
+        self.assertIsInstance(d, dict)
+        self.assertTrue(len(d) > 0)
+        print('d={}'.format(json.dumps(d)))
+
+        """
+            Expecting {"values": [{"name": "test1", "environments": [{"environmentName": "env1", "value": "val1"}, {"environmentName": "env2", "value": "val2"}]}, {"name": "test2", "environments": [{"environmentName": "env1", "value": "val3"}, {"environmentName": "env2", "value": "val4"}]}]}
+        """
+        self.assertTrue('values' in d)
+        self.assertIsInstance(d['values'], list)
+        for item in d['values']:
+            self.assertIsInstance(item, dict)
+            self.assertTrue('name' in item)
+            self.assertTrue('environments' in item)
+            self.assertIsInstance(item['environments'], list)
+            for item_env in item['environments']:
+                self.assertTrue('environmentName' in item_env)
+                self.assertTrue('value' in item_env)
+
+        v1 = vps.get_value_placeholder(placeholder_name='test1').get_environment_value(environment_name='env1')
+        v2 = vps.get_value_placeholder(placeholder_name='test1').get_environment_value(environment_name='env2')
+        v3 = vps.get_value_placeholder(placeholder_name='test2').get_environment_value(environment_name='env1')
+        v4 = vps.get_value_placeholder(placeholder_name='test2').get_environment_value(environment_name='env2')
+        self.assertEqual(v1, 'val1')
+        self.assertEqual(v2, 'val2')
+        self.assertEqual(v3, 'val3')
+        self.assertEqual(v4, 'val4')
+
+    def test_get_default_variable_value_for_missing_environment_value(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        value = vps.get_value_placeholder(placeholder_name='test1').get_environment_value(environment_name='env2', default_value_when_not_found=123, raise_exception_when_not_found=False)
+        self.assertIsInstance(value, int)
+        self.assertEqual(value, 123)
+
+    def test_string_parsing_simple_string_in_matches_str_out(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val3')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val4')
+
+        final_str = vps.parse_and_replace_placeholders_in_string(
+            input_str='abc',
+            environment_name='env1'
+        )
+        self.assertEqual(final_str, 'abc')
+
+    def test_string_parsing_env_string_in_parsed_correctly_01(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val3')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val4')
+
+        final_str = vps.parse_and_replace_placeholders_in_string(
+            input_str='{}{} .Values.test2 {}{}'.format('{','{','}','}'),
+            environment_name='env1'
+        )
+        self.assertEqual(final_str, 'val3')
+
+    def test_string_parsing_env_string_in_parsed_correctly_02(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val3')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val4')
+
+        final_str = vps.parse_and_replace_placeholders_in_string(
+            input_str='abc{}{} .Values.test2 {}{}def'.format('{','{','}','}'),
+            environment_name='env1'
+        )
+        self.assertEqual(final_str, 'abcval3def')
+
+    def test_string_parsing_env_string_in_parsed_correctly_03(self):
+        vps = ValuePlaceHolders(logger=get_logger())
+        vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val3')
+        vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val4')
+
+        final_str = vps.parse_and_replace_placeholders_in_string(
+            input_str='1: {}{} .Values.test1 {}{} and 2: {}{} .Values.test2 {}{}'.format('{','{','}','}','{','{','}','}'),
+            environment_name='env1'
+        )
+        self.assertEqual(final_str, '1: val1 and 2: val3')
+
+
+class TestValuePlaceHoldersScenarios(unittest.TestCase):    # pragma: no cover
+
+    def setUp(self):
+        print('-'*80)
+        self.manifest_1_v01_a_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-1
+    environments:
+    - env1
+    - env2
+    - env3
+spec:
+    val: '{}{} .Values.test1 {}{}'
+""".format('{','{','}','}')
+
+        # THIS ONE SHOULD NOT BE APPLIED... MISSING env3
+        self.manifest_1_v01_b_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-2
+    environments:
+    - env1
+    - env2
+spec:
+    val: '{}{} .Values.test2 {}{}'
+""".format('{','{','}','}')
+
+        self.manifest_1_v01_c_data =  """---
+kind: MyManifest1
+version: v0.1
+metadata:
+    name: test1-3
+    environments:
+    - env2
+    - env3
+spec:
+    val: '{}{} .Values.test3 {}{}'
+""".format('{','{','}','}')
+        
+        self.vps = ValuePlaceHolders(logger=get_logger())
+        self.vps.add_environment_value(placeholder_name='test1', environment_name='env1', value='val1')
+        self.vps.add_environment_value(placeholder_name='test1', environment_name='env2', value='val2')
+        self.vps.add_environment_value(placeholder_name='test1', environment_name='env3', value='val3')
+        self.vps.add_environment_value(placeholder_name='test2', environment_name='env1', value='val4')
+        self.vps.add_environment_value(placeholder_name='test2', environment_name='env2', value='val5')
+        self.vps.add_environment_value(placeholder_name='test2', environment_name='env3', value='val6')
+        self.vps.add_environment_value(placeholder_name='test3', environment_name='env1', value='val7')
+        self.vps.add_environment_value(placeholder_name='test3', environment_name='env2', value='val8')
+        self.vps.add_environment_value(placeholder_name='test3', environment_name='env3', value='val9')
+
+        if os.path.exists('/tmp/test_manifest_classes'):
+            if os.path.isdir(s='/tmp/test_manifest_classes'):
+                shutil.rmtree(path='/tmp/test_manifest_classes', ignore_errors=True)
+        os.mkdir(path='/tmp/test_manifest_classes')
+        os.mkdir(path='/tmp/test_manifest_classes/test1')
+        os.mkdir(path='/tmp/test_manifest_classes/test2')
+
+        self.source_to_dest_files = {
+            # MyManifest1 versions
+            '{}/tests/manifest_classes/test1v0-1.py'.format(running_path): '/tmp/test_manifest_classes/test1/test1v0-1.py',
+            '{}/tests/manifest_classes/test1v0-2.py'.format(running_path): '/tmp/test_manifest_classes/test1/test1v0-2.py',
+            '{}/tests/manifest_classes/test1v0-3.py'.format(running_path): '/tmp/test_manifest_classes/test1/test1v0-3.py',
+
+            # MyManifest2 versions
+            '{}/tests/manifest_classes/test2v0-1.py'.format(running_path): '/tmp/test_manifest_classes/test2/test2v0-1.py',
+            '{}/tests/manifest_classes/test2v0-2.py'.format(running_path): '/tmp/test_manifest_classes/test2/test2v0-2.py',
+            '{}/tests/manifest_classes/test2v0-3.py'.format(running_path): '/tmp/test_manifest_classes/test2/test2v0-3.py',
+        }
+
+        for source_file, dest_file in self.source_to_dest_files.items():
+            with open(source_file, 'r') as f1r:
+                with open(dest_file, 'w') as f1w:
+                    f1w.write(f1r.read())
+                    print('Copied "{}" to "{}"'.format(source_file, dest_file))
+
+        
+        print('PREP COMPLETED')
+        print('~'*80)
+
+    def tearDown(self):
+        if os.path.exists('/tmp/test_manifest_classes'):
+            if os.path.isdir(s='/tmp/test_manifest_classes'):
+                shutil.rmtree(path='/tmp/test_manifest_classes', ignore_errors=True)
+
+    # @mock.patch.dict(os.environ, {"DEBUG": "1"})   
+    def test_init_with_defaults(self):
+        ###
+        ### Init VariableCache and ManifestManager
+        ###
+        vc = VariableCache()
+        mm = ManifestManager(variable_cache=vc, max_calls_to_manifest=1, environments=['env3',])
+        mm.environment_values = self.vps
+
+        ###
+        ### Consume classes that extend ManifestBase and register with ManifestManager
+        ###
+        mm.load_manifest_class_definition_from_file(plugin_file_path='/tmp/test_manifest_classes/test1')
+        mm.load_manifest_class_definition_from_file(plugin_file_path='/tmp/test_manifest_classes/test2')
+        self.assertEqual(len(mm.versioned_class_register.classes), 6)
+
+        ###
+        ### Consume Manifests and link with class implementations registered in ManifestManager
+        ###
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=self.manifest_1_v01_a_data)['part_1'])
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=self.manifest_1_v01_b_data)['part_1'])
+        mm.parse_manifest(manifest_data=parse_raw_yaml_data(yaml_data=self.manifest_1_v01_c_data)['part_1'])
+
+        ###
+        ### Mimic the main() function apply all call
+        ###
+        print()
+        print('#################### APPLY ####################')
+        for target_environment in ('env3',):
+            print('   >>> Target Environment: {}'.format(target_environment))
+            for name in tuple(mm.manifest_instances.keys()):
+                print('---------- Applying manifest named "{}"'.format(name))
+                mm.apply_manifest(name=name, skip_dependency_processing=True, target_environment=target_environment)
+        mm.executions_per_manifest_instance = dict()
+
+        vc_data = vc.to_dict()
+        print()
+        print()
+        print('vc={}'.format(json.dumps(vc_data)))
+        print()
+        print()
+
+        self.assertEqual(vc_data['MyManifest1:test1-1-val']['value'], 'val3')
+        self.assertEqual(vc_data['MyManifest1:test1-3-val']['value'], 'val9')
+
+
+
 class TestDependencyReferences(unittest.TestCase):    # pragma: no cover
 
     def setUp(self):
         print('-'*80)
 
     def test_direct_dependency_negative_test(self):
         drs = DependencyReferences()
```

### Comparing `py_animus-1.0.8/tests/test_utiles.py` & `py_animus-1.0.9/tests/test_utiles.py`

 * *Files identical despite different names*

