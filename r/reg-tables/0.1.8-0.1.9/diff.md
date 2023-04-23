# Comparing `tmp/reg_tables-0.1.8.tar.gz` & `tmp/reg_tables-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reg_tables-0.1.8.tar", last modified: Mon Aug  8 14:07:38 2022, max compression
+gzip compressed data, was "reg_tables-0.1.9.tar", last modified: Tue Aug  9 09:16:28 2022, max compression
```

## Comparing `reg_tables-0.1.8.tar` & `reg_tables-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-08 14:07:38.847957 reg_tables-0.1.8/
--rw-r--r--   0 abramo     (501) staff       (20)     1517 2022-06-07 18:54:05.000000 reg_tables-0.1.8/LICENSE
--rw-r--r--   0 abramo     (501) staff       (20)     3687 2022-08-08 14:07:38.848016 reg_tables-0.1.8/PKG-INFO
--rw-r--r--   0 abramo     (501) staff       (20)     2855 2022-06-10 11:16:11.000000 reg_tables-0.1.8/README.md
--rw-r--r--   0 abramo     (501) staff       (20)       84 2022-06-10 11:07:22.000000 reg_tables-0.1.8/pyproject.toml
-drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-08 14:07:38.847055 reg_tables-0.1.8/reg_tables/
--rw-r--r--   0 abramo     (501) staff       (20)       29 2022-06-10 12:26:45.000000 reg_tables-0.1.8/reg_tables/__init__.py
--rw-r--r--   0 abramo     (501) staff       (20)     8412 2022-08-08 14:07:08.000000 reg_tables-0.1.8/reg_tables/main.py
-drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-08 14:07:38.847825 reg_tables-0.1.8/reg_tables.egg-info/
--rw-r--r--   0 abramo     (501) staff       (20)     3687 2022-08-08 14:07:38.000000 reg_tables-0.1.8/reg_tables.egg-info/PKG-INFO
--rw-r--r--   0 abramo     (501) staff       (20)      262 2022-08-08 14:07:38.000000 reg_tables-0.1.8/reg_tables.egg-info/SOURCES.txt
--rw-r--r--   0 abramo     (501) staff       (20)        1 2022-08-08 14:07:38.000000 reg_tables-0.1.8/reg_tables.egg-info/dependency_links.txt
--rw-r--r--   0 abramo     (501) staff       (20)       26 2022-08-08 14:07:38.000000 reg_tables-0.1.8/reg_tables.egg-info/requires.txt
--rw-r--r--   0 abramo     (501) staff       (20)       11 2022-08-08 14:07:38.000000 reg_tables-0.1.8/reg_tables.egg-info/top_level.txt
--rw-r--r--   0 abramo     (501) staff       (20)       79 2022-08-08 14:07:38.848206 reg_tables-0.1.8/setup.cfg
--rw-r--r--   0 abramo     (501) staff       (20)     1268 2022-08-08 14:05:14.000000 reg_tables-0.1.8/setup.py
+drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-09 09:16:28.726766 reg_tables-0.1.9/
+-rw-r--r--   0 abramo     (501) staff       (20)     1517 2022-06-07 18:54:05.000000 reg_tables-0.1.9/LICENSE
+-rw-r--r--   0 abramo     (501) staff       (20)     3687 2022-08-09 09:16:28.726823 reg_tables-0.1.9/PKG-INFO
+-rw-r--r--   0 abramo     (501) staff       (20)     2855 2022-06-10 11:16:11.000000 reg_tables-0.1.9/README.md
+-rw-r--r--   0 abramo     (501) staff       (20)       84 2022-06-10 11:07:22.000000 reg_tables-0.1.9/pyproject.toml
+drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-09 09:16:28.725897 reg_tables-0.1.9/reg_tables/
+-rw-r--r--   0 abramo     (501) staff       (20)       29 2022-06-10 12:26:45.000000 reg_tables-0.1.9/reg_tables/__init__.py
+-rw-r--r--   0 abramo     (501) staff       (20)     8407 2022-08-09 09:12:30.000000 reg_tables-0.1.9/reg_tables/main.py
+drwxr-xr-x   0 abramo     (501) staff       (20)        0 2022-08-09 09:16:28.726657 reg_tables-0.1.9/reg_tables.egg-info/
+-rw-r--r--   0 abramo     (501) staff       (20)     3687 2022-08-09 09:16:28.000000 reg_tables-0.1.9/reg_tables.egg-info/PKG-INFO
+-rw-r--r--   0 abramo     (501) staff       (20)      262 2022-08-09 09:16:28.000000 reg_tables-0.1.9/reg_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 abramo     (501) staff       (20)        1 2022-08-09 09:16:28.000000 reg_tables-0.1.9/reg_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 abramo     (501) staff       (20)       26 2022-08-09 09:16:28.000000 reg_tables-0.1.9/reg_tables.egg-info/requires.txt
+-rw-r--r--   0 abramo     (501) staff       (20)       11 2022-08-09 09:16:28.000000 reg_tables-0.1.9/reg_tables.egg-info/top_level.txt
+-rw-r--r--   0 abramo     (501) staff       (20)       79 2022-08-09 09:16:28.727033 reg_tables-0.1.9/setup.cfg
+-rw-r--r--   0 abramo     (501) staff       (20)     1268 2022-08-09 09:12:40.000000 reg_tables-0.1.9/setup.py
```

### Comparing `reg_tables-0.1.8/LICENSE` & `reg_tables-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reg_tables-0.1.8/PKG-INFO` & `reg_tables-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reg_tables
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple linearmodelsextension to run panel regressions with different specifications and export the results in a professional-looking latex table
 Home-page: https://www.abarbon.com
 Download-URL: https://github.com/AndreaBarbon/reg_tables/archive/refs/tags/0.0.5.tar.gz
 Author: Andrea Barbon, Kirill Kazakov
 Author-email: andrea.3arbon@gmail.com
 License: MIT
 Keywords: Linear models,regression table
