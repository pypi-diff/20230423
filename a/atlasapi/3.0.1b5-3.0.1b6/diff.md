# Comparing `tmp/atlasapi-3.0.1b5.tar.gz` & `tmp/atlasapi-3.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasapi-3.0.1b5.tar", last modified: Sun Jan 29 21:27:44 2023, max compression
+gzip compressed data, was "atlasapi-3.0.1b6.tar", last modified: Mon Mar 27 11:07:43 2023, max compression
```

## Comparing `atlasapi-3.0.1b5.tar` & `atlasapi-3.0.1b6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-01-29 21:27:44.752545 atlasapi-3.0.1b5/
--rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/LICENSE
--rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-01-29 21:27:44.752186 atlasapi-3.0.1b5/PKG-INFO
--rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/README.rst
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-01-29 21:27:44.744919 atlasapi-3.0.1b5/atlasapi/
--rw-r--r--   0 mgm        (502) staff       (20)      672 2023-01-29 21:24:34.000000 atlasapi-3.0.1b5/atlasapi/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/alerts.py
--rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/api_keys.py
--rw-r--r--   0 mgm        (502) staff       (20)   109176 2023-01-29 21:10:56.000000 atlasapi-3.0.1b5/atlasapi/atlas.py
--rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/atlas_types.py
--rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b5/atlasapi/atlas_users.py
--rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b5/atlasapi/cloud_backup.py
--rw-r--r--   0 mgm        (502) staff       (20)    36396 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/clusters.py
--rw-r--r--   0 mgm        (502) staff       (20)     8544 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/errors.py
--rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/events.py
--rw-r--r--   0 mgm        (502) staff       (20)    54299 2023-01-07 00:49:32.000000 atlasapi-3.0.1b5/atlasapi/events_event_types.py
--rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/invoices_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/lib.py
--rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/logs.py
--rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/maintenance_window.py
--rw-r--r--   0 mgm        (502) staff       (20)    15755 2022-06-22 22:40:25.000000 atlasapi-3.0.1b5/atlasapi/measurements.py
--rw-r--r--   0 mgm        (502) staff       (20)     9607 2023-01-29 19:20:13.000000 atlasapi-3.0.1b5/atlasapi/network.py
--rw-r--r--   0 mgm        (502) staff       (20)      863 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/organizations.py
--rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b5/atlasapi/projects.py
--rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/serverless_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)    11319 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/settings.py
--rw-r--r--   0 mgm        (502) staff       (20)    23639 2023-01-28 19:57:14.000000 atlasapi-3.0.1b5/atlasapi/specs.py
--rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b5/atlasapi/teams.py
--rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlasapi/whitelist.py
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-01-29 21:27:44.748656 atlasapi-3.0.1b5/atlasapi.egg-info/
--rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/PKG-INFO
--rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/entry_points.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/requires.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-01-29 21:27:44.000000 atlasapi-3.0.1b5/atlasapi.egg-info/top_level.txt
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-01-29 21:27:44.751636 atlasapi-3.0.1b5/atlascli/
--rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlascli/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlascli/atlaserrors.py
--rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlascli/atlaskey.py
--rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlascli/cli.py
--rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b5/atlascli/listcommand.py
--rw-r--r--   0 mgm        (502) staff       (20)       38 2023-01-29 21:27:44.752639 atlasapi-3.0.1b5/setup.cfg
--rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-01-29 21:24:34.000000 atlasapi-3.0.1b5/setup.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.544278 atlasapi-3.0.1b6/
+-rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/LICENSE
+-rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-03-27 11:07:43.543700 atlasapi-3.0.1b6/PKG-INFO
+-rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/README.rst
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.536459 atlasapi-3.0.1b6/atlasapi/
+-rw-r--r--   0 mgm        (502) staff       (20)      672 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/atlasapi/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/alerts.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/api_keys.py
+-rw-r--r--   0 mgm        (502) staff       (20)   110669 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/atlas.py
+-rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/atlas_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b6/atlasapi/atlas_users.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b6/atlasapi/cloud_backup.py
+-rw-r--r--   0 mgm        (502) staff       (20)    36466 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/clusters.py
+-rw-r--r--   0 mgm        (502) staff       (20)     8544 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/errors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/events.py
+-rw-r--r--   0 mgm        (502) staff       (20)    60586 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/events_event_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/invoices_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/lib.py
+-rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/logs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/maintenance_window.py
+-rw-r--r--   0 mgm        (502) staff       (20)    15755 2022-06-22 22:40:25.000000 atlasapi-3.0.1b6/atlasapi/measurements.py
+-rw-r--r--   0 mgm        (502) staff       (20)    10967 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/atlasapi/network.py
+-rw-r--r--   0 mgm        (502) staff       (20)      863 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/organizations.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b6/atlasapi/projects.py
+-rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/serverless_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11207 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/settings.py
+-rw-r--r--   0 mgm        (502) staff       (20)    23713 2023-03-26 17:22:20.000000 atlasapi-3.0.1b6/atlasapi/specs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b6/atlasapi/teams.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlasapi/whitelist.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.539936 atlasapi-3.0.1b6/atlasapi.egg-info/
+-rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/PKG-INFO
+-rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/entry_points.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/requires.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-03-27 11:07:43.000000 atlasapi-3.0.1b6/atlasapi.egg-info/top_level.txt
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-03-27 11:07:43.542785 atlasapi-3.0.1b6/atlascli/
+-rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/atlaserrors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/atlaskey.py
+-rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/cli.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b6/atlascli/listcommand.py
+-rw-r--r--   0 mgm        (502) staff       (20)       38 2023-03-27 11:07:43.544443 atlasapi-3.0.1b6/setup.cfg
+-rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-03-26 19:19:33.000000 atlasapi-3.0.1b6/setup.py
```

### Comparing `atlasapi-3.0.1b5/LICENSE` & `atlasapi-3.0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/PKG-INFO` & `atlasapi-3.0.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b5
+Version: 3.0.1b6
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b5/README.rst` & `atlasapi-3.0.1b6/README.rst`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/__init__.py` & `atlasapi-3.0.1b6/atlasapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "3.0.1b5"
+__version__ = "3.0.1b6"
```

### Comparing `atlasapi-3.0.1b5/atlasapi/alerts.py` & `atlasapi-3.0.1b6/atlasapi/alerts.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/api_keys.py` & `atlasapi-3.0.1b6/atlasapi/api_keys.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/atlas.py` & `atlasapi-3.0.1b6/atlasapi/atlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Atlas module
 
 Core module which provides access to MongoDB Atlas Cloud Provider APIs
 """
-from atlasapi.network import Network
+from atlasapi.network import Network, atlas_encode_params
 from atlasapi.errors import *
 from pprint import pprint
 from json import loads
 from datetime import datetime, timezone
 from dateutil.relativedelta import relativedelta
 from atlasapi.specs import Host, ListOfHosts, DatabaseUsersUpdatePermissionsSpecs, ReplicaSetTypes
 from atlasapi.measurements import AtlasMeasurementTypes, AtlasMeasurementValue, AtlasMeasurement
@@ -45,15 +45,14 @@
 from requests.auth import HTTPBasicAuth, HTTPDigestAuth
 from atlasapi.events_event_types import AtlasEventTypes
 from atlasapi.events import AtlasEvent
 from atlasapi.invoices_pydantic import ApiInvoiceView
 from atlasapi.serverless_pydantic import ServerlessInstance, ServerlessInstanceProviderSettings, BackingProviderName, \
     ServerlessProviderName, ServerlessRegionName, DeletedReturn
 import gzip
-import pytz
 
 logger = logging.getLogger('Atlas')
 
 
 # noinspection PyProtectedMember
 
 
@@ -482,24 +481,32 @@
             Keyword Args:
 
 
             Returns:
                 ListOfHosts: Iterable object representing this function
 
             """
-            uri = Settings.api_resources["Monitoring and Logs"]["Get all processes for group"].format(
-                group_id=self.atlas.group)
+            # Handling for Atlas Object which have been intantiated without a Group/Project (a Group Key)
+            # We need to handle the fact that for these atlas objects, we can not grab all hosts.
+            if not self.atlas.group:
+                logger.error("we do not have a group, the Atlas object does not have a group!")
+                print("we do not have a group, the Atlas object does not have a group!")
+                yield None
+            else:
 
