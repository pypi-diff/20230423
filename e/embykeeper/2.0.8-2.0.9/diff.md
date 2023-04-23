# Comparing `tmp/embykeeper-2.0.8.tar.gz` & `tmp/embykeeper-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.0.8.tar", last modified: Thu Apr 20 10:52:59 2023, max compression
+gzip compressed data, was "embykeeper-2.0.9.tar", last modified: Fri Apr 21 22:15:30 2023, max compression
```

## Comparing `embykeeper-2.0.8.tar` & `embykeeper-2.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 10:52:40.000000 embykeeper-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 10:52:40.000000 embykeeper-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-04-20 10:52:59.446127 embykeeper-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-04-20 10:52:40.000000 embykeeper-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/sosdbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/pornemby_exam.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 10:52:40.000000 embykeeper-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 10:52:59.446127 embykeeper-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-20 10:52:40.000000 embykeeper-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 22:15:17.000000 embykeeper-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-04-21 22:15:30.964925 embykeeper-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-21 22:15:17.000000 embykeeper-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.956925 embykeeper-2.0.9/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/pornemby_exam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.956925 embykeeper-2.0.9/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-21 22:15:17.000000 embykeeper-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:15:30.964925 embykeeper-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-21 22:15:17.000000 embykeeper-2.0.9/test/test_cli.py
```

### Comparing `embykeeper-2.0.8/LICENSE` & `embykeeper-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/PKG-INFO` & `embykeeper-2.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,8 @@
-Metadata-Version: 2.1
-Name: embykeeper
-Version: 2.0.8
-Summary: Daily checkin automator for emby bots in telegram.
-Home-page: https://github.com/embykeeper/embykeeper
-Author: jackzzs
-Author-email: jackzzs@outlook.com
-Keywords: emby,telegram,checkin,automator
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7,<3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
@@ -32,38 +11,38 @@
 
 ---
 
 Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
 
 ## 声明
 
-本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
-本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
 本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
 
-当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
-当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
   - 支持群组
     - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
     - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
     - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
     - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
     - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
     - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
     - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
     - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
     - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
     - 默认禁用:
       - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
       - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
       - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
   - 特性
     - 验证码识别与自动重试
     - 多账户签到
@@ -75,17 +54,67 @@
   - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
 
 ## 安装与使用
 
+### 从 PyPi 安装
+
+Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
 ### 从 Docker 安装
 
-Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 touch config.toml
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
 命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
@@ -103,15 +132,15 @@
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
@@ -144,81 +173,31 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
 
-### 从 Pypi 安装
-
-Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
-
-```bash
-pip install embykeeper
-```
-
-随后, 您需要执行:
-
-```bash
-embykeeper
-```
-
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-
-随后, 您需要再次执行:
-
-```bash
-embykeeper
-```
-
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
-
-```bash
-tmux
-```
-
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
-
-您随时可以通过运行:
-
-```bash
-tmux a
-```
-
-以重新连接到 `tmux` 终端.
-
-当版本更新时, 您需要执行:
-
-```
-pip install -U embykeeper
-```
-
-然后重新运行应用.
-
 ### 从源码构建
 
-首先拉取 Github 并安装:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
 cd embykeeper
-make develop
+pip install -e .
 ```
 
 然后即可执行 Embykeeper:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
 
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,18 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.8 Summary: Daily checkin
-automator for emby bots in telegram. Home-page: https://github.com/embykeeper/
-embykeeper Author: jackzzs Author-email: jackzzs@outlook.com Keywords:
-emby,telegram,checkin,automator Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
-Desktop Classifier: Natural Language :: Chinese (Simplified) Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.7,<3.11 Description-
-Content-Type: text/markdown License-File: LICENSE [![pypi badge](https://
-img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [!
-[downloads badge](https://img.shields.io/pypi/dm/
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
+project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
-pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
-pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
-badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
-github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
-img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
-[telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
-t.me/embykeeper)
+pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
+embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
+embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
+embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
+[telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
+embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
+channel-green)](https://t.me/embykeeper) [![telegram badge](https://
+img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -60,44 +50,65 @@
 Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
 [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
 t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
 [æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
 æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
-[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
-t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
-/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
-+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
-- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
+~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
+å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
 [æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
 [è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
 æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
 UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
 [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
-æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
+å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
+æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
+(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
+`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
+`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
+v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
 [telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
 [Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
 ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
 è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
 run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
 æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
@@ -106,46 +117,28 @@
 cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
 config.toml watchtower: container_name: watchtower image: containrrr/watchtower
 restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
 ``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
 f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
 å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
 1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
-[conda](https://github.com/conda/conda) æ [virtualvenv](https://
-virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
-å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
-è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
-embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
-monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
-instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
+ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
+embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
+Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
+(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
+s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
+I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
```

