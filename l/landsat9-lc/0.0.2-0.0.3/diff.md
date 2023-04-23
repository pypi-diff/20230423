# Comparing `tmp/landsat9_lc-0.0.2.tar.gz` & `tmp/landsat9_lc-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\landsat9_lc-0.0.2.tar", last modified: Sun Apr 23 17:19:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

