# Comparing `tmp/pyiArduinoI2Cbumper-1.0.0.tar.gz` & `tmp/pyiArduinoI2Cbumper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cbumper-1.0.0.tar", last modified: Mon Jan 11 11:47:30 2021, max compression
+gzip compressed data, was "pyiArduinoI2Cbumper-1.0.1.tar", last modified: Fri May 31 08:21:51 2024, max compression
```

## Comparing `pyiArduinoI2Cbumper-1.0.0.tar` & `pyiArduinoI2Cbumper-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-01-11 11:47:30.000000 pyiArduinoI2Cbumper-1.0.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     2442 2021-01-11 11:47:30.000000 pyiArduinoI2Cbumper-1.0.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2020-05-18 15:42:36.000000 pyiArduinoI2Cbumper-1.0.0/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1877 2020-05-18 15:42:36.000000 pyiArduinoI2Cbumper-1.0.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-01-11 11:47:30.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/
--rw-r--r--   0 pi        (1000) pi        (1000)       29 2020-05-18 15:42:36.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-01-11 11:47:30.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     9696 2020-12-16 18:29:01.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/FindDevices.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     1494 2020-12-16 18:29:08.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)      505 2020-12-16 18:41:29.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/Serial.h
--rw-r--r--   0 pi        (1000) pi        (1000)     4001 2020-12-16 18:32:47.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/changeLineType.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4690 2020-12-16 18:32:33.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/changeLineTypeAuto.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4467 2020-12-16 18:31:28.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/controlCalibrationButton.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4825 2020-12-16 18:34:56.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineAnalog.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3800 2020-12-16 18:34:38.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineDigital.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4511 2020-12-17 13:23:43.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineDigitalFast.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     6510 2021-01-09 15:44:55.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setCalibrationAuto.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     5666 2020-12-16 18:30:42.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setCalibrationManual.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2880 2020-12-16 18:33:19.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setTurnSignal.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3838 2020-12-16 18:30:52.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setTurnSignalAuto.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-01-11 11:47:30.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     6208 2020-12-17 14:50:01.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1617 2020-12-17 16:05:10.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/changeLineType.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3180 2021-01-09 16:41:15.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/changeLineTypeAuto.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2594 2021-01-11 11:42:01.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/controlCalibrationButton.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2620 2020-12-17 15:45:01.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineAnalog.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2744 2020-12-17 15:19:39.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineDigital.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2693 2020-12-17 16:31:25.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineDigitalFast.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1354 2020-12-17 14:52:58.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/newAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2798 2021-01-09 16:41:46.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setCalibrationAuto.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3776 2021-01-09 16:22:48.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setCalibrationManual.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1491 2020-12-17 16:37:22.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setTurnSignal.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3062 2020-12-17 16:40:10.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setTurnSignalAuto.py
--rw-r--r--   0 pi        (1000) pi        (1000)    52661 2021-01-09 16:47:02.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    26961 2020-12-15 13:51:27.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1294 2020-12-18 15:21:47.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.pxd
--rw-r--r--   0 pi        (1000) pi        (1000)    11841 2020-12-15 14:06:23.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   323444 2020-12-18 19:05:32.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     7567 2020-12-18 19:05:10.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      132 2020-05-18 15:42:36.000000 pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-05-18 15:41:19.000000 pyiArduinoI2Cbumper-1.0.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      723 2021-01-11 11:45:01.000000 pyiArduinoI2Cbumper-1.0.0/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 08:21:51.017576 pyiArduinoI2Cbumper-1.0.1/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       84 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2177 2024-05-31 08:21:51.017576 pyiArduinoI2Cbumper-1.0.1/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/README
+-rw-r--r--   0 dron      (1000) dron      (1000)     1877 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 08:21:51.001576 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/
+-rw-r--r--   0 dron      (1000) dron      (1000)       29 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 08:21:51.009576 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9696 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     1494 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)      505 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/Serial.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     4001 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/changeLineType.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4690 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/changeLineTypeAuto.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4467 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/controlCalibrationButton.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4825 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineAnalog.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3800 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineDigital.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4511 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineDigitalFast.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6510 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setCalibrationAuto.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5666 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setCalibrationManual.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2880 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setTurnSignal.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3838 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setTurnSignalAuto.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 08:21:51.017576 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     6208 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1617 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/changeLineType.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3180 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/changeLineTypeAuto.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2594 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/controlCalibrationButton.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2620 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineAnalog.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2744 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineDigital.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2693 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineDigitalFast.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1354 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/newAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2798 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setCalibrationAuto.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3776 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setCalibrationManual.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1491 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setTurnSignal.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3062 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setTurnSignalAuto.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    52661 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    26961 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1294 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.pxd
+-rw-r--r--   0 dron      (1000) dron      (1000)    11841 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   622430 2024-05-31 08:20:24.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     7567 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      132 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 08:21:51.001576 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2177 2024-05-31 08:21:50.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     1701 2024-05-31 08:21:50.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-05-31 08:21:50.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       20 2024-05-31 08:21:50.000000 pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-05-31 08:21:51.017576 pyiArduinoI2Cbumper-1.0.1/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      723 2024-05-31 08:19:30.000000 pyiArduinoI2Cbumper-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cbumper-1.0.0/PKG-INFO` & `pyiArduinoI2Cbumper-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-Metadata-Version: 1.1
-Name: pyiArduinoI2Cbumper
-Version: 1.0.0
-Summary: iarduino.ru module for Raspberry Pi
-Home-page: http://github.com/tremaru/pyiArduinoI2Cbumper
-Author: iarduino.ru
-Author-email: shop@iarduino.ru
-License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cbumper
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) []() от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        Подробнее про датчик читайте в нашей [Wiki]()
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Cbumper`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cbumper.git && cd pyiArduinoI2Cbumper/pyiArduinoI2Cbumper && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cbumper/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cbumper/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make reset`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Cbumper
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) []() от iArduino.ru по шине I2C на Raspberry Pi.**
+
+Подробнее про датчик читайте в нашей [Wiki]()
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Cbumper`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cbumper.git && cd pyiArduinoI2Cbumper/pyiArduinoI2Cbumper && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cbumper/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cbumper/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make reset`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
```

### Comparing `pyiArduinoI2Cbumper-1.0.0/README.md` & `pyiArduinoI2Cbumper-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyiArduinoI2Cbumper
+Version: 1.0.1
+Summary: iarduino.ru module for Raspberry Pi
+Home-page: http://github.com/tremaru/pyiArduinoI2Cbumper
+Author: iarduino.ru
+Author-email: shop@iarduino.ru
+License: MIT
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
 [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
 
 # pyiArduinoI2Cbumper
 
 **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) []() от iArduino.ru по шине I2C на Raspberry Pi.**
 
 Подробнее про датчик читайте в нашей [Wiki]()
