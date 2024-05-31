# Comparing `tmp/acai_aws-2.2.0.tar.gz` & `tmp/acai_aws-2.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acai_aws-2.2.0.tar", last modified: Wed May 22 18:57:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

