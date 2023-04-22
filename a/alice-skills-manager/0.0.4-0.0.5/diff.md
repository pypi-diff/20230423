# Comparing `tmp/alice-skills-manager-0.0.4.tar.gz` & `tmp/alice-skills-manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice-skills-manager-0.0.4.tar", last modified: Sat Apr 22 22:24:43 2023, max compression
+gzip compressed data, was "alice-skills-manager-0.0.5.tar", last modified: Sat Apr 22 22:28:27 2023, max compression
```

## Comparing `alice-skills-manager-0.0.4.tar` & `alice-skills-manager-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:24:43.417405 alice-skills-manager-0.0.4/
--rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2023-04-22 22:24:43.416379 alice-skills-manager-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 22:24:43.396809 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/
--rw-rw-rw-   0        0        0      617 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 22:24:43.000000 alice-skills-manager-0.0.4/alice_skills_manager.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 22:24:43.413811 alice-skills-manager-0.0.4/asm/
--rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.4/asm/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.4/asm/__main__.py
--rw-rw-rw-   0        0        0    20216 2023-04-22 21:57:47.000000 alice-skills-manager-0.0.4/asm/alice_skills_manager.py
--rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.4/asm/exceptions.py
--rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.4/asm/skill_entry.py
--rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.4/asm/skill_repo.py
--rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.4/asm/skill_state.py
--rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.4/asm/util.py
--rw-rw-rw-   0        0        0       42 2023-04-22 22:24:43.417918 alice-skills-manager-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1822 2023-04-22 22:23:06.000000 alice-skills-manager-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:28:27.735601 alice-skills-manager-0.0.5/
+-rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      617 2023-04-22 22:28:27.733542 alice-skills-manager-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 22:28:27.708343 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 22:28:27.000000 alice-skills-manager-0.0.5/alice_skills_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 22:28:27.730972 alice-skills-manager-0.0.5/asm/
+-rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.5/asm/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.5/asm/__main__.py
+-rw-rw-rw-   0        0        0    20216 2023-04-22 21:57:47.000000 alice-skills-manager-0.0.5/asm/alice_skills_manager.py
+-rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.5/asm/exceptions.py
+-rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.5/asm/skill_entry.py
+-rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.5/asm/skill_repo.py
+-rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.5/asm/skill_state.py
+-rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.5/asm/util.py
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:28:27.735601 alice-skills-manager-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1822 2023-04-22 22:27:41.000000 alice-skills-manager-0.0.5/setup.py
```

### Comparing `alice-skills-manager-0.0.4/PKG-INFO` & `alice-skills-manager-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-skills-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
 Author: Alice-IA
 Author-email: yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `alice-skills-manager-0.0.4/README.md` & `alice-skills-manager-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/alice_skills_manager.egg-info/PKG-INFO` & `alice-skills-manager-0.0.5/alice_skills_manager.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-skills-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
 Author: Alice-IA
 Author-email: yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `alice-skills-manager-0.0.4/asm/__main__.py` & `alice-skills-manager-0.0.5/asm/__main__.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/alice_skills_manager.py` & `alice-skills-manager-0.0.5/asm/alice_skills_manager.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/exceptions.py` & `alice-skills-manager-0.0.5/asm/exceptions.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/skill_entry.py` & `alice-skills-manager-0.0.5/asm/skill_entry.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/skill_repo.py` & `alice-skills-manager-0.0.5/asm/skill_repo.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/skill_state.py` & `alice-skills-manager-0.0.5/asm/skill_state.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/asm/util.py` & `alice-skills-manager-0.0.5/asm/util.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.4/setup.py` & `alice-skills-manager-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 
 setup(
     name='alice-skills-manager',
-    version='0.0.4',
+    version='0.0.5',
     packages=['asm'],
     install_requires=required('requirements/requirements.txt'),
     package_data={'': package_files('asm')},
     # tests_require=required('requirements/tests.txt'),
     python_requires='>=3.6',
     url='https://github.com/Alice-IA/alice-skills-manager',
     license='Apache-2.0',
```

