# Comparing `tmp/sentinel_satellites-0.0.8.tar.gz` & `tmp/sentinel_satellites-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinel_satellites-0.0.8.tar", last modified: Sat Apr  1 07:37:13 2023, max compression
+gzip compressed data, was "sentinel_satellites-0.0.9.tar", last modified: Sat Apr  1 07:47:14 2023, max compression
```

## Comparing `sentinel_satellites-0.0.8.tar` & `sentinel_satellites-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 francesco  (1001) francesco  (1001)        0 2023-04-01 07:37:13.556608 sentinel_satellites-0.0.8/
--rwxr-xr-x   0 francesco  (1001) francesco  (1001)     1072 2023-03-22 14:27:12.000000 sentinel_satellites-0.0.8/LICENSE
--rw-rw-r--   0 francesco  (1001) francesco  (1001)     8190 2023-04-01 07:37:13.556608 sentinel_satellites-0.0.8/PKG-INFO
--rwxrwxr-x   0 francesco  (1001) francesco  (1001)     7512 2023-04-01 07:26:36.000000 sentinel_satellites-0.0.8/README.md
--rwxrwxr-x   0 francesco  (1001) francesco  (1001)    20363 2023-03-31 21:07:54.000000 sentinel_satellites-0.0.8/optical_features.py
--rwxr-xr-x   0 francesco  (1001) francesco  (1001)       89 2023-03-23 13:53:23.000000 sentinel_satellites-0.0.8/pyproject.toml
--rwxrwxr-x   0 francesco  (1001) francesco  (1001)     7982 2023-03-31 21:44:44.000000 sentinel_satellites-0.0.8/radar_features.py
-drwxrwxr-x   0 francesco  (1001) francesco  (1001)        0 2023-04-01 07:37:13.556608 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/
--rw-rw-r--   0 francesco  (1001) francesco  (1001)     8190 2023-04-01 07:37:13.000000 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1001) francesco  (1001)      317 2023-04-01 07:37:13.000000 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1001) francesco  (1001)        1 2023-04-01 07:37:13.000000 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1001) francesco  (1001)       23 2023-04-01 07:37:13.000000 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1001) francesco  (1001)       52 2023-04-01 07:37:13.000000 sentinel_satellites-0.0.8/sentinel_satellites.egg-info/top_level.txt
--rwxr-xr-x   0 francesco  (1001) francesco  (1001)    18008 2023-04-01 07:17:18.000000 sentinel_satellites-0.0.8/sentinel_satellites.py
--rwxr-xr-x   0 francesco  (1001) francesco  (1001)      813 2023-04-01 07:37:13.556608 sentinel_satellites-0.0.8/setup.cfg
+drwxrwxr-x   0 francesco  (1001) francesco  (1001)        0 2023-04-01 07:47:14.053078 sentinel_satellites-0.0.9/
+-rwxr-xr-x   0 francesco  (1001) francesco  (1001)     1072 2023-03-22 14:27:12.000000 sentinel_satellites-0.0.9/LICENSE
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)     8195 2023-04-01 07:47:14.053078 sentinel_satellites-0.0.9/PKG-INFO
+-rwxrwxr-x   0 francesco  (1001) francesco  (1001)     7517 2023-04-01 07:45:55.000000 sentinel_satellites-0.0.9/README.md
+-rwxrwxr-x   0 francesco  (1001) francesco  (1001)    20363 2023-03-31 21:07:54.000000 sentinel_satellites-0.0.9/optical_features.py
+-rwxr-xr-x   0 francesco  (1001) francesco  (1001)       89 2023-03-23 13:53:23.000000 sentinel_satellites-0.0.9/pyproject.toml
+-rwxrwxr-x   0 francesco  (1001) francesco  (1001)     7982 2023-03-31 21:44:44.000000 sentinel_satellites-0.0.9/radar_features.py
+drwxrwxr-x   0 francesco  (1001) francesco  (1001)        0 2023-04-01 07:47:14.053078 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)     8195 2023-04-01 07:47:14.000000 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)      317 2023-04-01 07:47:14.000000 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)        1 2023-04-01 07:47:14.000000 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)       23 2023-04-01 07:47:14.000000 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1001) francesco  (1001)       52 2023-04-01 07:47:14.000000 sentinel_satellites-0.0.9/sentinel_satellites.egg-info/top_level.txt
+-rwxr-xr-x   0 francesco  (1001) francesco  (1001)    18008 2023-04-01 07:17:18.000000 sentinel_satellites-0.0.9/sentinel_satellites.py
+-rwxr-xr-x   0 francesco  (1001) francesco  (1001)      813 2023-04-01 07:47:14.053078 sentinel_satellites-0.0.9/setup.cfg
```

### Comparing `sentinel_satellites-0.0.8/LICENSE` & `sentinel_satellites-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sentinel_satellites-0.0.8/PKG-INFO` & `sentinel_satellites-0.0.9/sentinel_satellites.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentinel_satellites
-Version: 0.0.8
+Name: sentinel-satellites
+Version: 0.0.9
 Summary: A Python library that allows to extract data from sentinel satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 Home-page: https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/utils
 Author: Francesco Amato
 Author-email: amatofrancesco99@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,17 +16,19 @@
 
 # sentinel-satellites 🌍
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](./LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 
-This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**. These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**.<br>
 In addition to the already mentioned advantages, the implemented code also **exploits machine parallelism** (designed to work efficiently with large volumes of data, allowing for faster processing times and improved performances) and **relies on Google Earth Engine (GEE) APIs** (used to access satellites data and perform some tasks such as *cloud masking*, *image compositing*, and *time series selection*).
 
+These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+
 **How to install it?**
 ```bash
 $ pip install sentinel-satellites
 ```
 
 This library is composed of lot of functions, the main ones are here described.
 
@@ -101,12 +103,12 @@
     * Added new radar features
     * Reduced the `CLOUDY_PIXEL_PERCENTAGE` parameter to `25` (for optical features extraction)
     * The output DataFrame is now ordered by the first two columns (`field_name` & `acquisition_date`), in ascending order 
 
 * `version: 0.0.7`:
     * Fixed `EOMI3` formula
 
-* `version: 0.0.8` (current):
+* `version: 0.0.9` (current):
     * Improved parallelization in `get_features()` function by calculating all the radar and optical features using mean bands/polarizations values (this allowed to drastically reduce the number of queries to Google Earth Engine via APIs)
     *E.G:* `NDVI mean = (NIR mean - RED mean) / (NIR mean + RED mean)`
     * Adjusted descriptions and fixed all `optical_features` and `radar_features` functions, such that now are working directly on mean bands values (relative to a crop field of interest in a single date)
     * Added EE filters and allowed users to specify the list of parameters values to be used for filters to extract Sentinel Images Collections
```

### Comparing `sentinel_satellites-0.0.8/README.md` & `sentinel_satellites-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # sentinel-satellites 🌍
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](./LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 
-This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**. These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**.<br>
 In addition to the already mentioned advantages, the implemented code also **exploits machine parallelism** (designed to work efficiently with large volumes of data, allowing for faster processing times and improved performances) and **relies on Google Earth Engine (GEE) APIs** (used to access satellites data and perform some tasks such as *cloud masking*, *image compositing*, and *time series selection*).
 
+These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+
 **How to install it?**
 ```bash
 $ pip install sentinel-satellites
 ```
 
 This library is composed of lot of functions, the main ones are here described.
 
@@ -85,12 +87,12 @@
     * Added new radar features
     * Reduced the `CLOUDY_PIXEL_PERCENTAGE` parameter to `25` (for optical features extraction)
     * The output DataFrame is now ordered by the first two columns (`field_name` & `acquisition_date`), in ascending order 
 
 * `version: 0.0.7`:
     * Fixed `EOMI3` formula
 
-* `version: 0.0.8` (current):
+* `version: 0.0.9` (current):
     * Improved parallelization in `get_features()` function by calculating all the radar and optical features using mean bands/polarizations values (this allowed to drastically reduce the number of queries to Google Earth Engine via APIs)
     *E.G:* `NDVI mean = (NIR mean - RED mean) / (NIR mean + RED mean)`
     * Adjusted descriptions and fixed all `optical_features` and `radar_features` functions, such that now are working directly on mean bands values (relative to a crop field of interest in a single date)
     * Added EE filters and allowed users to specify the list of parameters values to be used for filters to extract Sentinel Images Collections
```

### Comparing `sentinel_satellites-0.0.8/optical_features.py` & `sentinel_satellites-0.0.9/optical_features.py`

 * *Files identical despite different names*

### Comparing `sentinel_satellites-0.0.8/radar_features.py` & `sentinel_satellites-0.0.9/radar_features.py`

 * *Files identical despite different names*

### Comparing `sentinel_satellites-0.0.8/sentinel_satellites.egg-info/PKG-INFO` & `sentinel_satellites-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentinel-satellites
-Version: 0.0.8
+Name: sentinel_satellites
+Version: 0.0.9
 Summary: A Python library that allows to extract data from sentinel satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 Home-page: https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/utils
 Author: Francesco Amato
 Author-email: amatofrancesco99@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,17 +16,19 @@
 
 # sentinel-satellites 🌍
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](./LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 
-This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**. These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+This library provides an **easy-to-use**, **comprehensive**, and **flexible** way to work with satellite data from the Sentinel-1 and Sentinel-2 satellites. Its key advantages include: a **well-documented** API, **support** for the mainly used satellites, **open-source code**, and **regular updates**.<br>
 In addition to the already mentioned advantages, the implemented code also **exploits machine parallelism** (designed to work efficiently with large volumes of data, allowing for faster processing times and improved performances) and **relies on Google Earth Engine (GEE) APIs** (used to access satellites data and perform some tasks such as *cloud masking*, *image compositing*, and *time series selection*).
 
+These advantages make it an excellent tool for anyone working with satellite data, since it allows to *generate datasets that can be both easily used for data analysis and efficiently integrated with well-known ML libraries, to deploy models*.
+
 **How to install it?**
 ```bash
 $ pip install sentinel-satellites
 ```
 
 This library is composed of lot of functions, the main ones are here described.
 
@@ -101,12 +103,12 @@
     * Added new radar features
     * Reduced the `CLOUDY_PIXEL_PERCENTAGE` parameter to `25` (for optical features extraction)
     * The output DataFrame is now ordered by the first two columns (`field_name` & `acquisition_date`), in ascending order 
 
 * `version: 0.0.7`:
     * Fixed `EOMI3` formula
 
-* `version: 0.0.8` (current):
+* `version: 0.0.9` (current):
     * Improved parallelization in `get_features()` function by calculating all the radar and optical features using mean bands/polarizations values (this allowed to drastically reduce the number of queries to Google Earth Engine via APIs)
     *E.G:* `NDVI mean = (NIR mean - RED mean) / (NIR mean + RED mean)`
     * Adjusted descriptions and fixed all `optical_features` and `radar_features` functions, such that now are working directly on mean bands values (relative to a crop field of interest in a single date)
     * Added EE filters and allowed users to specify the list of parameters values to be used for filters to extract Sentinel Images Collections
```

### Comparing `sentinel_satellites-0.0.8/sentinel_satellites.py` & `sentinel_satellites-0.0.9/sentinel_satellites.py`

 * *Files identical despite different names*

### Comparing `sentinel_satellites-0.0.8/setup.cfg` & `sentinel_satellites-0.0.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sentinel_satellites
-version = 0.0.8
+version = 0.0.9
 author = Francesco Amato
 author_email = amatofrancesco99@gmail.com
 description = A Python library that allows to extract data from sentinel satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = mit
 url = https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/utils
```

