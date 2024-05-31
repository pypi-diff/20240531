# Comparing `tmp/shrink_img-0.7.0.tar.gz` & `tmp/shrink_img-0.8.0-cp312-cp312-macosx_10_13_x86_64.macosx_11_0_arm64.macosx_10_13_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

