# Comparing `tmp/sweetrpg-library-objects-0.0.85.tar.gz` & `tmp/sweetrpg-library-objects-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sweetrpg-library-objects-0.0.85.tar", last modified: Thu Mar 10 04:22:04 2022, max compression
+gzip compressed data, was "dist/sweetrpg-library-objects-0.0.86.tar", last modified: Thu Mar 10 04:24:53 2022, max compression
```

## Comparing `sweetrpg-library-objects-0.0.85.tar` & `sweetrpg-library-objects-0.0.86.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/
--rwxr-xr-x   0 root         (0) root         (0)     1065 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6502 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     5819 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1198 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      343 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/
--rwxr-xr-x   0 root         (0) root         (0)      373 2022-03-10 04:22:02.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/contribution/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/contribution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1069 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/contribution/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/person/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/person/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1045 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/person/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/publisher/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/publisher/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      796 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/publisher/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/review/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/review/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1174 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/review/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/studio/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/studio/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/studio/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/system/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/system/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      745 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/system/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/volume/
--rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/volume/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1140 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/volume/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/
--rwxr-xr-x   0 root         (0) root         (0)       98 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/contribution/
--rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/contribution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1285 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/contribution/document.py
--rwxr-xr-x   0 root         (0) root         (0)      474 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/contribution/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/
--rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/property/
--rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/property/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/property/document.py
--rw-r--r--   0 root         (0) root         (0)      510 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/property/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/tag/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/tag/__init__.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/tag/document.py
--rw-r--r--   0 root         (0) root         (0)      392 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/embedded/tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/
--rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1274 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/document.py
--rwxr-xr-x   0 root         (0) root         (0)      542 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/
--rwxr-xr-x   0 root         (0) root         (0)      119 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1173 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/document.py
--rwxr-xr-x   0 root         (0) root         (0)      554 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/
--rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1287 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/document.py
--rwxr-xr-x   0 root         (0) root         (0)      598 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/
--rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1319 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/document.py
--rwxr-xr-x   0 root         (0) root         (0)      542 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/
--rwxr-xr-x   0 root         (0) root         (0)      121 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1220 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/document.py
--rwxr-xr-x   0 root         (0) root         (0)      512 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/
--rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1549 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/document.py
--rwxr-xr-x   0 root         (0) root         (0)      812 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/
--rwxr-xr-x   0 root         (0) root         (0)       95 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      780 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/contribution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/
--rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      533 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/property.py
--rwxr-xr-x   0 root         (0) root         (0)      621 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/tag.py
--rwxr-xr-x   0 root         (0) root         (0)      638 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/person.py
--rwxr-xr-x   0 root         (0) root         (0)      607 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/publisher.py
--rwxr-xr-x   0 root         (0) root         (0)      871 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/review.py
--rwxr-xr-x   0 root         (0) root         (0)      595 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/studio.py
--rwxr-xr-x   0 root         (0) root         (0)      610 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/system.py
--rwxr-xr-x   0 root         (0) root         (0)      773 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/utils/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3078 2022-03-10 04:22:00.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/utils/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6502 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3326 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       95 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-03-10 04:22:04.000000 sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/
+-rwxr-xr-x   0 root         (0) root         (0)     1065 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6502 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     5819 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1198 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      343 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/
+-rwxr-xr-x   0 root         (0) root         (0)      373 2022-03-10 04:24:52.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/contribution/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/contribution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1069 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/contribution/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/person/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/person/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1045 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/person/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/publisher/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/publisher/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      796 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/publisher/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/review/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/review/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1174 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/review/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/studio/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/studio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/studio/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/system/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/system/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      745 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/system/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/volume/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/volume/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1140 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/volume/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/
+-rwxr-xr-x   0 root         (0) root         (0)       98 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/contribution/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/contribution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1285 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/contribution/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      474 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/contribution/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/property/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/property/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/property/document.py
+-rw-r--r--   0 root         (0) root         (0)      510 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/property/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/tag/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/tag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/tag/document.py
+-rw-r--r--   0 root         (0) root         (0)      392 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/embedded/tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1274 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      542 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/
+-rwxr-xr-x   0 root         (0) root         (0)      119 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1173 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      554 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1287 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      598 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1319 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      542 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/
+-rwxr-xr-x   0 root         (0) root         (0)      121 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1220 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      512 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1549 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      812 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/
+-rwxr-xr-x   0 root         (0) root         (0)       95 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      780 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/contribution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      533 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/property.py
+-rwxr-xr-x   0 root         (0) root         (0)      621 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/tag.py
+-rwxr-xr-x   0 root         (0) root         (0)      638 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/person.py
+-rwxr-xr-x   0 root         (0) root         (0)      607 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/publisher.py
+-rwxr-xr-x   0 root         (0) root         (0)      871 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/review.py
+-rwxr-xr-x   0 root         (0) root         (0)      595 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/studio.py
+-rwxr-xr-x   0 root         (0) root         (0)      610 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/system.py
+-rwxr-xr-x   0 root         (0) root         (0)      773 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/utils/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3078 2022-03-10 04:24:51.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/utils/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6502 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3326 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-03-10 04:24:53.000000 sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/top_level.txt
```

### Comparing `sweetrpg-library-objects-0.0.85/LICENSE` & `sweetrpg-library-objects-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/PKG-INFO` & `sweetrpg-library-objects-0.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-library-objects
-Version: 0.0.85
+Version: 0.0.86
 Summary: UNKNOWN
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/library-objects
 Platform: UNKNOWN
```

### Comparing `sweetrpg-library-objects-0.0.85/README.md` & `sweetrpg-library-objects-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/setup.cfg` & `sweetrpg-library-objects-0.0.86/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/contribution/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/contribution/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/person/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/person/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/publisher/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/publisher/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/review/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/review/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/studio/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/studio/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/system/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/system/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/api/volume/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/api/volume/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/contribution/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/contribution/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/person/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/person/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/publisher/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/publisher/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/review/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/review/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/studio/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/studio/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/system/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/system/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/document.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/db/volume/schema.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/db/volume/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/contribution.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/contribution.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/property.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/property.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/embedded/tag.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/embedded/tag.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/person.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/person.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/publisher.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/publisher.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/review.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/review.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/studio.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/studio.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/system.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/system.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/model/volume.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/model/volume.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects/utils/user.py` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects/utils/user.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/PKG-INFO` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-library-objects
-Version: 0.0.85
+Version: 0.0.86
 Summary: UNKNOWN
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/library-objects
 Platform: UNKNOWN
```

### Comparing `sweetrpg-library-objects-0.0.85/src/sweetrpg_library_objects.egg-info/SOURCES.txt` & `sweetrpg-library-objects-0.0.86/src/sweetrpg_library_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

