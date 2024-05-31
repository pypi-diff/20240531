# Comparing `tmp/PyDicomGrouping-0.1.7.tar.gz` & `tmp/PyDicomGrouping-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyDicomGrouping-0.1.7.tar", last modified: Thu May 30 06:34:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

