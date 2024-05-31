# Comparing `tmp/getdist-1.4.8.tar.gz` & `tmp/getdist-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getdist-1.4.8.tar", last modified: Sat Apr 13 08:26:47 2024, max compression
+gzip compressed data, was "getdist-1.4.9.tar", last modified: Fri May 31 15:35:59 2024, max compression
```

## Comparing `getdist-1.4.8.tar` & `getdist-1.4.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.395977 getdist-1.4.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2024-04-13 08:24:04.000000 getdist-1.4.8/GetDistGUI.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68114 2024-04-13 08:24:04.000000 getdist-1.4.8/LICENCE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2024-04-13 08:24:04.000000 getdist-1.4.8/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-04-13 08:26:47.395977 getdist-1.4.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10649 2024-04-13 08:24:04.000000 getdist-1.4.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.375976 getdist-1.4.8/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.379976 getdist-1.4.8/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9201 2024-04-13 08:24:04.000000 getdist-1.4.8/docs/source/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.383976 getdist-1.4.8/getdist/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1947 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/analysis_defaults.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/chain_grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63744 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/chains.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11212 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/cobaya_interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12863 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/command_line.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9222 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/convolve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covcomb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3901 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covmat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      778 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covscale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12283 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/densities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/distparam_template.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    22044 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gaussian_mixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/SyntaxHighlight.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16164 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/Icon.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/delete.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/delete_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/open.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/open_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/remove.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/remove_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      373 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/save.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/save_large.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.375976 getdist-1.4.8/getdist/gui/mac_app/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1263 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/Info.plist
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/MacOS/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      122 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/MacOS/GetDistGUI
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)   559497 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns
--rw-rw-r--   0 travis    (2000) travis    (2000)    96734 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13684 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/inifile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11881 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/kde_bandwidth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16654 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/matplotlib_ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118646 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/mcsamples.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16211 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/paramnames.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/parampriors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   170183 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/plots.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist/styles/
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5921 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/planck.paramnames
--rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/planck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16929 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/sfmath.sty
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/tab10.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19711 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/getdist_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16705 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/test_distributions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37192 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/yaml_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2024-04-13 08:24:04.000000 getdist-1.4.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-13 08:26:47.395977 getdist-1.4.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2024-04-13 08:24:04.000000 getdist-1.4.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.386829 getdist-1.4.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2024-05-31 15:33:12.000000 getdist-1.4.9/GetDistGUI.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68114 2024-05-31 15:33:12.000000 getdist-1.4.9/LICENCE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2024-05-31 15:33:12.000000 getdist-1.4.9/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-05-31 15:35:59.386829 getdist-1.4.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10649 2024-05-31 15:33:12.000000 getdist-1.4.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.366827 getdist-1.4.9/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.370827 getdist-1.4.9/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9201 2024-05-31 15:33:12.000000 getdist-1.4.9/docs/source/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.378828 getdist-1.4.9/getdist/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1947 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/analysis_defaults.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/chain_grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63744 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/chains.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11212 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/cobaya_interface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12863 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/command_line.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9222 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/convolve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/covcomb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3901 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/covmat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      778 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/covscale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12283 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/densities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/distparam_template.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22044 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gaussian_mixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.378828 getdist-1.4.9/getdist/gui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/SyntaxHighlight.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.382828 getdist-1.4.9/getdist/gui/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16164 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/Icon.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      337 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/delete.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/delete_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/open.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      809 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/open_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/remove.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/remove_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      373 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/save.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      423 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/images/save_large.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.366827 getdist-1.4.9/getdist/gui/mac_app/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.382828 getdist-1.4.9/getdist/gui/mac_app/Contents/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1263 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/mac_app/Contents/Info.plist
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.382828 getdist-1.4.9/getdist/gui/mac_app/Contents/MacOS/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      122 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/mac_app/Contents/MacOS/GetDistGUI
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.382828 getdist-1.4.9/getdist/gui/mac_app/Contents/Resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   559497 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96734 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/gui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13684 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/inifile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11881 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/kde_bandwidth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16654 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/matplotlib_ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118646 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/mcsamples.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16211 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/paramnames.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/parampriors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   171470 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/plots.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.382828 getdist-1.4.9/getdist/styles/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/styles/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5921 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/styles/planck.paramnames
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/styles/planck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16929 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/styles/sfmath.sty
+-rw-rw-r--   0 travis    (2000) travis    (2000)      517 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/styles/tab10.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.386829 getdist-1.4.9/getdist/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19711 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/tests/getdist_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16705 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/tests/test_distributions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37192 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2024-05-31 15:33:12.000000 getdist-1.4.9/getdist/yaml_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-31 15:35:59.386829 getdist-1.4.9/getdist.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2024-05-31 15:35:59.000000 getdist-1.4.9/getdist.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2024-05-31 15:33:12.000000 getdist-1.4.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-31 15:35:59.386829 getdist-1.4.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2024-05-31 15:33:12.000000 getdist-1.4.9/setup.py
```

### Comparing `getdist-1.4.8/LICENCE.txt` & `getdist-1.4.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/PKG-INFO` & `getdist-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getdist
-Version: 1.4.8
+Version: 1.4.9
 Summary: GetDist Monte Carlo sample analysis, plotting and GUI
 Author: Antony Lewis
 License: GetDist, Copyright (c) 2019, Antony Lewis
         
         Code to find optimal bandwidths for basic kernel density estimators in 1 and 2D
         was adapted from Matlab code by Zdravko Botev. Original code notice:
