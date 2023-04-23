# Comparing `tmp/AEEGGOOSS-0.1.tar.gz` & `tmp/AEEGGOOSS-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AEEGGOOSS-0.1.tar", last modified: Sun Apr 23 16:51:48 2023, max compression
+gzip compressed data, was "AEEGGOOSS-0.2.tar", last modified: Sun Apr 23 17:10:32 2023, max compression
```

## Comparing `AEEGGOOSS-0.1.tar` & `AEEGGOOSS-0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:51:48.092082 AEEGGOOSS-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-23 16:51:48.089093 AEEGGOOSS-0.1/AEEGGOOSS.egg-info/
--rw-rw-rw-   0        0        0      266 2023-04-23 16:51:47.000000 AEEGGOOSS-0.1/AEEGGOOSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-04-23 16:51:47.000000 AEEGGOOSS-0.1/AEEGGOOSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:51:47.000000 AEEGGOOSS-0.1/AEEGGOOSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:51:47.000000 AEEGGOOSS-0.1/AEEGGOOSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 16:49:43.000000 AEEGGOOSS-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      266 2023-04-23 16:51:48.091085 AEEGGOOSS-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 16:51:48.092082 AEEGGOOSS-0.1/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-04-23 16:51:20.000000 AEEGGOOSS-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:10:32.339331 AEEGGOOSS-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-23 17:10:32.330353 AEEGGOOSS-0.2/AEEGGOOSS.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-04-23 17:10:32.000000 AEEGGOOSS-0.2/AEEGGOOSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-04-23 17:10:32.000000 AEEGGOOSS-0.2/AEEGGOOSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:10:32.000000 AEEGGOOSS-0.2/AEEGGOOSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 17:10:32.000000 AEEGGOOSS-0.2/AEEGGOOSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 16:49:43.000000 AEEGGOOSS-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      266 2023-04-23 17:10:32.335341 AEEGGOOSS-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 17:10:32.333349 AEEGGOOSS-0.2/code/
+-rw-rw-rw-   0        0        0       67 2023-04-23 16:49:18.000000 AEEGGOOSS-0.2/code/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:10:32.339331 AEEGGOOSS-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      363 2023-04-23 17:10:28.000000 AEEGGOOSS-0.2/setup.py
```

