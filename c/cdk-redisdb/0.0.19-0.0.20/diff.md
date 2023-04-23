# Comparing `tmp/cdk-redisdb-0.0.19.tar.gz` & `tmp/cdk-redisdb-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.19.tar", last modified: Fri Nov 25 04:03:48 2022, max compression
+gzip compressed data, was "cdk-redisdb-0.0.20.tar", last modified: Sun Apr 23 11:06:16 2023, max compression
```

## Comparing `cdk-redisdb-0.0.19.tar` & `cdk-redisdb-0.0.20.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    43790 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.19.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 04:03:32.000000 cdk-redisdb-0.0.19/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 04:03:48.016317 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2022-11-25 04:03:47.000000 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-11-25 04:03:47.000000 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 04:03:47.000000 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-11-25 04:03:47.000000 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-11-25 04:03:47.000000 cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48022 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25738 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.20.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:06:02.000000 cdk-redisdb-0.0.20/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:06:16.810687 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-23 11:06:16.000000 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-23 11:06:16.000000 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:06:16.000000 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 11:06:16.000000 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 11:06:16.000000 cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.19/LICENSE` & `cdk-redisdb-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.19/PKG-INFO` & `cdk-redisdb-0.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.19
+Version: 0.0.20
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -134,9 +134,7 @@
 
 * MemoryDB ACLs (commented out to avoid default bad practices, read comments to understand the CloudFormation)
 
 Features to come:
 
 * Replication Groups with cluster mode disabled (for those using multiple databases)
 * Improved API - sane choice of props
-
-
```

### Comparing `cdk-redisdb-0.0.19/README.md` & `cdk-redisdb-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.19/setup.py` & `cdk-redisdb-0.0.20/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.19",
+    "version": "0.0.20",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.19.jsii.tgz"
+            "cdk-redisdb@0.0.20.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.51.1, <3.0.0",
+        "aws-cdk-lib>=2.76.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.71.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-redisdb-0.0.19/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.20/src/cdk_redisdb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,52 +126,53 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import aws_cdk
-import aws_cdk.aws_ec2
-import aws_cdk.aws_elasticache
-import aws_cdk.aws_memorydb
-import constructs
+import aws_cdk as _aws_cdk_ceddda9d
+import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
+import aws_cdk.aws_elasticache as _aws_cdk_aws_elasticache_ceddda9d
+import aws_cdk.aws_memorydb as _aws_cdk_aws_memorydb_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class MemoryDB(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-redisdb.MemoryDB",
 ):
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
         auth_token: typing.Optional[builtins.str] = None,
         engine_version: typing.Optional[builtins.str] = None,
-        existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
+        existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
         existing_subnet_group_name: typing.Optional[builtins.str] = None,
-        existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         memory_autoscaling_target: typing.Optional[jsii.Number] = None,
         nodes: typing.Optional[jsii.Number] = None,
         nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         node_type: typing.Optional[builtins.str] = None,
         parameter_group_name: typing.Optional[builtins.str] = None,
         replicas: typing.Optional[jsii.Number] = None,
         replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         subnet_group_name: typing.Optional[builtins.str] = None,
-        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
-        synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
+        synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param at_rest_encryption_enabled: 
@@ -189,50 +190,22 @@
         :param replicas_cpu_autoscaling_target: 
         :param subnet_group_name: 
         :param transit_encryption_enabled: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
