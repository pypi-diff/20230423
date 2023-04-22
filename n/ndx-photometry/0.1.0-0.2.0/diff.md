# Comparing `tmp/ndx-photometry-0.1.0.tar.gz` & `tmp/ndx_photometry-0.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx-photometry-0.1.0.tar", last modified: Mon Sep 12 14:21:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

