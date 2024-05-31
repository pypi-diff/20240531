# Comparing `tmp/homeassistant_stubs-2024.6.0b1.tar.gz` & `tmp/homeassistant_stubs-2024.6.0b2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant_stubs-2024.6.0b1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

