# Comparing `tmp/scraibe-0.1.1.tar.gz` & `tmp/scraibe-0.1.1.dev361-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraibe-0.1.1.tar", last modified: Fri Sep 22 18:37:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

