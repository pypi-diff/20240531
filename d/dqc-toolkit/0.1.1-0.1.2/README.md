# Comparing `tmp/dqc_toolkit-0.1.1.tar.gz` & `tmp/dqc_toolkit-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc_toolkit-0.1.1.tar", last modified: Thu May  9 15:12:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

