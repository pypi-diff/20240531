# Comparing `tmp/gardener_cicd_cli-1.2405.0.tar.gz` & `tmp/gardener_cicd_cli-1.2406.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_cli-1.2405.0.tar", last modified: Fri May 31 07:19:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
