# Comparing `tmp/nbsite-0.8.6a5.tar.gz` & `tmp/nbsite-0.8.6a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsite-0.8.6a5.tar", last modified: Fri May  3 17:38:17 2024, max compression
+gzip compressed data, was "nbsite-0.8.6a6.tar", last modified: Fri May 31 14:57:23 2024, max compression
```

## Comparing `nbsite-0.8.6a5.tar` & `nbsite-0.8.6a6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/holoviz-icon-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/js/goatcounter.js
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/github-stars-button.html
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/_shared_templates/sidebar-nav-bs-alt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.578041 nbsite-0.8.6a5/nbsite/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31847 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23506 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.574041 nbsite-0.8.6a5/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.582041 nbsite-0.8.6a5/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:38:17.000000 nbsite-0.8.6a5/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 17:38:17.586041 nbsite-0.8.6a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-03 17:37:27.000000 nbsite-0.8.6a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.156312 nbsite-0.8.6a6/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.156312 nbsite-0.8.6a6/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/holoviz-icon-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.156312 nbsite-0.8.6a6/nbsite/_shared_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/js/goatcounter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_templates/github-stars-button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/_shared_templates/sidebar-nav-bs-alt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31847 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23506 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.152312 nbsite-0.8.6a6/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.160313 nbsite-0.8.6a6/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/tests/test_nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 14:57:23.000000 nbsite-0.8.6a6/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-31 14:57:23.164312 nbsite-0.8.6a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-31 14:56:35.000000 nbsite-0.8.6a6/setup.py
```

### Comparing `nbsite-0.8.6a5/LICENSE.txt` & `nbsite-0.8.6a6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/PKG-INFO` & `nbsite-0.8.6a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a5
+Version: 0.8.6a6
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.6a5/README.md` & `nbsite-0.8.6a6/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/__main__.py` & `nbsite-0.8.6a6/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/alert.css` & `nbsite-0.8.6a6/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.6a6/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.6a6/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/js/goatcounter.js` & `nbsite-0.8.6a6/nbsite/_shared_static/js/goatcounter.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.6a6/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.6a6/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/notebook.css` & `nbsite-0.8.6a6/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_static/scroller.css` & `nbsite-0.8.6a6/nbsite/_shared_static/scroller.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 /* CSS for side-scrolling admonition */
 #scroller-right {
   position: fixed;
   top: 80%;
   right: 1%;
   max-width: 10%;
-  background: #ffffff;
   padding: 0.8%;
   transform: translate(0%, -50%);
   border: 1px solid gray;
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
   font-size: smaller;
   z-index: 1;
 }
```

### Comparing `nbsite-0.8.6a5/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.6a6/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/_shared_templates/sidebar-nav-bs-alt.html` & `nbsite-0.8.6a6/nbsite/_shared_templates/sidebar-nav-bs-alt.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/analytics/__init__.py` & `nbsite-0.8.6a6/nbsite/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/cmd.py` & `nbsite-0.8.6a6/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/gallery/gen.py` & `nbsite-0.8.6a6/nbsite/gallery/gen.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.6a6/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/nbbuild.py` & `nbsite-0.8.6a6/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/paramdoc.py` & `nbsite-0.8.6a6/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.6a6/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.6a6/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.6a6/nbsite/pyodide/WorkerHandler.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,9 @@
-const pyodideWorker = new Worker(DOCUMENTATION_OPTIONS.URL_ROOT + '_static/PyodideWebWorker.js');
+const url_root = document.getElementsByTagName('html')[0].getAttribute('data-content_root')
+const pyodideWorker = new Worker(`${url_root}_static/PyodideWebWorker.js`);
 
 pyodideWorker.documents = {}
 pyodideWorker.busy = false
 pyodideWorker.queues = new Map()
 
 const patching = new Map();
```

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/__init__.py` & `nbsite-0.8.6a6/nbsite/pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.6a6/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.6a6/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.6a6/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/shared_conf.py` & `nbsite-0.8.6a6/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/templates/basic/conf.py` & `nbsite-0.8.6a6/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.6a6/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/tests/test_cmd.py` & `nbsite-0.8.6a6/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/tests/test_nbbuild.py` & `nbsite-0.8.6a6/nbsite/tests/test_nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/tests/test_util.py` & `nbsite-0.8.6a6/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite/util.py` & `nbsite-0.8.6a6/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.6a6/nbsite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a5
+Version: 0.8.6a6
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.6a5/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.6a6/nbsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/pyproject.toml` & `nbsite-0.8.6a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.6a6/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/scripts/nbsite_fix_links.py` & `nbsite-0.8.6a6/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/scripts/nbsite_generate_modules.py` & `nbsite-0.8.6a6/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.6a6/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/setup.cfg` & `nbsite-0.8.6a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a5/setup.py` & `nbsite-0.8.6a6/setup.py`

 * *Files identical despite different names*

