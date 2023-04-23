# Comparing `tmp/Solarflare-0.0.3.tar.gz` & `tmp/Solarflare-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Solarflare-0.0.3.tar", last modified: Sun Apr 23 17:06:45 2023, max compression
+gzip compressed data, was "Solarflare-0.0.4.tar", last modified: Sun Apr 23 17:37:18 2023, max compression
```

## Comparing `Solarflare-0.0.3.tar` & `Solarflare-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:06:45.116190 Solarflare-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 17:06:33.000000 Solarflare-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/Solarflare/
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/nightcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-23 17:06:33.000000 Solarflare-0.0.3/Solarflare/solarflare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:06:45.116190 Solarflare-0.0.3/Solarflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 17:06:45.000000 Solarflare-0.0.3/Solarflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:06:45.116190 Solarflare-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 17:06:33.000000 Solarflare-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.112101 Solarflare-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:37:18.112101 Solarflare-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 17:37:04.000000 Solarflare-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.108101 Solarflare-0.0.4/Solarflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/nightcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/solarflare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.112101 Solarflare-0.0.4/Solarflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:37:18.112101 Solarflare-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 17:37:04.000000 Solarflare-0.0.4/setup.py
```

### Comparing `Solarflare-0.0.3/Solarflare/conversions.py` & `Solarflare-0.0.4/Solarflare/conversions.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.3/Solarflare/nightcalc.py` & `Solarflare-0.0.4/Solarflare/nightcalc.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.3/Solarflare/solarflare.py` & `Solarflare-0.0.4/Solarflare/solarflare.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def tan(x): return math.tan(math.radians(x))
 def acos(x): return math.degrees(math.acos(x))
 def asin(x): return math.degrees(math.asin(x))
 def atan2(y, x): return math.degrees(math.atan2(y, x))
 
 # Version function
 def VERSION():
-    return "0.0.3"
+    return "0.0.4"
 
 # 1. TIME
 # for these calculations, it is convenient to use Julian dates.
 def julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() else 0
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5
@@ -86,27 +86,36 @@
     n = round(nx)
     jx = J + J3 * (n - nx)
     Jtransit = jx + J1 * sin(mean_anomaly(date)) + J2 * sin(2 * ecliptical_longitude(date))
     return Jtransit
 
 # 10. Sunset and Sunrise Julian
 def suntimes(latitude, longitude, date=datetime.datetime.now()):
-    ht = acos((sin(-0.83) - sin(latitude) * sin(declination(date))) / cos(latitude) * cos(declination(date)))
-    Jtransit = solar_transit(longitude, date)
-    Jrise = Jtransit - ht/360
-    Jset = Jtransit + ht / 360
-    return (Jrise, Jset)
+    try:
+        ht = acos((sin(-0.83) - sin(latitude) * sin(declination(date))) / cos(latitude) * cos(declination(date)))
+        Jtransit = solar_transit(longitude, date)
+        Jrise = Jtransit - ht/360
+        Jset = Jtransit + ht / 360
+        return (Jrise, Jset)
+    except:
+        return (None, None)
 
 def sunrise(latitude, longitude, date=datetime.datetime.now()):
-    sunrise = suntimes(latitude, longitude, date)[0]
-    return fromJulian(sunrise)
+    try:
+        sunrise = suntimes(latitude, longitude, date)[0]
+        return fromJulian(sunrise)
+    except:
+        return f"Sun does not rise at specified location: ({latitude}, {longitude})"
 
 def sunset(latitude, longitude, date=datetime.datetime.now()):
-    sunset = suntimes(latitude, longitude, date)[1]
-    return fromJulian(sunset)
+    try:
+        sunset = suntimes(latitude, longitude, date)[1]
+        return fromJulian(sunset)
+    except:
+        return f"Sun does not set at specified location: ({latitude}, {longitude})"
 
 # 11. Hour Angle & Horizontal Coordinates
 def hour_angle(longitude, date=datetime.datetime.now()):
     return sidereal_time(longitude, date) - right_ascension(date)
 
 # Horizontal Coordinates
 def azimuth(latitude, longitude, date=datetime.datetime.now()):
```

### Comparing `Solarflare-0.0.3/setup.py` & `Solarflare-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='Solarflare',
-    version='0.0.3',
+    version='0.0.4',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with solar calculations',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/Solarflare',
     project_urls = {
```