-        :param synthesizer: Synthesis method to use while deploying this stack. Default: - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag is set, ``LegacyStackSynthesizer`` otherwise.
+        :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
-            def stub(
-                scope: constructs.Construct,
-                id: builtins.str,
-                *,
-                at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-                auth_token: typing.Optional[builtins.str] = None,
-                engine_version: typing.Optional[builtins.str] = None,
-                existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
-                existing_subnet_group_name: typing.Optional[builtins.str] = None,
-                existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
-                memory_autoscaling_target: typing.Optional[jsii.Number] = None,
-                nodes: typing.Optional[jsii.Number] = None,
-                nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                node_type: typing.Optional[builtins.str] = None,
-                parameter_group_name: typing.Optional[builtins.str] = None,
-                replicas: typing.Optional[jsii.Number] = None,
-                replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                subnet_group_name: typing.Optional[builtins.str] = None,
-                transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-                analytics_reporting: typing.Optional[builtins.bool] = None,
-                cross_region_references: typing.Optional[builtins.bool] = None,
-                description: typing.Optional[builtins.str] = None,
-                env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
-                stack_name: typing.Optional[builtins.str] = None,
-                synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
-                tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-                termination_protection: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4d7a8dc42dc5ff5ca38eba77f973802f25574532651ca42df5294eac20265186)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = RedisDBProps(
             at_rest_encryption_enabled=at_rest_encryption_enabled,
             auth_token=auth_token,
             engine_version=engine_version,
             existing_security_group=existing_security_group,
@@ -247,59 +220,61 @@
             replicas_cpu_autoscaling_target=replicas_cpu_autoscaling_target,
             subnet_group_name=subnet_group_name,
             transit_encryption_enabled=transit_encryption_enabled,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
+            permissions_boundary=permissions_boundary,
             stack_name=stack_name,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_memorydb.CfnCluster:
-        return typing.cast(aws_cdk.aws_memorydb.CfnCluster, jsii.get(self, "cluster"))
+    def cluster(self) -> _aws_cdk_aws_memorydb_ceddda9d.CfnCluster:
+        return typing.cast(_aws_cdk_aws_memorydb_ceddda9d.CfnCluster, jsii.get(self, "cluster"))
 
 
 class RedisDB(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-redisdb.RedisDB",
 ):
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
         auth_token: typing.Optional[builtins.str] = None,
         engine_version: typing.Optional[builtins.str] = None,
-        existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
+        existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
         existing_subnet_group_name: typing.Optional[builtins.str] = None,
-        existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         memory_autoscaling_target: typing.Optional[jsii.Number] = None,
         nodes: typing.Optional[jsii.Number] = None,
         nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         node_type: typing.Optional[builtins.str] = None,
         parameter_group_name: typing.Optional[builtins.str] = None,
         replicas: typing.Optional[jsii.Number] = None,
         replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         subnet_group_name: typing.Optional[builtins.str] = None,
-        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
-        synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
+        synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param at_rest_encryption_enabled: 
@@ -317,50 +292,22 @@
         :param replicas_cpu_autoscaling_target: 
         :param subnet_group_name: 
         :param transit_encryption_enabled: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
-        :param synthesizer: Synthesis method to use while deploying this stack. Default: - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag is set, ``LegacyStackSynthesizer`` otherwise.
+        :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
-            def stub(
-                scope: constructs.Construct,
-                id: builtins.str,
-                *,
-                at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-                auth_token: typing.Optional[builtins.str] = None,
-                engine_version: typing.Optional[builtins.str] = None,
-                existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
-                existing_subnet_group_name: typing.Optional[builtins.str] = None,
-                existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
-                memory_autoscaling_target: typing.Optional[jsii.Number] = None,
-                nodes: typing.Optional[jsii.Number] = None,
-                nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                node_type: typing.Optional[builtins.str] = None,
-                parameter_group_name: typing.Optional[builtins.str] = None,
-                replicas: typing.Optional[jsii.Number] = None,
-                replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                subnet_group_name: typing.Optional[builtins.str] = None,
-                transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-                analytics_reporting: typing.Optional[builtins.bool] = None,
-                cross_region_references: typing.Optional[builtins.bool] = None,
-                description: typing.Optional[builtins.str] = None,
-                env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
-                stack_name: typing.Optional[builtins.str] = None,
-                synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
-                tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-                termination_protection: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__05da1aee3f253dc490da29cff41fe0598311857fc55a6db5bb2c62e3f73708d4)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = RedisDBProps(
             at_rest_encryption_enabled=at_rest_encryption_enabled,
             auth_token=auth_token,
             engine_version=engine_version,
             existing_security_group=existing_security_group,
@@ -375,36 +322,40 @@
             replicas_cpu_autoscaling_target=replicas_cpu_autoscaling_target,
             subnet_group_name=subnet_group_name,
             transit_encryption_enabled=transit_encryption_enabled,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
+            permissions_boundary=permissions_boundary,
             stack_name=stack_name,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="replicationGroup")
-    def replication_group(self) -> aws_cdk.aws_elasticache.CfnReplicationGroup:
-        return typing.cast(aws_cdk.aws_elasticache.CfnReplicationGroup, jsii.get(self, "replicationGroup"))
+    def replication_group(
+        self,
+    ) -> _aws_cdk_aws_elasticache_ceddda9d.CfnReplicationGroup:
+        return typing.cast(_aws_cdk_aws_elasticache_ceddda9d.CfnReplicationGroup, jsii.get(self, "replicationGroup"))
 
 
 @jsii.data_type(
     jsii_type="cdk-redisdb.RedisDBProps",
-    jsii_struct_bases=[aws_cdk.StackProps],
+    jsii_struct_bases=[_aws_cdk_ceddda9d.StackProps],
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
+        "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "at_rest_encryption_enabled": "atRestEncryptionEnabled",
         "auth_token": "authToken",
         "engine_version": "engineVersion",
@@ -418,49 +369,51 @@
         "parameter_group_name": "parameterGroupName",
         "replicas": "replicas",
         "replicas_cpu_autoscaling_target": "replicasCpuAutoscalingTarget",
         "subnet_group_name": "subnetGroupName",
         "transit_encryption_enabled": "transitEncryptionEnabled",
     },
 )