```

### Comparing `getdist-1.4.8/README.rst` & `getdist-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/docs/source/conf.py` & `getdist-1.4.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/__init__.py` & `getdist-1.4.9/getdist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'Antony Lewis'
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __url__ = "https://getdist.readthedocs.io"
 
 import os
 import sys
 from getdist.inifile import IniFile
 from getdist.paramnames import ParamInfo, ParamNames
 from getdist.chains import WeightedSamples
```

### Comparing `getdist-1.4.8/getdist/_base.py` & `getdist-1.4.9/getdist/_base.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/analysis_defaults.ini` & `getdist-1.4.9/getdist/analysis_defaults.ini`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/chain_grid.py` & `getdist-1.4.9/getdist/chain_grid.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/chains.py` & `getdist-1.4.9/getdist/chains.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/cobaya_interface.py` & `getdist-1.4.9/getdist/cobaya_interface.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/command_line.py` & `getdist-1.4.9/getdist/command_line.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/convolve.py` & `getdist-1.4.9/getdist/convolve.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/covmat.py` & `getdist-1.4.9/getdist/covmat.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/covscale.py` & `getdist-1.4.9/getdist/covscale.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/densities.py` & `getdist-1.4.9/getdist/densities.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/distparam_template.ini` & `getdist-1.4.9/getdist/distparam_template.ini`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gaussian_mixtures.py` & `getdist-1.4.9/getdist/gaussian_mixtures.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/SyntaxHighlight.py` & `getdist-1.4.9/getdist/gui/SyntaxHighlight.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/images/Icon.png` & `getdist-1.4.9/getdist/gui/images/Icon.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/images/delete_large.png` & `getdist-1.4.9/getdist/gui/images/delete_large.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/images/open_large.png` & `getdist-1.4.9/getdist/gui/images/open_large.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/mac_app/Contents/Info.plist` & `getdist-1.4.9/getdist/gui/mac_app/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns` & `getdist-1.4.9/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/gui/mainwindow.py` & `getdist-1.4.9/getdist/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/inifile.py` & `getdist-1.4.9/getdist/inifile.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/kde_bandwidth.py` & `getdist-1.4.9/getdist/kde_bandwidth.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/matplotlib_ext.py` & `getdist-1.4.9/getdist/matplotlib_ext.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/mcsamples.py` & `getdist-1.4.9/getdist/mcsamples.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/paramnames.py` & `getdist-1.4.9/getdist/paramnames.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/parampriors.py` & `getdist-1.4.9/getdist/parampriors.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/plots.py` & `getdist-1.4.9/getdist/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1692,35 +1692,34 @@
 
         """
         roots = makeList(roots)
         if isinstance(param1, (list, tuple)):
             param_pair = param1
             param1 = None
         _no_finish = kwargs.pop('_no_finish', False)
-        param_pair = self.get_param_array(roots[0], param_pair or [param1, param2])
+        param_pair = self.get_param_array(roots, param_pair or [param1, param2])
         ax = self.get_axes(ax, pars=param_pair)
         if self.settings.progress:
             print('plotting: ', [param.name for param in param_pair])
         if shaded is not False and not kwargs.get('filled'):
             self.add_2d_shading(roots[0 if shaded is True else shaded], *param_pair, ax=ax)
         xbounds, ybounds = None, None
         contour_args = self._make_contour_args(len(roots), **kwargs)
         for i, root in enumerate(roots):
             res = self.add_2d_contours(root, param_pair[0], param_pair[1], line_offset + i, of=len(roots), ax=ax,
                                        add_legend_proxy=add_legend_proxy and root not in proxy_root_exclude,
                                        **contour_args[i])
             xbounds, ybounds = self._update_limits(res, xbounds, ybounds)
-        if xbounds is None:
-            return
-        if 'lims' not in kwargs:
+        if xbounds is not None and 'lims' not in kwargs:
             lim1 = self._check_param_ranges(roots[0], param_pair[0].name, xbounds[0], xbounds[1])
             lim2 = self._check_param_ranges(roots[0], param_pair[1].name, ybounds[0], ybounds[1])
             kwargs['lims'] = [lim1[0], lim1[1], lim2[0], lim2[1]]
-
         self.set_axes(param_pair, ax=ax, **kwargs)
+        if xbounds is None:
+            return
         if not _no_finish and len(self.fig.axes) == 1:
             self.finish_plot()
         return xbounds, ybounds
 
     def default_col_row(self, nplot=1, nx=None, ny=None):
         """
         Get default subplot columns and rows depending on number of subplots.
