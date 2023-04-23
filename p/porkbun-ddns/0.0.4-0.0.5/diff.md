# Comparing `tmp/porkbun-ddns-0.0.4.tar.gz` & `tmp/porkbun-ddns-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porkbun-ddns-0.0.4.tar", last modified: Sun Apr 23 14:24:00 2023, max compression
+gzip compressed data, was "porkbun-ddns-0.0.5.tar", last modified: Sun Apr 23 14:27:56 2023, max compression
```

## Comparing `porkbun-ddns-0.0.4.tar` & `porkbun-ddns-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:24:00.723028 porkbun-ddns-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 14:24:00.723028 porkbun-ddns-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:24:00.719028 porkbun-ddns-0.0.4/porkbun_ddns/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/porkbun_ddns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/porkbun_ddns/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/porkbun_ddns/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/porkbun_ddns/porkbun_ddns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:24:00.723028 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 14:24:00.000000 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-23 14:24:00.000000 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:24:00.000000 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 14:24:00.000000 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 14:24:00.000000 porkbun-ddns-0.0.4/porkbun_ddns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 14:24:00.723028 porkbun-ddns-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-23 14:23:45.000000 porkbun-ddns-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:27:56.047479 porkbun-ddns-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 14:27:56.047479 porkbun-ddns-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:27:56.047479 porkbun-ddns-0.0.5/porkbun_ddns/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/porkbun_ddns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/porkbun_ddns/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/porkbun_ddns/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/porkbun_ddns/porkbun_ddns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:27:56.047479 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 14:27:56.000000 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-23 14:27:56.000000 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:27:56.000000 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 14:27:56.000000 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 14:27:56.000000 porkbun-ddns-0.0.5/porkbun_ddns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 14:27:56.051479 porkbun-ddns-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-23 14:27:39.000000 porkbun-ddns-0.0.5/setup.py
```

### Comparing `porkbun-ddns-0.0.4/LICENSE` & `porkbun-ddns-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.0.4/PKG-INFO` & `porkbun-ddns-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.0.4
+Version: 0.0.5
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

### Comparing `porkbun-ddns-0.0.4/README.md` & `porkbun-ddns-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.0.4/porkbun_ddns/cli.py` & `porkbun-ddns-0.0.5/porkbun_ddns/cli.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.0.4/porkbun_ddns/helpers.py` & `porkbun-ddns-0.0.5/porkbun_ddns/helpers.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.0.4/porkbun_ddns/porkbun_ddns.py` & `porkbun-ddns-0.0.5/porkbun_ddns/porkbun_ddns.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.0.4/porkbun_ddns.egg-info/PKG-INFO` & `porkbun-ddns-0.0.5/porkbun_ddns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.0.4
+Version: 0.0.5
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

### Comparing `porkbun-ddns-0.0.4/setup.py` & `porkbun-ddns-0.0.5/setup.py`

 * *Files identical despite different names*