-class RedisDBProps(aws_cdk.StackProps):
+class RedisDBProps(_aws_cdk_ceddda9d.StackProps):
     def __init__(
         self,
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
-        synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
+        synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
-        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
         auth_token: typing.Optional[builtins.str] = None,
         engine_version: typing.Optional[builtins.str] = None,
-        existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
+        existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
         existing_subnet_group_name: typing.Optional[builtins.str] = None,
-        existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         memory_autoscaling_target: typing.Optional[jsii.Number] = None,
         nodes: typing.Optional[jsii.Number] = None,
         nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         node_type: typing.Optional[builtins.str] = None,
         parameter_group_name: typing.Optional[builtins.str] = None,
         replicas: typing.Optional[jsii.Number] = None,
         replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
         subnet_group_name: typing.Optional[builtins.str] = None,
-        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
+        transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
-        :param synthesizer: Synthesis method to use while deploying this stack. Default: - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag is set, ``LegacyStackSynthesizer`` otherwise.
+        :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param at_rest_encryption_enabled: 
         :param auth_token: 
         :param engine_version: 
         :param existing_security_group: 
         :param existing_subnet_group_name: 
@@ -472,48 +425,22 @@
         :param parameter_group_name: 
         :param replicas: 
         :param replicas_cpu_autoscaling_target: 
         :param subnet_group_name: 
         :param transit_encryption_enabled: 
         '''
         if isinstance(env, dict):
-            env = aws_cdk.Environment(**env)
+            env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
-            def stub(
-                *,
-                analytics_reporting: typing.Optional[builtins.bool] = None,
-                cross_region_references: typing.Optional[builtins.bool] = None,
-                description: typing.Optional[builtins.str] = None,
-                env: typing.Optional[typing.Union[aws_cdk.Environment, typing.Dict[str, typing.Any]]] = None,
-                stack_name: typing.Optional[builtins.str] = None,
-                synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
-                tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-                termination_protection: typing.Optional[builtins.bool] = None,
-                at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-                auth_token: typing.Optional[builtins.str] = None,
-                engine_version: typing.Optional[builtins.str] = None,
-                existing_security_group: typing.Optional[aws_cdk.aws_ec2.ISecurityGroup] = None,
-                existing_subnet_group_name: typing.Optional[builtins.str] = None,
-                existing_vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
-                memory_autoscaling_target: typing.Optional[jsii.Number] = None,
-                nodes: typing.Optional[jsii.Number] = None,
-                nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                node_type: typing.Optional[builtins.str] = None,
-                parameter_group_name: typing.Optional[builtins.str] = None,
-                replicas: typing.Optional[jsii.Number] = None,
-                replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
-                subnet_group_name: typing.Optional[builtins.str] = None,
-                transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__feed39ed5eb19b3bf59d2dc1804bde942b946d763afce92b794e0259cb4d1191)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
+            check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument at_rest_encryption_enabled", value=at_rest_encryption_enabled, expected_type=type_hints["at_rest_encryption_enabled"])
             check_type(argname="argument auth_token", value=auth_token, expected_type=type_hints["auth_token"])
             check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
@@ -525,23 +452,25 @@
             check_type(argname="argument nodes_cpu_autoscaling_target", value=nodes_cpu_autoscaling_target, expected_type=type_hints["nodes_cpu_autoscaling_target"])
             check_type(argname="argument node_type", value=node_type, expected_type=type_hints["node_type"])
             check_type(argname="argument parameter_group_name", value=parameter_group_name, expected_type=type_hints["parameter_group_name"])
             check_type(argname="argument replicas", value=replicas, expected_type=type_hints["replicas"])
             check_type(argname="argument replicas_cpu_autoscaling_target", value=replicas_cpu_autoscaling_target, expected_type=type_hints["replicas_cpu_autoscaling_target"])
             check_type(argname="argument subnet_group_name", value=subnet_group_name, expected_type=type_hints["subnet_group_name"])
             check_type(argname="argument transit_encryption_enabled", value=transit_encryption_enabled, expected_type=type_hints["transit_encryption_enabled"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if analytics_reporting is not None:
             self._values["analytics_reporting"] = analytics_reporting
         if cross_region_references is not None:
             self._values["cross_region_references"] = cross_region_references
         if description is not None:
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
+        if permissions_boundary is not None:
+            self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
@@ -609,15 +538,15 @@
 
         :default: - No description.
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def env(self) -> typing.Optional[aws_cdk.Environment]:
+    def env(self) -> typing.Optional[_aws_cdk_ceddda9d.Environment]:
         '''The AWS environment (account/region) where this stack will be deployed.
 
         Set the ``region``/``account`` fields of ``env`` to either a concrete value to
         select the indicated environment (recommended for production stacks), or to
         the values of environment variables
         ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment
         depend on the AWS credentials/configuration that the CDK CLI is executed
@@ -676,36 +605,54 @@
             
             // Define an environment-agnostic stack:
             // `.account` and `.region` will resolve to `{ "Ref": "AWS::AccountId" }` and `{ "Ref": "AWS::Region" }` respectively.
             // which will only resolve to actual values by CloudFormation during deployment.
             new MyStack(app, 'Stack1');
         '''
         result = self._values.get("env")
-        return typing.cast(typing.Optional[aws_cdk.Environment], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Environment], result)
+
+    @builtins.property
+    def permissions_boundary(
+        self,
+    ) -> typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary]:
+        '''Options for applying a permissions boundary to all IAM Roles and Users created within this Stage.
+
+        :default: - no permissions boundary is applied
+        '''
+        result = self._values.get("permissions_boundary")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary], result)
 
     @builtins.property
     def stack_name(self) -> typing.Optional[builtins.str]:
         '''Name to deploy the stack with.
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def synthesizer(self) -> typing.Optional[aws_cdk.IStackSynthesizer]:
+    def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
-        :default:
+        The Stack Synthesizer controls aspects of synthesis and deployment,
+        like how assets are referenced and what IAM roles to use. For more
+        information, see the README of the main CDK package.
+
+        If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used.
+        If that is not specified, ``DefaultStackSynthesizer`` is used if
+        ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major
+        version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no
+        other synthesizer is specified.
 
-        - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag
-        is set, ``LegacyStackSynthesizer`` otherwise.
+        :default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         '''
         result = self._values.get("synthesizer")
-        return typing.cast(typing.Optional[aws_cdk.IStackSynthesizer], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Stack tags that will be applied to all the taggable resources and the stack itself.
 
         :default: {}
         '''
@@ -720,44 +667,44 @@
         '''
         result = self._values.get("termination_protection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def at_rest_encryption_enabled(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]]:
         result = self._values.get("at_rest_encryption_enabled")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]], result)
 
     @builtins.property
     def auth_token(self) -> typing.Optional[builtins.str]:
         result = self._values.get("auth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def engine_version(self) -> typing.Optional[builtins.str]:
         result = self._values.get("engine_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def existing_security_group(
         self,
-    ) -> typing.Optional[aws_cdk.aws_ec2.ISecurityGroup]:
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]:
         result = self._values.get("existing_security_group")
-        return typing.cast(typing.Optional[aws_cdk.aws_ec2.ISecurityGroup], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup], result)
 
     @builtins.property
     def existing_subnet_group_name(self) -> typing.Optional[builtins.str]:
         result = self._values.get("existing_subnet_group_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def existing_vpc(self) -> typing.Optional[aws_cdk.aws_ec2.IVpc]:
+    def existing_vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
         result = self._values.get("existing_vpc")
-        return typing.cast(typing.Optional[aws_cdk.aws_ec2.IVpc], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
 
     @builtins.property
     def memory_autoscaling_target(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("memory_autoscaling_target")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
@@ -794,17 +741,17 @@
     def subnet_group_name(self) -> typing.Optional[builtins.str]:
         result = self._values.get("subnet_group_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def transit_encryption_enabled(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]]:
         result = self._values.get("transit_encryption_enabled")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, aws_cdk.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -817,7 +764,101 @@
 __all__ = [
     "MemoryDB",
     "RedisDB",
     "RedisDBProps",
 ]
 
 publication.publish()
+
+def _typecheckingstub__4d7a8dc42dc5ff5ca38eba77f973802f25574532651ca42df5294eac20265186(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+    auth_token: typing.Optional[builtins.str] = None,
+    engine_version: typing.Optional[builtins.str] = None,
+    existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
+    existing_subnet_group_name: typing.Optional[builtins.str] = None,
+    existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    memory_autoscaling_target: typing.Optional[jsii.Number] = None,
+    nodes: typing.Optional[jsii.Number] = None,
+    nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    node_type: typing.Optional[builtins.str] = None,
+    parameter_group_name: typing.Optional[builtins.str] = None,
+    replicas: typing.Optional[jsii.Number] = None,
+    replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    subnet_group_name: typing.Optional[builtins.str] = None,
+    transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+    analytics_reporting: typing.Optional[builtins.bool] = None,
+    cross_region_references: typing.Optional[builtins.bool] = None,
+    description: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    stack_name: typing.Optional[builtins.str] = None,
+    synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__05da1aee3f253dc490da29cff41fe0598311857fc55a6db5bb2c62e3f73708d4(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+    auth_token: typing.Optional[builtins.str] = None,
+    engine_version: typing.Optional[builtins.str] = None,
+    existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
+    existing_subnet_group_name: typing.Optional[builtins.str] = None,
+    existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    memory_autoscaling_target: typing.Optional[jsii.Number] = None,
+    nodes: typing.Optional[jsii.Number] = None,
+    nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    node_type: typing.Optional[builtins.str] = None,
+    parameter_group_name: typing.Optional[builtins.str] = None,
+    replicas: typing.Optional[jsii.Number] = None,
+    replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    subnet_group_name: typing.Optional[builtins.str] = None,
+    transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+    analytics_reporting: typing.Optional[builtins.bool] = None,
+    cross_region_references: typing.Optional[builtins.bool] = None,
+    description: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    stack_name: typing.Optional[builtins.str] = None,
+    synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__feed39ed5eb19b3bf59d2dc1804bde942b946d763afce92b794e0259cb4d1191(
+    *,
+    analytics_reporting: typing.Optional[builtins.bool] = None,
+    cross_region_references: typing.Optional[builtins.bool] = None,
+    description: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    stack_name: typing.Optional[builtins.str] = None,
+    synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+    at_rest_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+    auth_token: typing.Optional[builtins.str] = None,
+    engine_version: typing.Optional[builtins.str] = None,
+    existing_security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup] = None,
+    existing_subnet_group_name: typing.Optional[builtins.str] = None,
+    existing_vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    memory_autoscaling_target: typing.Optional[jsii.Number] = None,
+    nodes: typing.Optional[jsii.Number] = None,
+    nodes_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    node_type: typing.Optional[builtins.str] = None,
+    parameter_group_name: typing.Optional[builtins.str] = None,
+    replicas: typing.Optional[jsii.Number] = None,
+    replicas_cpu_autoscaling_target: typing.Optional[jsii.Number] = None,
+    subnet_group_name: typing.Optional[builtins.str] = None,
+    transit_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _aws_cdk_ceddda9d.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cdk-redisdb-0.0.19/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.20/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.19
+Version: 0.0.20
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -134,9 +134,7 @@
 
 * MemoryDB ACLs (commented out to avoid default bad practices, read comments to understand the CloudFormation)
 
 Features to come:
 
 * Replication Groups with cluster mode disabled (for those using multiple databases)
 * Improved API - sane choice of props
-
-
```

