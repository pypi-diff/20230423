# Comparing `tmp/czech_workdays_holidays-0.1.6.tar.gz` & `tmp/czech_workdays_holidays-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.1.6.tar", last modified: Sat Apr 22 15:27:50 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.7.tar", last modified: Sun Apr 23 10:22:11 2023, max compression
```

## Comparing `czech_workdays_holidays-0.1.6.tar` & `czech_workdays_holidays-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/
--rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4808 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4140 2023-04-22 15:16:10.000000 czech_workdays_holidays-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.246507 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     4808 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13730 2023-04-22 15:27:26.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      756 2023-04-22 15:27:44.000000 czech_workdays_holidays-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.247508 czech_workdays_holidays-0.1.6/test/
--rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.6/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/
+-rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4808 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4140 2023-04-22 15:16:10.000000 czech_workdays_holidays-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.107367 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     4808 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 10:22:11.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14646 2023-04-23 10:21:16.000000 czech_workdays_holidays-0.1.7/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      756 2023-04-23 10:18:18.000000 czech_workdays_holidays-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:22:11.110368 czech_workdays_holidays-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:11.109368 czech_workdays_holidays-0.1.7/test/
+-rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.7/test/tests.py
```

### Comparing `czech_workdays_holidays-0.1.6/LICENSE` & `czech_workdays_holidays-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.6/PKG-INFO` & `czech_workdays_holidays-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.1.6
+Version: 0.1.7
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.6/README.md` & `czech_workdays_holidays-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.1.7/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.1.6
+Version: 0.1.7
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.6/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.7/czech_workdays_holidays.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 def get_holidays(year: int,
                  dates_only: bool = False,
                  dates_and_cz_names: bool = False,
                  dates_and_en_names: bool = False,
                  shopping_restricted: bool = False) -> list:
-
     """
     This function generates holidays (public and other) when working is usually restricted according to labor Law.
     Also offers possibilities to filter dates only, czech or english names or shopping restricted days.
 
     :param year: Desired year to generate holidays (int)
     :param dates_only: Returns only dates -> [datetime.date(2023, 1, 1), ...]
     :param dates_and_cz_names: Returns only dates and cz names
@@ -252,15 +251,14 @@
     return holidays
 
 
 def get_workdays(year: int,
                  include_saturday: bool = False,
                  include_sunday: bool = False,
                  include_holidays: bool = False) -> list:
-
     """
 
     :param year: Desired year to generate holidays (int)
     :param include_saturday: Includes also Saturdays in output
     :param include_sunday: Includes also Sundays in output
     :param include_holidays: Counts holidays as working days
     :return: List of all working days -> [datetime.date(2023, 1, 2), ...]
@@ -305,15 +303,14 @@
     return working_days
 
 
 def get_shopping_days(year: int,
                       include_saturday: bool = True,
                       include_sunday: bool = True,
                       exclude_shopping_restricted_days: bool = True) -> list:
-
     """
     Gets all shopping days in a given year. Full year returned if all parameters are True. Possibility to combine
     parameters
 
     :param year: Desired year to generate holidays (int)
     :param include_saturday: Includes also Saturdays in output
     :param include_sunday: Includes also Sundays in output
@@ -357,16 +354,39 @@
             all_shopping_days.append(start_date)
         start_date += timedelta(days=1)
 
     return all_shopping_days
 
 
 def get_holidays_during_weekend(year: int) -> list:
-
     # Verification for year data type
     if not isinstance(year, int):
         raise TypeError("Year must be an integer.")
 
     holiday_dates = list(holiday["date"] for holiday in get_holidays(year)
-                        if holiday["date"].strftime("%A") in ("Saturday", "Sunday"))
+                         if holiday["date"].strftime("%A") in ("Saturday", "Sunday"))
 
     return holiday_dates
+
+
+def get_workdays_during_weekend(year: int, include_holidays: bool = False) -> list:
+
+    """
+    Gets all workdays that are during weekend (Saturday or Sunday) with possibility to include holidays
+    :param year: Desired year to generate holidays (int)
+    :param include_holidays: Considers holidays as working days if True
+    :return: List of all workdays during weekend in a given year
+    """
+
+    # Verification for year data type
+    if not isinstance(year, int):
+        raise TypeError("Year must be an integer.")
+
+    workdays = get_workdays(year, include_saturday=True, include_sunday=True, include_holidays=include_holidays)
+
+    holidays_during_weekend = list(workday for workday in workdays
+                                   if workday.strftime("%A") in ("Saturday", "Sunday"))
+
+    return holidays_during_weekend
+
+
+print(get_workdays_during_weekend(2023, include_holidays=False))
```

### Comparing `czech_workdays_holidays-0.1.6/pyproject.toml` & `czech_workdays_holidays-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 42.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays, Holidays and Shopping Days"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `czech_workdays_holidays-0.1.6/test/tests.py` & `czech_workdays_holidays-0.1.7/test/tests.py`

 * *Files identical despite different names*

