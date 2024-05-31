# Comparing `tmp/pyiArduinoI2Cled-1.0.3.tar.gz` & `tmp/pyiArduinoI2Cled-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiArduinoI2Cled-1.0.3.tar", last modified: Fri May 31 18:01:18 2024, max compression
+gzip compressed data, was "dist/pyiArduinoI2Cled-1.1.0.tar", last modified: Fri Dec 11 12:44:35 2020, max compression
```

## Comparing `pyiArduinoI2Cled-1.0.3.tar` & `pyiArduinoI2Cled-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 18:01:18.806467 pyiArduinoI2Cled-1.0.3/
--rw-r--r--   0 dron      (1000) dron      (1000)     3291 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/LICENSE
--rw-r--r--   0 dron      (1000) dron      (1000)       81 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/MANIFEST.in
--rw-r--r--   0 dron      (1000) dron      (1000)     2205 2024-05-31 18:01:18.806467 pyiArduinoI2Cled-1.0.3/PKG-INFO
--rw-r--r--   0 dron      (1000) dron      (1000)       19 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/README
--rw-r--r--   0 dron      (1000) dron      (1000)     1911 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/README.md
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 18:01:18.798467 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/
--rw-r--r--   0 dron      (1000) dron      (1000)    17035 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/WString.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     9967 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/WString.h
--rw-r--r--   0 dron      (1000) dron      (1000)       26 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/__init__.py
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 18:01:18.802467 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/
--rw-r--r--   0 dron      (1000) dron      (1000)    11329 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/FindDevices.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     1506 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/NewAddress.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     1007 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowMillis.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)    17490 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowOptions.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)      662 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowTime.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     1091 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/dtostrf.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     1004 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/dtostrf.h
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 18:01:18.806467 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/
--rwxr-xr-x   0 dron      (1000) dron      (1000)     2495 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/Demo3x.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)     5902 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/FindDevices.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)      790 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowMillis.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)    14601 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowOptions.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)     1136 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowTime.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)     1399 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/newAddress.py
--rwxr-xr-x   0 dron      (1000) dron      (1000)    52821 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.cpp
--rwxr-xr-x   0 dron      (1000) dron      (1000)    28595 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.h
--rw-r--r--   0 dron      (1000) dron      (1000)     3158 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.pxd
--rwxr-xr-x   0 dron      (1000) dron      (1000)    11923 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_PI.h
--rw-r--r--   0 dron      (1000) dron      (1000)     2917 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/itoa.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     1253 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/itoa.h
--rw-r--r--   0 dron      (1000) dron      (1000)   595339 2024-05-31 17:59:31.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/pyiArduinoI2Cled.cpp
--rw-r--r--   0 dron      (1000) dron      (1000)     5068 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/pyiArduinoI2Cled.pyx
--rw-r--r--   0 dron      (1000) dron      (1000)      129 2024-03-29 13:35:16.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/setup.py
-drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-05-31 18:01:18.798467 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled.egg-info/
--rw-r--r--   0 dron      (1000) dron      (1000)     2205 2024-05-31 18:01:18.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled.egg-info/PKG-INFO
--rw-r--r--   0 dron      (1000) dron      (1000)     1074 2024-05-31 18:01:18.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled.egg-info/SOURCES.txt
--rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-05-31 18:01:18.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled.egg-info/dependency_links.txt
--rw-r--r--   0 dron      (1000) dron      (1000)       17 2024-05-31 18:01:18.000000 pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled.egg-info/top_level.txt
--rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-05-31 18:01:18.806467 pyiArduinoI2Cled-1.0.3/setup.cfg
--rw-r--r--   0 dron      (1000) dron      (1000)      708 2024-05-31 17:58:15.000000 pyiArduinoI2Cled-1.0.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-11 12:44:35.000000 pyiArduinoI2Cled-1.1.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2470 2020-12-11 12:44:35.000000 pyiArduinoI2Cled-1.1.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/README
+-rw-r--r--   0 pi        (1000) pi        (1000)     1911 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-11 12:44:35.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/
+-rw-r--r--   0 pi        (1000) pi        (1000)    17035 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/WString.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     9967 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/WString.h
+-rw-r--r--   0 pi        (1000) pi        (1000)       26 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-11 12:44:35.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/
+-rw-r--r--   0 pi        (1000) pi        (1000)    11329 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/FindDevices.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     1506 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/NewAddress.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     1007 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowMillis.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)    17490 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowOptions.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)      662 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowTime.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     1091 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/dtostrf.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     1004 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/dtostrf.h
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-12-11 12:44:35.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     2139 2020-12-08 10:25:56.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/Demo.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     2495 2020-12-11 12:43:04.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/Demo3x.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     5902 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/FindDevices.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1194 2020-12-04 14:41:08.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/SetLed.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1339 2020-12-07 10:14:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowEUR.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      790 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowMillis.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    14601 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowOptions.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1136 2020-12-11 12:40:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowTime.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1393 2020-12-07 10:16:16.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowUSD.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1399 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/newAddress.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    52819 2020-12-11 12:43:54.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.cpp
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    28595 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.h
+-rw-r--r--   0 pi        (1000) pi        (1000)     3158 2020-05-20 14:16:12.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.pxd
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    11923 2020-12-11 12:43:04.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_PI.h
+-rw-r--r--   0 pi        (1000) pi        (1000)     2917 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/itoa.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     1253 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/itoa.h
+-rw-r--r--   0 pi        (1000) pi        (1000)   316042 2020-12-11 12:43:04.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/pyiArduinoI2Cled.cpp
+-rw-r--r--   0 pi        (1000) pi        (1000)     5068 2020-12-04 14:41:57.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/pyiArduinoI2Cled.pyx
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       40 2020-05-20 14:12:53.000000 pyiArduinoI2Cled-1.1.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      708 2020-12-11 12:44:31.000000 pyiArduinoI2Cled-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyiArduinoI2Cled-1.0.3/PKG-INFO` & `pyiArduinoI2Cled-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pyiArduinoI2Cled
-Version: 1.0.3
-Summary: iarduino.ru module for Raspberry Pi
-Home-page: http://github.com/tremaru/pyiArduinoI2Cled
-Author: iarduino.ru
-Author-email: shop@iarduino.ru
-License: MIT
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
 
 # pyiArduinoI2Cled
 
 **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Четырёхразрядный индикатор LED]() от iArduino.ru по шине I2C на Raspberry Pi.**
 
 Подробнее про модуль читайте в нашей [Wiki]()
