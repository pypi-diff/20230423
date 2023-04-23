# Comparing `tmp/mymoviebook-1.8.0.tar.gz` & `tmp/mymoviebook-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymoviebook-1.8.0.tar", last modified: Sun Jun  5 06:28:45 2022, max compression
+gzip compressed data, was "mymoviebook-1.9.0.tar", last modified: Sun Nov 13 05:40:51 2022, max compression
```

## Comparing `mymoviebook-1.8.0.tar` & `mymoviebook-1.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.071207 mymoviebook-1.8.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2018-11-25 05:56:19.000000 mymoviebook-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      269 2020-01-04 09:12:39.000000 mymoviebook-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5150 2022-06-05 06:10:53.000000 mymoviebook-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/doc/
--rw-r--r--   0 root         (0) root         (0)   106543 2022-06-05 06:25:38.000000 mymoviebook-1.8.0/doc/Doxyfile
--rw-r--r--   0 root         (0) root         (0)       73 2020-05-16 06:04:35.000000 mymoviebook-1.8.0/doc/ENTITY_RELATIONSHIP.md
--rw-r--r--   0 root         (0) root         (0)      620 2020-05-16 06:07:04.000000 mymoviebook-1.8.0/doc/index.dox
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/locale/
--rw-r--r--   0 root         (0) root         (0)     9491 2022-06-05 06:21:07.000000 mymoviebook-1.8.0/locale/es.po
--rw-r--r--   0 root         (0) root         (0)    11548 2022-06-05 06:21:07.000000 mymoviebook-1.8.0/locale/fr.po
--rw-r--r--   0 root         (0) root         (0)     4953 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/locale/mymoviebook.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/man/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/man/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/man/es/man1/
--rw-r--r--   0 root         (0) root         (0)     2009 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/man/es/man1/mymoviebook.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/man/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/man/fr/man1/
--rw-r--r--   0 root         (0) root         (0)     1865 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/man/fr/man1/mymoviebook.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/man/man1/
--rw-r--r--   0 root         (0) root         (0)     1816 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/man/man1/mymoviebook.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.069207 mymoviebook-1.8.0/mymoviebook/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-28 04:49:38.000000 mymoviebook-1.8.0/mymoviebook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/images/
--rw-r--r--   0 root         (0) root         (0)   148291 2019-01-03 11:08:24.000000 mymoviebook-1.8.0/mymoviebook/images/mymoviebook.png
--rw-r--r--   0 root         (0) root         (0)    21907 2019-01-03 11:08:24.000000 mymoviebook-1.8.0/mymoviebook/images/mymoviebook_doxygen.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/mymoviebook/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/mymoviebook/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/locale/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     8416 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/mymoviebook/locale/es/LC_MESSAGES/mymoviebook.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.068207 mymoviebook-1.8.0/mymoviebook/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1566 2022-06-05 06:23:57.000000 mymoviebook-1.8.0/mymoviebook/locale/fr/LC_MESSAGES/mymoviebook.mo
--rw-r--r--   0 root         (0) root         (0)     3759 2021-10-02 16:46:30.000000 mymoviebook-1.8.0/mymoviebook/mem.py
--rw-r--r--   0 root         (0) root         (0)     1429 2021-10-02 16:46:41.000000 mymoviebook-1.8.0/mymoviebook/mymoviebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/objects/
--rw-r--r--   0 root         (0) root         (0)    17794 2021-10-03 10:35:20.000000 mymoviebook-1.8.0/mymoviebook/objects/films.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/reusing/
--rw-r--r--   0 root         (0) root         (0)     3642 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/admin_pg.py
--rw-r--r--   0 root         (0) root         (0)     1115 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/call_by_name.py
--rw-r--r--   0 root         (0) root         (0)     9769 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/casts.py
--rw-r--r--   0 root         (0) root         (0)    10305 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/connection_pg.py
--rw-r--r--   0 root         (0) root         (0)    17619 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/datetime_functions.py
--rw-r--r--   0 root         (0) root         (0)     3625 2019-01-09 20:01:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/dbupdates.py
--rw-r--r--   0 root         (0) root         (0)     3178 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/decorators.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/file_functions.py
--rw-r--r--   0 root         (0) root         (0)     2584 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/github.py
--rw-r--r--   0 root         (0) root         (0)    24873 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/libmanagers.py
--rw-r--r--   0 root         (0) root         (0)     4635 2022-06-05 06:04:31.000000 mymoviebook-1.8.0/mymoviebook/reusing/text_inputs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook/sql/
--rw-r--r--   0 root         (0) root         (0)     4598 2019-01-09 20:01:31.000000 mymoviebook-1.8.0/mymoviebook/sql/mymoviebook.sql
--rw-r--r--   0 root         (0) root         (0)      631 2019-01-09 20:01:31.000000 mymoviebook-1.8.0/mymoviebook/sql/update_sql_dir.sh
--rw-r--r--   0 root         (0) root         (0)       84 2022-06-05 06:09:38.000000 mymoviebook-1.8.0/mymoviebook/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-05 06:28:45.070207 mymoviebook-1.8.0/mymoviebook.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2022-06-05 06:28:44.000000 mymoviebook-1.8.0/mymoviebook.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1223 2022-06-05 06:28:45.000000 mymoviebook-1.8.0/mymoviebook.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-05 06:28:44.000000 mymoviebook-1.8.0/mymoviebook.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-06-05 06:28:44.000000 mymoviebook-1.8.0/mymoviebook.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-11-25 06:25:27.000000 mymoviebook-1.8.0/mymoviebook.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       33 2022-06-05 06:28:44.000000 mymoviebook-1.8.0/mymoviebook.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-06-05 06:28:44.000000 mymoviebook-1.8.0/mymoviebook.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3297 2021-10-03 03:25:45.000000 mymoviebook-1.8.0/mymoviebook.epj
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-05 06:28:45.071207 mymoviebook-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11695 2022-06-05 06:28:18.000000 mymoviebook-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.977484 mymoviebook-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2018-11-25 05:56:19.000000 mymoviebook-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      269 2020-01-04 09:12:39.000000 mymoviebook-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2022-11-13 05:40:51.977484 mymoviebook-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5245 2022-11-13 05:37:11.000000 mymoviebook-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/doc/
+-rw-r--r--   0 root         (0) root         (0)   106543 2022-11-13 05:32:28.000000 mymoviebook-1.9.0/doc/Doxyfile
+-rw-r--r--   0 root         (0) root         (0)       73 2020-05-16 06:04:35.000000 mymoviebook-1.9.0/doc/ENTITY_RELATIONSHIP.md
+-rw-r--r--   0 root         (0) root         (0)      620 2020-05-16 06:07:04.000000 mymoviebook-1.9.0/doc/index.dox
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/locale/
+-rw-r--r--   0 root         (0) root         (0)     8749 2022-11-13 05:28:14.000000 mymoviebook-1.9.0/locale/es.po
+-rw-r--r--   0 root         (0) root         (0)    11697 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/locale/fr.po
+-rw-r--r--   0 root         (0) root         (0)     5102 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/locale/mymoviebook.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/man/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.974484 mymoviebook-1.9.0/man/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/man/es/man1/
+-rw-r--r--   0 root         (0) root         (0)     2009 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/man/es/man1/mymoviebook.1
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/man/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/man/fr/man1/
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/man/fr/man1/mymoviebook.1
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/man/man1/
+-rw-r--r--   0 root         (0) root         (0)     1816 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/man/man1/mymoviebook.1
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-28 04:49:38.000000 mymoviebook-1.9.0/mymoviebook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook/images/
+-rw-r--r--   0 root         (0) root         (0)   148291 2019-01-03 11:08:24.000000 mymoviebook-1.9.0/mymoviebook/images/mymoviebook.png
+-rw-r--r--   0 root         (0) root         (0)    21907 2019-01-03 11:08:24.000000 mymoviebook-1.9.0/mymoviebook/images/mymoviebook_doxygen.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/mymoviebook/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/mymoviebook/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook/locale/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     8691 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/mymoviebook/locale/es/LC_MESSAGES/mymoviebook.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.975484 mymoviebook-1.9.0/mymoviebook/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     1566 2022-11-13 05:28:24.000000 mymoviebook-1.9.0/mymoviebook/locale/fr/LC_MESSAGES/mymoviebook.mo
+-rw-r--r--   0 root         (0) root         (0)     3759 2021-10-02 16:46:30.000000 mymoviebook-1.9.0/mymoviebook/mem.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-11-09 04:25:11.000000 mymoviebook-1.9.0/mymoviebook/mymoviebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook/objects/
+-rw-r--r--   0 root         (0) root         (0)    18290 2022-11-13 05:27:40.000000 mymoviebook-1.9.0/mymoviebook/objects/films.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.977484 mymoviebook-1.9.0/mymoviebook/reusing/
+-rw-r--r--   0 root         (0) root         (0)     3642 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/admin_pg.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/call_by_name.py
+-rw-r--r--   0 root         (0) root         (0)     9769 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/casts.py
+-rw-r--r--   0 root         (0) root         (0)    10305 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/connection_pg.py
+-rw-r--r--   0 root         (0) root         (0)    17619 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/datetime_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2019-01-09 20:01:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/dbupdates.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/file_functions.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/github.py
+-rw-r--r--   0 root         (0) root         (0)    24873 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/libmanagers.py
+-rw-r--r--   0 root         (0) root         (0)     4635 2022-06-05 06:04:31.000000 mymoviebook-1.9.0/mymoviebook/reusing/text_inputs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.977484 mymoviebook-1.9.0/mymoviebook/sql/
+-rw-r--r--   0 root         (0) root         (0)     4598 2019-01-09 20:01:31.000000 mymoviebook-1.9.0/mymoviebook/sql/mymoviebook.sql
+-rw-r--r--   0 root         (0) root         (0)      631 2019-01-09 20:01:31.000000 mymoviebook-1.9.0/mymoviebook/sql/update_sql_dir.sh
+-rw-r--r--   0 root         (0) root         (0)       86 2022-11-13 05:12:21.000000 mymoviebook-1.9.0/mymoviebook/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 05:40:51.976484 mymoviebook-1.9.0/mymoviebook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-11-25 06:25:27.000000 mymoviebook-1.9.0/mymoviebook.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-11-13 05:40:51.000000 mymoviebook-1.9.0/mymoviebook.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3297 2021-10-03 03:25:45.000000 mymoviebook-1.9.0/mymoviebook.epj
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-13 05:40:51.977484 mymoviebook-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    12144 2022-11-13 05:38:38.000000 mymoviebook-1.9.0/setup.py
```

### Comparing `mymoviebook-1.8.0/LICENSE` & `mymoviebook-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/PKG-INFO` & `mymoviebook-1.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymoviebook
-Version: 1.8.0
+Version: 1.9.0
 Summary: Generate your own personal movie collection book
 Home-page: https://github.com/Turulomio/mymoviebook
 Author: Turulomio
 Author-email: turulomio@yahoo.es
 License: GPL-3
 Keywords: movie collection book
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymoviebook-1.8.0/README.md` & `mymoviebook-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,37 +67,41 @@
 We can add as many directories as we want.
 
 Generating book movie
 ---------------------
 
 Once all our movies are quickly added to database and if our latex is working (pdflatex command is needed), after executing
 
