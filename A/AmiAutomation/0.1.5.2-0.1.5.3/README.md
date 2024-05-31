# Comparing `tmp/AmiAutomation-0.1.5.2.tar.gz` & `tmp/AmiAutomation-0.1.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AmiAutomation-0.1.5.2.tar", last modified: Wed Nov 29 17:12:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

