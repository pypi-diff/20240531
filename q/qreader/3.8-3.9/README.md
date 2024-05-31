# Comparing `tmp/qreader-3.8.tar.gz` & `tmp/qreader-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qreader-3.8.tar", last modified: Sun Sep 10 10:05:21 2023, max compression
+gzip compressed data, was "qreader-3.9.tar", last modified: Fri Sep 15 13:02:21 2023, max compression
```

## Comparing `qreader-3.8.tar` & `qreader-3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-09-10 10:05:21.643119 qreader-3.8/
--rw-rw-rw-   0        0        0     1089 2022-12-03 14:38:15.000000 qreader-3.8/LICENSE
--rw-rw-rw-   0        0        0    12994 2023-09-10 10:05:21.644127 qreader-3.8/PKG-INFO
--rw-rw-rw-   0        0        0    12090 2023-09-08 22:16:09.000000 qreader-3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-09-10 10:05:21.579239 qreader-3.8/documentation/
-drwxrwxrwx   0        0        0        0 2023-09-10 10:05:21.607052 qreader-3.8/documentation/benchmark/
--rw-rw-rw-   0        0        0     3133 2023-09-10 00:28:06.000000 qreader-3.8/documentation/benchmark/resizes.py
--rw-rw-rw-   0        0        0     6355 2023-09-08 21:04:07.000000 qreader-3.8/documentation/benchmark/rotations.py
-drwxrwxrwx   0        0        0        0 2023-09-10 10:05:21.642070 qreader-3.8/qreader.egg-info/
--rw-rw-rw-   0        0        0    12994 2023-09-10 10:05:21.000000 qreader-3.8/qreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-09-10 10:05:21.000000 qreader-3.8/qreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-10 10:05:21.000000 qreader-3.8/qreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-09-10 10:05:21.000000 qreader-3.8/qreader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-09-10 10:05:21.000000 qreader-3.8/qreader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14744 2023-09-10 10:04:29.000000 qreader-3.8/qreader.py
--rw-rw-rw-   0        0        0      111 2023-09-10 10:05:21.647155 qreader-3.8/setup.cfg
--rw-rw-rw-   0        0        0     1266 2023-09-10 10:05:07.000000 qreader-3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-15 13:02:21.221438 qreader-3.9/
+-rw-rw-rw-   0        0        0     1089 2022-12-03 14:38:15.000000 qreader-3.9/LICENSE
+-rw-rw-rw-   0        0        0    12994 2023-09-15 13:02:21.222436 qreader-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12090 2023-09-08 22:16:09.000000 qreader-3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-09-15 13:02:21.133098 qreader-3.9/documentation/
+drwxrwxrwx   0        0        0        0 2023-09-15 13:02:21.169032 qreader-3.9/documentation/benchmark/
+-rw-rw-rw-   0        0        0     3133 2023-09-10 00:28:06.000000 qreader-3.9/documentation/benchmark/resizes.py
+-rw-rw-rw-   0        0        0     6355 2023-09-08 21:04:07.000000 qreader-3.9/documentation/benchmark/rotations.py
+drwxrwxrwx   0        0        0        0 2023-09-15 13:02:21.220436 qreader-3.9/qreader.egg-info/
+-rw-rw-rw-   0        0        0    12994 2023-09-15 13:02:20.000000 qreader-3.9/qreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-09-15 13:02:20.000000 qreader-3.9/qreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-15 13:02:20.000000 qreader-3.9/qreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-09-15 13:02:20.000000 qreader-3.9/qreader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-09-15 13:02:20.000000 qreader-3.9/qreader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14568 2023-09-15 13:02:11.000000 qreader-3.9/qreader.py
+-rw-rw-rw-   0        0        0      111 2023-09-15 13:02:21.225437 qreader-3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2023-09-15 13:02:11.000000 qreader-3.9/setup.py
```

### Comparing `qreader-3.8/LICENSE` & `qreader-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qreader-3.8/PKG-INFO` & `qreader-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qreader
-Version: 3.8
+Version: 3.9
 Summary: Robust and Straight-Forward solution for reading difficult and tricky QR codes within images in Python. Supported by a YOLOv8 QR Segmentation model.
 Home-page: https://github.com/Eric-Canas/qreader
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qreader Version: 3.8 Summary: Robust and Straight-
+Metadata-Version: 2.1 Name: qreader Version: 3.9 Summary: Robust and Straight-
 Forward solution for reading difficult and tricky QR codes within images in
 Python. Supported by a YOLOv8 QR Segmentation model. Home-page: https://
 github.com/Eric-Canas/qreader Author: Eric Canas Author-email:
 elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `qreader-3.8/README.md` & `qreader-3.9/README.md`

 * *Files identical despite different names*

### Comparing `qreader-3.8/documentation/benchmark/resizes.py` & `qreader-3.9/documentation/benchmark/resizes.py`

 * *Files identical despite different names*

### Comparing `qreader-3.8/documentation/benchmark/rotations.py` & `qreader-3.9/documentation/benchmark/rotations.py`

 * *Files identical despite different names*

### Comparing `qreader-3.8/qreader.egg-info/PKG-INFO` & `qreader-3.9/qreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qreader
-Version: 3.8
+Version: 3.9
 Summary: Robust and Straight-Forward solution for reading difficult and tricky QR codes within images in Python. Supported by a YOLOv8 QR Segmentation model.
 Home-page: https://github.com/Eric-Canas/qreader
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qreader Version: 3.8 Summary: Robust and Straight-
+Metadata-Version: 2.1 Name: qreader Version: 3.9 Summary: Robust and Straight-
 Forward solution for reading difficult and tricky QR codes within images in
 Python. Supported by a YOLOv8 QR Segmentation model. Home-page: https://
 github.com/Eric-Canas/qreader Author: Eric Canas Author-email:
 elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `qreader-3.8/qreader.py` & `qreader-3.9/qreader.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,14 @@
         sometimes work.
         :param image: np.ndarray. The image to be read. It must be a np.ndarray (HxWxC) (uint8).
         :param detection_result: dict[str, np.ndarray|float|tuple[float|int, float|int]]. One of the detection dicts
             returned by the detect method. Note that QReader.detect() returns a tuple of these dicts. This method
             expects just one of them.
         :return: tuple. The decoded QR code in the zbar format.
         """
-        # Try to just decode the QR code
-        decodedQR = decodeQR(image=image, symbols=[ZBarSymbol.QRCODE])
-        if len(decodedQR) > 0:
-            return decodedQR
         # Crop the QR for bbox and quad
         cropped_bbox, _ = crop_qr(image=image, detection=detection_result, crop_key=BBOX_XYXY)
         cropped_quad, updated_detection = crop_qr(image=image, detection=detection_result, crop_key=PADDED_QUAD_XY)
         corrected_perspective = self.__correct_perspective(image=cropped_quad,
                                                            padded_quad_xy=updated_detection[PADDED_QUAD_XY])
 
         for scale_factor in (1, 0.5, 2, 0.25):
```

### Comparing `qreader-3.8/setup.py` & `qreader-3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='qreader',
-    version='3.8',
+    version='3.9',
     packages=find_namespace_packages(),
     # expose qreader.py as the unique module
     py_modules=['qreader'],
     url='https://github.com/Eric-Canas/qreader',
     license='MIT',
     author='Eric Canas',
     author_email='elcorreodeharu@gmail.com',
```