-            try:
-                response = self.atlas.network.get(Settings.BASE_URL + uri)
-                for page in response:
-                    for each_process in page.get("results"):
-                        yield Host(each_process)
-            except Exception as e:
-                raise e
+                uri = Settings.api_resources["Monitoring and Logs"]["Get all processes for group"].format(
+                    GROUP_ID=self.atlas.group)
+
+                try:
+                    response = self.atlas.network.get(Settings.BASE_URL + uri)
+                    for page in response:
+                        for each_process in page.get("results"):
+                            yield Host(each_process)
+                except Exception as e:
+                    raise e
 
         def fill_host_list(self, for_cluster: Optional[str] = None) -> Iterable[Host]:
             """
             Fills the `self.hostname` property with the current hosts for the project/group.
 
             Optionally, one can specify the `for_cluster` parameter to fill the host list with
             hosts only from the specified cluster.
@@ -602,30 +609,35 @@
             """
             for each_host in self.host_list:
                 if each_host.type == ReplicaSetTypes.REPLICA_SECONDARY:
                     yield each_host
 
         def get_measurement_for_hosts(self, granularity: Optional[AtlasGranularities] = None,
                                       period: Optional[AtlasPeriods] = None,
-                                      measurement: Optional[AtlasMeasurementTypes] = None, return_data: bool = False):
+                                      measurement: Optional[AtlasMeasurementTypes] = None, return_data: bool = False,
+                                      start: Optional[datetime] = None, end: Optional[datetime] = None):
             """Get measurement(s) for all hosts in the host_list
 
 
                         Populates all hosts in the host_list with the requested metric.
 
                         Multiple calls will append additional metrics to the same host object.
 
+                        You must provide both `start` and `end` or neither. You cannot provide `period`
+                        with `start` and `end`.
+
                         Please note that using the `return_data`  param will also return the updated
                         host objects, which may unnecessarily consume memory.
 
                         Keyword Args:
                             granularity (AtlasGranularities): the desired granularity
                             period (AtlasPeriods): The desired period
                             measurement (AtlasMeasurementTypes) : The desired measurement or Measurement class
-
+                            start (datetime): The start of the desired period
+                            end (datetime): The end of the desired period
 
 
                             :param return_data:
                             :rtype: List[measurements.AtlasMeasurement]
                             :type period: AtlasPeriods
                             :type granularity: AtlasGranularities
                             :type measurement: measurements.AtlasMeasurementTypes
@@ -640,14 +652,15 @@
                 logger.info(f'Measurement: {measurement}')
                 logger.info('Metric: {}'.format(granularity.__str__()))
                 logger.info('For Period: {}'.format(period.__str__()))
                 try:
                     logger.debug(f'The data type of measurement is is {type(measurement)}')
                     returned_data = self._get_measurement_for_host(each_host, granularity=granularity,
                                                                    period=period,
+                                                                   start=start, end=end,
                                                                    measurement=measurement)
                     each_host.measurements = list(returned_data)
                 except Exception as e:
                     logger.error('An error occurred while retrieving metrics for host: {}.'
                                  'The error was {}'.format(each_host.hostname, e))
                     logger.warning('Will continue with next host. . . ')
                 return_list.append(each_host)
@@ -677,34 +690,29 @@
             uri = Settings.api_resources["Monitoring and Logs"]["Get the log file for a host in the cluster"].format(
                 group_id=self.atlas.group,
                 host=host_obj.hostname,
                 logname=log_name.value,
                 date_from=date_from,
                 date_to=date_to
             )
-            params = dict()
-            if date_from:
-                try:
-                    date_from = pytz.utc.localize(date_from)
-                except ValueError:
-                    logger.info(f'The date_from value {date_from} is already localized. Will not re-localize.')
-                    pass
-
-                params.update({'startDate': int(round(date_from.timestamp()))})
-            if date_to:
-                try:
-                    date_to = pytz.utc.localize(date_to)
-                except ValueError:
-                    logger.info(f'The date_to value {date_to} is already localized. Will not re-localize.')
-                    pass
-                params.update({'endDate': int(round(date_to.timestamp()))})
-
             # Build the request
+            if date_to is None and date_from is None:
+                logger.info('No dates passed so we are not going to send date params, API default will be used.')
+                uri = Settings.BASE_URL + uri
+            # TODO: refator to use params instead of hand crafting the uri for the dates
+            elif date_to is None and date_from is not None:
+                logger.info('Received only a date_from, so sending only startDate')
+                uri = Settings.BASE_URL + uri + f'?startDate={int(round(date_from.timestamp()))}'
+            elif date_to is not None and date_from is None:
+                uri = Settings.BASE_URL + uri + f'?endDate={int(round(date_to.timestamp()))}'
+            else:
+                uri = Settings.BASE_URL + uri + f'?endDate={int(round(date_to.timestamp()))}' \
+                                                f'&startDate={int(round(date_from.timestamp()))}'
             logger.info(f'The URI used will be {uri}')
-            return_val = self.atlas.network.get_file(Settings.BASE_URL + uri, params=params)
+            return_val = self.atlas.network.get_file(uri)
             return return_val
 
         def get_loglines_for_host(self, host_obj: Host,
                                   log_name: AtlasLogNames = AtlasLogNames.MONGODB,
                                   date_from: datetime = None,
                                   date_to: datetime = None,
                                   ) -> Iterable[LogLine]:
@@ -792,15 +800,17 @@
                     raise e
                 each_host.add_log_file(name=log_name, file=log_file)
                 yield each_host
 
         def _get_measurement_for_host(self, host_obj: Host,
                                       granularity: Optional[AtlasGranularities] = None,
                                       period: Optional[AtlasPeriods] = None,
-                                      measurement: Optional[AtlasMeasurementTypes] = None
+                                      measurement: Optional[AtlasMeasurementTypes] = None,
+                                      start: Optional[datetime] = None,
+                                      end: Optional[datetime] = None
                                       ) -> Iterable[AtlasMeasurement]:
             """Get  measurement(s) for a host
 
             Internal use only, should come from the host obj itself.
 
             Returns measurements for the passed Host object.
 
@@ -816,14 +826,16 @@
                 host_obj (Host): the host
                 granularity (AtlasGranuarities): the desired granularity
                 period (AtlasPeriods): The desired period
                 measurement (AtlasMeasurementTypes) : The desired measurement or Measurement class
                 pageNum (int): Page number
                 itemsPerPage (int): Number of Users per Page
                 iterable (bool): To return an iterable high level object instead of a low level API response
+                start (datetime): Start of the desired period
+                end (datetime): End of the desired period
 
             Returns:
                  Iterable[AtlasMeasurement] or dict: Iterable object representing this function OR Response payload
 
             Raises:
                 ErrPaginationLimits: Out of limits
 
