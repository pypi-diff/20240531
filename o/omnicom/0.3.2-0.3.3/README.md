# Comparing `tmp/omnicom-0.3.2-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/omnicom-0.3.3-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 97490 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   208896 b- defN 24-May-31 07:24 omnicom.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat      188 b- defN 24-May-31 07:24 omnicom-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-May-31 07:24 omnicom-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-31 07:24 omnicom-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 24-May-31 07:24 omnicom-0.3.2.dist-info/RECORD
-5 files, 209588 bytes uncompressed, 96766 bytes compressed:  53.8%
+Zip file size: 98897 bytes, number of entries: 6
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-31 20:50 omnicom-0.3.3.dist-info/
+-rwxr-xr-x  2.0 unx   307424 b- defN 24-May-31 20:50 omnicom.pypy39-pp73-darwin.so
+-rw-rw-r--  2.0 unx      390 b- defN 24-May-31 20:50 omnicom-0.3.3.dist-info/RECORD
+-rw-r--r--  2.0 unx      115 b- defN 24-May-31 20:50 omnicom-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-31 20:50 omnicom-0.3.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      181 b- defN 24-May-31 20:50 omnicom-0.3.3.dist-info/METADATA
+6 files, 308118 bytes uncompressed, 98057 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: omnicom.pypy39-pp73-win_amd64.pyd
+Filename: omnicom-0.3.3.dist-info/
 Comment: 
 
-Filename: omnicom-0.3.2.dist-info/METADATA
+Filename: omnicom.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: omnicom-0.3.2.dist-info/WHEEL
+Filename: omnicom-0.3.3.dist-info/RECORD
 Comment: 
 
-Filename: omnicom-0.3.2.dist-info/top_level.txt
+Filename: omnicom-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: omnicom-0.3.2.dist-info/RECORD
+Filename: omnicom-0.3.3.dist-info/top_level.txt
+Comment: 
+
+Filename: omnicom-0.3.3.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

