# Comparing `tmp/application_properties-0.6.0.tar.gz` & `tmp/application_properties-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "application_properties-0.6.0.tar", last modified: Mon Apr 10 01:21:09 2023, max compression
+gzip compressed data, was "application_properties-0.7.0.tar", last modified: Sun Apr 23 21:02:14 2023, max compression
```

## Comparing `application_properties-0.6.0.tar` & `application_properties-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.989569 application_properties-0.6.0/
--rw-rw-rw-   0        0        0     1066 2022-08-24 23:33:16.000000 application_properties-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0       75 2022-08-24 23:33:16.000000 application_properties-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5862 2023-04-10 01:21:08.989569 application_properties-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    12928 2022-08-24 23:33:16.000000 application_properties-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.968567 application_properties-0.6.0/application_properties/
--rw-rw-rw-   0        0        0      553 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/__init__.py
--rw-rw-rw-   0        0        0    14116 2023-04-10 00:30:33.000000 application_properties-0.6.0/application_properties/application_properties.py
--rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/application_properties_facade.py
--rw-rw-rw-   0        0        0     2458 2023-04-09 23:30:24.000000 application_properties-0.6.0/application_properties/application_properties_json_loader.py
--rw-rw-rw-   0        0        0       13 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/py.typed
--rw-rw-rw-   0        0        0       65 2023-04-09 23:30:24.000000 application_properties-0.6.0/application_properties/version.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.977565 application_properties-0.6.0/application_properties.egg-info/
--rw-rw-rw-   0        0        0     5862 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2021-06-05 01:28:55.000000 application_properties-0.6.0/install-requirements.txt
--rw-rw-rw-   0        0        0      696 2023-04-10 01:21:08.995566 application_properties-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2691 2022-08-24 23:33:16.000000 application_properties-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.988569 application_properties-0.6.0/test/
--rw-rw-rw-   0        0        0    13948 2023-04-09 23:30:24.000000 application_properties-0.6.0/test/test_application_properties.py
--rw-rw-rw-   0        0        0     8524 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_application_properties_facade.py
--rw-rw-rw-   0        0        0     8742 2023-04-09 23:30:24.000000 application_properties-0.6.0/test/test_application_properties_json_loader.py
--rw-rw-rw-   0        0        0     3837 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_get_boolean.py
--rw-rw-rw-   0        0        0     3821 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_get_integer.py
--rw-rw-rw-   0        0        0     6155 2023-04-10 00:07:55.000000 application_properties-0.6.0/test/test_get_string.py
--rw-rw-rw-   0        0        0    12542 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_set_manual_property.py
--rw-rw-rw-   0        0        0      510 2021-06-05 04:57:29.000000 application_properties-0.6.0/test/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.370810 application_properties-0.7.0/
+-rw-rw-rw-   0        0        0     1066 2022-08-24 23:33:16.000000 application_properties-0.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       75 2022-08-24 23:33:16.000000 application_properties-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5862 2023-04-23 21:02:14.371812 application_properties-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12928 2022-08-24 23:33:16.000000 application_properties-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.352810 application_properties-0.7.0/application_properties/
+-rw-rw-rw-   0        0        0      893 2023-04-23 16:36:58.000000 application_properties-0.7.0/application_properties/__init__.py
+-rw-rw-rw-   0        0        0    17006 2023-04-23 03:07:39.000000 application_properties-0.7.0/application_properties/application_properties.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 13:51:18.000000 application_properties-0.7.0/application_properties/application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.7.0/application_properties/application_properties_facade.py
+-rw-rw-rw-   0        0        0     3048 2023-04-23 03:27:58.000000 application_properties-0.7.0/application_properties/application_properties_json_loader.py
+-rw-rw-rw-   0        0        0      955 2023-04-23 03:26:29.000000 application_properties-0.7.0/application_properties/application_properties_loader_helper.py
+-rw-rw-rw-   0        0        0     3566 2023-04-23 03:27:58.000000 application_properties-0.7.0/application_properties/application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0       13 2022-08-24 23:33:16.000000 application_properties-0.7.0/application_properties/py.typed
+-rw-rw-rw-   0        0        0       65 2023-04-23 02:12:55.000000 application_properties-0.7.0/application_properties/version.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.357810 application_properties-0.7.0/application_properties.egg-info/
+-rw-rw-rw-   0        0        0     5862 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-23 21:02:14.000000 application_properties-0.7.0/application_properties.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 13:44:16.000000 application_properties-0.7.0/install-requirements.txt
+-rw-rw-rw-   0        0        0      696 2023-04-23 21:02:14.372813 application_properties-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2691 2022-08-24 23:33:16.000000 application_properties-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:02:14.370810 application_properties-0.7.0/test/
+-rw-rw-rw-   0        0        0    13948 2023-04-09 23:30:24.000000 application_properties-0.7.0/test/test_application_properties.py
+-rw-rw-rw-   0        0        0    23261 2023-04-23 14:22:47.000000 application_properties-0.7.0/test/test_application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     8524 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_application_properties_facade.py
+-rw-rw-rw-   0        0        0    14040 2023-04-23 14:22:30.000000 application_properties-0.7.0/test/test_application_properties_json_loader.py
+-rw-rw-rw-   0        0        0    22990 2023-04-23 14:22:38.000000 application_properties-0.7.0/test/test_application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0     3837 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_get_boolean.py
+-rw-rw-rw-   0        0        0     3821 2022-08-24 23:33:16.000000 application_properties-0.7.0/test/test_get_integer.py
+-rw-rw-rw-   0        0        0     6155 2023-04-10 00:07:55.000000 application_properties-0.7.0/test/test_get_string.py
+-rw-rw-rw-   0        0        0     1437 2023-04-23 14:24:39.000000 application_properties-0.7.0/test/test_helpers.py
+-rw-rw-rw-   0        0        0    24230 2023-04-21 02:48:51.000000 application_properties-0.7.0/test/test_set_manual_property.py
+-rw-rw-rw-   0        0        0      510 2021-06-05 04:57:29.000000 application_properties-0.7.0/test/test_version.py
```

### Comparing `application_properties-0.6.0/LICENSE.txt` & `application_properties-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/PKG-INFO` & `application_properties-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: application_properties
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.6.0/README.md` & `application_properties-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/application_properties/__init__.py` & `application_properties-0.7.0/application_properties/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,13 +6,21 @@
 )
 from application_properties.application_properties_facade import (  # noqa F401
     ApplicationPropertiesFacade,
 )
 from application_properties.application_properties_json_loader import (  # noqa F401
     ApplicationPropertiesJsonLoader,
 )
