# Comparing `tmp/comiclib-0.0.5.tar.gz` & `tmp/comiclib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comiclib-0.0.5.tar", last modified: Tue Jan 16 11:44:57 2024, max compression
+gzip compressed data, was "comiclib-0.0.6.tar", last modified: Fri May 31 15:12:47 2024, max compression
```

## Comparing `comiclib-0.0.5.tar` & `comiclib-0.0.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.998911 comiclib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-16 11:44:49.000000 comiclib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-16 11:44:56.998911 comiclib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-01-16 11:44:49.000000 comiclib-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.982911 comiclib-0.0.5/comiclib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.982911 comiclib-0.0.5/comiclib/LANraragi/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.982911 comiclib-0.0.5/comiclib/LANraragi/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.982911 comiclib-0.0.5/comiclib/LANraragi/public/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/css/config.css
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/css/lrr.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.986911 comiclib-0.0.5/comiclib/LANraragi/public/img/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/empty.png
--rw-r--r--   0 runner    (1001) docker     (127)    47884 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/flubbed.gif
--rw-r--r--   0 runner    (1001) docker     (127)   390286 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55876 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/noThumb.png
--rw-r--r--   0 runner    (1001) docker     (127)   132249 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/notfound.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.986911 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/hachikuji.png
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/hverse.png
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/nadeko.png
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/sadpanda.png
--rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/yotsugi.png
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/img/wait_warmly.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.990911 comiclib-0.0.5/comiclib/LANraragi/public/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/backup.js
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/batch.js
--rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/category.js
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/common.js
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/config.js
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/index_datatables.js
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl.js
--rw-r--r--   0 runner    (1001) docker     (127)    36364 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   805177 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.wasm
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.worker.js
--rw-r--r--   0 runner    (1001) docker     (127)    36369 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder_simd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   792814 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder_simd.wasm
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/logs.js
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/plugins.js
--rw-r--r--   0 runner    (1001) docker     (127)    31178 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/reader.js
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/server.js
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/stats.js
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/translation.js
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/js/upload.js
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.990911 comiclib-0.0.5/comiclib/LANraragi/public/themes/
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/themes/ex.css
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/themes/g.css
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/themes/modern.css
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/themes/modern_clear.css
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/public/themes/modern_red.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.994911 comiclib-0.0.5/comiclib/LANraragi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/backup
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/batch
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/category
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/config
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/edit
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/footer
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/index
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/login
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/logs
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/opds
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/opds_entry
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/plugins
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/reader
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/stats
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/LANraragi/templates/upload
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.998911 comiclib-0.0.5/comiclib/eHunter/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/eHunter/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   605811 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/eHunter/ehunter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)  1735387 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/eHunter/ehunter.mjs.map
--rw-r--r--   0 runner    (1001) docker     (127)    27792 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/eHunter/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/frontend_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.998911 comiclib-0.0.5/comiclib/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/10-zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/11-archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/20-ccloli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/21-hath.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/22-ehviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/23-xeHentai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/30-importEHdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/40-thumb.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-01-16 11:44:49.000000 comiclib-0.0.5/comiclib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:44:56.998911 comiclib-0.0.5/comiclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-16 11:44:56.000000 comiclib-0.0.5/comiclib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-16 11:44:49.000000 comiclib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 11:44:56.998911 comiclib-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.926773 comiclib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 15:12:44.000000 comiclib-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-31 15:12:47.926773 comiclib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-31 15:12:44.000000 comiclib-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.906773 comiclib-0.0.6/comiclib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.906773 comiclib-0.0.6/comiclib/LANraragi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.906773 comiclib-0.0.6/comiclib/LANraragi/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.906773 comiclib-0.0.6/comiclib/LANraragi/public/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/css/config.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/css/lrr.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.910773 comiclib-0.0.6/comiclib/LANraragi/public/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47884 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/flubbed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   390286 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55876 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/noThumb.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132249 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/notfound.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.910773 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/hachikuji.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/hverse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/nadeko.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/sadpanda.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/yotsugi.png
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/img/wait_warmly.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.918773 comiclib-0.0.6/comiclib/LANraragi/public/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/backup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/batch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/category.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/index_datatables.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36364 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   805177 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36369 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder_simd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   792814 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder_simd.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/logs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/plugins.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31178 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/reader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/server.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/stats.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/translation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/js/upload.js
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.918773 comiclib-0.0.6/comiclib/LANraragi/public/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/themes/ex.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/themes/g.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/themes/modern.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/themes/modern_clear.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/public/themes/modern_red.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.922773 comiclib-0.0.6/comiclib/LANraragi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/backup
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/batch
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/category
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/config
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/edit
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/footer
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/index
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/login
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/logs
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/opds
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/opds_entry
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/plugins
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/reader
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/stats
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/LANraragi/templates/upload
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.926773 comiclib-0.0.6/comiclib/eHunter/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/eHunter/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   605811 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/eHunter/ehunter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)  1735387 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/eHunter/ehunter.mjs.map
+-rw-r--r--   0 runner    (1001) docker     (127)    27792 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/eHunter/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/frontend_boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.926773 comiclib-0.0.6/comiclib/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/10-zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/11-archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/20-ccloli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/21-hath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/22-ehviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/23-xeHentai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/30-importEHdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/40-thumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-31 15:12:44.000000 comiclib-0.0.6/comiclib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:12:47.926773 comiclib-0.0.6/comiclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:12:47.000000 comiclib-0.0.6/comiclib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-31 15:12:44.000000 comiclib-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:12:47.926773 comiclib-0.0.6/setup.cfg
```

### Comparing `comiclib-0.0.5/LICENSE` & `comiclib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/PKG-INFO` & `comiclib-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comiclib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Manage, read and share your comic/manga library
 Author: URenko
 Project-URL: Homepage, https://github.com/comiclib/comiclib
 Project-URL: Bug Tracker, https://github.com/comiclib/comiclib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `comiclib-0.0.5/README.md` & `comiclib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/COPYING` & `comiclib-0.0.6/comiclib/LANraragi/COPYING`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/css/config.css` & `comiclib-0.0.6/comiclib/LANraragi/public/css/config.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/css/lrr.css` & `comiclib-0.0.6/comiclib/LANraragi/public/css/lrr.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/flubbed.gif` & `comiclib-0.0.6/comiclib/LANraragi/public/img/flubbed.gif`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/logo.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/logo.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/noThumb.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/noThumb.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/notfound.jpg` & `comiclib-0.0.6/comiclib/LANraragi/public/img/notfound.jpg`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/hachikuji.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/hachikuji.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/hverse.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/hverse.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/nadeko.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/nadeko.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/sadpanda.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/sadpanda.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/theme_preview/yotsugi.png` & `comiclib-0.0.6/comiclib/LANraragi/public/img/theme_preview/yotsugi.png`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/img/wait_warmly.jpg` & `comiclib-0.0.6/comiclib/LANraragi/public/img/wait_warmly.jpg`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/backup.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/backup.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/batch.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/batch.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/category.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/category.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/common.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/common.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/config.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/config.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/edit.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/edit.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/index.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/index.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/index_datatables.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/index_datatables.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.min.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.min.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.wasm` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.wasm`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder.worker.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder.worker.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder_simd.min.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder_simd.min.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/jxl_decoder_simd.wasm` & `comiclib-0.0.6/comiclib/LANraragi/public/js/jxl_decoder_simd.wasm`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/logs.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/logs.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/plugins.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/plugins.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/reader.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/reader.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/server.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/server.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/stats.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/stats.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/translation.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/translation.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/js/upload.js` & `comiclib-0.0.6/comiclib/LANraragi/public/js/upload.js`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/themes/ex.css` & `comiclib-0.0.6/comiclib/LANraragi/public/themes/ex.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/themes/g.css` & `comiclib-0.0.6/comiclib/LANraragi/public/themes/g.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/themes/modern.css` & `comiclib-0.0.6/comiclib/LANraragi/public/themes/modern.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/themes/modern_clear.css` & `comiclib-0.0.6/comiclib/LANraragi/public/themes/modern_clear.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/public/themes/modern_red.css` & `comiclib-0.0.6/comiclib/LANraragi/public/themes/modern_red.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/backup` & `comiclib-0.0.6/comiclib/LANraragi/templates/backup`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/batch` & `comiclib-0.0.6/comiclib/LANraragi/templates/batch`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/category` & `comiclib-0.0.6/comiclib/LANraragi/templates/category`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/config` & `comiclib-0.0.6/comiclib/LANraragi/templates/config`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/edit` & `comiclib-0.0.6/comiclib/LANraragi/templates/edit`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/index` & `comiclib-0.0.6/comiclib/LANraragi/templates/index`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/login` & `comiclib-0.0.6/comiclib/LANraragi/templates/login`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/logs` & `comiclib-0.0.6/comiclib/LANraragi/templates/logs`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/opds` & `comiclib-0.0.6/comiclib/LANraragi/templates/opds`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/opds_entry` & `comiclib-0.0.6/comiclib/LANraragi/templates/opds_entry`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/plugins` & `comiclib-0.0.6/comiclib/LANraragi/templates/plugins`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/reader` & `comiclib-0.0.6/comiclib/LANraragi/templates/reader`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/stats` & `comiclib-0.0.6/comiclib/LANraragi/templates/stats`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/LANraragi/templates/upload` & `comiclib-0.0.6/comiclib/LANraragi/templates/upload`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/config.py` & `comiclib-0.0.6/comiclib/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     password: Union[str, None] = None
     skip_exits: bool = True
     watch: bool = True
     display_title_format: Optional[str] = None
     display_subtitle: Optional[bool] = None
     UA_convert_jxl: str = 'Android'
     UA_convert_all: str = r'\b\B'  # default: match nothing
