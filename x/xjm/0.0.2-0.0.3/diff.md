# Comparing `tmp/xjm-0.0.2.tar.gz` & `tmp/xjm-0.0.3-py3.6.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xjm-0.0.2.tar", last modified: Sun Apr 23 07:41:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

