# Comparing `tmp/google_re2-1.1.20240501.tar.gz` & `tmp/google_re2-1.1.20240601-1-cp311-cp311-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_re2-1.1.20240501.tar", last modified: Tue Apr 30 14:58:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

