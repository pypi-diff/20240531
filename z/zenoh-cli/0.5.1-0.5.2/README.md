# Comparing `tmp/zenoh_cli-0.5.1-py3-none-any.whl.zip` & `tmp/zenoh_cli-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10281 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13731 b- defN 24-Apr-19 19:31 zenoh_cli.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2282 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      564 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/RECORD
-7 files, 28077 bytes uncompressed, 9281 bytes compressed:  66.9%
+Zip file size: 10287 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13731 b- defN 24-May-31 07:02 zenoh_cli.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2282 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      564 b- defN 24-May-31 07:02 zenoh_cli-0.5.2.dist-info/RECORD
+7 files, 28077 bytes uncompressed, 9287 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: zenoh_cli.py
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/LICENSE
+Filename: zenoh_cli-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/METADATA
+Filename: zenoh_cli-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/WHEEL
+Filename: zenoh_cli-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/entry_points.txt
+Filename: zenoh_cli-0.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/top_level.txt
+Filename: zenoh_cli-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zenoh_cli-0.5.1.dist-info/RECORD
+Filename: zenoh_cli-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zenoh_cli-0.5.1.dist-info/LICENSE` & `zenoh_cli-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zenoh_cli-0.5.1.dist-info/METADATA` & `zenoh_cli-0.5.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zenoh-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: CLI for Zenoh
 Home-page: https://github.com/MO-RISE/zenoh-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eclipse-zenoh ==0.10.1-rc
+Requires-Dist: eclipse-zenoh ==0.11.0rc3
 Requires-Dist: parse
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: jsonpointer
 Requires-Dist: importlib-metadata ; python_version < "3.10"
 
 # zenoh-cli
```

## Comparing `zenoh_cli-0.5.1.dist-info/RECORD` & `zenoh_cli-0.5.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 zenoh_cli.py,sha256=u0i9Q7ryu-6oRFjx_mgzkQ0xiQcGVRpGndT0o94Ezvs,13731
-zenoh_cli-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-zenoh_cli-0.5.1.dist-info/METADATA,sha256=lSr4fJ_ABNlQReRrbdeFQ_2zH5xFmoxxGAoPDKe7dcw,2282
-zenoh_cli-0.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zenoh_cli-0.5.1.dist-info/entry_points.txt,sha256=aJfwoOb7Ak5fcAMmsVTFUKD3NTKV7NqeeTubpzDJ_9U,41
-zenoh_cli-0.5.1.dist-info/top_level.txt,sha256=PGGVngbuVqtbHeVek9BhAjXH9RX1zpSsTAzxcxR9jS0,10
-zenoh_cli-0.5.1.dist-info/RECORD,,
+zenoh_cli-0.5.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+zenoh_cli-0.5.2.dist-info/METADATA,sha256=zKDULG9FHITyjthWcyYC6BSauq2R8qKWpptgIqFW3Lo,2282
+zenoh_cli-0.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zenoh_cli-0.5.2.dist-info/entry_points.txt,sha256=aJfwoOb7Ak5fcAMmsVTFUKD3NTKV7NqeeTubpzDJ_9U,41
+zenoh_cli-0.5.2.dist-info/top_level.txt,sha256=PGGVngbuVqtbHeVek9BhAjXH9RX1zpSsTAzxcxR9jS0,10
+zenoh_cli-0.5.2.dist-info/RECORD,,
```

