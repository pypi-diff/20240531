# Comparing `tmp/trustregion-1.2.tar.gz` & `tmp/trustregion-1.2.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trustregion-1.2.tar", last modified: Thu Jul  8 03:33:01 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

