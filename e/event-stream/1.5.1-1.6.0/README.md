# Comparing `tmp/event_stream-1.5.1.tar.gz` & `tmp/event_stream-1.6.0-cp311-cp311-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_stream-1.5.1.tar", last modified: Mon Nov  6 02:20:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

