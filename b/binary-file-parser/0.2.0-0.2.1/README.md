# Comparing `tmp/binary_file_parser-0.2.0.tar.gz` & `tmp/binary_file_parser-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary_file_parser-0.2.0.tar", last modified: Thu May 16 07:58:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

