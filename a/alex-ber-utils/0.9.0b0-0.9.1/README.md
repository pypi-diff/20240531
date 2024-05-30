# Comparing `tmp/alex_ber_utils-0.9.0b0.tar.gz` & `tmp/alex_ber_utils-0.9.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.9.0b0.tar", last modified: Thu May 30 17:53:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

