# Comparing `tmp/pyCeph-0.4.2.tar.gz` & `tmp/pyCeph-0.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyCeph-0.4.2.tar", last modified: Tue Oct 25 02:18:23 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

