# Comparing `tmp/picframe-2023.7.26.post1.tar.gz` & `tmp/picframe-2024.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picframe-2023.7.26.post1.tar", last modified: Wed Jul 26 11:47:36 2023, max compression
+gzip compressed data, was "picframe-2024.2.19.tar", last modified: Mon Feb 19 11:49:02 2024, max compression
```

## Comparing `picframe-2023.7.26.post1.tar` & `picframe-2024.2.19.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.260265 picframe-2023.7.26.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/src/picframe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/config/configuration_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/mat/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_bevel.png
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_drop_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_highlight.png
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_inner_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/mat_texture.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/no_pictures.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.fs
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.vs
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/geo_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/get_image_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/html/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/html/pf_functions.js
--rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/mat_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/start.py
--rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/viewer_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/test/test_get_image_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.193328 picframe-2024.2.19/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-19 11:48:46.000000 picframe-2024.2.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-02-19 11:49:02.193328 picframe-2024.2.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-19 11:48:46.000000 picframe-2024.2.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-19 11:48:46.000000 picframe-2024.2.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-19 11:49:02.193328 picframe-2024.2.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-19 11:48:46.000000 picframe-2024.2.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.177328 picframe-2024.2.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.181328 picframe-2024.2.19/src/picframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-19 11:49:02.193328 picframe-2024.2.19/src/picframe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.185328 picframe-2024.2.19/src/picframe/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/config/configuration_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.185328 picframe-2024.2.19/src/picframe/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.185328 picframe-2024.2.19/src/picframe/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   455164 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   471004 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   470472 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   455188 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.189328 picframe-2024.2.19/src/picframe/data/mat/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/mat/9_patch_bevel.png
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/mat/9_patch_drop_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/mat/9_patch_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/mat/9_patch_inner_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)  2081776 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/mat/mat_texture.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   160442 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/no_pictures.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.189328 picframe-2024.2.19/src/picframe/data/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/shaders/blend_new.fs
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/data/shaders/blend_new.vs
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/geo_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.189328 picframe-2024.2.19/src/picframe/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/html/pf_functions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24352 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/interface_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/interface_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/interface_peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/mat_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18260 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27313 2024-02-19 11:48:46.000000 picframe-2024.2.19/src/picframe/viewer_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.193328 picframe-2024.2.19/src/picframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 11:49:02.000000 picframe-2024.2.19/src/picframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:49:02.189328 picframe-2024.2.19/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-02-19 11:48:46.000000 picframe-2024.2.19/test/test_get_image_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-02-19 11:48:46.000000 picframe-2024.2.19/versioneer.py
```

### Comparing `picframe-2023.7.26.post1/LICENSE` & `picframe-2024.2.19/LICENSE`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/PKG-INFO` & `picframe-2024.2.19/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.7.26.post1
+Version: 2024.2.19
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow>=10.0.1
+Requires-Dist: defusedxml
+Requires-Dist: pi3d>=2.51
+Requires-Dist: PyYAML
+Requires-Dist: paho-mqtt
+Requires-Dist: IPTCInfo3
+Requires-Dist: numpy
+Requires-Dist: ninepatch>=0.2.0
+Requires-Dist: pi_heif>=0.8.0
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
-- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26.post1/README.md` & `picframe-2024.2.19/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
-- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26.post1/pyproject.toml` & `picframe-2024.2.19/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 maintainers = [
   { name = "Helge Erbe", email = "helge@erbehome.de"  },
 ]
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.7"
 classifiers=[
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Multimedia :: Graphics :: Viewers",
 ]
 dynamic = ["version"]
 dependencies = [
-    "Pillow==9.5.0",
+    "Pillow>=10.0.1",
     "defusedxml",
-    "pi3d>=2.49",
+    "pi3d>=2.51",
     "PyYAML",
     "paho-mqtt",
     "IPTCInfo3",
     "numpy",
-    "ninepatch",
+    "ninepatch>=0.2.0",
     "pi_heif>=0.8.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/helgeerbe/picframe"
 
 [project.scripts]
```

### Comparing `picframe-2023.7.26.post1/src/picframe/config/configuration_example.yaml` & `picframe-2024.2.19/src/picframe/config/configuration_example.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
   device_id: "picframe"                   # default="picframe" unique id of device. change if there is more than one PictureFrame
   device_url: ""                          # if use_http==True, set url to picframe config page. Must be a valid url, or "" otherwise home assistant runs in an error.
 
 http:
   use_http: False                         # default=False. Set True to enable http NB THIS SERVER IS FOR LOCAL NETWORK AND SHOULD NOT BE EXPOSED TO EXTERNAL ACCESS
   path: "~/picframe_data/html"            # path to where html files are located
   port: 9000                              # port used to serve pages by http server < 1024 requires root which is *bad* idea
