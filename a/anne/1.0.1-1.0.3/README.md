# Comparing `tmp/anne-1.0.1.tar.gz` & `tmp/anne-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.0.1.tar", last modified: Fri May 31 00:29:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

