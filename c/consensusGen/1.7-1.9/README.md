# Comparing `tmp/consensusgen-1.7.tar.gz` & `tmp/consensusGen-1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.7.tar", last modified: Fri May 31 13:39:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