@@ -1763,42 +1762,40 @@
                        self.settings.subplot_size_inch * self.plot_row * ystretch)
         if self.settings.constrained_layout:
             self.fig = plt.figure(figsize=figsize, constrained_layout=True)
         else:
             self.fig = plt.figure(figsize=figsize)
         self.gridspec = matplotlib.gridspec.GridSpec(nrows=self.plot_row, ncols=self.plot_col, figure=self.fig)
 
-        if sharey:
-            self._share_kwargs = {'w_pad': 0, 'wspace': 0}
-        else:
-            self._share_kwargs = {}
+        self._share_kwargs = {'w_pad': 0, 'wspace': 0} if sharey else {}
         if sharex:
             self._share_kwargs.update({'h_pad': 0, 'hspace': 0})
 
         if self.settings.constrained_layout and self._share_kwargs:
-            self.fig.set_constrained_layout_pads(**self._share_kwargs)
+            self.fig.get_layout_engine().set(**self._share_kwargs)
 
         self.subplots = np.ndarray((self.plot_row, self.plot_col), dtype=object)
         self.subplots[:, :] = None
         return self.plot_col, self.plot_row
 
-    def get_param_array(self, root, params: Union[None, str, Sequence] = None, renames: Mapping = None):
+    def get_param_array(self, roots, params: Union[None, str, Sequence] = None, renames: Mapping = None):
         """
         Gets an array of :class:`~.paramnames.ParamInfo` for named params
         in the given `root`.
 
         If a parameter is not found in `root`, returns the original ParamInfo if ParamInfo
         was passed, or fails otherwise.
 
-        :param root: The root name of the samples to use
-        :param params: the parameter names (if not specified, get all)
+        :param roots: The root name of the samples to use, or list of roots
+        :param params: the parameter names (if not specified, get all in first root)
         :param renames: optional dictionary mapping input names and equivalent names
                         used by the samples
         :return: list of :class:`~.paramnames.ParamInfo` instances for the parameters
         """
