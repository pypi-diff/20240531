# Comparing `tmp/pgqueuer-0.3.6.tar.gz` & `tmp/PgQueuer-0.4.0b1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.6.tar", last modified: Mon May 20 20:52:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

