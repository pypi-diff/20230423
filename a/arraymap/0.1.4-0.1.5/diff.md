# Comparing `tmp/arraymap-0.1.4.tar.gz` & `tmp/arraymap-0.1.5-cp311-cp311-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.4.tar", last modified: Fri Apr 14 23:33:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