@@ -834,15 +846,15 @@
                 :type measurement: measurements.AtlasMeasurementTypes
 
             """
 
             #  Set default measurement, period and granularity if none are sent
             if measurement is None:
                 measurement = AtlasMeasurementTypes.Cache.dirty
-            if period is None:
+            if period is None and start is None and end is None:
                 period = AtlasPeriods.WEEKS_1
             if granularity is None:
                 granularity = AtlasGranularities.HOUR
 
             # Check to see if we received a leaf or branch of the measurements
             logger.debug(f'Measurement is: {measurement}')
             logger.debug(f'Measurement object type is {type(measurement)}')
@@ -866,19 +878,19 @@
             if isinstance(period, tuple):
                 logger.debug(f'Somehow got a tuple for period {period}. Need to get the str')
                 period: tuple = period[0]
 
             uri = Settings.api_resources["Monitoring and Logs"]["Get measurement for host"].format(
                 group_id=self.atlas.group,
                 host=host_obj.hostname,
-                port=host_obj.port,
-                granularity=granularity,
-                period=period,
-                measurement=measurement
-            )
+                port=host_obj.port
+            ) + "?" + atlas_encode_params({
+                "granularity": granularity, "m": measurement,
+                "period": period, "start": start, "end": end})
+
             logger.debug(f'The URI used will be {uri}')
             # Build the request
             return_val = self.atlas.network.get(Settings.BASE_URL + uri)
             for each_host in return_val:
                 try:
                     measurements = each_host.get('measurements')
                 except Exception as e:
```

### Comparing `atlasapi-3.0.1b5/atlasapi/atlas_users.py` & `atlasapi-3.0.1b6/atlasapi/atlas_users.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/cloud_backup.py` & `atlasapi-3.0.1b6/atlasapi/cloud_backup.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/clusters.py` & `atlasapi-3.0.1b6/atlasapi/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,19 +521,20 @@
                  replication_factor: Optional[int] = None,
                  state_name: Optional[ClusterStates] = None,
                  autoscaling: dict = {},
                  replication_specs: list = [],
                  srv_address: Optional[str] = None,
                  providerSettings: Optional[ProviderSettings] = None,
                  links: list = None,
-                 id: Optional[str] = None):
+                 id: Optional[str] = None,
+                 create_date: Optional[datetime] = None):
         super().__init__(backup_enabled, cluster_type, disk_size_gb, name, mongodb_major_version, mongodb_version,
                          num_shards, mongo_uri, mongo_uri_updated, mongo_uri_with_options, paused, pit_enabled,
                          replication_factor, state_name, autoscaling, [replication_specs], srv_address,
-                         providerSettings, links, id)
+                         providerSettings, links, id, create_date)
 
     def as_dict(self) -> dict:
         return_dict = self.__dict__
         return_dict['clusterType'] = self.cluster_type.name
         return_dict.__delitem__('cluster_type')
         return_dict['mongoDBMajorVersion'] = self.mongodb_major_version.value
         return_dict.__delitem__('mongodb_major_version')
```

### Comparing `atlasapi-3.0.1b5/atlasapi/errors.py` & `atlasapi-3.0.1b6/atlasapi/errors.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/events.py` & `atlasapi-3.0.1b6/atlasapi/events.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/events_event_types.py` & `atlasapi-3.0.1b6/atlasapi/events_event_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from enum import Enum
-
-
 class AtlasEventTypes(Enum):
     APP_SETTINGS_CHANGE = 'App Settings Change'
     PEER_CREATED = 'Peer Created'
     PEER_DELETED = 'Peer Deleted'
     PEER_UPDATED = 'Peer Updated'
     GCP_PEER_CREATED = 'GCP Peer Created'
     GCP_PEER_DELETED = 'GCP Peer Deleted'
@@ -48,14 +46,16 @@
     BACKUP_TOO_MANY_HEAD_START_ATTEMPTS = 'Backup Too Many Head Start Attempts'
     BLOCKSTORE_JOB_RECOVERED = 'Blockstore Job Recovered'
     BLOCKSTORE_JOB_TOO_MANY_RETRIES = 'Blockstore Job Too Many Retries'
     NO_RS_BIND_ERROR = 'No Rs Bind Error'
     RS_BIND_ERROR = 'Rs Bind Error'
     TIMELY_SNAPSHOT = 'Timely Snapshot'
     LATE_SNAPSHOT = 'Late Snapshot'
+    TIMELY_WTC_SNAPSHOT = 'Timely Wtc Snapshot'
+    LATE_WTC_SNAPSHOT = 'Late Wtc Snapshot'
     GOOD_CLUSTERSHOT = 'Good Clustershot'
     BAD_CLUSTERSHOTS = 'Bad Clustershots'
     SYNC_SLICE_PROGRESSED = 'Sync Slice Progressed'
     SYNC_SLICE_HAS_NOT_PROGRESSED = 'Sync Slice Has Not Progressed'
     BACKUP_JOB_NOT_BUSY = 'Backup Job Not Busy'
     BACKUP_JOB_TOO_BUSY = 'Backup Job Too Busy'
     CONSISTENT_BACKUP_CONFIGURATION = 'Consistent Backup Configuration'
@@ -87,14 +87,20 @@
     CPS_RESTORE_REQUESTED_AUDIT = 'Cps Restore Requested Audit'
     CPS_SNAPSHOT_SCHEDULE_UPDATED_AUDIT = 'Cps Snapshot Schedule Updated Audit'
     CPS_SNAPSHOT_DELETED_AUDIT = 'Cps Snapshot Deleted Audit'
     CPS_SNAPSHOT_RETENTION_MODIFIED_AUDIT = 'Cps Snapshot Retention Modified Audit'
     CPS_SNAPSHOT_IN_PROGRESS_AUDIT = 'Cps Snapshot In Progress Audit'
     CPS_SNAPSHOT_COMPLETED_AUDIT = 'Cps Snapshot Completed Audit'
     CPS_ON_DEMAND_SNAPSHOT_REQUESTED = 'Cps On Demand Snapshot Requested'
+    CPS_DATA_PROTECTION_ENABLE_REQUESTED = 'Cps Data Protection Enable Requested'
+    CPS_DATA_PROTECTION_ENABLED = 'Cps Data Protection Enabled'
+    CPS_DATA_PROTECTION_UPDATE_REQUESTED = 'Cps Data Protection Update Requested'
+    CPS_DATA_PROTECTION_UPDATED = 'Cps Data Protection Updated'
+    CPS_DATA_PROTECTION_DISABLE_REQUESTED = 'Cps Data Protection Disable Requested'
+    CPS_DATA_PROTECTION_DISABLED = 'Cps Data Protection Disabled'
     BUCKET_CREATED_AUDIT = 'Bucket Created Audit'
     BUCKET_DELETED_AUDIT = 'Bucket Deleted Audit'
     TENANT_SNAPSHOT_STARTED_AUDIT = 'Tenant Snapshot Started Audit'
     TENANT_SNAPSHOT_COMPLETED_AUDIT = 'Tenant Snapshot Completed Audit'
     TENANT_SNAPSHOT_DELETED_AUDIT = 'Tenant Snapshot Deleted Audit'
     TENANT_RESTORE_REQUESTED_AUDIT = 'Tenant Restore Requested Audit'
     TENANT_RESTORE_COMPLETED_AUDIT = 'Tenant Restore Completed Audit'
@@ -135,17 +141,27 @@
     ONE_INVOICE_FOR_MONTH = 'One Invoice For Month'
     MULTIPLE_INVOICES_FOR_MONTH = 'Multiple Invoices For Month'
     PAYMENT_METHODS_REMOVED = 'Payment Methods Removed'
     DISCOUNT_APPLIED = 'Discount Applied'
     CREDIT_ISSUED = 'Credit Issued'
     GCP_BILLING_ACCOUNT_CREDIT_ISSUED = 'GCP Billing Account Credit Issued'
     CREDIT_PULLED_FWD = 'Credit Pulled Fwd'
+    CREDIT_START_DATE_MODIFIED = 'Credit Start Date Modified'
     CREDIT_END_DATE_MODIFIED = 'Credit End Date Modified'
-    CREDIT_SFOLID_MODIFIED = 'Credit Sfolid Modified'
+    CREDIT_ELASTIC_INVOICING_MODIFIED = 'Credit Elastic Invoicing Modified'
+    CREDIT_TYPE_MODIFIED = 'Credit Type Modified'
+    CREDIT_AMOUNT_CENTS_MODIFIED = 'Credit Amount Cents Modified'
+    CREDIT_AMOUNT_REMAINING_CENTS_MODIFIED = 'Credit Amount Remaining Cents Modified'
+    CREDIT_TOTAL_BILLED_CENTS_MODIFIED = 'Credit Total Billed Cents Modified'
+    CREDIT_AWS_CUSTOMER_ID_MODIFIED = 'Credit AWS Customer Id Modified'
+    CREDIT_AWS_PRODUCT_CODE_MODIFIED = 'Credit AWS Product Code Modified'
+    CREDIT_GCP_MARKETPLACE_ENTITLEMENT_ID_MODIFIED = 'Credit GCP Marketplace Entitlement Id Modified'
+    CREDIT_AZURE_SUBSCRIPTION_ID_MODIFIED = 'Credit Azure Subscription Id Modified'
     CREDIT_AMOUNT_MODIFIED = 'Credit Amount Modified'
+    CREDIT_SFOLID_MODIFIED = 'Credit Sfolid Modified'
     PROMO_CODE_APPLIED = 'Promo Code Applied'
     REFUND_ISSUED = 'Refund Issued'
     PAYMENT_FORGIVEN = 'Payment Forgiven'
     ACCOUNT_UPGRADED = 'Account Upgraded'
     ACCOUNT_DOWNGRADED = 'Account Downgraded'
     SUPPORT_PLAN_ACTIVATED = 'Support Plan Activated'
     SUPPORT_PLAN_CANCELLED = 'Support Plan Cancelled'
@@ -164,14 +180,16 @@
     CLUSTER_MONGOS_IS_MISSING = 'Cluster Mongos Is Missing'
     SHARD_ADDED = 'Shard Added'
     SHARD_REMOVED = 'Shard Removed'
     DATA_EXPLORER = 'Data Explorer'
     DATA_EXPLORER_CRUD = 'Data Explorer Crud'
     DATA_EXPLORER_CRUD_ERROR = 'Data Explorer Crud Error'
     DATA_EXPLORER_CRUD_ATTEMPT = 'Data Explorer Crud Attempt'
+    DATA_EXPLORER_ENABLED = 'Data Explorer Enabled'
+    DATA_EXPLORER_DISABLED = 'Data Explorer Disabled'
     AWS_ENCRYPTION_KEY_ROTATED = 'AWS Encryption Key Rotated'
     AWS_ENCRYPTION_KEY_NEEDS_ROTATION = 'AWS Encryption Key Needs Rotation'
     AZURE_ENCRYPTION_KEY_ROTATED = 'Azure Encryption Key Rotated'
     AZURE_ENCRYPTION_KEY_NEEDS_ROTATION = 'Azure Encryption Key Needs Rotation'
     GCP_ENCRYPTION_KEY_ROTATED = 'GCP Encryption Key Rotated'
     GCP_ENCRYPTION_KEY_NEEDS_ROTATION = 'GCP Encryption Key Needs Rotation'
     CREDIT_CARD_ADDED = 'Credit Card Added'
@@ -258,14 +276,15 @@
     LOG_DOWNLOAD_STARTED = 'Log Download Started'
     MAINTENANCE_WINDOW_ADDED_AUDIT = 'Maintenance Window Added Audit'
     MAINTENANCE_WINDOW_CHANGED_AUDIT = 'Maintenance Window Changed Audit'
     MAINTENANCE_WINDOW_DELETED_AUDIT = 'Maintenance Window Deleted Audit'
     CLUSTER_CREATED = 'Cluster Created'
     CLUSTER_READY = 'Cluster Ready'
     CLUSTER_UPDATE_SUBMITTED = 'Cluster Update Submitted'
+    CLUSTER_FORCE_RECONFIG_REQUESTED = 'Cluster Force Reconfig Requested'
     CLUSTER_UPDATE_STARTED = 'Cluster Update Started'
     CLUSTER_UPDATE_COMPLETED = 'Cluster Update Completed'
     CLUSTER_PROCESS_ARGS_UPDATE_SUBMITTED = 'Cluster Process Args Update Submitted'
     CLUSTER_AUTOMATICALLY_PAUSED = 'Cluster Automatically Paused'
     CLUSTER_DELETE_SUBMITTED = 'Cluster Delete Submitted'
     CLUSTER_DELETED = 'Cluster Deleted'
     CLUSTER_IMPORT_STARTED = 'Cluster Import Started'
@@ -324,32 +343,25 @@
     PROXY_RESTARTED = 'Proxy Restarted'
     PROXY_PANICKED = 'Proxy Panicked'
     TENANT_CLUSTER_UPGRADE_FROM_MTM = 'Tenant Cluster Upgrade From MTM'
     TENANT_SNAPSHOT_FAILED = 'Tenant Snapshot Failed'
     TENANT_RESTORE_FAILED = 'Tenant Restore Failed'
     SCHEDULED_MAINTENANCE = 'Scheduled Maintenance'
     PROJECT_SCHEDULED_MAINTENANCE = 'Project Scheduled Maintenance'
+    PROJECT_BYPASSED_MAINTENANCE = 'Project Bypassed Maintenance'
     OS_MAINTENANCE = 'Os Maintenance'
     OS_MAINTENANCE_REPLACEMENT = 'Os Maintenance Replacement'
     ATLAS_MAINTENANCE_WINDOW_ADDED = 'Atlas Maintenance Window Added'
     ATLAS_MAINTENANCE_WINDOW_MODIFIED = 'Atlas Maintenance Window Modified'
     ATLAS_MAINTENANCE_WINDOW_REMOVED = 'Atlas Maintenance Window Removed'
     ATLAS_MAINTENANCE_DEFERRED = 'Atlas Maintenance Deferred'
     ATLAS_MAINTENANCE_AUTO_DEFER_ENABLED = 'Atlas Maintenance Auto Defer Enabled'
     ATLAS_MAINTENANCE_AUTO_DEFER_DISABLED = 'Atlas Maintenance Auto Defer Disabled'
     ATLAS_MAINTENANCE_START_ASAP = 'Atlas Maintenance Start Asap'
     ATLAS_MAINTENANCE_SCHEDULED_FOR_NEXT_WINDOW = 'Atlas Maintenance Scheduled For Next Window'
-    MAINTENANCE_WINDOW_ADDED = 'Atlas Maintenance Window Added'
-    MAINTENANCE_WINDOW_MODIFIED = 'Atlas Maintenance Window Modified'
-    MAINTENANCE_WINDOW_REMOVED = 'Atlas Maintenance Window Removed'
-    MAINTENANCE_DEFERRED = 'Atlas Maintenance Deferred'
-    MAINTENANCE_AUTO_DEFER_ENABLED = 'Atlas Maintenance Auto Defer Enabled'
-    MAINTENANCE_AUTO_DEFER_DISABLED = 'Atlas Maintenance Auto Defer Disabled'
-    MAINTENANCE_START_ASAP = 'Atlas Maintenance Start Asap'
-    MAINTENANCE_SCHEDULED_FOR_NEXT_WINDOW = 'Atlas Maintenance Scheduled For Next Window'
     COMPUTE_AUTO_SCALE_UNNECESSARY = 'Compute Auto Scale Unnecessary'
     COMPUTE_AUTO_SCALE_TRIGGERED = 'Compute Auto Scale Triggered'
     COMPUTE_AUTO_SCALE_SKIPPED = 'Compute Auto Scale Skipped'
     COMPUTE_AUTO_SCALE_INITIATED = 'Compute Auto Scale Initiated'
     DISK_AUTO_SCALE_INITIATED = 'Disk Auto Scale Initiated'
     FTS_INDEX_DELETION_FAILED = 'Fts Index Deletion Failed'
     FREE_UPGRADE_STARTED = 'Free Upgrade Started'
@@ -360,20 +372,24 @@
     ENCRYPTION_AT_REST_CONFIGURATION_VALIDATION_FAILED = 'Encryption At Rest Configuration Validation Failed'
     AGENT_VERSION_FIXED = 'Agent Version Fixed'
     AGENT_VERSION_UNFIXED = 'Agent Version Unfixed'
     CLUSTER_INSTANCE_CONFIG_UPDATED = 'Cluster Instance Config Updated'
     CLUSTER_INSTANCE_SSL_ROTATED = 'Cluster Instance SSL Rotated'
     CLUSTER_INSTANCE_SSL_ROTATED_PER_CLUSTER = 'Cluster Instance SSL Rotated Per Cluster'
     CLUSTER_INSTANCE_SSL_REVOKED = 'Cluster Instance SSL Revoked'
+    RELOAD_SSL_ON_PROCESSES = 'Reload SSL On Processes'
     NDS_SET_IMAGE_OVERRIDES = 'Nds Set Image Overrides'
     NDS_SET_CHEF_TARBALL_URI = 'Nds Set Chef Tarball Uri'
     RESTRICTED_EMPLOYEE_ACCESS_BYPASS = 'Restricted Employee Access Bypass'
     CLOUD_PROVIDER_ACCESS_AWS_IAM_ROLE_ADDED = 'Cloud Provider Access AWS Iam Role Added'
     CLOUD_PROVIDER_ACCESS_AWS_IAM_ROLE_DELETED = 'Cloud Provider Access AWS Iam Role Deleted'
     CLOUD_PROVIDER_ACCESS_AWS_IAM_ROLE_UPDATED = 'Cloud Provider Access AWS Iam Role Updated'
+    CLOUD_PROVIDER_ACCESS_AZURE_SERVICE_PRINCIPAL_ADDED = 'Cloud Provider Access Azure Service Principal Added'
+    CLOUD_PROVIDER_ACCESS_AZURE_SERVICE_PRINCIPAL_DELETED = 'Cloud Provider Access Azure Service Principal Deleted'
+    CLOUD_PROVIDER_ACCESS_AZURE_SERVICE_PRINCIPAL_UPDATED = 'Cloud Provider Access Azure Service Principal Updated'
     ORG_CONNECTED_TO_MLAB = 'Org Connected To Mlab'
     ORG_DISCONNECTED_FROM_MLAB = 'Org Disconnected From Mlab'
     MLAB_MIGRATION_INITIATED = 'Mlab Migration Initiated'
     MLAB_MIGRATION_COMPLETED = 'Mlab Migration Completed'
     MLAB_MIGRATION_CANCELLED = 'Mlab Migration Cancelled'
     MLAB_MIGRATION_PREREQUISITES_ACKNOWLEDGED = 'Mlab Migration Prerequisites Acknowledged'
     MLAB_MIGRATION_TARGET_PROJECT_SET = 'Mlab Migration Target Project Set'
@@ -433,25 +449,30 @@
     ORG_PUBLIC_API_WHITELIST_NOT_REQUIRED = 'Org Public API Whitelist Not Required'
     ORG_PUBLIC_API_ACCESS_LIST_REQUIRED = 'Org Public API Access List Required'
     ORG_PUBLIC_API_ACCESS_LIST_NOT_REQUIRED = 'Org Public API Access List Not Required'
     ORG_EMPLOYEE_ACCESS_RESTRICTED = 'Org Employee Access Restricted'
     ORG_EMPLOYEE_ACCESS_UNRESTRICTED = 'Org Employee Access Unrestricted'
     ORG_SFDC_ACCOUNT_ID_CHANGED = 'Org Sfdc Account Id Changed'
     ORG_OVERRIDE_PAYMENT_METHOD_ADDED = 'Org Override Payment Method Added'
+    ORG_UI_IP_ACCESS_LIST_DISABLED = 'Org Ui IP Access List Disabled'
+    ORG_UI_IP_ACCESS_LIST_ENABLED = 'Org Ui IP Access List Enabled'
+    ORG_EDITED_UI_IP_ACCESS_LIST_ENTRIES = 'Org Edited Ui IP Access List Entries'
     API_KEY_WHITELIST_ENTRY_ADDED = 'API Key Whitelist Entry Added'
     API_KEY_ACCESS_LIST_ENTRY_ADDED = 'API Key Access List Entry Added'
     API_KEY_CREATED = 'API Key Created'
     API_KEY_DELETED = 'API Key Deleted'
     TEMP_GLOBAL_API_KEY_CREATED = 'Temp Global API Key Created'
     API_KEY_WHITELIST_ENTRY_DELETED = 'API Key Whitelist Entry Deleted'
     API_KEY_ACCESS_LIST_ENTRY_DELETED = 'API Key Access List Entry Deleted'
     API_KEY_ROLES_CHANGED = 'API Key Roles Changed'
     API_KEY_DESCRIPTION_CHANGED = 'API Key Description Changed'
     API_KEY_ADDED_TO_GROUP = 'API Key Added To Group'
     API_KEY_REMOVED_FROM_GROUP = 'API Key Removed From Group'
+    API_KEY_UI_IP_ACCESS_LIST_INHERITANCE_ENABLED = 'API Key Ui IP Access List Inheritance Enabled'
+    API_KEY_UI_IP_ACCESS_LIST_INHERITANCE_DISABLED = 'API Key Ui IP Access List Inheritance Disabled'
     MONITORING_AGENT_LOGS = 'Monitoring Agent Logs'
     MONITORING_AGENT_LOGS_CSV_DOWNLOAD = 'Monitoring Agent Logs CSV Download'
     AUTOMATION_AGENT_LOGS = 'Automation Agent Logs'
     AUTOMATION_AGENT_LOGS_CSV_DOWNLOAD = 'Automation Agent Logs CSV Download'
     BACKUP_AGENT_LOGS = 'Backup Agent Logs'
     BACKUP_AGENT_LOGS_CSV_DOWNLOAD = 'Backup Agent Logs CSV Download'
     MONITORING_MONGOD_LOGS = 'Monitoring Mongod Logs'
@@ -472,14 +493,15 @@
     ATLAS_TENANT_UPGRADE_SNAPSHOTS = 'Atlas Tenant Upgrade Snapshots'
     VISUAL_PROFILER = 'Visual Profiler'
     REAL_TIME_PERFORMANCE_PANEL = 'Real Time Performance Panel'
     PERFORMANCE_ADVISOR = 'Performance Advisor'
     MONGODB_ACCESS_HISTORY = 'Mongodb Access History'
     TOGGLEABLE_FEATURE_FLAG = 'Toggleable Feature Flag'
     PUBLIC_API_MANAGED_SLOW_MS_FEATURE_FLAG = 'Public API Managed Slow Ms Feature Flag'
+    PUBLIC_API_SEARCH_QUERY_TELEMETRY_FLAG = 'Public API Search Query Telemetry Flag'
     MONITORING_DAILY_PING = 'Monitoring Daily Ping'
     MONITORING_LATEST_HOST_SPECIFIC_PING = 'Monitoring Latest Host Specific Ping'
     MONITORING_GROUP_PING = 'Monitoring Group Ping'
     PUBLIC_API_LATEST_MONITORING_GROUP_PING = 'Public API Latest Monitoring Group Ping'
     PUBLIC_API_LATEST_MONITORING_HOST_SPECIFIC_PING = 'Public API Latest Monitoring Host Specific Ping'
     MEMBER_ADDED = 'Member Added'
     MEMBER_REMOVED = 'Member Removed'
@@ -553,14 +575,16 @@
     MULTI_FACTOR_AUTH_RESET_EMAIL_SENT_AUDIT = 'Multi Factor Auth Reset Email Sent Audit'
     MULTI_FACTOR_AUTH_RESET_AUDIT = 'Multi Factor Auth Reset Audit'
     MULTI_FACTOR_AUTH_UPDATED_AUDIT = 'Multi Factor Auth Updated Audit'
     JOINED_GROUP = 'Joined Group'
     JOINED_ORG = 'Joined Org'
     JOINED_TEAM = 'Joined Team'
     REMOVED_FROM_GROUP = 'Removed From Group'
+    GROUP_INVITATION_DELETED = 'Group Invitation Deleted'
+    ORG_INVITATION_DELETED = 'Org Invitation Deleted'
     INVITED_TO_GROUP = 'Invited To Group'
     INVITED_TO_ORG = 'Invited To Org'
     REQUESTED_TO_JOIN_GROUP = 'Requested To Join Group'
     REMOVED_FROM_ORG = 'Removed From Org'
     REMOVED_FROM_TEAM = 'Removed From Team'
     PASSWORD_RESET_EMAIL_SENT_AUDIT = 'Password Reset Email Sent Audit'
     PASSWORD_RESET_FORM_VIEWED_AUDIT = 'Password Reset Form Viewed Audit'
@@ -595,20 +619,26 @@
     CLEAR_UNPROVISIONED_TARGET_GROUPS_REQUESTED = 'Clear Unprovisioned Target Groups Requested'
     GLOBAL_WHITELIST_ENTRY_CREATED = 'Global Whitelist Entry Created'
     GLOBAL_WHITELIST_ENTRY_UPDATED = 'Global Whitelist Entry Updated'
     GLOBAL_WHITELIST_ENTRY_DELETED = 'Global Whitelist Entry Deleted'
     GLOBAL_ACCESS_LIST_ENTRY_CREATED = 'Global Access List Entry Created'
     GLOBAL_ACCESS_LIST_ENTRY_UPDATED = 'Global Access List Entry Updated'
     GLOBAL_ACCESS_LIST_ENTRY_DELETED = 'Global Access List Entry Deleted'
-    NDS_X509_USER_AUTHENTICATION_MANAGED_USER_CERTS_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Managed User Certs Expiration Resolved'
-    NDS_X509_USER_AUTHENTICATION_MANAGED_USER_CERTS_EXPIRATION_CHECK = 'Nds X509 User Authentication Managed User Certs Expiration Check'
-    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CA_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Customer Ca Expiration Resolved'
-    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CA_EXPIRATION_CHECK = 'Nds X509 User Authentication Customer Ca Expiration Check'
-    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CRL_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Customer CRL Expiration Resolved'
-    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CRL_EXPIRATION_CHECK = 'Nds X509 User Authentication Customer CRL Expiration Check'
+    NDS_X509_USER_AUTHENTICATION_MANAGED_USER_CERTS_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Managed User ' \
+                                                                          'Certs Expiration Resolved '
+    NDS_X509_USER_AUTHENTICATION_MANAGED_USER_CERTS_EXPIRATION_CHECK = 'Nds X509 User Authentication Managed User ' \
+                                                                       'Certs Expiration Check '
+    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CA_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Customer Ca ' \
+                                                                   'Expiration Resolved '
+    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CA_EXPIRATION_CHECK = 'Nds X509 User Authentication Customer Ca Expiration ' \
+                                                                'Check '
+    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CRL_EXPIRATION_RESOLVED = 'Nds X509 User Authentication Customer CRL ' \
+                                                                    'Expiration Resolved '
+    NDS_X509_USER_AUTHENTICATION_CUSTOMER_CRL_EXPIRATION_CHECK = 'Nds X509 User Authentication Customer CRL ' \
+                                                                 'Expiration Check '
     ONLINE_ARCHIVE_INSUFFICIENT_INDEXES_CHECK = 'Online Archive Insufficient Indexes Check'
     ONLINE_ARCHIVE_INSUFFICIENT_INDEXES_RESOLVED = 'Online Archive Insufficient Indexes Resolved'
     ONLINE_ARCHIVE_MAX_CONSECUTIVE_OFFLOADS_CHECK = 'Online Archive Max Consecutive Offloads Check'
     ONLINE_ARCHIVE_UP_TO_DATE = 'Online Archive Up To Date'
     ONLINE_ARCHIVE_CREATED = 'Online Archive Created'
     ONLINE_ARCHIVE_DELETED = 'Online Archive Deleted'
     ONLINE_ARCHIVE_UPDATED = 'Online Archive Updated'
@@ -642,28 +672,31 @@
     CPS_SNAPSHOT_BEHIND = 'Cps Snapshot Behind'
     CPS_SNAPSHOT_FALLBACK_FAILED = 'Cps Snapshot Fallback Failed'
     CPS_OPLOG_BEHIND = 'Cps Oplog Behind'
     CPS_OPLOG_CAUGHT_UP = 'Cps Oplog Caught Up'
     CPS_OPLOG_NOT_CONTIGUOUS = 'Cps Oplog Not Contiguous'
     CPS_RESTORE_SUCCESSFUL = 'Cps Restore Successful'
     CPS_EXPORT_SUCCESSFUL = 'Cps Export Successful'
+    TENANT_UPGRADE_TO_SERVERLESS_SUCCESSFUL = 'Tenant Upgrade To Serverless Successful'
     CPS_RESTORE_FAILED = 'Cps Restore Failed'
     CPS_EXPORT_FAILED = 'Cps Export Failed'
+    TENANT_UPGRADE_TO_SERVERLESS_FAILED = 'Tenant Upgrade To Serverless Failed'
     CPS_SNAPSHOT_DOWNLOAD_REQUEST_FAILED = 'Cps Snapshot Download Request Failed'
     FTS_INDEX_BUILD_COMPLETE = 'Fts Index Build Complete'
     FTS_INDEX_BUILD_FAILED = 'Fts Index Build Failed'
     HOST_USAGE_TYPE_ASSIGNMENT_CHANGE = 'Host Usage Type Assignment Change'
     PHYSICAL_HOST_USAGE_TYPE_ASSIGNMENT_CHANGE = 'Physical Host Usage Type Assignment Change'
     FEDERATION_SETTINGS_CREATED = 'Federation Settings Created'
     FEDERATION_SETTINGS_DELETED = 'Federation Settings Deleted'
     FEDERATION_SETTINGS_UPDATED = 'Federation Settings Updated'
     IDENTITY_PROVIDER_CREATED = 'Identity Provider Created'
     IDENTITY_PROVIDER_UPDATED = 'Identity Provider Updated'
     IDENTITY_PROVIDER_DELETED = 'Identity Provider Deleted'
     IDENTITY_PROVIDER_ACTIVATED = 'Identity Provider Activated'
+    IDENTITY_PROVIDER_DEACTIVATED = 'Identity Provider Deactivated'
     DOMAINS_ASSOCIATED = 'Domains Associated'
     DOMAIN_CREATED = 'Domain Created'
     DOMAIN_DELETED = 'Domain Deleted'
     DOMAIN_VERIFIED = 'Domain Verified'
     ORG_SETTINGS_CONFIGURED = 'Org Settings Configured'
     ORG_SETTINGS_UPDATED = 'Org Settings Updated'
     ORG_SETTINGS_DELETED = 'Org Settings Deleted'
@@ -709,20 +742,24 @@
     HOST_MONGOT_RECOVERED_OOM = 'Host Mongot Recovered Oom'
     SELF_SERVE_DELETION_REQUESTED_AUDIT = 'Self Serve Deletion Requested Audit'
     NDS_BACKGROUND_PROCESSING_DISABLED = 'Nds Background Processing Disabled'
     NDS_BACKGROUND_PROCESSING_ENABLED = 'Nds Background Processing Enabled'
     METER_USAGE_UNDELETED_THROUGH_API = 'Meter Usage Undeleted Through API'
     SYNC_FAILURE = 'Sync Failure'
     TRIGGER_FAILURE = 'Trigger Failure'
+    TRIGGER_AUTO_RESUMED = 'Trigger Auto Resumed'
     URL_CONFIRMATION = 'Url Confirmation'
     SUCCESSFUL_DEPLOY = 'Successful Deploy'
     DEPLOYMENT_FAILURE = 'Deployment Failure'
+    DEPLOYMENT_MODEL_CHANGE_SUCCESS = 'Deployment Model Change Success'
+    DEPLOYMENT_MODEL_CHANGE_FAILURE = 'Deployment Model Change Failure'
     REQUEST_RATE_LIMIT = 'Request Rate Limit'
     ORG_IDP_CERTIFICATE_ABOUT_TO_EXPIRE = 'Org Idp Certificate About To Expire'
     ORG_IDP_CERTIFICATE_CURRENT = 'Org Idp Certificate Current'
+    SETUP_SERVERLESS_INITIATED = 'Setup Serverless Initiated'
     SERVERLESS_DEPLOYMENT_CREATED = 'Serverless Deployment Created'
     SERVERLESS_DEPLOYMENT_DELETED = 'Serverless Deployment Deleted'
     CLUSTER_INSTANCE_ADMIN_BACKUP_SNAPSHOT_REQUESTED = 'Cluster Instance Admin Backup Snapshot Requested'
     ATLAS_ENVOY_SERVERLESS_LOGS = 'Atlas Envoy Serverless Logs'
     ORG_LIMIT_UPDATED = 'Org Limit Updated'
     ATLAS_DATA_LAKE_LOGS = 'Atlas Data Lake Logs'
     PIT_LOGS = 'Pit Logs'
@@ -777,14 +814,15 @@
     CLUSTER_AUTOMATION_CONFIG_PUBLISHED = 'Cluster Automation Config Published'
     ORG_CONNECTED_TO_VERCEL = 'Org Connected To Vercel'
     DEVICE_CODE_CONFIRMED = 'Device Code Confirmed'
     DEVICE_CODE_AUTHORIZED = 'Device Code Authorized'
     UNLINKED_ORG = 'Unlinked Org'
     ORG_UNLINKED_FROM_PAYING_ORG = 'Org Unlinked From Paying Org'
     CLUSTER_LINKED_TO_VERCEL = 'Cluster Linked To Vercel'
+    DATA_API_SETUP_FOR_VERCEL = 'Data API Setup For Vercel'
     DEVICE_REVOKED = 'Device Revoked'
     ROLLING_INDEX_FAILED_INDEX_BUILD = 'Rolling Index Failed Index Build'
     SCHEDULE_CREATED = 'Schedule Created'
     SCHEDULE_DELETE_REQUESTED = 'Schedule Delete Requested'
     SCHEDULE_PAUSE_REQUESTED = 'Schedule Pause Requested'
     SCHEDULE_ENABLE_REQUESTED = 'Schedule Enable Requested'
     SCHEDULE_UPDATE_REQUESTED = 'Schedule Update Requested'
@@ -794,29 +832,38 @@
     DEVICE_REFRESHED = 'Device Refreshed'
     TENANT_ENDPOINT_SERVICE_DEPLOYMENT_CREATED = 'Tenant Endpoint Service Deployment Created'
     TENANT_ENDPOINT_SERVICE_CREATED = 'Tenant Endpoint Service Created'
     TENANT_ENDPOINT_SERVICE_AVAILABLE = 'Tenant Endpoint Service Available'
     TENANT_ENDPOINT_SERVICE_DEPLOYMENT_DELETE_REQUESTED = 'Tenant Endpoint Service Deployment Delete Requested'
     TENANT_ENDPOINT_SERVICE_DELETED = 'Tenant Endpoint Service Deleted'
     TENANT_ENDPOINT_SERVICE_DEPLOYMENT_DELETED = 'Tenant Endpoint Service Deployment Deleted'
-    TENANT_ENDPOINT_SERVICE_DEPLOYMENT_NUM_DESIRED_ENDPOINT_SERVICES_INCREASED = 'Tenant Endpoint Service Deployment Num Desired Endpoint Services Increased'
+    TENANT_ENDPOINT_SERVICE_DEPLOYMENT_NUM_DESIRED_ENDPOINT_SERVICES_INCREASED = 'Tenant Endpoint Service Deployment ' \
+                                                                                 'Num Desired Endpoint Services ' \
+                                                                                 'Increased '
     SERVERLESS_DEPLOYMENT_ENDPOINT_SERVICE_LINKED = 'Serverless Deployment Endpoint Service Linked'
     SERVERLESS_DEPLOYMENT_ENDPOINT_SERVICE_UNLINKED = 'Serverless Deployment Endpoint Service Unlinked'
     CLUSTER_CONNECTION_SAMPLE_COLLECTION_FIELD_NAMES = 'Cluster Connection Sample Collection Field Names'
     ROLLING_INDEX_SUCCESS_INDEX_BUILD = 'Rolling Index Success Index Build'
     ORG_CONNECTION_UNINSTALLED_FROM_VERCEL = 'Org Connection Uninstalled From Vercel'
     SIGNING_KEY_ROTATION_TRIGGERED = 'Signing Key Rotation Triggered'
     SIGNING_KEY_ROTATED = 'Signing Key Rotated'
+    INTERNAL_CLIENT_REGISTERED = 'Internal Client Registered'
+    INTERNAL_CLIENT_DELETED = 'Internal Client Deleted'
+    INTERNAL_CLIENT_ROLES_EDITED = 'Internal Client Roles Edited'
+    INTERNAL_CLIENT_METADATA_EDITED = 'Internal Client Metadata Edited'
+    INTERNAL_CLIENT_SECRET_CREATED = 'Internal Client Secret Created'
+    INTERNAL_CLIENT_SECRET_DELETED = 'Internal Client Secret Deleted'
     GCP_SELF_SERVE_ACCOUNT_LINK_PENDING = 'GCP Self Serve Account Link Pending'
     GCP_SELF_SERVE_ACCOUNT_LINK_FAILED = 'GCP Self Serve Account Link Failed'
     QUOTA_USAGE_EXCEEDED_EVENT = 'Quota Usage Exceeded Event'
     QUOTA_USAGE_WARNING_EVENT = 'Quota Usage Warning Event'
     QUOTA_USAGE_CRITICAL_WARNING_EVENT = 'Quota Usage Critical Warning Event'
     QUOTA_USAGE_CRITICAL_WARNING_PAGE_EVENT = 'Quota Usage Critical Warning Page Event'
     PROJECT_OPERATIONAL_LIMIT_UPDATED = 'Project Operational Limit Updated'
+    PROJECT_ENABLE_EXTENDED_STORAGE_SIZES = 'Project Enable Extended Storage Sizes'
     GCP_SELF_SERVE_ACCOUNT_LINKED = 'GCP Self Serve Account Linked'
     TENANT_ENDPOINT_CREATED = 'Tenant Endpoint Created'
     TENANT_ENDPOINT_RESERVED = 'Tenant Endpoint Reserved'
     TENANT_ENDPOINT_RESERVATION_FAILED = 'Tenant Endpoint Reservation Failed'
     TENANT_ENDPOINT_UPDATED = 'Tenant Endpoint Updated'
     TENANT_ENDPOINT_AVAILABLE = 'Tenant Endpoint Available'
     TENANT_ENDPOINT_FAILED = 'Tenant Endpoint Failed'
@@ -832,14 +879,16 @@
     BILLING_EMAIL_ADDRESS_ADDED = 'Billing Email Address Added'
     BILLING_EMAIL_ADDRESS_CHANGED = 'Billing Email Address Changed'
     BILLING_EMAIL_ADDRESS_REMOVED = 'Billing Email Address Removed'
     INDEX_FAILED_INDEX_BUILD = 'Index Failed Index Build'
     INDEX_SUCCESS_INDEX_BUILD = 'Index Success Index Build'
     INGESTION_PIPELINE_CREATED = 'Ingestion Pipeline Created'
     INGESTION_PIPELINE_UPDATED = 'Ingestion Pipeline Updated'
+    DATA_FEDERATION_QUERY_LIMIT_CONFIGURED = 'Data Federation Query Limit Configured'
+    DATA_FEDERATION_QUERY_LIMIT_DELETED = 'Data Federation Query Limit Deleted'
     CLUSTER_PREFERRED_CPU_ARCHITECTURE_MODIFIED = 'Cluster Preferred Cpu Architecture Modified'
     USER_ACCOUNT_EMAIL_ADDRESS_CHANGED_AUDIT = 'User Account Email Address Changed Audit'
     ONLINE_ARCHIVE_DATA_EXPIRATION_DID_NOT_RUN = 'Online Archive Data Expiration Did Not Run'
     ONLINE_ARCHIVE_DATA_EXPIRATION_RESOLVED = 'Online Archive Data Expiration Resolved'
     LOG_FORWARDER_FAILURE = 'Log Forwarder Failure'
     CLUSTER_UNLINKED_FROM_VERCEL = 'Cluster Unlinked From Vercel'
     INGESTION_PIPELINE_DESTROYED = 'Ingestion Pipeline Destroyed'
@@ -876,7 +925,41 @@
     PROJECT_LIVE_IMPORT_OVERRIDES_ADDED = 'Project Live Import Overrides Added'
     PROJECT_LIVE_IMPORT_OVERRIDES_UPDATED = 'Project Live Import Overrides Updated'
     PROJECT_LIVE_IMPORT_OVERRIDES_DELETED = 'Project Live Import Overrides Deleted'
     CLUSTER_FORCE_PLANNED = 'Cluster Force Planned'
     SUFFICIENT_FILESYSTEM_STORE_FREE_SPACE = 'Sufficient Filesystem Store Free Space'
     LOW_FILESYSTEM_STORE_FREE_SPACE_PERCENT = 'Low Filesystem Store Free Space Percent'
     PENDING_INDEXES_CANCELED = 'Pending Indexes Canceled'
+    PREPAID_PLAN_MODIFIED = 'Prepaid Plan Modified'
+    AZURE_SELF_SERVE_ACCOUNT_LINKED = 'Azure Self Serve Account Linked'
+    AZURE_SELF_SERVE_ACCOUNT_LINK_PENDING = 'Azure Self Serve Account Link Pending'
+    AZURE_SELF_SERVE_ACCOUNT_CANCELLED = 'Azure Self Serve Account Cancelled'
+    AZURE_SELF_SERVE_ACCOUNT_LINK_FAILED = 'Azure Self Serve Account Link Failed'
+    BACKUP_NOT_LATE_TRACKING_JOB = 'Backup Not Late Tracking Job'
+    BACKUP_LATE_TRACKING_JOB = 'Backup Late Tracking Job'
+    BACKUP_NOT_LATE_INTEGRITY_CHECK_JOB = 'Backup Not Late Integrity Check Job'
+    BACKUP_LATE_INTEGRITY_CHECK_JOB = 'Backup Late Integrity Check Job'
+    BACKUP_NOT_LATE_GROOM_JOB = 'Backup Not Late Groom Job'
+    BACKUP_LATE_GROOM_JOB = 'Backup Late Groom Job'
+    CHARGE_PENDING_REVERSAL = 'Charge Pending Reversal'
+    AZURE_USAGE_REPORTED = 'Azure Usage Reported'
+    COMPUTE_AUTO_SCALE_TRIGGERED_BASE = 'Compute Auto Scale Triggered Base'
+    COMPUTE_AUTO_SCALE_TRIGGERED_ANALYTICS = 'Compute Auto Scale Triggered Analytics'
+    COMPUTE_AUTO_SCALE_SKIPPED_BASE = 'Compute Auto Scale Skipped Base'
+    COMPUTE_AUTO_SCALE_SKIPPED_ANALYTICS = 'Compute Auto Scale Skipped Analytics'
+    COMPUTE_AUTO_SCALE_INITIATED_BASE = 'Compute Auto Scale Initiated Base'
+    COMPUTE_AUTO_SCALE_INITIATED_ANALYTICS = 'Compute Auto Scale Initiated Analytics'
+    DATA_PROCESSING_REGION_UPDATED = 'Data Processing Region Updated'
+    CLUSTER_REGIONAL_OUTAGE_SIMULATION_STARTED = 'Cluster Regional Outage Simulation Started'
+    CLUSTER_REGIONAL_OUTAGE_SIMULATION_FAILED_TO_START = 'Cluster Regional Outage Simulation Failed To Start'
+    CLUSTER_REGIONAL_OUTAGE_SIMULATION_END_REQUESTED = 'Cluster Regional Outage Simulation End Requested'
+    CLUSTER_REGIONAL_OUTAGE_SIMULATION_COMPLETED = 'Cluster Regional Outage Simulation Completed'
+    CLUSTER_REGIONAL_OUTAGE_SIMULATION_CANCELLED_CLUSTER_PAUSE = 'Cluster Regional Outage Simulation Cancelled ' \
+                                                                 'Cluster Pause '
+    AZURE_BILLING_ACCOUNT_CREDIT_ISSUED = 'Azure Billing Account Credit Issued'
+    UIS_PANICKED = 'Uis Panicked'
+    ADMIN_LOCK_UPDATED = 'Admin Lock Updated'
+    ATLAS_USER_IDENTITY_SERVICE_LOGS = 'Atlas User Identity Service Logs'
+    CLUSTER_UPDATE_SUBMITTED_INTERNAL = 'Cluster Update Submitted Internal'
+    CLUSTER_DELETE_SUBMITTED_INTERNAL = 'Cluster Delete Submitted Internal'
+    FLAPPING_STOPPED = 'Flapping Stopped'
+    FLAPPING_STARTED = 'Flapping Started'
```

### Comparing `atlasapi-3.0.1b5/atlasapi/invoices_pydantic.py` & `atlasapi-3.0.1b6/atlasapi/invoices_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/lib.py` & `atlasapi-3.0.1b6/atlasapi/lib.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/maintenance_window.py` & `atlasapi-3.0.1b6/atlasapi/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/measurements.py` & `atlasapi-3.0.1b6/atlasapi/measurements.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/network.py` & `atlasapi-3.0.1b6/atlasapi/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,32 +14,59 @@
 
 """
 Network module
 
 Module which handles the basic network operations with the Atlas API>
 """
 
+import datetime
 from math import ceil
 import requests
 from requests.auth import HTTPDigestAuth, HTTPBasicAuth
 from atlasapi.settings import Settings
 from atlasapi.errors import *
 import logging
+import urllib.parse
+import urllib.request
+from dateutil.tz import UTC
 from json import dumps
 from io import BytesIO
 from typing import Union
 
+
+
+
 logger = logging.getLogger('network')
 logger.setLevel(logging.WARNING)
 
+external_ip = 'Unknown'
+if logger.level == logging.INFO:
+    try:
+        external_ip = urllib.request.urlopen('https://ident.me').read().decode('utf8')
+    except Exception as e:
+        logger.warning(f"Could not get public IP: {e}")
+
 
 def merge(dict1, dict2):
     return dict2.update(dict1)
 
 
+def atlas_encode_dt(dt: datetime.datetime) -> str:
+    """Encode a datetime (must already be UTC!) for the Atlas API."""
+    # Atlas requires "Z" suffix, not Python's usual "+00:00" for UTC.
+    return dt.replace(tzinfo=None).isoformat() + 'Z'
+
+
+def atlas_encode_params(params: dict) -> str:
+    # Use "safe" to permit ":" in ISO8601 datetimes.
+    return urllib.parse.urlencode(
+        {k: atlas_encode_dt(v) if isinstance(v, datetime.datetime) else v
+         for k, v in params.items() if v is not None}, safe=':')
+
+
 class Network:
     """Network constructor
     
     Args:
         user (str): user
         password (str): password
     """
@@ -72,27 +99,28 @@
         if c in [Settings.SUCCESS, Settings.CREATED, Settings.ACCEPTED, Settings.NO_CONTENT]:
             return details
         elif c == Settings.BAD_REQUEST:
             raise ErrAtlasBadRequest(c, details)
         elif c == Settings.UNAUTHORIZED:
             raise ErrAtlasUnauthorized(c, details)
         elif c == Settings.FORBIDDEN:
+            logger.error(f"Got FORBIDDEN, we are using external ip {external_ip}")
+            details["external_ip"] = external_ip
             raise ErrAtlasForbidden(c, details)
         elif c == Settings.NOTFOUND:
             raise ErrAtlasNotFound(c, details)
         elif c == Settings.METHOD_NOT_ALLOWED:
             raise ErrAtlasMethodNotAllowed(c, details)
         elif c == Settings.CONFLICT:
             raise ErrAtlasConflict(c, details)
         else:
             # Settings.SERVER_ERRORS
             raise ErrAtlasServerErrors(c, details)
 
-    # noinspection PyArgumentList
-    def get_file(self, uri, **kwargs):
+    def get_file(self, uri):
         """Get request which returns a binary file
 
         Args:
             uri (str): URI
 
         Returns:
             Binary File: API response as file
