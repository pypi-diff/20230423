# Comparing `tmp/tzconv-1.2.tar.gz` & `tmp/tzconv-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzconv-1.2.tar", last modified: Fri Apr 21 19:25:01 2023, max compression
+gzip compressed data, was "tzconv-1.3.tar", last modified: Sun Apr 23 18:54:27 2023, max compression
```

## Comparing `tzconv-1.2.tar` & `tzconv-1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 19:25:01.620027 tzconv-1.2/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3972 2023-04-21 19:25:01.620027 tzconv-1.2/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3733 2023-04-21 19:20:51.000000 tzconv-1.2/README.md
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-21 19:25:01.620027 tzconv-1.2/setup.cfg
--rw-r--r--   0 bigmac    (1000) bigmac    (1000)      608 2023-04-21 19:23:51.000000 tzconv-1.2/setup.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 19:25:01.620027 tzconv-1.2/tzconv/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     5926 2023-04-21 18:50:30.000000 tzconv-1.2/tzconv/__init__.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 19:25:01.620027 tzconv-1.2/tzconv.egg-info/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3972 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      219 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/entry_points.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/requires.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-21 19:25:01.000000 tzconv-1.2/tzconv.egg-info/top_level.txt
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3935 2023-04-23 18:54:27.907143 tzconv-1.3/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3696 2023-04-23 18:44:19.000000 tzconv-1.3/README.md
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-23 18:54:27.907143 tzconv-1.3/setup.cfg
+-rw-r--r--   0 bigmac    (1000) bigmac    (1000)      608 2023-04-23 18:47:13.000000 tzconv-1.3/setup.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/tzconv/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     9457 2023-04-23 18:49:57.000000 tzconv-1.3/tzconv/__init__.py
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2716 2023-04-23 18:16:07.000000 tzconv-1.3/tzconv/test_tzconv.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/tzconv.egg-info/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3935 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      241 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/entry_points.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/requires.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/top_level.txt
```

### Comparing `tzconv-1.2/PKG-INFO` & `tzconv-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: tzconv
-Version: 1.2
-Summary: command-line tool to convert a date and time to several time zones at once
-Home-page: https://codeberg.org/gnyeki/tzconv
-Author: Gabor Nyeki
-Description-Content-Type: text/markdown
-
 
 # `tzconv`: convert a date and time to several time zones at once
 
 This Python package provides a small command-line utility to convert a `YYYY-MM-DD HH:MM` formatted date and time to several other time zones.
 
 ## Installation
 
@@ -31,85 +23,86 @@
 ### Basic usage
 
 `tzconv` uses the time zone information available through your operating system, so time zones have to be specified accordingly:
 
 ```
 $ tzconv \
     -f America/New_York \
-    -t America/Lima \
-    -t Asia/Seoul \
+    -t Pacific/Galapagos \
+    -t America/Santa_Isabel \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
-Time zone names can be shortened as long as they remain unique:
+Time zone names can be shortened as long as they remain unique.
+Initials, prefixes, and abbreviations are all recognized:
 
 ```
 $ tzconv \
