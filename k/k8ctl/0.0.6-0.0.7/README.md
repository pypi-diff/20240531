# Comparing `tmp/k8ctl-0.0.6-py3-none-any.whl.zip` & `tmp/k8ctl-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9482 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 11:40 k8ctl/__init__.py
--rw-r--r--  2.0 unx    16635 b- defN 24-May-30 11:40 k8ctl/k8ctl.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1481 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 24-May-30 11:41 k8ctl-0.0.6.dist-info/RECORD
-8 files, 30227 bytes uncompressed, 8416 bytes compressed:  72.2%
+Zip file size: 9385 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 12:19 k8ctl/__init__.py
+-rw-r--r--  2.0 unx    16623 b- defN 24-May-30 12:19 k8ctl/k8ctl.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/RECORD
+8 files, 29854 bytes uncompressed, 8319 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: k8ctl/__init__.py
 Comment: 
 
 Filename: k8ctl/k8ctl.py
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/LICENSE
+Filename: k8ctl-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/METADATA
+Filename: k8ctl-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/WHEEL
+Filename: k8ctl-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/entry_points.txt
+Filename: k8ctl-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/top_level.txt
+Filename: k8ctl-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: k8ctl-0.0.6.dist-info/RECORD
+Filename: k8ctl-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8ctl/k8ctl.py

```diff
@@ -55,15 +55,15 @@
 ## Program starts here
 
 @click.group()
 def k8ctl():
     '''
     k8ctl is a command line tool for managing rancher multicluster kubernetes environments
     '''
-    print("calling")
+    pass
 
 @k8ctl.group()
 def cluster():
     '''
     Switch, list and get the current cluster
     '''
     pass
```

## Comparing `k8ctl-0.0.6.dist-info/LICENSE` & `k8ctl-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `k8ctl-0.0.6.dist-info/METADATA` & `k8ctl-0.0.7.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8ctl
-Version: 0.0.6
+Version: 0.0.7
 Author: Kishorekarthik P
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 
 # k8ctl
 
@@ -25,23 +25,14 @@
 - `k8ctl`: Main command line tool.
 - `cluster`: Switch, list and get the current cluster.
 - `env`: Create, list and delete environment variables of an application.
 - `list`: List applications, web, timers, workers.
 - `console`: Connect to the application with railsconsole, psql, bash.
 - `restart`: Restart the applications, web, timers, workers.
 - `login`: Login to a cluster.
-- `get_logs`: Get the logs of the application.
-- `current_cluster`: Show the current cluster.
-- `list_clusters`: List all clusters.
-- `switch_cluster`: Switch to a cluster.
-- `list_env`: List all environment variables.
-- `set_env`: Set environment variables.
-- `list_apps`: List all applications.
-- `list_web`: List all web services.
-- `list_timers`: List all timers.
-- `list_workers`: List all workers.
+- `logs`: Get the logs of the application.
 
 For more detailed usage instructions, you can use the `-h` or `--help` flag with any command.
 
 ## License
 
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
```

## Comparing `k8ctl-0.0.6.dist-info/RECORD` & `k8ctl-0.0.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 k8ctl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-k8ctl/k8ctl.py,sha256=wu-aB-w_E9lcxuieUwG0hBqVxEf0C_R7G9PkGhCwCk4,16635
-k8ctl-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-k8ctl-0.0.6.dist-info/METADATA,sha256=RPmr12B5M1nUnakQj9mGtYI-QeCQ0FaAU54seWOH6hg,1481
-k8ctl-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-k8ctl-0.0.6.dist-info/entry_points.txt,sha256=snE4Lt3gioSbGG7Chpv4NxhrWV_Z8wI7MVBB6zauFGo,44
-k8ctl-0.0.6.dist-info/top_level.txt,sha256=MWKRJ9qlnCPm7r_pIheyUtZ4LqaWZ21y0H-O_NFS3Bw,6
-k8ctl-0.0.6.dist-info/RECORD,,
+k8ctl/k8ctl.py,sha256=xR8J0mzr4dkG4n06vYU9N0oHFZkSgJtBq_rSW6q_69U,16623
+k8ctl-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+k8ctl-0.0.7.dist-info/METADATA,sha256=wqzCMCaGRAD5SKE-AqYJrPWbSXamHDZztXPfd5ZpZrw,1120
+k8ctl-0.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+k8ctl-0.0.7.dist-info/entry_points.txt,sha256=snE4Lt3gioSbGG7Chpv4NxhrWV_Z8wI7MVBB6zauFGo,44
+k8ctl-0.0.7.dist-info/top_level.txt,sha256=MWKRJ9qlnCPm7r_pIheyUtZ4LqaWZ21y0H-O_NFS3Bw,6
+k8ctl-0.0.7.dist-info/RECORD,,
```