+        root, roots = (roots[0], roots) if isinstance(roots, (list, tuple)) else (roots, [roots])
         if hasattr(root, 'param_names'):
             names = root.param_names
         elif hasattr(root, 'paramNames'):
             names = root.paramNames
         elif hasattr(root, 'names'):
             names = ParamNames(names=root.names, default=getattr(root, 'dim', 0))
         else:
@@ -1817,39 +1814,65 @@
                                        for i, param in enumerate(params) if is_param_info[i]}
             if renames:
                 renames = mergeRenames(renames, renames_from_param_info)
             else:
                 renames = renames_from_param_info
             params_names = [getattr(param, "name", param) for param in params]
             old = [(old if isinstance(old, ParamInfo) else ParamInfo(old)) for old in params]
-            return [new or old for new, old in zip(names.parsWithNames(params_names,
-                                                                       error=error, renames=renames), old)]
+
+            if len(roots) == 1:
+                return [new or old for new, old in zip(names.parsWithNames(params_names,
+                                                                           error=error, renames=renames), old)]
+            # check if requesting parameter that is not in the first root
+            has_names = [i for i, param_name in enumerate(params_names) if names.hasParam(param_name)]
+            not_names = [i for i in range(len(params)) if i not in has_names]
+            if not not_names:
+                return names.parsWithNames(params_names, renames=renames)
+
+            first_params = names.parsWithNames([params_names[i] for i in has_names], renames=renames)
+            extra_params = self.get_param_array(roots[1:], [params[i] for i in not_names], renames)
+            result = list(params)
+            for i, j in enumerate(has_names):
+                result[j] = first_params[i]
+            for i, j in enumerate(not_names):
+                result[j] = extra_params[i]
+            return result
 
     def _check_param(self, root, param, renames=None):
         """
         Get :class:`~.paramnames.ParamInfo` for given name for samples with specified root
 
         If a parameter is not found in `root`, returns the original ParamInfo if ParamInfo
         was passed, or fails otherwise.
 
         :param root: The root name of the samples
         :param param: The parameter name (or :class:`~.paramnames.ParamInfo`)
         :param renames: optional dictionary mapping input names and equivalent names
                         used by the samples
         :return: a :class:`~.paramnames.ParamInfo` instance, or None if name not found
         """
+
         if isinstance(param, ParamInfo):
             name = param.name
             if hasattr(param, 'renames'):
                 if renames:
                     renames = {name: makeList(renames.get(name, [])) + list(param.renames)}
                 else:
                     renames = {name: list(param.renames)}
         else:
             name = param
+        if isinstance(root, (list, tuple)):
+            if isinstance(param, ParamInfo):
+                root = root[0]
+            else:
+                for a_root in root:
+                    par = self.param_names_for_root(a_root).parWithName(name, error=a_root is root[-1], renames=renames)
+                    if par is not None:
+                        return par
+
         # NB: If a parameter is not found, errors only if param is a ParamInfo instance
         return self.param_names_for_root(root).parWithName(name, error=(name == param), renames=renames)
 
     def param_latex_label(self, root, name, label_params=None):
         """
         Returns the latex label for given parameter.
 
@@ -2103,17 +2126,17 @@
             g = plots.get_subplot_plotter()
             g.plots_1d([samples1, samples2], ['x0', 'x1', 'x2'], nx=3, share_y=True, legend_ncol =2,
                          markers={'x1':0}, colors=['red', 'green'], ls=['--', '-.'])
 
         """
         roots = makeList(roots)
         if roots_per_param:
-            params = [self._check_param(root[0], param, param_renames) for root, param in zip(roots, params)]
+            params = [self._check_param(root, param, param_renames) for root, param in zip(roots, params)]
         else:
