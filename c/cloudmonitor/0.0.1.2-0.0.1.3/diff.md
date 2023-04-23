# Comparing `tmp/cloudmonitor-0.0.1.2.tar.gz` & `tmp/cloudmonitor-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmonitor-0.0.1.2.tar", last modified: Tue Apr 18 16:25:37 2023, max compression
+gzip compressed data, was "cloudmonitor-0.0.1.3.tar", last modified: Sun Apr 23 13:36:17 2023, max compression
```

## Comparing `cloudmonitor-0.0.1.2.tar` & `cloudmonitor-0.0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 15:27:26.000000 cloudmonitor-0.0.1.2/README.md
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-18 16:24:18.000000 cloudmonitor-0.0.1.2/cloudmonitor/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       59 2023-04-18 16:06:41.000000 cloudmonitor-0.0.1.2/cloudmonitor/__main__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1578 2023-04-18 12:09:13.000000 cloudmonitor-0.0.1.2/cloudmonitor/config.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/gpu/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       43 2023-04-18 15:23:00.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      277 2023-04-18 15:09:47.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/define.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1065 2023-04-18 16:00:25.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/query.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2611 2023-04-18 16:06:26.000000 cloudmonitor-0.0.1.2/cloudmonitor/server.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/ssh/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-18 15:28:12.000000 cloudmonitor-0.0.1.2/cloudmonitor/ssh/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      482 2023-04-18 15:00:34.000000 cloudmonitor-0.0.1.2/cloudmonitor/ssh/client.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      470 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       52 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/entry_points.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       33 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/requires.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/top_level.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/setup.cfg
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2488 2023-04-18 15:58:03.000000 cloudmonitor-0.0.1.2/setup.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 15:27:26.000000 cloudmonitor-0.0.1.3/README.md
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/cloudmonitor/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       50 2023-04-23 13:36:08.000000 cloudmonitor-0.0.1.3/cloudmonitor/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/__main__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2683 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/config.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2008 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/server.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/cloudmonitor/ssh/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/ssh/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1126 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/ssh/client.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/cloudmonitor/status/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/status/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/status/define.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.3/cloudmonitor/status/query.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      479 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       51 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/requires.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-23 13:36:17.000000 cloudmonitor-0.0.1.3/cloudmonitor.egg-info/top_level.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-23 13:36:17.296536 cloudmonitor-0.0.1.3/setup.cfg
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2502 2023-04-23 13:18:53.000000 cloudmonitor-0.0.1.3/setup.py
```

### Comparing `cloudmonitor-0.0.1.2/PKG-INFO` & `cloudmonitor-0.0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A Web-GUI Monitor for Academic Linux Servers
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cloudmonitor-0.0.1.2/cloudmonitor/server.py` & `cloudmonitor-0.0.1.3/cloudmonitor/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,72 @@
 from flask import Flask, render_template, jsonify
 import time
 import argparse, yaml
 import logging
 import functools
 from datetime import datetime, timedelta
-from .config import C
-from .gpu import update_gpu
+from .config import C, load_config, load_args
+from .status import update_servers
 
 __all__ = ["main"]
 
 app = Flask(__name__)
 parser = argparse.ArgumentParser(
-    prog='Cloud Monitor',
-    description='A Web-GUI for monitoring servers',
+    prog="Cloud Monitor",
+    description="A Web-GUI for monitoring servers",
     # epilog='Text at the bottom of help'
 )
-parser.add_argument('-c', "--config", dest="config", required=True,  type=str, help='path of YAML config file')
-parser.add_argument('-p', "--port",   dest="port",   required=False, default=8899, type=int, help='port for Web GUI')
+parser.add_argument("-c", "--config", dest="config", required=True, type=str, help="path of YAML config file")
+parser.add_argument("-p", "--port", dest="port", required=False, default=8899, type=int, help="port for Web GUI")
+parser.add_argument(
+    "-w", "--workers", dest="workers", required=False, default=4, type=int, help="number of multi-process workers"
+)
 args = parser.parse_args()
+load_args(args)
+if not load_config(args.config):
+    exit(0)
+
 
 def cache(seconds: int, maxsize: int = 128, typed: bool = False):
     def wrapper_cache(func):
         func = functools.lru_cache(maxsize=maxsize, typed=typed)(func)
         func.delta = timedelta(seconds=seconds)
         func.expiration = datetime.utcnow() + func.delta
+
         @functools.wraps(func)
         def wrapped_func(*args, **kwargs):
             if datetime.utcnow() >= func.expiration:
                 func.cache_clear()
                 func.expiration = datetime.utcnow() + func.delta
             return func(*args, **kwargs)
+
         return wrapped_func
+
     return wrapper_cache
 
 
-@app.route('/')
+@app.route("/")
 def hello_world():
-    return render_template("index.html")
+    status()
+    return render_template(os.path.join(C.root_path, "index.html"), servers=C.status)
 
-@app.route('/reload')
+
+@app.route("/reload")
 def reload():
-    if not load_config(args.config): return "Error! Please see logs."
+    if not load_config(args.config):
+        return "Error! Please see logs."
     return "Config reloaded."
 
-@app.route('/gpu')
-@cache(seconds=C.gpu_refresh)
-def gpu_status():
-    C.gpus = update_gpu(C.servers)
-    return jsonify(C.gpus)
-
-def load_config(path):
-    try:
-        with open(args.config, 'r', encoding='utf-8') as fr:
-            config = yaml.load(fr, yaml.FullLoader)
-            # Apply config files to config
-            C.servers = config["servers"]
-            if "gpu_refresh" in config: C.gpu_refresh = float(config["gpu_refresh"])
-            
-        # Set default key-value in config
-        for server_name in C.servers:
-            if "port" not in C.servers[server_name]:
-                C.servers[server_name]["port"] = 22
-            if "rank" not in C.servers[server_name]:
-                C.servers[server_name]["rank"] = 999
-            if "path" not in C.servers[server_name]:
-                C.servers[server_name]["path"] = ["/"]
-    except Exception as err:
-        logging.error(f"[CONFIG] Load config error: {err}.")
-        return False
-    return True
+
+@app.route("/status")
+@cache(seconds=C.refresh)
+def status():
+    C.status = update_servers(C.servers)
+    return jsonify(C.status)
+
 
 def main():
-    if not load_config(args.config): exit(0)
-    app.run(host='127.0.0.1', port=args.port, debug=True)
+    app.run(host="0.0.0.0", port=C.port, debug=True)
+
 
-if __name__ == "__main__": main()
-    
+if __name__ == "__main__":
+    main()
```

### Comparing `cloudmonitor-0.0.1.2/cloudmonitor.egg-info/PKG-INFO` & `cloudmonitor-0.0.1.3/cloudmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A Web-GUI Monitor for Academic Linux Servers
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cloudmonitor-0.0.1.2/setup.py` & `cloudmonitor-0.0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 # not sure about setuptools).
 if os.path.exists("MANIFEST"):
     os.remove("MANIFEST")
 
 # What packages are required for this module to be executed?
 # `estimator` may depend on other packages. In order to reduce dependencies, it is not written here.
 REQUIRED = [
-    "numpy>=1.12.0, <1.24",
-    "flask>=2.2.2"
+    "flask>=2.2.2",
+    "paramiko>=3.0.0",
+    "pyyaml>=6.0",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
@@ -65,11 +66,11 @@
             # "Operating System :: MacOS",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
         ],
         entry_points={
             'console_scripts': [
-                'cloud-monitor = cloudmonitor:main',
+                'cloudmonitor = cloudmonitor:main',
             ]
         }
     )
```