+  auth: false                             # default=False. Set True if enable basic auth for http
+  username: admin                         # username for basic auth
+  password: null                          # password for basic auth. If set null generate random password in file basic_auth.txt in parent http directory
   use_ssl: False
   keyfile: "path/to/key.pem"              # private-key
   certfile: "path/to/cert.pem"            # server certificate
 
 peripherals:
   input_type: null                        # default=null, valid options: {null, "keyboard", "touch", "mouse"}
   buttons:
```

### Comparing `picframe-2023.7.26.post1/src/picframe/controller.py` & `picframe-2024.2.19/src/picframe/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,19 +349,24 @@
                 self.__logger.error("Can't initialize mqtt. Stopping picframe")
                 sys.exit(1)
 
         # start http server
         if self.__http_config['use_http']:
             from picframe import interface_http
             model_config = self.__model.get_model_config()
-            self.__interface_http = interface_http.InterfaceHttp(self,
-                                                                 self.__http_config['path'],
-                                                                 model_config['pic_dir'],
-                                                                 model_config['no_files_img'],
-                                                                 self.__http_config['port'])  # TODO: Implement TLS
+            self.__interface_http = interface_http.InterfaceHttp(
+                                                                    self,
+                                                                    self.__http_config['path'],
+                                                                    model_config['pic_dir'],
+                                                                    model_config['no_files_img'],
+                                                                    self.__http_config['port'],
+                                                                    self.__http_config['auth'],
+                                                                    self.__http_config['username'],
+                                                                    self.__http_config['password'],
+                                                                )  # TODO: Implement TLS
             if self.__http_config['use_ssl']:
                 self.__interface_http.socket = ssl.wrap_socket(
                                                 self.__interface_http.socket,
                                                 keyfile=self.__http_config['keyfile'],
                                                 certfile=self.__http_config['certfile'],
                                                 server_side=True)
```

### Comparing `picframe-2023.7.26.post1/src/picframe/data/fonts/LICENSE.txt` & `picframe-2024.2.19/src/picframe/data/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Bold.ttf` & `picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-BoldItalic.ttf` & `picframe-2024.2.19/src/picframe/data/fonts/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Italic.ttf` & `picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Regular.ttf` & `picframe-2024.2.19/src/picframe/data/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_drop_shadow.png` & `picframe-2024.2.19/src/picframe/data/mat/9_patch_drop_shadow.png`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/mat/mat_texture.jpg` & `picframe-2024.2.19/src/picframe/data/mat/mat_texture.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/no_pictures.jpg` & `picframe-2024.2.19/src/picframe/data/no_pictures.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.fs` & `picframe-2024.2.19/src/picframe/data/shaders/blend_new.fs`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/geo_reverse.py` & `picframe-2024.2.19/src/picframe/geo_reverse.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/get_image_meta.py` & `picframe-2024.2.19/src/picframe/get_image_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,17 @@
         try:
             # ISO prior 2.2, ISOSpeedRatings 2.2, PhotographicSensitivity 2.3
             iso_keys = ['EXIF ISOSpeedRatings', 'EXIF PhotographicSensitivity', 'EXIF ISO']
             if key in iso_keys:
                 for iso in iso_keys:
                     val = self.__get_if_exist(iso)
                     if val:
+                        # If ISO is returned as a tuple, take the first element
+                        if type(val) is tuple:
+                            val = val[0]
                         break
             else:
                 val = self.__get_if_exist(key)
 
             if val is None:
                 grp, tag = key.split(" ", 1)
                 if grp == "EXIF":
```

### Comparing `picframe-2023.7.26.post1/src/picframe/html/index.html` & `picframe-2024.2.19/src/picframe/html/index.html`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/html/pf_functions.js` & `picframe-2024.2.19/src/picframe/html/pf_functions.js`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/image_cache.py` & `picframe-2024.2.19/src/picframe/image_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,16 +352,17 @@
     #     - Found on disk, but newer than the associated record in the 'folder' table
     #     - Found on disk, but flagged as 'missing' in the 'folder' table
     # --- Note that all folders returned currently exist on disk
     def __get_modified_folders(self):
         out_of_date_folders = []
         sql_select = "SELECT * FROM folder WHERE name = ?"
         for dir in [d[0] for d in os.walk(self.__picture_dir, followlinks=self.__follow_links)]:
