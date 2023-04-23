# Comparing `tmp/crowdcores-node-1.1.3.tar.gz` & `tmp/crowdcores-node-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.1.3.tar", last modified: Fri Apr 21 23:20:28 2023, max compression
+gzip compressed data, was "crowdcores-node-1.1.4.tar", last modified: Sun Apr 23 00:47:59 2023, max compression
```

## Comparing `crowdcores-node-1.1.3.tar` & `crowdcores-node-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:20:28.096267 crowdcores-node-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-21 23:20:28.092267 crowdcores-node-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-21 16:43:57.000000 crowdcores-node-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:20:28.092267 crowdcores-node-1.1.3/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.3/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-04-21 22:13:23.000000 crowdcores-node-1.1.3/crowdcores_node/crowdcores_node.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-04-19 22:09:24.000000 crowdcores-node-1.1.3/crowdcores_node/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:20:28.092267 crowdcores-node-1.1.3/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-21 23:20:28.000000 crowdcores-node-1.1.3/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 23:20:28.096267 crowdcores-node-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-21 23:19:46.000000 crowdcores-node-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:47:59.280064 crowdcores-node-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-23 00:47:59.280064 crowdcores-node-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-21 16:43:57.000000 crowdcores-node-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:47:59.280064 crowdcores-node-1.1.4/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.4/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-04-23 00:32:24.000000 crowdcores-node-1.1.4/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-04-23 00:44:23.000000 crowdcores-node-1.1.4/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 00:47:59.280064 crowdcores-node-1.1.4/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 00:47:59.000000 crowdcores-node-1.1.4/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 00:47:59.280064 crowdcores-node-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-23 00:47:45.000000 crowdcores-node-1.1.4/setup.py
```

### Comparing `crowdcores-node-1.1.3/LICENSE.txt` & `crowdcores-node-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.3/README.md` & `crowdcores-node-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.3/crowdcores_node/crowdcores_node.py` & `crowdcores-node-1.1.4/crowdcores_node/crowdcores_node.py`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.3/crowdcores_node/manager.py` & `crowdcores-node-1.1.4/crowdcores_node/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import subprocess
 import os
 import time
 import signal
+import psutil
 
 
 node_out_put_file="/tmp/crowdcores_log.txt"
 
 #os.environ["PYTHONUNBUFFERED"] = "1"
 def start():
     pid = get_pid()
@@ -32,15 +33,20 @@
     if pid:
         os.kill(pid, signal.SIGTERM)
         print("CrowdCore Node Stopped...")
     else:
         print("CrowdCore Node is not running.")
 
 def connect():
-    print("Connecting to CrowdCore Node...")
+    if get_pid():
+        print("CrowdCore Node is currently running...")
+        print("Connecting to CrowdCore Node...")
+    else:
+        print("CrowdCore Node is not running. Any logs below are probably from a previous run.")
+        print("Showing CrowdCore Node logs...")
     with open(node_out_put_file, 'r') as f:
         while True:
             line = f.readline().strip()
             if line:
                 print(line)
             else:
                 time.sleep(0.1)
@@ -48,45 +54,21 @@
 
 def update():
     subprocess.call(['pip', 'install', '--upgrade','--no-deps', 'crowdcores-node'])
 
 def restart():
     stop();
     start();
-#
-##print("Connecting to service...")
-##pid = get_pid()
-##if not pid:
-##    print("Service is not running.")
-##    return
-##process = subprocess.Popen(["tail", "-f", f"/proc/{pid}/fd/1"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-##for line in iter(process.stdout.readline, b''):
-##    print(line.decode("utf-8").strip())
-     
-
-  ##for line in iter(process.stdout.readline, b''):
-  ##    print("got a line");
-  ##    print(line.decode("utf-8").strip())
 
 def get_pid():
-    process = subprocess.Popen(["pgrep", "-f", "crowdcores_node.py"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    pid, error = process.communicate()
-    if not pid:
-        return None
-    pid = pid.decode("utf-8").strip()
-    return int(pid)
-
-##  def get_pid():
-##      process = subprocess.Popen(["pgrep", "-f", "my_script.py"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
-##      pid, error = process.communicate()
-##      if not pid:
-##          return None
-##      pid = pid.decode("utf-8").strip()
-##      pids = pid.split('\n')
-##      return int(pids[0])
+    for proc in psutil.process_iter():
+        # concatenate the cmdline elements into a single string to search for crowdcores_node.py
+        if 'crowdcores_node.py' in ' '.join(proc.cmdline()):
+            return proc.pid
+    return None
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('action', choices=['start', 'stop', 'restart', 'update','connect'], help='Action to perform')
     args = parser.parse_args()
```