-            params = self.get_param_array(roots[0], params, param_renames)
+            params = self.get_param_array(roots, params, param_renames)
         if param_list is None:
             param_list = kwargs.pop('paramList', None)
         if param_list is not None:
             wanted_params = ParamNames(param_list).list()
             params = [param for param in params if
                       param.name in wanted_params or param_renames and param_renames.get(param.name,
                                                                                          '') in wanted_params]
@@ -2175,24 +2198,24 @@
         pairs = []
         roots = makeList(roots)
         if isinstance(param1, (list, tuple)) and len(param1) == 2:
             params2 = [param1[1]]
             param1 = param1[0]
         if param_pairs is None:
             if param1 is not None:
-                param1 = self._check_param(roots[0], param1)
-                params2 = self.get_param_array(roots[0], params2)
+                param1 = self._check_param(roots, param1)
+                params2 = self.get_param_array(roots, params2)
                 for param in params2:
                     if param.name != param1.name:
                         pairs.append((param1, param))
             else:
                 raise GetDistPlotError('No parameter or parameter pairs for 2D plot')
         else:
             for pair in param_pairs:
-                pairs.append((self._check_param(roots[0], pair[0]), self._check_param(roots[0], pair[1])))
+                pairs.append((self._check_param(roots, pair[0]), self._check_param(roots, pair[1])))
         if filled and shaded:
             raise GetDistPlotError("Plots cannot be both filled and shaded")
         plot_col, plot_row = self.make_figure(len(pairs), nx=nx)
 
         for i, pair in enumerate(pairs):
             ax = self._subplot_number(i, pars=pair)
             self.plot_2d(roots, param_pair=pair, filled=filled, shaded=not filled and shaded,
@@ -2372,15 +2395,15 @@
             from getdist import plots, gaussian_mixtures
             samples1, samples2 = gaussian_mixtures.randomTestMCSamples(ndim=4, nMCSamples=2)
             g = plots.get_subplot_plotter()
             g.triangle_plot([samples1, samples2], ['x0','x1','x2'], plot_3d_with_param='x3')
 
         """
         roots = makeList(roots)
-        params = self.get_param_array(roots[0], params)
+        params = self.get_param_array(roots, params)
         plot_col = len(params)
         if plot_3d_with_param is not None:
             col_param = self._check_param(roots[0], plot_3d_with_param)
         self.make_figure(nx=plot_col, ny=plot_col, sharex=self.settings.no_triangle_axis_labels,
                          sharey=self.settings.no_triangle_axis_labels)
         lims = dict()
         if kwargs.pop('filled_compare', False):
```

### Comparing `getdist-1.4.8/getdist/styles/planck.paramnames` & `getdist-1.4.9/getdist/styles/planck.paramnames`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/styles/planck.py` & `getdist-1.4.9/getdist/styles/planck.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/styles/sfmath.sty` & `getdist-1.4.9/getdist/styles/sfmath.sty`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/styles/tab10.py` & `getdist-1.4.9/getdist/styles/tab10.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/tests/getdist_test.py` & `getdist-1.4.9/getdist/tests/getdist_test.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/tests/test_distributions.py` & `getdist-1.4.9/getdist/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/types.py` & `getdist-1.4.9/getdist/types.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist/yaml_tools.py` & `getdist-1.4.9/getdist/yaml_tools.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/getdist.egg-info/PKG-INFO` & `getdist-1.4.9/getdist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getdist
-Version: 1.4.8
+Version: 1.4.9
 Summary: GetDist Monte Carlo sample analysis, plotting and GUI
 Author: Antony Lewis
 License: GetDist, Copyright (c) 2019, Antony Lewis
         
         Code to find optimal bandwidths for basic kernel density estimators in 1 and 2D
         was adapted from Matlab code by Zdravko Botev. Original code notice:
```

### Comparing `getdist-1.4.8/getdist.egg-info/SOURCES.txt` & `getdist-1.4.9/getdist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/pyproject.toml` & `getdist-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdist-1.4.8/setup.py` & `getdist-1.4.9/setup.py`

 * *Files identical despite different names*

