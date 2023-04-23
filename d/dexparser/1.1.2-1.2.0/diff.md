# Comparing `tmp/dexparser-1.1.2.tar.gz` & `tmp/dexparser-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexparser-1.1.2.tar", last modified: Wed Mar 15 11:56:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

