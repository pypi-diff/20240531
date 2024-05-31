# Comparing `tmp/quickstats-0.7.0.4.2.tar.gz` & `tmp/quickstats-0.7.0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.4.2.tar", last modified: Tue May 28 16:18:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