-            if os.path.basename(dir)[0] == '.':
-                continue  # ignore hidden folders
+            if os.path.basename(dir):
+                if os.path.basename(dir)[0] == '.':
+                    continue  # ignore hidden folders
             mod_tm = int(os.stat(dir).st_mtime)
             found = self.__db.execute(sql_select, (dir,)).fetchone()
             if not found or found['last_modified'] < mod_tm or found['missing'] == 1:
                 out_of_date_folders.append((dir, mod_tm))
         return out_of_date_folders
 
     def __get_modified_files(self, modified_folders):
@@ -408,15 +409,18 @@
         self.__db_write_lock.acquire()
         self.__db.execute(folder_insert, (dir,))
         self.__db.execute(folder_update, (dir,))
         if file_id is None:
             self.__db.execute(file_insert, (dir, base, extension.lstrip("."), mod_tm))
         else:
             self.__db.execute(file_update, (dir, base, extension.lstrip("."), mod_tm, file_id))
-        self.__db.execute(meta_insert, vals)
+        try:
+            self.__db.execute(meta_insert, vals)
+        except:
+            self.__logger.error(f"###FAILED meta_insert = {meta_insert}, vals = {vals}")
         self.__db_write_lock.release()
 
     def __update_folder_info(self, folder_collection):
         update_data = []
         sql = "UPDATE folder SET last_modified = ?, missing = 0 WHERE name = ?"
         for folder, modtime in folder_collection:
             update_data.append((modtime, folder))
```

### Comparing `picframe-2023.7.26.post1/src/picframe/interface_http.py` & `picframe-2024.2.19/src/picframe/interface_http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import time
 import os
 import logging
 import json
 import threading
+import base64
 
 try:
     from http.server import BaseHTTPRequestHandler, HTTPServer  # py3
     import urllib.parse as urlparse
 except ImportError:
     from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer  # py2
     import urlparse
@@ -41,15 +42,41 @@
         logger = logging.getLogger("interface_http.heif_to_jpg")
         logger.warning("Failed attempt to convert %s \n** Have you installed pi_heif? **", fname)
         return ""  # this will not render as a page and will generate error TODO serve specific page with explicit error
 
 
 class RequestHandler(BaseHTTPRequestHandler):
 
+    def do_AUTHHEAD(self):
+        if self.server._auth is not None:
+            if self.headers.get("Authorization") == None:
+                self.send_response(401)
+                self.send_header("WWW-Authenticate", 'Basic realm="Restricted"')
+                self.send_header("Content-type", "text/html")
+                self.end_headers()
+                response_message = "Error: No authorization header received. Please provide valid credentials.\n"
+                self.wfile.write(response_message.encode('utf-8'))
+                self.connection.close()
+                return False
+            elif self.headers.get("Authorization") != "Basic " + self.server._auth:
+                self.send_response(403)
+                self.send_header("Content-type", "text/html")
+                self.end_headers()
+                response_message = "Error: Invalid authentication credentials. Access denied.\n"
+                self.wfile.write(response_message.encode('utf-8'))
+                self.connection.close()
+                return False
+        return True
+
     def do_GET(self):  # noqa: C901
+        if not self.do_AUTHHEAD():
+            source_ip = self.client_address[0]
+            log_message = f"Authentication failed for source IP: {source_ip}"
+            self.server._logger.warning(log_message)
+            return
         try:
             path_split = self.path.split("?")
             page_ok = False
             if len(path_split) == 1:  # i.e. no ? - just serve index.html or image
                 if path_split[0] != "/":  # serve static page from html_path...
                     html_page = path_split[0].strip("/")
                 else:
@@ -136,24 +163,37 @@
             super().end_headers()
         except BrokenPipeError as e:
             self.connection.close()
             self.server._logger.error('httpserver error: {}'.format(e))
 
 
 class InterfaceHttp(HTTPServer):
-    def __init__(self, controller, html_path, pic_dir, no_files_img, port=9000):
+    def __init__(
+            self,
+            controller,
+            html_path,
+            pic_dir,
+            no_files_img,
+            port=9000,
+            auth=False,
+            username=None,
+            password=None,
+        ):
         super(InterfaceHttp, self).__init__(("0.0.0.0", port), RequestHandler)
         # NB name mangling throws a spanner in the works here!!!!!
         # *no* __dunders
         self._logger = logging.getLogger("simple_server.InterfaceHttp")
         self._logger.info("creating an instance of InterfaceHttp")
         self._controller = controller
         self._pic_dir = os.path.expanduser(pic_dir)
         self._no_files_img = os.path.expanduser(no_files_img)
         self._html_path = os.path.expanduser(html_path)