@@ -105,35 +133,29 @@
         try:
             file_obj = BytesIO()
             r = requests.get(uri,
                              allow_redirects=False,
                              stream=True,
                              timeout=Settings.file_request_timeout,
                              headers={},
-                             auth=self.auth_method(self.key, self.secret),
-                             **kwargs)
+                             auth=self.auth_method(self.key, self.secret))
             logger.debug("Auth information = {} {}".format(self.key, self.secret))
-            if kwargs is not None:
-                logger.info(f"kwargs are: {kwargs}")
 
             for chunk in r.iter_content(chunk_size=1024):
                 # writing one chunk at a time to  file
                 if chunk:
                     logger.debug("Writing 1 Kbyte chunk to the file like object")
                     file_obj.write(chunk)
             logger.info("---- Completed downloading the file. ----")
             return self.answer(r.status_code, file_obj)
 
-        except Exception as e:
-            try:
-                logger.warning('Request: {}'.format(r.request.__dict__))
-                logger.warning('Response: {}'.format(r.__dict__))
-                raise e
-            except AttributeError:
-                raise e
+        except Exception:
+            logger.warning('Request: {}'.format(r.request.__dict__))
+            logger.warning('Response: {}'.format(r.__dict__))
+            raise
         finally:
             if r:
                 r.connection.close()
 
     def _paginate(self, method , url, **kwargs):
         """(Internal) Paginate requests
         
@@ -145,28 +167,39 @@
             dict: Response payload
         """
         session = None
 
         try:
             logger.debug(f"{method} - URI Being called is {url}")
             session = requests.Session()