### Comparing `embykeeper-2.0.8/README.md` & `embykeeper-2.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,28 @@
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
+Metadata-Version: 2.1
+Name: embykeeper
+Version: 2.0.9
+Summary: Daily checkin automator for emby bots in telegram.
+Author-email: jackzzs <jackzzs@outlook.com>
+Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
@@ -11,38 +31,38 @@
 
 ---
 
 Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
 
 ## 声明
 
-本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
-本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
 本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
 
-当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
-当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
   - 支持群组
     - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
     - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
     - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
     - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
     - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
     - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
     - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
     - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
     - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
     - 默认禁用:
       - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
       - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
       - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
   - 特性
     - 验证码识别与自动重试
     - 多账户签到
@@ -54,17 +74,67 @@
   - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
 
 ## 安装与使用
 
+### 从 PyPi 安装
+
+Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
 ### 从 Docker 安装
 
-Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 touch config.toml
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
 命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
@@ -82,15 +152,15 @@
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
@@ -123,81 +193,31 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
 
-### 从 Pypi 安装
-
-Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
-
-```bash
-pip install embykeeper
-```
-
-随后, 您需要执行:
-
-```bash
-embykeeper
-```
-
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-
-随后, 您需要再次执行:
-
-```bash
-embykeeper
-```
-
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
-
-```bash
-tmux
-```
-
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
-
-您随时可以通过运行:
-
-```bash
-tmux a
-```
-
-以重新连接到 `tmux` 终端.
-
-当版本更新时, 您需要执行:
-
-```
-pip install -U embykeeper
-```
-
-然后重新运行应用.
-
 ### 从源码构建
 
-首先拉取 Github 并安装:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
 cd embykeeper
-make develop
+pip install -e .
 ```
 
 然后即可执行 Embykeeper:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
 
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,29 @@
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
-project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
-embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
-pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
-pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
-badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
-github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
-img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
-[telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
-t.me/embykeeper)
+Metadata-Version: 2.1 Name: embykeeper Version: 2.0.9 Summary: Daily checkin
+automator for emby bots in telegram. Author-email: jackzzs
+outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
+:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.7 Description-Content-Type: text/markdown License-
+File: LICENSE [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https:/
+/pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
+dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
+embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
+embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
+embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
+[telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
+embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
+channel-green)](https://t.me/embykeeper) [![telegram badge](https://
+img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -49,44 +61,65 @@
 Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
 [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
 t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
 [æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
 æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
-[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
-t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
-/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
-+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
-- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
+~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
+å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
 [æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
 [è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
 æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
 UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
 [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
-æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
+å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
+æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
+(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
+`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
+`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
+v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
 [telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
 [Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
 ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
 è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
 run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
 æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
@@ -95,46 +128,28 @@
 cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
 config.toml watchtower: container_name: watchtower image: containrrr/watchtower
 restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
 ``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
 f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
 å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
 1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
-[conda](https://github.com/conda/conda) æ [virtualvenv](https://
-virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
-å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
-è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
-embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
-monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
-instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
+ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
+embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
+Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
+(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
+s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
+I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
```

### Comparing `embykeeper-2.0.8/embykeeper/cli.py` & `embykeeper-2.0.9/embykeeper/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,21 +81,15 @@
     follow: bool = typer.Option(False, "--follow", "-f", rich_help_panel="调试参数", help="仅启动消息调试"),
     analyze: bool = typer.Option(False, "--analyze", "-a", rich_help_panel="调试参数", help="仅启动历史信息分析"),
 ):
     from .log import logger, initialize
 
     initialize(level="DEBUG" if debug else "INFO")
 
-    try:
-        config = prepare_config(config)
-    except tomllib.TOMLDecodeError as e:
-        logger.error(f"TOML 配置文件错误: {e}.")
-        sys.exit(1)
-    if not config:
-        sys.exit(1)
+    config: dict = prepare_config(config)
 
     if debug:
         config.setdefault("nofail", False)
         logger.warning("您当前处于调试模式, 错误将会导致程序停止运行.")
 
     if emby < 0:
         emby = -emby
