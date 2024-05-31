# Comparing `tmp/lokzzpylib-0.2.dev90.tar.gz` & `tmp/lokzzpylib-0.2.dev92-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.2.dev90.tar", last modified: Wed May 29 13:12:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

