# Comparing `tmp/pvmodule-0.0.98.tar.gz` & `tmp/pvmodule-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pvmodule-0.0.98.tar", last modified: Wed Mar  8 22:23:09 2023, max compression
+gzip compressed data, was "dist\pvmodule-0.0.99.tar", last modified: Wed Mar  8 22:26:25 2023, max compression
```

## Comparing `pvmodule-0.0.98.tar` & `pvmodule-0.0.99.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 22:23:09.929419 pvmodule-0.0.98/
--rw-rw-rw-   0        0        0    24475 2023-03-08 22:23:09.928421 pvmodule-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0    19701 2023-03-04 22:29:07.000000 pvmodule-0.0.98/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 22:23:09.906417 pvmodule-0.0.98/pvmodule/
--rw-rw-rw-   0        0        0      276 2023-01-31 14:18:52.000000 pvmodule-0.0.98/pvmodule/__init__.py
--rw-rw-rw-   0        0        0     3226 2023-03-07 20:27:34.000000 pvmodule-0.0.98/pvmodule/inverter.py
--rw-rw-rw-   0        0        0    18001 2023-03-08 22:22:54.000000 pvmodule-0.0.98/pvmodule/irradiance.py
--rw-rw-rw-   0        0        0     5459 2023-03-05 12:55:45.000000 pvmodule-0.0.98/pvmodule/location.py
--rw-rw-rw-   0        0        0     4007 2023-03-07 20:27:45.000000 pvmodule-0.0.98/pvmodule/module.py
--rw-rw-rw-   0        0        0    26704 2023-03-02 16:16:53.000000 pvmodule-0.0.98/pvmodule/pvgis.py
--rw-rw-rw-   0        0        0     3599 2023-03-08 10:36:33.000000 pvmodule-0.0.98/pvmodule/simulation.py
--rw-rw-rw-   0        0        0     6980 2023-03-07 23:51:11.000000 pvmodule-0.0.98/pvmodule/system.py
-drwxrwxrwx   0        0        0        0 2023-03-08 22:23:09.927416 pvmodule-0.0.98/pvmodule.egg-info/
--rw-rw-rw-   0        0        0    24475 2023-03-08 22:23:09.000000 pvmodule-0.0.98/pvmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-03-08 22:23:09.000000 pvmodule-0.0.98/pvmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 22:23:09.000000 pvmodule-0.0.98/pvmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-08 22:23:09.000000 pvmodule-0.0.98/pvmodule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-08 22:23:09.000000 pvmodule-0.0.98/pvmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 22:23:09.930419 pvmodule-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-03-08 22:23:01.000000 pvmodule-0.0.98/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:26:25.017392 pvmodule-0.0.99/
+-rw-rw-rw-   0        0        0    24475 2023-03-08 22:26:25.016392 pvmodule-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0    19701 2023-03-04 22:29:07.000000 pvmodule-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2023-03-08 22:26:24.997392 pvmodule-0.0.99/pvmodule/
+-rw-rw-rw-   0        0        0      276 2023-01-31 14:18:52.000000 pvmodule-0.0.99/pvmodule/__init__.py
+-rw-rw-rw-   0        0        0     3226 2023-03-07 20:27:34.000000 pvmodule-0.0.99/pvmodule/inverter.py
+-rw-rw-rw-   0        0        0    18046 2023-03-08 22:26:11.000000 pvmodule-0.0.99/pvmodule/irradiance.py
+-rw-rw-rw-   0        0        0     5459 2023-03-05 12:55:45.000000 pvmodule-0.0.99/pvmodule/location.py
+-rw-rw-rw-   0        0        0     4007 2023-03-07 20:27:45.000000 pvmodule-0.0.99/pvmodule/module.py
+-rw-rw-rw-   0        0        0    26704 2023-03-02 16:16:53.000000 pvmodule-0.0.99/pvmodule/pvgis.py
+-rw-rw-rw-   0        0        0     3599 2023-03-08 10:36:33.000000 pvmodule-0.0.99/pvmodule/simulation.py
+-rw-rw-rw-   0        0        0     6980 2023-03-07 23:51:11.000000 pvmodule-0.0.99/pvmodule/system.py
+drwxrwxrwx   0        0        0        0 2023-03-08 22:26:25.015392 pvmodule-0.0.99/pvmodule.egg-info/
+-rw-rw-rw-   0        0        0    24475 2023-03-08 22:26:24.000000 pvmodule-0.0.99/pvmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-03-08 22:26:24.000000 pvmodule-0.0.99/pvmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-08 22:26:24.000000 pvmodule-0.0.99/pvmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-03-08 22:26:24.000000 pvmodule-0.0.99/pvmodule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-08 22:26:24.000000 pvmodule-0.0.99/pvmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-08 22:26:25.018392 pvmodule-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     1131 2023-03-08 22:26:15.000000 pvmodule-0.0.99/setup.py
```

### Comparing `pvmodule-0.0.98/PKG-INFO` & `pvmodule-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvmodule
-Version: 0.0.98
+Version: 0.0.99
 Summary: A library used to simulate photovoltaic energy production using PVGIS
 Home-page: UNKNOWN
 Author: Fábio Almeida
 Author-email: <fabio-r-almeida@outlook.com>
 License: UNKNOWN
 Description: # PV-Module
         ---
```

### Comparing `pvmodule-0.0.98/README.md` & `pvmodule-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/inverter.py` & `pvmodule-0.0.99/pvmodule/inverter.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/irradiance.py` & `pvmodule-0.0.99/pvmodule/irradiance.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,18 @@
       inputs, data , metadata = PVGIS().retrieve_daily(
                     location.latitude, 
                     location.longitude, 
                     month= i, 
                     angle = 0, 
                     aspect = azimuth, 
                     glob_2axis = 1)
+
+      df_res=  pd.concat([df_res, data])
       
-      df_res = df_res.concat(data)
+      #df_res = df_res.concat(data)
 
     threads = []
     for i in range(1,13):
       t1 = Thread(target=get_data, args=(i,))
       threads.append(t1)
 
     # Start all threads
```

### Comparing `pvmodule-0.0.98/pvmodule/location.py` & `pvmodule-0.0.99/pvmodule/location.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/module.py` & `pvmodule-0.0.99/pvmodule/module.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/pvgis.py` & `pvmodule-0.0.99/pvmodule/pvgis.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/simulation.py` & `pvmodule-0.0.99/pvmodule/simulation.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule/system.py` & `pvmodule-0.0.99/pvmodule/system.py`

 * *Files identical despite different names*

### Comparing `pvmodule-0.0.98/pvmodule.egg-info/PKG-INFO` & `pvmodule-0.0.99/pvmodule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvmodule
-Version: 0.0.98
+Version: 0.0.99
 Summary: A library used to simulate photovoltaic energy production using PVGIS
 Home-page: UNKNOWN
 Author: Fábio Almeida
 Author-email: <fabio-r-almeida@outlook.com>
 License: UNKNOWN
 Description: # PV-Module
         ---
```

### Comparing `pvmodule-0.0.98/setup.py` & `pvmodule-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 try:
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
-VERSION = '0.0.98'
+VERSION = '0.0.99'
 DESCRIPTION = 'A library used to simulate photovoltaic energy production using PVGIS'
 # Setting up
 setup(
     name="pvmodule",
     version=VERSION,
     author="Fábio Almeida",
     author_email="<fabio-r-almeida@outlook.com>",
```

