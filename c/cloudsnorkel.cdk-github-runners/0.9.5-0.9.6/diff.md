# Comparing `tmp/cloudsnorkel.cdk-github-runners-0.9.5.tar.gz` & `tmp/cloudsnorkel.cdk-github-runners-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.5.tar", last modified: Mon Apr 17 04:11:37 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.6.tar", last modified: Sun Apr 23 18:13:16 2023, max compression
```

## Comparing `cloudsnorkel.cdk-github-runners-0.9.5.tar` & `cloudsnorkel.cdk-github-runners-0.9.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/
--rw-r--r--   0 runner    (1001) docker     (123)   560908 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1988051 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.791942 cloudsnorkel.cdk-github-runners-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.791942 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)   562399 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1997391 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/LICENSE` & `cloudsnorkel.cdk-github-runners-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,12 @@
-Metadata-Version: 2.1
-Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.5
-Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
-Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
-Author: Amir Szekely<amir@cloudsnorkel.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -75,53 +51,131 @@
 * ECS is useful when you want to control the infrastructure, like leaving the runner host running for faster startups
 * Lambda is useful for short jobs that can work within time, size and readonly system constraints
 
 You can also create your own provider by implementing `IRunnerProvider`.
 
 ## Installation
 
-1. Confirm you're using CDK v2
-2. Install the appropriate package
+1. Install and use the appropriate package
+
+   <details><summary>Python</summary>
+
+   ### Install
+
+   Available on [PyPI](https://pypi.org/project/cloudsnorkel.cdk-github-runners).
+
+   ```bash
+   pip install cloudsnorkel.cdk-github-runners
+   ```
+
+   ### Use
+
+   ```python
+   from cloudsnorkel.cdk_github_runners import GitHubRunners
+
+   GitHubRunners(self, "runners")
+   ```
+
+   </details>
+   <details><summary>TypeScript or JavaScript</summary>
+
+   ### Install
+
+   Available on [npm](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners).
 
-   1. [Python](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
+   ```bash
+   npm i @cloudsnorkel/cdk-github-runners
+   ```
 
-      ```
-      pip install cloudsnorkel.cdk-github-runners
-      ```
-   2. [TypeScript or JavaScript](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
-
-      ```
-      npm i @cloudsnorkel/cdk-github-runners
-      ```
-   3. [Java](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+   ### Use
 
-      ```xml
-      <dependency>
+   ```python
+   import { GitHubRunners } from '@cloudsnorkel/cdk-github-runners';
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+   <details><summary>Java</summary>
+
+   ### Install
+
+   Available on [Maven](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/).
+
+   ```xml
+   <dependency>
       <groupId>com.cloudsnorkel</groupId>
       <artifactId>cdk.github.runners</artifactId>
-      </dependency>
-      ```
-   4. [Go](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
-
-      ```
-      go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
-      ```
-   5. [.NET](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
-
-      ```
-      dotnet add package CloudSnorkel.Cdk.Github.Runners
-      ```
-3. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
-4. Deploy your stack
-5. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
-6. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
-7. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
-8. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
-9. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
-10. If the action is not successful, see [troubleshooting](#Troubleshooting)
+   </dependency>
+   ```
+
+   ### Use
+
+   ```java
+   import com.cloudsnorkel.cdk.github.runners.GitHubRunners;
+
+   GitHubRunners.Builder.create(this, "runners").build();
+   ```
+
+   </details>
+   <details><summary>Go</summary>
+
+   ### Install
+
+   Available on [GitHub](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners).
+
+   ```bash
+   go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
+   ```
+
+   ### Use
+
+   ```go
+   import "github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners"
+
+   NewGitHubRunners(this, jsii.String("runners"))
+   ```
+
+   </details>
+   <details><summary>.NET</summary>
+
+   ### Install
+
+   Available on [Nuget](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/).
+
+   ```bash
+   dotnet add package CloudSnorkel.Cdk.Github.Runners
+   ```
+
+   ### Use
+
+   ```csharp
+   using CloudSnorkel;
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+2. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
+3. Deploy your stack
+4. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
+
+   ```
+    ✅  github-runners-test
+
+   ✨  Deployment time: 260.01s
+
+   Outputs:
+   github-runners-test.runnersstatuscommand4A30F0F5 = aws --region us-east-1 lambda invoke --function-name github-runners-test-runnersstatus1A5771C0-mvttg8oPQnQS status.json
+   ```
+5. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
+6. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
+7. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
+8. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
+9. If the action is not successful, see [troubleshooting](#Troubleshooting)
 
 [![Demo](demo-thumbnail.jpg)](https://youtu.be/wlyv_3V8lIw)
 
 ## Customizing
 
 The default providers configured by `GitHubRunners` are useful for testing but probably not too much for actual production work. They run in the default VPC or no VPC and have no added IAM permissions. You would usually want to configure the providers yourself.
 
@@ -131,17 +185,17 @@
 let vpc: ec2.Vpc;
 let runnerSg: ec2.SecurityGroup;
 let dbSg: ec2.SecurityGroup;
 let bucket: s3.Bucket;
 
 // create a custom CodeBuild provider
 const myProvider = new CodeBuildRunnerProvider(this, 'codebuild runner', {
-  label: 'my-codebuild',
-  vpc: vpc,
-  securityGroup: runnerSg,
+   labels: ['my-codebuild'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
 });
 // grant some permissions to the provider
 bucket.grantReadWrite(myProvider);
 dbSg.connections.allowFrom(runnerSg, ec2.Port.tcp(3306), 'allow runners to connect to MySQL database');
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
@@ -158,17 +212,17 @@
    rebuildInterval: Duration.days(14),
 });
 myBuilder.addComponent(
   RunnerImageComponent.custom({ commands: ['apt install -y nginx xz-utils'] })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-   label: 'customized-fargate',
+   labels: ['customized-fargate'],
    vpc: vpc,
-   securityGroup: runnerSg,
+   securityGroups: [runnerSg],
    imageBuilder: myBuilder,
 });
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
    providers: [myProvider],
 });
@@ -186,55 +240,55 @@
       - run: echo hello world
 ```
 
 Windows images can also be customized the same way.
 
 ```python
 const myWindowsBuilder = FargateRunnerProvider.imageBuilder(this, 'Windows image builder', {
-  architecture: Architecture.X86_64,
-  os: Os.WINDOWS,
-  runnerVersion: RunnerVersion.specific('2.291.0'),
-  rebuildInterval: Duration.days(14),
+   architecture: Architecture.X86_64,
+   os: Os.WINDOWS,
+   runnerVersion: RunnerVersion.specific('2.291.0'),
+   rebuildInterval: Duration.days(14),
 });
 myWindowsBuilder.addComponent(
-  RunnerImageComponent.custom({
-    name: 'Ninja',
-    commands: [
-      'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
-      'Expand-Archive ninja.zip -DestinationPath C:\\actions',
-      'del ninja.zip',
-    ],
-  })
+        RunnerImageComponent.custom({
+           name: 'Ninja',
+           commands: [
+              'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
+              'Expand-Archive ninja.zip -DestinationPath C:\\actions',
+              'del ninja.zip',
+           ],
+        })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-  label: 'customized-windows-fargate',
-  vpc: vpc,
-  securityGroup: runnerSg,
-  imageBuidler: myWindowsBuilder,
+   labels: ['customized-windows-fargate'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
+   imageBuidler: myWindowsBuilder,
 });
 
 new GitHubRunners(this, 'runners', {
-  providers: [myProvider],
+   providers: [myProvider],
 });
 ```
 
 The runner OS and architecture is determined by the image it is set to use. For example, to create a Fargate runner provider for ARM64 set the `architecture` property for the image builder to `Architecture.ARM64` in the image builder properties.
 
 ```python
 new GitHubRunners(this, 'runners', {
-  providers: [
-    new FargateRunnerProvider(this, 'fargate runner', {
-      labels: ['arm64', 'fargate'],
-      imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
-        architecture: Architecture.ARM64,
-        os: Os.LINUX,
+   providers: [
+      new FargateRunnerProvider(this, 'fargate runner', {
+         labels: ['arm64', 'fargate'],
+         imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
+            architecture: Architecture.ARM64,
+            os: Os.LINUX_UBUNTU,
+         }),
       }),
-    }),
-  ],
+   ],
 });
 ```
 
 ## Architecture
 
 ![Architecture diagram](architecture.svg)
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/setup.py` & `cloudsnorkel.cdk-github-runners-0.9.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-github-runners",
-    "version": "0.9.5",
+    "version": "0.9.6",
     "description": "CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-github-runners.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudsnorkel.cdk_github_runners",
         "cloudsnorkel.cdk_github_runners._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_github_runners._jsii": [
-            "cdk-github-runners@0.9.5.jsii.tgz"
+            "cdk-github-runners@0.9.6.jsii.tgz"
         ],
         "cloudsnorkel.cdk_github_runners": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/__init__.py` & `cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -52,53 +52,131 @@
 * ECS is useful when you want to control the infrastructure, like leaving the runner host running for faster startups
 * Lambda is useful for short jobs that can work within time, size and readonly system constraints
 
 You can also create your own provider by implementing `IRunnerProvider`.
 
 ## Installation
 
-1. Confirm you're using CDK v2
-2. Install the appropriate package
+1. Install and use the appropriate package
 
-   1. [Python](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
+   <details><summary>Python</summary>
 
-      ```
-      pip install cloudsnorkel.cdk-github-runners
-      ```
-   2. [TypeScript or JavaScript](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
-
-      ```
-      npm i @cloudsnorkel/cdk-github-runners
-      ```
-   3. [Java](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+   ### Install
 
-      ```xml
-      <dependency>
+   Available on [PyPI](https://pypi.org/project/cloudsnorkel.cdk-github-runners).
+
+   ```bash
+   pip install cloudsnorkel.cdk-github-runners
+   ```
+
+   ### Use
+
+   ```python
+   from cloudsnorkel.cdk_github_runners import GitHubRunners
+
+   GitHubRunners(self, "runners")
+   ```
+
+   </details>
+   <details><summary>TypeScript or JavaScript</summary>
+
+   ### Install
+
+   Available on [npm](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners).
+
+   ```bash
+   npm i @cloudsnorkel/cdk-github-runners
+   ```
+
+   ### Use
+
+   ```python
+   import { GitHubRunners } from '@cloudsnorkel/cdk-github-runners';
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+   <details><summary>Java</summary>
+
+   ### Install
+
+   Available on [Maven](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/).
+
+   ```xml
+   <dependency>
       <groupId>com.cloudsnorkel</groupId>
       <artifactId>cdk.github.runners</artifactId>
-      </dependency>
-      ```
-   4. [Go](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
-
-      ```
-      go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
-      ```
-   5. [.NET](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
-
-      ```
-      dotnet add package CloudSnorkel.Cdk.Github.Runners
-      ```
-3. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
-4. Deploy your stack
-5. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
-6. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
-7. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
-8. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
-9. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
-10. If the action is not successful, see [troubleshooting](#Troubleshooting)
+   </dependency>
+   ```
+
+   ### Use
+
+   ```java
+   import com.cloudsnorkel.cdk.github.runners.GitHubRunners;
+
+   GitHubRunners.Builder.create(this, "runners").build();
+   ```
+
+   </details>
+   <details><summary>Go</summary>
+
+   ### Install
+
+   Available on [GitHub](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners).
+
+   ```bash
+   go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
+   ```
+
+   ### Use
+
+   ```go
+   import "github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners"
+
+   NewGitHubRunners(this, jsii.String("runners"))
+   ```
+
+   </details>
+   <details><summary>.NET</summary>
+
+   ### Install
+
+   Available on [Nuget](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/).
+
+   ```bash
+   dotnet add package CloudSnorkel.Cdk.Github.Runners
+   ```
+
+   ### Use
+
+   ```csharp
+   using CloudSnorkel;
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+2. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
+3. Deploy your stack
+4. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
+
+   ```
+    ✅  github-runners-test
+
+   ✨  Deployment time: 260.01s
+
+   Outputs:
+   github-runners-test.runnersstatuscommand4A30F0F5 = aws --region us-east-1 lambda invoke --function-name github-runners-test-runnersstatus1A5771C0-mvttg8oPQnQS status.json
+   ```
+5. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
+6. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
+7. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
+8. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
+9. If the action is not successful, see [troubleshooting](#Troubleshooting)
 
 [![Demo](demo-thumbnail.jpg)](https://youtu.be/wlyv_3V8lIw)
 
 ## Customizing
 
 The default providers configured by `GitHubRunners` are useful for testing but probably not too much for actual production work. They run in the default VPC or no VPC and have no added IAM permissions. You would usually want to configure the providers yourself.
 
@@ -108,17 +186,17 @@
 let vpc: ec2.Vpc;
 let runnerSg: ec2.SecurityGroup;
 let dbSg: ec2.SecurityGroup;
 let bucket: s3.Bucket;
 
 // create a custom CodeBuild provider
 const myProvider = new CodeBuildRunnerProvider(this, 'codebuild runner', {
-  label: 'my-codebuild',
-  vpc: vpc,
-  securityGroup: runnerSg,
+   labels: ['my-codebuild'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
 });
 // grant some permissions to the provider
 bucket.grantReadWrite(myProvider);
 dbSg.connections.allowFrom(runnerSg, ec2.Port.tcp(3306), 'allow runners to connect to MySQL database');
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
@@ -135,17 +213,17 @@
    rebuildInterval: Duration.days(14),
 });
 myBuilder.addComponent(
   RunnerImageComponent.custom({ commands: ['apt install -y nginx xz-utils'] })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-   label: 'customized-fargate',
+   labels: ['customized-fargate'],
    vpc: vpc,
-   securityGroup: runnerSg,
+   securityGroups: [runnerSg],
    imageBuilder: myBuilder,
 });
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
    providers: [myProvider],
 });
@@ -163,55 +241,55 @@
       - run: echo hello world
 ```
 
 Windows images can also be customized the same way.
 
 ```python
 const myWindowsBuilder = FargateRunnerProvider.imageBuilder(this, 'Windows image builder', {
-  architecture: Architecture.X86_64,
-  os: Os.WINDOWS,
-  runnerVersion: RunnerVersion.specific('2.291.0'),
-  rebuildInterval: Duration.days(14),
+   architecture: Architecture.X86_64,
+   os: Os.WINDOWS,
+   runnerVersion: RunnerVersion.specific('2.291.0'),
+   rebuildInterval: Duration.days(14),
 });
 myWindowsBuilder.addComponent(
-  RunnerImageComponent.custom({
-    name: 'Ninja',
-    commands: [
-      'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
-      'Expand-Archive ninja.zip -DestinationPath C:\\actions',
-      'del ninja.zip',
-    ],
-  })
+        RunnerImageComponent.custom({
+           name: 'Ninja',
+           commands: [
+              'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
+              'Expand-Archive ninja.zip -DestinationPath C:\\actions',
+              'del ninja.zip',
+           ],
+        })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-  label: 'customized-windows-fargate',
-  vpc: vpc,
-  securityGroup: runnerSg,
-  imageBuidler: myWindowsBuilder,
+   labels: ['customized-windows-fargate'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
+   imageBuidler: myWindowsBuilder,
 });
 
 new GitHubRunners(this, 'runners', {
-  providers: [myProvider],
+   providers: [myProvider],
 });
 ```
 
 The runner OS and architecture is determined by the image it is set to use. For example, to create a Fargate runner provider for ARM64 set the `architecture` property for the image builder to `Architecture.ARM64` in the image builder properties.
 
 ```python
 new GitHubRunners(this, 'runners', {
-  providers: [
-    new FargateRunnerProvider(this, 'fargate runner', {
-      labels: ['arm64', 'fargate'],
-      imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
-        architecture: Architecture.ARM64,
-        os: Os.LINUX,
+   providers: [
+      new FargateRunnerProvider(this, 'fargate runner', {
+         labels: ['arm64', 'fargate'],
+         imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
+            architecture: Architecture.ARM64,
+            os: Os.LINUX_UBUNTU,
+         }),
       }),
-    }),
-  ],
+   ],
 });
 ```
 
 ## Architecture
 
 ![Architecture diagram](architecture.svg)
 
@@ -1411,20 +1489,20 @@
 
        const vpc = ec2.Vpc.fromLookup(this, 'vpc', { vpcId: 'vpc-1234567' });
        const runnerSg = new ec2.SecurityGroup(this, 'runner security group', { vpc: vpc });
        const dbSg = ec2.SecurityGroup.fromSecurityGroupId(this, 'database security group', 'sg-1234567');
        const bucket = new s3.Bucket(this, 'runner bucket');
 
        // create a custom CodeBuild provider
-       const myProvider = new CodeBuildRunner(
+       const myProvider = new CodeBuildRunnerProvider(
          this, 'codebuild runner',
          {
-            label: 'my-codebuild',
+            labels: ['my-codebuild'],
             vpc: vpc,
-            securityGroup: runnerSg,
+            securityGroups: [runnerSg],
          },
        );
        // grant some permissions to the provider
        bucket.grantReadWrite(myProvider);
        dbSg.connections.allowFrom(runnerSg, ec2.Port.tcp(3306), 'allow runners to connect to MySQL database');
 
        // create the runner infrastructure
@@ -3092,15 +3170,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -4153,15 +4231,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -4224,15 +4302,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -4451,15 +4529,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -4631,15 +4709,15 @@
         result = self._values.get("log_retention")
         return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays], result)
 
     @builtins.property
     def os(self) -> typing.Optional[Os]:
         '''(experimental) Image OS.
 
-        :default: OS.LINUX
+        :default: OS.LINUX_UBUNTU
 
         :stability: experimental
         '''
         result = self._values.get("os")
         return typing.cast(typing.Optional[Os], result)
 
     @builtins.property
@@ -5708,16 +5786,16 @@
          platform: 'Linux',
          displayName: 'p7zip',
          description: 'Install some more packages',
          commands: [
            'apt-get install p7zip',
          ],
        }));
