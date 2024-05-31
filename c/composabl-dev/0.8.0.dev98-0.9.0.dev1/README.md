# Comparing `tmp/composabl_dev-0.8.0.dev98-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/composabl_dev-0.9.0.dev1-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 106018 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 19:11 composabl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 19:11 composabl_dev.libs/
--rw-r--r--  2.0 unx      225 b- defN 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/top_level.txt
--rw-r--r--  2.0 unx       56 b- defN 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx      777 b- defN 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/RECORD
--rw-r--r--  2.0 unx     1829 b- defN 24-May-26 19:11 composabl_dev-0.8.0.dev98.dist-info/METADATA
--rwxr-xr-x  2.0 unx    93456 b- defN 24-May-26 19:11 composabl/ray.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    94456 b- defN 24-May-26 19:11 composabl/__init__.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    93456 b- defN 24-May-26 19:11 composabl/core.cpython-311-x86_64-linux-gnu.so
-11 files, 284265 bytes uncompressed, 104292 bytes compressed:  63.3%
+Zip file size: 25519 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      742 b- defN 24-May-31 12:56 composabl_dev-0.9.0.dev1.dist-info/RECORD
+-rw-r--r--  2.0 unx      111 b- defN 24-May-31 12:56 composabl_dev-0.9.0.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-May-31 12:56 composabl_dev-0.9.0.dev1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-31 12:56 composabl_dev-0.9.0.dev1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1832 b- defN 24-May-31 12:56 composabl_dev-0.9.0.dev1.dist-info/METADATA
+-rwxr-xr-x  2.0 unx    39432 b- defN 24-May-31 12:56 composabl/__init__.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    39232 b- defN 24-May-31 12:56 composabl/ray.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    39240 b- defN 24-May-31 12:56 composabl/core.cpython-310-darwin.so
+8 files, 120655 bytes uncompressed, 24221 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
-Filename: composabl_dev-0.8.0.dev98.dist-info/
+Filename: composabl_dev-0.9.0.dev1.dist-info/RECORD
 Comment: 
 
-Filename: composabl/
+Filename: composabl_dev-0.9.0.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: composabl_dev.libs/
+Filename: composabl_dev-0.9.0.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev98.dist-info/WHEEL
+Filename: composabl_dev-0.9.0.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev98.dist-info/top_level.txt
+Filename: composabl_dev-0.9.0.dev1.dist-info/METADATA
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev98.dist-info/entry_points.txt
+Filename: composabl/__init__.cpython-310-darwin.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev98.dist-info/RECORD
+Filename: composabl/ray.cpython-310-darwin.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev98.dist-info/METADATA
-Comment: 
-
-Filename: composabl/ray.cpython-311-x86_64-linux-gnu.so
-Comment: 
-
-Filename: composabl/__init__.cpython-311-x86_64-linux-gnu.so
-Comment: 
-
-Filename: composabl/core.cpython-311-x86_64-linux-gnu.so
+Filename: composabl/core.cpython-310-darwin.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `composabl_dev-0.8.0.dev98.dist-info/METADATA` & `composabl_dev-0.9.0.dev1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: composabl-dev
-Version: 0.8.0.dev98
+Version: 0.9.0.dev1
 Summary: a distributed trainer to be able to train agents across a cluster of machines
 Author-email: Xavier Geerinck <xavier@composabl.io>, Hunter Park <hunter@composabl.io>
-Requires-Python: >=3.10
+Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown
-Requires-Dist: composabl-core-dev >=0.8.0.dev98
-Requires-Dist: composabl-train-dev >=0.8.0.dev98
-Requires-Dist: composabl-cli-dev >=0.8.0.dev98
+Requires-Dist: composabl-core-dev >=0.9.0.dev1
+Requires-Dist: composabl-train-dev >=0.9.0.dev1
+Requires-Dist: composabl-cli-dev >=0.9.0.dev1
 
 # Composabl
 
 Composabl helps you build Autonomous Agents! Through an easy SDK you get access to outscaled simulator training tools.
 
 ## Licenses / Seats
```

