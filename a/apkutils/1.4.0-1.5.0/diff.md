# Comparing `tmp/apkutils-1.4.0.tar.gz` & `tmp/apkutils-1.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkutils-1.4.0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