-            request = session.request(method=method, url=url, **kwargs)
-            logger.debug("Request arguments: {}".format(str(kwargs)))
+            logger.info("🔎🔎Request arguments: {}".format(str(kwargs)))
+            if kwargs.get('params'):
+                existing_params: dict = kwargs.get('params')
+                logger.debug(f"Existing params are: {existing_params}")
+                existing_params.update(dict(itemsPerPage=Settings.itemsPerPage))
+                logger.debug(f"New params are {existing_params}")
+                kwargs["params"] = existing_params
+                logger.debug(f"Fully updated kwargs is now... {kwargs}")
+
+            request = session.request(method=method, url=url,**kwargs)
+            logger.info("Request arguments: {}".format(str(kwargs)))
+
             first_page = self.answer(request.status_code, request.json())
             yield first_page
             total_count = first_page.get("totalCount", 0)
             items_per_page = Settings.itemsPerPage
             if total_count > items_per_page:
                 logger.warning(f"More than on page required, proceeding . . .")
                 for page_number in range(2, ceil(total_count / items_per_page) + 1):
                     # Need to ensure that any params sent in kwargs are merged with the pageNum param.
                     if kwargs.get('params'):
                         existing_params: dict = kwargs.get('params')
                         logger.debug(f"Existing params are: {existing_params}")
                         existing_params.update(dict(pageNum=page_number))