+    skip_scan_error: bool = False
 
 settings = Settings()
 
 if settings.debug:
     settings.loglevel = 'DEBUG'
 numeric_level = getattr(logging, settings.loglevel.upper(), None)
 if not isinstance(numeric_level, int):
```

### Comparing `comiclib-0.0.5/comiclib/database.py` & `comiclib-0.0.6/comiclib/database.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/eHunter/ehunter.mjs` & `comiclib-0.0.6/comiclib/eHunter/ehunter.mjs`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/eHunter/ehunter.mjs.map` & `comiclib-0.0.6/comiclib/eHunter/ehunter.mjs.map`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/eHunter/style.css` & `comiclib-0.0.6/comiclib/eHunter/style.css`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/frontend_boost.py` & `comiclib-0.0.6/comiclib/frontend_boost.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/main.py` & `comiclib-0.0.6/comiclib/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 print(f" >>> ComicLib v{__version__}")
 
 from .scan import watch, scannow
 from .config import settings
 from .utils import is_image, extract_thumbnail, convert_image, ArchiveFile, ordered
 from typing import Union, Annotated
 from enum import Enum
```

### Comparing `comiclib-0.0.5/comiclib/scan.py` & `comiclib-0.0.6/comiclib/scan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import importlib
 import itertools
 import os
 import sys
 import copy
 import hashlib
 import time
