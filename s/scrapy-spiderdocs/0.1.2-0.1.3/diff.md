# Comparing `tmp/scrapy-spiderdocs-0.1.2.tar.gz` & `tmp/scrapy-spiderdocs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapy-spiderdocs-0.1.2.tar", last modified: Wed Jan 11 02:58:58 2017, max compression
+gzip compressed data, was "scrapy-spiderdocs-0.1.3.tar", last modified: Sun Apr 23 08:37:31 2023, max compression
```

## Comparing `scrapy-spiderdocs-0.1.2.tar` & `scrapy-spiderdocs-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/documented/
--rw-r--r--   0 nanvel     (501) staff       (20)        0 2017-01-07 13:55:59.000000 scrapy-spiderdocs-0.1.2/documented/__init__.py
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/documented/commands/
--rw-r--r--   0 nanvel     (501) staff       (20)        0 2017-01-07 14:29:17.000000 scrapy-spiderdocs-0.1.2/documented/commands/__init__.py
--rw-r--r--   0 nanvel     (501) staff       (20)     5212 2017-01-11 02:57:26.000000 scrapy-spiderdocs-0.1.2/documented/commands/spiderdocs.py
--rw-r--r--   0 nanvel     (501) staff       (20)     3493 2017-01-10 03:33:17.000000 scrapy-spiderdocs-0.1.2/documented/settings.py
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/documented/spiders/
--rw-r--r--   0 nanvel     (501) staff       (20)      161 2017-01-07 13:55:59.000000 scrapy-spiderdocs-0.1.2/documented/spiders/__init__.py
--rw-r--r--   0 nanvel     (501) staff       (20)      911 2017-01-11 02:43:03.000000 scrapy-spiderdocs-0.1.2/documented/spiders/example.py
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/documented/tests/
--rw-r--r--   0 nanvel     (501) staff       (20)       29 2017-01-07 17:25:04.000000 scrapy-spiderdocs-0.1.2/documented/tests/__init__.py
--rw-r--r--   0 nanvel     (501) staff       (20)      184 2017-01-08 06:58:57.000000 scrapy-spiderdocs-0.1.2/documented/tests/test_commands.py
--rw-r--r--   0 nanvel     (501) staff       (20)      357 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/PKG-INFO
--rw-r--r--   0 nanvel     (501) staff       (20)     3583 2017-01-10 04:11:24.000000 scrapy-spiderdocs-0.1.2/README.rst
-drwxr-xr-x   0 nanvel     (501) staff       (20)        0 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/
--rw-r--r--   0 nanvel     (501) staff       (20)        1 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/dependency_links.txt
--rw-r--r--   0 nanvel     (501) staff       (20)       71 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/entry_points.txt
--rw-r--r--   0 nanvel     (501) staff       (20)      357 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/PKG-INFO
--rw-r--r--   0 nanvel     (501) staff       (20)       12 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/requires.txt
--rw-r--r--   0 nanvel     (501) staff       (20)      503 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/SOURCES.txt
--rw-r--r--   0 nanvel     (501) staff       (20)       11 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/scrapy_spiderdocs.egg-info/top_level.txt
--rw-r--r--   0 nanvel     (501) staff       (20)       59 2017-01-11 02:58:58.000000 scrapy-spiderdocs-0.1.2/setup.cfg
--rw-r--r--   0 nanvel     (501) staff       (20)     1637 2017-01-11 02:57:57.000000 scrapy-spiderdocs-0.1.2/setup.py
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.861198 scrapy-spiderdocs-0.1.3/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)      145 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/AUTHORS
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     1083 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/LICENSE
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     5816 2023-04-23 08:37:31.861098 scrapy-spiderdocs-0.1.3/PKG-INFO
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     4330 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/README.rst
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.859357 scrapy-spiderdocs-0.1.3/documented/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/__init__.py
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.859582 scrapy-spiderdocs-0.1.3/documented/commands/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/commands/__init__.py
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     5284 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/commands/spiderdocs.py
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     3493 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/settings.py
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.859876 scrapy-spiderdocs-0.1.3/documented/spiders/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)      161 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/spiders/__init__.py
+-rw-r--r--   0 nanvel-air   (501) staff       (20)      911 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/spiders/example.py
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.860155 scrapy-spiderdocs-0.1.3/documented/tests/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)       29 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/tests/__init__.py
+-rw-r--r--   0 nanvel-air   (501) staff       (20)      184 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/documented/tests/test_commands.py
+drwxr-xr-x   0 nanvel-air   (501) staff       (20)        0 2023-04-23 08:37:31.860903 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     5816 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/PKG-INFO
+-rw-r--r--   0 nanvel-air   (501) staff       (20)      519 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 nanvel-air   (501) staff       (20)        1 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 nanvel-air   (501) staff       (20)       70 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/entry_points.txt
+-rw-r--r--   0 nanvel-air   (501) staff       (20)       12 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/requires.txt
+-rw-r--r--   0 nanvel-air   (501) staff       (20)       29 2023-04-23 08:37:31.000000 scrapy-spiderdocs-0.1.3/scrapy_spiderdocs.egg-info/top_level.txt
+-rw-r--r--   0 nanvel-air   (501) staff       (20)       38 2023-04-23 08:37:31.861229 scrapy-spiderdocs-0.1.3/setup.cfg
+-rw-r--r--   0 nanvel-air   (501) staff       (20)     2067 2023-04-23 08:33:57.000000 scrapy-spiderdocs-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scrapy-spiderdocs-0.1.2/documented/commands/spiderdocs.py` & `scrapy-spiderdocs-0.1.3/documented/commands/spiderdocs.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,21 @@
 
     def short_desc(self):
         return "Generate spiders documentation md file for specified module."
 
     def add_options(self, parser):
         parser.usage = "usage: scrapy spiderdocs [<module.name>] [-o <filename.md>]"
         ScrapyCommand.add_options(self, parser)
-        parser.add_option("-o", "--output", dest="output_filename", metavar="FILE", help="Output file name.")
+        parser.add_argument(
+            "-o",
+            "--output",
+            dest="output_filename",
+            metavar="FILE",
+            help="Output file name."
+        )
 
     def process_options(self, args, opts):
         ScrapyCommand.process_options(self, args, opts)
         if args:
             self._locations[args[0]] = opts.output_filename
         else:
             locations = self.settings.get('SPIDERDOCS_LOCATIONS', None)
```

### Comparing `scrapy-spiderdocs-0.1.2/documented/settings.py` & `scrapy-spiderdocs-0.1.3/documented/settings.py`

 * *Files identical despite different names*

### Comparing `scrapy-spiderdocs-0.1.2/documented/spiders/example.py` & `scrapy-spiderdocs-0.1.3/documented/spiders/example.py`

 * *Files identical despite different names*

