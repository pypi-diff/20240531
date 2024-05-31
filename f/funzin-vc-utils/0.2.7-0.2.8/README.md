# Comparing `tmp/funzin_vc_utils-0.2.7-py3-none-any.whl.zip` & `tmp/funzin_vc_utils-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,12 +3,12 @@
 -rwxrwxrwx  2.0 unx     4120 b- defN 23-Jun-22 05:48 fz_capture/fz_capture.py
 -rwxrwxrwx  2.0 unx       24 b- defN 23-Jun-22 05:48 fz_logger/__init__.py
 -rw-rw-r--  2.0 unx     2354 b- defN 24-May-29 05:14 fz_logger/fz_logger.py
 -rwxrwxrwx  2.0 unx       24 b- defN 23-Jun-22 05:48 fz_mlflow/__init__.py
 -rwxrwxrwx  2.0 unx    10430 b- defN 23-Jun-22 05:48 fz_mlflow/fz_mlflow.py
 -rwxrwxrwx  2.0 unx       23 b- defN 23-Jun-22 05:48 fz_wandb/__init__.py
 -rwxrwxrwx  2.0 unx      710 b- defN 23-Jun-22 05:48 fz_wandb/fz_wandb.py
--rw-rw-r--  2.0 unx     5162 b- defN 24-May-29 05:15 funzin_vc_utils-0.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-29 05:15 funzin_vc_utils-0.2.7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       17 b- defN 24-May-29 05:15 funzin_vc_utils-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      950 b- defN 24-May-29 05:15 funzin_vc_utils-0.2.7.dist-info/RECORD
+-rw-rw-r--  2.0 unx     5162 b- defN 24-May-29 05:16 funzin_vc_utils-0.2.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-29 05:16 funzin_vc_utils-0.2.8.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       17 b- defN 24-May-29 05:16 funzin_vc_utils-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      950 b- defN 24-May-29 05:16 funzin_vc_utils-0.2.8.dist-info/RECORD
 12 files, 23931 bytes uncompressed, 7422 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: fz_wandb/__init__.py
 Comment: 
 
 Filename: fz_wandb/fz_wandb.py
 Comment: 
 
-Filename: funzin_vc_utils-0.2.7.dist-info/METADATA
+Filename: funzin_vc_utils-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: funzin_vc_utils-0.2.7.dist-info/WHEEL
+Filename: funzin_vc_utils-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: funzin_vc_utils-0.2.7.dist-info/top_level.txt
+Filename: funzin_vc_utils-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: funzin_vc_utils-0.2.7.dist-info/RECORD
+Filename: funzin_vc_utils-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `funzin_vc_utils-0.2.7.dist-info/METADATA` & `funzin_vc_utils-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funzin-vc-utils
-Version: 0.2.7
+Version: 0.2.8
 Summary: funzin vc solution utils
 Home-page: https://dnchoi.github.io
 Author: dnchoi
 Author-email: luke.dn.choi@funzin.co.kr
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

## Comparing `funzin_vc_utils-0.2.7.dist-info/RECORD` & `funzin_vc_utils-0.2.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 fz_capture/fz_capture.py,sha256=bB3MM80lVZMPRmHr2HyXTwQKONP1ROm6j47dsrLqkVY,4120
 fz_logger/__init__.py,sha256=J1R_O3OAmaj-JCMgAN-YY6VjC-4fmjCvegQJ8CIms3o,24
 fz_logger/fz_logger.py,sha256=ghr8kit3Y4NUyZQozLYuw2uTy_LtylS4KSd_tc2IyKk,2354
 fz_mlflow/__init__.py,sha256=R3V694roln8vm0Bnno0EuzDLwMg3chcPSiPAAhK1JB8,24
 fz_mlflow/fz_mlflow.py,sha256=-GiY_RRBMVvLLtY0Okwa4mUK9kztNMsjJtm1bSDIhCU,10430
 fz_wandb/__init__.py,sha256=_vsaLlPXEb5YihW6a_yFA0uBXg1-0nV-VE85RZiY_Z0,23
 fz_wandb/fz_wandb.py,sha256=-3i6k73ZEbbyAQSthx7GcSdsHkENoFFK3UWB0HQ5y_M,710
-funzin_vc_utils-0.2.7.dist-info/METADATA,sha256=DfpY3KQolkPA8C0bYQCjvTEJrr7Oqj57rzlYl93V7Tk,5162
-funzin_vc_utils-0.2.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-funzin_vc_utils-0.2.7.dist-info/top_level.txt,sha256=LYvYxnJsQuhImtqKwjM7dWvPnIiU4xw1NOTnAWQAIJM,17
-funzin_vc_utils-0.2.7.dist-info/RECORD,,
+funzin_vc_utils-0.2.8.dist-info/METADATA,sha256=p_pb5vBy7vunhXuf5AunSy5QLw9Z8cFwvhkwN0eMLsk,5162
+funzin_vc_utils-0.2.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+funzin_vc_utils-0.2.8.dist-info/top_level.txt,sha256=LYvYxnJsQuhImtqKwjM7dWvPnIiU4xw1NOTnAWQAIJM,17
+funzin_vc_utils-0.2.8.dist-info/RECORD,,
```

