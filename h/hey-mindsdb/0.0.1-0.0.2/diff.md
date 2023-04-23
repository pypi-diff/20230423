# Comparing `tmp/hey-mindsdb-0.0.1.tar.gz` & `tmp/hey-mindsdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hey-mindsdb-0.0.1.tar", last modified: Sat Apr 22 16:13:37 2023, max compression
+gzip compressed data, was "hey-mindsdb-0.0.2.tar", last modified: Sun Apr 23 08:05:24 2023, max compression
```

## Comparing `hey-mindsdb-0.0.1.tar` & `hey-mindsdb-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.953612 hey-mindsdb-0.0.1/
--rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey-mindsdb-0.0.1/LICENSE
--rw-r--r--   0 sadra      (501) staff       (20)      190 2023-04-22 16:11:10.000000 hey-mindsdb-0.0.1/MANIFEST.in
--rw-r--r--   0 sadra      (501) staff       (20)     1685 2023-04-22 16:13:37.953660 hey-mindsdb-0.0.1/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)      979 2023-04-18 09:48:31.000000 hey-mindsdb-0.0.1/README.md
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.950383 hey-mindsdb-0.0.1/hey/
--rw-r--r--   0 sadra      (501) staff       (20)      126 2023-04-22 15:53:14.000000 hey-mindsdb-0.0.1/hey/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2780 2023-04-22 15:42:30.000000 hey-mindsdb-0.0.1/hey/cli.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.951135 hey-mindsdb-0.0.1/hey/constants/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey-mindsdb-0.0.1/hey/constants/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      594 2023-04-22 16:01:00.000000 hey-mindsdb-0.0.1/hey/constants/informations.py
--rw-r--r--   0 sadra      (501) staff       (20)      130 2023-04-22 08:20:35.000000 hey-mindsdb-0.0.1/hey/constants/service.py
--rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey-mindsdb-0.0.1/hey/constants/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.951900 hey-mindsdb-0.0.1/hey/exceptions/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey-mindsdb-0.0.1/hey/exceptions/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey-mindsdb-0.0.1/hey/exceptions/auth.py
--rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey-mindsdb-0.0.1/hey/exceptions/connection.py
--rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey-mindsdb-0.0.1/hey/exceptions/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.952184 hey-mindsdb-0.0.1/hey/middlewares/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey-mindsdb-0.0.1/hey/middlewares/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2406 2023-04-22 15:16:23.000000 hey-mindsdb-0.0.1/hey/middlewares/mindsdb.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.953077 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/
--rw-r--r--   0 sadra      (501) staff       (20)     1685 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)      626 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/SOURCES.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/dependency_links.txt
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/entry_points.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/not-zip-safe
--rw-r--r--   0 sadra      (501) staff       (20)       49 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/requires.txt
--rw-r--r--   0 sadra      (501) staff       (20)        4 2023-04-22 16:13:37.000000 hey-mindsdb-0.0.1/hey_mindsdb.egg-info/top_level.txt
--rw-r--r--   0 sadra      (501) staff       (20)     1277 2023-04-22 16:13:37.953927 hey-mindsdb-0.0.1/setup.cfg
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey-mindsdb-0.0.1/setup.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-22 16:13:37.953415 hey-mindsdb-0.0.1/tests/
--rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey-mindsdb-0.0.1/tests/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey-mindsdb-0.0.1/tests/test_accounts.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437730 hey-mindsdb-0.0.2/
+-rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey-mindsdb-0.0.2/LICENSE
+-rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey-mindsdb-0.0.2/MANIFEST.in
+-rw-r--r--   0 sadra      (501) staff       (20)     5060 2023-04-23 08:05:24.437778 hey-mindsdb-0.0.2/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)     3861 2023-04-23 08:00:16.000000 hey-mindsdb-0.0.2/README.md
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.434116 hey-mindsdb-0.0.2/hey/
+-rw-r--r--   0 sadra      (501) staff       (20)      126 2023-04-23 08:05:04.000000 hey-mindsdb-0.0.2/hey/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2780 2023-04-23 05:58:41.000000 hey-mindsdb-0.0.2/hey/cli.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.434986 hey-mindsdb-0.0.2/hey/constants/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey-mindsdb-0.0.2/hey/constants/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      594 2023-04-22 16:01:00.000000 hey-mindsdb-0.0.2/hey/constants/informations.py
+-rw-r--r--   0 sadra      (501) staff       (20)      130 2023-04-22 08:20:35.000000 hey-mindsdb-0.0.2/hey/constants/service.py
+-rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey-mindsdb-0.0.2/hey/constants/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.435822 hey-mindsdb-0.0.2/hey/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey-mindsdb-0.0.2/hey/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey-mindsdb-0.0.2/hey/exceptions/auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey-mindsdb-0.0.2/hey/exceptions/connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey-mindsdb-0.0.2/hey/exceptions/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.436225 hey-mindsdb-0.0.2/hey/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey-mindsdb-0.0.2/hey/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2498 2023-04-23 06:45:03.000000 hey-mindsdb-0.0.2/hey/middlewares/mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437190 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/
+-rw-r--r--   0 sadra      (501) staff       (20)     5060 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)      626 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/entry_points.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/not-zip-safe
+-rw-r--r--   0 sadra      (501) staff       (20)       49 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/requires.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        4 2023-04-23 08:05:24.000000 hey-mindsdb-0.0.2/hey_mindsdb.egg-info/top_level.txt
+-rw-r--r--   0 sadra      (501) staff       (20)     1660 2023-04-23 08:05:24.438049 hey-mindsdb-0.0.2/setup.cfg
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey-mindsdb-0.0.2/setup.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-23 08:05:24.437511 hey-mindsdb-0.0.2/tests/
+-rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey-mindsdb-0.0.2/tests/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey-mindsdb-0.0.2/tests/test_accounts.py
```

### Comparing `hey-mindsdb-0.0.1/LICENSE` & `hey-mindsdb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.1/hey/cli.py` & `hey-mindsdb-0.0.2/hey/cli.py`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.1/hey/constants/informations.py` & `hey-mindsdb-0.0.2/hey/constants/informations.py`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.1/hey/middlewares/mindsdb.py` & `hey-mindsdb-0.0.2/hey/middlewares/mindsdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     def collect_database(server: Server) -> Database:
         return server.list_databases()[0]
 
     def answer(self, question: str) -> Markdown:
         """
         takes the question and queries then converts the response into `rich.Markdown`
         Args:
-            question: 
+            question: the value from `ask` positional argument
 
         Returns:
-
+            response from MindsDB in Markdown format
         """
         return Markdown(to_data(
             self.database.query(
                 MindsDB.SQL_ASKING_QUERY.format(question)
             ).fetch()
         ))
```

### Comparing `hey-mindsdb-0.0.1/hey_mindsdb.egg-info/SOURCES.txt` & `hey-mindsdb-0.0.2/hey_mindsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.0.1/setup.cfg` & `hey-mindsdb-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 [metadata]
 author = Sadra Yahyapour
 author_email = lnxpylnxpy@gmail.com
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
+	Intended Audience :: Education
 	License :: OSI Approved :: MIT License
+	Operating System :: Unix
+	Operating System :: POSIX
 	Natural Language :: English
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: Implementation :: PyPy
+	Topic :: Utilities
 description = Your AI-powered pair programming friend.
 license = MIT license
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = hey
 name = hey-mindsdb
 url = https://github.com/lnxpy/hey
-version = 0.0.1
+version = 0.0.2
 
 [options]
 python_requires = >=3.6
 install_requires = 
 	mindsdb-sdk>=1.0.2
 	keyring>=23.13.1
 	rich>=13.3.4
@@ -35,15 +45,15 @@
 	hey.*
 
 [options.entry_points]
 console_scripts = 
 	hey=hey.cli:main
 
 [bumpversion]
-current_version = 0.0.1
+current_version = 0.0.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

