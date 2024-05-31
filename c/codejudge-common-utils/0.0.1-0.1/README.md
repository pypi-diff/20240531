# Comparing `tmp/codejudge-common-utils-0.0.1.tar.gz` & `tmp/codejudge_common_utils-0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codejudge-common-utils-0.0.1.tar", last modified: Fri May 31 09:00:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

