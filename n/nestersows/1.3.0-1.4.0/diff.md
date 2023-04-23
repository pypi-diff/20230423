# Comparing `tmp/nestersows-1.3.0.tar.gz` & `tmp/nestersows-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestersows-1.3.0.tar", last modified: Sun Apr 23 06:32:50 2023, max compression
+gzip compressed data, was "nestersows-1.4.0.tar", last modified: Sun Apr 23 06:48:06 2023, max compression
```

## Comparing `nestersows-1.3.0.tar` & `nestersows-1.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 06:32:50.926497 nestersows-1.3.0/
--rw-rw-rw-   0        0        0      249 2023-04-23 06:32:50.926497 nestersows-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-23 06:32:05.052262 nestersows-1.3.0/nestersows.py
--rw-rw-rw-   0        0        0      297 2023-04-23 06:32:18.065443 nestersows-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:48:06.211219 nestersows-1.4.0/
+-rw-rw-rw-   0        0        0      249 2023-04-23 06:48:06.211219 nestersows-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-04-23 06:47:35.877423 nestersows-1.4.0/nestersows.py
+-rw-rw-rw-   0        0        0      297 2023-04-23 06:47:48.079142 nestersows-1.4.0/setup.py
```

