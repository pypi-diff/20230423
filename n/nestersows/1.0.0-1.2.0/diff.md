# Comparing `tmp/nestersows-1.0.0.tar.gz` & `tmp/nestersows-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestersows-1.0.0.tar", last modified: Fri Apr 14 05:56:14 2023, max compression
+gzip compressed data, was "nestersows-1.2.0.tar", last modified: Sun Apr 23 06:23:06 2023, max compression
```

## Comparing `nestersows-1.0.0.tar` & `nestersows-1.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:56:14.045709 nestersows-1.0.0/
--rw-rw-rw-   0        0        0      249 2023-04-14 05:56:14.045709 nestersows-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-10 05:09:06.885226 nestersows-1.0.0/nester.py
--rw-rw-rw-   0        0        0      293 2023-04-14 05:54:25.022140 nestersows-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:23:06.086317 nestersows-1.2.0/
+-rw-rw-rw-   0        0        0      249 2023-04-23 06:23:06.086317 nestersows-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-23 05:42:36.384980 nestersows-1.2.0/nestersows.py
+-rw-rw-rw-   0        0        0      297 2023-04-23 06:22:58.944075 nestersows-1.2.0/setup.py
```

