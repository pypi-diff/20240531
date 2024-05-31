# Comparing `tmp/lines_dataset-0.1.4.tar.gz` & `tmp/lines_dataset-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.1.4.tar", last modified: Fri May 31 09:48:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