```

### Comparing `reg_tables-0.1.8/README.md` & `reg_tables-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `reg_tables-0.1.8/reg_tables/main.py` & `reg_tables-0.1.9/reg_tables/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             if coeff_decimals!=None:
                 def change_decimals(cell):
                     try:
                         return re.sub('^-?[0-9]*\.[0-9]*',str(round(float(re.search('^-?[0-9]*\.[0-9]*' ,cell)[0]),coeff_decimals)),cell)
                     except:
                         return cell
                 coeffs=coeffs.applymap(change_decimals)
-                s = "\{0:0.{0}f\}".format(coeff_decimals)
+                s = "{0:0."+str(coeff_decimals)+"f}"
                 R2s  = [ s.format(x) for x in R2s ]
             else:
                 R2s  = [ "{0:0.4f}".format(x) for x in R2s ]
 
             if const!=0:coeffs=pd.concat([coeffs[2:],coeffs[0:2]])
             coeffs_dict={}
             for idx,name in enumerate(coeffs.index):
```

### Comparing `reg_tables-0.1.8/reg_tables.egg-info/PKG-INFO` & `reg_tables-0.1.9/reg_tables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reg-tables
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple linearmodelsextension to run panel regressions with different specifications and export the results in a professional-looking latex table
 Home-page: https://www.abarbon.com
 Download-URL: https://github.com/AndreaBarbon/reg_tables/archive/refs/tags/0.0.5.tar.gz
 Author: Andrea Barbon, Kirill Kazakov
 Author-email: andrea.3arbon@gmail.com
 License: MIT
 Keywords: Linear models,regression table
```

### Comparing `reg_tables-0.1.8/setup.py` & `reg_tables-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh: long_description = fh.read()
 
 setuptools.setup(
     name="reg_tables",                     
-    version="0.1.8",
+    version="0.1.9",
     author="Andrea Barbon, Kirill Kazakov",                     
     author_email='andrea.3arbon@gmail.com',
     url = 'https://www.abarbon.com',
     download_url='https://github.com/AndreaBarbon/reg_tables/archive/refs/tags/0.0.5.tar.gz',
     description="A simple linearmodelsextension to run panel regressions with different specifications and export the results in a professional-looking latex table",
     license='MIT',
     long_description=long_description,
```

