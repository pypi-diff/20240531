# Comparing `tmp/pyiArduinoI2Cmatrix-1.0.1.tar.gz` & `tmp/pyiArduinoI2Cmatrix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cmatrix-1.0.1.tar", last modified: Thu Oct  3 11:21:52 2019, max compression
+gzip compressed data, was "pyiArduinoI2Cmatrix-1.0.3.tar", last modified: Fri May 31 17:51:00 2024, max compression
```

## Comparing `pyiArduinoI2Cmatrix-1.0.1.tar` & `pyiArduinoI2Cmatrix-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,33 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      316 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/README
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     3150 2019-09-26 16:36:40.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Angle.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1622 2019-09-30 11:30:36.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Blink.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2021 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/BlinkAnimation.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3762 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Image.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2777 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/PrintCharAnimationRus.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3362 2019-09-30 11:30:42.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/PrintTickerRus.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    17035 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/WString.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     9967 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/WString.h
--rw-r--r--   0 pi        (1000) pi        (1000)       29 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1091 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/dtostrf.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1004 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/dtostrf.h
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-10-03 11:21:52.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     2670 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/10Image.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4453 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/11PrintTicker.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1437 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/1Blink.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2292 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/2Ani.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1889 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/3newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1316 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/4PrintNum.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2146 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/5PrintChar.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2319 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/6PrintCharAnimation.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2139 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/7PrintCharRus.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1197 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/8PrintTicker.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1126 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/examples/9PrintTicker.py
--rw-r--r--   0 pi        (1000) pi        (1000)    58387 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    26176 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1849 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)    12711 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)     2917 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/itoa.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1253 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/itoa.h
--rw-r--r--   0 pi        (1000) pi        (1000)   353410 2019-10-03 11:20:28.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     8775 2019-10-03 11:18:06.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      132 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2019-09-26 15:27:03.000000 pyiArduinoI2Cmatrix-1.0.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      814 2019-10-03 11:19:24.000000 pyiArduinoI2Cmatrix-1.0.1/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 17:51:00.575533 pyiArduinoI2Cmatrix-1.0.3/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       83 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)      299 2024-05-31 17:51:00.575533 pyiArduinoI2Cmatrix-1.0.3/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-05-31 17:50:59.000000 pyiArduinoI2Cmatrix-1.0.3/README
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 17:51:00.575533 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 17:51:00.575533 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3150 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Angle.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1622 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Blink.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2021 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/BlinkAnimation.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3762 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Image.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2777 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/PrintCharAnimationRus.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3362 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/PrintTickerRus.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    17035 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/WString.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     9967 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/WString.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1091 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/dtostrf.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1004 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/dtostrf.h
+-rw-r--r--   0 dron      (1000) dron      (1000)    58387 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    26176 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1849 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)    12711 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     2917 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/itoa.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1253 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/itoa.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   714565 2024-05-31 17:48:47.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     8775 2024-03-29 13:35:31.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.pyx
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 17:51:00.575533 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)      299 2024-05-31 17:51:00.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)      913 2024-05-31 17:51:00.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-05-31 17:51:00.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       20 2024-05-31 17:51:00.000000 pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-05-31 17:51:00.579533 pyiArduinoI2Cmatrix-1.0.3/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      814 2024-05-31 17:50:56.000000 pyiArduinoI2Cmatrix-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Angle.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Angle.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Blink.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Blink.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/BlinkAnimation.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/BlinkAnimation.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/Image.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/Image.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/PrintCharAnimationRus.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/PrintCharAnimationRus.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/Cpp/PrintTickerRus.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/Cpp/PrintTickerRus.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/WString.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/WString.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/WString.h` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/WString.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/dtostrf.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/dtostrf.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/dtostrf.h` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/dtostrf.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.h` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.pxd` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_Matrix_8x8.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/iarduino_I2C_PI.h` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/itoa.cpp` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/itoa.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/itoa.h` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/itoa.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.pyx` & `pyiArduinoI2Cmatrix-1.0.3/pyiArduinoI2Cmatrix/pyiArduinoI2Cmatrix.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cmatrix-1.0.1/setup.py` & `pyiArduinoI2Cmatrix-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from distutils.extension import Extension
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(name='pyiArduinoI2Cmatrix',
-    version='1.0.1',
+    version='1.0.3',
     description='iarduino.ru module for Raspberry Pi',
 #   long_description=long_description,
 #   long_description_content_type="text/markdown",
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cmatrix',
```