-    -f america/ne \
-    -t america/li \
-    -t asia/se \
+    -f ny \
+    -t gal \
+    -t san_i \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
 Available time zones can be listed with the `--list-tz` option (or `-l` for short):
 
 ```
-$ tzconv -l america/n
-The following time zones are available that begin with 'america/n':
+$ tzconv -l am/n
+The following time zones are available that match 'am/n':
 
   America/Nassau, America/New_York, America/Nipigon, America/Nome,
   America/Noronha, America/North_Dakota/Beulah, America/North_Dakota/Center,
   America/North_Dakota/New_Salem, America/Nuuk
 $
 ```
 
 ### Imputing the current date and the current time
 
 If the date is omitted, today's date is imputed:
 
 ```
-$ tzconv -f america/ne -t africa/ad 10:00
+$ tzconv -f ny -t aa 10:00
 EDT: 2023-04-20 10:00 (America/New_York)
 EAT: 2023-04-20 17:00 (Africa/Addis_Ababa)
 $
 
 ```
 
 If the time is omitted, too, then `tzconv` imputes the current time:
 
 ```
-$ tzconv -f america/ne -t africa/ad
+$ tzconv -f ny -t aa
 EDT: 2023-04-20 15:03 (America/New_York)
 EAT: 2023-04-20 22:03 (Africa/Addis_Ababa)
 $
 ```
 
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
 
 ```
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-07 10:00"
+$ tzconv -f ny -t bud "2023-03-07 10:00"
 EST: 2023-03-07 10:00 (America/New_York)
 CET: 2023-03-07 16:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-14 10:00"
+$ tzconv -f ny -t bud "2023-03-14 10:00"
 EDT: 2023-03-14 10:00 (America/New_York)
 CET: 2023-03-14 15:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-28 10:00"
+$ tzconv -f ny -t bud "2023-03-28 10:00"
 EDT: 2023-03-28 10:00 (America/New_York)
 CEST: 2023-03-28 16:00 (Europe/Budapest)
 $
 ```
 
 ### Custom shell commands for common conversions
```

### Comparing `tzconv-1.2/README.md` & `tzconv-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: tzconv
+Version: 1.3
+Summary: command-line tool to convert a date and time to several time zones at once
+Home-page: https://codeberg.org/gnyeki/tzconv
+Author: Gabor Nyeki
+Description-Content-Type: text/markdown
+
 
 # `tzconv`: convert a date and time to several time zones at once
 
 This Python package provides a small command-line utility to convert a `YYYY-MM-DD HH:MM` formatted date and time to several other time zones.
 
 ## Installation
 
@@ -23,85 +31,86 @@
 ### Basic usage
 
 `tzconv` uses the time zone information available through your operating system, so time zones have to be specified accordingly:
 
 ```
 $ tzconv \
     -f America/New_York \
-    -t America/Lima \
-    -t Asia/Seoul \
+    -t Pacific/Galapagos \
+    -t America/Santa_Isabel \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
-Time zone names can be shortened as long as they remain unique:
+Time zone names can be shortened as long as they remain unique.
+Initials, prefixes, and abbreviations are all recognized:
 
 ```
 $ tzconv \
-    -f america/ne \
-    -t america/li \
-    -t asia/se \
+    -f ny \
+    -t gal \
+    -t san_i \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
 Available time zones can be listed with the `--list-tz` option (or `-l` for short):
 
 ```
-$ tzconv -l america/n
-The following time zones are available that begin with 'america/n':
+$ tzconv -l am/n
+The following time zones are available that match 'am/n':
 
   America/Nassau, America/New_York, America/Nipigon, America/Nome,
   America/Noronha, America/North_Dakota/Beulah, America/North_Dakota/Center,
   America/North_Dakota/New_Salem, America/Nuuk
 $
 ```
 
 ### Imputing the current date and the current time
 
 If the date is omitted, today's date is imputed:
 
 ```
-$ tzconv -f america/ne -t africa/ad 10:00
+$ tzconv -f ny -t aa 10:00
 EDT: 2023-04-20 10:00 (America/New_York)
 EAT: 2023-04-20 17:00 (Africa/Addis_Ababa)
 $
 
 ```
 
 If the time is omitted, too, then `tzconv` imputes the current time:
 
 ```
-$ tzconv -f america/ne -t africa/ad
+$ tzconv -f ny -t aa
 EDT: 2023-04-20 15:03 (America/New_York)
 EAT: 2023-04-20 22:03 (Africa/Addis_Ababa)
 $
 ```
 
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
 
 ```
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-07 10:00"
+$ tzconv -f ny -t bud "2023-03-07 10:00"
 EST: 2023-03-07 10:00 (America/New_York)
 CET: 2023-03-07 16:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-14 10:00"
+$ tzconv -f ny -t bud "2023-03-14 10:00"
 EDT: 2023-03-14 10:00 (America/New_York)
 CET: 2023-03-14 15:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-28 10:00"
+$ tzconv -f ny -t bud "2023-03-28 10:00"
 EDT: 2023-03-28 10:00 (America/New_York)
 CEST: 2023-03-28 16:00 (Europe/Budapest)
 $
 ```
 
 ### Custom shell commands for common conversions