+import traceback
 from pathlib import Path
 from pprint import pformat
 
 import logging
 logger = logging.getLogger(__name__)
 
 from .database import engine, Base, Archive, Tag, Category
@@ -31,19 +32,22 @@
 scanners = [(importlib.import_module('.scanner.'+name, __package__).Scanner(), name) for name in scanner.__all__] + \
           [(importlib.import_module(p.stem).Scanner(), p.stem) for p in Path('.').glob('*.py')]
 scanners.sort(key=lambda t:t[1])
 logger.info(f"Loaded scanners: {[scanner[1] for scanner in scanners]}")
 
 
 def scan(paths):
+    exceptions = Exception if settings.skip_scan_error else ()
+    errors = {}
     with Session(engine) as db:
         try:
             for p in paths:
                 checkpoint = db.begin_nested()
                 try:
+                    name = None
                     p = Path(os.path.relpath(p, settings.content))
                     if p.is_relative_to('thumb'):
                         continue
                     old_a = db.scalar(select(Archive).where(
                         Archive.path == p.as_posix()))
                     if old_a is None:
                         a = Archive(path=p.as_posix())
@@ -55,18 +59,19 @@
                         archive_id = old_a.id
                     metadata = {"id": archive_id, "title": a.title, "subtitle": a.subtitle, "source": a.source, "pagecount": a.pagecount, "tags": set(
                         t.tag for t in a.tags if not t.tag.startswith("date_added:")), "categories": set(c.name for c in a.categories)}
                     real_path = Path(settings.content) / p
                     prev_scanners = []
                     for scanner, name in scanners:
                         prev_metadata = copy.deepcopy(metadata)