+                        existing_params.update(dict(itemsPerPage=Settings.itemsPerPage))
                         logger.debug(f"New params are {existing_params}")
                         kwargs["params"] = existing_params
                         logger.debug(f"Fully updated kwargs is now... {kwargs}")
                     request = session.request(method=method, url=url, **kwargs)
                     logger.debug("Request arguments: {}".format(str(kwargs)))
                     next_page = self.answer(request.status_code, request.json())
                     yield next_page
@@ -210,14 +243,15 @@
             
         Raises:
             Exception: Network issue
         """
         r = None
 
         try:
+            print(f"The URI is: {uri}")
             r = requests.post(uri,
                               json=payload,
                               allow_redirects=True,
                               timeout=Settings.requests_timeout,
                               headers={"Content-Type": "application/json"},
                               auth=self.auth_method(self.key, self.secret))
             return self.answer(r.status_code, r.json())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atlasapi-3.0.1b5/atlasapi/organizations.py` & `atlasapi-3.0.1b6/atlasapi/organizations.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/projects.py` & `atlasapi-3.0.1b6/atlasapi/projects.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/serverless_pydantic.py` & `atlasapi-3.0.1b6/atlasapi/serverless_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/settings.py` & `atlasapi-3.0.1b6/atlasapi/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,19 @@
     ITEMS_PER_PAGE: int = int(os.getenv('ITEMS_PER_PAGE', 500))
 
     api_resources = {
         "Project": {
             "Get One Project": URI_STUB + "/groups/{GROUP_ID}"
         },
         "Monitoring and Logs": {
-            "Get all processes for group": URI_STUB + "/groups/{group_id}/processes",
+            "Get all processes for group": URI_STUB + "/groups/{GROUP_ID}/processes",
             "Get information for process in group": URI_STUB + "/groups/%s/processes/%s:&s?pageNum=%d"
                                                                "&itemsPerPage=%d",
             "Get measurement for host": URI_STUB + "/groups/{group_id}/processes/{host}:{"
-                                                   "port}/measurements?granularity={granularity}&period={period}"
-                                                   "&m={measurement}",
+                                                   "port}/measurements",
             "Get list of databases for host": "/api/atlas/v1.0/groups/{GROUP-ID}/processes/{HOST}:{PORT}/databases",
             "Get measurements of database for host.": "/api/atlas/v1.0/groups/{GROUP-ID}/processes/{HOST}:{"
                                                       "PORT}/databases/{DATABASE-NAME}/measurements",
             "Get list of disks or partitions for host.": "/api/atlas/v1.0/groups/{GROUP-ID}/processes/{HOST}:{"
                                                          "PORT}/disks",
             "Get measurements of for host": "/api/atlas/v1.0/groups/{GROUP-ID}/processes/{HOST}:{PORT}/disks/{"
                                             "DISK-NAME}/measurements",
```

### Comparing `atlasapi-3.0.1b5/atlasapi/specs.py` & `atlasapi-3.0.1b6/atlasapi/specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         Returns:
              Iterable[AtlasMeasurement] or dict: Iterable object representing this function OR Response payload
 
         Raises:
 
 
         """
