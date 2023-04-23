# Comparing `tmp/aws-solutions-constructs.aws-fargate-eventbridge-2.39.0.tar.gz` & `tmp/aws-solutions-constructs.aws-fargate-eventbridge-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src259931730/src/source/patterns/@aws-solutions-constructs/aws-fargate-eventbridge/dist/python/aws-solutions-", last modified: Sun Apr 23 17:27:36 2023, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-fargate-eventbridge/dist/python/aws-solutions-", last modified: Mon Jun 13 20:50:05 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0.tar` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9959 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9004 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1994 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/
--rw-r--r--   0 root         (0) root         (0)    34514 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   133343 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/aws-fargate-eventbridge@2.39.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs/aws_fargate_eventbridge/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9959 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-23 17:27:36.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9914 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8991 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1912 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/
+-rw-r--r--   0 root         (0) root         (0)    28487 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      461 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   132626 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/aws-fargate-eventbridge@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs/aws_fargate_eventbridge/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9914 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/LICENSE` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/PKG-INFO` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-eventbridge
-Version: 2.39.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS Fargate to Amazon Eventbridge integration
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aws-fargate-eventbridge module
@@ -95,36 +95,36 @@
 ```
 
 ## Pattern Construct Props
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | publicApi | boolean | Whether the construct is deploying a private or public API. This has implications for the VPC. |
-| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
-| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
-| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
+| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
+| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
+| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
 | ecrRepositoryArn? | `string` | The arn of an ECR Repository containing the image to use to generate the containers. Either this or the image property of containerDefinitionProps must be provided. format: arn:aws:ecr:*region*:*account number*:repository/*Repository Name* |
 | ecrImageVersion? | `string` | The version of the image to use from the repository. Defaults to 'Latest'|
-| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
-| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
-| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
-| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
-| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
-| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
-| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
+| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
+| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
+| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
+| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
+| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
+| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
+| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
 |eventBusEnvironmentVariableName?|`string`|Optional Name for the container environment variable set to the DynamoDB table name. Default: EVENTBUS_NAME|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
-| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
-| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
-| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
-| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
+| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
+| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
+| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
+| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
 
 ## Default settings
 
 Out of the box implementation of the Construct without any override will set the following defaults:
 
 ### AWS Fargate Service
 
@@ -150,8 +150,10 @@
 ## Architecture
 
 ![Architecture Diagram](architecture.png)
 
 ---
 
 
-© Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+© Copyright 2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+
+
```

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/README.md` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -72,36 +72,36 @@
 ```
 
 ## Pattern Construct Props
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | publicApi | boolean | Whether the construct is deploying a private or public API. This has implications for the VPC. |
-| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
-| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
-| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
+| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
+| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
+| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
 | ecrRepositoryArn? | `string` | The arn of an ECR Repository containing the image to use to generate the containers. Either this or the image property of containerDefinitionProps must be provided. format: arn:aws:ecr:*region*:*account number*:repository/*Repository Name* |
 | ecrImageVersion? | `string` | The version of the image to use from the repository. Defaults to 'Latest'|
-| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
-| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
-| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
-| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
-| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
-| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
-| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
+| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
+| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
+| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
+| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
+| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
+| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
+| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
 |eventBusEnvironmentVariableName?|`string`|Optional Name for the container environment variable set to the DynamoDB table name. Default: EVENTBUS_NAME|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
-| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
-| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
-| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
-| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
+| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
+| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
+| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
+| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
 
 ## Default settings
 
 Out of the box implementation of the Construct without any override will set the following defaults:
 
 ### AWS Fargate Service
 
@@ -127,8 +127,8 @@
 ## Architecture
 
 ![Architecture Diagram](architecture.png)
 
 ---
 
 
-© Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+© Copyright 2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
```

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/setup.py` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-fargate-eventbridge",
-    "version": "2.39.0",
+    "version": "2.9.0",
     "description": "CDK Constructs for AWS Fargate to Amazon Eventbridge integration",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,39 +22,37 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_fargate_eventbridge",
         "aws_solutions_constructs.aws_fargate_eventbridge._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_fargate_eventbridge._jsii": [
-            "aws-fargate-eventbridge@2.39.0.jsii.tgz"
+            "aws-fargate-eventbridge@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_fargate_eventbridge": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.76.0, <3.0.0",
-        "aws-solutions-constructs.core==2.39.0",
+        "aws-cdk-lib>=2.23.0, <3.0.0",
+        "aws-solutions-constructs.core==2.9.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "jsii>=1.60.1, <2.0.0",
+        "publication>=0.0.3"
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
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-eventbridge
-Version: 2.39.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS Fargate to Amazon Eventbridge integration
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aws-fargate-eventbridge module
@@ -95,36 +95,36 @@
 ```
 
 ## Pattern Construct Props
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | publicApi | boolean | Whether the construct is deploying a private or public API. This has implications for the VPC. |
-| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
-| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
-| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
+| vpcProps? | [ec2.VpcProps](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.VpcProps.html) | Optional custom properties for a VPC the construct will create. This VPC will be used by any Private Hosted Zone the construct creates (that's why loadBalancerProps and privateHostedZoneProps can't include a VPC). Providing both this and existingVpc is an error. |
+| existingVpc? | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | An existing VPC in which to deploy the construct. Providing both this and vpcProps is an error. If the client provides an existing load balancer and/or existing Private Hosted Zone, those constructs must exist in this VPC. |
+| clusterProps? | [ecs.ClusterProps](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ClusterProps.html) | Optional properties to create a new ECS cluster. To provide an existing cluster, use the cluster attribute of fargateServiceProps. |
 | ecrRepositoryArn? | `string` | The arn of an ECR Repository containing the image to use to generate the containers. Either this or the image property of containerDefinitionProps must be provided. format: arn:aws:ecr:*region*:*account number*:repository/*Repository Name* |
 | ecrImageVersion? | `string` | The version of the image to use from the repository. Defaults to 'Latest'|
-| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
-| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
-| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
-| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
-| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
-| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
-| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
+| containerDefinitionProps? | [ecs.ContainerDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinitionProps.html) | Optional props to define the container created for the Fargate Service (defaults found in fargate-defaults.ts) |
+| fargateTaskDefinitionProps? | [ecs.FargateTaskDefinitionProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateTaskDefinitionProps.html) | Optional props to define the Fargate Task Definition for this construct  (defaults found in fargate-defaults.ts) |
+| fargateServiceProps? | [ecs.FargateServiceProps | any](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateServiceProps.html) | Optional values to override default Fargate Task definition properties (fargate-defaults.ts). The construct will default to launching the service is the most isolated subnets available (precedence: Isolated, Private and Public). Override those and other defaults here. |
+| existingFargateServiceObject? | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | A Fargate Service already instantiated (probably by another Solutions Construct). If this is specified, then no props defining a new service can be provided, including: ecrImageVersion, containerDefinitionProps, fargateTaskDefinitionProps, ecrRepositoryArn, fargateServiceProps, clusterProps |
+| existingContainerDefinitionObject? | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | A container definition already instantiated as part of a Fargate service. This must be the container in the existingFargateServiceObject |
+| existingEventBusInterface? | [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)| Optional user-provided custom event bus for construct to use. Providing both this and `eventBusProps` results an error.|
+| eventBusProps?	| [`events.EventBusProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.EventBusProps.html)|Optional user-provided properties to override the default properties when creating a custom event bus. Setting this value to `{}` will create a custom event bus using all default properties. If neither this nor `existingEventBusInterface` is provided the construct will use the `default` event bus. Providing both this and `existingEventBusInterface` results an error.|
 |eventBusEnvironmentVariableName?|`string`|Optional Name for the container environment variable set to the DynamoDB table name. Default: EVENTBUS_NAME|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
-| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
-| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
-| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
-| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
+| vpc | [ec2.IVpc](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-ec2.IVpc.html) | The VPC used by the construct (whether created by the construct or provided by the client) |
+| service | [ecs.FargateService](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.FargateService.html) | The AWS Fargate service used by this construct (whether created by this construct or passed to this construct at initialization) |
+| container | [ecs.ContainerDefinition](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-ecs.ContainerDefinition.html) | The container associated with the AWS Fargate service in the service property. |
+| eventBus?	| [`events.IEventBus`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-events.IEventBus.html)|Returns the instance of `events.IEventBus` used by the construct|
 
 ## Default settings
 
 Out of the box implementation of the Construct without any override will set the following defaults:
 
 ### AWS Fargate Service
 
@@ -150,8 +150,10 @@
 ## Architecture
 
 ![Architecture Diagram](architecture.png)
 
 ---
 
 
-© Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+© Copyright 2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+
+
```

### Comparing `aws-solutions-constructs.aws-fargate-eventbridge-2.39.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-fargate-eventbridge-2.9.0/src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/requires.txt
 src/aws_solutions_constructs.aws_fargate_eventbridge.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_fargate_eventbridge/__init__.py
 src/aws_solutions_constructs/aws_fargate_eventbridge/py.typed
 src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/__init__.py
-src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/aws-fargate-eventbridge@2.39.0.jsii.tgz
+src/aws_solutions_constructs/aws_fargate_eventbridge/_jsii/aws-fargate-eventbridge@2.9.0.jsii.tgz
```