+from application_properties.application_properties_toml_loader import (  # noqa F401
+    ApplicationPropertiesTomlLoader,
+)
+from application_properties.application_properties_config_loader import (  # noqa F401
+    ApplicationPropertiesConfigLoader,
+)
 
 __all__ = [
     "ApplicationProperties",
     "ApplicationPropertiesFacade",
     "ApplicationPropertiesJsonLoader",
+    "ApplicationPropertiesTomlLoader",
+    "ApplicationPropertiesConfigLoader",
 ]
```

### Comparing `application_properties-0.6.0/application_properties/application_properties.py` & `application_properties-0.7.0/application_properties/application_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Module that provides for an encapsulation of properties for an application.
 """
+
+import contextlib
 import copy
 import logging
-from typing import Any, Callable, Dict, List, Optional, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, cast
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ApplicationProperties:
     """
     Class that provides for an encapsulation of properties for an application.
@@ -20,68 +22,94 @@
     __manual_property_type_integer = "#"
     __manual_property_type_boolean = "!"
 
     """
     Class to provide for a container of properties that belong to the application.
     """
 
-    def __init__(self, strict_mode: bool = False) -> None:
+    def __init__(
+        self, strict_mode: bool = False, convert_untyped_if_possible: bool = False
+    ) -> None:
         """
         Initializes an new instance of the ApplicationProperties class.
         """
         self.__flat_property_map: Dict[str, Any] = {}
         self.__strict_mode: bool = strict_mode
+        self.__convert_untyped_if_possible: bool = convert_untyped_if_possible
 
     @property
     def separator(self) -> str:
         """
         Separator used to split the hierarchy of the property names.
         """
         return self.__separator
 
     @property
     def number_of_properties(self) -> int:
         """
         Number of properties that exist in the map.
         """
-        return len(self.__flat_property_map)
+        return len(self.property_names)
 
     @property
     def property_names(self) -> List[str]:
         """
         List of each of the properties in the map.
         """
-        return list(self.__flat_property_map.keys())
+        return [
+            next_item
+            for next_item in self.__flat_property_map
+            if not next_item.startswith(ApplicationProperties.__separator)
+        ]
 
     @property
     def strict_mode(self) -> bool:
         """
         Gets whether strict mode is on by default.
         """
         return self.__strict_mode
 
     def enable_strict_mode(self) -> None:
         """
-        Sets struct mode to True to enable it.
+        Sets strict mode to True to enable it.
         """
         self.__strict_mode = True
 