-       new Ec2Runner(this, 'EC2 provider', {
-           label: 'custom-ec2',
+       new Ec2RunnerProvider(this, 'EC2 provider', {
+           labels: ['custom-ec2'],
            amiBuilder: builder,
        });
 
     :deprecated: use RunnerImageBuilder
 
     :stability: deprecated
     '''
@@ -6006,21 +6084,21 @@
     Each builder re-runs automatically at a set interval to make sure the images contain the latest versions of everything.
 
     You can create an instance of this construct to customize the image used to spin-up runners. Each provider has its own requirements for what an image should do. That's why they each provide their own Dockerfile.
 
     For example, to set a specific runner version, rebuild the image every 2 weeks, and add a few packages for the Fargate provider, use::
 
        const builder = new CodeBuildImageBuilder(this, 'Builder', {
-           dockerfilePath: FargateProvider.LINUX_X64_DOCKERFILE_PATH,
+           dockerfilePath: FargateRunnerProvider.LINUX_X64_DOCKERFILE_PATH,
            runnerVersion: RunnerVersion.specific('2.293.0'),
            rebuildInterval: Duration.days(14),
        });
        builder.setBuildArg('EXTRA_PACKAGES', 'nginx xz-utils');
-       new FargateRunner(this, 'Fargate provider', {
-           label: 'customized-fargate',
+       new FargateRunnerProvider(this, 'Fargate provider', {
+           labels: ['customized-fargate'],
            imageBuilder: builder,
        });
 
     :deprecated: use RunnerImageBuilder
 
     :stability: deprecated
     '''
@@ -6325,15 +6403,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -6861,16 +6939,16 @@
 
     For example, to set a specific runner version, rebuild the image every 2 weeks, and add a few packages for the Fargate provider, use::
 
        const builder = new ContainerImageBuilder(this, 'Builder', {
            runnerVersion: RunnerVersion.specific('2.293.0'),
            rebuildInterval: Duration.days(14),
        });
-       new CodeBuildRunner(this, 'CodeBuild provider', {
-           label: 'custom-codebuild',
+       new CodeBuildRunnerProvider(this, 'CodeBuild provider', {
+           labels: ['custom-codebuild'],
            imageBuilder: builder,
        });
 
     :deprecated: use RunnerImageBuilder
 
     :stability: deprecated
     '''
@@ -7185,15 +7263,15 @@
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         retry_options: typing.Optional[typing.Union[ProviderRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param ami_builder: 
-        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2ProviderProps.imageBuilder()
+        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2RunnerProvider.imageBuilder()
         :param instance_type: (experimental) Instance type for launched runner instances. Default: m5.large
         :param labels: (experimental) GitHub Actions labels used for this provider. These labels are used to identify which provider should spawn a new on-demand runner. Every job sends a webhook with the labels it's looking for based on runs-on. We match the labels from the webhook with the labels specified here. If all the labels specified here are present in the job's labels, this provider will be chosen and spawn a new runner. Default: ['ec2']
         :param security_group: (deprecated) Security Group to assign to launched runner instances. Default: a new security group
         :param security_groups: (experimental) Security groups to assign to launched runner instances. Default: a new security group
         :param spot: (experimental) Use spot instances to save money. Spot instances are cheaper but not always available and can be stopped prematurely. Default: false
         :param spot_max_price: (experimental) Set a maximum price for spot instances. Default: no max price (you will pay current spot price)
         :param storage_size: (experimental) Size of volume available for launched runner instances. This modifies the boot volume size and doesn't add any additional volumes. Default: 30GB
@@ -7270,15 +7348,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -7494,15 +7572,15 @@
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Properties for {@link Ec2RunnerProvider} construct.
 
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param retry_options: (experimental) Options to retry operation in case of failure like missing capacity, or API quota issues. Default: retry 10 times up to about 45 minutes
         :param ami_builder: 
-        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2ProviderProps.imageBuilder()
+        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2RunnerProvider.imageBuilder()
         :param instance_type: (experimental) Instance type for launched runner instances. Default: m5.large
         :param labels: (experimental) GitHub Actions labels used for this provider. These labels are used to identify which provider should spawn a new on-demand runner. Every job sends a webhook with the labels it's looking for based on runs-on. We match the labels from the webhook with the labels specified here. If all the labels specified here are present in the job's labels, this provider will be chosen and spawn a new runner. Default: ['ec2']
         :param security_group: (deprecated) Security Group to assign to launched runner instances. Default: a new security group
         :param security_groups: (experimental) Security groups to assign to launched runner instances. Default: a new security group
         :param spot: (experimental) Use spot instances to save money. Spot instances are cheaper but not always available and can be stopped prematurely. Default: false
         :param spot_max_price: (experimental) Set a maximum price for spot instances. Default: no max price (you will pay current spot price)
         :param storage_size: (experimental) Size of volume available for launched runner instances. This modifies the boot volume size and doesn't add any additional volumes. Default: 30GB
@@ -7602,15 +7680,15 @@
 
     @builtins.property
     def image_builder(self) -> typing.Optional[IRunnerImageBuilder]:
         '''(experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements.
 
         The image builder determines the OS and architecture of the runner.
 
-        :default: Ec2ProviderProps.imageBuilder()
+        :default: Ec2RunnerProvider.imageBuilder()
 
         :stability: experimental
         '''
         result = self._values.get("image_builder")
         return typing.cast(typing.Optional[IRunnerImageBuilder], result)
 
     @builtins.property
@@ -7889,15 +7967,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -8569,15 +8647,15 @@
         :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
-        :param os: (experimental) Image OS. Default: OS.LINUX
+        :param os: (experimental) Image OS. Default: OS.LINUX_UBUNTU
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_groups: (experimental) Security Groups to assign to this instance.
         :param subnet_selection: (experimental) Where to place the network interfaces within the VPC. Default: no subnet
         :param vpc: (experimental) VPC to build the image in. Default: no VPC
 
         :stability: experimental
@@ -9650,15 +9728,15 @@
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         retry_options: typing.Optional[typing.Union[ProviderRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param ami_builder: 
-        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2ProviderProps.imageBuilder()
+        :param image_builder: (experimental) Runner image builder used to build AMI containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: Ec2RunnerProvider.imageBuilder()
         :param instance_type: (experimental) Instance type for launched runner instances. Default: m5.large
         :param labels: (experimental) GitHub Actions labels used for this provider. These labels are used to identify which provider should spawn a new on-demand runner. Every job sends a webhook with the labels it's looking for based on runs-on. We match the labels from the webhook with the labels specified here. If all the labels specified here are present in the job's labels, this provider will be chosen and spawn a new runner. Default: ['ec2']
         :param security_group: (deprecated) Security Group to assign to launched runner instances. Default: a new security group
         :param security_groups: (experimental) Security groups to assign to launched runner instances. Default: a new security group
         :param spot: (experimental) Use spot instances to save money. Spot instances are cheaper but not always available and can be stopped prematurely. Default: false
         :param spot_max_price: (experimental) Set a maximum price for spot instances. Default: no max price (you will pay current spot price)
         :param storage_size: (experimental) Size of volume available for launched runner instances. This modifies the boot volume size and doesn't add any additional volumes. Default: 30GB
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.5
+Version: 0.9.6
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -75,53 +75,131 @@
 * ECS is useful when you want to control the infrastructure, like leaving the runner host running for faster startups
 * Lambda is useful for short jobs that can work within time, size and readonly system constraints
 
 You can also create your own provider by implementing `IRunnerProvider`.
 
 ## Installation
 
-1. Confirm you're using CDK v2
-2. Install the appropriate package
+1. Install and use the appropriate package
 
-   1. [Python](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
+   <details><summary>Python</summary>
 
-      ```
-      pip install cloudsnorkel.cdk-github-runners
-      ```
-   2. [TypeScript or JavaScript](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
-
-      ```
-      npm i @cloudsnorkel/cdk-github-runners
-      ```
-   3. [Java](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+   ### Install
 
-      ```xml
-      <dependency>
+   Available on [PyPI](https://pypi.org/project/cloudsnorkel.cdk-github-runners).
+
+   ```bash
+   pip install cloudsnorkel.cdk-github-runners
+   ```
+
+   ### Use
+
+   ```python
+   from cloudsnorkel.cdk_github_runners import GitHubRunners
+
+   GitHubRunners(self, "runners")
+   ```
+
+   </details>
+   <details><summary>TypeScript or JavaScript</summary>
+
+   ### Install
+
+   Available on [npm](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners).
+
+   ```bash
+   npm i @cloudsnorkel/cdk-github-runners
+   ```
+
+   ### Use
+
+   ```python
+   import { GitHubRunners } from '@cloudsnorkel/cdk-github-runners';
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+   <details><summary>Java</summary>
+
+   ### Install
+
+   Available on [Maven](https://central.sonatype.com/artifact/com.cloudsnorkel/cdk.github.runners/).
+
+   ```xml
+   <dependency>
       <groupId>com.cloudsnorkel</groupId>
       <artifactId>cdk.github.runners</artifactId>
-      </dependency>
-      ```
-   4. [Go](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
-
-      ```
-      go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
-      ```
-   5. [.NET](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
-
-      ```
-      dotnet add package CloudSnorkel.Cdk.Github.Runners
-      ```
-3. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
-4. Deploy your stack
-5. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
-6. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
-7. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
-8. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
-9. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
-10. If the action is not successful, see [troubleshooting](#Troubleshooting)
+   </dependency>
+   ```
+
+   ### Use
+
+   ```java
+   import com.cloudsnorkel.cdk.github.runners.GitHubRunners;
+
+   GitHubRunners.Builder.create(this, "runners").build();
+   ```
+
+   </details>
+   <details><summary>Go</summary>
+
+   ### Install
+
+   Available on [GitHub](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners).
+
+   ```bash
+   go get github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners
+   ```
+
+   ### Use
+
+   ```go
+   import "github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners"
+
+   NewGitHubRunners(this, jsii.String("runners"))
+   ```
+
+   </details>
+   <details><summary>.NET</summary>
+
+   ### Install
+
+   Available on [Nuget](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/).
+
+   ```bash
+   dotnet add package CloudSnorkel.Cdk.Github.Runners
+   ```
+
+   ### Use
+
+   ```csharp
+   using CloudSnorkel;
+
+   new GitHubRunners(this, "runners");
+   ```
+
+   </details>
+2. Use `GitHubRunners` construct in your code (starting with default arguments is fine)
+3. Deploy your stack
+4. Look for the status command output similar to `aws --region us-east-1 lambda invoke --function-name status-XYZ123 status.json`
+
+   ```
+    ✅  github-runners-test
+
+   ✨  Deployment time: 260.01s
+
+   Outputs:
+   github-runners-test.runnersstatuscommand4A30F0F5 = aws --region us-east-1 lambda invoke --function-name github-runners-test-runnersstatus1A5771C0-mvttg8oPQnQS status.json
+   ```
+5. Execute the status command (you may need to specify `--profile` too) and open the resulting `status.json` file
+6. Open the URL in `github.setup.url` from `status.json` or [manually setup GitHub](SETUP_GITHUB.md) integration as an app or with personal access token
+7. Run status command again to confirm `github.auth.status` and `github.webhook.status` are OK
+8. Trigger a GitHub action that has a `self-hosted` label with `runs-on: [self-hosted, linux, codebuild]` or similar
+9. If the action is not successful, see [troubleshooting](#Troubleshooting)
 
 [![Demo](demo-thumbnail.jpg)](https://youtu.be/wlyv_3V8lIw)
 
 ## Customizing
 
 The default providers configured by `GitHubRunners` are useful for testing but probably not too much for actual production work. They run in the default VPC or no VPC and have no added IAM permissions. You would usually want to configure the providers yourself.
 
@@ -131,17 +209,17 @@
 let vpc: ec2.Vpc;
 let runnerSg: ec2.SecurityGroup;
 let dbSg: ec2.SecurityGroup;
 let bucket: s3.Bucket;
 
 // create a custom CodeBuild provider
 const myProvider = new CodeBuildRunnerProvider(this, 'codebuild runner', {
-  label: 'my-codebuild',
-  vpc: vpc,
-  securityGroup: runnerSg,
+   labels: ['my-codebuild'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
 });
 // grant some permissions to the provider
 bucket.grantReadWrite(myProvider);
 dbSg.connections.allowFrom(runnerSg, ec2.Port.tcp(3306), 'allow runners to connect to MySQL database');
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
@@ -158,17 +236,17 @@
    rebuildInterval: Duration.days(14),
 });
 myBuilder.addComponent(
   RunnerImageComponent.custom({ commands: ['apt install -y nginx xz-utils'] })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-   label: 'customized-fargate',
+   labels: ['customized-fargate'],
    vpc: vpc,
-   securityGroup: runnerSg,
+   securityGroups: [runnerSg],
    imageBuilder: myBuilder,
 });
 
 // create the runner infrastructure
 new GitHubRunners(this, 'runners', {
    providers: [myProvider],
 });
@@ -186,55 +264,55 @@
       - run: echo hello world
 ```
 
 Windows images can also be customized the same way.
 
 ```python
 const myWindowsBuilder = FargateRunnerProvider.imageBuilder(this, 'Windows image builder', {
-  architecture: Architecture.X86_64,
-  os: Os.WINDOWS,
-  runnerVersion: RunnerVersion.specific('2.291.0'),
-  rebuildInterval: Duration.days(14),
+   architecture: Architecture.X86_64,
+   os: Os.WINDOWS,
+   runnerVersion: RunnerVersion.specific('2.291.0'),
+   rebuildInterval: Duration.days(14),
 });
 myWindowsBuilder.addComponent(
-  RunnerImageComponent.custom({
-    name: 'Ninja',
-    commands: [
-      'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
-      'Expand-Archive ninja.zip -DestinationPath C:\\actions',
-      'del ninja.zip',
-    ],
-  })
+        RunnerImageComponent.custom({
+           name: 'Ninja',
+           commands: [
+              'Invoke-WebRequest -UseBasicParsing -Uri "https://github.com/ninja-build/ninja/releases/download/v1.11.1/ninja-win.zip" -OutFile ninja.zip',
+              'Expand-Archive ninja.zip -DestinationPath C:\\actions',
+              'del ninja.zip',
+           ],
+        })
 );
 
 const myProvider = new FargateRunnerProvider(this, 'fargate runner', {
-  label: 'customized-windows-fargate',
-  vpc: vpc,
-  securityGroup: runnerSg,
-  imageBuidler: myWindowsBuilder,
+   labels: ['customized-windows-fargate'],
+   vpc: vpc,
+   securityGroups: [runnerSg],
+   imageBuidler: myWindowsBuilder,
 });
 
 new GitHubRunners(this, 'runners', {
-  providers: [myProvider],
+   providers: [myProvider],
 });
 ```
 
 The runner OS and architecture is determined by the image it is set to use. For example, to create a Fargate runner provider for ARM64 set the `architecture` property for the image builder to `Architecture.ARM64` in the image builder properties.
 
 ```python
 new GitHubRunners(this, 'runners', {
-  providers: [
-    new FargateRunnerProvider(this, 'fargate runner', {
-      labels: ['arm64', 'fargate'],
-      imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
-        architecture: Architecture.ARM64,
-        os: Os.LINUX,
+   providers: [
+      new FargateRunnerProvider(this, 'fargate runner', {
+         labels: ['arm64', 'fargate'],
+         imageBuidler: FargateRunnerProvider.imageBuilder(this, 'image builder', {
+            architecture: Architecture.ARM64,
+            os: Os.LINUX_UBUNTU,
+         }),
       }),
-    }),
-  ],
+   ],
 });
 ```
 
 ## Architecture
 
 ![Architecture diagram](architecture.svg)
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
 src/cloudsnorkel/cdk_github_runners/__init__.py
 src/cloudsnorkel/cdk_github_runners/py.typed
 src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
-src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.5.jsii.tgz
+src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.6.jsii.tgz
```