-
+        measurement_list = list()
         # Set default
         if measurement is None:
             measurement = AtlasMeasurementTypes.Cache.dirty
             logger.info(f'The measurement is {measurement}')
         if period is None:
             period = AtlasPeriods.WEEKS_1
         logger.info(f'The granularity is {granularity}')
@@ -195,31 +195,30 @@
 
         # Check to see if we received a leaf or branch of the measurements
         try:
             parent = super(measurement)
             logger.info('We received a branch, whos parent is {}'.format(parent.__str__()))
             leaves = measurement.get_all()
             measurement_list = list(leaves)
-            measurement = '&m='.join(measurement_list)
         except TypeError:
             logger.info('We received a leaf')
+        if len(measurement_list) < 1:
+            measurement_list.append(measurement)
 
         # Build the URL
         uri = Settings.api_resources["Monitoring and Logs"]["Get measurement for host"].format(
             group_id=self.group_id,
             host=self.hostname,
-            port=self.port,
-            granularity=granularity,
-            period=period,
-            measurement=measurement
+            port=self.port
         )
         logger.info(f'The URI is.... {uri}')
+        parameters = {'granularity': granularity, 'period': period, 'm': measurement_list}
 
         # Build the request
-        return_val = atlas_obj.network.get(Settings.BASE_URL + uri)
+        return_val = atlas_obj.network.get(Settings.BASE_URL + uri, params=parameters)
         for each_response in return_val:
             for each_measurement in each_response.get("measurements"):
                 measurement_obj = AtlasMeasurement(name=each_measurement.get('name'),
                                                    units=each_measurement.get('units', None),
                                                    period=period,
                                                    granularity=granularity)
                 for each_and_every in each_measurement.get('dataPoints'):