-                        if scanner.scan(real_path, archive_id, metadata, prev_scanners):
+                        if scanner.scan(path=real_path, id=archive_id, metadata=metadata, prev_scanners=prev_scanners):
                             prev_scanners.append(name)
                         else:
                             metadata = prev_metadata
+                    name = 'post_process'
                     if not prev_scanners:
                         continue
                     if not any(tag.startswith("date_added:") for tag in metadata["tags"]):
                         # Directory modification times are often difficult to synchronize.
                         mtime_path = next(real_path.iterdir()) if real_path.is_dir() else real_path
                         metadata["tags"].add(f"date_added:{int(mtime_path.stat().st_mtime)}")
                     logging.debug(pformat(metadata))
@@ -87,19 +92,24 @@
                             db.add(c)
                         a.categories.append(c)
                     if old_a is None:
                         assert len(metadata["id"]) == 40, f'The length of ID {metadata["id"]} is incorrect.'
                         a.id = metadata["id"]
                         db.add(a)
                     checkpoint.commit()
+                except exceptions:
+                    logger.error(traceback.format_exc())
+                    errors[str(p)] = name
                 finally:
                     if checkpoint.is_active:
                         checkpoint.rollback()
         finally:
             db.commit()
+            if settings.skip_scan_error and errors:
+                logger.error('Processing failed while scanning the following files:\n%s', pformat(errors))
 
 def get_files_inuse():
     ret = set()
     for proc in psutil.process_iter():
         try:
             ret |= {f.path for f in proc.open_files()}
         except (psutil.AccessDenied, psutil.NoSuchProcess):
```

### Comparing `comiclib-0.0.5/comiclib/scanner/10-zip.py` & `comiclib-0.0.6/comiclib/scanner/10-zip.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/scanner/11-archive.py` & `comiclib-0.0.6/comiclib/scanner/11-archive.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/scanner/20-ccloli.py` & `comiclib-0.0.6/comiclib/scanner/20-ccloli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,14 @@
             metadata["subtitle"] = info[1]
             metadata["id"] = f"EH{m[1]:>018}{m[2]}{id[-10:]}"
             line_tags = False
             for line in info:
                 if line.startswith("Category: "): metadata["categories"].add(line.removeprefix("Category: "))
                 elif line_tags:
                     if line.startswith("> "):
-                        namespace, _, names = line.removeprefix("> ").replace("：", ":").partition(':')
+                        namespace, _, names = line.removeprefix("> ").replace("：", ":", 1).partition(':')
                         for name in names.split(","):
                             metadata["tags"].add(f"{namespace}:{name.strip()}")
                     else:
                         line_tags = False
                 elif line == "Tags:": line_tags = True
             return True
```

### Comparing `comiclib-0.0.5/comiclib/scanner/21-hath.py` & `comiclib-0.0.6/comiclib/scanner/21-hath.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/scanner/22-ehviewer.py` & `comiclib-0.0.6/comiclib/scanner/22-ehviewer.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/scanner/23-xeHentai.py` & `comiclib-0.0.6/comiclib/scanner/23-xeHentai.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/scanner/30-importEHdb.py` & `comiclib-0.0.6/comiclib/scanner/30-importEHdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,43 @@
 logger = logging.getLogger(__name__)
 
 def blur_title(title: str):
     if not isinstance(title, str):
         return title
     if settings.importEHdb_matchtitle == 'exact':
         return title
