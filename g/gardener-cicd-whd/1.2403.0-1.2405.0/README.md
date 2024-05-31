# Comparing `tmp/gardener_cicd_whd-1.2403.0.tar.gz` & `tmp/gardener_cicd_whd-1.2405.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_whd-1.2403.0.tar", last modified: Wed May 29 10:55:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

