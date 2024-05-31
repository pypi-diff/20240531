# Comparing `tmp/fish_simulator-0.1.4.tar.gz` & `tmp/fish_simulator-0.1.4b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_simulator-0.1.4.tar", last modified: Thu May 30 22:36:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

