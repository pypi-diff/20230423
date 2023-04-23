# Comparing `tmp/gptrim-0.1.3.tar.gz` & `tmp/gptrim-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptrim-0.1.3.tar", last modified: Fri Apr 21 21:13:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

