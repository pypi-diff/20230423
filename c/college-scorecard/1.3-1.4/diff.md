# Comparing `tmp/college-scorecard-1.3.tar.gz` & `tmp/college-scorecard-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "college-scorecard-1.3.tar", last modified: Tue Jan  3 18:55:36 2023, max compression
+gzip compressed data, was "college-scorecard-1.4.tar", last modified: Sun Apr 23 01:17:33 2023, max compression
```

## Comparing `college-scorecard-1.3.tar` & `college-scorecard-1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 18:55:36.337318 college-scorecard-1.3/
--rw-rw-rw-   0        0        0     1090 2022-09-11 17:22:46.000000 college-scorecard-1.3/LICENSE
--rw-rw-rw-   0        0        0     1092 2023-01-03 18:55:36.337318 college-scorecard-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-01-03 16:14:03.000000 college-scorecard-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-03 18:55:36.333327 college-scorecard-1.3/college_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-01-03 18:55:36.000000 college-scorecard-1.3/college_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-01-03 18:55:36.000000 college-scorecard-1.3/college_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 18:55:36.000000 college-scorecard-1.3/college_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-01-03 18:55:36.000000 college-scorecard-1.3/college_scorecard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-03 18:55:36.336320 college-scorecard-1.3/scorecard/
--rw-rw-rw-   0        0        0     3357 2023-01-03 18:53:31.000000 college-scorecard-1.3/scorecard/api.py
--rw-rw-rw-   0        0        0      376 2022-09-22 17:29:26.000000 college-scorecard-1.3/scorecard/exceptions.py
--rw-rw-rw-   0        0        0     6431 2023-01-03 18:50:39.000000 college-scorecard-1.3/scorecard/objects.py
--rw-rw-rw-   0        0        0       86 2023-01-03 18:55:36.340317 college-scorecard-1.3/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-01-03 18:52:48.000000 college-scorecard-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:33.476466 college-scorecard-1.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 00:53:19.000000 college-scorecard-1.4/LICENSE
+-rw-rw-rw-   0        0        0     1051 2023-04-23 01:17:33.476466 college-scorecard-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-04-23 00:53:19.000000 college-scorecard-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:33.476466 college-scorecard-1.4/college_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1051 2023-04-23 01:17:33.000000 college-scorecard-1.4/college_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-23 01:17:33.000000 college-scorecard-1.4/college_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:17:33.000000 college-scorecard-1.4/college_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 01:17:33.000000 college-scorecard-1.4/college_scorecard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 01:17:33.476466 college-scorecard-1.4/scorecard/
+-rw-rw-rw-   0        0        0       66 2023-04-23 01:11:15.000000 college-scorecard-1.4/scorecard/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-04-23 00:53:19.000000 college-scorecard-1.4/scorecard/api.py
+-rw-rw-rw-   0        0        0      376 2023-04-23 00:53:19.000000 college-scorecard-1.4/scorecard/exceptions.py
+-rw-rw-rw-   0        0        0     6431 2023-04-23 00:53:19.000000 college-scorecard-1.4/scorecard/objects.py
+-rw-rw-rw-   0        0        0       86 2023-04-23 01:17:33.501333 college-scorecard-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-04-23 01:13:55.000000 college-scorecard-1.4/setup.py
```

### Comparing `college-scorecard-1.3/LICENSE` & `college-scorecard-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `college-scorecard-1.3/PKG-INFO` & `college-scorecard-1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: college-scorecard
-Version: 1.3
+Version: 1.4
 Summary: A python library for collegescorecard.ed.gov
 Home-page: https://github.com/ahoodatheguy/scorecard
 Author: Ahadu Kebede
 Author-email: ahadukebede@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scorecard
 
 A python library for collegescorecard.ed.gov
 
@@ -41,9 +39,7 @@
 You can also search for a specific college using it's id.
 
 ```python
 howard = sc.search(id=131520)
 ```
 
 For further information you can read the [documentation](https://scorecard.readthedocs.io/en/latest/)
-
-
```

### Comparing `college-scorecard-1.3/README.md` & `college-scorecard-1.4/README.md`

 * *Files identical despite different names*

### Comparing `college-scorecard-1.3/college_scorecard.egg-info/PKG-INFO` & `college-scorecard-1.4/college_scorecard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: college-scorecard
-Version: 1.3
+Version: 1.4
 Summary: A python library for collegescorecard.ed.gov
 Home-page: https://github.com/ahoodatheguy/scorecard
 Author: Ahadu Kebede
 Author-email: ahadukebede@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scorecard
 
 A python library for collegescorecard.ed.gov
 
@@ -41,9 +39,7 @@
 You can also search for a specific college using it's id.
 
 ```python
 howard = sc.search(id=131520)
 ```
 
 For further information you can read the [documentation](https://scorecard.readthedocs.io/en/latest/)
-
-
```

### Comparing `college-scorecard-1.3/scorecard/api.py` & `college-scorecard-1.4/scorecard/api.py`

 * *Files identical despite different names*

### Comparing `college-scorecard-1.3/scorecard/objects.py` & `college-scorecard-1.4/scorecard/objects.py`

 * *Files identical despite different names*

