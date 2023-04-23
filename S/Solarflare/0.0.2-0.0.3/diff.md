# Comparing `tmp/Solarflare-0.0.2.tar.gz` & `tmp/Solarflare-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Solarflare-0.0.2.tar", last modified: Sun Apr 23 16:40:45 2023, max compression
+gzip compressed data, was "Solarflare-0.0.3.tar", last modified: Sun Apr 23 17:06:45 2023, max compression
```

## Comparing `Solarflare-0.0.2.tar` & `Solarflare-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:40:45.275122 Solarflare-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 16:40:45.275122 Solarflare-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 16:40:31.000000 Solarflare-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:40:45.275122 Solarflare-0.0.2/Solarflare/
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 16:40:31.000000 Solarflare-0.0.2/Solarflare/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 16:40:31.000000 Solarflare-0.0.2/Solarflare/nightcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-23 16:40:31.000000 Solarflare-0.0.2/Solarflare/solarflare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:40:45.275122 Solarflare-0.0.2/Solarflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 16:40:45.000000 Solarflare-0.0.2/Solarflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 16:40:45.000000 Solarflare-0.0.2/Solarflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:40:45.000000 Solarflare-0.0.2/Solarflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 16:40:45.000000 Solarflare-0.0.2/Solarflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:40:45.275122 Solarflare-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 16:40:31.000000 Solarflare-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:06:45.116190 Solarflare-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 17:06:33.000000 Solarflare-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/Solarflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/nightcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/solarflare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/Solarflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:06:45.116190 Solarflare-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 17:06:33.000000 Solarflare-0.0.3/setup.py
```

### Comparing `Solarflare-0.0.2/Solarflare/conversions.py` & `Solarflare-0.0.3/Solarflare/conversions.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.2/Solarflare/nightcalc.py` & `Solarflare-0.0.3/Solarflare/nightcalc.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.2/Solarflare/solarflare.py` & `Solarflare-0.0.3/Solarflare/solarflare.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def tan(x): return math.tan(math.radians(x))
 def acos(x): return math.degrees(math.acos(x))
 def asin(x): return math.degrees(math.asin(x))
 def atan2(y, x): return math.degrees(math.atan2(y, x))
 
 # Version function
 def VERSION():
-    return "0.0.2"
+    return "0.0.3"
 
 # 1. TIME
 # for these calculations, it is convenient to use Julian dates.
 def julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() else 0
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5
@@ -117,14 +117,47 @@
 
 def altitude(latitude, longitude, date=datetime.datetime.now()):
     H = hour_angle(longitude, date)
     delta = declination(date)
     sinh = sin(delta) * sin(latitude) + cos(delta) * cos(latitude) * cos(H)
     return asin(sinh)
 
+# Seasons based on sun Longitude
+def spring():
+    date = datetime.datetime(datetime.datetime.now().year, 1, 1)
+    for i in range(365):
+        if round(ecliptical_longitude(date)) == 0:
+            return date - datetime.timedelta(days=1)
+        else:
+            date += datetime.timedelta(days = 1)
+
+def summer():
+    date = datetime.datetime(datetime.datetime.now().year, 1, 1)
+    for i in range(365):
+        if round(ecliptical_longitude(date)) == 90:
+            return date
+        else:
+            date += datetime.timedelta(days=1)
+
+def autumn():
+    date = datetime.datetime(datetime.datetime.now().year, 1, 1)
+    for i in range(365):
+        if round(ecliptical_longitude(date)) == 180:
+            return date - datetime.timedelta(days=1)
+        else:
+            date += datetime.timedelta(days=1)
+
+def winter():
+    date = datetime.datetime(datetime.datetime.now().year, 1, 1)
+    for i in range(365):
+        if round(ecliptical_longitude(date)) == 270:
+            return date
+        else:
+            date += datetime.timedelta(days=1)
+
 
 #12. Combine all previous methods into a convenient class
 class Daystar:
     def __init__(self, latitude, longitude, height=0):
         self.lat = latitude
         self.long = longitude
         self.ht = height
```

### Comparing `Solarflare-0.0.2/setup.py` & `Solarflare-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='Solarflare',
-    version='0.0.2',
+    version='0.0.3',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with solar calculations',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/Solarflare',
     project_urls = {
```

