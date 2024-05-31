# Comparing `tmp/scanvulnpy-0.2.0-py3-none-any.whl.zip` & `tmp/scanvulnpy-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20433 bytes, number of entries: 14
+Zip file size: 20431 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-03 23:37 scanvulnpy/__init__.py
 -rw-rw-rw-  2.0 fat     4140 b- defN 24-Apr-09 13:41 scanvulnpy/__main__.py
--rw-rw-rw-  2.0 fat     1078 b- defN 24-Apr-09 13:41 scanvulnpy/__version__.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-May-31 19:51 scanvulnpy/__version__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-11 14:38 scanvulnpy/modules/__init__.py
 -rw-rw-rw-  2.0 fat     2170 b- defN 24-Mar-20 13:36 scanvulnpy/modules/banners.py
 -rw-rw-rw-  2.0 fat     1706 b- defN 24-Mar-22 09:39 scanvulnpy/modules/cmd.py
--rw-rw-rw-  2.0 fat     2693 b- defN 24-Mar-22 09:39 scanvulnpy/modules/loggers.py
--rw-rw-rw-  2.0 fat     9230 b- defN 24-Apr-09 13:41 scanvulnpy/modules/scanner.py
--rw-rw-rw-  2.0 fat     3899 b- defN 24-Apr-09 13:41 scanvulnpy/modules/utils.py
--rw-rw-rw-  2.0 fat    11545 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17241 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1148 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/RECORD
-14 files, 54953 bytes uncompressed, 18523 bytes compressed:  66.3%
+-rw-rw-rw-  2.0 fat     2693 b- defN 24-May-31 19:50 scanvulnpy/modules/loggers.py
+-rw-rw-rw-  2.0 fat     9230 b- defN 24-May-31 19:50 scanvulnpy/modules/scanner.py
+-rw-rw-rw-  2.0 fat     3899 b- defN 24-May-31 19:50 scanvulnpy/modules/utils.py
+-rw-rw-rw-  2.0 fat    11545 b- defN 24-May-31 19:59 scanvulnpy-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17241 b- defN 24-May-31 19:59 scanvulnpy-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 19:59 scanvulnpy-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-31 19:59 scanvulnpy-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1148 b- defN 24-May-31 19:59 scanvulnpy-0.2.1.dist-info/RECORD
+14 files, 54953 bytes uncompressed, 18521 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: scanvulnpy/modules/scanner.py
 Comment: 
 
 Filename: scanvulnpy/modules/utils.py
 Comment: 
 
-Filename: scanvulnpy-0.2.0.dist-info/LICENSE
+Filename: scanvulnpy-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: scanvulnpy-0.2.0.dist-info/METADATA
+Filename: scanvulnpy-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: scanvulnpy-0.2.0.dist-info/WHEEL
+Filename: scanvulnpy-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: scanvulnpy-0.2.0.dist-info/top_level.txt
+Filename: scanvulnpy-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: scanvulnpy-0.2.0.dist-info/RECORD
+Filename: scanvulnpy-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scanvulnpy/__version__.py

```diff
@@ -15,12 +15,12 @@
 # limitations under the License.
 #
 
 """ scanvulnpy - A simple Package Python to scan vulnerability PyPI Packages"""
 
 __title__ = "scanvulnpy"
 __description__ = "A simple scan vulnerability PyPI Packages, the data provided by https://osv.dev"
-__version__ = "0.2.0"  # 0.1.0.dev1 | 0.1.0a1 | 0.1.0.b1 | 0.1.0rc | 0.1.0
+__version__ = "0.2.1"  # 0.1.0.dev1 | 0.1.0a1 | 0.1.0.b1 | 0.1.0rc | 0.1.0
 __author__ = "little-scripts developers"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright little-scripts"
 __uri__ = "https://github.com/little-scripts/scanvulnpy"
```

## Comparing `scanvulnpy-0.2.0.dist-info/LICENSE` & `scanvulnpy-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scanvulnpy-0.2.0.dist-info/METADATA` & `scanvulnpy-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanvulnpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple Package Python to scan vulnerability PyPI Packages, the data provided by https://osv.dev.
 Author-email: little-scripts <jgdevrennes@gmail.com>
 Maintainer-email: little-scripts <jgdevrennes@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `scanvulnpy-0.2.0.dist-info/RECORD` & `scanvulnpy-0.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 scanvulnpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scanvulnpy/__main__.py,sha256=VMIXnCHE4oGCQ7kDFEajb6tV2zsSx7y2myRbvOwQOys,4140
-scanvulnpy/__version__.py,sha256=j5kHicnl2ZMgUbu9-KZG5nY2PY2wO67VbCmICuAjkJ0,1078
+scanvulnpy/__version__.py,sha256=9M_2AqHkP5UDLHGfyAY0aJGz_HdtxokOtVquE9BuYSE,1078
 scanvulnpy/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scanvulnpy/modules/banners.py,sha256=j279WcbW-05_e4mdV6DC-F-uEmGTncQ4hh0lNu2sty0,2170
 scanvulnpy/modules/cmd.py,sha256=rwDRlyBzb7FNkn-UT1Vf0imrhKNO19pygAcqfKde9PA,1706
 scanvulnpy/modules/loggers.py,sha256=uhGyGBBe2h_BzxXaNZDxEDN8VSilbvYkWRoU9RbOfwY,2693
 scanvulnpy/modules/scanner.py,sha256=UXDEDcshDJrUTw2JlysMHup9SBrPi5H4SF5QNYho-LI,9230
 scanvulnpy/modules/utils.py,sha256=JNBbC-_T2h8i8Sm7N9fyy7ThdgoZIM3V5dZeAlpYitI,3899
-scanvulnpy-0.2.0.dist-info/LICENSE,sha256=O-phqS7heXdql5KGdAaLCVhdAOq9NIbrfkpXSHeikFw,11545
-scanvulnpy-0.2.0.dist-info/METADATA,sha256=FtsFS7I8asEFWwPeYGBH24NSAiwq5dk582RucxItrqk,17241
-scanvulnpy-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-scanvulnpy-0.2.0.dist-info/top_level.txt,sha256=gn9Ja-bTxrMpkcrQCfLMNq5-10N3hIO1IoAL-jEO5Sg,11
-scanvulnpy-0.2.0.dist-info/RECORD,,
+scanvulnpy-0.2.1.dist-info/LICENSE,sha256=O-phqS7heXdql5KGdAaLCVhdAOq9NIbrfkpXSHeikFw,11545
+scanvulnpy-0.2.1.dist-info/METADATA,sha256=ST3QJbG7go5-ZJUnPx8VMXCsqli6D-_ETd3e4p0w6Qg,17241
+scanvulnpy-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+scanvulnpy-0.2.1.dist-info/top_level.txt,sha256=gn9Ja-bTxrMpkcrQCfLMNq5-10N3hIO1IoAL-jEO5Sg,11
+scanvulnpy-0.2.1.dist-info/RECORD,,
```

