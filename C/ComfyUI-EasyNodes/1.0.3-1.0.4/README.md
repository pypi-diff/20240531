# Comparing `tmp/comfyui_easynodes-1.0.3.tar.gz` & `tmp/ComfyUI_EasyNodes-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfyui_easynodes-1.0.3.tar", last modified: Fri May 31 03:01:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