```

### Comparing `atlasapi-3.0.1b5/atlasapi/teams.py` & `atlasapi-3.0.1b6/atlasapi/teams.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi/whitelist.py` & `atlasapi-3.0.1b6/atlasapi/whitelist.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlasapi.egg-info/PKG-INFO` & `atlasapi-3.0.1b6/atlasapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b5
+Version: 3.0.1b6
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b5/atlasapi.egg-info/SOURCES.txt` & `atlasapi-3.0.1b6/atlasapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlascli/__init__.py` & `atlasapi-3.0.1b6/atlascli/__init__.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlascli/atlaserrors.py` & `atlasapi-3.0.1b6/atlascli/atlaserrors.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlascli/atlaskey.py` & `atlasapi-3.0.1b6/atlascli/atlaskey.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlascli/cli.py` & `atlasapi-3.0.1b6/atlascli/cli.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/atlascli/listcommand.py` & `atlasapi-3.0.1b6/atlascli/listcommand.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b5/setup.py` & `atlasapi-3.0.1b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import find_packages, setup
 
 setup(
     name='atlasapi',
-    version='3.0.1b5',
+    version='3.0.1b6',
     python_requires='>=3.7',
     packages=find_packages(exclude=("tests",)),
     install_requires=['requests', 'python-dateutil', 'isodate', 'future', 'pytz','coolname',
                       'humanfriendly', 'pydantic', 'pyhumps', 'nose'],
     setup_requires=['wheel'],
     # Metadata
     author="Matthew G. Monteleone",
```

