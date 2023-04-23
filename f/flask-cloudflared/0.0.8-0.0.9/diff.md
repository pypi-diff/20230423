# Comparing `tmp/flask_cloudflared-0.0.8.tar.gz` & `tmp/flask_cloudflared-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cloudflared-0.0.8.tar", last modified: Wed Apr 13 07:22:37 2022, max compression
+gzip compressed data, was "flask_cloudflared-0.0.9.tar", last modified: Fri May 20 21:07:22 2022, max compression
```

## Comparing `flask_cloudflared-0.0.8.tar` & `flask_cloudflared-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ralfrademacher   (501) staff       (20)        0 2022-04-13 07:22:37.855229 flask_cloudflared-0.0.8/
--rw-r--r--   0 ralfrademacher   (501) staff       (20)      552 2022-04-12 10:44:31.000000 flask_cloudflared-0.0.8/LICENSE
--rw-r--r--   0 ralfrademacher   (501) staff       (20)     3685 2022-04-13 07:22:37.855040 flask_cloudflared-0.0.8/PKG-INFO
--rw-r--r--   0 ralfrademacher   (501) staff       (20)     3197 2022-04-12 12:50:25.000000 flask_cloudflared-0.0.8/README.md
-drwxr-xr-x   0 ralfrademacher   (501) staff       (20)        0 2022-04-13 07:22:37.854784 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/
--rw-r--r--   0 ralfrademacher   (501) staff       (20)     3685 2022-04-13 07:22:37.000000 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/PKG-INFO
--rw-r--r--   0 ralfrademacher   (501) staff       (20)      251 2022-04-13 07:22:37.000000 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/SOURCES.txt
--rw-r--r--   0 ralfrademacher   (501) staff       (20)        1 2022-04-13 07:22:37.000000 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/dependency_links.txt
--rw-r--r--   0 ralfrademacher   (501) staff       (20)       20 2022-04-13 07:22:37.000000 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/requires.txt
--rw-r--r--   0 ralfrademacher   (501) staff       (20)       18 2022-04-13 07:22:37.000000 flask_cloudflared-0.0.8/flask_cloudflared.egg-info/top_level.txt
--rw-r--r--   0 ralfrademacher   (501) staff       (20)     6595 2022-04-13 07:21:58.000000 flask_cloudflared-0.0.8/flask_cloudflared.py
--rw-r--r--   0 ralfrademacher   (501) staff       (20)       38 2022-04-13 07:22:37.855299 flask_cloudflared-0.0.8/setup.cfg
--rw-r--r--   0 ralfrademacher   (501) staff       (20)      723 2022-04-13 07:21:58.000000 flask_cloudflared-0.0.8/setup.py
+drwxr-xr-x   0 ralfrademacher   (501) staff       (20)        0 2022-05-20 21:07:22.134540 flask_cloudflared-0.0.9/
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)      552 2022-04-12 10:44:31.000000 flask_cloudflared-0.0.9/LICENSE
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)     3648 2022-05-20 21:07:22.134337 flask_cloudflared-0.0.9/PKG-INFO
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)     3197 2022-04-12 12:50:25.000000 flask_cloudflared-0.0.9/README.md
+drwxr-xr-x   0 ralfrademacher   (501) staff       (20)        0 2022-05-20 21:07:22.134068 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)     3648 2022-05-20 21:07:21.000000 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/PKG-INFO
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)      251 2022-05-20 21:07:22.000000 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/SOURCES.txt
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)        1 2022-05-20 21:07:21.000000 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/dependency_links.txt
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)       20 2022-05-20 21:07:22.000000 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/requires.txt
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)       18 2022-05-20 21:07:22.000000 flask_cloudflared-0.0.9/flask_cloudflared.egg-info/top_level.txt
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)     6594 2022-05-20 21:05:30.000000 flask_cloudflared-0.0.9/flask_cloudflared.py
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)       38 2022-05-20 21:07:22.134613 flask_cloudflared-0.0.9/setup.cfg
+-rw-r--r--   0 ralfrademacher   (501) staff       (20)      723 2022-05-20 21:05:55.000000 flask_cloudflared-0.0.9/setup.py
```

### Comparing `flask_cloudflared-0.0.8/LICENSE` & `flask_cloudflared-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cloudflared-0.0.8/PKG-INFO` & `flask_cloudflared-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: flask_cloudflared
-Version: 0.0.8
+Version: 0.0.9
 Summary: Start a TryCloudflare Tunnel from your flask app.
 Home-page: https://github.com/UWUplus/flask-cloudflared
 Author: Ralf Rademacher
-License: UNKNOWN
 Keywords: flask cloudflared
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flask-cloudflared
@@ -22,9 +20,7 @@
 
 ### Users on Apple Silicon
 Because [cloudflared](https://github.com/cloudflare/cloudflared) doesn't support Darwin arm64 natively yet, Rosetta 2 is used to create a compatibility layer. If you don't have Rosetta 2 installed yet, please check [Apple's support page](https://support.apple.com/en-us/HT211861).
 
 ## Acknowledgements
 
 This project is based on [flask-ngrok](https://github.com/gstaff/flask-ngrok).
-
-
```

### Comparing `flask_cloudflared-0.0.8/README.md` & `flask_cloudflared-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flask_cloudflared-0.0.8/flask_cloudflared.egg-info/PKG-INFO` & `flask_cloudflared-0.0.9/flask_cloudflared.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: flask-cloudflared
-Version: 0.0.8
+Version: 0.0.9
 Summary: Start a TryCloudflare Tunnel from your flask app.
 Home-page: https://github.com/UWUplus/flask-cloudflared
 Author: Ralf Rademacher
-License: UNKNOWN
 Keywords: flask cloudflared
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flask-cloudflared
@@ -22,9 +20,7 @@
 
 ### Users on Apple Silicon
 Because [cloudflared](https://github.com/cloudflare/cloudflared) doesn't support Darwin arm64 natively yet, Rosetta 2 is used to create a compatibility layer. If you don't have Rosetta 2 installed yet, please check [Apple's support page](https://support.apple.com/en-us/HT211861).
 
 ## Acknowledgements
 
 This project is based on [flask-ngrok](https://github.com/gstaff/flask-ngrok).
-
-
```

### Comparing `flask_cloudflared-0.0.8/flask_cloudflared.py` & `flask_cloudflared-0.0.9/flask_cloudflared.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             update_cloudflared = subprocess.Popen(['arch', '-x86_64', (cloudflared_path+'/'+'cloudflared'), 'update'], stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         elif system == "Darwin" and machine == "x86_64":
             update_cloudflared = subprocess.Popen([(cloudflared_path+'/'+'cloudflared'), 'update'], stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         else:
             update_cloudflared = subprocess.Popen([(cloudflared_path+'/'+command), 'update'], stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         return
     if system == "Windows":
-        if machine == "x86_64":
+        if machine == "AMD64":
             url = "https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-amd64.exe"
         elif machine == "i386":
             url = "https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-386.exe"
     elif system == "Linux":
         if machine == "x86_64":
             url = "https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64"
         elif machine == "i386":
```

### Comparing `flask_cloudflared-0.0.8/setup.py` & `flask_cloudflared-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flask_cloudflared",
-    version="0.0.8",
+    version="0.0.9",
     author="Ralf Rademacher",
     description="Start a TryCloudflare Tunnel from your flask app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UWUplus/flask-cloudflared",
     classifiers=[
         "Programming Language :: Python :: 3.6",
```

