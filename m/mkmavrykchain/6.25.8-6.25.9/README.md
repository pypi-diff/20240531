# Comparing `tmp/mkmavrykchain-6.25.8-py3-none-any.whl.zip` & `tmp/mkmavrykchain-6.25.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9480 bytes, number of entries: 9
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-23 12:42 mavrykchain/_version.py
--rw-r--r--  2.0 unx     1918 b- defN 24-Apr-23 12:42 mavrykchain/keys.py
--rw-r--r--  2.0 unx    12385 b- defN 24-Apr-23 12:42 mavrykchain/mkmavrykchain.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Apr-23 12:42 mavrykchain/parameters.yaml
--rw-r--r--  2.0 unx     5167 b- defN 24-Apr-23 12:42 mkmavrykchain-6.25.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 12:42 mkmavrykchain-6.25.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-23 12:42 mkmavrykchain-6.25.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-23 12:42 mkmavrykchain-6.25.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      753 b- defN 24-Apr-23 12:42 mkmavrykchain-6.25.8.dist-info/RECORD
-9 files, 23471 bytes uncompressed, 8174 bytes compressed:  65.2%
+Zip file size: 9477 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      498 b- defN 24-May-14 09:40 mavrykchain/_version.py
+-rw-r--r--  2.0 unx     1918 b- defN 24-May-14 09:40 mavrykchain/keys.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-14 09:40 mavrykchain/mkmavrykchain.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-May-14 09:40 mavrykchain/parameters.yaml
+-rw-r--r--  2.0 unx     5167 b- defN 24-May-14 09:40 mkmavrykchain-6.25.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:40 mkmavrykchain-6.25.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-May-14 09:40 mkmavrykchain-6.25.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-14 09:40 mkmavrykchain-6.25.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-May-14 09:40 mkmavrykchain-6.25.9.dist-info/RECORD
+9 files, 23471 bytes uncompressed, 8171 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mavrykchain/mkmavrykchain.py
 Comment: 
 
 Filename: mavrykchain/parameters.yaml
 Comment: 
 
-Filename: mkmavrykchain-6.25.8.dist-info/METADATA
+Filename: mkmavrykchain-6.25.9.dist-info/METADATA
 Comment: 
 
-Filename: mkmavrykchain-6.25.8.dist-info/WHEEL
+Filename: mkmavrykchain-6.25.9.dist-info/WHEEL
 Comment: 
 
-Filename: mkmavrykchain-6.25.8.dist-info/entry_points.txt
+Filename: mkmavrykchain-6.25.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.8.dist-info/top_level.txt
+Filename: mkmavrykchain-6.25.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.8.dist-info/RECORD
+Filename: mkmavrykchain-6.25.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mavrykchain/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-23T14:41:02+0200",
+ "date": "2024-05-14T11:35:56+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "e73e0d6c38c816e298286c99a780f6b0bc92a773",
- "version": "6.25.8"
+ "full-revisionid": "605cb0ee2d1580c6f469990666adfb0c45967a2d",
+ "version": "6.25.9"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `mkmavrykchain-6.25.8.dist-info/METADATA` & `mkmavrykchain-6.25.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkmavrykchain
-Version: 6.25.8
+Version: 6.25.9
 Summary: A utility to generate k8s configs for a Mavryk blockchain
 Home-page: https://github.com/mavryk-network/mavryk-k8s
 Author: MavrykDynamics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `mkmavrykchain-6.25.8.dist-info/RECORD` & `mkmavrykchain-6.25.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-mavrykchain/_version.py,sha256=6Q2QzlfjkN9oxIq8zrjDpts0W1K-qxfo1uFHmShX9Dk,498
+mavrykchain/_version.py,sha256=DzgEemW64GZ_m8tVTzkrwtKLdAXj5r_WBycQQeyq51E,498
 mavrykchain/keys.py,sha256=Rd9TwFb5uFPhfktW16YhpT7Nt0h0ycAuvxugNr2egF0,1918
 mavrykchain/mkmavrykchain.py,sha256=fMcH9CK4kYpOjCsrIWd5EZmaD49bw8pNULGGEL_yqVI,12385
 mavrykchain/parameters.yaml,sha256=7bLg5OtDeWjgTTijnNir2V-nGyFC2aaLJQpQCIRgK90,2580
-mkmavrykchain-6.25.8.dist-info/METADATA,sha256=ETvWzhwYKJTF9HjPUcokDfdZyObRKWq9I6d7TeOrRuo,5167
-mkmavrykchain-6.25.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mkmavrykchain-6.25.8.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
-mkmavrykchain-6.25.8.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
-mkmavrykchain-6.25.8.dist-info/RECORD,,
+mkmavrykchain-6.25.9.dist-info/METADATA,sha256=cbP7sox7eI2OWfqLrYxHvNONP6TBWcVVpA4dzOjIHeQ,5167
+mkmavrykchain-6.25.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mkmavrykchain-6.25.9.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
+mkmavrykchain-6.25.9.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
+mkmavrykchain-6.25.9.dist-info/RECORD,,
```