-`mymoviebook --generate --output /home/user/mymoviebook.pdf`
+`mymoviebook --report /home/user/mymoviebook.pdf`
 
 we get our movie collection book. This is the ![demo movie book](https://raw.githubusercontent.com/Turulomio/mymoviebook/master/doc/demo.pdf).
 
 
 Links
 =====
 
 Doxygen documentation:
-    http://turulomio.users.sourceforge.net/doxygen/mymoviebook/
+    https://coolnewton.mooo.com/doxygen/mymoviebook/
 
 Pypi web page:
     https://pypi.org/project/mymoviebook/
 
 Dependencies
 ============
 * https://www.python.org/, as the main programming language.
 * https://pypi.org/project/colorama/, to give console colors.
 * https://www.latex-project.org/, to generate PDF documents
 * https://github.com/turulomio/officegenerator/, to generate ODT documents (Beta)
 
 Changelog
 =========
+1.9.0 (2022-11-13)
+------------------
+-  --insert parameter now checks there aren't more than 6 films per directory
+
 1.8.0
 -----
 - Replaced officegenerator by unogenerator
 
 1.7.0
 -----
 - Fixed error parsing names
```

### Comparing `mymoviebook-1.8.0/doc/Doxyfile` & `mymoviebook-1.9.0/doc/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = MyMovieBook
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER         = 1.8.0
+PROJECT_NUMBER         = 1.9.0
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          = "Generate your personal movie collection book"
```

### Comparing `mymoviebook-1.8.0/doc/index.dox` & `mymoviebook-1.9.0/doc/index.dox`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/locale/es.po` & `mymoviebook-1.9.0/locale/es.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # root <turulomio@yahoo.es>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: RecPermissions\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-05 08:21+0200\n"
+"POT-Creation-Date: 2022-11-13 06:23+0100\n"
 "PO-Revision-Date: 2018-10-22 18:51+0100\n"
 "Last-Translator: root <turulomio@yahoo.es>\n"
 "Language-Team: Spanish\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -227,48 +227,21 @@
 
 msgid "Checking that the movies have the correct format..."
 msgstr "Comprobando que las películas tienen el formato correcto..."
 
 msgid "There isn't a movie with the same name '{}'"
 msgstr "No hay una película con el mismo nombre '{}'"
 
+msgid "Checking the number of films in the directory..."
+msgstr "Comprobando el número de películas en el directorio..."
+
+msgid "There are more than 6 films in this directory. Please fix it."
+msgstr "Hay más de 6 películas en este directorio. Por favor corrígelo."
+
 msgid "Do you want to overwrite the information of directory '{}'?"
 msgstr "¿Quieres sobreescribir la información del directorio '{}'?"
 
 msgid "Deleting information..."
 msgstr "Borrando la información..."
 
 msgid "Adding movies to the database"
 msgstr "Añadiendo películas a la base de datos"
-
-#~ msgid "Write the password for {}"
-#~ msgstr "Escribe la contraseña para {}"
-
-#~ msgid "Postgres database connection parameters"
-#~ msgstr "Parámetros de conexión de la base de datos Postgres"
-
-#~ msgid "Postgresql user"
-#~ msgstr "Usuario de Postgresql"
-
-#~ msgid "Postgresql server port"
-#~ msgstr "Puerto del servidor Postgres"
-
-#~ msgid "Postgresql server address"
-#~ msgstr "Dirección del servidor Postgres"
-
-#~ msgid "Postgresql database"
-#~ msgstr "Base de datos Postgresql"
-
-#~ msgid "MyMovieBook database needs to be updated. Please login with a superuser role."
-#~ msgstr "La base de datos de MyMovieBook necesita ser actualizada. Por favor autentícate con un perfil de administrador."
-
-#~ msgid "MyMovieBook app is older than database. Please update it."
-#~ msgstr "La aplicación MyMovieBook es más antigua que la base de datos. Por favor actualízala."
-
-#~ msgid "Y"
-#~ msgstr "S"
-
-#~ msgid "N"
-#~ msgstr "N"
-
-#~ msgid "Please enter '{}' or '{}'"
-#~ msgstr "Por favor introduce '{}' o '{}'"
```

### Comparing `mymoviebook-1.8.0/locale/fr.po` & `mymoviebook-1.9.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Turulomio <turulomio@yahoo.es>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: RecPermissions\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-05 08:21+0200\n"
+"POT-Creation-Date: 2022-11-13 06:28+0100\n"
 "PO-Revision-Date: 2018-11-03 07:11+0100\n"
 "Last-Translator: root <turulomio@yahoo.es>\n"
 "Language-Team: French\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -226,14 +226,20 @@
 
 msgid "Checking that the movies have the correct format..."
 msgstr ""
 
 msgid "There isn't a movie with the same name '{}'"
 msgstr ""
 
+msgid "Checking the number of films in the directory..."
+msgstr ""
+
+msgid "There are more than 6 films in this directory. Please fix it."
+msgstr ""
+
 msgid "Do you want to overwrite the information of directory '{}'?"
 msgstr ""
 
 msgid "Deleting information..."
 msgstr ""
 
 msgid "Adding movies to the database"
```

### Comparing `mymoviebook-1.8.0/locale/mymoviebook.pot` & `mymoviebook-1.9.0/locale/mymoviebook.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-05 08:23+0200\n"
+"POT-Creation-Date: 2022-11-13 06:28+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -226,14 +226,20 @@
 
 msgid "Checking that the movies have the correct format..."
 msgstr ""
 
 msgid "There isn't a movie with the same name '{}'"
 msgstr ""
 
+msgid "Checking the number of films in the directory..."
+msgstr ""
+
+msgid "There are more than 6 films in this directory. Please fix it."
+msgstr ""
+
 msgid "Do you want to overwrite the information of directory '{}'?"
 msgstr ""
 
 msgid "Deleting information..."
 msgstr ""
 
 msgid "Adding movies to the database"
```

### Comparing `mymoviebook-1.8.0/man/es/man1/mymoviebook.1` & `mymoviebook-1.9.0/man/es/man1/mymoviebook.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH MYMOVIEBOOK 1 2022\-06\-05
+.TH MYMOVIEBOOK 1 2022\-11\-13
 .SH NAME
 
 .B mymoviebook:
 Cambia el propietario y los permisos de ficheros y directorios recursivamente.
 .SH SYNOPSIS
 
 mymoviebook usage: mymoviebook [\-h] [\-\-version] [\-\-insert | \-\-generate] [\-\-user USER]
```

### Comparing `mymoviebook-1.8.0/man/fr/man1/mymoviebook.1` & `mymoviebook-1.9.0/man/fr/man1/mymoviebook.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH MYMOVIEBOOK 1 2022\-06\-05
+.TH MYMOVIEBOOK 1 2022\-11\-13
 .SH NAME
 
 .B mymoviebook:
 Changer le propri\('etaire et les permissions des fichiers et des r\('epertoires r\('ecursivement.
 .SH SYNOPSIS
 
 mymoviebook usage: mymoviebook [\-h] [\-\-version] [\-\-insert | \-\-generate] [\-\-user USER]
```

### Comparing `mymoviebook-1.8.0/man/man1/mymoviebook.1` & `mymoviebook-1.9.0/man/man1/mymoviebook.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH MYMOVIEBOOK 1 2022\-06\-05
+.TH MYMOVIEBOOK 1 2022\-11\-13
 .SH NAME
 
 .B mymoviebook:
 Change files and directories owner and permissions recursively.
 .SH SYNOPSIS
 
 mymoviebook usage: mymoviebook [\-h] [\-\-version] [\-\-insert | \-\-generate] [\-\-user USER]
```

### Comparing `mymoviebook-1.8.0/mymoviebook/images/mymoviebook.png` & `mymoviebook-1.9.0/mymoviebook/images/mymoviebook.png`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/images/mymoviebook_doxygen.png` & `mymoviebook-1.9.0/mymoviebook/images/mymoviebook_doxygen.png`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/locale/es/LC_MESSAGES/mymoviebook.mo` & `mymoviebook-1.9.0/mymoviebook/locale/es/LC_MESSAGES/mymoviebook.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -48,14 +48,17 @@
 msgstr ""
 "Cambia el propietario y los permisos de ficheros y directorios "
 "recursivamente."
 
 msgid "Checking that the movies have the correct format..."
 msgstr "Comprobando que las películas tienen el formato correcto..."
 
+msgid "Checking the number of films in the directory..."
+msgstr "Comprobando el número de películas en el directorio..."
+
 msgid ""
 "Creates a new postgresql database, checking if already exists. Copy "
 "MyMovieBook schema on it"
 msgstr ""
 "Crea una nueva base de datos en postgresql, si no existiera. Copia el "
 "esquema de MyMovieBook en ella"
 
@@ -193,14 +196,17 @@
 msgid ""
 "The main page of the project is in \\href{https://github.com/turulomio/"
 "mymoviebook}{GitHub}."
 msgstr ""
 "La página principal del proyecto se encuentra en \\href{https://github.com/"
 "turulomio/mymoviebook}{GitHub}."
 
+msgid "There are more than 6 films in this directory. Please fix it."
+msgstr "Hay más de 6 películas en este directorio. Por favor corrígelo."
+
 msgid "There are {} collection films duplicated."
 msgstr "Hay {} películas duplicadas en la colección."
 
 msgid "There are {} collection films in this year:"
 msgstr "Hay {} películas de la colección en este año:"
 
 msgid "There are {} collection films without year."
```

### Comparing `mymoviebook-1.8.0/mymoviebook/locale/fr/LC_MESSAGES/mymoviebook.mo` & `mymoviebook-1.9.0/mymoviebook/locale/fr/LC_MESSAGES/mymoviebook.mo`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/mem.py` & `mymoviebook-1.9.0/mymoviebook/mem.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/mymoviebook.py` & `mymoviebook-1.9.0/mymoviebook/mymoviebook.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/objects/films.py` & `mymoviebook-1.9.0/mymoviebook/objects/films.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,22 +85,22 @@
         
     ## Includes the cover in latex. Remember that to scape {} in python strings, you need to double them {{}}
     ## Used for one  cover in a different paragrahp
     ## @param width Float with the width of the cover
     ## @param height Float with the height of the cover
     ## @param show_name Boolean. If True shows the name and the id_dvd. If False only show id_dvd
     ## @return string
-    def tex_cover_tabular(self,width=2.2,height=2.2, show_name=True):
+    def tex_cover_tabular(self,width=2,height=2, show_name=True):
         bd=""       
-        bd=bd + "\\begin{tabular}{m{2.3cm} m{15cm}}\n"
+        bd=bd + "\\begin{tabular}{ m{2.2cm} m{13cm} }\n"
         if show_name==True:
-            bd=bd + "{0} & {1}. (~\\nameref{{sec:{2}}} )\\\\\n".format(self.tex_cover(width, height), string2tex(self.name()), self.id_dvd)
+            bd=bd + "{0} & {1}. (~\\nameref{{sec:{2}}} )\n".format(self.tex_cover(width, height), string2tex(self.name()), self.id_dvd)
         else:
-            bd=bd + "{0} & ~\\nameref{{sec:{1}}}\\\\\n".format(self.tex_cover(width, height), self.id_dvd)#Reference to DVD page
-        bd = bd + "\\end{tabular} \\\\\n\n"
+            bd=bd + "{0} & ~\\nameref{{sec:{1}}}\n".format(self.tex_cover(width, height), self.id_dvd)#Reference to DVD page
+        bd = bd + "\\end{tabular} \n\n"
         return bd
 
     ## Coverpath points to the path of the file system where the cover is. 
     def save(self, coverpath):
         if self.id==None:
             self.id=self.mem.con.cursor_one_field("insert into films (savedate, name, id_dvd) values (%s, %s, %s) returning id_films",(self.savedate, self.rawname, self.id_dvd))
             bytea=open(coverpath, "rb").read()
@@ -129,18 +129,19 @@
         header = header + "\\usepackage{geometry}\n"
         header = header + "\\usepackage{setspace}\n"
         header = header + "\\usepackage{graphicx}\n"
         header = header + "\\usepackage{ae,aecompl}\n"
         header = header + "\\usepackage[bookmarksnumbered, colorlinks=true, urlcolor=blue, linkcolor=blue, pdftitle={"+ self.mem._("My movie book") +"}, pdfauthor={MyMovieBook-"+ __version__ +"}, pdfkeywords={movie book}]{hyperref}\n"
         header = header + "\\geometry{verbose,a4paper}\n"
         header = header + "\\usepackage{anysize}\n"
-        header = header + "\\marginsize{1.5cm}{1.5cm}{1.5cm}{1.5cm} \n"
+        header = header + "\\marginsize{1.5cm}{1.5cm}{0.5cm}{1cm} \n"
         header = header + "\\usepackage{array}\n"
         header = header + "\\begin{document}\n"
         header = header + "\\title{\\textbf{" + self.mem._("My movie book") + "}}\n"
+        header = header + "\\author{MyMovieBook-"+ __version__ +"}\n"
 
         header = header + "\\setlength{\\parindent}{1cm}\n"
         header = header + "\\setlength{\\parskip}{0.2cm}\n"
 
 
         bd=""
         bd=bd + "\\maketitle\n"
@@ -156,40 +157,44 @@
         bd=bd + self.mem._("The main page of the project is in \href{https://github.com/turulomio/mymoviebook}{GitHub}.")+ "\\par\n"
         bd=bd + self.mem._("This book has {} movies and it was generated at {}.").format(self.length(), datetime.now().time()) +"\\par\n"
         bd=bd + self.mem._("If you make click over a film cover, you'll be redirected to FilmAffinity portal to try to get information of the movie.")
         bd=bd +"\\newpage\n"
 
         print ("  - " + self.mem._("List by index"))
         bd = bd + "\section{"+ self.mem._("Big covers") +"}\n"
+        bd = bd + "\\setlength{\\parindent}{0cm}\n"
         for id_dvd in reversed(self.distinct_id_dvd()):
             bd=bd + "\\subsection*{"+ self.mem._("Index") + " " + str(id_dvd)+"}\n" 
             bd=bd + "\\label{{sec:{0}}}\n".format(id_dvd)
             bd=bd + "\\addcontentsline{toc}{subsection}{"+ self.mem._("Index") + " " + str(id_dvd)+"}\n" 
+            
+            bd=bd + "\\begin{center}\n"
             bd=bd + "\\begin{tabular}{c c}\n"
             for i, fi in enumerate(self.films_in_id_dvd(id_dvd).arr):
-                bd=bd+ "\\begin{tabular}{p{7.1cm}}\n" #Tabla foto name interior
-                bd=bd+ fi.tex_cover(6.7,6.7) + "\\\\\n"
+                bd=bd+ "\\begin{tabular}{p{8cm}}\n" #Tabla foto name interior
+                bd=bd+ fi.tex_cover(8,6.8) + "\\\\\n"
                 bd=bd+ string2tex(fi) +"\\\\\n"
                 bd=bd+ "\\end{tabular} &"
                 if i % 2==1:
                     bd=bd[:-2]+"\\\\\n"
             bd = bd + "\\end{tabular}\n"
+            bd=bd + "\\end{center}\n"
             bd=bd +"\n\\newpage\n\n"
 
 
         print (self.mem._("  - Films list with small covers"))
         bd = bd + "\\setlength{\\parindent}{0cm}\n"
         bd=bd + "\section{"+ self.mem._("Small covers") +"}\n"
         for id_dvd in reversed(self.distinct_id_dvd()):
-            bd=bd + "\\begin{tabular}{m{2.1cm} m{2.1cm} m{2.1cm} m{2.1cm} m{2.1cm} m{2.1cm} m{2.1cm}}\n"
+            bd=bd + "\\begin{tabular}{m{2cm} m{2cm} m{2cm} m{2cm} m{2cm} m{2cm} m{2cm}}\n"
             bd=bd + self.mem._("Index") + " " +str(id_dvd) + " & "
             for fi in self.films_in_id_dvd(id_dvd).arr:
-                bd=bd + fi.tex_cover(2.1,2.1) + " &" 
-            bd = bd[:-2]  + "\\\\\n"
-            bd = bd + "\\end{tabular} \\\\\n\n"
+                bd=bd + fi.tex_cover(2,2) + " &" 
+            bd = bd[:-2]  + "\n"
+            bd = bd + "\\end{tabular} \n\n"
         bd=bd +"\n\\newpage\n\n"
 
         print (self.mem._("  - Films list ordered by title"))
         bd=bd + "\section{"+self.mem._("Order by movie title") +"}\n"
         self.order_by_name()
         for f in self.arr:
             bd=bd + "\\subsection*{"+ string2tex(f) + "} \n"
@@ -375,18 +380,28 @@
         print (mem._("Current directory is not numeric"))
         exit(100)
 
     if input_YN(mem._("The id of the directory to add is '{}'. Do you want to continue?").format(id))==False:
         exit(100)
 
     print ("+ " + mem._("Checking that the movies have the correct format..."))
+    
+    number_images=0
     for file in glob( getcwd()+ "/*.jpg" ):
         if path.exists(file[:-3]+"avi")==False and path.exists(file[:-3]+"mpg")==False and path.exists(file[:-3]+"mkv")==False:
             print (mem._("There isn't a movie with the same name '{}'").format(file[:-3]))
             exit(100)
+        number_images=number_images+1
+        
+    #Check if there are more than 6 images
+    print ("+ " + mem._("Checking the number of films in the directory..."))
+    if number_images>6:
+        print(mem._("There are more than 6 films in this directory. Please fix it."))
+        exit(100)
+        
 
     # "Chequeando si hay registros en la base de datos del dispositivo " + str(id)
     sf=FilmManager_from_db_query(mem, mem.con.mogrify("SELECT * FROM films WHERE id_dvd=%s", (id, )))
     if sf.length()>0:
         if input_YN("+ " + mem._("Do you want to overwrite the information of directory '{}'?").format(id))==False:
             exit(100)
         else:
```

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/admin_pg.py` & `mymoviebook-1.9.0/mymoviebook/reusing/admin_pg.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/call_by_name.py` & `mymoviebook-1.9.0/mymoviebook/reusing/call_by_name.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/casts.py` & `mymoviebook-1.9.0/mymoviebook/reusing/casts.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/connection_pg.py` & `mymoviebook-1.9.0/mymoviebook/reusing/connection_pg.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/datetime_functions.py` & `mymoviebook-1.9.0/mymoviebook/reusing/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/dbupdates.py` & `mymoviebook-1.9.0/mymoviebook/reusing/dbupdates.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/decorators.py` & `mymoviebook-1.9.0/mymoviebook/reusing/decorators.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/github.py` & `mymoviebook-1.9.0/mymoviebook/reusing/github.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/libmanagers.py` & `mymoviebook-1.9.0/mymoviebook/reusing/libmanagers.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/reusing/text_inputs.py` & `mymoviebook-1.9.0/mymoviebook/reusing/text_inputs.py`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/sql/mymoviebook.sql` & `mymoviebook-1.9.0/mymoviebook/sql/mymoviebook.sql`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook/sql/update_sql_dir.sh` & `mymoviebook-1.9.0/mymoviebook/sql/update_sql_dir.sh`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook.egg-info/PKG-INFO` & `mymoviebook-1.9.0/mymoviebook.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymoviebook
-Version: 1.8.0
+Version: 1.9.0
 Summary: Generate your own personal movie collection book
 Home-page: https://github.com/Turulomio/mymoviebook
 Author: Turulomio
 Author-email: turulomio@yahoo.es
 License: GPL-3
 Keywords: movie collection book
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymoviebook-1.8.0/mymoviebook.egg-info/SOURCES.txt` & `mymoviebook-1.9.0/mymoviebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/mymoviebook.epj` & `mymoviebook-1.9.0/mymoviebook.epj`

 * *Files identical despite different names*

### Comparing `mymoviebook-1.8.0/setup.py` & `mymoviebook-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,50 @@
 import gettext
 import os
 from platform import system as platform_system
 import site
 
 gettext.install('mymoviebook', 'mymoviebook/locale')
 
+
+
+## Class to define doxygen command
 class Doxygen(Command):
     description = "Create/update doxygen documentation in doc/html"
-    user_options = []
+
+    user_options = [
+      # The format is (long option, short option, description).
+      ( 'user=', None, 'Remote ssh user'),
+      ( 'directory=', None, 'Remote ssh path'),
+      ( 'port=', None, 'Remote ssh port'),
+      ( 'server=', None, 'Remote ssh server'),
+  ]
 
     def initialize_options(self):
-        pass
+        self.user="root"
+        self.directory="/var/www/html/doxygen/mymoviebook/"
+        self.port=22
+        self.server="127.0.0.1"
 
     def finalize_options(self):
         pass
 
     def run(self):
         print("Creating Doxygen Documentation")
         os.system("""sed -i -e "41d" doc/Doxyfile""")#Delete line 41
         os.system("""sed -i -e "41iPROJECT_NUMBER         = {}" doc/Doxyfile""".format(__version__))#Insert line 41
         os.system("rm -Rf build")
         os.chdir("doc")
-        os.system("doxygen Doxyfile") 
-
-        os.system("rsync -avzP -e 'ssh -l turulomio' html/ frs.sourceforge.net:/home/users/t/tu/turulomio/userweb/htdocs/doxygen/mymoviebook/ --delete-after")
+        os.system("doxygen Doxyfile")      
+        command=f"""rsync -avzP -e 'ssh -l {self.user} -p {self.port} ' html/ {self.server}:{self.directory} --delete-after"""
+        print(command)
+        os.system(command)
         os.chdir("..")
 
+
 class Procedure(Command):
     description = "Create/update doxygen documentation in doc/html"
     user_options = []
 
     def initialize_options(self):
         pass
 
@@ -47,15 +62,15 @@
         print("  * python setup.py doc")
         print("  * python setup.py install")
         print("  * python setup.py doxygen")
         print("  * git commit -a -m 'mymoviebook-{}'".format(__version__))
         print("  * git push")
         print(_("  * Make a new tag in github"))
         print("  * python setup.py sdist")
-        print("  * twine upload dist/unogenerator-{0}.tar.gz".format(__version__))
+        print("  * twine upload dist/mymoviebook-{0}.tar.gz".format(__version__))
         print("  * python setup.py uninstall")
         print(_("  * Create a new gentoo ebuild with the new version"))
         print(_("  * Upload to portage repository")) 
 
 class Uninstall(Command):
     description = "Uninstall installed files with install"
     user_options = []
@@ -253,15 +268,15 @@
     author='Turulomio',
     author_email='turulomio@yahoo.es',
     license='GPL-3',
     packages=['mymoviebook'],
     entry_points = {'console_scripts': ['mymoviebook=mymoviebook.mymoviebook:main',
                                        ],
                    },
-    install_requires=['colorama','setuptools', 'unogenerator'],
+    install_requires=['colorama','setuptools', 'unogenerator', 'mangenerator'],
     data_files=data_files,
     cmdclass={ 'doxygen': Doxygen,
                'doc': Doc,
                'uninstall': Uninstall,
                'video': Video,
                'procedure': Procedure,
                'reusing': Reusing,
```