+    @property
+    def convert_untyped_if_possible(self) -> bool:
+        """
+        Gets whether the package is allowed to try and unconvert untyped entries.
+        """
+        return self.__convert_untyped_if_possible
+
+    def enable_convert_untyped_if_possible(self) -> None:
+        """
+        Sets convert_untyped_if_possible to True to enable it.
+        """
+        self.__convert_untyped_if_possible = True
+
+    def clear(self) -> None:
+        """
+        Clear the configuration map.
+        """
+        self.__flat_property_map.clear()
+
     def load_from_dict(
         self, config_map: Dict[Any, Any], clear_map: bool = True
     ) -> None:
         """
         Load the properties from a provided dictionary.
         """
 
         if not isinstance(config_map, dict):
             raise ValueError("Specified parameter was not a dictionary.")
 
         LOGGER.debug("Loading from dictionary: {%s}", str(config_map))
         if clear_map:
-            self.__flat_property_map.clear()
+            self.clear()
         self.__scan_map(config_map, "")
 
     @staticmethod
     def verify_full_part_form(property_key: str) -> str:
         """
         Given one part of a full key, verify that it is composed properly.
         """
@@ -99,32 +127,36 @@
         if not property_key:
             raise ValueError(
                 "Each part of the property key must contain at least one character."
             )
         return property_key
 
     @staticmethod
-    def verify_full_key_form(property_key: str) -> str:
+    def verify_full_key_form(
+        property_key: str, alternate_name: Optional[str] = None
+    ) -> str:
         """
         Given a full key, verify that it is composed properly.
         """
 
+        key_name = alternate_name or "Full property key"
+
         if property_key.startswith(
             ApplicationProperties.__separator
         ) or property_key.endswith(ApplicationProperties.__separator):
             raise ValueError(
-                f"Full property key must not start or end with the '{ApplicationProperties.__separator}' character."
+                f"{key_name} must not start or end with the '{ApplicationProperties.__separator}' character."
             )
         doubles = (
             f"{ApplicationProperties.__separator}{ApplicationProperties.__separator}"
         )
         doubles_index = property_key.find(doubles)
         if doubles_index != -1:
             raise ValueError(
-                "Full property key cannot contain multiples of "
+                f"{key_name} cannot contain multiples of "
                 + f"the {ApplicationProperties.__separator} without any text between them."
             )
         split_key = property_key.split(ApplicationProperties.__separator)
         for next_key in split_key:
             ApplicationProperties.verify_full_part_form(next_key)
         return property_key
 
@@ -173,14 +205,25 @@
         if (
             property_value.startswith(
                 ApplicationProperties.__manual_property_type_prefix
             )
             and len(property_value) >= 2
         ):
             composed_property_value = self.__adjust_property_type(property_value)
+
+        # This is a bit of a kludge, but it works consistently.  The manually set property
+        # is always a string.  If the string has no type information associatede with it,
+        # it is eligible for conversion into one of the other types.  To properly denote that
+        # the value did not have any type information, it is saved again in the dictionary
+        # with a prefix of the separator character, to denote eligibility.
+        else:
+            self.__flat_property_map[
+                f"{ApplicationProperties.__separator}{property_key}"
+            ] = property_value
+
         self.__flat_property_map[property_key] = copy.deepcopy(composed_property_value)
         LOGGER.debug(
             "Adding configuration '%s' : {%s}",
             property_key,
             str(composed_property_value),
         )
 
@@ -247,24 +290,50 @@
             )
         elif is_required:
             raise ValueError(
                 f"A value for property '{property_name}' must be provided."
             )
         return property_value
 
