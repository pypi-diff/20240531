# Comparing `tmp/aily_code_sdk-0.1.0b1.tar.gz` & `tmp/aily_code_sdk-0.1.0b2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk-0.1.0b1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

