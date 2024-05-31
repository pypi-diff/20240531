# Comparing `tmp/QuantumRingsLib-0.4.0-cp311-cp311-win_amd64.whl.zip` & `tmp/QuantumRingsLib-0.5.1-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1069203 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  2624000 b- defN 24-Apr-22 05:32 QuantumRingsLib.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat    11097 b- defN 24-Apr-22 06:55 QuantumRingsLib-0.4.0.dist-info/LICENSE.rst
--rw-rw-rw-  2.0 fat    20660 b- defN 24-Apr-22 06:55 QuantumRingsLib-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 24-Apr-22 06:55 QuantumRingsLib-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 24-Apr-22 06:55 QuantumRingsLib-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 24-Apr-22 06:55 QuantumRingsLib-0.4.0.dist-info/RECORD
-6 files, 2656403 bytes uncompressed, 1068249 bytes compressed:  59.8%
+Zip file size: 1322583 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat  3282432 b- defN 24-May-31 17:50 QuantumRingsLib.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    11097 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/LICENSE.rst
+-rw-rw-rw-  2.0 fat    20473 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/RECORD
+6 files, 3314648 bytes uncompressed, 1321629 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: QuantumRingsLib.cp311-win_amd64.pyd
 Comment: 
 
-Filename: QuantumRingsLib-0.4.0.dist-info/LICENSE.rst
+Filename: QuantumRingsLib-0.5.1.dist-info/LICENSE.rst
 Comment: 
 
-Filename: QuantumRingsLib-0.4.0.dist-info/METADATA
+Filename: QuantumRingsLib-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: QuantumRingsLib-0.4.0.dist-info/WHEEL
+Filename: QuantumRingsLib-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: QuantumRingsLib-0.4.0.dist-info/top_level.txt
+Filename: QuantumRingsLib-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: QuantumRingsLib-0.4.0.dist-info/RECORD
+Filename: QuantumRingsLib-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `QuantumRingsLib-0.4.0.dist-info/LICENSE.rst` & `QuantumRingsLib-0.5.1.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `QuantumRingsLib-0.4.0.dist-info/METADATA` & `QuantumRingsLib-0.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumRingsLib
-Version: 0.4.0
+Version: 0.5.1
 Summary: A Quantum Development Library
 Author-email: "Quantum Rings Inc." <contact@quantumrings.com>
 License: 
         ====================
         EVALUATION AGREEMENT
         ====================
         
@@ -352,15 +352,8 @@
 
     # Execute the circuit
     job = backend.run(qc, shots)
     job.wait_for_final_state(0, 5, jobCallback)
     counts = job.result().get_counts() 
 
 
-==========================
-Version 0.4.0 Known Issues
-==========================
-
-
-* qasm2 importer does not process include statements. This will be updated in a future release.
-
```

