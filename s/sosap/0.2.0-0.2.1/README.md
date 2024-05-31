# Comparing `tmp/sosap-0.2.0.tar.gz` & `tmp/sosap-0.2.1-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosap-0.2.0.tar", last modified: Thu May 23 03:55:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

