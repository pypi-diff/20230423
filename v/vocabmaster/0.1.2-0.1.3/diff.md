# Comparing `tmp/vocabmaster-0.1.2.tar.gz` & `tmp/vocabmaster-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.2.tar", last modified: Sun Apr 23 17:59:58 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.3.tar", last modified: Sun Apr 23 18:11:53 2023, max compression
```

## Comparing `vocabmaster-0.1.2.tar` & `vocabmaster-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.735184 vocabmaster-0.1.2/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.2/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2560 2023-04-23 17:55:42.000000 vocabmaster-0.1.2/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 17:59:58.735184 vocabmaster-0.1.2/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 17:59:52.000000 vocabmaster-0.1.2/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.2/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18035 2023-04-23 17:51:07.000000 vocabmaster-0.1.2/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.2/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.2/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.2/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.2/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 17:59:58.725184 vocabmaster-0.1.2/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 17:59:58.000000 vocabmaster-0.1.2/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.3/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2560 2023-04-23 17:55:42.000000 vocabmaster-0.1.3/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 18:11:40.000000 vocabmaster-0.1.3/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.865177 vocabmaster-0.1.3/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.3/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18018 2023-04-23 18:08:54.000000 vocabmaster-0.1.3/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.3/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.3/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.3/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.3/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.2/LICENSE` & `vocabmaster-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.2/PKG-INFO` & `vocabmaster-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: vocabmaster
-Version: 0.1.2
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
```

### Comparing `vocabmaster-0.1.2/README.md` & `vocabmaster-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: vocabmaster
+Version: 0.1.3
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
```

### Comparing `vocabmaster-0.1.2/setup.py` & `vocabmaster-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.2/vocabmaster/cli.py` & `vocabmaster-0.1.3/vocabmaster/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,14 @@
         )
 
 
 def print_default_language_pair():
     """
     Print the current default language pair.
     """
-    click.echo()
     click.echo(f"{BLUE}The current default language pair is:{RESET}")
     default_language_to_learn = config_handler.get_default_language_pair()[
         "language_to_learn"
     ]
     default_mother_tongue = config_handler.get_default_language_pair()["mother_tongue"]
     click.echo(
         f"{BOLD}{ORANGE}{default_language_to_learn}:{default_mother_tongue}{RESET}"
```

### Comparing `vocabmaster-0.1.2/vocabmaster/config_handler.py` & `vocabmaster-0.1.3/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.2/vocabmaster/csv_handler.py` & `vocabmaster-0.1.3/vocabmaster/csv_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.2/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.3/vocabmaster/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.2/vocabmaster/utils.py` & `vocabmaster-0.1.3/vocabmaster/utils.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.2/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.3/vocabmaster.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.2
+Version: 0.1.3
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
```