+    def __get_present_property_value(
+        self, property_name: str, property_type: type
+    ) -> Tuple[bool, Any]:
+        found_value = self.__flat_property_map[property_name]
+        is_eligible = type(found_value) == property_type
+
+        covertable_property_name = f"{ApplicationProperties.__separator}{property_name}"
+        if (
+            not is_eligible
+            and property_type != str
+            and self.__convert_untyped_if_possible
+            and covertable_property_name in self.__flat_property_map
+        ):
+            found_value = self.__flat_property_map[covertable_property_name]
+            # print(f"::{covertable_property_name}::{found_value}::")
+            if property_type == bool:
+                found_value = f"{ApplicationProperties.__manual_property_type_prefix}{ApplicationProperties.__manual_property_type_boolean}{found_value}"
+            else:
+                found_value = f"{ApplicationProperties.__manual_property_type_prefix}{ApplicationProperties.__manual_property_type_integer}{found_value}"
+            with contextlib.suppress(ValueError):
+                found_value = self.__adjust_property_type(found_value)
+                is_eligible = True
+            # print(f"::{covertable_property_name}::{found_value}::")
+        return is_eligible, found_value
+
     def __get_present_property(
         self,
         property_name: str,
         property_value: Any,
         property_type: type,
         strict_mode: bool,
         valid_value_fn: Optional[Callable[[Any], Any]],
     ) -> Any:
-        found_value = self.__flat_property_map[property_name]
-        is_eligible = type(found_value) == property_type
+        is_eligible, found_value = self.__get_present_property_value(
+            property_name, property_type
+        )
         if not is_eligible and strict_mode:
             raise ValueError(
                 f"The value for property '{property_name}' must be of type '{property_type.__name__}'."
             )
         if is_eligible and valid_value_fn:
             try:
                 valid_value_fn(found_value)
```

### Comparing `application_properties-0.6.0/application_properties/application_properties_facade.py` & `application_properties-0.7.0/application_properties/application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/application_properties.egg-info/PKG-INFO` & `application_properties-0.7.0/application_properties.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: application-properties
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.6.0/setup.cfg` & `application_properties-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/setup.py` & `application_properties-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/test/test_application_properties.py` & `application_properties-0.7.0/test/test_application_properties.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/test/test_application_properties_facade.py` & `application_properties-0.7.0/test/test_application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/test/test_application_properties_json_loader.py` & `application_properties-0.7.0/test/test_application_properties_json_loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,355 @@
 """
 Tests for the ApplicationProperties class
 """
 import io
 import json
 import os
 import sys
-import tempfile
+from test.test_helpers import TestHelpers
 
 from application_properties import (
     ApplicationProperties,
     ApplicationPropertiesJsonLoader,
 )
 
 
-def write_temporary_configuration(supplied_configuration):
+def test_json_loader_config_not_present():
     """
-    Write the configuration as a temporary file that is kept around.
+    Test to make sure that we do not try and load a configuration file that is not present.
     """