```

### Comparing `embykeeper-2.0.8/embykeeper/embywatcher/emby.py` & `embykeeper-2.0.9/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/embywatcher/main.py` & `embykeeper-2.0.9/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/log.py` & `embykeeper-2.0.9/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/loop.py` & `embykeeper-2.0.9/embykeeper/loop.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/settings.py` & `embykeeper-2.0.9/embykeeper/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
+import sys
 from loguru import logger
 
 import tomli as tomllib
+from schema import And, Optional, Or, Regex, Schema, SchemaError, Use
 
 
 def check_config(config):
-    from schema import And, Optional, Or, Regex, Schema, SchemaError, Use
-
     PositiveInt = lambda: And(Use(int), lambda n: n > 0)
     schema = Schema(
         {
             Optional("timeout"): PositiveInt(),
             Optional("retries"): PositiveInt(),
             Optional("concurrent"): PositiveInt(),
             Optional("random"): PositiveInt(),
@@ -57,23 +57,23 @@
                 )
             ],
         }
     )
     try:
         schema.validate(config)
     except SchemaError as e:
-        logger.error(f"配置文件错误, 请检查配置文件:\n{e}.")
-        return False
-    return True
+        return e
+    else:
+        return None
 
 
 def write_faked_config(path):
     import uuid
 
-    from tomlkit import document, nl, comment, item, dump, table
+    from tomlkit import document, nl, comment, item, dump
     from faker import Faker
     from faker.providers import internet, profile
 
     from .telechecker.main import get_names
     from . import __name__, __version__
 
     logger.warning("需要输入一个toml格式的config文件.")
@@ -84,14 +84,17 @@
     fake.add_provider(profile)
 
     doc = document()
     doc.add(comment("This is an example config file."))
     doc.add(comment("Please fill in your account information."))
     doc.add(comment("See details: https://github.com/embykeeper/embykeeper#安装与使用"))
     doc.add(nl())
+    doc.add(comment("将关键信息发送到第一个 Telegram 账号, 设为N以发送到第 N 个."))
+    doc["notifier"] = True
+    doc.add(nl())
     doc.add(comment("每个 Telegram Bot 签到的最大尝试时间."))
     doc["timeout"] = 120
     doc.add(nl())
     doc.add(comment("每个 Telegram Bot 签到的最大尝试次数."))
     doc["retries"] = 10
     doc.add(nl())
     doc.add(comment("最大可同时进行的 Telegram Bot 签到."))
@@ -156,24 +159,41 @@
         t["progress"].comment("模拟观看后设置的时间进度 (秒)")
         emby.append(t)
     doc["emby"] = emby
     with open(path, "w+") as f:
         dump(doc, f)
 
 
-def prepare_config(config=None):
-    default_config = "config.toml"
-    if not config:
-        if not Path(default_config).exists():
-            return write_faked_config(default_config)
-    with open(config, "rb") as f:
-        config = tomllib.load(f)
-    if not config:
-        return write_faked_config(default_config)
-    if not check_config(config):
-        return
-    proxy = config.get("proxy", None)
+def prepare_config(config_file=None):
+    default_config_file = Path("config.toml")
+    if not config_file:
+        if not default_config_file.exists():
+            write_faked_config(default_config_file)
+            sys.exit(250)
+        else:
+            config_file = default_config_file
+    try:
+        if not Path(config_file).exists():
+            logger.error(f'配置文件 "{config_file}" 不存在.')
+            sys.exit(251)
+        elif config_file == default_config_file:
+            with open(config_file, "rb") as f:
+                config = tomllib.load(f)
+            if not config:
+                write_faked_config(config_file)
+                sys.exit(250)
+        else:
+            with open(config_file, "rb") as f:
+                config = tomllib.load(f)
+    except tomllib.TOMLDecodeError as e:
+        logger.error(f"TOML 配置文件错误: {e}.")
+        sys.exit(252)
+    error = check_config(config)
+    if error:
+        logger.error(f"配置文件错误, 请检查配置文件:\n{error}.")
+        sys.exit(253)
+    proxy: dict = config.get("proxy", None)
     if proxy:
         proxy.setdefault("scheme", "socks5")
         proxy.setdefault("hostname", "127.0.0.1")
         proxy.setdefault("port", "1080")
     return config
