# Comparing `tmp/mechanical_bull-0.0.5.tar.gz` & `tmp/mechanical_bull-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanical_bull-0.0.5.tar", max compression
+gzip compressed data, was "mechanical_bull-0.0.6.tar", max compression
```

## Comparing `mechanical_bull-0.0.5.tar` & `mechanical_bull-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1062 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/LICENSE
--rw-r--r--   0        0        0     3161 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-18 13:15:41.978646 mechanical_bull-0.0.5/mechanical_bull/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:15:41.978646 mechanical_bull-0.0.5/mechanical_bull/actions/__init__.py
--rw-r--r--   0        0        0      196 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1206 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0      930 2023-04-18 13:16:06.362846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
--rw-r--r--   0        0        0     1236 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0     1985 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      491 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/accept_follow_request.py
--rw-r--r--   0        0        0      225 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/log_to_file.py
--rw-r--r--   0        0        0      521 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/reject_follow_request.py
--rw-r--r--   0        0        0      847 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/test_accept_reject_follow_request.py
--rw-r--r--   0        0        0     1362 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/add_user.py
--rw-r--r--   0        0        0      787 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/event_loop.py
--rw-r--r--   0        0        0      335 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/handlers.py
--rw-r--r--   0        0        0      685 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/run.py
--rw-r--r--   0        0        0      542 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/test_event_loop.py
--rw-r--r--   0        0        0      484 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/test_handlers.py
--rw-r--r--   0        0        0      683 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 mechanical_bull-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3110 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 12:23:50.009197 mechanical_bull-0.0.6/mechanical_bull/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 12:23:50.009197 mechanical_bull-0.0.6/mechanical_bull/actions/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-23 12:24:23.137503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1206 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0      930 2023-04-23 12:24:23.153503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0     1985 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      491 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/accept_follow_request.py
+-rw-r--r--   0        0        0      225 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/log_to_file.py
+-rw-r--r--   0        0        0      521 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/reject_follow_request.py
+-rw-r--r--   0        0        0      847 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/test_accept_reject_follow_request.py
+-rw-r--r--   0        0        0     1604 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/add_user.py
+-rw-r--r--   0        0        0      787 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/event_loop.py
+-rw-r--r--   0        0        0      335 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/handlers.py
+-rw-r--r--   0        0        0      685 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/run.py
+-rw-r--r--   0        0        0      542 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/test_event_loop.py
+-rw-r--r--   0        0        0      484 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/test_handlers.py
+-rw-r--r--   0        0        0      896 2023-04-23 12:23:49.937196 mechanical_bull-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mechanical_bull-0.0.6/PKG-INFO
```

### Comparing `mechanical_bull-0.0.5/LICENSE` & `mechanical_bull-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/README.md` & `mechanical_bull-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ```bash
 pip install mechanical-bull
 ```
 
 Once can then add a new user by running
 
 ```bash
-python -m mechanical_bull.add_user
+python -m mechanical_bull.add_user [--accept] name hostname
 ```
 
-This will then ask you to enter a name, the hostname, your ActivityPub Actor lives on, then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).
+This will  then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).
 
 The configuration is saved in `config.toml`. bovine also supports authentication through private keys and HTTP signatures. For the details on how to configure this, please consult bovine. You can add further automations there.
 
 Then you should be able to run mechanical bull via
 
 ```bash
 python -m mechanical_bull.run
```

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc` & `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
+moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
 files sz: 491
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc` & `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
+moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
 files sz: 225
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc` & `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
+moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
 files sz: 521
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc` & `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
+moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
 files sz: 847
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/reject_follow_request.py` & `mechanical_bull-0.0.6/mechanical_bull/actions/reject_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/mechanical_bull/actions/test_accept_reject_follow_request.py` & `mechanical_bull-0.0.6/mechanical_bull/actions/test_accept_reject_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/mechanical_bull/event_loop.py` & `mechanical_bull-0.0.6/mechanical_bull/event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/mechanical_bull/run.py` & `mechanical_bull-0.0.6/mechanical_bull/run.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/mechanical_bull/test_event_loop.py` & `mechanical_bull-0.0.6/mechanical_bull/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.5/PKG-INFO` & `mechanical_bull-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: mechanical-bull
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework to automate reacting to ActivityStreams events.
 Home-page: https://codeberg.org/bovine/mechanical_bull
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bovine (>=0.1.1,<0.2.0)
+Requires-Dist: sphinx-argparse (>=0.4.0,<0.5.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Project-URL: Documentation, https://mechanical-bull.readthedocs.io/en/latest/
 Project-URL: Repository, https://codeberg.org/bovine/mechanical_bull
 Description-Content-Type: text/markdown
 
 # Mechanical Bull
 
 Mechanical Bull is an ActivityPub Client application build based on [bovine](https://codeberg.org/bovine/bovine/). It's main goal is to provide a platform for automating activities undertaking in the FediVerse. Furthermore, it serves as a demonstration how ActivityPub Clients can be build with bovine.
 
@@ -26,18 +28,18 @@
 ```bash
 pip install mechanical-bull
 ```
 
 Once can then add a new user by running
 
 ```bash
-python -m mechanical_bull.add_user
+python -m mechanical_bull.add_user [--accept] name hostname
 ```
 
-This will then ask you to enter a name, the hostname, your ActivityPub Actor lives on, then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).
+This will  then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).
 
 The configuration is saved in `config.toml`. bovine also supports authentication through private keys and HTTP signatures. For the details on how to configure this, please consult bovine. You can add further automations there.
 
 Then you should be able to run mechanical bull via
 
 ```bash
 python -m mechanical_bull.run
```

