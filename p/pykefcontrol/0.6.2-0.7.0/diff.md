# Comparing `tmp/pykefcontrol-0.6.2.tar.gz` & `tmp/pykefcontrol-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykefcontrol-0.6.2.tar", last modified: Sun Dec 18 11:03:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

