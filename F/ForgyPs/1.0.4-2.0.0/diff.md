# Comparing `tmp/ForgyPs-1.0.4.tar.gz` & `tmp/ForgyPs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForgyPs-1.0.4.tar", last modified: Sun Apr 23 18:53:52 2023, max compression
+gzip compressed data, was "ForgyPs-2.0.0.tar", last modified: Sun Apr 23 18:57:53 2023, max compression
```

## Comparing `ForgyPs-1.0.4.tar` & `ForgyPs-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:53:52.926822 ForgyPs-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-23 18:53:52.909818 ForgyPs-1.0.4/ForgyPs/
--rw-rw-rw-   0        0        0   196200 2023-04-23 18:43:04.000000 ForgyPs-1.0.4/ForgyPs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:53:52.925822 ForgyPs-1.0.4/ForgyPs.egg-info/
--rw-rw-rw-   0        0        0      249 2023-04-23 18:53:52.000000 ForgyPs-1.0.4/ForgyPs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-23 18:53:52.000000 ForgyPs-1.0.4/ForgyPs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:53:52.000000 ForgyPs-1.0.4/ForgyPs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 18:53:52.000000 ForgyPs-1.0.4/ForgyPs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 18:53:52.000000 ForgyPs-1.0.4/ForgyPs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      249 2023-04-23 18:53:52.926822 ForgyPs-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-04-04 20:52:05.000000 ForgyPs-1.0.4/README.md
--rw-rw-rw-   0        0        0      415 2023-04-23 18:53:52.928822 ForgyPs-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      299 2023-04-23 18:53:46.000000 ForgyPs-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:57:53.409178 ForgyPs-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-23 18:57:53.389174 ForgyPs-2.0.0/ForgyPs/
+-rw-rw-rw-   0        0        0   296896 2023-04-23 18:56:28.000000 ForgyPs-2.0.0/ForgyPs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:57:53.408177 ForgyPs-2.0.0/ForgyPs.egg-info/
+-rw-rw-rw-   0        0        0      249 2023-04-23 18:57:53.000000 ForgyPs-2.0.0/ForgyPs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-23 18:57:53.000000 ForgyPs-2.0.0/ForgyPs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:57:53.000000 ForgyPs-2.0.0/ForgyPs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-23 18:57:53.000000 ForgyPs-2.0.0/ForgyPs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 18:57:53.000000 ForgyPs-2.0.0/ForgyPs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      249 2023-04-23 18:57:53.409178 ForgyPs-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-04-04 20:52:05.000000 ForgyPs-2.0.0/README.md
+-rw-rw-rw-   0        0        0      415 2023-04-23 18:57:53.411179 ForgyPs-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      332 2023-04-23 18:57:35.000000 ForgyPs-2.0.0/setup.py
```