+        self._auth = None
+        if auth:
+            self._auth = base64.b64encode(f"{username}:{password}".encode()).decode()
         # TODO check below works with all decorated methods.. seems to work
         controller_class = controller.__class__
         self._setters = [method for method in dir(controller_class)
                          if 'setter' in dir(getattr(controller_class, method))]
         t = threading.Thread(target=self.serve_forever)
         t.start()
```

### Comparing `picframe-2023.7.26.post1/src/picframe/interface_mqtt.py` & `picframe-2024.2.19/src/picframe/interface_mqtt.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/interface_peripherals.py` & `picframe-2024.2.19/src/picframe/interface_peripherals.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/mat_image.py` & `picframe-2024.2.19/src/picframe/mat_image.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/model.py` & `picframe-2024.2.19/src/picframe/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,14 +204,24 @@
     def get_model_config(self):
         return self.__config['model']
 
     def get_mqtt_config(self):
         return self.__config['mqtt']
 
     def get_http_config(self):
+        if 'auth' in self.__config['http'] and self.__config['http']['auth'] and self.__config['http']['password'] is None:
+            http_parent = os.path.abspath(os.path.join(self.__config['http']['path'], os.pardir))
+            password_path = os.path.join(http_parent, 'basic_auth.txt')
+            if not os.path.exists(password_path):
+                new_password = self.__generate_random_string(64)
+                with open(password_path, "w") as f:
+                    f.write(new_password)
+            with open(password_path, "r") as f:
+                password = f.read()
+                self.__config['http']['password'] = password
         return self.__config['http']
 
     def get_peripherals_config(self):
         return self.__config['peripherals']
 
     @property
     def fade_time(self):
@@ -421,7 +431,12 @@
         sort_clause = ",".join(sort_list)
 
         self.__file_list = self.__image_cache.query_cache(where_clause, sort_clause)
         self.__number_of_files = len(self.__file_list)
         self.__file_index = 0
         self.__num_run_through = 0
         self.__reload_files = False
+
+    def __generate_random_string(self, length):
+        random_bytes = os.urandom(length // 2)
+        random_string = ''.join('{:02x}'.format(ord(chr(byte))) for byte in random_bytes)
+        return random_string
```

### Comparing `picframe-2023.7.26.post1/src/picframe/start.py` & `picframe-2024.2.19/src/picframe/start.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/src/picframe/viewer_display.py` & `picframe-2024.2.19/src/picframe/viewer_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,18 @@
         else:  # no transition effect safe to update database, resuffle etc
             self.__in_transition = False
 
         self.__slide.draw()
 
         if self.__alpha >= 1.0 and tm < self.__name_tm:
             # this sets alpha for the TextBlock from 0 to 1 then back to 0
-            dt = 1.0 - (self.__name_tm - tm) / self.__show_text_tm
+            if self.__show_text_tm > 0:
+                dt = 1.0 - (self.__name_tm - tm) / self.__show_text_tm
+            else:
+                dt = 1
             if dt > 0.995:
                 dt = 1  # ensure that calculated alpha value fully reaches 0 (TODO: Improve!)
             ramp_pt = max(4.0, self.__show_text_tm / 4.0)  # always > 4 so text fade will always < 4s
 
             # create single saw tooth over 0 to __show_text_tm
             alpha = max(0.0, min(1.0, ramp_pt * (1.0 - abs(1.0 - 2.0 * dt))))  # function only run if image alpha is 1.0 so can use 1.0 - abs... # noqa: E501
```

### Comparing `picframe-2023.7.26.post1/src/picframe.egg-info/PKG-INFO` & `picframe-2024.2.19/src/picframe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.7.26.post1
+Version: 2024.2.19
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow>=10.0.1
+Requires-Dist: defusedxml
+Requires-Dist: pi3d>=2.51
+Requires-Dist: PyYAML
+Requires-Dist: paho-mqtt
+Requires-Dist: IPTCInfo3
+Requires-Dist: numpy
+Requires-Dist: ninepatch>=0.2.0
+Requires-Dist: pi_heif>=0.8.0
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
-- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26.post1/src/picframe.egg-info/SOURCES.txt` & `picframe-2024.2.19/src/picframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/test/test_get_image_meta.py` & `picframe-2024.2.19/test/test_get_image_meta.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26.post1/versioneer.py` & `picframe-2024.2.19/versioneer.py`

 * *Files identical despite different names*

