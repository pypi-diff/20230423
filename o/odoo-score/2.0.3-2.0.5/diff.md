# Comparing `tmp/odoo_score-2.0.3.tar.gz` & `tmp/odoo_score-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo_score-2.0.3.tar", last modified: Sun Dec  4 19:47:17 2022, max compression
+gzip compressed data, was "odoo_score-2.0.5.tar", last modified: Sun Apr 23 13:59:27 2023, max compression
```

## Comparing `odoo_score-2.0.3.tar` & `odoo_score-2.0.5.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:47:17.000000 odoo_score-2.0.3/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-11-09 07:22:00.000000 odoo_score-2.0.3/odoo_score.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      186 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      940 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1118 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2022-12-04 19:47:17.000000 odoo_score-2.0.3/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1737 2022-11-12 18:00:54.000000 odoo_score-2.0.3/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score/
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      164 2022-09-09 18:30:58.000000 odoo_score-2.0.3/odoo_score/__main__.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_8.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_14.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     3075 2022-09-09 18:30:58.000000 odoo_score-2.0.3/odoo_score/secure_db.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      874 2022-11-13 11:50:05.000000 odoo_score-2.0.3/odoo_score/models.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_11.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    15844 2022-12-04 14:44:29.000000 odoo_score-2.0.3/odoo_score/set_workers
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)   160186 2022-11-12 18:00:54.000000 odoo_score-2.0.3/odoo_score/odoo_shell.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_9.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:47:17.000000 odoo_score-2.0.3/odoo_score/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1737 2022-12-04 18:00:20.000000 odoo_score-2.0.3/odoo_score/scripts/setup.info
--rw-r--r--   0 odoo      (1000) odoo      (1000)     5916 2022-11-12 18:00:54.000000 odoo_score-2.0.3/odoo_score/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      992 2022-10-11 15:29:25.000000 odoo_score-2.0.3/odoo_score/scripts/run_odoo_debug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26616 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/scripts/run_odoo_debug.sh
--rw-r--r--   0 odoo      (1000) odoo      (1000)     5807 2022-11-12 18:00:54.000000 odoo_score-2.0.3/odoo_score/scripts/map_module_dependecies.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     4769 2022-11-12 18:00:54.000000 odoo_score-2.0.3/odoo_score/scripts/rename_odoo_module.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      142 2022-11-05 14:16:30.000000 odoo_score-2.0.3/odoo_score/scripts/__init__.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_7.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:29.000000 odoo_score-2.0.3/odoo_score/odoo_score_12.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)    11822 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_6.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:30.000000 odoo_score-2.0.3/odoo_score/odoo_score_13.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)       92 2022-11-13 12:02:07.000000 odoo_score-2.0.3/odoo_score/__init__.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     6144 2022-09-09 18:30:58.000000 odoo_score-2.0.3/odoo_score/migrate.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-04 14:44:29.000000 odoo_score-2.0.3/odoo_score/odoo_score_10.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1118 2022-12-04 19:47:17.000000 odoo_score-2.0.3/PKG-INFO
--rw-r--r--   0 odoo      (1000) odoo      (1000)     8461 2022-12-04 19:47:17.000000 odoo_score-2.0.3/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1117 2023-04-23 13:59:27.229416 odoo_score-2.0.5/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8940 2023-04-23 13:59:26.000000 odoo_score-2.0.5/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      758 2023-04-20 06:09:47.000000 odoo_score-2.0.5/odoo_score/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/__main__.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      299 2022-12-13 18:54:38.000000 odoo_score-2.0.5/odoo_score/api.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      413 2022-12-13 18:54:38.000000 odoo_score-2.0.5/odoo_score/fields.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6144 2023-04-15 07:42:48.000000 odoo_score-2.0.5/odoo_score/migrate.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      455 2023-04-20 06:11:16.000000 odoo_score-2.0.5/odoo_score/models_2.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      431 2023-04-20 06:11:16.000000 odoo_score-2.0.5/odoo_score/models_3.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    11822 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/odoo_score.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_10.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_11.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_12.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_13.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_14.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_6.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_7.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      277 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/odoo_score_9.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)   163851 2023-04-15 07:43:03.000000 odoo_score-2.0.5/odoo_score/odoo_shell.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      144 2023-04-23 10:07:05.000000 odoo_score-2.0.5/odoo_score/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5916 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5807 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/map_module_dependecies.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     4769 2023-03-25 14:32:15.000000 odoo_score-2.0.5/odoo_score/scripts/rename_odoo_module.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29084 2023-04-20 10:41:38.000000 odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1821 2023-04-23 13:49:43.000000 odoo_score-2.0.5/odoo_score/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3075 2022-12-09 05:08:44.000000 odoo_score-2.0.5/odoo_score/secure_db.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    15765 2023-04-15 08:02:21.000000 odoo_score-2.0.5/odoo_score/set_workers
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 13:59:27.229416 odoo_score-2.0.5/odoo_score.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1117 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1004 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      130 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:00.000000 odoo_score-2.0.5/odoo_score.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-04-23 13:59:27.000000 odoo_score-2.0.5/odoo_score.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 13:59:27.229416 odoo_score-2.0.5/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1821 2023-04-23 10:07:05.000000 odoo_score-2.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odoo_score-2.0.3/odoo_score.egg-info/SOURCES.txt` & `odoo_score-2.0.5/odoo_score.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 README.rst
 setup.py
 odoo_score/__init__.py
 odoo_score/__main__.py
+odoo_score/api.py
+odoo_score/fields.py
 odoo_score/migrate.py
-odoo_score/models.py
+odoo_score/models_2.py
+odoo_score/models_3.py
 odoo_score/odoo_score.py
 odoo_score/odoo_score_10.py
 odoo_score/odoo_score_11.py
 odoo_score/odoo_score_12.py
 odoo_score/odoo_score_13.py
 odoo_score/odoo_score_14.py
 odoo_score/odoo_score_6.py
```

### Comparing `odoo_score-2.0.3/odoo_score.egg-info/PKG-INFO` & `odoo_score-2.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 1.2
-Name: odoo-score
-Version: 2.0.3
+Metadata-Version: 2.1
+Name: odoo_score
+Version: 2.0.5
 Summary: Odoo super core
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Odoo supercore
-        
-        odoo_score is a library that extends the odoo orm functionality
-        and makes available a simple odoo shell.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+Odoo supercore
+
+odoo_score is a library that extends the odoo orm functionality
+and makes available a simple odoo shell.
+
+
```

### Comparing `odoo_score-2.0.3/setup.py` & `odoo_score-2.0.5/odoo_score/scripts/setup.info`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='odoo_score',
-    version='2.0.3',
+    version='2.0.5',
     description='Odoo super core',
     long_description="""
 Odoo supercore
 
 odoo_score is a library that extends the odoo orm functionality
 and makes available a simple odoo shell.
 """,
@@ -14,14 +14,15 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: System Shells',
     ],
     keywords='odoo',
     url='https://zeroincombenze-tools.readthedocs.io',
@@ -33,17 +34,19 @@
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
     install_requires=['z0lib', 'future'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': [
         'scripts/setup.info',
         'scripts/run_odoo_debug.sh',
-        './set_workers']},
+        './set_workers',
+        './models_barely',
+    ]},
     entry_points={
         'console_scripts': [
             'odoo_score-info = odoo_score.scripts.main:main',
             'rename_odoo_module = odoo_score.scripts.rename_odoo_module:main',
-            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
+            # 'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `odoo_score-2.0.3/odoo_score/secure_db.py` & `odoo_score-2.0.5/odoo_score/secure_db.py`

 * *Files identical despite different names*

### Comparing `odoo_score-2.0.3/odoo_score/set_workers` & `odoo_score-2.0.5/odoo_score/set_workers`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,24 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 ODOOLIBDIR=$(findpkg odoorc "$PYPATH" "clodoo")
 [[ -z "$ODOOLIBDIR" ]] && echo "Library file odoorc not found!" && exit 72
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.3
+__version__=2.0.5
 
 
 evaluate_params() {
     local val prc minconn
     [[ $opt_branch =~ ^1[123456789] ]] && minconn=64 || minconn=32
     if [[ $opt_nopsql -ne 0 ]]; then
         ((AVAI_MEM=(CUR_MEM*3)/4))
```

### Comparing `odoo_score-2.0.3/odoo_score/odoo_shell.py` & `odoo_score-2.0.5/odoo_score/odoo_shell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
+from past.builtins import long
 
 import csv
 import getpass
 import re
-# import os
+import os
 import sys
 import time
 from builtins import *  # noqa
 from builtins import input
 from datetime import date, datetime, timedelta
+# import itertools
 
 from future import standard_library
 from openpyxl import load_workbook
 
 from os0 import os0
 from python_plus import _b
 
@@ -29,15 +31,15 @@
     from z0lib import z0lib
 
 import pdb  # pylint: disable=deprecated-module
 
 standard_library.install_aliases()  # noqa: E402
 
 
