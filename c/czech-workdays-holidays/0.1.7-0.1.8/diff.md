# Comparing `tmp/czech_workdays_holidays-0.1.7.tar.gz` & `tmp/czech_workdays_holidays-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.1.7.tar", last modified: Sun Apr 23 10:22:11 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.8.tar", last modified: Sun Apr 23 10:28:41 2023, max compression
```

## Comparing `czech_workdays_holidays-0.1.7.tar` & `czech_workdays_holidays-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/
--rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     4808 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4140 2023-04-22 15:16:10.000000 czech_workdays_holidays-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.107367 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     4808 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14646 2023-04-23 10:21:16.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      756 2023-04-23 10:18:18.000000 czech_workdays_holidays-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.109368 czech_workdays_holidays-0.1.7/test/
--rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.7/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:28:41.777186 czech_workdays_holidays-0.1.8/
+-rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     5210 2023-04-23 10:28:41.777186 czech_workdays_holidays-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4537 2023-04-23 10:28:04.000000 czech_workdays_holidays-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:28:41.777186 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     5210 2023-04-23 10:28:41.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-23 10:28:41.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:28:41.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-23 10:28:41.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 10:28:41.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14646 2023-04-23 10:21:16.000000 czech_workdays_holidays-0.1.8/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      756 2023-04-23 10:28:31.000000 czech_workdays_holidays-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:28:41.777186 czech_workdays_holidays-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 10:28:41.777186 czech_workdays_holidays-0.1.8/test/
+-rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.8/test/tests.py
```

### Comparing `czech_workdays_holidays-0.1.7/LICENSE` & `czech_workdays_holidays-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.7/PKG-INFO` & `czech_workdays_holidays-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.1.7
+Version: 0.1.8
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,14 +60,19 @@
 [datetime.date(2023, 5, 1), datetime.date(2023, 4, 7), datetime.date(2023, 10, 28), datetime.date(2023, 12, 25), datetime.date(2023, 12, 26), datetime.date(2023, 4, 10), datetime.date(2023, 7, 5), datetime.date(2023, 11, 17), datetime.date(2023, 12, 24), datetime.date(2023, 5, 8), datetime.date(2023, 7, 6), datetime.date(2023, 9, 28), datetime.date(2023, 1, 1)]
 ```
 
 ### get_workdays()
 
 This function calculates the number of workdays in a given year, taking into account optional parameters for including or excluding weekend days and holidays
 
+By default, function return workdays in a given year. If parameters are set to False, it will return Monday to Friday days.
+
+In case you set `include_saturday=True`, it will return Monday to Saturday days but Saturdays that are also holidays would be excluded.
+In case you set `include_holidays=True`, including weekend days would remain False then holidays during weekend would not be returned.
+
 Raises exception if year entered is 2000 and earlier
 
 #### Example
 
 Calling function `get_workdays()` with argument `include_holidays=True` and with argument `include_sunday` will return sorted list of `datetime.date(YYYY/MM//DD)` workdays
 
 Notice that 2023/1/1 was a Sunday and Holiday and it is in the output. If one of those arguments were False, it would not appear
```

### Comparing `czech_workdays_holidays-0.1.7/README.md` & `czech_workdays_holidays-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 [datetime.date(2023, 5, 1), datetime.date(2023, 4, 7), datetime.date(2023, 10, 28), datetime.date(2023, 12, 25), datetime.date(2023, 12, 26), datetime.date(2023, 4, 10), datetime.date(2023, 7, 5), datetime.date(2023, 11, 17), datetime.date(2023, 12, 24), datetime.date(2023, 5, 8), datetime.date(2023, 7, 6), datetime.date(2023, 9, 28), datetime.date(2023, 1, 1)]
 ```
 
 ### get_workdays()
 
 This function calculates the number of workdays in a given year, taking into account optional parameters for including or excluding weekend days and holidays
 
+By default, function return workdays in a given year. If parameters are set to False, it will return Monday to Friday days.
+
+In case you set `include_saturday=True`, it will return Monday to Saturday days but Saturdays that are also holidays would be excluded.
+In case you set `include_holidays=True`, including weekend days would remain False then holidays during weekend would not be returned.
+
 Raises exception if year entered is 2000 and earlier
 
 #### Example
 
 Calling function `get_workdays()` with argument `include_holidays=True` and with argument `include_sunday` will return sorted list of `datetime.date(YYYY/MM//DD)` workdays
 
 Notice that 2023/1/1 was a Sunday and Holiday and it is in the output. If one of those arguments were False, it would not appear
```

### Comparing `czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.1.8/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.1.7
+Version: 0.1.8
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,14 +60,19 @@
 [datetime.date(2023, 5, 1), datetime.date(2023, 4, 7), datetime.date(2023, 10, 28), datetime.date(2023, 12, 25), datetime.date(2023, 12, 26), datetime.date(2023, 4, 10), datetime.date(2023, 7, 5), datetime.date(2023, 11, 17), datetime.date(2023, 12, 24), datetime.date(2023, 5, 8), datetime.date(2023, 7, 6), datetime.date(2023, 9, 28), datetime.date(2023, 1, 1)]
 ```
 
 ### get_workdays()
 
 This function calculates the number of workdays in a given year, taking into account optional parameters for including or excluding weekend days and holidays
 
+By default, function return workdays in a given year. If parameters are set to False, it will return Monday to Friday days.
+
+In case you set `include_saturday=True`, it will return Monday to Saturday days but Saturdays that are also holidays would be excluded.
+In case you set `include_holidays=True`, including weekend days would remain False then holidays during weekend would not be returned.
+
 Raises exception if year entered is 2000 and earlier
 
 #### Example
 
 Calling function `get_workdays()` with argument `include_holidays=True` and with argument `include_sunday` will return sorted list of `datetime.date(YYYY/MM//DD)` workdays
 
 Notice that 2023/1/1 was a Sunday and Holiday and it is in the output. If one of those arguments were False, it would not appear
```

### Comparing `czech_workdays_holidays-0.1.7/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.8/czech_workdays_holidays.py`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.7/pyproject.toml` & `czech_workdays_holidays-0.1.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 42.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays, Holidays and Shopping Days"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `czech_workdays_holidays-0.1.7/test/tests.py` & `czech_workdays_holidays-0.1.8/test/tests.py`

 * *Files identical despite different names*

