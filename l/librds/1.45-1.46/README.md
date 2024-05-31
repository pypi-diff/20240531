# Comparing `tmp/librds-1.45.tar.gz` & `tmp/librds-1.46-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.45.tar", last modified: Wed May 29 14:26:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