```

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/base.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.0.9/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/link.py` & `embykeeper-2.0.9/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/main.py` & `embykeeper-2.0.9/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/messager/base.py` & `embykeeper-2.0.9/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/messager/common.py` & `embykeeper-2.0.9/embykeeper/telechecker/messager/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,10 +76,10 @@
                 "水不用解释，水就是水",
                 "我水，故我在",
                 "生命在于水，积分在于水",
                 "水，让生命更加美好",
                 "今天又水一水~",
             ),
             *args,
-            **kw
+            **kw,
         )
     ] * n
```

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.0.9/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.0.9/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.0.9/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/monitor/pornemby_exam.py` & `embykeeper-2.0.9/embykeeper/telechecker/monitor/pornemby_exam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import random
-import string
-
 from pyrogram.types import Message, InlineKeyboardMarkup
 
 from ...utils import truncate_str
 from ..link import Link
 from .base import Monitor
 
 
@@ -14,15 +11,15 @@
     chat_user = "pornemby_question_bot"
     chat_keyword = r"问题\d：(.*)\n+(A:.*\n+B:.*\n+C:.*\n+D:.*)"
 
     async def on_trigger(self, message: Message, keys, reply):
         if "答案" in message.text or not isinstance(message.reply_markup, InlineKeyboardMarkup):
             return
         question = truncate_str(keys[0], 20)
-        result = await Link(self.client).captcha(keys[0] + "\n" + keys[1])
+        result = await Link(self.client).answer(keys[0] + "\n" + keys[1])
         if result:
             self.log.info(f'检测到新问题: "{question}", 回答: {result}.')
         else:
             self.log.info(f'检测到新问题: "{question}", 但解析回答失败.')
         try:
             await message.click(result)
         except ValueError:
```

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.0.9/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.8/embykeeper/telechecker/tele.py` & `embykeeper-2.0.9/embykeeper/telechecker/tele.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
                 self.phone_code = None
                 retry = True
             except SessionPasswordNeeded:
                 retry = False
                 while True:
                     if not self.password:
                         if retry:
-                            msg = f'需要输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认): '
-                        else:
                             msg = f'密码错误, 请重新输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认):'
+                        else:
+                            msg = f'需要输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认): '
                         self.password = Prompt.ask(" " * 29 + msg, password=True)
                     try:
                         return await self.check_password(self.password)
                     except BadRequest:
                         self.password = None
                         retry = True
             else:
```

### Comparing `embykeeper-2.0.8/embykeeper/utils.py` & `embykeeper-2.0.9/embykeeper/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 from collections import namedtuple
 from functools import wraps
+import sys
 from typing import Any, Iterable, Union
 
 from loguru import logger
 import click
 from typer import Typer, Exit
 from typer.core import TyperCommand
 
@@ -28,15 +29,15 @@
                     return asyncio.run(async_func(*_args, **_kwargs))
                 except KeyboardInterrupt:
                     print("\r", end="")
                     logger.info("所有客户端已停止, 欢迎您再次使用 Embykeeper.")
                 except Exception as e:
                     print("\r", end="")
                     fail_message(e)
-                    raise Exit(1) from None
+                    sys.exit(1)
 
             self.command(*args, **kwargs)(sync_func)
             return async_func
 
         return decorator
```

### Comparing `embykeeper-2.0.8/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.0.9/embykeeper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.0.8
+Version: 2.0.9
 Summary: Daily checkin automator for emby bots in telegram.
-Home-page: https://github.com/embykeeper/embykeeper
-Author: jackzzs
-Author-email: jackzzs@outlook.com
-Keywords: emby,telegram,checkin,automator
+Author-email: jackzzs <jackzzs@outlook.com>
+Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7,<3.11
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
@@ -32,38 +31,38 @@
 
 ---
 
 Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
 
 ## 声明
 
-本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
-本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
 本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
 
-当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
-当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
   - 支持群组
     - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
     - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
     - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
     - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
     - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
     - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
     - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
     - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
     - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
     - 默认禁用:
       - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
       - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
       - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
   - 特性
     - 验证码识别与自动重试
     - 多账户签到
@@ -75,17 +74,67 @@
   - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
 
 ## 安装与使用
 
+### 从 PyPi 安装
+
+Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
 ### 从 Docker 安装
 
-Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 touch config.toml
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
 命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
