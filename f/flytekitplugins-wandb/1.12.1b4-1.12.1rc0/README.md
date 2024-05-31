# Comparing `tmp/flytekitplugins_wandb-1.12.1b4.tar.gz` & `tmp/flytekitplugins_wandb-1.12.1rc0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_wandb-1.12.1b4.tar", last modified: Tue May 28 15:50:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

