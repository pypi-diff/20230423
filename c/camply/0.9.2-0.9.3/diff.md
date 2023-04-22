# Comparing `tmp/camply-0.9.2.tar.gz` & `tmp/camply-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camply-0.9.2.tar", max compression
+gzip compressed data, was "camply-0.9.3.tar", max compression
```

## Comparing `camply-0.9.2.tar` & `camply-0.9.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1072 2023-01-31 05:46:12.413924 camply-0.9.2/LICENSE
--rw-r--r--   0        0        0     7877 2023-01-31 05:46:12.413924 camply-0.9.2/README.md
--rw-r--r--   0        0        0      575 2023-01-31 05:46:12.413924 camply-0.9.2/camply/__init__.py
--rw-r--r--   0        0        0      105 2023-01-31 05:46:12.413924 camply-0.9.2/camply/__main__.py
--rw-r--r--   0        0        0      141 2023-01-31 05:46:12.413924 camply-0.9.2/camply/_version.py
--rw-r--r--   0        0        0    20360 2023-01-31 05:46:12.413924 camply-0.9.2/camply/cli.py
--rw-r--r--   0        0        0      870 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/__init__.py
--rw-r--r--   0        0        0    18825 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/api_config.py
--rw-r--r--   0        0        0     1189 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/data_columns.py
--rw-r--r--   0        0        0     2610 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/file_config.py
--rw-r--r--   0        0        0     2080 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/logging_config.py
--rw-r--r--   0        0        0     3148 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/notification_config.py
--rw-r--r--   0        0        0     1863 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/search_config.py
--rw-r--r--   0        0        0     3585 2023-01-31 05:46:12.413924 camply-0.9.2/camply/config/yellowstone_config.py
--rw-r--r--   0        0        0      370 2023-01-31 05:46:12.413924 camply-0.9.2/camply/containers/__init__.py
--rw-r--r--   0        0        0    11617 2023-01-31 05:46:12.413924 camply-0.9.2/camply/containers/api_responses.py
--rw-r--r--   0        0        0     1609 2023-01-31 05:46:12.413924 camply-0.9.2/camply/containers/base_container.py
--rw-r--r--   0        0        0     2844 2023-01-31 05:46:12.413924 camply-0.9.2/camply/containers/data_containers.py
--rw-r--r--   0        0        0      414 2023-01-31 05:46:12.413924 camply-0.9.2/camply/containers/gtc_api_responses.py
--rw-r--r--   0        0        0      714 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/__init__.py
--rwxr-xr-x   0        0        0     2703 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/base_notifications.py
--rwxr-xr-x   0        0        0     4465 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/email_notifications.py
--rw-r--r--   0        0        0     3537 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/multi_provider_notifications.py
--rwxr-xr-x   0        0        0     2834 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/pushbullet.py
--rwxr-xr-x   0        0        0     3488 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/pushover.py
--rwxr-xr-x   0        0        0     1655 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/silent_notifications.py
--rwxr-xr-x   0        0        0     3727 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/slack.py
--rwxr-xr-x   0        0        0     3496 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/telegram.py
--rwxr-xr-x   0        0        0     2725 2023-01-31 05:46:12.413924 camply-0.9.2/camply/notifications/twilio.py
--rw-r--r--   0        0        0     1272 2023-01-31 05:46:12.413924 camply-0.9.2/camply/providers/__init__.py
--rw-r--r--   0        0        0     1281 2023-01-31 05:46:12.413924 camply-0.9.2/camply/providers/base_provider.py
--rw-r--r--   0        0        0       37 2023-01-31 05:46:12.413924 camply-0.9.2/camply/providers/going_to_camp/__init__.py
--rw-r--r--   0        0        0    20926 2023-01-31 05:46:12.413924 camply-0.9.2/camply/providers/going_to_camp/going_to_camp_provider.py
--rw-r--r--   0        0        0       34 2023-01-31 05:46:12.413924 camply-0.9.2/camply/providers/recreation_dot_gov/__init__.py
--rw-r--r--   0        0        0     7969 2023-01-31 05:46:12.417924 camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_camps.py
--rw-r--r--   0        0        0    24408 2023-01-31 05:46:12.417924 camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_provider.py
--rw-r--r--   0        0        0    16021 2023-01-31 05:46:12.417924 camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_tours.py
--rw-r--r--   0        0        0       26 2023-01-31 05:46:12.417924 camply-0.9.2/camply/providers/xanterra/__init__.py
--rwxr-xr-x   0        0        0    19635 2023-01-31 05:46:12.417924 camply-0.9.2/camply/providers/xanterra/yellowstone_lodging.py
--rw-r--r--   0        0        0        0 2023-01-31 05:46:12.417924 camply-0.9.2/camply/py.typed
--rw-r--r--   0        0        0     1336 2023-01-31 05:46:12.417924 camply-0.9.2/camply/search/__init__.py
--rw-r--r--   0        0        0    34101 2023-01-31 05:46:12.417924 camply-0.9.2/camply/search/base_search.py
--rw-r--r--   0        0        0     9336 2023-01-31 05:46:12.417924 camply-0.9.2/camply/search/search_going_to_camp.py
--rw-r--r--   0        0        0    15519 2023-01-31 05:46:12.417924 camply-0.9.2/camply/search/search_recreationdotgov.py
--rw-r--r--   0        0        0     6366 2023-01-31 05:46:12.417924 camply-0.9.2/camply/search/search_yellowstone.py
--rw-r--r--   0        0        0      223 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/__init__.py
--rw-r--r--   0        0        0     1815 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/api_utils.py
--rw-r--r--   0        0        0     3978 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/configure_camply.py
--rw-r--r--   0        0        0      804 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/general_utils.py
--rw-r--r--   0        0        0     2714 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/logging_utils.py
--rw-r--r--   0        0        0     4649 2023-01-31 05:46:12.417924 camply-0.9.2/camply/utils/yaml_utils.py
--rw-r--r--   0        0        0     2423 2023-01-31 05:46:12.425924 camply-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     9270 1970-01-01 00:00:00.000000 camply-0.9.2/setup.py
--rw-r--r--   0        0        0     9676 1970-01-01 00:00:00.000000 camply-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-31 05:57:30.001636 camply-0.9.3/LICENSE
+-rw-r--r--   0        0        0     7877 2023-01-31 05:57:30.001636 camply-0.9.3/README.md
+-rw-r--r--   0        0        0      575 2023-01-31 05:57:30.001636 camply-0.9.3/camply/__init__.py
+-rw-r--r--   0        0        0      105 2023-01-31 05:57:30.001636 camply-0.9.3/camply/__main__.py
+-rw-r--r--   0        0        0      141 2023-01-31 05:57:30.001636 camply-0.9.3/camply/_version.py
+-rw-r--r--   0        0        0    20360 2023-01-31 05:57:30.001636 camply-0.9.3/camply/cli.py
+-rw-r--r--   0        0        0      870 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/__init__.py
+-rw-r--r--   0        0        0    18825 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/api_config.py
+-rw-r--r--   0        0        0     1189 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/data_columns.py
+-rw-r--r--   0        0        0     2610 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/file_config.py
+-rw-r--r--   0        0        0     2080 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/logging_config.py
+-rw-r--r--   0        0        0     3148 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/notification_config.py
+-rw-r--r--   0        0        0     1863 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/search_config.py
+-rw-r--r--   0        0        0     3585 2023-01-31 05:57:30.001636 camply-0.9.3/camply/config/yellowstone_config.py
+-rw-r--r--   0        0        0      370 2023-01-31 05:57:30.001636 camply-0.9.3/camply/containers/__init__.py
+-rw-r--r--   0        0        0    11617 2023-01-31 05:57:30.001636 camply-0.9.3/camply/containers/api_responses.py
+-rw-r--r--   0        0        0     1609 2023-01-31 05:57:30.001636 camply-0.9.3/camply/containers/base_container.py
+-rw-r--r--   0        0        0     2844 2023-01-31 05:57:30.001636 camply-0.9.3/camply/containers/data_containers.py
+-rw-r--r--   0        0        0      414 2023-01-31 05:57:30.001636 camply-0.9.3/camply/containers/gtc_api_responses.py
+-rw-r--r--   0        0        0      714 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/__init__.py
+-rwxr-xr-x   0        0        0     2703 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/base_notifications.py
+-rwxr-xr-x   0        0        0     4465 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/email_notifications.py
+-rw-r--r--   0        0        0     3537 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/multi_provider_notifications.py
+-rwxr-xr-x   0        0        0     2834 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/pushbullet.py
+-rwxr-xr-x   0        0        0     3488 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/pushover.py
+-rwxr-xr-x   0        0        0     1643 2023-01-31 05:57:30.001636 camply-0.9.3/camply/notifications/silent_notifications.py
+-rwxr-xr-x   0        0        0     3727 2023-01-31 05:57:30.005636 camply-0.9.3/camply/notifications/slack.py
+-rwxr-xr-x   0        0        0     3496 2023-01-31 05:57:30.005636 camply-0.9.3/camply/notifications/telegram.py
+-rwxr-xr-x   0        0        0     2725 2023-01-31 05:57:30.005636 camply-0.9.3/camply/notifications/twilio.py
+-rw-r--r--   0        0        0     1272 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/__init__.py
+-rw-r--r--   0        0        0     1281 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/base_provider.py
+-rw-r--r--   0        0        0       37 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/going_to_camp/__init__.py
+-rw-r--r--   0        0        0    20926 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/going_to_camp/going_to_camp_provider.py
+-rw-r--r--   0        0        0       34 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/recreation_dot_gov/__init__.py
+-rw-r--r--   0        0        0     7969 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_camps.py
+-rw-r--r--   0        0        0    24408 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_provider.py
+-rw-r--r--   0        0        0    16021 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_tours.py
+-rw-r--r--   0        0        0       26 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/xanterra/__init__.py
+-rwxr-xr-x   0        0        0    19635 2023-01-31 05:57:30.005636 camply-0.9.3/camply/providers/xanterra/yellowstone_lodging.py
+-rw-r--r--   0        0        0        0 2023-01-31 05:57:30.005636 camply-0.9.3/camply/py.typed
+-rw-r--r--   0        0        0     1336 2023-01-31 05:57:30.005636 camply-0.9.3/camply/search/__init__.py
+-rw-r--r--   0        0        0    34101 2023-01-31 05:57:30.005636 camply-0.9.3/camply/search/base_search.py
+-rw-r--r--   0        0        0     9336 2023-01-31 05:57:30.005636 camply-0.9.3/camply/search/search_going_to_camp.py
+-rw-r--r--   0        0        0    15519 2023-01-31 05:57:30.005636 camply-0.9.3/camply/search/search_recreationdotgov.py
+-rw-r--r--   0        0        0     6366 2023-01-31 05:57:30.005636 camply-0.9.3/camply/search/search_yellowstone.py
+-rw-r--r--   0        0        0      223 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/__init__.py
+-rw-r--r--   0        0        0     1815 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/api_utils.py
+-rw-r--r--   0        0        0     3978 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/configure_camply.py
+-rw-r--r--   0        0        0      804 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/general_utils.py
+-rw-r--r--   0        0        0     2714 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/logging_utils.py
+-rw-r--r--   0        0        0     4649 2023-01-31 05:57:30.005636 camply-0.9.3/camply/utils/yaml_utils.py
+-rw-r--r--   0        0        0     2423 2023-01-31 05:57:30.017636 camply-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     9270 1970-01-01 00:00:00.000000 camply-0.9.3/setup.py
+-rw-r--r--   0        0        0     9676 1970-01-01 00:00:00.000000 camply-0.9.3/PKG-INFO
```

### Comparing `camply-0.9.2/LICENSE` & `camply-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/README.md` & `camply-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/__init__.py` & `camply-0.9.3/camply/__init__.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/cli.py` & `camply-0.9.3/camply/cli.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/__init__.py` & `camply-0.9.3/camply/config/__init__.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/api_config.py` & `camply-0.9.3/camply/config/api_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/data_columns.py` & `camply-0.9.3/camply/config/data_columns.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/file_config.py` & `camply-0.9.3/camply/config/file_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/logging_config.py` & `camply-0.9.3/camply/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/notification_config.py` & `camply-0.9.3/camply/config/notification_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/search_config.py` & `camply-0.9.3/camply/config/search_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/config/yellowstone_config.py` & `camply-0.9.3/camply/config/yellowstone_config.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/containers/api_responses.py` & `camply-0.9.3/camply/containers/api_responses.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/containers/base_container.py` & `camply-0.9.3/camply/containers/base_container.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/containers/data_containers.py` & `camply-0.9.3/camply/containers/data_containers.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/__init__.py` & `camply-0.9.3/camply/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/base_notifications.py` & `camply-0.9.3/camply/notifications/base_notifications.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/email_notifications.py` & `camply-0.9.3/camply/notifications/email_notifications.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/multi_provider_notifications.py` & `camply-0.9.3/camply/notifications/multi_provider_notifications.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/pushbullet.py` & `camply-0.9.3/camply/notifications/pushbullet.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/pushover.py` & `camply-0.9.3/camply/notifications/pushover.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/silent_notifications.py` & `camply-0.9.3/camply/notifications/silent_notifications.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 
 
 class SilentNotifications(BaseNotifications):
     """
     Silent Notifications
     """
 