```

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/FindDevices.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/NewAddress.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/changeLineType.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/changeLineType.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/changeLineTypeAuto.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/changeLineTypeAuto.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/controlCalibrationButton.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/controlCalibrationButton.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineAnalog.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineAnalog.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineDigital.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineDigital.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/getLineDigitalFast.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/getLineDigitalFast.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setCalibrationAuto.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setCalibrationAuto.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setCalibrationManual.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setCalibrationManual.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setTurnSignal.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setTurnSignal.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/cpp/setTurnSignalAuto.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/cpp/setTurnSignalAuto.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/FindDevices.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/changeLineType.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/changeLineType.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/changeLineTypeAuto.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/changeLineTypeAuto.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/controlCalibrationButton.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/controlCalibrationButton.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineAnalog.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineAnalog.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineDigital.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineDigital.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/getLineDigitalFast.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/getLineDigitalFast.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/newAddress.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setCalibrationAuto.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setCalibrationAuto.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setCalibrationManual.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setCalibrationManual.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setTurnSignal.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setTurnSignal.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/examples/setTurnSignalAuto.py` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/examples/setTurnSignalAuto.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.cpp` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.h` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.pxd` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_Bumper.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/iarduino_I2C_PI.h` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.pyx` & `pyiArduinoI2Cbumper-1.0.1/pyiArduinoI2Cbumper/pyiArduinoI2Cbumper.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cbumper-1.0.0/setup.py` & `pyiArduinoI2Cbumper-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cbumper',
-    version='1.0.0',
+    version='1.0.1',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cbumper',
     author='iarduino.ru',
```

