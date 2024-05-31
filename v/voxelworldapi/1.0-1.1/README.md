# Comparing `tmp/voxelworldapi-1.0.tar.gz` & `tmp/voxelworldapi-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelworldapi-1.0.tar", last modified: Fri May 31 08:11:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