```

### Comparing `tzconv-1.2/setup.py` & `tzconv-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as handle:
     readme = handle.read()
 
 setup(
     name="tzconv",
-    version="1.2",
+    version="1.3",
     description="command-line tool to convert a date and time to several time zones at once",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Gabor Nyeki",
     url="https://codeberg.org/gnyeki/tzconv",
     packages=["tzconv"],
     install_requires=["click"],
```

### Comparing `tzconv-1.2/tzconv.egg-info/PKG-INFO` & `tzconv-1.3/tzconv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzconv
-Version: 1.2
+Version: 1.3
 Summary: command-line tool to convert a date and time to several time zones at once
 Home-page: https://codeberg.org/gnyeki/tzconv
 Author: Gabor Nyeki
 Description-Content-Type: text/markdown
 
 
 # `tzconv`: convert a date and time to several time zones at once
@@ -31,85 +31,86 @@
 ### Basic usage
 
 `tzconv` uses the time zone information available through your operating system, so time zones have to be specified accordingly:
 
 ```
 $ tzconv \
     -f America/New_York \
-    -t America/Lima \
-    -t Asia/Seoul \
+    -t Pacific/Galapagos \
+    -t America/Santa_Isabel \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
-Time zone names can be shortened as long as they remain unique:
+Time zone names can be shortened as long as they remain unique.
+Initials, prefixes, and abbreviations are all recognized:
 
 ```
 $ tzconv \
-    -f america/ne \
-    -t america/li \
-    -t asia/se \
+    -f ny \
+    -t gal \
+    -t san_i \
     "2023-04-25 10:00"
 EDT: 2023-04-25 10:00 (America/New_York)
--05: 2023-04-25 09:00 (America/Lima)
-KST: 2023-04-25 23:00 (Asia/Seoul)
+-06: 2023-04-25 08:00 (Pacific/Galapagos)
+PDT: 2023-04-25 07:00 (America/Santa_Isabel)
 $
 ```
 
 Available time zones can be listed with the `--list-tz` option (or `-l` for short):
 
 ```
-$ tzconv -l america/n
-The following time zones are available that begin with 'america/n':
+$ tzconv -l am/n
+The following time zones are available that match 'am/n':
 
   America/Nassau, America/New_York, America/Nipigon, America/Nome,
   America/Noronha, America/North_Dakota/Beulah, America/North_Dakota/Center,
   America/North_Dakota/New_Salem, America/Nuuk
 $
 ```
 
 ### Imputing the current date and the current time
 
 If the date is omitted, today's date is imputed:
 
 ```
-$ tzconv -f america/ne -t africa/ad 10:00
+$ tzconv -f ny -t aa 10:00
 EDT: 2023-04-20 10:00 (America/New_York)
 EAT: 2023-04-20 17:00 (Africa/Addis_Ababa)
 $
 
 ```
 
 If the time is omitted, too, then `tzconv` imputes the current time:
 
 ```
-$ tzconv -f america/ne -t africa/ad
+$ tzconv -f ny -t aa
 EDT: 2023-04-20 15:03 (America/New_York)
 EAT: 2023-04-20 22:03 (Africa/Addis_Ababa)
 $
 ```
 
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
 
 ```
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-07 10:00"
+$ tzconv -f ny -t bud "2023-03-07 10:00"
 EST: 2023-03-07 10:00 (America/New_York)
 CET: 2023-03-07 16:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-14 10:00"
+$ tzconv -f ny -t bud "2023-03-14 10:00"
 EDT: 2023-03-14 10:00 (America/New_York)
 CET: 2023-03-14 15:00 (Europe/Budapest)
-$ tzconv -f America/New_York -t Europe/Budapest "2023-03-28 10:00"
+$ tzconv -f ny -t bud "2023-03-28 10:00"
 EDT: 2023-03-28 10:00 (America/New_York)
 CEST: 2023-03-28 16:00 (Europe/Budapest)
 $
 ```
 
 ### Custom shell commands for common conversions
```