-    def send_message(self, message: Iterable, **kwargs) -> None:
+    def send_message(self, message: str, **kwargs) -> None:
         """
         Send a message via Email
 
         Parameters
         ----------
-        message: Iterable
+        message: str
             Email Body
         **kwargs
             kwargs are disregarded
 
         Returns
         -------
         None
         """
-        message_string = "\n\t• " + "\n\t• ".join(list(message))
-        logger.debug(f"SilentNotification: {message_string}")
+        logger.debug(f"SilentNotification: {message}")
 
     def send_campsites(self, campsites: List[AvailableCampsite], **kwargs):
         """
         Send a message with a campsite object
 
         Parameters
         ----------
@@ -51,10 +50,11 @@
                 ),
                 campsite.campsite_type,
                 campsite.campsite_site_name,
                 campsite.recreation_area,
                 campsite.facility_name,
                 campsite.booking_url,
             )
-            self.send_message(campsite_tuple)
+            message_string = "\n\t• " + "\n\t• ".join(campsite_tuple)
+            self.send_message(message_string)
             campsite_formatted = pformat(campsite.dict())
             logger.debug("Campsite Info: " + campsite_formatted)
```

### Comparing `camply-0.9.2/camply/notifications/slack.py` & `camply-0.9.3/camply/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/telegram.py` & `camply-0.9.3/camply/notifications/telegram.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/notifications/twilio.py` & `camply-0.9.3/camply/notifications/twilio.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/__init__.py` & `camply-0.9.3/camply/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/base_provider.py` & `camply-0.9.3/camply/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/going_to_camp/going_to_camp_provider.py` & `camply-0.9.3/camply/providers/going_to_camp/going_to_camp_provider.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_camps.py` & `camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_camps.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_provider.py` & `camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_provider.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/recreation_dot_gov/recdotgov_tours.py` & `camply-0.9.3/camply/providers/recreation_dot_gov/recdotgov_tours.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/providers/xanterra/yellowstone_lodging.py` & `camply-0.9.3/camply/providers/xanterra/yellowstone_lodging.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/search/__init__.py` & `camply-0.9.3/camply/search/__init__.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/search/base_search.py` & `camply-0.9.3/camply/search/base_search.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/search/search_going_to_camp.py` & `camply-0.9.3/camply/search/search_going_to_camp.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/search/search_recreationdotgov.py` & `camply-0.9.3/camply/search/search_recreationdotgov.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/search/search_yellowstone.py` & `camply-0.9.3/camply/search/search_yellowstone.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/utils/api_utils.py` & `camply-0.9.3/camply/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/utils/configure_camply.py` & `camply-0.9.3/camply/utils/configure_camply.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/utils/general_utils.py` & `camply-0.9.3/camply/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/utils/logging_utils.py` & `camply-0.9.3/camply/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/camply/utils/yaml_utils.py` & `camply-0.9.3/camply/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `camply-0.9.2/pyproject.toml` & `camply-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "camply"
 description = "camply, the campsite finder 🏕"
-version = "0.9.2"
+version = "0.9.3"
 authors = ["Justin Flannery <juftin@juftin.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/juftin/camply"
 repository = "https://github.com/juftin/camply"
 documentation = "https://juftin.github.io/camply"
 classifiers = [
```

### Comparing `camply-0.9.2/setup.py` & `camply-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 {'all': ['twilio>=7.14.0'], 'twilio': ['twilio>=7.14.0']}
 
 entry_points = \
 {'console_scripts': ['camply = camply.cli:cli']}
 
 setup_kwargs = {
     'name': 'camply',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'camply, the campsite finder 🏕',
     'long_description': '<div align="center">\n<a href="https://github.com/juftin/camply">\n  <img src="https://raw.githubusercontent.com/juftin/camply/main/docs/_static/camply.svg"\n    width="400" height="400" alt="camply">\n</a>\n</div>\n\n`camply`, the campsite finder ⛺️, is a tool to help you book a campground online. Finding\nreservations at sold out campgrounds can be tough. That\'s where camply comes in. It searches the\nAPIs of booking services like https://recreation.gov (which indexes thousands of campgrounds across\nthe USA) to continuously check for cancellations and availabilities to pop up. Once a campsite\nbecomes available, camply sends you a notification to book your spot!\n\n---\n\n---\n\n[![PyPI](https://img.shields.io/pypi/v/camply?color=blue&label=⛺️camply)](https://github.com/juftin/camply)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/camply)](https://pypi.python.org/pypi/camply/)\n[![Docker Image Version](https://img.shields.io/docker/v/juftin/camply?color=blue&label=docker&logo=docker)](https://hub.docker.com/r/juftin/camply)\n[![Testing Status](https://github.com/juftin/camply/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/camply/actions/workflows/tests.yaml)\n[![GitHub License](https://img.shields.io/github/license/juftin/camply?color=blue&label=License)](https://github.com/juftin/camply/blob/main/LICENSE)\n[![Black Codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)]()\n[![Discord Chat](https://img.shields.io/static/v1?label=chat&message=discord&color=blue&logo=discord)](https://discord.gg/qZDr78kKvB)\n[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)\n\n## [Check Out The Docs](https://juftin.com/camply/)\n\n## Installing\n\nInstall camply via pip:\n\n```\npip install camply\n```\n\n## Documentation\n\nHead over to the [camply documentation](https://juftin.com/camply/) to see what you can do!\n\n```commandline\ncamply --help\n\nUsage: camply [OPTIONS] COMMAND [ARGS]...\n\n  Welcome to camply, the campsite finder.\n\n  Finding reservations at sold out campgrounds can be tough. That\'s where\n  camply comes in. It searches the APIs of booking services like\n  https://recreation.gov (which indexes thousands of campgrounds across the\n  USA) to continuously check for cancellations and availabilities to pop up.\n  Once a campsite becomes available, camply sends you a notification to book\n  your spot!\n\n  visit the camply documentation at https://github.com/juftin/camply\n\nOptions:\n  --version             Show the version and exit.\n  --provider TEXT       Camping Search Provider. Options available are\n                        \'Yellowstone\' and \'RecreationDotGov\'. Defaults to\n                        \'RecreationDotGov\', not case-sensitive.\n  --debug / --no-debug  Enable extra debugging output\n  --help                Show this message and exit.\n\nCommands:\n  campgrounds       Search for Campgrounds (inside of Recreation Areas)...\n  campsites         Find available Campsites using search criteria\n  configure         Set up camply configuration file with an interactive...\n  recreation-areas  Search for Recreation Areas and list them\n```\n\n## Contributing\n\nCamply doesn\'t support your favorite campsite booking provider yet? Consider\n[contributing](https://juftin.com/camply/contributing/) 😉.\n\n## Table of Contents\n\n-   [Installation](docs/installation.md)\n    -   [PyPI](docs/installation.md#pypi)\n    -   [Docker](docs/installation.md#docker)\n-   [Providers](docs/providers.md)\n    -   [RecreationDotGov](docs/providers.md#recreationgov)\n    -   [Yellowstone](docs/providers.md#yellowstone)\n    -   [GoingToCamp](docs/providers.md#goingtocamp)\n    -   [RecDotGov Tours + Tickets + Timed Entry](docs/providers.md#recreationgov-tickets-tours--timed-entry)\n-   [Command Line Usage](docs/command_line_usage.md)\n    -   [campsites](docs/command_line_usage.md#campsites)\n    -   [recreation-areas](docs/command_line_usage.md#recreation-areas)\n    -   [campgrounds](docs/command_line_usage.md#campgrounds)\n    -   [configure](docs/command_line_usage.md#configure)\n    -   [Examples](docs/command_line_usage.md#examples)\n        -   [Searching for a Campsite](docs/command_line_usage.md#searching-for-a-campsite)\n        -   [Searching for a Campsite by Campground ID](docs/command_line_usage.md#searching-for-a-campsite-by-campground-id)\n        -   [Searching for a Specific Campsite by ID](docs/command_line_usage.md#searching-for-a-specific-campsite-by-id)\n        -   [Continuously Searching for A Campsite](docs/command_line_usage.md#continuously-searching-for-a-campsite)\n        -   [Continue Looking After The First Match Is Found](docs/command_line_usage.md#continue-looking-after-the-first-match-is-found)\n        -   [Send a Push Notification](docs/command_line_usage.md#send-a-push-notification)\n        -   [Send a Text Message](docs/command_line_usage.md#send-a-text-message)\n        -   [Send a Notification to Different Services](docs/command_line_usage.md#send-a-notification-to-different-services)\n        -   [Look for Weekend Campsite Availabilities](docs/command_line_usage.md#look-for-weekend-campsite-availabilities)\n        -   [Look for Consecutive Nights at the Same Campsite](docs/command_line_usage.md#look-for-consecutive-nights-at-the-same-campsite)\n        -   [Look for a Campsite Inside of Yellowstone](docs/command_line_usage.md#look-for-a-campsite-inside-of-yellowstone)\n        -   [Look for a Campsite from GoingToCamp](docs/command_line_usage.md#look-for-a-campsite-from-goingtocamp)\n        -   [Searching GoingToCamp Using Equipment](docs/command_line_usage.md#searching-goingtocamp-using-equipment)\n        -   [Look for a Campsite Across Multiple Recreation areas](docs/command_line_usage.md#look-for-a-campsite-across-multiple-recreation-areas)\n        -   [Using a YAML Configuration file to search for campsites](docs/command_line_usage.md#using-a-yaml-configuration-file-to-search-for-campsites)\n        -   [Searching for a Campsite That Fits Your Equipment](docs/command_line_usage.md#searching-for-a-campsite-that-fits-your-equipment)\n        -   [Saving the Results of a Search](docs/command_line_usage.md#saving-the-results-of-a-search)\n        -   [Search for Recreation Areas by Query String](docs/command_line_usage.md#search-for-recreation-areas-by-query-string)\n        -   [Look for Specific Campgrounds Within a Recreation Area](docs/command_line_usage.md#look-for-specific-campgrounds-within-a-recreation-area)\n        -   [Look for Specific Campgrounds by Query String](docs/command_line_usage.md#look-for-specific-campgrounds-by-query-string)\n        -   [Searching for Tickets and Timed Entries](docs/ccommand_line_usage.md#searching-for-tickets-and-timed-entries)\n            -   [Tickets + Tours](docs/ccommand_line_usage.md#tickets-tours)\n            -   [Timed Entry](docs/ccommand_line_usage.md#timed-entry)\n            -   [Using the Daily Providers](command_line_usage.md#using-the-daily-providers)\n-   [Finding Recreation Areas IDs and Campground IDs To Search Without Using the Command Line](docs/command_line_usage.md#finding-recreation-areas-ids-and-campground-ids-to-search-without-using-the-command-line)\n-   [Object-Oriented Usage (Python)](docs/python.md)\n    -   [Search for a Recreation.gov Campsite](docs/python.md#search-for-a-recreationgov-campsite)\n    -   [Continuously Search for Recreation.gov Campsites](docs/python.md#continuously-search-for-recreationgov-campsites)\n-   [Running in Docker](docs/docker.md)\n-   [Dependencies](docs/dependencies.md)\n-   [Contributing](docs/contributing.md)\n\n<br/>\n\nRecreation data provided by [**Recreation.gov**](https://ridb.recreation.gov/)\n\n---\n\n---\n\n<br/>\n\n[<p align="center" ><img src="https://raw.githubusercontent.com/juftin/juftin/main/static/juftin.png" width="120" height="120"  alt="juftin logo"> </p>](https://github.com/juftin)\n',
     'author': 'Justin Flannery',
     'author_email': 'juftin@juftin.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/juftin/camply',
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 'camply.providers.recreation_dot_gov', 'camply.providers.xanterra',
 'camply.search', 'camply.utils'] package_data = \ {'': ['*']} install_requires
 = \ ['PyYAML>=5.1,<7.0', 'click>=8.0.1', 'pandas>=1.3,<1.4',
 'pydantic>=1.2,<2.0', 'python-dotenv>=0.10.4', 'pytz>=2019.1',
 'requests>=2.26.0', 'rich>=10.0.0', 'tenacity>=5.1.0'] extras_require = \
 {'all': ['twilio>=7.14.0'], 'twilio': ['twilio>=7.14.0']} entry_points = \
 {'console_scripts': ['camply = camply.cli:cli']} setup_kwargs = { 'name':
-'camply', 'version': '0.9.2', 'description': 'camply, the campsite finder
+'camply', 'version': '0.9.3', 'description': 'camply, the campsite finder
 ð', 'long_description': '
                \n\n_n_width="400"_height="400"_alt="camply">\n\n
 \n\n`camply`, the campsite finder âºï¸, is a tool to help you book a
 campground online. Finding\nreservations at sold out campgrounds can be tough.
 That\'s where camply comes in. It searches the\nAPIs of booking services like
 https://recreation.gov (which indexes thousands of campgrounds across\nthe USA)
 to continuously check for cancellations and availabilities to pop up. Once a
```

### Comparing `camply-0.9.2/PKG-INFO` & `camply-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camply
-Version: 0.9.2
+Version: 0.9.3
 Summary: camply, the campsite finder 🏕
 Home-page: https://github.com/juftin/camply
 License: MIT
 Keywords: recdotgov,outdoors,camping,reservations,national-parks
 Author: Justin Flannery
 Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: camply Version: 0.9.2 Summary: camply, the campsite
+Metadata-Version: 2.1 Name: camply Version: 0.9.3 Summary: camply, the campsite
 finder ð Home-page: https://github.com/juftin/camply License: MIT Keywords:
 recdotgov,outdoors,camping,reservations,national-parks Author: Justin Flannery
 Author-email: juftin@juftin.com Requires-Python: >=3.7.1,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