-    try:
-        with tempfile.NamedTemporaryFile("wt", delete=False) as outfile:
-            if isinstance(supplied_configuration, str):
-                outfile.write(supplied_configuration)
-            else:
-                json.dump(supplied_configuration, outfile)
-            return outfile.name
-    except IOError as ex:
-        raise AssertionError(
-            f"Test configuration file was not written ({str(ex)})."
-        ) from ex
+
+    # Arrange
+    configuration_file = "does-not-exist"
+    configuration_file = os.path.abspath(configuration_file)
+    assert not os.path.exists(configuration_file)
+    application_properties = ApplicationProperties()
+
+    expected_did_apply = False
+    expected_did_error = False
+    expected_value = -1
+
+    # Act
+    actual_did_apply, actual_did_error = ApplicationPropertiesJsonLoader.load_and_set(
+        application_properties, configuration_file, None, True, True
+    )
+    actual_value = application_properties.get_integer_property(
+        "plugins.md999.test_value", -1
+    )
+
+    # Assert
+    assert expected_value == actual_value
+    assert expected_did_error == actual_did_error
+    assert expected_did_apply == actual_did_apply
 
 
 def test_json_loader_valid_json():
     """
     Test to make sure that we can load a valid Json file.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test_value": 2}}}
     expected_value = 2
+    expected_did_apply = True
+    expected_did_error = False
 
     configuration_file = None
     try:
-        configuration_file = write_temporary_configuration(supplied_configuration)
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
         application_properties = ApplicationProperties()
 
         # Act
-        ApplicationPropertiesJsonLoader.load_and_set(
-            application_properties, configuration_file, None
+        (
+            actual_did_apply,
+            actual_did_error,
+        ) = ApplicationPropertiesJsonLoader.load_and_set(
+            application_properties, configuration_file
         )
         actual_value = application_properties.get_integer_property(
-            "plugins.md999.test_value", -1
+            "plugins.md999.test_value", -1, None
         )
 
         # Assert
         assert expected_value == actual_value
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
+    finally:
+        if configuration_file and os.path.exists(configuration_file):
+            os.remove(configuration_file)
+
+
+def test_json_loader_valid_json_but_wrong_get_property_type():
+    """
+    Test to make sure that we can load a valid Json file, even if the property
+    we are looking for is of the wrong type.  The load should succeed, even
+    if the get fails.
+    """
+
+    # Arrange
+    supplied_configuration = {"plugins": {"md999": {"test_value": "2"}}}
+    expected_error = (
+        "The value for property 'plugins.md999.test_value' must be of type 'int'."
+    )
+    expected_did_apply = True
+    expected_did_error = False
+
+    configuration_file = None
+    try:
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
+        application_properties = ApplicationProperties()
+
+        # Act
+        captured_exception = None
+        (
+            actual_did_apply,
+            actual_did_error,
+        ) = ApplicationPropertiesJsonLoader.load_and_set(
+            application_properties, configuration_file
+        )
+        try:
+            application_properties.get_integer_property(
+                "plugins.md999.test_value", -1, None, strict_mode=True
+            )
+        except ValueError as this_exception:
+            captured_exception = this_exception
+
+        # Assert
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
+        assert not application_properties.convert_untyped_if_possible
+        assert captured_exception is not None
+        assert str(captured_exception) == expected_error
+    finally:
+        if configuration_file and os.path.exists(configuration_file):
+            os.remove(configuration_file)
+
+
+def test_json_loader_valid_json_but_wrong_get_property_type_with_untyped_conversion():
+    """
+    Test to make sure that we can load a valid Json file, even if the property
+    we are looking for is of the wrong type.  The load should succeed, even
+    if the get fails.  The get should still fail as JSON is a typed source.
+    """
+
+    # Arrange
+    supplied_configuration = {"plugins": {"md999": {"test_value": "2"}}}
+    expected_error = (
+        "The value for property 'plugins.md999.test_value' must be of type 'int'."
+    )
+    expected_did_apply = True
+    expected_did_error = False
+
+    configuration_file = None
+    try:
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
+        application_properties = ApplicationProperties(convert_untyped_if_possible=True)
+
+        # Act
+        captured_exception = None
+        (
+            actual_did_apply,
+            actual_did_error,
+        ) = ApplicationPropertiesJsonLoader.load_and_set(
+            application_properties, configuration_file
+        )
+        try:
+            application_properties.get_integer_property(
+                "plugins.md999.test_value", -1, None, strict_mode=True
+            )
+        except ValueError as this_exception:
+            captured_exception = this_exception
+
+        # Assert
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
+        assert application_properties.convert_untyped_if_possible
+        assert captured_exception is not None
+        assert str(captured_exception) == expected_error
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
 def test_json_loader_invalid_json():
     """
     Test to make sure that we cannot load an invalid Json file.
     """
 
     # Arrange
     supplied_configuration = "this is not a json file"
+    expected_did_apply = False
+    expected_did_error = True
 
     handled_error_parameters = []
 
     def inner_func(formatted_error, this_exception):
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = None
     try:
-        configuration_file = write_temporary_configuration(supplied_configuration)
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
         application_properties = ApplicationProperties()
 
         # Act
-        ApplicationPropertiesJsonLoader.load_and_set(
+        (
+            actual_did_apply,
+            actual_did_error,
+        ) = ApplicationPropertiesJsonLoader.load_and_set(
             application_properties, configuration_file, handle_error_fn=inner_func
         )
 
         # Assert
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
         assert handled_error_parameters
         assert handled_error_parameters[0].startswith("Specified configuration file ")
         assert (
-            "' is not a valid JSON file (Expecting value: line 1 column 1 (char 0))."
+            "' is not a valid JSON file: Expecting value: line 1 column 1 (char 0)."
             in handled_error_parameters[0]
         )
         assert isinstance(handled_error_parameters[1], json.decoder.JSONDecodeError)
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
 def test_json_loader_missing_file():
     """
     Test to make sure that we fail to load a file that isn't there.
     """
 
     # Arrange
+    expected_did_apply = False
+    expected_did_error = True
     handled_error_parameters = []
 
     def inner_func(formatted_error, this_exception):
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = "missing_file_name.other"
     assert not os.path.exists(configuration_file)
     application_properties = ApplicationProperties()
 
     # Act
-    ApplicationPropertiesJsonLoader.load_and_set(
-        application_properties, configuration_file, handle_error_fn=inner_func
+    actual_did_apply, actual_did_error = ApplicationPropertiesJsonLoader.load_and_set(
+        application_properties,
+        configuration_file,
+        handle_error_fn=inner_func,
+        check_for_file_presence=False,
     )
 
     # Assert
+    assert expected_did_apply == actual_did_apply
+    assert expected_did_error == actual_did_error
     assert handled_error_parameters
     assert handled_error_parameters[0].startswith(
-        "Specified configuration file 'missing_file_name.other' was not loaded"
+        "Specified configuration file 'missing_file_name.other' was not loaded: "
     )
     assert isinstance(handled_error_parameters[1], FileNotFoundError)
 
 
 def test_json_loader_valid_json_but_invalid_key():
     """
     Test to make sure that we can load a valid Json file, but fail when there is an invalid key.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test.value": 2}}}
