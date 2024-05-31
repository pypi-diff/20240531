# Comparing `tmp/pulumi_ns1-3.3.0a1716962249.tar.gz` & `tmp/pulumi_ns1-3.3.0a1717135393-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.3.0a1716962249.tar", last modified: Wed May 29 06:01:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

