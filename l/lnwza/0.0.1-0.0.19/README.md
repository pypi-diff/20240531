# Comparing `tmp/lnwza-0.0.1.tar.gz` & `tmp/lnwza-0.0.19-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnwza-0.0.1.tar", last modified: Sun May 26 08:00:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