-__version__ = '2.0.3'
+__version__ = '2.0.5'
 
 
 MAX_DEEP = 20
 PAY_MOVE_STS_2_DRAFT = ['posted']
 INVOICES_STS_2_DRAFT = ['open', 'paid']
 STATES_2_DRAFT = ['open', 'paid', 'posted']
 TECH_FIELDS = [
@@ -122,15 +124,15 @@
 msg_time = time.time()
 os0.set_tlog_file('./odoo_shell.log', echo=True)
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
-    if t > 3:
+    if t > 4:
         print(text, '\r')
         msg_time = time.time()
 
 
 def env_ref(ctx, xref, retxref_id=None):
     xrefs = xref.split('.')
     if len(xrefs) == 2:
@@ -230,59 +232,53 @@
     if tax_id:
         tax_id = tax_id[0]
     else:
         tax_id = False
     return tax_id
 
 
-def param_date(param, model=None, date_field=None, domain=None, ctx=ctx):
+def param_date(param, date_field=None, ctx=ctx):
     """Return record ids of model by user request;
     param values:
         'yyyy-mm-dd': specific date
         '+n': from today + n days
         '': from current month (if day >= 15) or from prior month (if day < 15)
         'n': record n of model
         '[n,..]': records n ... of model
-    model: Odoo model
-    date_field: Odoo model field with date to manage
+    date_field: Odoo model field with date to manage (means return domain)
     """
     if param == '?':
-        date_ids = False
+        domain = False
+    elif not param:
+        day = datetime.now().day
+        month = datetime.now().month
+        year = datetime.now().year
+        if day < 15:
+            month -= 1
+            if month < 1:
+                month = 12
+                year -= 1
+        day = 1
+        from_date = '%04d-%02d-%02d' % (year, month, day)
+        domain = [(date_field, '>=', from_date)]
+    elif param.isdigit():
+        domain = [('id', '=', int(param))]
+    elif "," in param:
+        domain = [('id', 'in', [int(x) for x in param.split(",")])]
+    elif param and param.startswith('+'):
+        date_ids = date.strftime(
+            date.today() - timedelta(eval(param)), '%04Y-%02m-%02d'
+        )
+        domain = [(date_field, '>=', date_ids)]
+    elif ".." in param:
+        domain = [(date_field, '>=', param.split("..")[0]),
+                  (date_field, '<=', param.split("..")[1])]
     else:
-        if param and param.startswith('+'):
-            date_ids = date.strftime(
-                date.today() - timedelta(eval(param)), '%04Y-%02m-%02d'
-            )
-        else:
-            day = datetime.now().day
-            month = datetime.now().month
-            year = datetime.now().year
-            if day < 15:
-                month -= 1
-                if month < 1:
-                    month = 12
-                    year -= 1
-            day = 1
-            from_date = '%04d-%02d-%02d' % (year, month, day)
-            date_ids = param or from_date
-    if not date_ids:
-        date_ids = input('IDS to manage or date yyyy-mm-dd (empty means all)? ')
-    if model and date_field:
-        if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-            if isinstance(domain, (list, tuple)):
-                where = [x for x in domain]
-                where.append((date_field, '>=', date_ids))
-            else:
-                where = [(date_field, '>=', date_ids)]
-            date_ids = clodoo.searchL8(ctx, model, where)
-        else:
-            date_ids = eval(date_ids)
-            if domain and isinstance(date_ids, int):
-                date_ids = [date_ids]
-    return date_ids
+        domain = [(date_field, '>=', param)]
+    return domain
 
 
 def param_mode_commission(param):
     mode = ctx['param_1'] or 'A'
     while mode not in ('A', 'R', 'C'):
         mode = input('Mode (Add_missed,Recalculate,Check)? ')
         mode = mode[0].upper() if mode else ''
@@ -300,703 +296,379 @@
 
 
 def all_addr_same_customer(ctx):
     print('Set delivery address to the same of customer on sale order')
     if ctx['param_1'] == 'help':
         print(
             'delivery_addr_same_customer '
-            '[from_date|+days|ids] [Inv|Del|Both] [partner_id]'
+            '[FROM_DATE|+DAYS|IDS] [Inv|Delivery|Both] [partner_id]'
         )
         return
-    model = 'sale.order'
-    date_ids = param_date(ctx['param_1'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, model, [('date_order', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
+    resource_so = 'sale.order'
+    domain = param_date(ctx['param_1'], date_field='date_order')
     select = 'B'
     if ctx['param_2'] in ('I', 'D', 'B'):
         select = ctx['param_2']
     if ctx['param_3']:
         force_partner_id = eval(ctx['param_3'])
     else:
         force_partner_id = False
     ctr = 0
-    for so in clodoo.browseL8(ctx, model, ids):
+    for so in clodoo.browseL8(ctx, resource_so, domain):
         vals = {}
         if force_partner_id:
-            vals['partner_id'] = force_partner_id
+            if so.partner_id != force_partner_id:
+                vals['partner_id'] = force_partner_id
         else:
             if select in ('B', 'D') and so.partner_shipping_id != so.partner_id:
                 vals['partner_shipping_id'] = so.partner_id.id
             if select in ('B', 'I') and so.partner_invoice_id != so.partner_id:
                 vals['partner_invoice_id'] = so.partner_id.id
         if vals:
-            clodoo.writeL8(ctx, model, so.id, vals)
+            clodoo.writeL8(ctx, resource_so, so.id, vals)
             print('so.number=%s' % so.name)
             ctr += 1
     print('%d sale orders updated' % ctr)
 
 
-def set_db_4_test(ctx):
-    print('Set database ready for tests')
-    if ctx['param_1'] == 'help':
-        print('set_db_4_test')
-        return
-    main_company = env_ref(ctx, 'base.main_company')
-    company_id = env_ref(ctx, 'z0bug.mycompany')
-    partner_company = env_ref(ctx, 'z0bug.partner_mycompany')
-    if not company_id or company_id == main_company:
-        model = 'res.company'
-        domain = [('id', '!=', main_company)]
-        if partner_company:
-            domain.append(('partner_id', '=', partner_company))
-        companies = clodoo.searchL8(ctx, model, domain)
-        if not companies and partner_company:
-            print('Wrong config! Company partner is not the declared one!')
-            domain = [('id', '!=', main_company)]
-            companies = clodoo.searchL8(ctx, model, domain)
-        if not companies:
-            raise IOError('!!No company to test!')
-        add_xref(ctx, 'z0bug.mycompany', 'res.company', companies[0])
-        print('Database set to test')
-    else:
-        print('Database is already set to test')
-    model = 'res.company'
-    company_id = env_ref(ctx, 'z0bug.mycompany')
-    partner_company_id = env_ref(ctx, 'z0bug.partner_mycompany')
-    company = clodoo.browseL8(ctx, model, company_id)
-    if company.partner_id != partner_company_id:
-        print('Wrong config! Company partner is not the declared one!')
-        valid_partner = False
-        if partner_company_id:
-            partner = clodoo.browseL8(ctx, 'res.partner', partner_company_id)
-            if partner.city == 'Ozzero':
-                valid_partner = True
-        if valid_partner:
-            clodoo.writeL8(ctx, model, company_id, {'partner_id': partner_company_id})
-        else:
-            add_xref(
-                ctx, 'z0bug.partner_mycompany', 'res.partner', company.partner_id.id
-            )
-
-
 def order_inv_group_by_partner(ctx):
-    print('Set order invoicing group by customer')
+    print('Set order invoicing group by customer setting')
     if ctx['param_1'] == 'help':
-        print('order_inv_group_by_partner' '[from_date|+days|ids]')
+        print('order_inv_group_by_partner' '[FROM_DATE|+DAYS|IDS]')
         return
-    model = 'sale.order'
-    date_ids = param_date(ctx['param_1'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, model, [('date_order', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
-    if ids:
-        if isinstance(ids, int):
-            domain = [('order_id', '=', ids)]
-        else:
-            domain = [('order_id', 'in', ids)]
-    else:
-        domain = []
+    resource_so = 'sale.order'
+    domain = param_date(ctx['param_1'], date_field='date_order')
     ctr = 0
     for order in clodoo.browseL8(
-        ctx, model, clodoo.searchL8(ctx, model, domain, order='name desc,id')
-    ):
+        ctx, resource_so, clodoo.searchL8(
+            ctx, resource_so, domain, order='name desc,id')):
         msg_burst('%s ...' % order.name)
         partner_group = order.partner_id.ddt_invoicing_group
         sale_group = order.ddt_invoicing_group
         if sale_group != partner_group:
             print('Changing group of %s' % order.name)
-            clodoo.writeL8(ctx, model, order.id, {'ddt_invoicing_group': partner_group})
+            clodoo.writeL8(
+                ctx, resource_so, order.id, {'ddt_invoicing_group': partner_group})
             ctr += 1
     print('%d sale order updated' % ctr)
 
 
-def order_commission_by_partner(ctx):
-    print('If missed, set commission in order lines from customer')
-    if ctx['param_1'] == 'help':
-        print(
-            'order_commission_by_partner '
-            '[Add|Recalc|Check] [from_date|+days|ids]'
-            ' [Pproduct_id|Aagent_id]'
-        )
-        return
-    ord_model = 'sale.order'
-    ord_line_model = 'sale.order.line'
-    sale_agent_model = 'sale.order.line.agent'
-    mode = param_mode_commission(ctx['param_1'])
-    date_ids = param_date(ctx['param_2'])
-    product_id, agent_id = param_product_agent(ctx['param_3'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, ord_model, [('date_order', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
-    if ids:
-        if isinstance(ids, int):
-            domain = [('order_id', '=', ids)]
-            domain1 = [('id', '=', ids)]
-        else:
-            domain = [('order_id', 'in', ids)]
-            domain1 = [('id', 'in', ids)]
-    else:
-        domain = []
-        domain1 = []
-    if product_id:
-        domain.append(('product_id', '=', product_id))
-    print('Starting mode %s from %s' % (mode, date_ids))
-    ctr = 0
-    for ord_line in clodoo.browseL8(
-        ctx,
-        ord_line_model,
-        clodoo.searchL8(ctx, ord_line_model, domain, order='order_id desc,id'),
-    ):
-        msg_burst('%s ...' % ord_line.order_id.name)
-        commission_free = ord_line.product_id.commission_free
-        if ord_line.agents and not commission_free:
-            if mode in ('A', 'C'):
-                continue
-            clodoo.unlinkL8(ctx, sale_agent_model, ord_line.agents.id)
-        if mode == 'C':
-            if not commission_free:
-                print(
-                    'Ord. %s to %-30.30s line %-30.30s w/o commission'
-                    % (
-                        ord_line.order_id.number,
-                        ord_line.order_id.partner_id.name,
-                        ord_line.name,
-                    )
-                )
-            continue
-        rec = {}
-        if not commission_free:
-            for agent in ord_line.order_id.partner_id.agents:
-                rec = {'agent': agent.id, 'commission': agent.commission.id}
-                break
-        vals = {}
-        if rec:
-            vals['agents'] = [(0, 0, rec)]
-        if commission_free:
-            vals['commission_free'] = commission_free
-        if vals:
-            clodoo.writeL8(ctx, ord_line_model, ord_line.id, vals)
-            ctr += 1
-    if mode != 'C':
-        # Force line update
-        for order in clodoo.browseL8(
-            ctx, ord_model, clodoo.searchL8(ctx, ord_model, domain1, order='id desc')
-        ):
-            msg_burst('%s ...' % order.name)
-            clodoo.writeL8(ctx, ord_model, order.id, {'name': order.name})
-    print('%d sale order lines updated' % ctr)
+def make_refund_for_wrong_delivery(ctx):
+    print('Make refund from wrong delivery')
 
+    resource_inv = 'account.invoice'
+    # resource_invline = 'account.invoice.line'
+    # resource_so = 'sale.order'
+    # resource_soline = 'sale.order.line'
+    resource_carrier = 'delivery.carrier'
+    resource_company = 'res.company'
 
-def inv_commission_by_partner(ctx):
-    print('If missed, set commission in invoice lines from customer')
     if ctx['param_1'] == 'help':
-        print('inv_commission_by_partner [Add,Recalc|Check] from_date|ids')
+        print('Make refund from wrong delivery [FROM_DATE|+DAYS|IDS]')
         return
-    inv_model = 'account.invoice'
-    inv_line_model = 'account.invoice.line'
-    inv_agent_model = 'account.invoice.line.agent'
-    mode = param_mode_commission(ctx['param_1'])
-    date_ids = param_date(ctx['param_2'])
-    product_id, agent_id = param_product_agent(ctx['param_3'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, inv_model, [('date_invoice', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
-    if ids:
-        if isinstance(ids, int):
-            domain = [('invoice_id', '=', ids)]
-            domain1 = [('id', '=', ids)]
-        else:
-            domain = [('invoice_id', 'in', ids)]
-            domain1 = [('id', 'in', ids)]
-    else:
-        domain = []
-        domain1 = []
-    if product_id:
-        domain.append(('product_id', '=', product_id))
-    domain.append(('invoice_id.type', 'in', ('out_invoice', 'out_refund')))
-    domain1.append(('type', 'in', ('out_invoice', 'out_refund')))
-    print('Starting mode %s from %s' % (mode, date_ids))
-    ctr = 0
-    for inv_line in clodoo.browseL8(
-        ctx,
-        inv_line_model,
-        clodoo.searchL8(ctx, inv_line_model, domain, order='invoice_id desc,id'),
-    ):
-        msg_burst('%s ...' % inv_line.invoice_id.number)
-        commission_free = False
-        if commission_free == inv_line.product_id:
-            commission_free = inv_line.product_id.commission_free
-        if inv_line.agents and not commission_free:
-            if mode in ('A', 'C'):
-                continue
-            clodoo.unlinkL8(ctx, inv_agent_model, inv_line.agents.id)
-        if mode == 'C':
-            if not commission_free:
-                print(
-                    'Inv. %s to %-30.30s line %-30.30s w/o commission'
-                    % (
-                        inv_line.invoice_id.number,
-                        inv_line.invoice_id.partner_id.name,
-                        inv_line.name,
-                    )
-                )
-            continue
-        rec = {}
-        if not commission_free:
-            for agent in inv_line.invoice_id.partner_id.agents:
-                rec = {'agent': agent.id, 'commission': agent.commission.id}
-                break
-        vals = {}
-        if rec:
-            vals['agents'] = [(0, 0, rec)]
-        if commission_free:
-            vals['commission_free'] = commission_free
-        if vals:
-            clodoo.writeL8(ctx, inv_line_model, inv_line.id, vals)
-            ctr += 1
-    if mode != 'C':
-        # Force line update
-        for invoice in clodoo.browseL8(
-            ctx, inv_model, clodoo.searchL8(ctx, inv_model, domain1, order='id desc')
-        ):
-            msg_burst('%s ...' % invoice.name)
-            clodoo.writeL8(ctx, inv_model, invoice.id, {'name': invoice.name})
-    print('%d account invoice lines updated' % ctr)
-
-
-def correct_invoice_entry_date(ctx):
-    print('Move old registration_date into date')
-    if ctx['param_1'] == 'help':
-        print('correct_invoice_entry_date from_date|ids')
-        return
-    inv_model = 'account.invoice'
-    ctr = 0
-    date_ids = param_date(ctx['param_1'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, inv_model, [('date_invoice', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
-    query = "update account_invoice set date=registration_date"
-    query += " where type in ('in_invoice', 'in_refund')"
-    if ids:
-        query += " and id in %s" % ids
-    clodoo.exec_sql(ctx, query)
-    print('%d invoice lines updated' % ctr)
+    domain = param_date(ctx['param_1'], date_field='date_invoice')
+    domain.append(('type', '=', 'out_invoice'))
 
+    shipping_ids = []
+    for delivery in clodoo.browseL8(ctx, resource_carrier,
+                                    clodoo.searchL8(ctx, resource_carrier, [])):
+        shipping_ids.append(delivery.product_id.id)
+    conai_product_ids = []
+    for company in clodoo.browseL8(ctx, resource_company,
+                                   clodoo.searchL8(ctx, resource_company, [])):
+        if (
+            hasattr(company, 'conai_product_id')
+            and not callable(company.conai_product_id)
+            and company.conai_product_id
+        ):
+            conai_product_ids.append(company.conai_product_id.id)
 
-def inv_commission_from_order(ctx):
-    print('If missed, copy commission in invoice lines from sale order lines')
-    if ctx['param_1'] == 'help':
-        print('inv_commission_from_order [Add,Recalc|Check] from_date|ids')
-        return
-    inv_model = 'account.invoice'
-    inv_line_model = 'account.invoice.line'
-    inv_agent_model = 'account.invoice.line.agent'
-    ctr = 0
-    mode = param_mode_commission(ctx['param_1'])
-    date_ids = param_date(ctx['param_2'])
-    product_id, agent_id = param_product_agent(ctx['param_3'])
-    if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
-        ids = clodoo.searchL8(ctx, inv_model, [('date_invoice', '>=', date_ids)])
-    else:
-        ids = eval(date_ids)
-    if ids:
-        if isinstance(ids, int):
-            domain = [('invoice_id', '=', ids)]
-            domain1 = [('id', '=', ids)]
-        else:
-            domain = [('invoice_id', 'in', ids)]
-            domain1 = [('id', 'in', ids)]
-    else:
-        domain = []
-        domain1 = []
-    if product_id:
-        domain.append(('product_id', '=', product_id))
-    domain.append(('invoice_id.type', 'in', ('out_invoice', 'out_refund')))
-    domain1.append(('type', 'in', ('out_invoice', 'out_refund')))
-    for inv_line in clodoo.browseL8(
-        ctx,
-        inv_line_model,
-        clodoo.searchL8(ctx, inv_line_model, domain, order='invoice_id desc,id'),
-    ):
-        msg_burst('%s ...' % inv_line.invoice_id.number)
-        commission_free = False
-        if commission_free == inv_line.product_id:
-            commission_free = inv_line.product_id.commission_free
-        if inv_line.agents and not commission_free:
-            if mode in ('A', 'C'):
-                continue
-            clodoo.unlinkL8(ctx, inv_agent_model, inv_line.agents.id)
-        if mode == 'C':
-            if not commission_free:
-                print(
-                    'Inv. %s to %-30.30s line %-30.30s w/o commission'
-                    % (
-                        inv_line.invoice_id.number,
-                        inv_line.invoice_id.partner_id.name,
-                        inv_line.name,
-                    )
-                )
+    ctr_read = ctr_upd = ctr_wrong = 0
+    invoices = {}
+    for inv in clodoo.browseL8(ctx, resource_inv,
+                               clodoo.searchL8(ctx, resource_inv, domain)):
+        msg_burst('%s (%d/%d) ...' % (inv.number, ctr_upd, ctr_read))
+        ctr_read += 1
+        has_ddt = True
+        for ln in inv.invoice_line_ids:
+            msg_burst('%s (%d/%d) - %s ...'
+                      % (inv.number, ctr_upd, ctr_read, ln.name[:40]))
+            if (
+                ln.product_id
+                and ln.product_id.id not in shipping_ids
+                and ln.product_id.id not in conai_product_ids
+                and not ln.ddt_line_id
+            ):
+                has_ddt = False
+                break
+        if not has_ddt:
             continue
-        for ord_line in inv_line.sale_line_ids:
-            if not ord_line.agents.amount:
-                continue
-            agents = [
-                (0, 0, {'agent': x.agent.id, 'commission': x.commission.id})
-                for x in ord_line.agents
-            ]
-            clodoo.writeL8(ctx, inv_line_model, inv_line.id, {'agents': agents})
-            ctr += 1
-    if mode != 'C':
-        for invoice in clodoo.browseL8(
-            ctx, inv_model, clodoo.searchL8(ctx, inv_model, domain1, order='id desc')
-        ):
-            msg_burst('%s ...' % invoice.number)
-            clodoo.writeL8(ctx, inv_model, invoice.id, {'number': invoice.number})
-    print('%d invoice lines updated' % ctr)
 
+        ddts = {}
+        last_ddt_id = False
+        for ln in inv.invoice_line_ids:
+            msg_burst('%s (%d/%d) - %s ...'
+                      % (inv.number, ctr_upd, ctr_read, ln.name[:40]))
+            if (
+                ln.product_id and (
+                    ln.product_id.id in shipping_ids
+                    or ln.product_id.id in conai_product_ids)
+            ):
+                ctr_read += 1
+                if ddts[last_ddt_id]:
+                    if inv.partner_id.id not in invoices:
+                        invoices[inv.partner_id.id] = []
+                    invoices[inv.partner_id.id].append(ln)
+                    ctr_wrong += 1
+                ddts[last_ddt_id] = True
+            else:
+                if ln.ddt_line_id.package_preparation_id:
+                    last_ddt_id = ln.ddt_line_id.package_preparation_id.id
+                    if last_ddt_id not in ddts:
+                        ddts[last_ddt_id] = False
 
-def update_einvoice_out_attachment(ctx):
-    print('Update e-attachment of invoice')
-    model = 'account.invoice'
-    if ctx['param_1'] == 'help':
-        print('update_einvoice_out_attachment invoice_id [state]')
-        return
-    if ctx['param_1']:
-        inv_id = eval(ctx['param_1'])
-    else:
-        inv_id = input('Invoice id: ')
-        inv_id = eval(inv_id) if inv_id else 0
-    if inv_id:
-        inv = clodoo.browseL8(ctx, model, inv_id)
-        att = inv.fatturapa_attachment_out_id
-        if not att:
-            print('Invoice %s w/o attachment' % inv.number)
-            return
-        print('Processing invoice %s' % inv.number)
-        model_att = 'fatturapa.attachment.out'
-        att = clodoo.browseL8(ctx, model_att, att.id)
-        print('Attachment ID = %d, state=%s' % (att.id, att.state))
-        state = ctx['param_2']
-        while state not in (
-            'ready',
-            'sent',
-            'sender_error',
-            'recipient_error',
-            'rejected',
-            'validated',
-            'accepted',
-            'discarted',
-        ):
-            state = input(
-                'State (ready,sent,sender|recipient_error,reject,'
-                'validated,accepted,discarted): '
-            )
-        clodoo.writeL8(ctx, model_att, att.id, {'state': state})
+    for line_ids in invoices.values():
+        inv = False
+        vals = {}
+        for ln in line_ids:
+            if not inv:
+                inv = ln.invoice_id
+                vals['type'] = 'out_refund'
+                vals['account_id'] = inv.account_id.id
+                vals['company_id'] = inv.company_id.id
+                vals['fiscal_position_id'] = inv.fiscal_position_id.id or False
+                vals['journal_id'] = inv.journal_id.id
+                vals['partner_id'] = inv.partner_id.id
+                vals['invoice_line_ids'] = []
+                vals['origin'] = ''
+            vals['origin'] += (' %s' % inv.number)
+            line_vals = {
+                'account_id': ln.account_id.id,
+                'product_id': ln.product_id.id,
+                'discount': ln.discount,
+                'invoice_line_tax_ids': [6, 0, [x.id for x in ln.invoice_line_tax_ids]],
+                'name': ln.name,
+                'origin': inv.number,
+                'price_unit': ln.price_unit,
+                'quantity': ln.quantity,
+                'uom_id': ln.uom_id.id,
+            }
+            vals['invoice_line_ids'].append((0, 0, line_vals))
+        clodoo.createL8(ctx, resource_inv, vals)
+        ctr_upd += 1
+    print('%d sale order updated of %d read!' % (ctr_upd, ctr_read))
 
 
-def unlink_einvoice_out_attachment(ctx):
-    print('Unlink e-attachment of invoice')
-    model = 'account.invoice'
+def recalc_delivery_price(ctx):
+    print('Recalculate delivery price on DdT')
+
+    resource_ddt = 'stock.picking.package.preparation'
+    resource_line = 'stock.picking.package.preparation.line'
+    resource_soline = 'sale.order.line'
+    resource_carrier = 'delivery.carrier'
     if ctx['param_1'] == 'help':
-        print('unlink_einvoice_out_attachment invoice_id IN|OUT')
+        print('recalc_delivery_price [FROM_DATE|+DAYS|IDS]')
         return
-    if ctx['param_1']:
-        inv_id = eval(ctx['param_1'])
-    else:
-        inv_id = input('Invoice id: ')
-        inv_id = eval(inv_id) if inv_id else 0
-    if ctx['param_2'] in ('IN', 'in', 'OUT', 'out'):
-        in_out = ctx['param_2'].lower()
-    else:
-        in_out = input('IN/OUT: ')
-        if in_out.lower() == 'in':
-            field = 'fatturapa_attachment_in_id'
-        else:
-            field = 'fatturapa_attachment_out_id'
-    if inv_id:
-        inv = clodoo.browseL8(ctx, model, inv_id)
-        print('Processing invoice %s' % inv.number)
-        clodoo.writeL8(ctx, model, inv.id, {field: False})
-
-
-def revaluate_due_date_in_invoces(ctx, inv_id=False):
-    print('Revaluate all due dates of invoices from xml')
-    model = 'account.invoice'
-    if not inv_id:
-        inv_id = input('Invoice id: ')
-        if inv_id:
-            inv_id = eval(inv_id)
-    if inv_id:
-        inv = clodoo.browseL8(ctx, model, inv_id)
-        att = inv.fatturapa_attachment_in_id
-        if not att:
-            print('Invoice %s w/o attachment' % inv.number)
-            return
-        print('Processing invoice %s' % inv.number)
-        inv_state = inv.state
-        if inv.state in INVOICES_STS_2_DRAFT:
-            reconcile_dict, move_dict = clodoo.get_reconcile_from_invoices(
-                [inv_id], ctx
-            )
-            clodoo.unreconcile_invoices(reconcile_dict, ctx)
-            try:
-                clodoo.upd_invoices_2_draft(move_dict, ctx)
-            except BaseException:
-                return
-        clodoo.executeL8(ctx, 'fatturapa.attachment.in', 'revaluate_due_date', att.id)
-        if inv_state in INVOICES_STS_2_DRAFT:
-            try:
-                clodoo.upd_invoices_2_posted(move_dict, ctx)
-            except BaseException:
-                return
-            reconciles = reconcile_dict[inv_id]
-            if len(reconciles):
-                cur_reconciles, cur_reconcile_dict = clodoo.refresh_reconcile_from_inv(
-                    inv_id, reconciles, ctx
-                )
-                clodoo.reconcile_invoices(cur_reconcile_dict, ctx)
-
-
-def set_tax_code_on_invoice(ctx):
-    print('Set tax code on invoice lines, if missed and if no line amount')
-    inv_model = 'account.invoice'
-    inv_line_model = 'account.invoice.line'
-    inv_id = input('Invoice id: ')
-    ctr = 0
-    if inv_id:
-        inv_id = eval(inv_id)
-        invoice = clodoo.browseL8(ctx, inv_model, inv_id)
-        tax_id = _get_tax_record(ctx, company_id=invoice.company_id.id)
-        if not tax_id:
-            print('Tax 22v not found!')
-        for inv_line in clodoo.browseL8(
-            ctx,
-            inv_line_model,
-            clodoo.searchL8(ctx, inv_line_model, [('invoice_id', '=', inv_id)]),
-        ):
-            msg_burst('%s ...' % inv_line.name)
-            if inv_line.invoice_line_tax_ids:
-                continue
-            if inv_line.price_subtotal != 0.0:
-                print('Line w/o tax but with total amount!')
-                continue
+    shipping_ids = []
+    for delivery in clodoo.browseL8(ctx, resource_carrier,
+                                    clodoo.searchL8(ctx, resource_carrier, [])):
+        shipping_ids.append(delivery.product_id.id)
+    domain = param_date(ctx['param_1'], date_field='date')
+    domain.append(("carrier_id", "!=", False))
+    ctr_read = ctr_upd = 0
+    for ddt in clodoo.browseL8(
+        ctx, resource_ddt, clodoo.searchL8(
+            ctx, resource_ddt, domain)):
+        msg_burst('%s ...' % ddt.id)
+        clodoo.executeL8(ctx, resource_ddt, "delivery_set", ddt.id)
+        ctr_read += 1
+        ddt = clodoo.browseL8(ctx, resource_ddt, ddt.id)
+        sale_id = False
+        delivery_price = 0.0
+        if ddt.delivery_price == 0.0:
+            for line in clodoo.browseL8(
+                ctx, resource_line, clodoo.searchL8(
+                    ctx, resource_line, [("package_preparation_id", "=", ddt.id)])):
+                if line.sale_id:
+                    sale_id = line.sale_id.id
+                    break
+        if sale_id:
+            for soline in clodoo.browseL8(
+                ctx, resource_soline, clodoo.searchL8(
+                    ctx, resource_soline, [("order_id", "=", sale_id),
+                                           ("product_id", "in", shipping_ids)])):
+                delivery_price += soline.price_subtotal
+        if delivery_price:
             clodoo.writeL8(
-                ctx,
-                inv_line_model,
-                inv_line.id,
-                {'invoice_line_tax_ids': [(6, 0, [tax_id])]},
-            )
-            ctr += 1
-
-        clodoo.writeL8(ctx, inv_model, inv_id, {'number': invoice.number})
-    print('%d invoice lines updated' % ctr)
-
-
-def show_module_group(ctx):
-    print('Show group infos and external names')
-    model_grp = 'res.groups'
-    model_ctg = 'ir.module.category'
-    model_ir_md = 'ir.model.data'
-    gid = True
-    while gid:
-        gid = input('Res.groups id: ')
-        if gid:
-            gid = eval(gid)
-        if gid:
-            group = clodoo.browseL8(ctx, model_grp, gid, context={'lang': 'en_US'})
-            cid = group.category_id.id
-            categ = clodoo.browseL8(ctx, model_ctg, cid, context={'lang': 'en_US'})
-            print('%6d) Category %s' % (cid, categ.name))
-            uniq_field = []
-            grp_ids = clodoo.searchL8(ctx, model_grp, [('category_id', '=', cid)])
-            for group in clodoo.browseL8(ctx, model_grp, grp_ids):
-                if group.implied_ids:
-                    uniq_field.append(group.id)
-                    uniq_field += [x.id for x in group.implied_ids]
-            for group in clodoo.browseL8(
-                ctx, model_grp, grp_ids, context={'lang': 'en_US'}
-            ):
-                ir_md = clodoo.browseL8(
-                    ctx,
-                    model_ir_md,
-                    clodoo.searchL8(
-                        ctx,
-                        model_ir_md,
-                        [('model', '=', model_grp), ('res_id', '=', group.id)],
-                    ),
-                )
-                if group.id in uniq_field:
-                    tag = '*'
-                else:
-                    tag = ''
-                print(
-                    '%6d) -- Value [%-16.16s] > [%-32.32s] as "%s.%s" {%s}'
-                    % (
-                        group.id,
-                        group.name,
-                        group.full_name,
-                        ir_md.module,
-                        ir_md.name,
-                        tag,
-                    )
-                )
-
+                ctx, resource_ddt, ddt.id, {"delivery_price": delivery_price})
+            ctr_upd += 1
 
-def clean_translations(ctx):
-    print('Delete unuseful translations')
-    model = 'ir.translation'
-    domain = [
-        ('lang', '=', 'it_IT'),
-        '|',
-        ('name', '=', 'ir.module.module,description'),
-        ('name', '=', 'ir.module.module,shortdesc'),
-    ]
-    ids = clodoo.searchL8(ctx, model, domain)
-    print('unlink %s' % ids)
-    clodoo.unlinkL8(ctx, model, ids)
-    print('%d records deleted' % len(ids))
+    print('%d delivery notes read, %d written' % (ctr_read, ctr_upd))
 
 
 def close_sale_orders(ctx):
     print('Close sale orders with linked invoice')
+
+    resource_so = 'sale.order'
+    resource_line = 'sale.order.line'
+    resource_carrier = 'delivery.carrier'
+    resource_company = 'res.company'
+
     if ctx['param_1'] == 'help':
-        print('close_sale_orders [no|to invoice] [SHIP_CODE]')
+        print('close_sale_orders [no|to invoice|invoiced] [FROM_DATE|+DAYS|IDS]')
         return
     if ctx['param_1'] in ('no', 'to invoice', 'both'):
         sel_state = ctx['param_1']
     else:
         sel_state = 'both'
-    if ctx.get('param_2'):
-        prod = clodoo.searchL8(
-            ctx, 'product.product', [('default_code', '=', ctx['param_2'])]
-        )
-        if prod:
-            prod = clodoo.browseL8(ctx, 'product.product', prod[0])
-    model = 'sale.order'
-    ctr = 0
-    domain = [
-        ('state', '=', 'sale'),
-        ('invoice_count', '>', 0),
-    ]
-    if sel_state == 'both':
-        domain.append(('invoice_status', 'in', ['no', 'to invoice']))
-    else:
+    domain = param_date(ctx['param_2'], date_field='date_order')
+    domain.append(('state', '=', 'sale'))
+
+    shipping_ids = []
+    for delivery in clodoo.browseL8(ctx, resource_carrier,
+                                    clodoo.searchL8(ctx, resource_carrier, [])):
+        shipping_ids.append(delivery.product_id.id)
+    conai_product_ids = []
+    for company in clodoo.browseL8(ctx, resource_company,
+                                   clodoo.searchL8(ctx, resource_company, [])):
+        if (
+            hasattr(company, 'conai_product_id')
+            and not callable(company.conai_product_id)
+            and company.conai_product_id
+        ):
+            conai_product_ids.append(company.conai_product_id.id)
+
+    ctr_read = ctr_upd = ctr_wrong = 0
+    if sel_state != 'both':
         domain.append(('invoice_status', '=', sel_state))
-    for so in clodoo.browseL8(
-        ctx,
-        model,
-        clodoo.searchL8(ctx, model, domain),
-    ):
-        if so.invoice_ids:
-            clodoo.writeL8(ctx, model, so.id, {'invoice_status': 'invoiced'})
-            ctr += 1
-        else:
-            invoiced = True
-            ships = []
+    for so in clodoo.browseL8(ctx, resource_so,
+                              clodoo.searchL8(ctx, resource_so, domain)):
+        msg_burst('%s (%d/%d) ...' % (so.name, ctr_upd, ctr_read))
+        ctr_read += 1
+        if so.state not in ("sale", "done"):
+            if so.invoice_status == "invoiced":
+                clodoo.writeL8(ctx,
+                               resource_so,
+                               so.id,
+                               {
+                                   'invoiced': 'no'
+                               })
+                print('Order %s -> %s' % (so.name, 'no'))
+                ctr_upd += 1
+            continue
+
+        invoice_status = 'invoiced'
+        if not so.force_invoiced:
             for ln in so.order_line:
-                if ln.invoice_lines or not ln.product_id:
+                msg_burst('%s (%d/%d) ...' % (so.name, ctr_upd, ctr_read))
+                if (
+                    ln.product_id and (
+                        ln.product_id.id in shipping_ids
+                        or ln.product_id.id in conai_product_ids)
+                ):
+                    if not so.carrier_id or so.carrier_id.product_id != ln.product_id:
+                        print("*** Order %s - '%s' - Inv. %s - multiple amount %s ***"
+                              % (so.name,
+                                 ln.name[:40],
+                                 (ln.invoice_lines
+                                  and ln.invoice_lines[0].invoice_id.number),
+                                 ln.price_subtotal))
+                        ctr_wrong += 1
+                    if ln.qty_invoiced != ln.product_qty:
+                        clodoo.writeL8(ctx,
+                                       resource_line,
+                                       ln.id,
+                                       {
+                                           'qty_invoiced': ln.product_qty,
+                                           'qty_to_invoice': 0.0,
+                                       })
+                        ctr_upd += 1
                     continue
-                if ln.product_id == prod:
-                    ships.append(ln.id)
-                elif ln.product_id != prod:
-                    invoiced = False
-                    break
-            if invoiced:
-                for ln_id in ships:
-                    ln = clodoo.browseL8(ctx, 'sale.order.line', ln_id)
-                    clodoo.writeL8(ctx,
-                                   'sale.order.line',
-                                   ln_id,
-                                   {'qty_invoiced': ln.qty_to_invoice}
-                                   )
-                    ctr += 1
-                clodoo.writeL8(ctx, model, so.id, {'invoice_status': 'invoiced'})
-                ctr += 1
-    print('%d sale order updated!' % ctr)
+
+                if ln.invoice_lines:
+                    continue
+                invoice_status = 'to invoice'
+                if so.invoice_status != invoice_status:
+                    print("\nSO=%s - %s\n" % (so.name, ln.name[:40]))
+                break
+
+        if so.invoice_status != invoice_status:
+            clodoo.writeL8(ctx,
+                           resource_so,
+                           so.id,
+                           {
+                               'invoice_status': invoice_status,
+                           })
+            print('Order %s -> %s' % (so.name, invoice_status))
+            ctr_upd += 1
+
+    print('%d sale order updated of %d read!' % (ctr_upd, ctr_read))
 
 
 def close_ddts(ctx):
     print('Close Delivery Document Type with linked invoice')
     if ctx['param_1'] == 'help':
-        print('close_sale_orders')
+        print('close_ddts [FROM_DATE|+DAYS|IDS]')
         return
-    model = 'stock.picking.package.preparation.line'
-    model1 = 'stock.picking.package.preparation'
+    domain = param_date(ctx['param_1'], date_field='date')
 
-    ctr = 0
-    transportation_reason = False
-    for ln in clodoo.browseL8(
-        ctx,
-        model1,
-        clodoo.searchL8(
-            ctx,
-            model1,
-            [
-                ('invoice_id', '=', False),
-            ],
-        ),
-    ):
-        msg_burst('%s ...' % ln.name)
-        if ln.transportation_reason_id != transportation_reason:
-            transportation_reason = ln.transportation_reason_id
-        if ln.to_be_invoiced != transportation_reason.to_be_invoiced:
-            clodoo.writeL8(ctx,
-                           model1,
-                           ln.id,
-                           {'to_be_invoiced': transportation_reason.to_be_invoiced})
-            ctr += 1
+    resource_ddt = 'stock.picking.package.preparation'
+    resource_product = 'product.product'
 
-    for ln in clodoo.browseL8(
-        ctx,
-        model1,
-        clodoo.searchL8(
-            ctx,
-            model1,
-            [
-                ('invoice_id', '!=', False),
-                ('to_be_invoiced', '=', True)
-            ],
-        ),
-    ):
-        msg_burst('%s ...' % ln.name)
-        clodoo.writeL8(ctx,
-                       model1,
-                       ln.id,
-                       {'to_be_invoiced': False})
-        ctr += 1
+    ctr_read = ctr_upd = 0
+    transportation_reason = False
+    for ddt in clodoo.browseL8(ctx, resource_ddt,
+                               clodoo.searchL8(ctx, resource_ddt, domain)):
+        msg_burst('%s (%d/%d) ...' % ((ddt.ddt_number or ddt.name), ctr_upd, ctr_read))
+        ctr_read += 1
+        if ddt.transportation_reason_id != transportation_reason:
+            transportation_reason = ddt.transportation_reason_id
+        if ddt.state != "done" or not transportation_reason.to_be_invoiced:
+            if ddt.to_be_invoiced != transportation_reason.to_be_invoiced:
+                clodoo.writeL8(ctx,
+                               resource_ddt,
+                               ddt.id,
+                               {
+                                   'to_be_invoiced':
+                                       transportation_reason.to_be_invoiced
+                               })
+                ctr_upd += 1
+            continue
 
-    for ln in clodoo.browseL8(
-        ctx,
-        model,
-        clodoo.searchL8(
-            ctx,
-            model,
-            [
-                ('package_preparation_id.to_be_invoiced', '=', True),
-                '|',
-                ('invoice_line_id', '!=', False),
-                ('sale_line_id.order_id.invoice_status', '=', 'invoiced')
-            ],
-        ),
-    ):
-        msg_burst('%s ...' % ln.package_preparation_id.name)
-        # Header may be updated by previous line, so test weather have to anything
-        if ln.package_preparation_id.to_be_invoiced:
+        invoice_id = to_be_invoiced = False
+        for ln in ddt.line_ids:
+            msg_burst('%s (%d/%d) ...' % (
+                (ddt.ddt_number or ddt.name), ctr_upd, ctr_read))
+            if ln.invoice_line_id:
+                if not invoice_id:
+                    invoice_id = ln.invoice_line_id.invoice_id.id
+                continue
+            if (
+                ln.sale_line_id
+                and ln.sale_line_id.order_id
+                and ln.sale_line_id.order_id.invoice_status == 'invoiced'
+            ):
+                continue
+            if ln.product_id:
+                product = clodoo.browseL8(ctx, resource_product, ln.product_id.id)
+                if product.type == 'service':
+                    continue
+            to_be_invoiced = True
+            break
+        if ddt.to_be_invoiced != to_be_invoiced:
             clodoo.writeL8(ctx,
-                           model1,
-                           ln.package_preparation_id.id,
-                           {'to_be_invoiced': False})
-            ctr += 1
-    print('%d DdT updated!' % ctr)
+                           resource_ddt,
+                           ddt.id,
+                           {
+                               'to_be_invoiced': to_be_invoiced,
+                               'invoice_id': invoice_id,
+                           })
+            ctr_upd += 1
+
+    print('%d DdT updated of %d read!' % (ctr_upd, ctr_read))
 
 
 def close_purchase_orders(ctx):
     print('Close purchase orders lines that are delivered')
     if ctx['param_1'] == 'help':
         print('close_purchase_orders ' '[byLine|Header] [from_date|+days|ids]')
         return
@@ -1008,15 +680,15 @@
     model_line = 'purchase.order.line'
     date_ids = param_date(ctx['param_2'])
     if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
         ids = clodoo.searchL8(ctx, model, [('date_order', '>=', date_ids)])
     else:
         ids = eval(date_ids)
     if ids:
-        if isinstance(ids, int):
+        if isinstance(ids, (int, long)):
             domain = [('order_id', '=', ids)]
             domain1 = [('id', '=', ids)]
         else:
             domain = [('order_id', 'in', ids)]
             domain1 = [('id', 'in', ids)]
     else:
         domain = []
@@ -1167,15 +839,15 @@
         return
     model = 'account.move.line'
     date_ids = param_date(ctx['param_1'])
     if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
         ids = clodoo.searchL8(ctx, model, [('date', '>=', date_ids)])
     else:
         ids = eval(date_ids)
-        if isinstance(ids, int):
+        if isinstance(ids, (int, long)):
             ids = [ids]
     for rec_id in ids:
         rec = clodoo.browseL8(ctx, model, rec_id)
         print(rec.name, rec.move_id.name)
         if rec.distinta_line_ids:
             riba_list_ids = []
             for ln in rec.distinta_line_ids:
@@ -1194,15 +866,15 @@
             )
             clodoo.writeL8(ctx, model, rec_id, {'distinta_line_ids': [(5, 0)]})
         elif action == 'L':
             riba_lines = input('Riba lines to link (i.e. 1,2,3): ')
             if not riba_lines:
                 continue
             riba_lines = eval(riba_lines)
-            if isinstance(riba_lines, int):
+            if isinstance(riba_lines, (int, long)):
                 riba_lines = [riba_lines]
             clodoo.writeL8(
                 ctx, model, rec_id, {'distinta_line_ids': [(6, 0, riba_lines)]}
             )
 
 
 def set_report_config(ctx):
@@ -1776,462 +1448,14 @@
             'reply_to': reply_to,
             'email_from': email_from,
             'report_name': RPT_NAME[template.model_id.model],
         }
         clodoo.writeL8(ctx, model, template.id, vals)
 
 
-def configure_fiscal_position(ctx):
-    print('Configure Fiscal Position')
-    company_id = env_ref(ctx, 'z0bug.mycompany')
-    if not company_id:
-        raise IOError('!!Internal error: no company to test found!')
-    company_partner_id = env_ref(ctx, 'z0bug.partner_mycompany')
-
-    model = 'account.account'
-    vals = {
-        'code': '490050',
-        'name': 'Transitorio Reverse Charge',
-        'company_id': company_id,
-    }
-    if ctx['majver'] < 9:
-        vals['user_type'] = env_ref(ctx, 'account.data_account_type_expense')
-    else:
-        vals['user_type_id'] = env_ref(ctx, 'account.data_account_type_expenses')
-    account_rc_id = synchro(ctx, model, vals)
-
-    vals = {
-        'code': '153050',
-        'name': 'Integr. IVA da c/acquisti UE (L.427/93)',
-        'company_id': company_id,
-    }
-    if ctx['majver'] < 9:
-        vals['user_type'] = env_ref(ctx, 'account.data_account_type_asset')
-    else:
-        vals['user_type_id'] = env_ref(ctx, 'account.data_account_type_current_assets')
-    account_vat_eup_id = synchro(ctx, model, vals)
-
-    vals = {
-        'code': '260050',
-        'name': 'IVA autofatture da c/acquisti UE',
-        'company_id': company_id,
-    }
-    if ctx['majver'] < 9:
-        vals['user_type'] = env_ref(ctx, 'account.data_account_type_liability')
-    else:
-        vals['user_type_id'] = env_ref(
-            ctx, 'account.data_account_type_current_liabilities'
-        )
-    account_vat_eus_id = synchro(ctx, model, vals)
-
-    vals = {
-        'code': '260030',
-        'name': 'IVA n/deb. split-payment',
-        'company_id': company_id,
-    }
-    if ctx['majver'] < 9:
-        vals['user_type'] = env_ref(ctx, 'account.data_account_type_liability')
-    else:
-        vals['user_type_id'] = env_ref(
-            ctx, 'account.data_account_type_current_liabilities'
-        )
-    account_vat_sp_id = synchro(ctx, model, vals)
-
-    model = 'account.journal'
-    vals = {
-        'code': 'SAJ2',
-        'name': 'Integrazione acquisti UE',
-        'company_id': company_id,
-        'type': 'sale',
-        'reverse_charge': True,
-        'update_posted': True,
-        'show_on_dashboard': False,
-    }
-    journal_id = synchro(ctx, model, vals)
-
-    vals = {
-        'code': 'GCRC',
-        'name': 'G/conti reverse charge',
-        'company_id': company_id,
-        'type': 'general',
-        'update_posted': True,
-        'default_debit_account': account_rc_id,
-        'default_credit_account': account_rc_id,
-        'show_on_dashboard': False,
-    }
-    journal_gcrc_id = synchro(ctx, model, vals)
-
-    model = 'account.tax'
-    vat_a17c2a_id = _get_tax_record(ctx, code='a17c2a')
-    vals = {
-        'description': 'a17c2a',
-        'name': 'N.I. art.17 c.2 DPR633',
-        'type_tax_use': 'purchase',
-        'account_id': account_vat_eup_id,
-        'refund_account_id': account_vat_eup_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n6'),
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if vat_a17c2a_id:
-        vals['id'] = vat_a17c2a_id
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c2a_id = synchro(ctx, model, vals)
-
-    vat_a17c2v_id = _get_tax_record(ctx, code='a17c2v')
-    vals = {
-        'description': 'aa17c2v',
-        'name': 'Rev. charge art.17 c.2 DPR633',
-        'type_tax_use': 'sale',
-        'account_id': account_vat_eus_id,
-        'refund_account_id': account_vat_eus_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if vat_a17c2v_id:
-        vals['id'] = vat_a17c2v_id
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c2v_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a17c6ba',
-        'name': 'N.I. art.17 c.6 lett. B DPR633 (Cellulari)',
-        'type_tax_use': 'purchase',
-        'account_id': account_vat_eup_id,
-        'refund_account_id': account_vat_eup_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n6'),
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c6ba_id = synchro(ctx, model, vals)
-
-    vat_a17c6bv_id = _get_tax_record(ctx, code='a17c6bv')
-    vals = {
-        'description': 'aa17c6bv',
-        'name': 'Rev. Charge art.17 c.6 lett. B DPR633 (Cellulari)',
-        'type_tax_use': 'sale',
-        'account_id': account_vat_eus_id,
-        'refund_account_id': account_vat_eus_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': False,
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if vat_a17c6bv_id:
-        vals['id'] = vat_a17c6bv_id
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c6bv_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a17c6ca',
-        'name': 'N.I. Art.17 c.6 lett. C DPR633 (Elettronici)',
-        'type_tax_use': 'purchase',
-        'account_id': account_vat_eup_id,
-        'refund_account_id': account_vat_eup_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n6'),
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c6ca_id = synchro(ctx, model, vals)
-
-    vat_a17c6cv_id = _get_tax_record(ctx, code='a17c6cv')
-    vals = {
-        'description': 'aa17c6cv',
-        'name': 'Rev. Charge Art.17 c.6 lett. C DPR633 (Elettronici)',
-        'type_tax_use': 'sale',
-        'account_id': account_vat_eus_id,
-        'refund_account_id': account_vat_eus_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': False,
-        'payability': 'I',
-        'law_reference': False,
-    }
-    if vat_a17c6cv_id:
-        vals['id'] = vat_a17c6cv_id
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_a17c6cv_id = synchro(ctx, model, vals)
-
-    vat_22spv_id = _get_tax_record(ctx, code='22SPv')
-    vals = {
-        'description': '22SPv',
-        'name': 'Art. 17ter - split-payment',
-        'type_tax_use': 'sale',
-        'account_id': account_vat_eus_id,
-        'refund_account_id': account_vat_sp_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': False,
-        'payability': 'S',
-        'law_reference': 'Art. 17ter DPR633- split-payment',
-    }
-    if vat_22spv_id:
-        vals['id'] = vat_22spv_id
-    if ctx['majver'] < 9:
-        vals['amount'] = 0.22
-    else:
-        vals['amount'] = 22.0
-    vat_22spv_id = synchro(ctx, model, vals)
-
-    vat_storno22spv_id = _get_tax_record(ctx, code='-22SPv')
-    vals = {
-        'description': '-22SPv',
-        'name': 'Storno split-payment',
-        'type_tax_use': 'sale',
-        'account_id': account_vat_eus_id,
-        'refund_account_id': account_vat_sp_id,
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': False,
-        'payability': 'S',
-        'law_reference': False,
-    }
-    if vat_storno22spv_id:
-        vals['id'] = vat_storno22spv_id
-    if ctx['majver'] < 9:
-        vals['amount'] = -0.22
-    else:
-        vals['amount'] = -22.0
-    vat_storno22spv_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a8c2v',
-        'name': 'Vend.N.I. art.8c2 DPR633 (lett.Intento)',
-        'type_tax_use': 'sale',
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n3'),
-        'law_reference': 'N.I. art.8c2 DPR633 (lett.Intento)',
-    }
-    vat_a8c2v_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a41v',
-        'name': 'Vend.N.I. art.41 L.427/93',
-        'type_tax_use': 'sale',
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n3'),
-        'law_reference': 'Vend.N.I. art.41 L.427/93',
-    }
-    vat_a41v_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a8av',
-        'name': 'Vend.N.I. art.8a DPR633 (Dogana)',
-        'type_tax_use': 'sale',
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n3'),
-        'law_reference': 'N.I. art.8a DPR633 (Dogana)',
-    }
-    vat_a8av_id = synchro(ctx, model, vals)
-
-    vals = {
-        'description': 'a7tv',
-        'name': 'Vend.NI art.7ter DPR633 (servizi xUE)',
-        'type_tax_use': 'sale',
-        'amount_type': 'percent',
-        'company_id': company_id,
-        'nature_id': env_ref(ctx, 'l10n_it_ade.n2'),
-        'law_reference': 'NI art.7ter DPR633 (servizi xUE)',
-    }
-    vat_a7tv_id = synchro(ctx, model, vals)
-
-    rc_type_id = False
-    if ctx['majver'] > 7:
-        model = 'account.rc.type'
-        rc_type_id = env_ref(ctx, 'l10n_it_reverse_charge.account_rc_type_1')
-        if rc_type_id:
-            # rc_type = clodoo.browseL8(ctx, model, rc_type_id)
-            vals = {
-                'name': 'Acquisti in reverse charge',
-                'description': 'Acquisti Intra-UE con autofattura',
-                'method': 'selfinvoice',
-                'partner_type': 'other',
-                'partner_id': company_partner_id,
-            }
-            if journal_id:
-                vals['journal_id'] = journal_id
-            if journal_gcrc_id:
-                vals['payment_journal_id'] = journal_gcrc_id
-            rc_type_id = synchro(ctx, model, vals)
-
-            model = 'account.rc.type.tax'
-            purchase_tax_id = _get_tax_record(ctx, code='a17c2a')
-            sale_tax_id = _get_tax_record(ctx, code='a17c2v')
-            vals = {
-                'rc_type_id': rc_type_id,
-                'purchase_tax_id': purchase_tax_id,
-                'sale_tax_id': sale_tax_id,
-            }
-            synchro(ctx, model, vals)
-            model = 'account.rc.type.tax'
-            purchase_tax_id = _get_tax_record(ctx, code='a17c6ba')
-            sale_tax_id = _get_tax_record(ctx, code='a17c6bv')
-            vals = {
-                'rc_type_id': rc_type_id,
-                'purchase_tax_id': purchase_tax_id,
-                'sale_tax_id': sale_tax_id,
-            }
-            synchro(ctx, model, vals)
-            purchase_tax_id = _get_tax_record(ctx, code='a17c6ca')
-            sale_tax_id = _get_tax_record(ctx, code='a17c6cv')
-            vals = {
-                'rc_type_id': rc_type_id,
-                'purchase_tax_id': purchase_tax_id,
-                'sale_tax_id': sale_tax_id,
-            }
-            synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {'name': 'Reverse charge', 'company_id': company_id}
-    if ctx['majver'] > 7:
-        vals['rc_type_id'] = rc_type_id
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx, code='22a'),
-            'tax_dest_id': vat_a17c6ba_id,
-        }
-        synchro(ctx, model, vals)
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx, code='22a'),
-            'tax_dest_id': vat_a17c6ba_id,
-        }
-        synchro(ctx, model, vals)
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx, code='22a'),
-            'tax_dest_id': vat_a17c6ca_id,
-        }
-        synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {
-        'name': 'Split Payment',
-        'company_id': company_id,
-        'split_payment': True,
-        'note': 'Operazione effettuata ai sensi degli art. 17-ter comma 1 / '
-        '17-quater DPR 633/72 - scissione pagamenti (split payment)',
-    }
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': vat_22spv_id,
-        }
-        synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {
-        'name': 'Lettera d\'intento',
-        'company_id': company_id,
-        'note': 'Operazione senza IVA Vs. lettera d\'intento n. ______ '
-        'del __/__/____',
-    }
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': vat_a8c2v_id,
-        }
-        synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {'name': 'Regime Intra comunitario', 'company_id': company_id}
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': vat_a41v_id,
-        }
-        synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {'name': 'Regime Extra comunitario', 'company_id': company_id}
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': vat_a8av_id,
-        }
-        synchro(ctx, model, vals)
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': vat_a7tv_id,
-        }
-        synchro(ctx, model, vals)
-
-    model = 'account.fiscal.position'
-    vals = {'name': 'IVA al 4%', 'company_id': company_id}
-    ids = clodoo.searchL8(ctx, model, [('name', 'ilike', 'IVA%4')])
-    if len(ids) != 1:
-        ids = clodoo.searchL8(
-            ctx, model, [('name', 'ilike', 'IVA%4'), ('company_id', '=', company_id)]
-        )
-    if len(ids) == 1:
-        vals['id'] = ids[0]
-    fiscal_pos_id = synchro(ctx, model, vals)
-    if fiscal_pos_id:
-        model = 'account.fiscal.position.tax'
-        vals = {
-            'position_id': fiscal_pos_id,
-            'tax_src_id': _get_tax_record(ctx),
-            'tax_dest_id': _get_tax_record(ctx, code='4v'),
-        }
-        synchro(ctx, model, vals)
-
-    vals = {'sp_account_id': account_vat_sp_id, 'sp_tax_id': vat_storno22spv_id}
-    clodoo.writeL8(ctx, 'res.company', company_id, vals)
-
-    print('Set fiscal positions for RC, Split-payment, lett., EU, xEU and 4%')
-
-
 def simulate_user_profile(ctx):
     print('Show data as required user')
 
     def get_agent_names(agents):
         agent_names = []
         try:
             for agent in agents:
@@ -2985,15 +2209,15 @@
     if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', inv_date_ids):
         ids = clodoo.searchL8(
             ctx, invoice_model, [('date_invoice', '>=', inv_date_ids)]
         )
     else:
         ids = eval(inv_date_ids)
     if ids:
-        if isinstance(ids, int):
+        if isinstance(ids, (int, long)):
             # inv_domain = [('invoice_id', '=', ids)]
             inv_domain1 = [('id', '=', ids)]
         else:
             # inv_domain = [('invoice_id', 'in', ids)]
             inv_domain1 = [('id', 'in', ids)]
     else:
         # inv_domain = []
@@ -3001,15 +2225,15 @@
     inv_domain1.append(('type', 'in', ('out_invoice', 'out_refund')))
     ddt_date_ids = param_date(ctx['param_2'])
     if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', ddt_date_ids):
         ids = clodoo.searchL8(ctx, ddt_model, [('date', '>=', ddt_date_ids)])
     else:
         ids = eval(ddt_date_ids)
     if ids:
-        if isinstance(ids, int):
+        if isinstance(ids, (int, long)):
             # ddt_domain = [('package_preparation_id', '=', ids)]
             ddt_domain1 = [('id', '=', ids)]
         else:
             # ddt_domain = [('package_preparation_id', 'in', ids)]
             ddt_domain1 = [('id', 'in', ids)]
     else:
         # ddt_domain = []
@@ -3707,15 +2931,15 @@
     inv_line_model = 'account.invoice.line'
     date_ids = param_date(ctx['param_1'])
     if re.match('[0-9]{4}-[0-9]{2}-[0-9]{2}', date_ids):
         ids = clodoo.searchL8(ctx, inv_model, [('date_invoice', '>=', date_ids)])
     else:
         ids = eval(date_ids)
     if ids:
-        if isinstance(ids, int):
+        if isinstance(ids, (int, long)):
             domain = [('invoice_id', '=', ids)]
             domain1 = [('id', '=', ids)]
         else:
             domain = [('invoice_id', 'in', ids)]
             domain1 = [('id', 'in', ids)]
     else:
         domain = []
@@ -4140,20 +3364,20 @@
     ctr_ulk = 0
     ctr_upd = 0
     model_stmt = "account.bank.statement"
     model_bank = "account.bank.statement.line"
     model_move = "account.move"
     model_line = "account.move.line"
     if ctx.get('param_2', '') == 'hard':
-        print('Hard redet of statement id %d' % statement_id)
+        print('Hard reset of statement id %d' % statement_id)
         for stmt_line in clodoo.browseL8(
                 ctx, model_bank, clodoo.searchL8(ctx, model_bank, [
                     ("statement_id", "=", statement_id,
                      "|",
-                     ("journal_entry_ids", "<>", []),
+                     ("journal_entry_ids", "!=", []),
                      ('move_name', '!=', False))])):
             clodoo.writeL8(
                 ctx, model_bank, stmt_line.id, {"move_name": False,
                                                 "journal_entry_ids": [(5, 0)]})
             ctr_upd += 1
         for move_line in clodoo.browseL8(
                 ctx, model_line, clodoo.searchL8(
@@ -4352,14 +3576,738 @@
             wl = clodoo.browseL8(ctx, model, main_locations[item]['id'])
             wl_parent = clodoo.browseL8(
                 ctx, model, main_locations[item]['location_id'])
             name = '%s / %s' % (wl_parent.name, wl.name.split('/')[-1].strip())
             clodoo.writeL8(ctx, model, wl.id, {'name': name})
 
 
+def rename_user(ctx):
+    print('rename_user')
+    if ctx['param_1'] == 'help':
+        print('rename_user prior_name new_name')
+        return
+    prior_user = ctx['param_1']
+    new_user = ctx['param_2']
+    if not prior_user or not new_user or prior_user == new_user:
+        print('Missed or invalid user names')
+        print('rename_user prior_name new_name')
+        return
+    _res_user = "res.users"
+    user_ids = clodoo.searchL8(ctx, _res_user, [("login", "=", prior_user)])
+    if len(user_ids) != 1:
+        print('User %s not found' % prior_user)
+        return
+    clodoo.writeL8(ctx, _res_user, user_ids, {"login": new_user})
+    print("🎺 User %s renamed to %s" % (prior_user, new_user))
+
+
+def recalc_group_left_right(ctx):
+    resorce_group = "account.group"
+    ctr = 0
+    for group in clodoo.browseL8(
+        ctx, resorce_group, clodoo.searchL8(
+            ctx, resorce_group, [("parent_id", "=", False)], order="code_prefix")):
+        ctr += 1
+        print("%s.group.parent_left %s -> %s, level %s -> %s " % (
+            group.code_prefix, group.parent_left, ctr, group.level, 1))
+        clodoo.writeL8(ctx, resorce_group, group.id, {"parent_left": ctr})
+        for group1 in clodoo.browseL8(
+            ctx, resorce_group, clodoo.searchL8(
+                ctx, resorce_group, [("parent_id", "=", group.id)],
+                order="code_prefix")):
+            ctr += 1
+            print("%s.group.parent_left %s -> %s, level %s -> %s " % (
+                group1.code_prefix, group1.parent_left, ctr, group1.level, 2))
+            clodoo.writeL8(ctx, resorce_group, group1.id, {"parent_left": ctr})
+            for group2 in clodoo.browseL8(
+                ctx, resorce_group, clodoo.searchL8(
+                    ctx, resorce_group, [("parent_id", "=", group1.id)],
+                    order="code_prefix")):
+                ctr += 1
+                print("%s.group.parent_left %s -> %s, level %s -> %s " % (
+                    group2.code_prefix, group2.parent_left, ctr, group2.level, 3))
+                clodoo.writeL8(ctx, resorce_group, group2.id, {"parent_left": ctr})
+                for group3 in clodoo.browseL8(
+                    ctx, resorce_group, clodoo.searchL8(
+                        ctx, resorce_group, [("parent_id", "=", group2.id)],
+                        order="code_prefix")):
+                    ctr += 1
+                    print("%s.group.parent_left %s -> %s, level %s -> %s " % (
+                        group3.code_prefix, group3.parent_left, ctr, group3.level, 4))
+                    clodoo.writeL8(ctx, resorce_group, group3.id, {"parent_left": ctr})
+                    for group4 in clodoo.browseL8(
+                        ctx, resorce_group, clodoo.searchL8(
+                            ctx, resorce_group, [("parent_id", "=", group3.id)],
+                            order="code_prefix")):
+                        ctr += 1
+                        print("%s.group.parent_left %s -> %s, level %s -> %s " % (
+                            group4.code_prefix, group4.parent_left, ctr, group4.level,
+                            5))
+                        clodoo.writeL8(ctx, resorce_group, group4.id,
+                                       {"parent_left": ctr})
+                        ctr += 1
+                        print("%s.group.parent_right %s -> %s" % (
+                            group4.code_prefix, group4.parent_right, ctr))
+                        clodoo.writeL8(ctx, resorce_group, group4.id,
+                                       {"parent_right": ctr})
+                    ctr += 1
+                    print("%s.group.parent_right %s -> %s" % (
+                        group3.code_prefix, group3.parent_right, ctr))
+                    clodoo.writeL8(ctx, resorce_group, group3.id, {"parent_right": ctr})
+                ctr += 1
+                print("%s.group.parent_right %s -> %s" % (
+                    group2.code_prefix, group2.parent_right, ctr))
+                clodoo.writeL8(ctx, resorce_group, group2.id, {"parent_right": ctr})
+            ctr += 1
+            print("%s.group.parent_right %s -> %s" % (
+                group1.code_prefix, group1.parent_right, ctr))
+            clodoo.writeL8(ctx, resorce_group, group1.id, {"parent_right": ctr})
+        ctr += 1
+        print("%s.group.parent_right %s -> %s" % (
+            group.code_prefix, group.parent_right, ctr))
+        clodoo.writeL8(ctx, resorce_group, group.id, {"parent_right": ctr})
+
+
+def rebuild_database(ctx):
+    def get_jids_no_vat(ctx):
+        return clodoo.searchL8(
+            ctx,
+            resource_journal,
+            ["|",
+             ("type", "not in", ["sale", "purchase"])
+                , ("code", "in", ("SAJ2", "XIT", "EXJ"))])
+
+    def reset_sequence(ctx):
+        resource_journal = "account.journal"
+        resource_sequence = "ir.sequence"
+        ctr = 0
+        for ir_seq in clodoo.browseL8(
+            ctx, resource_sequence, clodoo.searchL8(
+                ctx, resource_sequence,
+                ["|", ("prefix", "like", "%201_/"), ("prefix", "like", "%202_/")])):
+            if not clodoo.searchL8(ctx,
+                                   resource_journal,
+                                   [("sequence_id", "=", ir_seq.id)]):
+                clodoo.unlinkL8(ctx, resource_sequence, ir_seq.id)
+        journal_no_vat_ids = get_jids_no_vat(ctx)
+        for journal in clodoo.browseL8(
+            ctx, resource_journal, clodoo.searchL8(
+                ctx, resource_journal, [("id", "in", journal_no_vat_ids)])):
+            msg_burst("Resetting <%s> ..." % journal.name)
+            ir_seq = clodoo.browseL8(ctx, resource_sequence, journal.sequence_id.id)
+            if ir_seq.prefix and ir_seq.prefix.startswith("%"):
+                prefix = ir_seq.prefix.replace("%(year)s", "%(range_year)s")
+            else:
+                prefix = journal.code + "/%(range_year)s/"
+            vals = {"prefix": prefix} if prefix != ir_seq.prefix else {}
+            vals["use_date_range"] = True
+            vals["number_next"] = 1
+            vals["number_next_actual"] = 1
+            clodoo.writeL8(ctx, resource_sequence, journal.sequence_id.id, vals)
+            ctr += 1
+            # clodoo.unlinkL8(
+            #     ctx, resource_sequence_range, [x.id for x in ir_seq.date_range_ids])
+            for move in ir_seq.date_range_ids:
+                clodoo.writeL8(
+                    ctx, resource_sequence_range, move.id, {"number_next": 1,
+                                                            "number_next_actual": 1})
+                ctr += 1
+        return ctr
+
+    def load_inv_att_file(ctx, fn_attach_list):
+        attachments = {}
+        if os.path.isfile(fn_attach_list):
+            with open(fn_attach_list, "r") as fd:
+                hdr = True
+                csv_obj = csv.DictReader(fd, fieldnames=[], restkey='undef_name')
+                for row in csv_obj:
+                    if hdr:
+                        hdr = False
+                        csv_obj.fieldnames = row['undef_name']
+                        continue
+                    vals = {}
+                    for item in ("out", "in", "rc_p", "rc_self", "rc_sp"):
+                        if row[item]:
+                            vals[item] = int(row[item])
+                    attachments[int(row["id"])] = vals
+        return attachments
+
+    def store_inv_att_file(ctx, attachments, fn_attach_list):
+        with open(fn_attach_list, "w") as fd:
+            writer = csv.DictWriter(
+                fd, fieldnames=("id", "out", "in", "rc_p", "rc_self", "rc_sp"))
+            writer.writeheader()
+            for rec_id in attachments.keys():
+                vals = {"id": rec_id}
+                for item in ("out", "in", "rc_p", "rc_self", "rc_sp"):
+                    vals[item] = attachments[rec_id].get(item, "")
+                writer.writerow(vals)
+
+    def check_move_type(ctx, move, journal=None):
+        resource_invoice = "account.invoice"
+        resource_move = "account.move"
+        if not journal:
+            journal = move.journal_id
+        invs = clodoo.searchL8(ctx, resource_invoice, [("move_id", "=", move.id)])
+        if invs:
+            move_type = move_type_match[clodoo.browseL8(
+                ctx, resource_invoice, invs[0]).type]
+        elif journal.type in move_type_match:
+            move_type = move_type_match[journal.type]
+        elif journal.type in ("sale", "purchase"):
+            print("Invalid move %d (%s)" % (move.id, move.name))
+            move_type = move.move_type
+            if move.line_ids:
+                print("*** Please recover move %d" % move.id)
+            else:
+                if move.state == "post":
+                    clodoo.executeL8(ctx, resource_move, "button_cancel", move.id)
+                clodoo.unlinkL8(ctx, resource_move, move.id)
+                return False
+        else:
+            move_type = "other"
+        if move_type != move.move_type:
+            print("Invalid move type of id %d" % move.id)
+            clodoo.writeL8(ctx, resource_move, move.id, {"move_type": move_type})
+        return True
+
+    def cancel_inv_n_save_attachments(ctx):
+        ctr = 0
+        if ctx['_cr']:
+            query = (
+                "update account_invoice"
+                " set state='open'"
+                " where state='paid' and amount_total=0.0"
+            )
+            clodoo.exec_sql(ctx, query)
+
+        fn_attach_list = os.path.expanduser("~/attachments_saved.csv")
+        attachments = load_inv_att_file(ctx, fn_attach_list)
+        resource_invoice = "account.invoice"
+        for inv in clodoo.browseL8(
+            ctx, resource_invoice, clodoo.searchL8(
+                ctx, resource_invoice, [], order="date,id")):
+            msg_burst('Saving attachment inv %s (%d) ...' % (inv.number, inv.id))
+            vals = {}
+            for item, field in (
+                ("out", "fatturapa_attachment_out_id"),
+                ("in", "fatturapa_attachment_in_id"),
+                ("rc_p", "rc_purchase_invoice_id"),
+                ("rc_self", "rc_self_invoice_id"),
+                ("rc_sp", "rc_self_purchase_invoice_id"),
+            ):
+                if inv[field]:
+                    vals[item] = inv[field].id
+            if vals:
+                attachments[inv.id] = vals
+
+            query = (
+                "update account_invoice"
+                " set fatturapa_attachment_out_id=null"
+                ",fatturapa_attachment_in_id=null"
+                ",rc_purchase_invoice_id=null"
+                ",rc_self_invoice_id=null"
+                ",rc_self_purchase_invoice_id=null"
+                " where id=%d"
+            ) % inv.id
+            clodoo.exec_sql(ctx, query)
+
+            if inv.state in ("draft", "open"):
+                msg_burst('Cancelling inv %s (%d) ...' % (inv.number, inv.id))
+                try:
+                    clodoo.executeL8(
+                        ctx, resource_invoice, "action_invoice_cancel", inv.id)
+                    ctr += 1
+                except BaseException:
+                    print("Cannot cancel invoice %s (%d)" % (inv.number, inv.id))
+
+        store_inv_att_file(ctx, attachments, fn_attach_list)
+
+        query = (
+            "update fatturapa_attachment_in"
+            " set registered=false"
+        )
+        clodoo.exec_sql(ctx, query)
+        return ctr, attachments
+
+    def delete_reconciliations(ctx):
+        print("Deleting reconcilations ....")
+
+        ctr = 0
+
+        model = "account.full.reconcile"
+        for rec_id in clodoo.searchL8(ctx, model, []):
+            try:
+                clodoo.unlinkL8(ctx, model, rec_id)
+                ctr += 1
+            except BaseException:
+                pass
+
+        model = "account.partial.reconcile"
+        for rec_id in clodoo.searchL8(ctx, model, []):
+            try:
+                clodoo.unlinkL8(ctx, model, rec_id)
+                ctr += 1
+            except BaseException:
+                pass
+
+        query = "delete from account_full_reconcile"
+        clodoo.exec_sql(ctx, query)
+
+        query = "delete from account_partial_reconcile"
+        clodoo.exec_sql(ctx, query)
+
+        query = "delete from account_payment"
+        clodoo.exec_sql(ctx, query)
+
+        query = "update account_move_line set full_reconcile_id=null,reconciled=false"
+        clodoo.exec_sql(ctx, query)
+
+        return ctr
+
+    def cancel_moves(ctx):
+        print("Canceling moves ...")
+        ctr = 0
+        journal_no_vat_ids = get_jids_no_vat(ctx)
+        domain = [("state", "=", "posted"), ("journal_id", "in", journal_no_vat_ids)]
+        for rec_id in clodoo.searchL8(ctx, resource_move, domain, order="date,id"):
+            msg_burst('Cancelling move id %d ...' % rec_id)
+            try:
+                clodoo.executeL8(ctx, resource_move, "button_cancel", rec_id)
+                ctr += 1
+            except BaseException:
+                print("Cannot cancel move id %d" % rec_id)
+        return ctr
+
+    def reset_taxes(ctx):
+        resource_tax = "account.tax"
+        resource_line = "account.invoice.line"
+        rc_taxes = clodoo.searchL8(ctx, resource_tax, [("rc", "=", True)])
+        ctr = 0
+        for line in clodoo.browseL8(
+            ctx, resource_line, clodoo.searchL8
+                (ctx, resource_line, [])):
+            if (
+                line.invoice_line_tax_ids
+                and line.invoice_line_tax_ids[0] in rc_taxes
+                and not line.rc
+            ):
+                clodoo.writeL8(ctx, resource_line, line.id, {"rc": True})
+                ctr += 1
+            elif (
+                line.invoice_line_tax_ids
+                and line.invoice_line_tax_ids[0] not in rc_taxes
+                and line.rc
+            ):
+                clodoo.writeL8(ctx, resource_line, line.id, {"rc": False})
+                ctr += 1
+        return ctr
+
+    def validate_invoices(ctx):
+        print("Validation invoices ...")
+        ctr = 0
+        for inv in clodoo.browseL8(
+            ctx, resource_invoice, clodoo.searchL8(
+                ctx, resource_invoice,
+                [("journal_id.code", "in", ("SAJ2", "XIT", "EXJ"))])):
+            clodoo.writeL8(ctx, resource_invoice, inv.id, {"move_name": False})
+            ctr += 1
+
+        for inv in clodoo.browseL8(
+            ctx, resource_invoice, clodoo.searchL8(
+                ctx, resource_invoice,
+                ["|",
+                 ("type", "!=", "out_invoice"),
+                 ("rc_purchase_invoice_id", "=", False)],
+                order="date,type,id")):
+            msg_burst('Validating inv %s ...' % inv.move_name)
+
+            if inv.state == "cancel":
+                try:
+                    clodoo.executeL8(
+                        ctx, resource_invoice, "action_invoice_draft", inv.id)
+                    ctr += 1
+                    inv.state = "draft"
+                except BaseException:
+                    print("Cannot set invoice id %d to draft" % inv.id)
+
+            if inv.state != "draft":
+                continue
+
+            if inv.partner_id.property_account_position_id != inv.fiscal_position_id:
+                clodoo.writeL8(
+                    ctx,
+                    resource_invoice,
+                    inv.id,
+                    {
+                        "fiscal_position_id":
+                            inv.partner_id.property_account_position_id.id
+                    })
+                ctr += 1
+            clodoo.executeL8(ctx, resource_invoice, "compute_taxes", inv.id)
+            try:
+                clodoo.executeL8(ctx, resource_invoice, "action_invoice_open", inv.id)
+                ctr += 1
+                inv.state = "open"
+            except BaseException:
+                print("Cannot validate invoice id %d" % inv.id)
+
+            if inv.state != "open":
+                continue
+
+            inv = clodoo.browseL8(ctx, resource_invoice, inv.id)
+            recalc_sequence(ctx, inv.journal_id, inv.number)
+
+            if inv.rc_self_invoice_id:
+                sinv_id = False
+                att_out = False
+                if inv.id in attachments:
+                    if "rc_self" in attachments[inv.id]:
+                        sinv_id = attachments[inv.id]["rc_self"]
+                    else:
+                        print("Invoice %s (%d) configuration changed"
+                              % (inv.number, inv.id))
+                    if sinv_id and "out" in attachments[sinv_id]:
+                        att_out = attachments[sinv_id]["out"]
+                    else:
+                        print("Invalid self invoice %s (%d) configuration"
+                              % (inv.number, inv.id))
+                else:
+                    print("Invoice %s (%d) configuration not found"
+                          % (inv.number, inv.id))
+                if att_out:
+                    # Move attachment from prior self-invoice to current
+                    self_inv = clodoo.browseL8(
+                        ctx, resource_invoice, inv.rc_self_invoice_id.id)
+                    if self_inv.fatturapa_attachment_out_id:
+                        try:
+                            clodoo.unlinkL8(
+                                ctx,
+                                resource_att_out,
+                                self_inv.fatturapa_attachment_out_id.id)
+                        except BaseException:
+                            print("Cannot delete attachment id %d" %
+                                  self_inv.fatturapa_attachment_out_id.id)
+                    clodoo.writeL8(
+                        ctx,
+                        resource_invoice,
+                        self_inv.id, {"fatturapa_attachment_out_id": att_out})
+
+                self_inv = clodoo.browseL8(ctx, resource_invoice, sinv_id)
+                if self_inv.state == "cancel":
+                    clodoo.writeL8(
+                        ctx, resource_invoice, sinv_id, {"move_name": False})
+                    try:
+                        clodoo.unlinkL8(
+                            ctx,
+                            resource_invoice,
+                            sinv_id)
+                    except BaseException:
+                        print("Cannot remove self invoice id %d" % sinv_id)
+                    if sinv_id in attachments and "out" in attachments[sinv_id]:
+                        del attachments[sinv_id]["out"]
+                    if sinv_id in attachments and not attachments[sinv_id]:
+                        del attachments[sinv_id]
+
+                if sinv_id in attachments and "rc_self" in attachments[sinv_id]:
+                    del attachments[inv.id]["rc_self"]
+                if inv.id in attachments and not attachments[inv.id]:
+                    del attachments[inv.id]
+            elif inv.id in attachments and "rc_self" in attachments[inv.id]:
+                print("Invoice %s (%d): self-invoice configuration lost"
+                      % (inv.number, inv.id))
+
+            if inv.id in attachments and "out" in attachments[inv.id]:
+                att_out = attachments[inv.id]["out"]
+                try:
+                    clodoo.writeL8(
+                        ctx,
+                        resource_invoice,
+                        inv.id,
+                        {"fatturapa_attachment_out_id": att_out})
+                except BaseException:
+                    print("Cannot link attachment %d to invoice %d" % (att_out, inv.id))
+                    continue
+                del attachments[inv.id]["out"]
+                if not attachments[inv.id]:
+                    del attachments[inv.id]
+
+            if inv.id in attachments and "in" in attachments[inv.id]:
+                att_in = attachments[inv.id]["in"]
+                try:
+                    clodoo.writeL8(
+                        ctx,
+                        resource_invoice,
+                        inv.id,
+                        {"fatturapa_attachment_in_id": att_in})
+                except BaseException:
+                    print("Cannot link attachment %d to invoice %d" % (att_in, inv.id))
+                    continue
+                clodoo.writeL8(
+                    ctx, "fatturapa.attachment.in", att_in, {"registered": True})
+                del attachments[inv.id]["in"]
+                if not attachments[inv.id]:
+                    del attachments[inv.id]
+        return ctr
+
+    def validate_moves(ctx):
+        print("Validation moves ...")
+        journal_no_vat_ids = get_jids_no_vat(ctx)
+        ctr = 0
+        domain = [("state", "=", "draft"), ("journal_id", "in", journal_no_vat_ids)]
+        for move in clodoo.browseL8(
+            ctx, resource_move, clodoo.searchL8(
+                ctx, resource_move, domain, order="date,id")):
+            msg_burst('Validating move id %d ...' % move.id)
+            check_move_type(ctx, move)
+            try:
+                clodoo.writeL8(ctx, resource_move, move.id, {"name": "/"})
+            except BaseException:
+                print("Cannot removing entry name %d" % move.id)
+            try:
+                clodoo.executeL8(ctx, resource_move, "post", move.id)
+                ctr += 1
+                recalc_sequence(ctx, move.journal_id, move.name)
+            except BaseException:
+                print("Cannot post move id %d" % move.id)
+        return ctr
+
+    def recalc_sequence(ctx, journal, name):
+        resource_sequence = "ir.sequence"
+        ir_seq = clodoo.browseL8(ctx, resource_sequence, journal.sequence_id.id)
+        prefix = ir_seq.prefix.replace("%(year)s", "%(range_year)s")
+        if prefix != ir_seq.prefix:
+            clodoo.writeL8(ctx, resource_sequence, ir_seq.id, {"prefix": prefix})
+        parts = name.split("/")
+        if len(parts) == 3 and len(parts[1]) == 4 and parts[1].startswith("2"):
+            # i.e. "SAJ/2023/1234
+            next_number = int(parts[2]) + 1
+            year = int(parts[1])
+        elif (
+            len(parts) == 2 and len(parts[0]) == 4 and parts[0].startswith("2")
+        ):
+            # i.e. "2013/0123"
+            next_number = int(parts[1]) + 1
+            year = int(parts[0])
+        else:
+            print("Unrecognized number %s" % name)
+            return
+        range_ids = clodoo.searchL8(
+            ctx, resource_sequence_range, [
+                ("sequence_id", "=", journal.sequence_id.id),
+                ("date_from", ">=", "%d-01-01" % year),
+                ("date_to", "<=", "%d-12-31" % year),
+            ])
+        if len(range_ids) > 1:
+            print("Invalid sequence range %s for id %s" % (year, journal.code))
+        elif not range_ids:
+            clodoo.createL8(ctx, resource_sequence_range, {
+                "sequence_id": journal.sequence_id.id,
+                "date_from": "%d-01-01" % year,
+                "date_to": "%d-12-31" % year,
+                "number_next": next_number,
+                "number_next_actual": next_number,
+            })
+        else:
+            ir_seq_range = clodoo.browseL8(ctx, resource_sequence_range, range_ids[0])
+            if (
+                ir_seq_range.number_next < next_number
+                or ir_seq_range.number_next_actual < next_number
+            ):
+                clodoo.writeL8(ctx,
+                               resource_sequence_range,
+                               range_ids[0],
+                               {
+                                   "number_next": next_number,
+                                   "number_next_actual": next_number,
+                               })
+
+    print('🎺🎺🎺 Rebuild database')
+    if ctx['param_1'] == 'help':
+        print('rebuild database [no-invoice|no-reconcile]')
+        return
+
+    move_type_match = {
+        "out_invoice": "receivable",
+        "out_refund": "receivable_refund",
+        "in_invoice": "payable",
+        "in_refund": "payable_refund",
+        "bank": "liquidity",
+        "cash": "liquidity",
+    }
+    resource_invoice = "account.invoice"
+    resource_move = "account.move"
+    resource_journal = "account.journal"
+    # resource_sequence = "ir.sequence"
+    resource_sequence_range = "ir.sequence.date_range"
+    resource_att_out = "fatturapa.attachment.out"
+    # resource_att_in = "fatturapa.attachment.in"
+    ctr = 0
+
+    print("Resetting sequences ...")
+    for rec_id in clodoo.searchL8(ctx,
+                                  resource_journal,
+                                  [("update_posted", "=", False)]):
+        clodoo.writeL8(ctx, resource_journal, rec_id, {"update_posted": True})
+        ctr += 1
+    ctr += reset_sequence(ctx)
+
+    if not ctx['param_1'] or "no-rec" not in ctx['param_1']:
+        ctr += delete_reconciliations(ctx)
+
+    attachments = {}
+    if not ctx['param_1'] or "no-inv" not in ctx['param_1']:
+        ctr, attachments = cancel_inv_n_save_attachments(ctx)
+
+    ctr += cancel_moves(ctx)
+
+    if ctx['_cr']:
+        query = (
+            "update account_move_line"
+            " set account_id=2147"
+            " where account_id=5053"
+        )
+        clodoo.exec_sql(ctx, query)
+
+        query = (
+            "update account_move"
+            " set journal_id=29"
+            " where journal_id=23"
+        )
+        clodoo.exec_sql(ctx, query)
+        query = (
+            "update account_move_line"
+            " set journal_id=29"
+            " where journal_id=23"
+        )
+        clodoo.exec_sql(ctx, query)
+
+        query = (
+            "update account_move"
+            " set journal_id=39"
+            " where journal_id=12"
+        )
+        clodoo.exec_sql(ctx, query)
+        query = (
+            "update account_move_line"
+            " set journal_id=39"
+            " where journal_id=12"
+        )
+        clodoo.exec_sql(ctx, query)
+
+        query = (
+            "update account_move"
+            " set journal_id=40"
+            " where journal_id=13"
+        )
+        clodoo.exec_sql(ctx, query)
+        query = (
+            "update account_move_line"
+            " set journal_id=40"
+            " where journal_id=13"
+        )
+        clodoo.exec_sql(ctx, query)
+
+        query = (
+            "delete from account_move"
+            " where journal_id=22"
+        )
+        clodoo.exec_sql(ctx, query)
+
+    ctr += reset_taxes(ctx)
+
+    if not ctx['param_1'] or "no-inv" not in ctx['param_1']:
+        ctr += validate_invoices(ctx)
+
+    fn_attach_list = os.path.expanduser("~/attachments_saved.csv")
+    store_inv_att_file(ctx, attachments, fn_attach_list)
+
+    ctr += validate_moves(ctx)
+
+    print("%d records update!" % ctr)
+
+
+def move_database_by_postgres(ctx):
+    print('🎺🎺🎺 Move database from postgres version to another')
+    if ctx['param_1'] == 'help':
+        print('move_database_by_postgres pg_port_orig pg_port_dest role')
+        return
+    if not ctx.get('param_1'):
+        print("Missed postgres port of orig")
+        print('move_database_by_postgres pg_port_orig pg_port_dest role')
+        return
+    if not ctx.get('param_2'):
+        print("Missed postgres port of dest")
+        print('move_database_by_postgres pg_port_orig pg_port_dest role')
+        return
+    if not ctx.get('param_3'):
+        print("Missed postgres role")
+        print('move_database_by_postgres pg_port_orig pg_port_dest role')
+        return
+    if not ctx['_cr']:
+        print("Cannot connect via SQL")
+        return
+    pg_port_orig = ctx['param_1']
+    pg_port_dest = ctx['param_2']
+    role = ctx['param_3']
+    response = clodoo.exec_sql(
+        ctx,
+        ("SELECT d.datname,pg_catalog.pg_get_userbyid(d.datdba)"
+         " FROM pg_catalog.pg_database d order by d.datname"),
+        response=True)
+    dry_run = False
+    sqlfn = os.path.expanduser("~/db.sql")
+    ctr = 0
+    for rec in response:
+        db = rec[0]
+        if (
+            db.startswith("template")
+            or db.startswith("test")
+            or db.startswith("postgres")
+            or db.startswith("demo")
+            or db.startswith("oca")
+        ):
+            continue
+        owner = rec[1]
+        if owner != role:
+            continue
+        if os.path.isfile(sqlfn):
+            os.unlink(sqlfn)
+        sts, stdout, stderr = z0lib.run_traced(
+            "pg_dump -p%s -d \"%s\" -U%s -Fp -f %s" % (pg_port_orig, db, role, sqlfn),
+            verbose=True, dry_run=dry_run)
+        print(stdout)
+        if not dry_run and sts:
+            print("Error %d" % sts)
+            print(stderr)
+            return
+        if not os.path.isfile(sqlfn):
+            print("Non sql file %s found" % sqlfn)
+            return
+        sts, stdout, stderr = z0lib.run_traced(
+            "createdb -p%s -U%s \"%s\"" % (pg_port_dest, role, db),
+            verbose=True, dry_run=dry_run)
+        print(stdout)
+        if not dry_run and sts:
+            print("Error %d" % sts)
+            print(stderr)
+            return
+        sts, stdout, stderr = z0lib.run_traced(
+            "psql -p%s -U%s \"%s\" -f %s" % (pg_port_dest, role, db, sqlfn),
+            verbose=True, dry_run=dry_run)
+        # print(stdout)
+        if not dry_run and sts:
+            print("Error %d" % sts)
+            print(stderr)
+            return
+        os.unlink(sqlfn)
+        ctr += 1
+    print("%d databases moved")
+
+
 if ctx['function']:
     function = ctx['function']
     globals()[function](ctx)
     exit()
 
 print('Avaiable functions:')
 print(' SALE ORDER                      ACCOUNT INVOICE')
@@ -4374,15 +4322,15 @@
 print(' - set_products_delivery_policy  - unlink_ddt_from_invoice')
 print(' - set_fiscal_on_products        COMMISSION')
 print(' ACCOUNT                         - create_commission_env')
 print(' - create_RA_config              DELIVERY/SHIPPING')
 print(' - manage_due_line               - change_ddt_number')
 print(' PARTNER/USER                    - create_delivery_env')
 print(' - check_integrity_by_vg7        - show_empty_ddt')
-print(' - configure_fiscal_position     RIBA')
+print('                                 RIBA')
 print(' - set_ppf_on_partner            - configure_RiBA')
 print(' - deduplicate_partner           - manage_riba')
 print(' - reset_email_admins             OTHER TABLES')
 print(' - solve_unamed                   - set_report_config')
 print(' - solve_flag_einvoice            - setup_balance_report')
 print(' - simulate_user_profile          - show_module_group')
 print(' SYSTEM                           - check_rec_links')
```

### Comparing `odoo_score-2.0.3/odoo_score/scripts/setup.info` & `odoo_score-2.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='odoo_score',
-    version='2.0.3',
+    version='2.0.5',
     description='Odoo super core',
     long_description="""
 Odoo supercore
 
 odoo_score is a library that extends the odoo orm functionality
 and makes available a simple odoo shell.
 """,
@@ -14,14 +14,15 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: System Shells',
     ],
     keywords='odoo',
     url='https://zeroincombenze-tools.readthedocs.io',
@@ -33,17 +34,19 @@
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
     install_requires=['z0lib', 'future'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': [
         'scripts/setup.info',
         'scripts/run_odoo_debug.sh',
-        './set_workers']},
+        './set_workers',
+        './models_barely',
+    ]},
     entry_points={
         'console_scripts': [
             'odoo_score-info = odoo_score.scripts.main:main',
             'rename_odoo_module = odoo_score.scripts.rename_odoo_module:main',
-            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
+            # 'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `odoo_score-2.0.3/odoo_score/scripts/main.py` & `odoo_score-2.0.5/odoo_score/scripts/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.5"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `odoo_score-2.0.3/odoo_score/scripts/run_odoo_debug.py` & `odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.py`

 * *Files identical despite different names*

### Comparing `odoo_score-2.0.3/odoo_score/scripts/run_odoo_debug.sh` & `odoo_score-2.0.5/odoo_score/scripts/run_odoo_debug.sh`

 * *Files 7% similar despite different names*

```diff
@@ -23,27 +23,25 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 ODOOLIBDIR=$(findpkg odoorc "$PYPATH" "clodoo")
 [[ -z "$ODOOLIBDIR" ]] && echo "Library file odoorc not found!" && exit 72
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 # ODOO_ROOT=$(readlink -f $HOME_DEVEL/..)
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.3
+__version__=2.0.5
 
 run_traced_debug() {
     if [[ $opt_verbose -gt 1 ]]; then
         run_traced "$1"
     elif [[ $opt_dry_run -eq 0 ]]; then
         eval $1
     fi
@@ -119,35 +117,70 @@
     [[ $PRJNAME == "Odoo" ]] && UMLI="${GIT_ORGID}${odoo_ver}" || UMLI="${GIT_ORGID}"
     [[ -n "$REPOSNAME" && $REPOSNAME != "OCB" ]] && UMLI="${UMLI}.${REPOSNAME//,/+}"
     [[ -n $m ]] && UMLI="${UMLI}.$m"
 #    if [[ -n $opt_flog ]]; then
 #      LOGDIR="$(dirname $opt_flog)"
 #      LOGFILE="$opt_flog"
 #    else
-      LOGDIR="$(get_cfg_value "" "LOGDIR")"
-      [[ -z $LOGDIR ]] && LOGDIR="$ODOO_ROOT/travis_log"
-      [[ -d $LOGDIR ]] || mkdir $LOGDIR
-      LOGFILE="$LOGDIR/${UMLI}.log"
+#      LOGDIR="$(get_cfg_value "" "LOGDIR")"
+#      [[ -z $LOGDIR ]] && LOGDIR="$ODOO_ROOT/travis_log"
+#      [[ -d $LOGDIR ]] || mkdir $LOGDIR
+#      LOGFILE="$LOGDIR/${UMLI}.log"
 #    fi
-    OLD_LOGFILE=${LOGFILE/.log/_old.log}
+    LOGDIR="$PKGPATH/tests/logs"
+    # [[ -d $LOGDIR ]] || mkdir $LOGDIR
+    LOGFILE="$LOGDIR/${PKGNAME}_$(date +%Y%m%d).txt"
+    [[ -f $LOGFILE ]] && rm -f $LOGFILE
+    # OLD_LOGFILE=${LOGFILE/.log/_old.log}
     # set +x  #debug
 }
 
 check_path_n_branch() {
     # check_path_n_branch(path branch)
     local x
     [[ -n $1 ]] && odoo_fver=$(build_odoo_param FULLVER "$1") || odoo_fver=""
     [[ -n $2 ]] && x=$(build_odoo_param FULLVER "$2") || x=""
     [[ -n $odoo_fver && -n $x && $odoo_fver != $x ]] && echo "Version mismatch -p $1 != -b $2" && exit 1
     [[ -z $odoo_fver ]] && odoo_fver=$x
 }
 
+replace_web_module() {
+    # replace_web_module()
+    local l m param z w woca
+    woca="$ODOO_RUNDIR/addons/_web_oca"
+    w="$ODOO_RUNDIR/addons/web"
+    if [[ $odoo_ver -le 7 ]]; then
+        z=""
+        l=""
+        param=$(grep -E "^server_wide_modules *=.*" $FULL_LCONFN|cut -d"=" -f2|tr -d " ")
+        [[ $param == "Non" ]] && param=""
+        if [[ -n $param ]]; then
+          for m in ${param//,/ }; do
+              [[ $m =~ ^(web|web_kanban|None)$ ]] && continue
+              [[ $m == "web_zeroincombenze" ]] && z=$m || l="$l,$m"
+          done
+          [[ -n $l ]] && OPTS="$OPTS --load=\"${l:1}\""
+        fi
+        if [[ -z $z ]]; then
+            [[ -L $w ]] && rm -f $w
+            [[ -d $woca ]] && mv $woca $w
+        else
+            z=$(find $ODOO_RUNDIR -type f -path "*/$z/*" -not -path "*/doc/*" -name "__openerp__.py"|head -n 1)
+            if [[ -n $z ]]; then
+                z=$(dirname $z)
+                [[ ! -d $woca ]] && mv $w $woca
+                [[ ! -L $w ]] && ln -s $z $w
+            fi
+        fi
+    fi
+}
+
 
 OPTOPTS=(h        B       b          c        C           d        e       f         k        i       I       l        L        m           M         n           o         O      p        P         q           S        s        T        t         U          u       V           v           w       W        x)
-OPTLONG=(help     debug   branch     conf     no-coverage database export  force     keep     import  install lang     lint-lev modules     multi     dry-run     ""        ""     path     psql-port quiet       stat     stop     test     ""        db-user    update  version     verbose     web     ""       xmlrpc-port)
+OPTLONG=(help     debug   branch     config   no-coverage database export  force     keep     import  install lang     lint-lev modules     multi     dry-run     ""        ""     path     psql-port quiet       stat     stop     test     ""        db-user    update  version     verbose     web     ""       xmlrpc-port)
 OPTDEST=(opt_help opt_dbg opt_branch opt_conf opt_nocov   opt_db   opt_exp opt_force opt_keep opt_imp opt_xtl opt_lang opt_llvl opt_modules opt_multi opt_dry_run opt_ofile opt_ou opt_odir opt_qport opt_verbose opt_stat opt_stop opt_test opt_touch opt_dbuser opt_upd opt_version opt_verbose opt_web opt_venv opt_rport)
 OPTACTI=("+"      "+"     "=>"       "=>"     1           "="      1       1         1        1       1       1        "="      "="         1         1           "="       1      "="      "="       0           1        1        1        1         "="        1       "*>"        "+"         1       1        "=")
 OPTDEFL=(1        0       ""         ""       0           ""       0       0         0        0       0       0        ""       ""          -1        0           ""        0      ""       ""        0           0        0        0        0         ""         0       ""          -1          0       0        "")
 OPTMETA=("help"   ""      "version"  "fname"  ""          "name"   ""      ""        ""       ""      ""      ""       "level"  "modules"   ""        "no op"     "file"    ""     "dir"    "port"    ""          ""       ""       ""       "touch"   "user"     ""      "version"   "verbose"   0       ""       "port")
 OPTHELP=("this help"
     "debug mode (-BB debug via pycharm)"
     "odoo branch (version id)"
@@ -301,15 +334,14 @@
     opt_lang=0 opt_exp=0 opt_imp=0
     opt_upd=0 opt_stop=1
     opt_xtl=1
     [[ $opt_dbg -ne 0 ]] && opt_nocov=1 || opt_nocov=0
     [[ -z $opt_db && $opt_keep -eq 0 ]] && opt_db="test_${UDI}" && drop_db=1
     [[ -z $opt_db && $opt_keep -ne 0 ]] && opt_db="${MQT_TEST_DB}_${odoo_ver}" && drop_db=0
     create_db=1
-    # [[ $opt_keep -eq 0 ]] && drop_db=1 || drop_db=0
     [[ ! -d $ODOO_ROOT/travis_log ]] && run_traced "mkdir $ODOO_ROOT/travis_log"
 elif [[ $opt_lang -ne 0 ]]; then
     opt_keep=1
     opt_stop=1
     [[ -n "$opt_modules" ]] && opt_modules=
 elif [[ $opt_exp -ne 0 || $opt_imp -ne 0 ]]; then
     opt_keep=1
@@ -420,25 +452,27 @@
     exit 0
 fi
 
 if [[ $opt_touch -eq 0 ]]; then
     [[ -n "$VDIR" ]] && ve_root=$VDIR || ve_root=$HOME
     OPT_LLEV=
     # [[ $opt_test -ne 0 && ! -d $HOME/tmp ]] && mkdir $HOME/tmp
+    [[ $opt_test -ne 0 && ! -d $LOGDIR ]] && mkdir -p $LOGDIR
     [[ $opt_test -ne 0 ]] && FULL_LCONFN="$LOGDIR/${UMLI}.conf" || FULL_LCONFN="$ve_root/$LCONFN"
     [[ $opt_test -gt 1 ]] && FULL_LCONFN="$ve_root/pycharm_odoo.conf"
     OPT_CONF="--config=$FULL_LCONFN"
     if [[ $opt_dry_run -eq 0 ]]; then
         for f in .openerp_serverrc .odoorc; do
             for d in $HOME $ve_root; do
                 [[ -f $d/$f ]] && rm -f $d/$f
             done
         done
     fi
     [[ -f "$CONFN" ]] && run_traced "cp $CONFN $FULL_LCONFN"
+    replace_web_module
     # [[ $opt_verbose -gt 0 ]] && echo "===================================================================="
     [[ ! -f "$CONFN" ]] && run_traced "$script -s --stop-after-init"
     tty -s
     if [[ $? == 0 ]]; then
         run_traced_debug "sed -e \"s|^logfile *=.*|logfile = False|\" -i $FULL_LCONFN"
     else
         run_traced_debug "sed -e \"s|^logfile *=.*|logfile = $ve_root/$$.log|\" -i $FULL_LCONFN"
@@ -463,15 +497,16 @@
         OPT_LLEV="--log-level=$opt_llvl"
     fi
     run_traced_debug "sed -e \"s|^workers *=.*|workers = 0|\" -i $FULL_LCONFN"
 
     if [[ -n "$VDIR" ]]; then
       coverage_set
       x=$(date +"%Y-%m-%d %H:%M:%S,000")
-      [[ $opt_verbose -gt 0 ]] && echo "$x $$ DAEMON ? $(basename $0): cd $VDIR; source ./bin/activate"
+      [[ $opt_verbose -gt 0 && $opt_test -eq 0 ]] && echo "$x $$ DAEMON ? $(basename $0): cd $VDIR; source ./bin/activate"
+      [[ $opt_verbose -gt 0 && $opt_test -ne 0 ]] && echo "$x $$ DAEMON ? $(basename $0): cd $VDIR; source ./bin/activate" | tee -a $LOGFILE
       if [[ $opt_dry_run -eq 0 ]]; then
         cd $VDIR
         source ./bin/activate
         if [[ $opt_test -ne 0 && $opt_nocov -eq 0 ]]; then
           cov=$(which coverage 2>/dev/null)
           [[ -z $cov || ! $cov =~ $HOME ]] && run_traced "pip install coverage"
           cov=$(which coverage 2>/dev/null)
@@ -479,97 +514,114 @@
             v=$(coverage --version|grep --color=never -Eo "[0-9]+"|head -n1)
             [[ $v -lt 5 ]] && run_traced "pip install coverage -U"
           fi
         fi
       fi
     fi
 
-    [[ $opt_keep -ne 0 ]] && export ODOO_COMMIT_TEST="1"
-    [[ $opt_keep -eq 0 && -n $ODOO_COMMIT_TEST ]] && unset ODOO_COMMIT_TEST
+    [[ -n $ODOO_COMMIT_TEST ]] && unset ODOO_COMMIT_TEST
     if [[ $create_db -gt 0 ]]; then
         [[ -n "$DB_PORT" ]] && opts="-U$DB_USER -p$DB_PORT" || opts="-U$DB_USER"
         if [[ -n "$depmods" && $opt_test -ne 0 ]]; then
             c="cd $ODOO_RUNDIR; $script $OPTDB $OPT_CONF --log-level=error -i $depmods"
             cmd="$c $OPT_CONFPORT"
             TEMPLATE="${opt_db/test/template}"
             [[ $opt_keep -ne 0 ]] && TEMPLATE="${MQT_TEMPLATE_DB}_${odoo_ver}"
             [[ opt_dbg -gt 1 && $opt_keep -eq 0 ]] && TEMPLATE="template_${UDI}"
             cmd="${cmd/$opt_db/$TEMPLATE}"
             fnparam="$LOGDIR/${UDI}.sh"
             if [[ $opt_force -ne 0 || ! -f $fnparam ]] || ! echo $c|diff -qw $fnparam - || ! psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE"; then
               # Create DB for test
               run_traced "pg_db_active -L -wa '$TEMPLATE' && dropdb $opts --if-exists '$TEMPLATE'"
-              psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE" && echo "Database $TEMPLATE removal failed!" && exit 1
-              run_traced "$cmd"
-              run_traced "pg_db_active -L '$TEMPLATE'"
+              if [[ $opt_dry_run -eq 0 ]]; then
+                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE" && echo "Database $TEMPLATE removal failed!" && exit 1
+                run_traced "$cmd"
+                run_traced "pg_db_active -L '$TEMPLATE'"
+              fi
             fi
             if psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE"; then
               [[ $opt_dry_run -eq 0 ]] && echo $c > $fnparam
               run_traced "pg_db_active -L -wa '$opt_db' && dropdb $opts --if-exists '$opt_db'"
-              psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$opt_db" && echo "Database $opt_db removal failed!" && exit 1
-              run_traced "pg_db_active -L -wa '$TEMPLATE'"
-              run_traced "psql -U$DB_USER template1 -c 'create database \"$opt_db\" owner $DB_USER template \"$TEMPLATE\"'"
+              if [[ $opt_dry_run -eq 0 ]]; then
+                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$opt_db" && echo "Database $opt_db removal failed!" && exit 1
+                run_traced "pg_db_active -L -wa '$TEMPLATE'"
+                run_traced "psql -U$DB_USER template1 -c 'create database \"$opt_db\" owner $DB_USER template \"$TEMPLATE\"'"
+              fi
             else
               echo "Template $TEMPLATE not found!"
               cmd="${cmd/$TEMPLATE$opt_db/}"
               run_traced "$cmd"
             fi
        else
             run_traced "cd $ODOO_RUNDIR; $script $OPTDB $OPT_CONF --log-level=error"
        fi
     fi
 
+    [[ $opt_keep -ne 0 ]] && export ODOO_COMMIT_TEST="1"
     if [[ $opt_test -ne 0 && $opt_dbg -eq 0 ]]; then
-      [[ -f $LOGFILE ]] && rm -f $LOGFILE
-      if [[ -n $COVERAGE_PROCESS_START ]]; then
-        v=$(coverage --version|grep --color=never -Eo "[0-9]+"|head -n1)
-        if [[ $v -ge 6 ]]; then
-          run_traced "cd $ODOO_RUNDIR; coverage run --rcfile=$COVERAGE_PROCESS_START --data-file=$COVERAGE_DATA_FILE $script $OPT_CONF $OPT_LLEV $OPTS"
+        run_traced "pip list --format=freeze > $LOGDIR/requirements.txt"
+        if [[ -n $COVERAGE_PROCESS_START ]]; then
+            v=$(coverage --version|grep --color=never -Eo "[0-9]+"|head -n1)
+            if [[ $v -ge 6 ]]; then
+                run_traced "cd $ODOO_RUNDIR; coverage run --rcfile=$COVERAGE_PROCESS_START --data-file=$COVERAGE_DATA_FILE $script $OPT_CONF $OPT_LLEV $OPTS 2>&1 | stdbuf -i0 -o0 -e0 tee -a $LOGFILE"
+            else
+                run_traced "cd $ODOO_RUNDIR; coverage run --rcfile=$COVERAGE_PROCESS_START $script $OPT_CONF $OPT_LLEV $OPTS 2>&1 | stdbuf -i0 -o0 -e0 tee -a $LOGFILE"
+            fi
         else
-          run_traced "cd $ODOO_RUNDIR; coverage run --rcfile=$COVERAGE_PROCESS_START $script $OPT_CONF $OPT_LLEV $OPTS"
+            run_traced "cd $ODOO_RUNDIR; $script $OPT_CONF $OPT_LLEV $OPTS 2>&1 | stdbuf -i0 -o0 -e0 tee -a $LOGFILE"
         fi
-      else
-        run_traced "cd $ODOO_RUNDIR; $script $OPT_CONF $OPT_LLEV $OPTS"
-      fi
     elif [[ opt_dbg -gt 1 ]]; then
-      echo ""
-      echo "Now you can test module $opt_module on pycharm"
-      echo ""
-      echo "Debug Odoo by pycharm after set configuration \"Debug Odoo $odoo_fver\""
-      echo -e "parameters=\"\e[33m$script\e[0m \e[31m$OPT_CONF $OPT_LLEV $OPTS\e[0m\""
-      echo ""
-      echo "If your test code contains the follow statements"
-      echo ""
-      echo -e "    \e[33mdef tearDown(self):\e[0m"
-      echo -e "        \e[33mself.env.cr.commit()\e[0m  # pylint: disable=invalid-commit"
-      echo ""
-      echo "you can browse test database from:"
-      echo -e "\e[33mhttp://localhost:8069\e[0m or \e[33mhttp://localhost:$(build_odoo_param RPCPORT $odoo_fver)\e[0m"
-      echo -e "DB=\e[31m$opt_db\e[0m login: admin/admin"
-      echo ""
+        echo ""
+        echo "Now you can test module $opt_modules on pycharm"
+        echo ""
+        echo "Debug Odoo by pycharm after set configuration \"Debug Odoo $odoo_fver\""
+        echo -e "parameters=\"\e[33m$script\e[0m \e[31m$OPT_CONF $OPT_LLEV $OPTS\e[0m\""
+        echo ""
+        echo "If your test code contains the follow statements"
+        echo ""
+        echo -e "    \e[33mdef tearDown(self):\e[0m"
+        echo -e "        \e[33mself.env.cr.commit()\e[0m  # pylint: disable=invalid-commit"
+        echo ""
+        echo "you can browse test database from:"
+        echo -e "\e[33mhttp://localhost:8069\e[0m or \e[33mhttp://localhost:$(build_odoo_param RPCPORT $odoo_fver)\e[0m"
+        echo -e "DB=\e[31m$opt_db\e[0m login: admin/admin"
+        echo ""
     else
-      run_traced "cd $ODOO_RUNDIR; $script $OPT_CONF $OPT_LLEV $OPTS"
+        run_traced "cd $ODOO_RUNDIR; $script $OPT_CONF $OPT_LLEV $OPTS"
     fi
 
-    coverage_report
-
     if [[ -n "$VDIR" ]]; then
         x=$(date +"%Y-%m-%d %H:%M:%S,000")
         [[ $opt_verbose -gt 0 && opt_dbg -le 1 ]] && echo "$x $$ DAEMON ? $(basename $0): deactivate"
         [[ $opt_dry_run -eq 0 ]] && deactivate
     fi
     [[ $opt_test -ne 0 && -f $FULL_LCONFN ]] && rm -f FULL_LCONFN
     [[ -n $ODOO_COMMIT_TEST ]] && unset ODOO_COMMIT_TEST
-    if [[ $drop_db -gt 0 ]]; then
-        if [[ -z "$opt_modules" || $opt_stop -eq 0 ]]; then
-            [[ -n "$DB_PORT" ]] && opts="-U$DB_USER -p$DB_PORT" || opts="-U$DB_USER"
-            run_traced "pg_db_active -L -wa '$opt_db'; dropdb $opts --if-exists '$opt_db'"
-            [[ opt_dbg -ne 1 ]] && run_traced "pg_db_active -L -wa '$TEMPLATE'; dropdb $opts --if-exists '$TEMPLATE'"
+
+    if [[ $opt_test -ne 0 && $opt_dbg -eq 0 ]]; then
+        if [[ $opt_dry_run -eq 0 ]]; then
+            echo -e "\n+===================================================================" | tee -a $LOGFILE
+            grep -Eq " (ERROR|CRITICAL) " $LOGFILE && x="\e[31mFAILED!\e[0m" || x="\e[32mSUCCESS!\e[0m"
+            echo -e "| please test \e[36m${opt_modules}\e[0m (${odoo_fver}): $x" | tee -a $LOGFILE
+            echo -e "+===================================================================\n"  | tee -a $LOGFILE
+            coverage_report | tee -a $LOGFILE
+            echo "less -R \$(readlink -f \$(dirname \$0))/$(basename $LOGFILE)" > $LOGDIR/show-log.sh
+            chmod +x $LOGDIR/show-log.sh
+        else
+            run_traced "coverage_report | tee -a $LOGFILE"
         fi
     fi
     if [[ $opt_exp -ne 0 ]]; then
         makepo_it.py -b$odoo_fver -m$opt_modules $src
         echo "# Translation exported to '$src' file"
     elif [[ $opt_imp -ne 0 ]]; then
         echo "# Translation imported from '$src' file"
     fi
+
+    if [[ $drop_db -gt 0 ]]; then
+        if [[ -z "$opt_modules" || $opt_stop -eq 0 ]]; then
+            [[ -n "$DB_PORT" ]] && opts="-U$DB_USER -p$DB_PORT" || opts="-U$DB_USER"
+            run_traced "pg_db_active -L -wa '$opt_db'; dropdb $opts --if-exists '$opt_db'"
+            [[ opt_dbg -ne 1 ]] && run_traced "pg_db_active -L -wa '$TEMPLATE'; dropdb $opts --if-exists '$TEMPLATE'"
+        fi
+    fi
 fi
```

### Comparing `odoo_score-2.0.3/odoo_score/scripts/map_module_dependecies.py` & `odoo_score-2.0.5/odoo_score/scripts/map_module_dependecies.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # import os
 from datetime import datetime
 import argparse
 import ast
 from python_plus import unicodes
 
-__version__ = "2.0.3"
+__version__ = "2.0.5"
 
 
 class OdooMap(object):
     """ """
 
     def __init__(self, opt_args):
         self.opt_args = opt_args
```

### Comparing `odoo_score-2.0.3/odoo_score/scripts/rename_odoo_module.py` & `odoo_score-2.0.5/odoo_score/scripts/rename_odoo_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import argparse
 
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.3'
+__version__ = '2.0.5'
 
 
 def update_module_names(ctx, namespec, merge_modules=False):
     """Deal with changed module names, making all the needed changes on the
     related tables, like XML-IDs, translations, and so on.
 
     :param namespec: list of tuples of (old name, new name)
```

### Comparing `odoo_score-2.0.3/odoo_score/odoo_score.py` & `odoo_score-2.0.5/odoo_score/odoo_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     try:
         import oerplib  # noqa: F401
         __db_protocol__ = 'xml' if not __db_protocol__ else 'json+xml'
     except ImportError:
         pass
 
 
-__version__ = '2.0.3'
+__version__ = '2.0.5'
 
 MODULE_ID = 'odoo_score'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 class SingletonCache(object):
```

### Comparing `odoo_score-2.0.3/odoo_score/migrate.py` & `odoo_score-2.0.5/odoo_score/migrate.py`

 * *Files identical despite different names*

### Comparing `odoo_score-2.0.3/PKG-INFO` & `odoo_score-2.0.5/odoo_score.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 1.2
-Name: odoo_score
-Version: 2.0.3
+Metadata-Version: 2.1
+Name: odoo-score
+Version: 2.0.5
 Summary: Odoo super core
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Odoo supercore
-        
-        odoo_score is a library that extends the odoo orm functionality
-        and makes available a simple odoo shell.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+Odoo supercore
+
+odoo_score is a library that extends the odoo orm functionality
+and makes available a simple odoo shell.
+
+
```

### Comparing `odoo_score-2.0.3/README.rst` & `odoo_score-2.0.5/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 
 ================
-odoo_score 2.0.3
+odoo_score 2.0.5
 ================
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
 
 
 Overview
 ========
 
 Odoo supercore
 
-odoo_score is a library that extends the odoo orm functionality and makes available a simple odoo shell.
+odoo_score is a library that extends the odoo orm functionality and makes available
+a simple odoo shell even for older Odoo version.
 
+In order to complete all full tests, it required to test the
+Odoo module test_odoo_score-* in repository
+`zerobug_test <https://github.com/zeroincombenze/zerobug-test.git>`
 
 
 odoo_shell
 ----------
 
 Odoo shell is a simple line command shell to manager Odoo database using the internal Odoo functions.
 
@@ -146,14 +150,29 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.6 (2023-04-16)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] Import class models.Model
+
+2.0.5 (2023-03-23)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] run_odoo_debug.sh: moved to package wok_code
+
+2.0.4 (2023-01-13)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] run_odoo_debug.sh: test creates log
+
 2.0.3 (2022-11-11)
 ~~~~~~~~~~~~~~~~~~
 
 * [IMP] odoo_score: implementation of models and fields for Odoo 8-0+ modules
 
 2.0.2 (2022-10-20)
 ~~~~~~~~~~~~~~~~~~
@@ -209,21 +228,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2022-11-20
+Last Update / Ultimo aggiornamento: 2023-04-23
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

