# Comparing `tmp/zar-2.0.0.tar.gz` & `tmp/zar-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zar-2.0.0.tar", last modified: Mon Oct 31 15:13:53 2022, max compression
+gzip compressed data, was "zar-2.0.1.tar", last modified: Sun Apr 23 14:04:27 2023, max compression
```

## Comparing `zar-2.0.0.tar` & `zar-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-10-31 15:13:53.000000 zar-2.0.0/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-10-31 15:13:53.000000 zar-2.0.0/zar/
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      164 2022-09-09 18:30:59.000000 zar-2.0.0/zar/__main__.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)       46 2022-10-15 13:20:30.000000 zar-2.0.0/zar/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-10-31 15:13:53.000000 zar-2.0.0/zar.egg-info/
--rw-r--r--   0 odoo      (1000) odoo      (1000)        4 2022-10-31 15:13:53.000000 zar-2.0.0/zar.egg-info/top_level.txt
--rw-r--r--   0 odoo      (1000) odoo      (1000)        1 2022-10-31 15:13:53.000000 zar-2.0.0/zar.egg-info/dependency_links.txt
--rw-r--r--   0 odoo      (1000) odoo      (1000)        1 2022-09-09 18:30:59.000000 zar-2.0.0/zar.egg-info/not-zip-safe
--rw-r--r--   0 odoo      (1000) odoo      (1000)      185 2022-10-31 15:13:53.000000 zar-2.0.0/zar.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-10-31 15:13:53.000000 zar-2.0.0/zar.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2022-10-31 15:13:53.000000 zar-2.0.0/setup.cfg
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     1261 2022-10-21 11:42:37.000000 zar-2.0.0/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-10-31 15:13:53.000000 zar-2.0.0/PKG-INFO
--rw-r--r--   0 odoo      (1000) odoo      (1000)     6118 2022-10-31 15:13:52.000000 zar-2.0.0/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1199 2023-04-23 14:04:27.171901 zar-2.0.1/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6678 2023-04-23 14:04:26.000000 zar-2.0.1/README.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:04:27.171901 zar-2.0.1/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1359 2023-02-25 14:51:46.000000 zar-2.0.1/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/zar/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 zar-2.0.1/zar/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zar-2.0.1/zar/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:04:27.171901 zar-2.0.1/zar.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1199 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      185 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 09:05:11.000000 zar-2.0.1/zar.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        4 2023-04-23 14:04:27.000000 zar-2.0.1/zar.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zar-2.0.0/zar.egg-info/PKG-INFO` & `zar-2.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zar
-Version: 2.0.0
+Version: 2.0.1
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        ZAR stand for Zeroincombenze® Archive Replica.
-        It is a tool kit to backup, restore, replicate files and/or database.
-        
-        ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: backup,restore,replica
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+ZAR stand for Zeroincombenze® Archive Replica.
+It is a tool kit to backup, restore, replicate files and/or database.
+
+ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
+
+
```

### Comparing `zar-2.0.0/setup.py` & `zar-2.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='zar',
-    version='2.0.0',
+    version='2.0.1',
     description='Zeroincombenze Archive Replica',
     long_description="""
 ZAR stand for Zeroincombenze® Archive Replica.
 It is a tool kit to backup, restore, replicate files and/or database.
 
 ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
 """,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: System Shells',
     ],
     keywords='backup, restore, replica',
     project_urls={
```

### Comparing `zar-2.0.0/PKG-INFO` & `zar-2.0.1/zar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zar
-Version: 2.0.0
+Version: 2.0.1
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        ZAR stand for Zeroincombenze® Archive Replica.
-        It is a tool kit to backup, restore, replicate files and/or database.
-        
-        ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: backup,restore,replica
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+ZAR stand for Zeroincombenze® Archive Replica.
+It is a tool kit to backup, restore, replicate files and/or database.
+
+ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
+
+
```

### Comparing `zar-2.0.0/README.rst` & `zar-2.0.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
-============
-zar 1.3.36
-============
+=========
+zar 2.0.1
+=========
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
-.. contents::
 
 
 Overview
 ========
 
 zar
 ===
@@ -36,19 +35,45 @@
 * backup and restore based on rules by configuration file
 * restore database with automatic actions disabled
 * multiple copies of database by configuration file
 * automatic purging of oldest copies
 * configuration based on host name: it works on duplicate host image too
 * backup on same host or on remote host
 
+
+|
+
+Usage
+=====
+
+zar should be execute by postgres user
+
+Execute zar_upd to install and configure.
+Configuration file is zar.conf
+Execute zar_bck to do backup or restore, based on host role
+Execute zar_rest to do restore
+
+To execute in cron, use zar_bck -k
+
+
+There are avaiable two postgresql facilities:
+
+* pg_db_active
+* pg_db_reassign owner
+
+`pg_db_active` show and kill postgres session. It can kill oldest session out of pool.
+
+`pg_db_reassign_owner` can reassign owner to database. It reassign the ownership of all objects.
+
+
 |
 |
 
-Quick start
-===========
+Getting started
+===============
 
 
 |
 
 Installation
 ------------
 
@@ -60,44 +85,60 @@
 
 `cd $HOME`
 `git@github.com:zeroincombenze/tools.git`
 `cd $HOME/tools`
 `./install_tools.sh`
 
 
+Upgrade
+-------
+
+Upgrade
+-------
+
+Stable version via Python Package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    pip install zar -U
+
 |
 
-Usage
-=====
+Current stable version
+~~~~~~~~~~~~~~~~~~~~~~
 
-zar should be execute by postgres user
+::
 
-Execute zar_upd to install and configure.
-Configuration file is zar.conf
-Execute zar_bck to do backup or restore, based on host role
-Execute zar_rest to do restore
+    cd $HOME
+    ./install_tools.sh -U
+    source /opt/odoo/devel/activate_tools
 
-To execute in cron, use zar_bck -k
+Current development version
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+::
 
-There are avaiable two postgresql facilities:
+    cd $HOME
+    ./install_tools.sh -Ud
+    source /opt/odoo/devel/activate_tools
 
-* pg_db_active
-* pg_db_reassign owner
 
-`pg_db_active` show and kill postgres session. It can kill oldest session out of pool.
+History
+-------
 
-`pg_db_reassign_owner` can reassign owner to database. It reassign the ownership of all objects.
+2.0.1 (2023-02-25)
+~~~~~~~~~~~~~~~~~~
 
+* [IMP] Remote bckdir different from local
+
+2.0.0 (2022-10-20)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Stable version
 
-|
-|
 
-Get involved
-============
 
 |
 |
 
 Credits
 =======
 
@@ -107,51 +148,54 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2019-11-11
+Last Update / Ultimo aggiornamento: 2023-04-23
 
-.. |Maturity| image:: https://img.shields.io/badge/maturity-Alfa-red.png
+.. |Maturity| image:: https://img.shields.io/badge/maturity-Alfa-black.png
     :target: https://odoo-community.org/page/development-status
-    :alt: Alfa
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=.
-    :target: https://travis-ci.org/zeroincombenze/tools
+    :alt: 
+.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
+    :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=.
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=.
+.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
+    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
     :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/./graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/.
+.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
+    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
     :alt: Codecov
-.. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-0.svg
-    :target: https://wiki.zeroincombenze.org/en/Odoo/./dev
+.. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
+    :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
-.. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-0.svg
-    :target: https://wiki.zeroincombenze.org/it/Odoo/./man
+.. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
+    :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
-.. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-0.svg
-    :target: https://erp0.zeroincombenze.it
+.. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
+    :target: https://erp2.zeroincombenze.it
     :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/./graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/.
+.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
+    :target: https://codecov.io/gh/OCA/tools/branch/2.0
     :alt: Codecov
 .. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
    :target: https://odoo-italia.org
    :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
@@ -172,9 +216,10 @@
 .. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
    :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
 .. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
    :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
 .. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
    :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
 .. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
-   :target: https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b
+   :target: https://t.me/Assitenza_clienti_powERP
+
```