-    return title.translate(str.maketrans({
+    # also restrict to Basic Multilingual Plane
+    return ''.join(map(lambda c:c if ord(c) <= 0xFFFF else '_', title)).translate(
+        str.maketrans({
         ' ': None,
-        '*': None,
         '_': None,
         '(': None,
         ')': None,
         ':': None,
-        '+': None
+        '：': None,
+        '"': None,
+        '＂': None,
+        '*': None,
+        '＊': None,
+        '?': None,
+        '？': None,
+        '|': None,
+        '｜': None,
+        '<': None,
+        '＜': None,
+        '>': None,
+        '＞': None,
+        '/': None,
+        '／': None,
+        '\\': None,
+        '＼': None,
     }))
 
 # Please update the version once the above function is updated.
-blur_title_version = 1
+blur_title_version = 3
 title2gid_table = 'gallery' if settings.importEHdb_matchtitle == 'exact' else f'comiclib_title2gid_v{blur_title_version}'
 title2gid_index = 'gallery_title' if settings.importEHdb_matchtitle == 'exact' else f'title_index_v{blur_title_version}'
 titlejpn2gid_table = f"comiclib_titlejpn2gid_v{0 if settings.importEHdb_matchtitle == 'exact' else blur_title_version}"
 titlejpn2gid_index = f"titlejpn_index_v{0 if settings.importEHdb_matchtitle == 'exact' else blur_title_version}"
 # The title_jpn field in table galley contains many NULL, thus use table titlejpn_index_v0 for index instead here.
 
 def dict_factory(cursor, row):
@@ -47,14 +64,17 @@
     '''Import the dumped e-hentai metadata database api_dump.sqlite (you can download it from https://sukebei.nyaa.si/user/gipaf23445).
 Currently only support matching by the source URL (from previous scanners).'''
     
     def __init__(self) -> None:
         db_path = urlsplit(settings.importEHdb_database_URI).path
         if Path(db_path).exists():
             self.con = sqlite3.connect(settings.importEHdb_database_URI, uri=True, check_same_thread=False)
+            # Check if the database is out of date
+            if self.con.execute("SELECT posted FROM gallery INDEXED BY gallery_posted ORDER BY posted DESC LIMIT 1").fetchone()[0] < 1705903491:
+                logger.warning("There is a new version of api_dump.sqlite, you can download it from https://sukebei.nyaa.si/user/gipaf23445")
             # Build cache during the first run
             if settings.importEHdb_matchtitle:
                 req_title2gid_index = self.con.execute(f"SELECT name FROM sqlite_master WHERE type='index' AND name=?", (title2gid_index,)).fetchone() is None
                 req_titlejpn2gid_index = self.con.execute(f"SELECT name FROM sqlite_master WHERE type='index' AND name=?", (titlejpn2gid_index,)).fetchone() is None
                 if req_title2gid_index or req_titlejpn2gid_index:
                     logger.info('Building ehentai database title cache, please wait...')
                     if req_title2gid_index:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `comiclib-0.0.5/comiclib/scanner/40-thumb.py` & `comiclib-0.0.6/comiclib/scanner/40-thumb.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib/utils.py` & `comiclib-0.0.6/comiclib/utils.py`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/comiclib.egg-info/PKG-INFO` & `comiclib-0.0.6/comiclib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comiclib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Manage, read and share your comic/manga library
 Author: URenko
 Project-URL: Homepage, https://github.com/comiclib/comiclib
 Project-URL: Bug Tracker, https://github.com/comiclib/comiclib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `comiclib-0.0.5/comiclib.egg-info/SOURCES.txt` & `comiclib-0.0.6/comiclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comiclib-0.0.5/pyproject.toml` & `comiclib-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "comiclib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="URenko" },
 ]
 description = "Manage, read and share your comic/manga library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