```

### Comparing `pyiArduinoI2Cled-1.0.3/README.md` & `pyiArduinoI2Cled-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-
-# pyiArduinoI2Cled
-
-**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Четырёхразрядный индикатор LED]() от iArduino.ru по шине I2C на Raspberry Pi.**
-
-Подробнее про модуль читайте в нашей [Wiki]()
-
-## Установка ##
-
-[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-
-Установка из репозиториев PyPI в терминале Raspberry:
-
-`sudo pip3 install pyiArduinoI2Cled`
-
-Самостоятельная сборка из исходников:
-
-`git clone https://github.com/tremaru/pyiArduinoI2Cled.git && cd pyiArduinoI2Cled/pyiArduinoI2Cled && python3 setup.py build_ext --inplace`
-
-Примеры для Python находятся в папке `pyiArduinoI2Cled/examples`
-
-Примеры для С++ находятся в папке `pyiArduinoI2Cled/cpp`. Так же в этой папке лежит *Makefile* для сборки
-из исходников. Можно собрать сразу все примеры командой:
-`make all` или `make`
-Для сборки конкретного примера: `make "название примера"`
-Например:
-`make reset`
-Для удаления собранных исполняемых файлов:
-`make clean`
-
-**This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
+Metadata-Version: 1.1
+Name: pyiArduinoI2Cled
+Version: 1.1.0
+Summary: iarduino.ru module for Raspberry Pi
+Home-page: http://github.com/tremaru/pyiArduinoI2Cled
+Author: iarduino.ru
+Author-email: shop@iarduino.ru
+License: MIT
+Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+        
+        # pyiArduinoI2Cled
+        
+        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) [Четырёхразрядный индикатор LED]() от iArduino.ru по шине I2C на Raspberry Pi.**
+        
+        Подробнее про модуль читайте в нашей [Wiki]()
+        
+        ## Установка ##
+        
+        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+        
+        Установка из репозиториев PyPI в терминале Raspberry:
+        
+        `sudo pip3 install pyiArduinoI2Cled`
+        
+        Самостоятельная сборка из исходников:
+        
+        `git clone https://github.com/tremaru/pyiArduinoI2Cled.git && cd pyiArduinoI2Cled/pyiArduinoI2Cled && python3 setup.py build_ext --inplace`
+        
+        Примеры для Python находятся в папке `pyiArduinoI2Cled/examples`
+        
+        Примеры для С++ находятся в папке `pyiArduinoI2Cled/cpp`. Так же в этой папке лежит *Makefile* для сборки
+        из исходников. Можно собрать сразу все примеры командой:
+        `make all` или `make`
+        Для сборки конкретного примера: `make "название примера"`
+        Например:
+        `make reset`
+        Для удаления собранных исполняемых файлов:
+        `make clean`
+        
+        **This is a Python3 module for Raspberry Pi. It can work with []() by iarduino.ru**
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
```

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/WString.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/WString.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/WString.h` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/WString.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/FindDevices.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/NewAddress.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowMillis.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowMillis.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowOptions.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowOptions.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/cpp/ShowTime.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/cpp/ShowTime.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/dtostrf.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/dtostrf.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/dtostrf.h` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/dtostrf.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/Demo3x.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/Demo3x.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/FindDevices.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowMillis.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowMillis.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowOptions.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowOptions.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/ShowTime.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/ShowTime.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/examples/newAddress.py` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/examples/newAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 				if(_readBytes(REG_BITS_0,1)==false){return false;}																//	Читаем 1 байт регистра «BITS_0» в массив «data».
 				data[0] |= 0b10000000;																							//	Устанавливаем бит «SET_RESET»
 				if(_writeBytes(REG_BITS_0,1)==false){return false;}																//	Записываем 1 байт в регистр «BITS_0» из массива «data».
 			//	Ждём установки флага завершения перезагрузки:																	//
                 delay(500);
                 /*
                 int counter = 0;
-				do { 
+				do {
                     if(_readBytes(REG_FLAGS_0,1)==false) {
                         return false;
-                    } 
+                    }
                     delay(1);
                     counter++;
                 }														//	Читаем 1 байт регистра «REG_FLAGS_0» в массив «data».
 				while(((data[0]&0b10000000) == 0) || (counter < 50));																				//	Повторяем чтение пока не установится флаг «FLG_RESET».
                 */
                 //std::cout << "i'm here" << '\n';
 				return true;																									//
```

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.h` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_4LED.pxd` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_4LED.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/iarduino_I2C_PI.h` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/iarduino_I2C_PI.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/itoa.cpp` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/itoa.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/itoa.h` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/itoa.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/pyiArduinoI2Cled/pyiArduinoI2Cled.pyx` & `pyiArduinoI2Cled-1.1.0/pyiArduinoI2Cled/pyiArduinoI2Cled.pyx`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cled-1.0.3/setup.py` & `pyiArduinoI2Cled-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cled',
-    version='1.0.3',
+    version='1.1.0',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cled',
     author='iarduino.ru',
```

