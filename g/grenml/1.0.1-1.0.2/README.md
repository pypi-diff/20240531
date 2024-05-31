# Comparing `tmp/grenml-1.0.1-py3-none-any.whl.zip` & `tmp/grenml-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 43745 bytes, number of entries: 29
--rw-r--r--  2.0 unx       58 b- defN 24-May-30 16:23 grenml/__init__.py
+Zip file size: 43747 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       58 b- defN 24-May-31 14:27 grenml/__init__.py
 -rw-r--r--  2.0 unx     2431 b- defN 24-May-29 17:25 grenml/exceptions.py
 -rw-r--r--  2.0 unx     8667 b- defN 24-May-29 17:25 grenml/managers.py
 -rw-r--r--  2.0 unx     2520 b- defN 24-May-29 17:25 grenml/parse.py
 -rw-r--r--  2.0 unx     1265 b- defN 24-May-29 17:25 grenml/write.py
 -rw-r--r--  2.0 unx       61 b- defN 24-May-17 14:28 grenml/excel_converter/__init__.py
 -rw-r--r--  2.0 unx    26010 b- defN 24-May-29 17:25 grenml/excel_converter/convert_excel_to_xml.py
 -rw-r--r--  2.0 unx       96 b- defN 22-Nov-08 21:00 grenml/models/__init__.py
@@ -19,13 +19,13 @@
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-19 14:57 grenml/schemas/__init__.py
 -rw-r--r--  2.0 unx     5232 b- defN 24-May-29 17:25 grenml/schemas/grenml.xsd
 -rw-r--r--  2.0 unx    21612 b- defN 24-Jan-19 14:57 grenml/schemas/nmlbase.xsd
 -rw-r--r--  2.0 unx       41 b- defN 22-Nov-08 21:00 grenml/validation/__init__.py
 -rw-r--r--  2.0 unx    18618 b- defN 24-May-29 17:25 grenml/validation/validator.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-08 21:00 grenml/writing/__init__.py
 -rw-r--r--  2.0 unx     7035 b- defN 24-May-29 17:25 grenml/writing/grenml.py
--rw-r--r--  2.0 unx    10762 b- defN 24-May-30 16:23 grenml-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13119 b- defN 24-May-30 16:23 grenml-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 16:23 grenml-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-30 16:23 grenml-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2341 b- defN 24-May-30 16:23 grenml-1.0.1.dist-info/RECORD
-29 files, 165601 bytes uncompressed, 40007 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx    10762 b- defN 24-May-31 14:28 grenml-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13119 b- defN 24-May-31 14:28 grenml-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 14:28 grenml-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-31 14:28 grenml-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2341 b- defN 24-May-31 14:28 grenml-1.0.2.dist-info/RECORD
+29 files, 165601 bytes uncompressed, 40009 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: grenml/writing/__init__.py
 Comment: 
 
 Filename: grenml/writing/grenml.py
 Comment: 
 
-Filename: grenml-1.0.1.dist-info/LICENSE
+Filename: grenml-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: grenml-1.0.1.dist-info/METADATA
+Filename: grenml-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: grenml-1.0.1.dist-info/WHEEL
+Filename: grenml-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: grenml-1.0.1.dist-info/top_level.txt
+Filename: grenml-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: grenml-1.0.1.dist-info/RECORD
+Filename: grenml-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grenml/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .managers import GRENMLManager
-__version__ = '1.0.1'
+__version__ = '1.0.2'
```

## Comparing `grenml-1.0.1.dist-info/LICENSE` & `grenml-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `grenml-1.0.1.dist-info/METADATA` & `grenml-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grenml
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for creating, parsing, and storing GRENML
 Home-page: https://github.com/grenmap/grenml
 Author: GREN Map Working Group
 License: Apache Software License
 Keywords: global,network,markup,language,gren,national,research,education,regional,institution,nren
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `grenml-1.0.1.dist-info/RECORD` & `grenml-1.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-grenml/__init__.py,sha256=VzCuOzkw1IlRu0eZHcP7ZzAalVURLxf16BuQ7LSq4EU,58
+grenml/__init__.py,sha256=DxoM-vN4V6TG4i-6xHMSCNJXgbAR8iSBJeKVp1kW09A,58
 grenml/exceptions.py,sha256=ymhEerjFUGAroBA3xy9DBqCP60-DLLNMBoNg9J_ZivA,2431
 grenml/managers.py,sha256=SsKkeibtw90cSak-TaOJ3CqA01ucjznLKnEu-6XCjqc,8667
 grenml/parse.py,sha256=Q5i_9o-_0KW2wvVPQrd0BXLgW0cq6LdMHpMeIxj6hKw,2520
 grenml/write.py,sha256=oy-JiSQ6UH6pRZ2siI9Y7ep6-8CW9S-kOBc31f1y2VQ,1265
 grenml/excel_converter/__init__.py,sha256=hhHP3uEkRjkTjCmz9Hfx23ZXp3M041WC6LRF0W8sq3s,61
 grenml/excel_converter/convert_excel_to_xml.py,sha256=sW0m-9mY96NyyF_ym4orIpFmcIEeDeAcjDdoKdlcGNw,26010
 grenml/models/__init__.py,sha256=MKFIiOEb3QltupB32HhYz99Cj2pQcss67q2TgUWyIzg,96
@@ -18,12 +18,12 @@
 grenml/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 grenml/schemas/grenml.xsd,sha256=bW86HhnOYwHlWDywwlQqhnIaLV7Wv1fDD6KAMIOfZ9Y,5232
 grenml/schemas/nmlbase.xsd,sha256=V84nDWDs8KaaabAg4LU-TeSzO3XwX6lJnhrdbxKTxcY,21612
 grenml/validation/__init__.py,sha256=v8NECCU0zlwDZA3ooqGENMAkRjxx1J21a2j3Fm3FbOs,41
 grenml/validation/validator.py,sha256=I5gv07qt3XpDi7Ph-tgkZRb5KoZrI_Z22XJpNSqeGTk,18618
 grenml/writing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 grenml/writing/grenml.py,sha256=pwGAG9fWOp_-ZFhBCkEyfrAFAfG_XsCgOCFJzw1a468,7035
-grenml-1.0.1.dist-info/LICENSE,sha256=QVN1NqD_Wohwd3pYGr-bL5ZUxMnuAUYZkMvtux_z2Rc,10762
-grenml-1.0.1.dist-info/METADATA,sha256=uTDH_DR8Y431v-CsNfhQxPpSIgLeYrnOaTStAgGzcM4,13119
-grenml-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-grenml-1.0.1.dist-info/top_level.txt,sha256=-JLOqiSBFQef6uuluxYVtDAfLWeivPV7PsWEhzj-o1I,7
-grenml-1.0.1.dist-info/RECORD,,
+grenml-1.0.2.dist-info/LICENSE,sha256=QVN1NqD_Wohwd3pYGr-bL5ZUxMnuAUYZkMvtux_z2Rc,10762
+grenml-1.0.2.dist-info/METADATA,sha256=XVyQHbP0IigVSZw5oBCwBjFDxmTto5FKpRs4tEsQPOY,13119
+grenml-1.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+grenml-1.0.2.dist-info/top_level.txt,sha256=-JLOqiSBFQef6uuluxYVtDAfLWeivPV7PsWEhzj-o1I,7
+grenml-1.0.2.dist-info/RECORD,,
```

