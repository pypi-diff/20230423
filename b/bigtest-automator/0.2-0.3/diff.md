# Comparing `tmp/bigtest_automator-0.2.tar.gz` & `tmp/bigtest_automator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtest_automator-0.2.tar", last modified: Sun Apr 23 16:06:18 2023, max compression
+gzip compressed data, was "bigtest_automator-0.3.tar", last modified: Sun Apr 23 16:18:36 2023, max compression
```

## Comparing `bigtest_automator-0.2.tar` & `bigtest_automator-0.3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.817711 bigtest_automator-0.2/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:06:18.817564 bigtest_automator-0.2/PKG-INFO
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.810818 bigtest_automator-0.2/bigtest_automator.egg-info/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/PKG-INFO
--rw-r--r--   0 shantharamp   (502) staff       (20)      798 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/SOURCES.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/dependency_links.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       68 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/entry_points.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/requires.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       66 2023-04-23 16:06:18.000000 bigtest_automator-0.2/bigtest_automator.egg-info/top_level.txt
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.812370 bigtest_automator-0.2/core_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.2/core_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6620 2023-04-22 06:17:51.000000 bigtest_automator-0.2/core_utils/generate_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.2/core_utils/run_scp.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.2/core_utils/run_vmstat.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.2/core_utils/take_awr_snapshot.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.813638 bigtest_automator-0.2/internal_db_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.2/internal_db_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1236 2023-04-22 06:33:13.000000 bigtest_automator-0.2/internal_db_management/db_ops.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.2/internal_db_management/get_server_details.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1086 2023-04-03 11:48:57.000000 bigtest_automator-0.2/internal_db_management/pwd_handler.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.814657 bigtest_automator-0.2/oracle_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.2/oracle_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.2/oracle_utils/oracle_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.2/oracle_utils/remote_oracle_db_connector.py
--rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-23 16:06:18.817757 bigtest_automator-0.2/setup.cfg
--rw-r--r--   0 shantharamp   (502) staff       (20)      677 2023-04-23 16:04:38.000000 bigtest_automator-0.2/setup.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.815709 bigtest_automator-0.2/temp/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.2/temp/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.2/temp/initiator.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.2/temp/playground.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:06:18.816984 bigtest_automator-0.2/ui_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.2/ui_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.2/ui_management/dynamic_logger.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.2/ui_management/grid.py
--rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.2/ui_management/tk_page_layouts.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.963812 bigtest_automator-0.3/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:18:36.963649 bigtest_automator-0.3/PKG-INFO
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.955704 bigtest_automator-0.3/bigtest_automator.egg-info/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/PKG-INFO
+-rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       79 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/entry_points.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/requires.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-23 16:18:36.000000 bigtest_automator-0.3/bigtest_automator.egg-info/top_level.txt
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.957502 bigtest_automator-0.3/core_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.3/core_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6620 2023-04-22 06:17:51.000000 bigtest_automator-0.3/core_utils/generate_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.3/core_utils/run_scp.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.3/core_utils/run_vmstat.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.3/core_utils/take_awr_snapshot.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.958573 bigtest_automator-0.3/entrypoint/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.3/entrypoint/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1708 2023-04-23 15:23:40.000000 bigtest_automator-0.3/entrypoint/initialize.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      647 2023-04-23 16:17:30.000000 bigtest_automator-0.3/entrypoint/main_class.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.959694 bigtest_automator-0.3/internal_db_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.3/internal_db_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1236 2023-04-22 06:33:13.000000 bigtest_automator-0.3/internal_db_management/db_ops.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.3/internal_db_management/get_server_details.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1086 2023-04-03 11:48:57.000000 bigtest_automator-0.3/internal_db_management/pwd_handler.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.960648 bigtest_automator-0.3/oracle_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.3/oracle_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.3/oracle_utils/oracle_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.3/oracle_utils/remote_oracle_db_connector.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-23 16:18:36.963867 bigtest_automator-0.3/setup.cfg
+-rw-r--r--   0 shantharamp   (502) staff       (20)      688 2023-04-23 16:18:12.000000 bigtest_automator-0.3/setup.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.961601 bigtest_automator-0.3/temp/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.3/temp/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.3/temp/initiator.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.3/temp/playground.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:18:36.962854 bigtest_automator-0.3/ui_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.3/ui_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.3/ui_management/dynamic_logger.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.3/ui_management/grid.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.3/ui_management/tk_page_layouts.py
```

### Comparing `bigtest_automator-0.2/bigtest_automator.egg-info/SOURCES.txt` & `bigtest_automator-0.3/bigtest_automator.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 bigtest_automator.egg-info/requires.txt
 bigtest_automator.egg-info/top_level.txt
 core_utils/__init__.py
 core_utils/generate_awr.py
 core_utils/run_scp.py
 core_utils/run_vmstat.py
 core_utils/take_awr_snapshot.py
+entrypoint/__init__.py
+entrypoint/initialize.py
+entrypoint/main_class.py
 internal_db_management/__init__.py
 internal_db_management/db_ops.py
 internal_db_management/get_server_details.py
 internal_db_management/pwd_handler.py
 oracle_utils/__init__.py
 oracle_utils/oracle_awr.py
 oracle_utils/remote_oracle_db_connector.py
```

### Comparing `bigtest_automator-0.2/core_utils/generate_awr.py` & `bigtest_automator-0.3/core_utils/generate_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/core_utils/run_scp.py` & `bigtest_automator-0.3/core_utils/run_scp.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/core_utils/run_vmstat.py` & `bigtest_automator-0.3/core_utils/run_vmstat.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/core_utils/take_awr_snapshot.py` & `bigtest_automator-0.3/core_utils/take_awr_snapshot.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/internal_db_management/db_ops.py` & `bigtest_automator-0.3/internal_db_management/db_ops.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/internal_db_management/get_server_details.py` & `bigtest_automator-0.3/internal_db_management/get_server_details.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/internal_db_management/pwd_handler.py` & `bigtest_automator-0.3/internal_db_management/pwd_handler.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/oracle_utils/oracle_awr.py` & `bigtest_automator-0.3/oracle_utils/oracle_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/oracle_utils/remote_oracle_db_connector.py` & `bigtest_automator-0.3/oracle_utils/remote_oracle_db_connector.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/setup.py` & `bigtest_automator-0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bigtest_automator',
-    version='0.2',
+    version='0.3',
     author='Shantharam Puranik M',
     author_email='shantharam.puranik@ellucian.com',
     description='A small tool that helps to run and collect performance related metrics such as VMSTAT and AWR. Highly specific to my ORG, might not be useful for general public. SORRY! - Noob.',
     packages=find_packages(),
     install_requires=[
         'scp',
         'paramiko',
         'oracledb'
     ],
     entry_points={
         'console_scripts': [
-            'reportscraper=bigtest_automator.main_class:main',
+            'reportscraper=bigtest_automator.entrypoint.main_class:main',
             # Add other command-line tools here
         ],
     },
 )
```

### Comparing `bigtest_automator-0.2/temp/playground.py` & `bigtest_automator-0.3/temp/playground.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.2/ui_management/tk_page_layouts.py` & `bigtest_automator-0.3/ui_management/tk_page_layouts.py`

 * *Files identical despite different names*

