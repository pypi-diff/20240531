# Comparing `tmp/punchboot-2.0.0.tar.gz` & `tmp/punchboot-2.1.0-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punchboot-2.0.0.tar", last modified: Sun Feb 18 20:00:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

