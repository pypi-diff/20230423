# Comparing `tmp/foursight-3.4.0.1b7.tar.gz` & `tmp/foursight-3.4.0.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.4.0.1b7.tar", max compression
+gzip compressed data, was "foursight-3.4.0.5b2.tar", max compression
```

## Comparing `foursight-3.4.0.1b7.tar` & `foursight-3.4.0.5b2.tar`

### file list

```diff
@@ -1,34 +1,27 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.0.1b7/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.0.1b7/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.0.1b7/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.0.1b7/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.0.1b7/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0    53878 2022-12-28 10:57:56.906089 foursight-3.4.0.1b7/chalicelib_fourfront/check_setup.json-20221228
--rw-r--r--   0        0        0    54449 2023-01-06 03:27:49.344020 foursight-3.4.0.1b7/chalicelib_fourfront/check_setup.json-debug
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.0.1b7/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    59585 2023-01-19 14:12:17.959883 foursight-3.4.0.1b7/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.0.1b7/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.0.1b7/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.0.1b7/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.0.1b7/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.0.1b7/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.0.1b7/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.0.1b7/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45202 2023-01-19 14:12:17.990151 foursight-3.4.0.1b7/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0    45238 2023-01-06 03:27:33.359253 foursight-3.4.0.1b7/chalicelib_fourfront/checks/system_checks.py-debug
--rw-r--r--   0        0        0     2325 2022-11-23 00:12:24.017150 foursight-3.4.0.1b7/chalicelib_fourfront/checks/test_checks.py-backup-for-delete-20221128
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.0.1b7/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.0.1b7/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.0.1b7/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.0.1b7/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.0.1b7/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     8580 2022-11-04 15:36:09.144135 foursight-3.4.0.1b7/chalicelib_fourfront/x
--rw-r--r--   0        0        0     8506 2022-11-04 15:36:19.535078 foursight-3.4.0.1b7/chalicelib_fourfront/xx
--rw-r--r--   0        0        0     1210 2023-04-21 20:52:11.585907 foursight-3.4.0.1b7/pyproject.toml
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 foursight-3.4.0.1b7/setup.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 foursight-3.4.0.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.0.5b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.0.5b2/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.0.5b2/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.0.5b2/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.0.5b2/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.0.5b2/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    59585 2023-01-19 14:12:17.959883 foursight-3.4.0.5b2/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.0.5b2/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.0.5b2/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.0.5b2/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.0.5b2/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.0.5b2/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.0.5b2/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.0.5b2/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45202 2023-01-19 14:12:17.990151 foursight-3.4.0.5b2/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.0.5b2/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.0.5b2/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.0.5b2/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.0.5b2/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.0.5b2/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1210 2023-04-23 01:26:20.887567 foursight-3.4.0.5b2/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 foursight-3.4.0.5b2/PKG-INFO
```

### Comparing `foursight-3.4.0.1b7/LICENSE.txt` & `foursight-3.4.0.5b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/app_utils.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/check_schedules.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/check_setup.json` & `foursight-3.4.0.5b2/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/system_checks.py-debug` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,984 +1,859 @@
-import requests
-import json
-import datetime
-import boto3
-import time
-import geocoder
-from foursight_core.stage import Stage
-from foursight_core.checks.helpers.sys_utils import (
-    parse_datetime_to_utc,
-    wipe_build_indices
-)
-from dcicutils import (
-    ff_utils,
-    es_utils,
-    beanstalk_utils,
-    env_utils
-)
+from datetime import datetime
+from dcicutils import ff_utils
+from dcicutils.s3_utils import s3Utils
+from .helpers import wfr_utils
+from .helpers import wfrset_utils
 
 # Use confchecks to import decorators object and its methods for each check module
 # rather than importing check_function, action_function, CheckResult, ActionResult
 # individually - they're now part of class Decorators in foursight-core::decorators
 # that requires initialization with foursight prefix.
 from .helpers.confchecks import *
 
+lambda_limit = wfr_utils.lambda_limit
 
-# XXX: put into utils?
-FF_BLUE_ES_CLUSTER_DOMAIN = 'fourfront-blue-6-8'
-FF_GREEN_ES_CLUSTER_DOMAIN = 'fourfront-green-6-8'
-PROD_ES_CLUSTERS = [
-    FF_BLUE_ES_CLUSTER_DOMAIN,
-    FF_GREEN_ES_CLUSTER_DOMAIN
-]
-FF_TEST_CLUSTER = 'search-fourfront-testing-6-8-kncqa2za2r43563rkcmsvgn2fq.us-east-1.es.amazonaws.com:443'
-TEST_ES_CLUSTERS = [
-    FF_TEST_CLUSTER
-]
-
-
-@check_function()
-def wipe_ff_build_indices(connection, **kwargs):
-    """ Wipes build (number prefixed) indices (on fourfront-testing) """
-    check = CheckResult(connection, 'wipe_ff_build_indices')
-    return wipe_build_indices(FF_TEST_CLUSTER, check)
-
-
-@check_function(xyzzy_item_type=["SampleProcessing"])
-def elastic_search_space(connection, **kwargs):
-    """ Checks that our ES nodes all have a certain amount of space remaining """
-    check = CheckResult(connection, 'elastic_search_space')
-    full_output = {}
-    client = es_utils.create_es_client(connection.ff_es, True)
-    # use cat.nodes to get id,diskAvail for all nodes, filter out empties
-    node_space_entries = filter(None, [data.split() for data in client.cat.nodes(h='id,diskAvail').split('\n')])
-    check.summary = check.description = None
-    full_output['nodes'] = {}
-    for _id, remaining_space in node_space_entries:
-        if 'gb' not in remaining_space:
-            if 'mb' not in remaining_space:
-                check.status = 'FAIL'
-                check.summary = check.description = 'At least one of the nodes in this env has no space remaining'
-            else:
-                check.status = 'WARN'
-                check.summary = check.description = 'At least one of the nodes in this env is low on space'
-        full_output['nodes'][_id.strip()] = { 'remaining_space': remaining_space }
-    if check.summary is None:
-        check.status = 'PASS'
-        check.summary = check.description = 'All nodes have >1gb remaining disk space'
-    check.full_output = full_output
-    return check
 
-
-def resolve_es_domain_name(connection):
-    """ Resolves blue vs. green depending on the URL, throwing exception if something.  """
-    if 'fourfront-blue' in connection.ff_es:
-        return FF_BLUE_ES_CLUSTER_DOMAIN
-    elif 'fourfront-green' in connection.ff_es:
-        return FF_GREEN_ES_CLUSTER_DOMAIN
-    else:
-        raise Exception('Tried to run autoscaling check on non-production cluster! %s' % connection.ff_es)
-
-
-@check_function()
-def scale_down_elasticsearch_production(connection, **kwargs):
-    """ Scales down Elasticsearch (production configuration).
-        HOT (0600 to 2000 EST):
-            Master:
-                3x c5.large.elasticsearch
-            Data:
-                2x c5.2xlarge.elasticsearch
-        COLD (2000 to 0600 EST):  This is what we are resizing to
-            Master:
-                None
-            Data:
-                3x c5.xlarge.elasticsearch
-        XXX: should probably use constants in ElasticSearchServiceClient
-        For now, must be explicitly triggered - but should be put on a schedule.
+@check_function(lab_title=None, start_date=None, action="chipseq_start")
+def chipseq_status(connection, **kwargs):
     """
-    check = CheckResult(connection, 'scale_down_elasticsearch_production')
-    es_client = es_utils.ElasticSearchServiceClient()
-    success = es_client.resize_elasticsearch_cluster(
-                domain_name=resolve_es_domain_name(connection),
-                master_node_type='t2.medium.elasticsearch',  # discarded
-                master_node_count=0,
-                data_node_type='c5.xlarge.elasticsearch',
-                data_node_count=3
-            )
-    if not success:
-        check.status = 'ERROR'
-        check.description = 'Could not trigger cluster resize - check lambda logs'
-    else:
-        check.status = 'PASS'
-        check.description = 'Downward cluster resize triggered'
-    return check
-
-
-@check_function()
-def scale_up_elasticsearch_production(connection, **kwargs):
-    """ Scales up Elasticsearch (production configuration).
-        HOT (0600 to 2000 EST):  This is what we are resizing to
-            Master:
-                3x c5.large.elasticsearch
-            Data:
-                2x c5.2xlarge.elasticsearch
-        COLD (2000 to 0600 EST):
-            Master:
-                None
-            Data:
-                2x c5.large.elasticsearch
-        XXX: should probably use constants in ElasticSearchServiceClient
-        For now, must be explicitly triggered - but should be put on a schedule.
+    Keyword arguments:
+    lab_title -- limit search with a lab i.e. Bing+Ren, UCSD
+    start_date -- limit search to files generated since a date formatted YYYY-MM-DD
+    run_time -- assume runs beyond run_time are dead
     """
-    check = CheckResult(connection, 'scale_up_elasticsearch_production')
-    es_client = es_utils.ElasticSearchServiceClient()
-    success = es_client.resize_elasticsearch_cluster(
-                domain_name=resolve_es_domain_name(connection),
-                master_node_type='c5.large.elasticsearch',
-                master_node_count=3,
-                data_node_type='c5.2xlarge.elasticsearch',
-                data_node_count=2
-            )
-    if not success:
-        check.status = 'ERROR'
-        check.description = 'Could not trigger cluster resize - check lambda logs'
-    else:
-        check.status = 'PASS'
-        check.description = 'Downward cluster resize triggered'
-    return check
-
-
-# @check_function()
-# def elastic_beanstalk_health(connection, **kwargs):
-#     """
-#     Check both environment health and health of individual instances
-#     """
-#     check = CheckResult(connection, 'elastic_beanstalk_health')
-#     full_output = {}
-#     eb_client = boto3.client('elasticbeanstalk')
-#     resp = eb_client.describe_environment_health(
-#         EnvironmentName=connection.ff_env,
-#         AttributeNames=['All']
-#     )
-#     resp_status = resp.get('ResponseMetadata', {}).get('HTTPStatusCode', None)
-#     if resp_status >= 400:
-#         check.status = 'ERROR'
-#         check.description = 'Could not establish a connection to AWS (status %s).' % resp_status
-#         return check
-#     full_output['status'] = resp.get('Status')
-#     full_output['environment_name'] = resp.get('EnvironmentName')
-#     full_output['color'] = resp.get('Color')
-#     full_output['health_status'] = resp.get('HealthStatus')
-#     full_output['causes'] = resp.get('Causes')
-#     full_output['instance_health'] = []
-#     # now look at the individual instances
-#     resp = eb_client.describe_instances_health(
-#         EnvironmentName=connection.ff_env,
-#         AttributeNames=['All']
-#     )
-#     resp_status = resp.get('ResponseMetadata', {}).get('HTTPStatusCode', None)
-#     if resp_status >= 400:
-#         check.status = 'ERROR'
-#         check.description = 'Could not establish a connection to AWS (status %s).' % resp_status
-#         return check
-#     instances_health = resp.get('InstanceHealthList', [])
-#     for instance in instances_health:
-#         inst_info = {}
-#         inst_info['deploy_status'] = instance['Deployment']['Status']
-#         inst_info['deploy_version'] = instance['Deployment']['VersionLabel']
-#         # get version deployment time
-#         application_versions = eb_client.describe_application_versions(
-#             ApplicationName='4dn-web',
-#             VersionLabels=[inst_info['deploy_version']]
-#         )
-#         deploy_info = application_versions['ApplicationVersions'][0]
-#         inst_info['version_deployed_at'] = datetime.datetime.strftime(deploy_info['DateCreated'], "%Y-%m-%dT%H:%M:%S")
-#         inst_info['instance_deployed_at'] = datetime.datetime.strftime(instance['Deployment']['DeploymentTime'], "%Y-%m-%dT%H:%M:%S")
-#         inst_info['instance_launced_at'] = datetime.datetime.strftime(instance['LaunchedAt'], "%Y-%m-%dT%H:%M:%S")
-#         inst_info['id'] = instance['InstanceId']
-#         inst_info['color'] = instance['Color']
-#         inst_info['health'] = instance['HealthStatus']
-#         inst_info['causes'] = instance.get('causes', [])
-#         full_output['instance_health'].append(inst_info)
-#     if full_output['color'] == 'Grey':
-#         check.status = 'WARN'
-#         check.summary = check.description = 'EB environment is updating'
-#     elif full_output['color'] == 'Yellow':
-#         check.status = 'WARN'
-#         check.summary = check.description = 'EB environment is compromised; requests may fail'
-#     elif full_output['color'] == 'Red':
-#         check.status = 'FAIL'
-#         check.summary = check.description = 'EB environment is degraded; requests are likely to fail'
-#     else:
-#         check.summary = check.description = 'EB environment seems healthy'
-#         check.status = 'PASS'
-#     check.full_output = full_output
-#     return check
-
-
-@check_function()
-def status_of_elasticsearch_indices(connection, **kwargs):
-    check = CheckResult(connection, 'status_of_elasticsearch_indices')
-    ### the check
-    client = es_utils.create_es_client(connection.ff_es, True)
-    indices = client.cat.indices(v=True).split('\n')
-    split_indices = [ind.split() for ind in indices]
-    headers = split_indices.pop(0)
-    index_info = {} # for full output
-    warn_index_info = {} # for brief output
-    for index in split_indices:
-        if len(index) == 0:
-            continue
-        index_info[index[2]] = {header: index[idx] for idx, header in enumerate(headers)}
-        if index_info[index[2]]['health'] != 'green' or index_info[index[2]]['status'] != 'open':
-            warn_index_info[index[2]] = index_info[index[2]]
-    # set fields, store result
-    if not index_info:
-        check.status = 'FAIL'
-        check.summary = 'Error reading status of ES indices'
-        check.description = 'Error reading status of ES indices'
-    elif warn_index_info:
-        check.status = 'WARN'
-        check.summary = 'ES indices may not be healthy'
-        check.description = 'One or more ES indices have health != green or status != open.'
-        check.brief_output = warn_index_info
-    else:
-        check.status = 'PASS'
-        check.summary = 'ES indices seem healthy'
-    check.full_output = index_info
-    return check
-
-
-@check_function()
-def indexing_progress(connection, **kwargs):
-    check = CheckResult(connection, 'indexing_progress')
-    # get latest and db/es counts closest to 10 mins ago
-    counts_check = CheckResult(connection, 'item_counts_by_type')
-    latest = counts_check.get_primary_result()
-    prior = counts_check.get_closest_result(diff_mins=30)
-    if not latest.get('full_output') or not prior.get('full_output'):
-        check.status = 'ERROR'
-        check.description = 'There are no item_counts_by_type results to run this check with.'
+    start = datetime.utcnow()
+    check = CheckResult(connection, 'chipseq_status')
+    my_auth = connection.ff_keys
+    check.action = "chipseq_start"
+    check.description = "run missing steps and add processing results to processed files, match set status"
+    check.brief_output = []
+    check.summary = ""
+    check.full_output = {'skipped': [], 'running_runs': [], 'needs_runs': [],
+                         'completed_runs': [], 'problematic_runs': []}
+    check.status = 'PASS'
+    exp_type = 'ChIP-seq'
+    # completion tag
+    tag = wfr_utils.accepted_versions[exp_type][-1]
+    # check indexing queue
+    check, skip = wfr_utils.check_indexing(check, connection)
+    if skip:
         return check
-    latest_unindexed = latest['full_output']['ALL']['DB'] - latest['full_output']['ALL']['ES']
-    prior_unindexed = prior['full_output']['ALL']['DB'] - prior['full_output']['ALL']['ES']
-    diff_unindexed = latest_unindexed - prior_unindexed
-    if diff_unindexed == 0 and latest_unindexed != 0:
-        check.status = 'FAIL'
-        check.summary = 'Indexing is not progressing'
-        check.description = ' '.join(['Total number of unindexed items is',
-            str(latest_unindexed), 'and has not changed in the past thirty minutes.',
-            'The indexer may be malfunctioning.'])
-    elif diff_unindexed > 0:
-        check.status = 'PASS'
-        check.summary = 'Indexing load has increased'
-        check.description = ' '.join(['Total number of unindexed items has increased by',
-            str(diff_unindexed), 'in the past thirty minutes. Remaining items to index:',
-            str(latest_unindexed)])
-    else:
-        check.status = 'PASS'
-        check.summary = 'Indexing seems healthy'
-        check.description = ' '.join(['Indexing seems healthy. There are', str(latest_unindexed),
-        'remaining items to index, a change of', str(diff_unindexed), 'from thirty minutes ago.'])
-    return check
+    # Build the query, add date and lab if available
+    query = wfr_utils.build_exp_type_query(exp_type, kwargs)
+    res = ff_utils.search_metadata(query, key=my_auth)
+    print(len(res))
 
-
-@check_function()
-def indexing_records(connection, **kwargs):
-    check = CheckResult(connection, 'indexing_records')
-    client = es_utils.create_es_client(connection.ff_es, True)
-    namespaced_index = connection.ff_env + 'indexing'
-    # make sure we have the index and items within it
-    if (not client.indices.exists(namespaced_index) or
-        client.count(index=namespaced_index).get('count', 0) < 1):
-        check.summary = check.description = 'No indexing records found'
-        check.status = 'PASS'
+    if not res:
+        check.summary = 'All Good!'
         return check
-
-    res = client.search(index=namespaced_index, doc_type='indexing', sort='uuid:desc', size=1000,
-                        body={'query': {'query_string': {'query': '_exists_:indexing_status'}}})
-    delta_days = datetime.timedelta(days=3)
-    all_records = res.get('hits', {}).get('hits', [])
-    recent_records = []
-    warn_records = []
-    for rec in all_records:
-        if rec['_id'] == 'latest_indexing':
+    # run step 0 on all experiments with more than 2 sets of files
+    # for control sets, run step1c on each experiment and finish
+    # for non-control sets, run step1 on each experiment, check if control is ready, run step2 on set
+    step0_name = 'merge-fastq'
+    step1_name = 'encode-chipseq-aln-chip'
+    step1c_name = 'encode-chipseq-aln-ctl'
+    step2_name = 'encode-chipseq-postaln'
+
+    for a_set in res:
+        set_acc = a_set['accession']
+        all_items, all_uuids = ff_utils.expand_es_metadata([a_set['uuid']], my_auth,
+                                                           store_frame='embedded',
+                                                           add_pc_wfr=True,
+                                                           ignore_field=[  # 'experiment_relation',
+                                                                         'biosample_relation',
+                                                                         'references',
+                                                                         'reference_pubs'])
+        now = datetime.utcnow()
+        print(a_set['accession'], (now-start).seconds, len(all_uuids))
+        if (now-start).seconds > lambda_limit:
+            break
+        # are all files uploaded ?
+        all_uploaded = True
+        for a_file in all_items['file_fastq']:
+            if a_file['status'] in ['uploading', 'upload failed']:
+                all_uploaded = False
+
+        if not all_uploaded:
+            final_status = a_set['accession'] + ' skipped, waiting for file upload'
+            print(final_status)
+            check.brief_output.append(final_status)
+            check.full_output['skipped'].append({a_set['accession']: 'files status uploading'})
             continue
-        time_diff = (datetime.datetime.utcnow() -
-            datetime.datetime.strptime(rec['_id'], "%Y-%m-%dT%H:%M:%S.%f"))
-        if time_diff < delta_days:
-            body = rec['_source']
-            # needed to handle transition to queue. can use 'indexing_started'
-            body['timestamp'] = rec['_id']
-            if body.get('errors') or body.get('indexing_status') != 'finished':
-                warn_records.append(body)
-            recent_records.append(body)
-    del all_records
-    # sort so most recent records are first
-    sort_records = sorted(recent_records, key=lambda rec: datetime.datetime.strptime(rec['timestamp'], "%Y-%m-%dT%H:%M:%S.%f"), reverse=True)
-    check.full_output = sort_records
-    if warn_records:
-        sort_warn_records = sorted(warn_records, key=lambda rec: datetime.datetime.strptime(rec['timestamp'], "%Y-%m-%dT%H:%M:%S.%f"), reverse=True)
-        check.summary = check.description = 'Indexing runs in the past three days may require attention'
-        check.status = 'WARN'
-        check.brief_output = sort_warn_records
-    else:
-        check.summary = check.description = 'Indexing runs from the past three days seem normal'
-        check.status = 'PASS'
-    return check
-
-
-# this is a dummy check that is not run but instead updated with put API
-# do_not_store parameter ensures running this check normally won't add to s3
-@check_function(do_not_store=True)
-def staging_deployment(connection, **kwargs):
-    check = CheckResult(connection, 'staging_deployment')
-    return check
-
 
-#@check_function()
-def fourfront_performance_metrics(connection, **kwargs):
-    check = CheckResult(connection, 'fourfront_performance_metrics')
-    full_output = {}  # contains ff_env, env_health, deploy_version, num instances, and performance
-    performance = {}  # keyed by check_url
-    # get information from elastic_beanstalk_health
-    eb_check = CheckResult(connection, 'elastic_beanstalk_health')
-    eb_info = eb_check.get_primary_result()['full_output']
-    full_output['ff_env'] = connection.ff_env
-    full_output['env_health'] = eb_info.get('health_status', 'Unknown')
-    # get deploy version from the first instance
-    full_output['deploy_version'] = eb_info.get('instance_health', [{}])[0].get('deploy_version', 'Unknown')
-    full_output['num_instances'] = len(eb_info.get('instance_health', []))
-    check_urls = [
-        'counts',
-        'joint-analysis-plans',
-        'bar_plot_aggregations/type=ExperimentSetReplicate&experimentset_type=replicate/?field=experiments_in_set.experiment_type',
-        'browse/?type=ExperimentSetReplicate&experimentset_type=replicate',
-        'experiment-set-replicates/4DNESIE5R9HS/',
-        'experiment-set-replicates/4DNESIE5R9HS/?datastore=database',
-        'experiment-set-replicates/4DNESQWI9K2F/',
-        'experiment-set-replicates/4DNESQWI9K2F/?datastore=database',
-        'workflow-runs-awsem/ba50d240-5312-4aa7-b600-6b18d8230311/',
-        'workflow-runs-awsem/ba50d240-5312-4aa7-b600-6b18d8230311/?datastore=database',
-        'files-fastq/4DNFIX75FSJM/',
-        'files-fastq/4DNFIX75FSJM/?datastore=database'
-    ]
-    for check_url in check_urls:
-        performance[check_url] = {}
-        try:
-            # set timeout really high
-            ff_resp = ff_utils.authorized_request(connection.ff_server + check_url,
-                                                  auth=connection.ff_keys, timeout=1000)
-        except Exception as e:
-            performance[check_url]['error'] = str(e)
-        if ff_resp and hasattr(ff_resp, 'headers') and 'X-stats' in ff_resp.headers:
-            x_stats = ff_resp.headers['X-stats']
-            if not isinstance(x_stats, str):
-                performance[check_url]['error'] = 'Stats response is not a string.'
+        all_wfrs = all_items.get('workflow_run_awsem', []) + all_items.get('workflow_run_sbg', [])
+        all_files = [i for typ in all_items for i in all_items[typ] if typ.startswith('file_')]
+        all_qcs = [i for typ in all_items for i in all_items[typ] if typ.startswith('quality_metric')]
+        library = {'wfrs': all_wfrs, 'files': all_files, 'qcs': all_qcs}
+        keep = {'missing_run': [], 'running': [], 'problematic_run': []}
+        # if all completed, patch this info
+        complete = {'patch_opf': [],
+                    'add_tag': []}
+        set_acc = a_set['accession']
+
+        # some feature to extract from each set
+        control = ""  # True or False (True if set is control)
+        control_set = ""  # None if there are no control experiments or if the set is control
+        target_type = ""  # Histone or TF (or None for control)
+        paired = ""  # single or paired , checked for each experiment
+        organism = ""
+        replicate_exps = a_set['replicate_exps']
+        replicate_exps = sorted(replicate_exps, key=lambda x: [x['bio_rep_no'], x['tec_rep_no']])
+        # get organism, target and control from the first replicate
+        f_exp = replicate_exps[0]['replicate_exp']['uuid']
+        # have to do another get for control experiments if there is one
+        f_exp_resp = [i for i in all_items['experiment_seq'] if i['uuid'] == f_exp][0]
+        control, control_set, target_type, organism = wfr_utils.get_chip_info(f_exp_resp, all_items)
+        print('ORG:', organism, "CONT:", control, "TARGET:", target_type, "CONT_SET:", control_set)
+        set_summary = " - ".join([set_acc, str(organism), str(target_type), str(control)])
+        # sanity checks
+        # if control and also has an AB with target
+        if control and target_type:
+            set_summary += "| error - has target and is control"
+            check.brief_output.append(set_summary)
+            check.full_output['skipped'].append({set_acc: set_summary})
+            continue
+        # can only process mouse and human at the moment
+        if organism not in ['mouse', 'human']:
+            set_summary += "| organism not ready for chip"
+            check.brief_output.append(set_summary)
+            check.full_output['skipped'].append({set_acc: set_summary})
+            continue
+        # if not control, we need a target
+        if not control and not target_type:
+            set_summary += "| missing target type"
+            check.brief_output.append(set_summary)
+            check.full_output['skipped'].append({set_acc: set_summary})
+            continue
+        # collect results from step1 runs for step2
+        ta = []
+        taxcor = []
+        ta_cnt = []
+        # track if all experiments completed step0 and step1
+        ready_for_step2 = True
+        for an_exp in replicate_exps:
+            # track if all experiments completed step0
+            ready_for_step1 = True
+            # track if all control experiments are completed processing
+            control_ready = True
+            exp_id = an_exp['replicate_exp']['accession']
+            exp_resp = [i for i in all_items['experiment_seq'] if i['accession'] == exp_id][0]
+            exp_files, paired = wfr_utils.get_chip_files(exp_resp, all_files)
+            # if there are more then 2 files, we need to merge:
+            print(exp_id, len(exp_files), paired)
+            # if too many input, merge them
+            if len(exp_files) > 2:
+                # exp_files format [[pair1,pair2], [pair1, pair2]]  @id
+                input_list = []
+                if paired == 'paired':
+                    # first add paired end 1s
+                    input_list.append([i[0] for i in exp_files])
+                    input_list.append([i[1] for i in exp_files])
+                elif paired == 'single':
+                    input_list.append([i[0] for i in exp_files])
+                # collect files for step1 and step1c
+                merged_files = []
+                step0_status = 'complete'
+                merge_enum = 0
+                # if paired, need to run merge twice for each end
+                for merge_case in input_list:
+                    merge_enum += 1
+                    # RUN STEP 0
+                    s0_input_files = {'input_fastqs': merge_case}
+                    s0_tag = exp_id + '_p' + str(merge_enum)
+                    keep, step0_status, step0_output = wfr_utils.stepper(library, keep,
+                                                                         'step0', s0_tag, merge_case,
+                                                                         s0_input_files, step0_name, 'merged_fastq', organism=organism)
+                    if step0_status == 'complete':
+                        merged_files.append(step0_output)
+                    else:
+                        ready_for_step1 = False
+
+                if ready_for_step1:
+                    # rewrite exp_files with merged ones
+                    exp_files = [[]]
+                    for a_merged in merged_files:
+                        exp_files[0].append(a_merged)
+            # if step0 was not complete, skip checks for step2
+            if not ready_for_step1:
+                ready_for_step2 = False
                 continue
-            # X-stats in form: 'db_count=148&db_time=1215810&es_count=4& ... '
-            split_stats = x_stats.strip().split('&')
-            parse_stats = [stat.split('=') for stat in split_stats]
-            # stats can be strings or integers
-            for stat in parse_stats:
-                if not len(stat) == 2:
-                    continue
-                try:
-                    performance[check_url][stat[0]] = int(stat[1])
-                except ValueError:
-                    performance[check_url][stat[0]] = stat[1]
-            performance[check_url]['error'] = ''
-    check.status = 'PASS'
-    full_output['performance'] = performance
-    check.full_output = full_output
-    return check
-
 
-#@check_function(time_limit=480)
-def secondary_queue_deduplication(connection, **kwargs):
-    check = CheckResult(connection, 'secondary_queue_deduplication')
-    # maybe handle this in check_setup.json
-    if Stage.is_stage_prod() is False:
-        check.full_output = 'Will not run on dev foursight.'
-        check.status = 'PASS'
-        return check
+            # step1 references:
+            input_files = {}
+            if organism == 'human':
+                org = 'hs'
+                input_files['chip.bwa_idx_tar'] = '/files-reference/4DNFIZQB369V/'
+                input_files['chip.blacklist'] = '/files-reference/4DNFIZ1TGJZR/'
+                input_files['chip.chrsz'] = '/files-reference/4DNFIZJB62D1/'
+                input_files['additional_file_parameters'] = {"chip.bwa_idx_tar": {"rename": "GRCh38_no_alt_analysis_set_GCA_000001405.15.fasta.tar"}}
+            if organism == 'mouse':
+                org = 'mm'
+                input_files['chip.bwa_idx_tar'] = '/files-reference/4DNFIZ2PWCC2/'
+                input_files['chip.blacklist'] = '/files-reference/4DNFIZ3FBPK8/'
+                input_files['chip.chrsz'] = '/files-reference/4DNFIBP173GC/'
+                input_files['additional_file_parameters'] = {"chip.bwa_idx_tar": {"rename": "mm10_no_alt_analysis_set_ENCODE.fasta.tar"}}
+            # step1 Parameters
+            parameters = {}
+            parameters["chip.gensz"] = org
+            if paired == 'single':
+                frag_temp = [300]
+                fraglist = frag_temp * len(exp_files)
+                parameters['chip.fraglen'] = fraglist
+                parameters['chip.paired_end'] = False
+            elif paired == 'paired':
+                parameters['chip.paired_end'] = True
+
+            # run step1 for control
+            if control:
+                # control run on tf mode
+                # input_files = {'chip.ctl_fastqs': [exp_files]}
+                input_files['chip.ctl_fastqs'] = [exp_files]
+                control_parameters = {
+                    "chip.pipeline_type": 'tf',
+                    "chip.choose_ctl.always_use_pooled_ctl": True,
+                    "chip.bam2ta_ctl.regex_grep_v_ta": "chr[MUE]|random|alt",
+                    "chip.bwa_ctl.cpu": 8,
+                    "chip.merge_fastq_ctl.cpu": 8,
+                    "chip.filter_ctl.cpu": 8,
+                    "chip.bam2ta_ctl.cpu": 8,
+                    "chip.align_only": True
+                }
+                parameters.update(control_parameters)
 
-    client = boto3.client('sqs')
-    sqs_res = client.get_queue_url(
-        QueueName=connection.ff_env + '-secondary-indexer-queue'
-    )
-    queue_url = sqs_res['QueueUrl']
-    # get approx number of messages
-    attrs = client.get_queue_attributes(
-        QueueUrl=queue_url,
-        AttributeNames=['ApproximateNumberOfMessages']
-    )
-    visible = attrs.get('Attributes', {}).get('ApproximateNumberOfMessages', '0')
-    starting_count = int(visible)
-    time_limit = kwargs['time_limit']
-    t0 = time.time()
-    sent = 0
-    deleted = 0
-    deduplicated = 0
-    total_msgs = 0
-    replaced = 0
-    repeat_replaced = 0
-    problem_msgs = []
-    elapsed = round(time.time() - t0, 2)
-    failed = []
-    seen_uuids = set()
-    # this is a bit of a hack -- send maximum sid with every message we replace
-    # get the maximum sid at the start of deduplication and update it if we
-    # encounter a higher sid
-    max_sid_resp = ff_utils.authorized_request(connection.ff_server + 'max-sid',
-                                               auth=connection.ff_keys).json()
-    if max_sid_resp['status'] != 'success':
-        check.status = 'FAIL'
-        check.summary = 'Could not retrieve max_sid from the server'
-        return check
-    max_sid = max_sid_resp['max_sid']
+                s1c_input_files = input_files
+                s1c_tag = exp_id
+                keep, step1c_status, step1c_output = wfr_utils.stepper(library, keep,
+                                                                       'step1c', s1c_tag, exp_files,
+                                                                       s1c_input_files, step1c_name, 'chip.first_ta_ctl',
+                                                                       additional_input={'parameters': parameters}, organism=organism)
+                if step1c_status == 'complete':
+                    # accumulate files to patch on experiment
+                    patch_data = [step1c_output, ]
+                    complete['patch_opf'].append([exp_id, patch_data])
+                else:
+                    # don't patch anything if at least one exp is still missing
+                    ready_for_step2 = False
+                print('step1c')
+                print(step1c_status, step1c_output)
 
-    exit_reason = 'out of time'
-    dedup_msg = 'FS dedup uuid: %s' % kwargs['uuid']
-    while elapsed < time_limit:
-        # end if we are spinning our wheels replacing the same uuids
-        if (replaced + repeat_replaced) >= starting_count:
-            exit_reason = 'starting uuids fully covered'
-            break
-        send_uuids = set()
-        to_send = []
-        to_delete = []
-        recieved = client.receive_message(
-            QueueUrl=queue_url,
-            MaxNumberOfMessages=10,  # batch size for all sqs ops
-            WaitTimeSeconds=1  # 1 second of long polling
-        )
-        batch = recieved.get("Messages", [])
-        if not batch:
-            exit_reason = 'no messages left'
-            break
-        for msg in batch:
-            try:
-                msg_body = json.loads(msg['Body'])
-            except json.JSONDecodeError:
-                problem_msgs.append(msg['Body'])
-                continue
-            total_msgs += 1
-            msg_uuid = msg_body['uuid']
-            # update max_sid with message sid if applicable
-            if msg_body.get('sid') is not None and msg_body['sid'] > max_sid:
-                max_sid = msg_body['sid']
-            msg_body['sid'] = max_sid
-            to_process = {
-                'Id': msg['MessageId'],
-                'ReceiptHandle': msg['ReceiptHandle']
-            }
-            # every item gets deleted; original uuids get re-sent
-            to_delete.append(to_process)
-            if msg_uuid in seen_uuids and msg_body.get('fs_detail', '') != dedup_msg:
-                deduplicated += 1
+            # run step1
             else:
-                # don't increment replaced count if we've seen the item before
-                if msg_uuid not in seen_uuids:
-                    replaced += 1
-                else:
-                    repeat_replaced += 1
-                time.sleep(0.0001)  # slight sleep for time-based Id
-                # add foursight uuid stamp
-                msg_body['fs_detail'] = dedup_msg
-                # add a slight delay to recycled messages, so that they are
-                # not available for consumption for 2 seconds
-                send_info = {
-                    'Id': str(int(time.time() * 1000000)),
-                    'MessageBody': json.dumps(msg_body),
-                    'DelaySeconds': 2
+                # input_files = {'chip.fastqs': [exp_files]}
+                input_files['chip.fastqs'] = [exp_files]
+                exp_parameters = {
+                    "chip.pipeline_type": target_type,
+                    "chip.choose_ctl.always_use_pooled_ctl": True,
+                    "chip.bam2ta.regex_grep_v_ta": "chr[MUE]|random|alt",
+                    "chip.bwa.cpu": 8,
+                    "chip.merge_fastq.cpu": 8,
+                    "chip.filter.cpu": 8,
+                    "chip.bam2ta.cpu": 8,
+                    "chip.xcor.cpu": 8,
+                    "chip.align_only": True
                 }
-                to_send.append(send_info)
-                seen_uuids.add(msg_uuid)
-                send_uuids.add(msg_uuid)
-        if to_send:
-            res = client.send_message_batch(
-                QueueUrl=queue_url,
-                Entries=to_send
-            )
-            # undo deduplication if errors are detected
-            res_failed = res.get('Failed', [])
-            failed.extend(res_failed)
-            if res_failed:
-                # handle conservatively on error and don't delete
-                for uuid in send_uuids:
-                    if uuid in seen_uuids:
-                        seen_uuids.remove(uuid)
-                        replaced -= 1
-                continue
-            sent += len(to_send)
-        if to_delete:
-            res = client.delete_message_batch(
-                QueueUrl=queue_url,
-                Entries=to_delete
-            )
-            failed.extend(res.get('Failed', []))
-            deleted += len(to_delete)
-        elapsed = round(time.time() - t0, 2)
-
-    check.full_output = {
-        'total_messages_covered': total_msgs,
-        'uuids_covered': len(seen_uuids),
-        'deduplicated': deduplicated,
-        'replaced': replaced,
-        'repeat_replaced': repeat_replaced,
-        'time': elapsed,
-        'problem_messages': problem_msgs,
-        'exit_reason': exit_reason
-    }
-    # these are some standard things about the result that should always be true
-    if replaced != len(seen_uuids) or (deduplicated + replaced + repeat_replaced) != total_msgs:
-        check.status = 'FAIL'
-        check.summary = 'Message totals do not add up. Report to Carl'
-    if failed:
-        if check.status != 'FAIL':
-            check.status = 'WARN'
-            check.summary = 'Queue deduplication encountered an error'
-        check.full_output['failed'] = failed
-    else:
-        check.status = 'PASS'
-        check.summary = 'Removed %s duplicates from %s secondary queue' % (deduplicated, connection.ff_env)
-    check.description = 'Items on %s secondary queue were deduplicated. Started with approximately %s items; replaced %s items and removed %s duplicates. Covered %s unique uuids. Took %s seconds.' % (connection.ff_env, starting_count, replaced, deduplicated, len(seen_uuids), elapsed)
-
-    return check
-
-
-# @check_function()
-def clean_up_travis_queues(connection, **kwargs):
-    """
-    Clean up old sqs queues based on the name ("travis-job")
-    and the creation date. Only run on data for now
-    """
-    check = CheckResult(connection, 'clean_up_travis_queues')
-    check.status = 'PASS'
-    if connection.fs_env != 'data' or Stage.is_stage_prod() is False:
-        check.summary = check.description = 'This check only runs on the data environment for Foursight prod'
-        return check
-    sqs_client = boto3.client('sqs')
-    sqs = boto3.resource('sqs')
-    queues = sqs.queues.all()
-    num_deleted = 0
-    for queue in queues:
-        if 'travis-job' in queue.url:
-            try:
-                creation = queue.attributes['CreatedTimestamp']
-            except sqs_client.exceptions.QueueDoesNotExist:
-                continue
-            if isinstance(creation, str):
-                creation = float(creation)
-            dt_creation = datetime.datetime.utcfromtimestamp(creation)
-            queue_age = datetime.datetime.utcnow() - dt_creation
-            # delete queues 3 days old or older
-            if queue_age > datetime.timedelta(days=3):
-                queue.delete()
-                num_deleted += 1
-    check.summary = 'Cleaned up %s old indexing queues' % num_deleted
-    check.description = 'Cleaned up all indexing queues from Travis that are 3 days old or older. %s queues deleted.' % num_deleted
-    return check
+                parameters.update(exp_parameters)
 
+                s1_input_files = input_files
+                s1_tag = exp_id
+                # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
+                keep, step1_status, step1_output = wfr_utils.stepper(library, keep,
+                                                                     'step1', s1_tag, exp_files,
+                                                                     s1_input_files, step1_name, ['chip.first_ta', 'chip.first_ta_xcor'],
+                                                                     additional_input={'parameters': parameters}, organism=organism)
+                if step1_status == 'complete':
+                    exp_ta_file = step1_output[0]
+                    exp_taxcor_file = step1_output[1]
+                    # accumulate files to patch on experiment
+                    patch_data = [exp_ta_file, ]
+                    complete['patch_opf'].append([exp_id, patch_data])
+                    ta.append(exp_ta_file)
+                    taxcor.append(exp_taxcor_file)
+
+                    # find the control file if there is a control set found
+                    if control_set:
+                        try:
+                            exp_cnt_ids = [i['experiment'] for i in exp_resp['experiment_relation'] if i['relationship_type'] == 'controlled by']
+                            exp_cnt_ids = [i['@id'] for i in exp_cnt_ids]
+                        except:
+                            control_ready = False
+                            print('Control Relation has problems for this exp', exp_id)
+                            continue
+                        if len(exp_cnt_ids) != 1:
+                            control_ready = False
+                            print('Multiple controls for this exp', exp_id)
+                            continue
+                        exp_cnt_id = exp_cnt_ids[0]
+                        print('controled by set', exp_cnt_id)
+                        # have to do a get for the control experiment
+                        exp_cnt_resp = [i for i in all_items['experiment_seq'] if i['@id'] == exp_cnt_id][0]
+                        cont_file = ''
+                        # check opf for control file
+                        for opf_case in exp_cnt_resp.get('other_processed_files', []):
+                            if opf_case['title'] == 'ENCODE ChIP-Seq Pipeline - Preliminary Files':
+                                opf_files = opf_case['files']
+                                assert len(opf_files) == 1
+                                cont_file = opf_files[0]['@id']
+                        # if not in opf, check processed files
+                        if not cont_file:
+                            pf_list = exp_cnt_resp.get('processed_files', [])
+                            if pf_list:
+                                if pf_list:
+                                    assert len(pf_list) == 1
+                                    cont_file = pf_list[0]['@id']
+                        # did we find it, if so, add it to ta_cnt
+                        if cont_file:
+                            ta_cnt.append(cont_file)
+                        else:
+                            control_ready = False
 
-# @check_function()
-# def manage_old_filebeat_logs(connection, **kwargs):
-#     # import curator
-#     check = CheckResult(connection, 'manage_old_filebeat_logs')
-#
-#     # temporary -- disable this check
-#     check.status = 'PASS'
-#     check.description = 'Not currently running this check'
-#     return check
-
-    # check.status = "WARNING"
-    # check.description = "not able to get data from ES"
-    #
-    # # configure this thing
-    # start_backup = 14
-    # trim_backup = 30
-    # timestring = '%Y.%m.%d'
-    #
-    # log_index = 'filebeat-'
-    # #TODO: this probably needs to change when namespacing is implemented
-    # snapshot = 'backup-%s-' % connection.ff_env
-    # today = datetime.datetime.today().strftime(timestring)
-    #
-    # # run the check
-    # client = es_utils.create_es_client(connection.ff_es, True)
-    # # store backups in foursight s3, cause I know we have access to this..
-    # # maybe this should change?
-    # es_utils.create_snapshot_repo(client, snapshot[:-1], 'foursight-runs')
-    #
-    # # amazon es auto backups first 14 days, so we only need backup after that
-    # ilo = es_utils.get_index_list(client, log_index, start_backup, timestring)
-    #
-    # if len(ilo.indices) > 0:
-    #     try:
-    #         new_snapshot = curator.Snapshot(ilo, repository=snapshot[:-1], name='%s%s' % (snapshot, today))
-    #         new_snapshot.do_action()
-    #         check.full_output = "Snapshot taken for %s indices" % len(ilo.indices)
-    #     except curator.exceptions.FailedExecution as e:
-    #         # snapshot already exists
-    #         if "Invalid snapshot name" in str(e):
-    #             check.full_output = "Snapshot already exists with same name for %s indices, so skipping." % len(ilo.indices)
-    #         else:
-    #             raise(e)
-    #
-    # # now trim further to only be indexes 30-days or older and delete
-    # ilo = es_utils.get_index_list(client, log_index, trim_backup, timestring, ilo=ilo)
-    #
-    # if len(ilo.indices) > 0:
-    #     cleanupIndices = curator.DeleteIndices(ilo)
-    #     cleanupIndices.do_action()
-    #     check.full_output += " Cleaned up %s old indices" % len(ilo.indices)
-    #
-    # check.status = "PASS"
-    # check.description = 'Performed auto-backup to repository %s' % snapshot[:-1]
-    # return check
-
-
-@check_function()
-def snapshot_rds(connection, **kwargs):
-    check = CheckResult(connection, 'snapshot_rds')
-    if Stage.is_stage_prod() is False:
-        check.summary = check.description = 'This check only runs on Foursight prod'
-        return check
-    rds_name = 'fourfront-production' if (env_utils.is_fourfront_env(connection.ff_env) and env_utils.is_stg_or_prd_env(connection.ff_env)) else connection.ff_env
-    # snapshot ID can only have letters, numbers, and hyphens
-    snap_time = datetime.datetime.strptime(kwargs['uuid'], "%Y-%m-%dT%H:%M:%S.%f").strftime("%Y-%m-%dT%H-%M-%S")
-    snapshot_name = 'foursight-snapshot-%s-%s' % (rds_name, snap_time)
-    client = boto3.client('rds', region_name=beanstalk_utils.REGION)
-    res = client.create_db_snapshot(
-             DBSnapshotIdentifier=snapshot_name,
-             DBInstanceIdentifier=rds_name
-    )
-    if not res.get('DBSnapshot'):
-        check.status = 'FAIL'
-        check.summary = check.description = 'Something went wrong during snapshot creation'
-        check.full_output = res
-    else:
-        check.status = 'PASS'
-        # there is a datetime in the response that must be str formatted
-        res['DBSnapshot']['InstanceCreateTime'] = str(res['DBSnapshot']['InstanceCreateTime'])
-        check.full_output = res
-        check.summary = 'Snapshot successfully created'
-        check.description = 'Snapshot succesfully created with name: %s' % snapshot_name
-    return check
-
-
-# @check_function()
-def process_download_tracking_items(connection, **kwargs):
-    """
-    Do a few things here, and be mindful of the 5min lambda limit.
-    - Consolidate tracking items with download_tracking.range_query=True
-    - Change remote_ip to geo_country and geo_city
-    - If the user_agent looks to be a bot, set status=deleted
-    - Change unused range query items to status=deleted
-    """
-    check = CheckResult(connection, 'process_download_tracking_items')
-    # maybe handle this in check_setup.json
-    if Stage.is_stage_prod() is False:
-        check.full_output = 'Will not run on dev foursight.'
-        check.status = 'PASS'
-        return check
-    # hold warning messages
-    check.brief_output = {'cannot_parse_date_created': []}
-    range_cache = {}
-    # duration we want to consolidate range queries over
-    # search older entries since range_consolidation_hrs * 2 to avoid duplication
-    range_consolidation_hrs = 1
-    cons_date = (datetime.datetime.utcnow() -
-                 datetime.timedelta(hours=range_consolidation_hrs * 2)).strftime('%Y-%m-%dT%H\:%M')
-    range_search_query = ''.join(['search/?type=TrackingItem&tracking_type=download_tracking',
-                                  '&download_tracking.range_query=true&sort=-date_created',
-                                  '&status=released&q=last_modified.date_modified:>=', cons_date])
-    cons_query = ff_utils.search_metadata(range_search_query, key=connection.ff_keys)
-    for tracking in cons_query:
-        dl_info = tracking['download_tracking']
-        user_agent = dl_info.get('user_agent', 'unknown_user_agent').lower()
-        range_key = '//'.join([dl_info['remote_ip'], dl_info['filename'],
-                               user_agent, dl_info['user_uuid']])
-        parsed_date = parse_datetime_to_utc(tracking['date_created'])
-        # check for date parsing error
-        if parsed_date is None:
-            continue
-        if range_key in range_cache:
-            range_cache[range_key].append(parsed_date)
-        else:
-            range_cache[range_key] = [parsed_date]
-    del cons_query
-    ip_cache = {}
-    time_limit = 270  # 4.5 minutes
-    # list of strings used to flag user_agent as a bot. By no means complete
-    bot_agents = ['bot', 'crawl', 'slurp', 'spider', 'mediapartners', 'ltx71']
-    # list of user_agents we always consider range_query=True
-    range_query_agents = ['igv', 'java', 'python-requests']
-    t0 = time.time()  # keep track of how start time
-
-    # batch large groups of tracking items at once to save time with geocoder
-    # for now, this function will process only <search_limit> results.
-    # I would love to use a generator, but search results change as items are indexed...
-    search_limit = 1000
-    search_query = ''.join(['search/?type=TrackingItem&tracking_type=download_tracking',
-                            '&download_tracking.geo_country=No+value',
-                            '&status=in+review+by+lab&sort=-date_created&limit=', str(search_limit)])
-    search_page = ff_utils.search_metadata(search_query, key=connection.ff_keys, page_limit=200)
-    counts = {'proc': 0, 'deleted': 0, 'released': 0}
-
-    page_ips = set([tracking['download_tracking']['remote_ip'] for tracking in search_page])
-    # transform all IP addresses into GEO information with a persistent connection
-    with requests.Session() as session:
-        for track_ip in page_ips:
-            if track_ip in ip_cache:
-                continue
-            geo = geocoder.ip(track_ip, session=session)
-            geo_country = getattr(geo, 'country') or 'Unknown'
-            geo_city = getattr(geo, 'city') or 'Unknown'
-            geo_state = getattr(geo, 'state', None)
-            if geo_state:
-                geo_city = ', '.join([geo_city, geo_state])
-            # cache the geo info in an arbitrary form
-            ip_cache[track_ip] = '//'.join([geo_city, geo_country])
-
-    # iterate over the individual tracking items
-    for tracking in search_page:
-        if round(time.time() - t0, 2) > time_limit:
-            break
-        dl_info = tracking['download_tracking']
-        user_agent = dl_info.get('user_agent', 'unknown_user_agent').lower()
-        # remove request_headers, which may contain sensitive information
-        if 'request_headers' in dl_info:
-            del dl_info['request_headers']
-        geo_info = ip_cache[dl_info['remote_ip']]
-        dl_info['geo_city'], dl_info['geo_country'] = geo_info.split('//')
-        patch_body = {'status': 'released', 'download_tracking': dl_info}
-        # delete items from bot user agents
-        if (any(bot_str in user_agent for bot_str in bot_agents)
-            and dl_info['user_uuid'] == 'anonymous'):
-            patch_body['status'] = 'deleted'
-        # set range_query=True for select user agents
-        if (any(ua_str in user_agent for ua_str in range_query_agents)):
-            dl_info['range_query'] = True
-        # deduplicate range query requests by ip/filename/user_agent/user_uuid
-        if patch_body['status'] != 'deleted' and dl_info['range_query'] is True:
-            range_key = '//'.join([dl_info['remote_ip'], dl_info['filename'],
-                                   user_agent, dl_info['user_uuid']])
-            parsed_date = parse_datetime_to_utc(tracking['date_created'])
-            if parsed_date is not None:
-                if range_key in range_cache:
-                    # for all reference range queries with this info, see if this one
-                    # was created within one hour of it. if so, it is redundant and delete
-                    for range_reference in range_cache[range_key]:
-                        compare_date_low = range_reference - datetime.timedelta(hours=range_consolidation_hrs)
-                        compare_date_high = range_reference + datetime.timedelta(hours=range_consolidation_hrs)
-                        if parsed_date > compare_date_low and parsed_date < compare_date_high:
-                            patch_body['status'] = 'deleted'
-                            break
-                    if patch_body['status'] != 'deleted':
-                        range_cache[range_key].append(parsed_date)
                 else:
-                    # set the upper limit for for range queries to consolidate
-                    range_cache[range_key] = [parsed_date]
+                    # don't patch anything if at least one exp is still missing
+                    ready_for_step2 = False
+                print('step1')
+                print(step1_status, step1_output, control_ready)
+        # back to set level
+        final_status = set_acc  # start the reporting with acc
+        all_completed = False
+        # is step0 step1 complete
+        if ready_for_step2 and not control_ready:
+            final_status += ' waiting for control experiments to finish processing'
+        elif ready_for_step2:
+            # for control, add tag to set, and files to experiments
+            if control:
+                complete['add_tag'] = [set_acc, tag]
+            # for non controls check for step2
             else:
-                check.brief_output['cannot_parse_date_created'].append(tracking['uuid'])
-
-        ff_utils.patch_metadata(patch_body, tracking['uuid'], key=connection.ff_keys)
-        counts['proc'] += 1
-        if patch_body['status'] == 'released':
-            counts['released'] += 1
+                # this only works with 2 experiments, if 3, pick best 2, if more, skip for now
+                if len(ta) > 3:
+                    set_summary += "| skipped - more then 3 experiments in set, can not process at the moment"
+                    check.brief_output.append(set_summary)
+                    check.full_output['skipped'].append({set_acc: set_summary})
+                    continue
+                if len(ta) > 2:
+                    ta_2 = []
+                    taxcor_2 = []
+                    print('ExperimentSet has 3 experiments, selecting best 2')
+                    ta_2 = wfr_utils.select_best_2(ta, all_files, all_qcs)
+                    # xcor does not have qc, use ta indexes to find the correct files
+                    for ta_f in ta_2:
+                        taxcor_2.append(taxcor[ta.index(ta_f)])
+                    ta = ta_2
+                    taxcor = taxcor_2
+                    # for control files ,also select best2
+                    ta_cnt = wfr_utils.select_best_2(ta_cnt, all_files, all_qcs)
+
+                # collect step2 input files
+                s2_input_files = {}
+                if organism == 'human':
+                    org = 'hs'
+                    s2_input_files['chip.blacklist'] = '/files-reference/4DNFIZ1TGJZR/'
+                    s2_input_files['chip.chrsz'] = '/files-reference/4DNFIZJB62D1/'
+                if organism == 'mouse':
+                    org = 'mm'
+                    s2_input_files['chip.blacklist'] = '/files-reference/4DNFIZ3FBPK8/'
+                    s2_input_files['chip.chrsz'] = '/files-reference/4DNFIBP173GC/'
+
+                def rename_chip(input_at_id_list):
+                    # rename bed.gz to tagAlign.gz
+                    renamed = []
+                    for a_file in input_at_id_list:
+                        acc = a_file.split('/')[2]
+                        renamed.append(acc + '.tagAlign.gz')
+                    return renamed
+
+                s2_input_files['additional_file_parameters'] = {}
+                s2_input_files['chip.tas'] = ta
+                s2_input_files['additional_file_parameters']['chip.tas'] = {"rename": rename_chip(ta)}
+                s2_input_files['chip.bam2ta_no_filt_R1.ta'] = taxcor
+                s2_input_files['additional_file_parameters']['chip.bam2ta_no_filt_R1.ta'] = {"rename": rename_chip(taxcor)}
+                if ta_cnt:
+                    s2_input_files['chip.ctl_tas'] = ta_cnt
+                    s2_input_files['additional_file_parameters']['chip.ctl_tas'] = {"rename": rename_chip(ta_cnt)}
+
+                # collect parameters
+                parameters = {}
+                if paired == 'single':
+                    chip_p = False
+                elif paired == 'paired':
+                    chip_p = True
+                if not control_set:
+                    if target_type == 'histone':
+                        set_summary += "| skipped - histone without control needs attention, ie change to tf"
+                        check.brief_output.append(set_summary)
+                        check.full_output['skipped'].append({set_acc: set_summary})
+                        continue
+                run_ids = {'desc': set_acc + a_set.get('description', '')}
+                parameters = {
+                    "chip.pipeline_type": target_type,
+                    "chip.paired_end": chip_p,
+                    "chip.choose_ctl.always_use_pooled_ctl": True,
+                    "chip.qc_report.desc": run_ids['desc'],
+                    "chip.gensz": org,
+                    "chip.xcor.cpu": 4,
+                }
+                if paired == 'single':
+                    frag_temp = [300]
+                    fraglist = frag_temp * len(ta)
+                    parameters['chip.fraglen'] = fraglist
+
+                # if the target is a tf and there is no control, use macs2
+                if not control_set:
+                    if target_type == 'tf':
+                        parameters['chip.peak_caller'] = "macs2"
+
+                s2_tag = set_acc
+                # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
+                keep, step2_status, step2_output = wfr_utils.stepper(library, keep,
+                                                                     'step2', s2_tag, ta,
+                                                                     s2_input_files, step2_name,
+                                                                     ['chip.optimal_peak', 'chip.conservative_peak', 'chip.sig_fc'],
+                                                                     additional_input={'parameters': parameters}, organism=organism)
+                if step2_status == 'complete':
+                    set_opt_peak = step2_output[0]
+                    set_cons_peak = step2_output[1]
+                    set_sig_fc = step2_output[2]
+                    # accumulate files to patch on experiment
+                    patch_data = [set_opt_peak, set_cons_peak, set_sig_fc]
+                    complete['patch_opf'].append([set_acc, patch_data])
+                    complete['add_tag'] = [set_acc, tag]
+                    all_completed = True
+
+        # unpack results
+        missing_run = keep['missing_run']
+        running = keep['running']
+        problematic_run = keep['problematic_run']
+        if all_completed:
+            final_status += ' completed'
         else:
-            counts['deleted'] += 1
-    if any(check.brief_output.values()):
+            if missing_run:
+                final_status += ' |Missing: ' + " ".join([i[0] for i in missing_run])
+            if running:
+                final_status += ' |Running: ' + " ".join([i[0] for i in running])
+            if problematic_run:
+                final_status += ' |Problem: ' + " ".join([i[0] for i in problematic_run])
+
+        # add dictionaries to main ones
+        check.brief_output.append(final_status)
+        print(final_status)
+        if running:
+            check.full_output['running_runs'].append({set_acc: running})
+        if missing_run:
+            check.full_output['needs_runs'].append({set_acc: missing_run})
+        if problematic_run:
+            check.full_output['problematic_runs'].append({set_acc: problematic_run})
+        # if made it till the end
+        if complete.get('add_tag'):
+            assert not running
+            assert not problematic_run
+            assert not missing_run
+            check.full_output['completed_runs'].append(complete)
+
+    # complete check values
+    check.summary = ""
+    if check.full_output['running_runs']:
+        check.summary = str(len(check.full_output['running_runs'])) + ' running|'
+    if check.full_output['skipped']:
+        check.summary += str(len(check.full_output['skipped'])) + ' skipped|'
+        check.status = 'WARN'
+    if check.full_output['needs_runs']:
+        check.summary += str(len(check.full_output['needs_runs'])) + ' missing|'
+        check.status = 'WARN'
+        check.allow_action = True
+    if check.full_output['completed_runs']:
+        check.summary += str(len(check.full_output['completed_runs'])) + ' completed|'
+        check.status = 'WARN'
+        check.allow_action = True
+    if check.full_output['problematic_runs']:
+        check.summary += str(len(check.full_output['problematic_runs'])) + ' problem|'
         check.status = 'WARN'
-    else:
-        check.status = 'PASS'
-    check.summary = 'Successfully processed %s download tracking items' % counts['proc']
-    check.description = '%s. Released %s items and deleted %s items' % (check.summary, counts['released'], counts['deleted'])
     return check
 
 
-# @check_function()
-def purge_download_tracking_items(connection, **kwargs):
-    """
-    This check was originally created to take in any search through kwargs.
-    Changed to hardcode a search for tracking items, but it can easily
-    adapted; as it is, already handles recording for any number of item types.
-    Ensure search includes limit, field=uuid, and status=deleted
-    """
-    check = CheckResult(connection, 'purge_download_tracking_items')
-
-    # Don't run if staging deployment is running
-    # Only need to check if our env is data
-    # XXX: Removing for now as we find the check can never run without this
-    # if the staging deploy takes long enough or errors
-    # if connection.fs_env == 'data':
-    #     from ..app_utils import AppUtils
-    #     staging_conn = AppUtils().init_connection('staging')
-    #     staging_deploy = CheckResult(staging_conn, 'staging_deployment').get_primary_result()
-    #     if staging_deploy['status'] != 'PASS':
-    #         check.summary = 'Staging deployment is running - skipping'
-    #         return check
+@action_function(start_runs=True, patch_completed=True)
+def chipseq_start(connection, **kwargs):
+    """Start runs by sending compiled input_json to run_workflow endpoint"""
+    start = datetime.utcnow()
+    action = ActionResult(connection, 'chipseq_start')
+    my_auth = connection.ff_keys
+    my_env = connection.ff_env
+    fs_env = connection.fs_env
+    chipseq_check_result = action.get_associated_check_result(kwargs).get('full_output', {})
+    missing_runs = []
+    patch_meta = []
+    if kwargs.get('start_runs'):
+        missing_runs = chipseq_check_result.get('needs_runs')
+    if kwargs.get('patch_completed'):
+        patch_meta = chipseq_check_result.get('completed_runs')
+    action = wfr_utils.start_tasks(missing_runs, patch_meta, action, my_auth, my_env, fs_env, start,  move_to_pc=True, runtype='chip')
+    return action
 
-    if Stage.is_stage_prod() is False:
-        check.summary = check.description = 'This check only runs on Foursight prod'
-        return check
 
-    time_limit = 270  # 4.5 minutes
-    t0 = time.time()
-    check.full_output = {}  # purged items by item type
-    search = '/search/?type=TrackingItem&tracking_type=download_tracking&status=deleted&field=uuid&limit=300'
-    search_res = ff_utils.search_metadata(search, key=connection.ff_keys)
-    search_uuids = [res['uuid'] for res in search_res]
-    client = es_utils.create_es_client(connection.ff_es, True)
-    # a bit convoluted, but we want the frame=raw, which does not include uuid
-    # use get_es_metadata to handle this. Use it as a generator
-    for to_purge in ff_utils.get_es_metadata(search_uuids, es_client=client, is_generator=True,
-                                             key=connection.ff_keys):
-        if round(time.time() - t0, 2) > time_limit:
-            break
-        purge_properties = to_purge['properties']
-        purge_properties['uuid'] = to_purge['uuid']  # add uuid to frame=raw
-        try:
-            purge_res = ff_utils.purge_metadata(to_purge['uuid'], key=connection.ff_keys)
-        except Exception as exc:
-            purge_status = 'error'
-            purge_detail = str(exc)
-        else:
-            purge_status = purge_res['status']
-            purge_detail = purge_properties if purge_status == 'success' else purge_res
-        purge_record = {'uuid': to_purge['uuid'], 'result': purge_detail}
-        if to_purge['item_type'] not in check.full_output:
-            check.full_output[to_purge['item_type']] = {}
-        if purge_status not in check.full_output[to_purge['item_type']]:
-            check.full_output[to_purge['item_type']][purge_status] = []
-        check.full_output[to_purge['item_type']][purge_status].append(purge_record)
-    purge_out_str = '. '.join(['%s: %s' % (it, len(check.full_output[it]['success']))
-                               for it in check.full_output if check.full_output[it].get('success')])
-    check.description = 'Purged: ' + purge_out_str + '. Search used: %s' % search
-    if any([it for it in check.full_output if check.full_output[it].get('error')]):
-        check.status = 'WARN'
-        check.summary = 'Some items failed to purge. See full output'
-    else:
-        check.status = 'PASS'
-        check.summary = 'Items purged successfully'
-    return check
-
-
-@check_function()
-def check_long_running_ec2s(connection, **kwargs):
+@check_function(lab_title=None, start_date=None, pick_best_2=False, action="atacseq_start")
+def atacseq_status(connection, **kwargs):
     """
-    Flag all ec2s that have been running for longer than 1 week (WARN) or 2 weeks
-    (FAIL) if any contain any strings from `flag_names` in their
-    names, or if they have no name.
+    Keyword arguments:
+    lab_title -- limit search with a lab i.e. Bing+Ren, UCSD
+    start_date -- limit search to files generated since a date formatted YYYY-MM-DD
+    run_time -- assume runs beyond run_time are dead
+    pick_best_2 -- False by default. If set the True, for sets more than 2 experiments,
+                   2 best will be used instead of running mergebed
     """
-    check = CheckResult(connection, 'check_long_running_ec2s')
-    if Stage.is_stage_prod() is False:
-        check.summary = check.description = 'This check only runs on Foursight prod'
+    start = datetime.utcnow()
+    check = CheckResult(connection, 'atacseq_status')
+    my_auth = connection.ff_keys
+    check.action = "atacseq_start"
+    check.description = "run missing steps and add processing results to processed files, match set status"
+    check.brief_output = []
+    check.summary = ""
+    check.full_output = {'skipped': [], 'running_runs': [], 'needs_runs': [],
+                         'completed_runs': [], 'problematic_runs': []}
+    check.status = 'PASS'
+    exp_type = 'ATAC-seq'
+    # completion tag
+    tag = wfr_utils.accepted_versions[exp_type][-1]
+    pick_best_2 = kwargs.get('pick_best_2', False)
+    # check indexing queue
+    check, skip = wfr_utils.check_indexing(check, connection)
+    if skip:
         return check
+    # Build the query, add date and lab if available
+    query = wfr_utils.build_exp_type_query(exp_type, kwargs)
+    res = ff_utils.search_metadata(query, key=my_auth)
+    print(len(res))
 
-    client = boto3.client('ec2')
-    # flag instances that contain any of flag_names and have been running
-    # longer than warn_time
-    flag_names = ['awsem']
-    warn_time = (datetime.datetime.now(datetime.timezone.utc) -
-                 datetime.timedelta(days=7))
-    fail_time = (datetime.datetime.now(datetime.timezone.utc) -
-                 datetime.timedelta(days=14))
-    ec2_res = client.describe_instances(
-        Filters=[{'Name': 'instance-state-name', 'Values': ['running']}]
-    )
-    check.full_output = []
-    check.brief_output = {'one_week': [], 'two_weeks': []}
-    for ec2_info in ec2_res.get('Reservations', []):
-        instances = ec2_info.get('Instances', [])
-        if not instances:
+    if not res:
+        check.summary = 'All Good!'
+        return check
+    # run step 0 on all experiments with more than 2 sets of files
+    # step1 on each experiment,if multiple exps, merge beds, run step3 on set
+    step0_name = 'merge-fastq'
+    step1_name = 'encode-atacseq-aln'
+    step2_name = 'mergebed'
+    step3_name = 'encode-atacseq-postaln'
+
+    for a_set in res:
+        set_acc = a_set['accession']
+        all_items, all_uuids = ff_utils.expand_es_metadata([a_set['uuid']], my_auth,
+                                                           store_frame='embedded',
+                                                           add_pc_wfr=True,
+                                                           ignore_field=['experiment_relation',
+                                                                         'biosample_relation',
+                                                                         'references',
+                                                                         'reference_pubs'])
+        now = datetime.utcnow()
+        print(a_set['accession'], (now-start).seconds, len(all_uuids))
+        if (now-start).seconds > lambda_limit:
+            break
+        # are all files uploaded ?
+        all_uploaded = True
+        for a_file in all_items['file_fastq']:
+            if a_file['status'] in ['uploading', 'upload failed']:
+                all_uploaded = False
+        if not all_uploaded:
+            final_status = a_set['accession'] + ' skipped, waiting for file upload'
+            print(final_status)
+            check.brief_output.append(final_status)
+            check.full_output['skipped'].append({a_set['accession']: 'files status uploading'})
+            continue
+        all_wfrs = all_items.get('workflow_run_awsem', []) + all_items.get('workflow_run_sbg', [])
+        all_files = [i for typ in all_items for i in all_items[typ] if typ.startswith('file_')]
+        all_qcs = [i for typ in all_items for i in all_items[typ] if typ.startswith('quality_metric')]
+        library = {'wfrs': all_wfrs, 'files': all_files, 'qcs': all_qcs}
+        keep = {'missing_run': [], 'running': [], 'problematic_run': []}
+        # if all completed, patch this info
+        complete = {'patch_opf': [],
+                    'add_tag': []}
+        set_acc = a_set['accession']
+
+        # some feature to extract from each set
+        paired = ""  # single or paired , checked for each experiment
+        organism = ""
+        replicate_exps = a_set['replicate_exps']
+        replicate_exps = sorted(replicate_exps, key=lambda x: [x['bio_rep_no'], x['tec_rep_no']])
+        # get organism
+        f_exp = replicate_exps[0]['replicate_exp']['uuid']
+        # have to do another get for control experiments if there is one
+        f_exp_resp = [i for i in all_items['experiment_atacseq'] if i['uuid'] == f_exp][0]
+        biosample = f_exp_resp['biosample']
+        organism = list(set([bs['organism']['name'] for bs in biosample['biosource']]))[0]
+        set_summary = " - ".join([set_acc, str(organism)])
+        print(set_summary)
+        # sanity checks
+        # can only process mouse and human at the moment
+        if organism not in ['mouse', 'human']:
+            set_summary += "| organism not ready for atac"
+            check.brief_output.append(set_summary)
+            check.full_output['skipped'].append({set_acc: set_summary})
             continue
-        # for multiple instance (?) just check if any of them require warnings
-        for ec2_inst in instances:
-            state = ec2_inst.get('State')
-            created = ec2_inst.get('LaunchTime')
-            if not state or not created:
+
+        # collect results from step1 runs for step2
+        ta = []
+        # track if all experiments completed step0 and step1
+        ready_for_step2 = True
+        for an_exp in replicate_exps:
+            # track if all experiments completed step0
+            ready_for_step1 = True
+            exp_id = an_exp['replicate_exp']['accession']
+            exp_resp = [i for i in all_items['experiment_atacseq'] if i['accession'] == exp_id][0]
+            # exp_files [[pair1,pair2], [pair1, pair2]]
+            exp_files, paired = wfr_utils.get_chip_files(exp_resp, all_files)
+            # if there are more then 2 files, we need to merge:
+            print(exp_id, len(exp_files), paired)
+            # if too many input, merge them
+            if len(exp_files) > 2:
+                # exp_files format [[pair1,pair2], [pair1, pair2]]  @id
+                input_list = []
+                if paired == 'paired':
+                    # first add paired end 1s
+                    input_list.append([i[0] for i in exp_files])
+                    input_list.append([i[1] for i in exp_files])
+                elif paired == 'single':
+                    input_list.append([i[0] for i in exp_files])
+                # collect files for step1 and step1c
+                merged_files = []
+                step0_status = 'complete'
+                merge_enum = 0
+                # if paired, need to run merge twice for each end
+                for merge_case in input_list:
+                    merge_enum += 1
+                    # RUN STEP 0
+                    s0_input_files = {'input_fastqs': merge_case}
+                    s0_tag = exp_id + '_p' + str(merge_enum)
+                    keep, step0_status, step0_output = wfr_utils.stepper(library, keep,
+                                                                         'step0', s0_tag, merge_case,
+                                                                         s0_input_files, step0_name, 'merged_fastq')
+                    if step0_status == 'complete':
+                        merged_files.append(step0_output)
+                    else:
+                        ready_for_step1 = False
+
+                if ready_for_step1:
+                    # rewrite exp_files with merged ones
+                    exp_files = [[]]
+                    for a_merged in merged_files:
+                        exp_files[0].append(a_merged)
+            # if step0 was not complete, skip checks for step2
+            if not ready_for_step1:
+                ready_for_step2 = False
                 continue
-            inst_name = [kv['Value'] for kv in ec2_inst.get('Tags', [])
-                         if kv['Key'] == 'Name']
-            other_tags = {kv['Key']: kv['Value'] for kv in ec2_inst.get('Tags', [])
-                         if kv['Key'] != 'Name'}
-            ec2_log = {
-                'state': state['Name'], 'name': inst_name,
-                'id': ec2_inst.get('InstanceId'),
-                'type': ec2_inst.get('InstanceType'),
-                'date_created_utc': created.strftime('%Y-%m-%dT%H:%M')
+
+            # step1 files
+            # references
+            input_files = {}
+            if organism == 'human':
+                org = 'hs'
+                input_files['atac.bowtie2_idx_tar'] = '/files-reference/4DNFIMQPTYDY/'
+                input_files['atac.blacklist'] = '/files-reference/4DNFIZ1TGJZR/'
+                input_files['atac.chrsz'] = '/files-reference/4DNFIZJB62D1/'
+                input_files['additional_file_parameters'] = {"atac.bowtie2_idx_tar": {"rename": "GRCh38_no_alt_analysis_set_GCA_000001405.15.fasta.tar"}}
+            if organism == 'mouse':
+                org = 'mm'
+                input_files['atac.bowtie2_idx_tar'] = '/files-reference/4DNFI2493SDN/'
+                input_files['atac.blacklist'] = '/files-reference/4DNFIZ3FBPK8/'
+                input_files['atac.chrsz'] = '/files-reference/4DNFIBP173GC/'
+                input_files['additional_file_parameters'] = {"atac.bowtie2_idx_tar": {"rename": "mm10_no_alt_analysis_set_ENCODE.fasta.tar"}}
+            # add input files
+            input_files['atac.fastqs'] = [exp_files]
+            # step1 Parameters
+            parameters = {
+                "atac.pipeline_type": 'atac',
+                "atac.gensz": org,
+                "atac.bam2ta.regex_grep_v_ta": "chr[MUE]|random|alt",
+                "atac.disable_ataqc": True,
+                "atac.enable_xcor": False,
+                "atac.trim_adapter.auto_detect_adapter": True,
+                "atac.bowtie2.cpu": 4,
+                "atac.filter.cpu": 4,
+                "atac.bam2ta.cpu": 4,
+                "atac.trim_adapter.cpu": 4,
+                "atac.align_only": True
             }
-            if not inst_name:
-                flag_instance = True
-                # include all other tags if Name tag is empty
-                ec2_log['tags'] = other_tags
-            elif any([wn for wn in flag_names if wn in ','.join(inst_name)]):
-                flag_instance = True
-            else:
-                flag_instance = False
-            # see if long running instances are associated with a deleted WFR
-            if flag_instance and inst_name and created < warn_time:
-                search_url = 'search/?type=WorkflowRunAwsem&awsem_job_id='
-                search_url += '&awsem_job_id='.join([name[6:] for name in inst_name if name.startswith('awsem-')])
-                wfrs = ff_utils.search_metadata(search_url, key=connection.ff_keys)
-                if wfrs:
-                    ec2_log['active workflow runs'] = [wfr['@id'] for wfr in wfrs]
-                deleted_wfrs = ff_utils.search_metadata(search_url + '&status=deleted', key=connection.ff_keys)
-                if deleted_wfrs:
-                    ec2_log['deleted workflow runs'] = [wfr['@id'] for wfr in deleted_wfrs]
-            # always add record to full_output; add to brief_output if
-            # the instance is flagged based on 'Name' tag
-            if created < fail_time:
-                if flag_instance:
-                    check.brief_output['two_weeks'].append(ec2_log)
-                check.full_output.append(ec2_log)
-            elif created < warn_time:
-                if flag_instance:
-                    check.brief_output['one_week'].append(ec2_log)
-                check.full_output.append(ec2_log)
-
-    if check.brief_output['one_week'] or check.brief_output['two_weeks']:
-        num_1wk = len(check.brief_output['one_week'])
-        num_2wk = len(check.brief_output['two_weeks'])
-        check.summary = ''
-        if check.brief_output['two_weeks']:
-            check.status = 'FAIL'
-            check.summary = '%s suspect EC2s running longer than 2 weeks' % num_2wk
-        if check.brief_output['one_week']:
-            if check.status != 'FAIL':
-                check.status = 'WARN'
-            if check.summary:
-                check.summary += ' and %s others longer than 1 week' % num_1wk
+            if paired == 'single':
+                frag_temp = [300]
+                fraglist = frag_temp * len(exp_files)
+                parameters['atac.fraglen'] = fraglist
+                parameters['atac.paired_end'] = False
+            elif paired == 'paired':
+                parameters['atac.paired_end'] = True
+
+            s1_input_files = input_files
+            s1_tag = exp_id
+            # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
+            keep, step1_status, step1_output = wfr_utils.stepper(library, keep,
+                                                                 'step1', s1_tag, exp_files,
+                                                                 s1_input_files, step1_name, 'atac.first_ta',
+                                                                 additional_input={'parameters': parameters})
+            if step1_status == 'complete':
+                # accumulate files to patch on experiment
+                patch_data = [step1_output, ]
+                complete['patch_opf'].append([exp_id, patch_data])
+                ta.append(step1_output)
             else:
-                check.summary = '%s suspect EC2s running longer than 1 week' % num_1wk
-        check.description = check.summary + '. Flagged because name is empty or contains %s. There are also %s non-flagged instances.' % (flag_names, len(check.full_output) - (num_1wk + num_2wk))
-    else:
-        check.status = 'PASS'
-        check.summary = '%s EC2s running longer than 1 week' % (len(check.full_output))
-    return check
-
+                # don't patch anything if at least one exp is still missing
+                ready_for_step2 = False
+            print('step1', step1_status, step1_output)
+
+        # back to set level
+        final_status = set_acc  # start the reporting with acc
+        all_completed = False
+        # is step0 step1 complete
+        if ready_for_step2:
+            # Following was the proposed logic, but it is not implemented
+            # Currently, for sets with more than 2 experiments, there are 2 options
+            # 1) pick best 2,   2) run mergebed (default)
+
+            # Proposed logic
+            # if there are more then 2 experiments, check the number of biological replicates
+            # if there is 1 Biological Replicate
+            # -pick best 2 exp
+            # if there are 2 Biological replicates
+            #  - run mergebed on bioreps with more then 1 technical replicate
+            # if there are 3 Biological replicates
+            # - if there are 3 total experiments (1 in each biological rep), pick best 2
+            # - else, run mergebed on bioreps with more then 1 technical replicate, and pick best 2 biorep
+            # if there are 4 or more Biolofical replicates
+            # - run mergebed on bioreps with more then 1 technical replicate, and pick best 2 biorep
+            # this only works with 2 experiments, if 3, pick best 2, if more, skip for now
+            ready_for_step3 = True
+            if len(ta) > 2:
+                if pick_best_2:
+                    # pick best 2 - False by default
+                    print('ExperimentSet has 3 experiments, selecting best 2')
+                    ta = wfr_utils.select_best_2(ta, all_files, all_qcs)
+                else:
+                    # run mergebed - default option
+                    s2_input_files = {'input_bed': ta}
+                    s2_tag = set_acc
+                    # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
+                    keep, step2_status, step2_output = wfr_utils.stepper(library, keep,
+                                                                         'step2', s2_tag, ta,
+                                                                         s2_input_files, step2_name, 'merged_bed')
+                    if step2_status == 'complete':
+                        ta = [step2_output, ]
+                    else:
+                        ready_for_step3 = False
+            if ready_for_step3:
+                # collect step3 input files
+                s3_input_files = {}
+                if organism == 'human':
+                    org = 'hs'
+                    s3_input_files['atac.blacklist'] = '/files-reference/4DNFIZ1TGJZR/'
+                    s3_input_files['atac.chrsz'] = '/files-reference/4DNFIZJB62D1/'
+                if organism == 'mouse':
+                    org = 'mm'
+                    s3_input_files['atac.blacklist'] = '/files-reference/4DNFIZ3FBPK8/'
+                    s3_input_files['atac.chrsz'] = '/files-reference/4DNFIBP173GC/'
+
+                def rename_chip(input_at_id_list):
+                    # rename bed.gz to tagAlign.gz
+                    renamed = []
+                    for a_file in input_at_id_list:
+                        acc = a_file.split('/')[2]
+                        renamed.append(acc + '.tagAlign.gz')
+                    return renamed
+
+                s3_input_files['additional_file_parameters'] = {}
+                s3_input_files['atac.tas'] = ta
+                s3_input_files['additional_file_parameters']['chip.tas'] = {"rename": rename_chip(ta)}
+                # collect parameters
+                if paired == 'single':
+                    chip_p = False
+                elif paired == 'paired':
+                    chip_p = True
+                parameters = {
+                    "atac.pipeline_type": 'atac',
+                    "atac.paired_end": chip_p,
+                    "atac.gensz": org,
+                    "atac.disable_ataqc": True,
+                    "atac.enable_xcor": False,
+                }
+                if paired == 'single':
+                    frag_temp = [300]
+                    fraglist = frag_temp * len(ta)
+                    parameters['atac.fraglen'] = fraglist
+
+                s3_tag = set_acc
+                # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
+                keep, step3_status, step3_output = wfr_utils.stepper(library, keep,
+                                                                     'step3', s3_tag, ta,
+                                                                     s3_input_files, step3_name,
+                                                                     ['atac.optimal_peak', 'atac.conservative_peak', 'atac.sig_fc'],
+                                                                     additional_input={'parameters': parameters})
+                if step3_status == 'complete':
+                    set_opt_peak = step3_output[0]
+                    set_cons_peak = step3_output[1]
+                    set_sig_fc = step3_output[2]
+                    # accumulate files to patch on experiment
+                    patch_data = [set_opt_peak, set_cons_peak, set_sig_fc]
+                    complete['patch_opf'].append([set_acc, patch_data])
+                    complete['add_tag'] = [set_acc, tag]
+                    all_completed = True
+
+        # unpack results
+        missing_run = keep['missing_run']
+        running = keep['running']
+        problematic_run = keep['problematic_run']
+        if all_completed:
+            final_status += ' completed'
+        else:
+            if missing_run:
+                final_status += ' |Missing: ' + " ".join([i[0] for i in missing_run])
+            if running:
+                final_status += ' |Running: ' + " ".join([i[0] for i in running])
+            if problematic_run:
+                final_status += ' |Problem: ' + " ".join([i[0] for i in problematic_run])
+
+        # add dictionaries to main ones
+        check.brief_output.append(final_status)
+        print(final_status)
+        if running:
+            check.full_output['running_runs'].append({set_acc: running})
+        if missing_run:
+            check.full_output['needs_runs'].append({set_acc: missing_run})
+        if problematic_run:
+            check.full_output['problematic_runs'].append({set_acc: problematic_run})
+        # if made it till the end
+        if complete.get('add_tag'):
+            assert not running
+            assert not problematic_run
+            assert not missing_run
+            check.full_output['completed_runs'].append(complete)
 
-@check_function(FS_dev='free', FF_hotseat='free', FF_mastertest='free', FF_webdev='free')
-def say_my_name(connection, **kwargs):
-    """List the person working on each environment."""
-    check = CheckResult(connection, 'say_my_name')
-    check.description = "Enter the new name or if you are done, use 'free' to clear your name"
+    # complete check values
     check.summary = ""
-    check.brief_output = ""
-    check.status = "PASS"
-    output = {}
-    # update with the new parameters ()
-    for a_key in ['FS_dev', 'FF_hotseat', 'FF_mastertest', 'FF_webdev']:
-        if kwargs.get(a_key):
-            val = kwargs[a_key]
-            if val.lower() == 'free':
-                val = 'free'
-            output[a_key] = val
-        else:
-            output[a_key] = 'free'
-    sum = str(output)[1:-1].replace("'", "")
-    check.summary = sum
-    check.brief_output = sum
+    if check.full_output['running_runs']:
+        check.summary = str(len(check.full_output['running_runs'])) + ' running|'
+    if check.full_output['skipped']:
+        check.summary += str(len(check.full_output['skipped'])) + ' skipped|'
+        check.status = 'WARN'
+    if check.full_output['needs_runs']:
+        check.summary += str(len(check.full_output['needs_runs'])) + ' missing|'
+        check.status = 'WARN'
+        check.allow_action = True
+    if check.full_output['completed_runs']:
+        check.summary += str(len(check.full_output['completed_runs'])) + ' completed|'
+        check.status = 'WARN'
+        check.allow_action = True
+    if check.full_output['problematic_runs']:
+        check.summary += str(len(check.full_output['problematic_runs'])) + ' problem|'
+        check.status = 'WARN'
     return check
+
+
+@action_function(start_runs=True, patch_completed=True)
+def atacseq_start(connection, **kwargs):
+    """Start runs by sending compiled input_json to run_workflow endpoint"""
+    start = datetime.utcnow()
+    action = ActionResult(connection, 'atacseq_start')
+    my_auth = connection.ff_keys
+    my_env = connection.ff_env
+    fs_env = connection.fs_env
+    atacseq_check_result = action.get_associated_check_result(kwargs).get('full_output', {})
+    missing_runs = []
+    patch_meta = []
+    if kwargs.get('start_runs'):
+        missing_runs = atacseq_check_result.get('needs_runs')
+    if kwargs.get('patch_completed'):
+        patch_meta = atacseq_check_result.get('completed_runs')
+    action = wfr_utils.start_tasks(missing_runs, patch_meta, action, my_auth, my_env, fs_env, start,  move_to_pc=True, runtype='atac')
+    return action
```

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/chalicelib_fourfront/package.py` & `foursight-3.4.0.5b2/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.1b7/pyproject.toml` & `foursight-3.4.0.5b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight"
-version = "3.4.0.1b7"
+version = "3.4.0.5b2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
@@ -20,15 +20,15 @@
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "4.1.0.1b7"
+foursight-core = "4.1.0.5b1"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.4.0.1b7/PKG-INFO` & `foursight-3.4.0.5b2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.4.0.1b7
+Version: 3.4.0.5b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dcicutils (==7.2.0.1b3)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.1.0.1b7)
+Requires-Dist: foursight-core (==4.1.0.5b1)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
```