@@ -103,15 +152,15 @@
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
@@ -144,81 +193,31 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
 
-### 从 Pypi 安装
-
-Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
-
-```bash
-pip install embykeeper
-```
-
-随后, 您需要执行:
-
-```bash
-embykeeper
-```
-
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-
-随后, 您需要再次执行:
-
-```bash
-embykeeper
-```
-
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
-
-```bash
-tmux
-```
-
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
-
-您随时可以通过运行:
-
-```bash
-tmux a
-```
-
-以重新连接到 `tmux` 终端.
-
-当版本更新时, 您需要执行:
-
-```
-pip install -U embykeeper
-```
-
-然后重新运行应用.
-
 ### 从源码构建
 
-首先拉取 Github 并安装:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
 cd embykeeper
-make develop
+pip install -e .
 ```
 
 然后即可执行 Embykeeper:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
 
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.8 Summary: Daily checkin
-automator for emby bots in telegram. Home-page: https://github.com/embykeeper/
-embykeeper Author: jackzzs Author-email: jackzzs@outlook.com Keywords:
-emby,telegram,checkin,automator Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
-Desktop Classifier: Natural Language :: Chinese (Simplified) Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.7,<3.11 Description-
-Content-Type: text/markdown License-File: LICENSE [![pypi badge](https://
-img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [!
-[downloads badge](https://img.shields.io/pypi/dm/
-embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
-pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
-pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
-badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
-github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
-img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
-[telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
-t.me/embykeeper)
+Metadata-Version: 2.1 Name: embykeeper Version: 2.0.9 Summary: Daily checkin
+automator for emby bots in telegram. Author-email: jackzzs
+outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
+:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.7 Description-Content-Type: text/markdown License-
+File: LICENSE [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https:/
+/pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
+dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
+embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
+embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
+embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
+[telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
+embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
+channel-green)](https://t.me/embykeeper) [![telegram badge](https://
+img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -60,44 +61,65 @@
 Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
 [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
 t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
 [æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
 æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
-[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
-t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
-/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
-+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
-- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
+~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
+å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
 [æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
 [è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
 æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
 UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
 [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
-æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
+å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
+æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
+(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
+`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
+`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
+v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
 [telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
 [Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
 ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
 è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
 run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
 æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
@@ -106,46 +128,28 @@
 cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
 config.toml watchtower: container_name: watchtower image: containrrr/watchtower
 restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
 ``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
 f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
 å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
 1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
-[conda](https://github.com/conda/conda) æ [virtualvenv](https://
-virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
-å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
-è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
-embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
-monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
-instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
+ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
+embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
+Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
+(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
+s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
+I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
```

### Comparing `embykeeper-2.0.8/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.0.9/embykeeper.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 LICENSE
-MANIFEST.in
 README.md
-setup.cfg
-setup.py
-./requirements.txt
+pyproject.toml
 embykeeper/__init__.py
 embykeeper/cli.py
 embykeeper/log.py
 embykeeper/loop.py
 embykeeper/settings.py
 embykeeper/utils.py
 embykeeper.egg-info/PKG-INFO
@@ -31,20 +28,21 @@
 embykeeper/telechecker/bots/jms.py
 embykeeper/telechecker/bots/jms_iptv.py
 embykeeper/telechecker/bots/ljyy.py
 embykeeper/telechecker/bots/nebula.py
 embykeeper/telechecker/bots/peach.py
 embykeeper/telechecker/bots/pornemby.py
 embykeeper/telechecker/bots/singularity.py
-embykeeper/telechecker/bots/sosdbot.py
+embykeeper/telechecker/bots/sssq.py
 embykeeper/telechecker/bots/terminus.py
 embykeeper/telechecker/messager/__init__.py
 embykeeper/telechecker/messager/base.py
 embykeeper/telechecker/messager/common.py
 embykeeper/telechecker/messager/nakonako.py
 embykeeper/telechecker/messager/test.py
 embykeeper/telechecker/monitor/__init__.py
 embykeeper/telechecker/monitor/base.py
 embykeeper/telechecker/monitor/bgk.py
 embykeeper/telechecker/monitor/embyhub.py
 embykeeper/telechecker/monitor/pornemby_exam.py
-embykeeper/telechecker/monitor/test.py
+embykeeper/telechecker/monitor/test.py
+test/test_cli.py
```

