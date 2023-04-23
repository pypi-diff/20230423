# Comparing `tmp/AIUT_RoboticsToolbox-0.0.0.1.tar.gz` & `tmp/AIUT_RoboticsToolbox-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\subjects\postgraduate\robotics\AIUTAPP\dist\tmpp5lt8ekc\AIUT_RoboticsToolbox-0.0.0.1.tar", last modified: Fri Mar 11 14:25:35 2022, max compression
+gzip compressed data, was "D:\subjects\postgraduate\robotics\AIUTAPP0002\dist\.tmp-szlurci_\AIUT_RoboticsToolbox-0.0.0.2.tar", last modified: Sun Apr 23 07:25:23 2023, max compression
```

## Comparing `AIUT_RoboticsToolbox-0.0.0.1.tar` & `AIUT_RoboticsToolbox-0.0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-03-11 14:25:35.426264 AIUT_RoboticsToolbox-0.0.0.1/
--rw-rw-rw-   0        0        0     1091 2022-03-11 09:15:32.000000 AIUT_RoboticsToolbox-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      660 2022-03-11 14:25:35.426264 AIUT_RoboticsToolbox-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2022-03-11 09:13:50.000000 AIUT_RoboticsToolbox-0.0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2022-03-11 09:04:24.000000 AIUT_RoboticsToolbox-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      672 2022-03-11 14:25:35.441892 AIUT_RoboticsToolbox-0.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-03-11 14:25:35.395012 AIUT_RoboticsToolbox-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-03-11 14:25:35.410640 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox/
--rw-rw-rw-   0        0        0     6958 2022-03-06 18:14:21.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox/Toolbox.py
--rw-rw-rw-   0        0        0        0 2022-03-06 18:20:23.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:25:35.426264 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/
--rw-rw-rw-   0        0        0      660 2022-03-11 14:25:35.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2022-03-11 14:25:35.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-11 14:25:35.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-03-11 14:25:35.000000 AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/
+-rw-rw-rw-   0        0        0     1091 2022-03-11 09:15:32.000000 AIUT_RoboticsToolbox-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      700 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2022-03-11 09:13:50.000000 AIUT_RoboticsToolbox-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0      633 2023-04-23 07:22:09.000000 AIUT_RoboticsToolbox-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      672 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.813674 AIUT_RoboticsToolbox-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/
+-rw-rw-rw-   0        0        0     7258 2023-04-23 07:12:05.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/Toolbox.py
+-rw-rw-rw-   0        0        0        0 2022-03-06 18:20:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/
+-rw-rw-rw-   0        0        0      700 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/top_level.txt
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.1/LICENSE` & `AIUT_RoboticsToolbox-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AIUT_RoboticsToolbox-0.0.0.1/PKG-INFO` & `AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
-Name: AIUT_RoboticsToolbox
-Version: 0.0.0.1
-Summary: a robotics toolbox
+Name: AIUT-RoboticsToolbox
+Version: 0.0.0.2
+Summary: A simple Robotics package
 Home-page: https://github.com/pypa/AIUT_RoboticsToolBox
 Author: Maziar Palhang
-Author-email: palhang@cc.iut.ac.ir
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pypa/AIUT_RoboticsToolBox/issues
-Platform: UNKNOWN
+Author-email: Maziar Palhang <palhang@cc.iut.ac.ir>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Robotics Toolbox from Maziar Palhang
 
 This is a simple Robotics Toolbox package.
-
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.1/setup.cfg` & `AIUT_RoboticsToolbox-0.0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox/Toolbox.py` & `AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/Toolbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #In the Name of Allah
 # programmer : Maziar Palhang
 # First Edit : Wed. 1399/12/6
-# Last  Edit : Thu. 1400/12/12
+# Last  Edit : Thu. 1402/2/3
 
 import math
 from scipy.linalg import logm, expm
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.mplot3d import axes3d
 import matplotlib.pyplot as plt
@@ -181,26 +181,33 @@
         fig = plt.figure(1)
         ax = fig.gca(projection='3d')
         TT = np.eye(4)
         for i in range(np.size(self.links,0)):
             To = TT
             TT = TT.dot(self.makeT(self.links[i]))
             ax.plot3D([To[0][3],TT[0][3]],[To[1][3],TT[1][3]],[To[2][3],TT[2][3]])
-        ax.plot3D([TT[0][3],TT[0][3]+3*TT[0][0]],
-                  [TT[1][3],TT[1][3]+3*TT[1][0]],
-                  [TT[2][3],TT[2][3]+3*TT[2][0]])
-        ax.plot3D([TT[0][3],TT[0][3]+3*TT[0][1]],
-                  [TT[1][3],TT[1][3]+3*TT[1][1]],
-                  [TT[2][3],TT[2][3]+3*TT[2][1]],'g')
-        ax.plot3D([TT[0][3],TT[0][3]+3*TT[0][2]],
-                  [TT[1][3],TT[1][3]+3*TT[1][2]],
-                  [TT[2][3],TT[2][3]+3*TT[2][2]],'b')
-        ax.set_xlim(-1, 90)
-        ax.set_ylim(-1, 50)
-        ax.set_zlim(-50, 10)
+        ax.plot3D([TT[0][3],TT[0][3]+2*TT[0][0]],
+                  [TT[1][3],TT[1][3]+2*TT[1][0]],
+                  [TT[2][3],TT[2][3]+2*TT[2][0]])
+        ax.plot3D([TT[0][3],TT[0][3]+2*TT[0][1]],
+                  [TT[1][3],TT[1][3]+2*TT[1][1]],
+                  [TT[2][3],TT[2][3]+2*TT[2][1]],'g')
+        ax.plot3D([TT[0][3],TT[0][3]+2*TT[0][2]],
+                  [TT[1][3],TT[1][3]+2*TT[1][2]],
+                  [TT[2][3],TT[2][3]+2*TT[2][2]],'b')
+
+        minAll = min(TT[0][3],TT[1][3],TT[2][3])
+        maxAll = max(TT[0][3],TT[1][3],TT[2][3])
+        ax.plot3D([0, 0],[0,0],[0,minAll-1],'y')
+        #ax.set_xlim(-1, TT[0][3]+5)
+        #ax.set_ylim(-1, TT[1][3]+5)
+        #ax.set_zlim(-50, TT[2][3]+5)
+        ax.set_xlim(minAll-1, maxAll+1)
+        ax.set_ylim(minAll-1, maxAll+1)
+        ax.set_zlim(minAll-1, maxAll+1)
         ax.set_xlabel('x')
         ax.set_ylabel('y')
         ax.set_zlabel('z')
         plt.title(self.name)
         #ax.view_init(30, 60)
         plt.show()
         return
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.1/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO` & `AIUT_RoboticsToolbox-0.0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
-Name: AIUT-RoboticsToolbox
-Version: 0.0.0.1
-Summary: a robotics toolbox
+Name: AIUT_RoboticsToolbox
+Version: 0.0.0.2
+Summary: A simple Robotics package
 Home-page: https://github.com/pypa/AIUT_RoboticsToolBox
 Author: Maziar Palhang
-Author-email: palhang@cc.iut.ac.ir
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pypa/AIUT_RoboticsToolBox/issues
-Platform: UNKNOWN
+Author-email: Maziar Palhang <palhang@cc.iut.ac.ir>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Robotics Toolbox from Maziar Palhang
 
 This is a simple Robotics Toolbox package.
-
```

