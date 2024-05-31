# Comparing `tmp/degann-1.1.4.tar.gz` & `tmp/degann-1.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degann-1.1.4.tar", last modified: Thu May 30 18:26:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

