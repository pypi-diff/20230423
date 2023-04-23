# Comparing `tmp/systems_manager-0.8.0-py2.py3-none-any.whl.zip` & `tmp/systems_manager-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 22086 bytes, number of entries: 9
+Zip file size: 22185 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      335 b- defN 23-Apr-14 02:11 systems_manager/__init__.py
--rw-r--r--  2.0 unx    32644 b- defN 23-Apr-14 03:34 systems_manager/systems_manager.py
--rw-r--r--  2.0 unx      116 b- defN 23-Apr-14 03:34 systems_manager/version.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2359 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      788 b- defN 23-Apr-14 03:34 systems_manager-0.8.0.dist-info/RECORD
-9 files, 71591 bytes uncompressed, 20712 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx    32905 b- defN 23-Apr-23 19:26 systems_manager/systems_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-23 19:26 systems_manager/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2359 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      788 b- defN 23-Apr-23 19:27 systems_manager-0.9.0.dist-info/RECORD
+9 files, 71852 bytes uncompressed, 20811 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: systems_manager/systems_manager.py
 Comment: 
 
 Filename: systems_manager/version.py
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/LICENSE
+Filename: systems_manager-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/METADATA
+Filename: systems_manager-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/WHEEL
+Filename: systems_manager-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/entry_points.txt
+Filename: systems_manager-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/top_level.txt
+Filename: systems_manager-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: systems_manager-0.8.0.dist-info/RECORD
+Filename: systems_manager-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## systems_manager/systems_manager.py

```diff
@@ -6,14 +6,15 @@
 import subprocess
 import os
 import platform
 import requests
 import zipfile
 import glob
 import json
+from systems_manager.version import __version__, __author__, __credits__
 
 
 class SystemsManager:
     def __init__(self, silent=False):
         self.system = platform.system()
         self.release = platform.release()
         self.version = platform.version()
@@ -514,25 +515,29 @@
             self.python_modules = modules
 
         for module in self.python_modules:
             self.install_python_modules_command.append(['python', '-m', 'pip', 'install', '--upgrade', f'{module}'])
 
 
 def usage():
-    print(f"Usage: \n"
+    print(f'Systems-Manager: A tool to manage your systems software!\n'
+          f'Version: {__version__}\n'
+          f'Author: {__author__}\n'
+          f'Credits: {__credits__}\n'
+          f"\nUsage: \n"
           f"-h | --help            [ See usage for script ]\n"
           f"-c | --clean           [ Clean Recycle/Trash bin ]\n"
           f"-e | --enable-features [ Enable Window Features ]\n"
           f"-f | --font            [ Install Hack NF Font ]\n"
           f"-i | --install         [ Install applications ]\n"
           f"-p | --python          [ Install Python Modules ]\n"
           f"-s | --silent          [ Don't print to stdout ]\n"
           f"-t | --theme           [ Apply Takuyuma Terminal Theme ]\n"
           f"-u | --update          [ Update your applications and Operating System ]\n"
-          f"Example: \n"
+          f"\nExample: \n"
           f"systems-manager --font --update --clean --theme --python 'geniusbot' --install 'python3'\n")
 
 
 def systems_manager(argv):
     system_manager_instance = SystemsManager()
     applications = []
     features = []
```

## systems_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `systems_manager-0.8.0.dist-info/LICENSE` & `systems_manager-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `systems_manager-0.8.0.dist-info/METADATA` & `systems_manager-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systems-manager
-Version: 0.8.0
+Version: 0.9.0
 Summary: Systems-Manager will update your system and install/upgrade applications.
 Home-page: https://github.com/Knuckles-Team/systems-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
 
 # Systems-Manager
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 Systems-Manager will update your system and install/upgrade applications.
 
 ### Usage:
 | Short Flag | Long Flag         | Description                                   |
 |------------|-------------------|-----------------------------------------------|
 | -h         | --help            | See usage for script                          |
```

## Comparing `systems_manager-0.8.0.dist-info/RECORD` & `systems_manager-0.9.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 systems_manager/__init__.py,sha256=uWwoY0W8q86L6py_9DSgjxt8bqy6jRmJ_BbzEU9mVSU,335
-systems_manager/systems_manager.py,sha256=R6qRyANUL1zIvMoZpkijy9lBDGjNJ_fyR2pcwUEb2Rc,32644
-systems_manager/version.py,sha256=tDDkCMChiJvcYngqfjlW_EaRz0JpbXA3z7tYvqWYe8M,116
-systems_manager-0.8.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-systems_manager-0.8.0.dist-info/METADATA,sha256=TUi5LbgBO_OJJCBchczVUzaBLP8vbCxVtYUEFdSimUo,2359
-systems_manager-0.8.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-systems_manager-0.8.0.dist-info/entry_points.txt,sha256=nw6W7EqOUK-gVmX8o1T12ZFBysvpt0aXWat9rNzpP58,74
-systems_manager-0.8.0.dist-info/top_level.txt,sha256=4BlAsWtCOTIoxPSPyeacWxqt0ahm5qbO4sgcOvHQ-RI,16
-systems_manager-0.8.0.dist-info/RECORD,,
+systems_manager/systems_manager.py,sha256=nHE8VPb6furSiK9FOWknRVfEH2PqPHeMYZ8hQSqnlwM,32905
+systems_manager/version.py,sha256=swhRnSKFIqDu9_CTMLtKcx393Adi5vpxEYYazFr8kkE,116
+systems_manager-0.9.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+systems_manager-0.9.0.dist-info/METADATA,sha256=uD7iQ6g5OAnnkPeU8XrpcxqeXUP5VZ2_uFHvM4J6E-I,2359
+systems_manager-0.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+systems_manager-0.9.0.dist-info/entry_points.txt,sha256=nw6W7EqOUK-gVmX8o1T12ZFBysvpt0aXWat9rNzpP58,74
+systems_manager-0.9.0.dist-info/top_level.txt,sha256=4BlAsWtCOTIoxPSPyeacWxqt0ahm5qbO4sgcOvHQ-RI,16
+systems_manager-0.9.0.dist-info/RECORD,,
```