+    expected_did_apply = False
+    expected_did_error = True
 
     handled_error_parameters = []
 
     def inner_func(formatted_error, this_exception):
         handled_error_parameters.append(formatted_error)
         handled_error_parameters.append(this_exception)
 
     configuration_file = None
     try:
-        configuration_file = write_temporary_configuration(supplied_configuration)
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
         application_properties = ApplicationProperties()
 
         # Act
-        ApplicationPropertiesJsonLoader.load_and_set(
+        (
+            actual_did_apply,
+            actual_did_error,
+        ) = ApplicationPropertiesJsonLoader.load_and_set(
             application_properties, configuration_file, inner_func
         )
 
         # Assert
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
         assert handled_error_parameters
         assert handled_error_parameters[0].startswith("Specified configuration file '")
         assert (
-            "' is not valid (Keys strings cannot contain the separator character '.'.)."
+            "' is not valid: Keys strings cannot contain the separator character '.'."
             in handled_error_parameters[0]
         )
         assert isinstance(handled_error_parameters[1], ValueError)
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
 
-def test_json_loader_valid_json_but_invalid_key_xx():
+def test_json_loader_valid_json_but_invalid_key_with_stdin_capture():
     """
     Test to make sure that we can load a valid Json file, but fail when there is an invalid key.
     """
 
     # Arrange
     supplied_configuration = {"plugins": {"md999": {"test.value": 2}}}
+    expected_did_apply = False
+    expected_did_error = True
 
     configuration_file = None
     try:
-        configuration_file = write_temporary_configuration(supplied_configuration)
+        configuration_file = TestHelpers.write_temporary_configuration(
+            supplied_configuration
+        )
         application_properties = ApplicationProperties()
 
         # Act
         saved_stdout = sys.stdout
         saved_stderr = sys.stderr
         new_stdout = io.StringIO()
         new_stderr = io.StringIO()
         try:
             sys.stdout = new_stdout
             sys.stderr = new_stderr
 
-            ApplicationPropertiesJsonLoader.load_and_set(
+            (
+                actual_did_apply,
+                actual_did_error,
+            ) = ApplicationPropertiesJsonLoader.load_and_set(
                 application_properties, configuration_file
             )
         finally:
             sys.stdout = saved_stdout
             sys.stderr = saved_stderr
 
         # Assert
+        assert expected_did_apply == actual_did_apply
+        assert expected_did_error == actual_did_error
         assert new_stdout.getvalue().startswith("Specified configuration file '")
         assert (
-            "' is not valid (Keys strings cannot contain the separator character '.'.)."
+            "' is not valid: Keys strings cannot contain the separator character '.'."
             in new_stdout.getvalue()
         )
         assert not new_stderr.getvalue()
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
 
@@ -218,18 +369,18 @@
     }
     expected_value_a = 2
     expected_value_b = 4
     expected_value_c = 5
 
     configuration_file_first = None
     try:
-        configuration_file_first = write_temporary_configuration(
+        configuration_file_first = TestHelpers.write_temporary_configuration(
             supplied_configuration_first
         )
-        configuration_file_second = write_temporary_configuration(
+        configuration_file_second = TestHelpers.write_temporary_configuration(
             supplied_configuration_second
         )
         application_properties = ApplicationProperties()
 
         # Act
         ApplicationPropertiesJsonLoader.load_and_set(
             application_properties,
```

### Comparing `application_properties-0.6.0/test/test_get_boolean.py` & `application_properties-0.7.0/test/test_get_boolean.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/test/test_get_integer.py` & `application_properties-0.7.0/test/test_get_integer.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.6.0/test/test_get_string.py` & `application_properties-0.7.0/test/test_get_string.py`

 * *Files identical despite different names*

