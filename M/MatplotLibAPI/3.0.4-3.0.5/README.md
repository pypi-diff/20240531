# Comparing `tmp/matplotlibapi-3.0.4.tar.gz` & `tmp/MatplotLibAPI-3.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlibapi-3.0.4.tar", last modified: Wed May 29 13:53:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

