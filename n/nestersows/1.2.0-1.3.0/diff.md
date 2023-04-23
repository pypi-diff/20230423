# Comparing `tmp/nestersows-1.2.0.tar.gz` & `tmp/nestersows-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestersows-1.2.0.tar", last modified: Sun Apr 23 06:23:06 2023, max compression
+gzip compressed data, was "nestersows-1.3.0.tar", last modified: Sun Apr 23 06:32:50 2023, max compression
```

## Comparing `nestersows-1.2.0.tar` & `nestersows-1.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 06:23:06.086317 nestersows-1.2.0/
--rw-rw-rw-   0        0        0      249 2023-04-23 06:23:06.086317 nestersows-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-23 05:42:36.384980 nestersows-1.2.0/nestersows.py
--rw-rw-rw-   0        0        0      297 2023-04-23 06:22:58.944075 nestersows-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:32:50.926497 nestersows-1.3.0/
+-rw-rw-rw-   0        0        0      249 2023-04-23 06:32:50.926497 nestersows-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-23 06:32:05.052262 nestersows-1.3.0/nestersows.py
+-rw-rw-rw-   0        0        0      297 2023-04-23 06:32:18.065443 nestersows-1.3.0/setup.py
```

