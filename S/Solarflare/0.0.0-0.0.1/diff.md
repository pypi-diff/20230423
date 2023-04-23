# Comparing `tmp/Solarflare-0.0.0.tar.gz` & `tmp/Solarflare-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Solarflare-0.0.0.tar", last modified: Sat Apr 22 22:07:55 2023, max compression
+gzip compressed data, was "Solarflare-0.0.1.tar", last modified: Sun Apr 23 01:47:29 2023, max compression
```

## Comparing `Solarflare-0.0.0.tar` & `Solarflare-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:55.948892 Solarflare-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-22 22:07:55.948892 Solarflare-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-22 22:07:45.000000 Solarflare-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:55.948892 Solarflare-0.0.0/Solarflare/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-22 22:07:45.000000 Solarflare-0.0.0/Solarflare/solarflare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:07:55.948892 Solarflare-0.0.0/Solarflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-22 22:07:55.000000 Solarflare-0.0.0/Solarflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 22:07:55.000000 Solarflare-0.0.0/Solarflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:07:55.000000 Solarflare-0.0.0/Solarflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 22:07:55.000000 Solarflare-0.0.0/Solarflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:07:55.948892 Solarflare-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-22 22:07:45.000000 Solarflare-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:29.225452 Solarflare-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 01:47:29.221452 Solarflare-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 01:47:18.000000 Solarflare-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:29.221452 Solarflare-0.0.1/Solarflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 01:47:18.000000 Solarflare-0.0.1/Solarflare/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 01:47:18.000000 Solarflare-0.0.1/Solarflare/nightcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-23 01:47:18.000000 Solarflare-0.0.1/Solarflare/solarflare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:29.221452 Solarflare-0.0.1/Solarflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 01:47:29.000000 Solarflare-0.0.1/Solarflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 01:47:29.000000 Solarflare-0.0.1/Solarflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 01:47:29.000000 Solarflare-0.0.1/Solarflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 01:47:29.000000 Solarflare-0.0.1/Solarflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 01:47:29.225452 Solarflare-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 01:47:18.000000 Solarflare-0.0.1/setup.py
```

### Comparing `Solarflare-0.0.0/Solarflare/solarflare.py` & `Solarflare-0.0.1/Solarflare/solarflare.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 def sin(x): return math.sin(math.radians(x))
 def cos(x): return math.cos(math.radians(x))
 def tan(x): return math.tan(math.radians(x))
 def acos(x): return math.degrees(math.acos(x))
 def asin(x): return math.degrees(math.asin(x))
 def atan2(y, x): return math.degrees(math.atan2(y, x))
 
+# Version function
+def VERSION():
+    return "0.0.1"
 
 # 1. TIME
 # for these calculations, it is convenient to use Julian dates.
 def julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() else 0
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5
@@ -118,7 +121,8 @@
     def right_ascension(self, date = datetime.datetime.now()): return right_ascension(date)
     def declination(self, date=datetime.datetime.now()): return declination(date)
     def ecliptical_longitude(self, date=datetime.datetime.now()): return ecliptical_longitude(date)
     def nadir(self, date=datetime.datetime.now()): return fromJulian(solar_transit(self.long, date) - 0.5)
     def hour_angle(self, date=datetime.datetime.now()): return hour_angle(self.long, date)
     def observer_angle(self): return -2.076 * math.sqrt(self.ht) / 60
 
+
```

### Comparing `Solarflare-0.0.0/setup.py` & `Solarflare-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='Solarflare',
-    version='0.0.0',
+    version='0.0.1',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with solar calculations',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/Solarflare',
     project_urls = {
```

