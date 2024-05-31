# Comparing `tmp/webinspectra-1.0.1.tar.gz` & `tmp/webinspectra-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webinspectra-1.0.1.tar", last modified: Thu May 30 17:13:45 2024, max compression
+gzip compressed data, was "webinspectra-1.0.2.tar", last modified: Thu May 30 17:43:32 2024, max compression
```

## Comparing `webinspectra-1.0.1.tar` & `webinspectra-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,3614 @@
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    35157 2024-05-29 19:56:36.000000 webinspectra-1.0.1/LICENSE
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      165 2024-05-30 16:44:15.000000 webinspectra-1.0.1/MANIFEST.in
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:13:45.220967 webinspectra-1.0.1/PKG-INFO
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6383 2024-05-29 21:01:19.000000 webinspectra-1.0.1/README.md
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/WebInspectra.egg-info/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/PKG-INFO
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      468 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/SOURCES.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        1 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/dependency_links.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      105 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/requires.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       13 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/top_level.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       38 2024-05-30 17:13:45.220967 webinspectra-1.0.1/setup.cfg
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-05-30 16:44:58.000000 webinspectra-1.0.1/setup.py
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.216967 webinspectra-1.0.1/tests/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-27 19:54:40.000000 webinspectra-1.0.1/tests/__init__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-05-29 18:21:09.000000 webinspectra-1.0.1/tests/test_webinspectra.py
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/webinspectra/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       64 2024-05-29 18:06:56.000000 webinspectra-1.0.1/webinspectra/__init__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      984 2024-05-29 19:57:07.000000 webinspectra-1.0.1/webinspectra/__main__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18871 2024-05-29 19:57:27.000000 webinspectra-1.0.1/webinspectra/inspectra.py
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/webinspectra/utils/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 16:38:14.000000 webinspectra-1.0.1/webinspectra/utils/__init__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3312 2024-04-17 19:29:48.000000 webinspectra-1.0.1/webinspectra/utils/selenium_utils.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6701 2024-05-27 19:29:48.000000 webinspectra-1.0.1/webinspectra/utils/signature_utils.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9060 2024-05-27 19:30:04.000000 webinspectra-1.0.1/webinspectra/webpage.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.945020 webinspectra-1.0.2/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    35157 2024-05-29 19:56:36.000000 webinspectra-1.0.2/LICENSE
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      253 2024-05-30 17:40:58.000000 webinspectra-1.0.2/MANIFEST.in
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:43:32.945020 webinspectra-1.0.2/PKG-INFO
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6383 2024-05-29 21:01:19.000000 webinspectra-1.0.2/README.md
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.941020 webinspectra-1.0.2/WebInspectra.egg-info/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:43:32.000000 webinspectra-1.0.2/WebInspectra.egg-info/PKG-INFO
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   135844 2024-05-30 17:43:32.000000 webinspectra-1.0.2/WebInspectra.egg-info/SOURCES.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        1 2024-05-30 17:43:32.000000 webinspectra-1.0.2/WebInspectra.egg-info/dependency_links.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      105 2024-05-30 17:43:32.000000 webinspectra-1.0.2/WebInspectra.egg-info/requires.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       13 2024-05-30 17:43:32.000000 webinspectra-1.0.2/WebInspectra.egg-info/top_level.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       38 2024-05-30 17:43:32.945020 webinspectra-1.0.2/setup.cfg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-05-30 17:42:54.000000 webinspectra-1.0.2/setup.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.353020 webinspectra-1.0.2/tests/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-27 19:54:40.000000 webinspectra-1.0.2/tests/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-05-29 18:21:09.000000 webinspectra-1.0.2/tests/test_webinspectra.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.353020 webinspectra-1.0.2/webinspectra/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       64 2024-05-29 18:06:56.000000 webinspectra-1.0.2/webinspectra/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      984 2024-05-29 19:57:07.000000 webinspectra-1.0.2/webinspectra/__main__.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.353020 webinspectra-1.0.2/webinspectra/data/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10233 2024-03-25 22:11:08.000000 webinspectra-1.0.2/webinspectra/data/categories.json
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.937020 webinspectra-1.0.2/webinspectra/data/icons/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    57348 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/.DS_Store
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1306 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/1C-Bitrix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2497 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/24nettbutikk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5157 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/2badvice.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2276 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/30namaPlayer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      781 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/33Across.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      937 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/34SP.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/4-Tell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17824 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/42stores.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/4Partners.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      672 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/51.LA.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      770 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/5centsCDN.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      976 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/6sense.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/8base.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/A-Frame.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1083 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/A8.net.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3023 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AB Tasty.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ABOUT YOU Commerce Suite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ADAPT.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      659 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ADFOX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1594 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AFThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4585 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AIOSEO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      493 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ALL-INKL.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ANDCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      473 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AOLserver.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      431 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AOS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      803 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/APC.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1083 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ARI Network Services.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AT Internet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1382 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ATSHOP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AWIN.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2425 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AWS Certificate Manager.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AWS WAF Captcha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AWStats.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Absorb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      649 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accelerated-Mobile-Pages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1082 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accentuate Custom Fields.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      502 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AccessTrade.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AccessiBe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1409 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accessibility Toolbar Plugin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2486 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accessible360.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3448 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accessibly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5753 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Accesso.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1577 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Acconsento.click.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1362 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AccuWeather.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ace.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1313 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ackee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Acoustic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Acquire.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3067 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Act-On.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1760 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ActBlue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1017 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Actito.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ActiveCampaign.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Acuity Scheduling.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      470 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AcuityAds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ad Lightning.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2093 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdBridg.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1361 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdInfinity.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1155 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdOcean.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2488 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdOpt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdRiver.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      450 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdRoll.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1232 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdScale.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1053 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdThrive.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ada.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3118 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdaSiteCompliance.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adabra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      755 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adally.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adalyser.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1501 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adcash.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      866 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AddEvent.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AddShoppers.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AddThis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      574 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AddToAny.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      797 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Addsearch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adjust.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adloox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1320 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Admiral.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Admitad.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Admixer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      880 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Admo.tv.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      818 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adnegah.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe Analytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe ColdFusion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4697 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe Experience Manager Franklin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1803 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe Experience Platform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe Flash.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      374 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe GoLive.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe Portfolio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe RoboHelp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      592 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adobe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1334 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdobeMuse.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AdonisJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Advally.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1564 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Advanced Custom Fields.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1397 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Advert Stream.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      472 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adverticum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      831 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Adyen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2669 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aegea.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2287 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aero Commerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1602 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affilae.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2251 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affiliate B.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1506 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affiliate Future.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      827 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affiliatly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affilio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1071 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affilo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1172 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Affirm.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Afosto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1211 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AfterBuy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AfterSell.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2751 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AfterShip Returns Center.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2689 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AfterShip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2265 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AiSpeed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1430 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aimtell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2076 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Air360.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AirRobe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      485 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Airee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1918 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Airform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20463 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Airship.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Airtable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      997 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Akamai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2109 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Akilli Ticaret.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      714 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Akismet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aklamio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   117872 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aksara CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5622 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Albacross.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      773 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlertifyJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5461 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alexa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1751 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Algolia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alibaba Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alireviews.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1693 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alli.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alliance Auth.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlloyUI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1524 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Allyable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlmaLinux.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2045 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alpine Linux.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2953 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Alpine.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1073 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlternC.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      149 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlumnIQ.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6957 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AlvandCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      454 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amaya.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2773 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Aurora.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2810 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon CloudWatch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Cloudfront.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Cognito.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1984 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon EC2.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2223 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon ECS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon EFS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    26825 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon ELB.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4344 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Pay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2580 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon S3.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3062 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon SES.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Web Services.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15863 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon Webstore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2951 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amazon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1185 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ambassador.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      567 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ametys.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8938 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amex.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1711 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amiro.CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      489 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amobee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1572 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amplience.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5797 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Amplitude.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2973 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Analysys Ark.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2683 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Analyzee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1234 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AndersNoren.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1709 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Anetwork.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      483 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Angular.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AngularDart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      733 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AngularJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7788 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Animate.css.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      870 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aniview.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      818 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AnswerDash.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4729 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ant Design.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7040 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AntV.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1267 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Antee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      472 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Anthology.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1059 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Antsomi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7173 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AnyClip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apache APISIX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apache Tomcat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4564 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apache Traffic Server.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1186 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apache Wicket.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11125 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apache.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1549 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apereo CAS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1853 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ApexChat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4003 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apigee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apisearch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aplazame.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apollo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      854 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apollo13Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ApostropheCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2220 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AppDynamics.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1359 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AppNexus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      415 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Appcues.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      771 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Appian.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1717 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apple.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1300 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ApplicantStack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      720 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Appointy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1437 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Appsflyer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5447 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Apptus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Appwrite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1176 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aprimo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1720 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AptusShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AquilaCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1146 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Arastta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Arc XP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Arc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ArcoDesign.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Arena.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Arreva.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Artifactory.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    26383 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aruba.it.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ArvanCloud.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Asana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AsciiDoc.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Asciidoctor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      424 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Asciinema.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      783 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Asendia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1099 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Asgaros Forum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      641 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Assertive Yield.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1174 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Astra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1491 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Astro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3637 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Astute Solutions.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1526 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atatus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      862 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Athena Search.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atlassian Bitbucket.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1580 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atlassian Confluence.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      814 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atlassian FishEye.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atlassian Jira.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      946 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Atlassian Statuspage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1829 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Attentive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    25666 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Attraqt.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AudioEye.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1611 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Audiohook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aument.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3706 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aurelia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Auryc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      459 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AusPost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      623 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Auth0.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1054 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Autoketing.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Automatic.css.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1677 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Automizely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      371 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Autopilot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Autoptimize.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Avada.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Avangate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3000 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Avanser.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Avasize.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2683 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Avis Verifies.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3765 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Aweber.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Axeptio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      293 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Axios.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      247 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Azion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2355 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Azko CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1451 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Azoya.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3049 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Azure.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/AzureADB2C.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2341 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/B2C Europe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      128 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BEM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      617 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BIGACE.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8938 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BON Loyalty.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5524 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BRT.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BSmart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6158 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Babel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1832 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Babylist.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1322 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Back In Stock.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1525 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Backbone.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      330 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Backdrop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1310 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Baidu Maps.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Baidu Tongji.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1368 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BambooHR.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3068 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bambuser.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      430 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BandsInTown.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Banshee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      925 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Barba.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1739 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Barilliance.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16229 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Base.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1098 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Basis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Batflat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    55854 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bazaarvoice.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      818 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beam.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1390 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beamer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      944 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beans.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2551 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beehiiv.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1293 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beeketing.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      559 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beeswax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2042 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bentobox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1781 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Better Price.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1035 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Better Stack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1727 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BetterDocs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Betty Blocks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Beyable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1728 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BeyondMenu.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      647 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Big Cartel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2206 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BigCommerce B2B Edition.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1137 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BigCommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1282 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BigDataCloud-IPGeolocation.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      949 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BigTree CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bigin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      750 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bigware.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2928 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bikayi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2039 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Billbee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      831 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Binance.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1636 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Birdeye.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2272 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bitcoin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3016 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BiteSpeed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1289 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bitrix24.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      184 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BittAds.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2908 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blackbaud.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2127 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blade.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1156 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blazor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1633 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blessing Skin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1041 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blesta.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blitz.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1296 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blocksy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blogger.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1471 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bloomreach.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1312 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blossom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blotout.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      366 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blue Triangle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      981 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BlueConic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2527 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bluecore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1871 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bluefish.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bluehost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1581 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blueknow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3130 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Blueshift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2340 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bluestone PIM.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6055 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Boats Group.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6559 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bobonus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      949 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BoidCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bokun.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2072 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bold Page Builder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bold Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      770 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bold.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      184 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BoldChat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bolt CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      199 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bolt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1994 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bonfire.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BookDinners.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1940 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BookStack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1551 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BookThatApp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1244 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BookVisit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      539 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bookafy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    21111 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bookatable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bookeo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1360 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bookero.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1615 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Booking.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bookingkit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   200358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Booksy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1641 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Boost Commerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1213 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BoosterApps.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bootic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bootstrap Icons.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      285 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bootstrap Table.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3175 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bootstrap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2913 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Booxi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      615 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Borderfree.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Borlabs Cookie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1748 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Botble-CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Boulevard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1987 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Boutiq.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1671 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BowNow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      806 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Boxtal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bpost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2795 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BrainSINS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      686 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Braintree.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1313 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Branch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2321 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Brandfolder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2220 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Braze.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1039 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bread.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1497 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Breadcrumb NavXT.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1064 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Breakdance.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1307 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Breinify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      240 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bricks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2038 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bricksite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2820 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bridgetown.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1004 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BrightEdge.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      814 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BrightInfo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1343 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Brightcove.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      732 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Brightspot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1728 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Brilliant Web-to-Lead.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Broadstreet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      270 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bronto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1664 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Brownie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1487 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Browser-Update.org.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      509 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BrowserCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1426 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bsale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      513 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Budbee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4401 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BuddyPress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BugHerd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      907 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BugSnag.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2438 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bugcrowd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      641 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bugzilla.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Builder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1051 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Buildertrend.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      244 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bulma.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      945 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bump.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4040 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bunny.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2919 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Business Catalyst.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3852 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Buttonizer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6477 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Buy me a coffee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BuySellAds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      839 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Buyapowa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/BySide.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1227 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Bynder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1655 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/C.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3047 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CDK Global.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1983 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CDN77.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      824 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CEMax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      310 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CFML.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3490 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CJDropshipping.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      712 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CKEditor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1168 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CMS Made Simple.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CPABuild.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CPG Dragonfly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CRM+.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CS Cart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6573 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CSSIgniter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1163 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CTT.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1693 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Caast.tv.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2110 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CacheFly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1148 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cachet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CactiveCloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      502 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cafe24.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1660 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Caisy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      597 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CakePHP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1850 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Caldera Forms.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1159 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CalendarHero.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4386 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Calendly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CallRail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1557 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CallTrackingMetrics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Callbell.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      880 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Campaign Monitor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Candid Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Canny.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Canto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2881 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Canva.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6643 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Canvas LMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      192 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Captch Me.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3170 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Captivate.fm.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    26381 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Carbon Ads.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2173 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CareCart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2272 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cargo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2247 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Carrd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1225 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Carro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3515 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Carrot quest.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      722 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cart-generic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5526 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cart.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1681 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cart.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2528 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CartKit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CartStack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Carts Guru.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1552 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Catberry.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1402 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Catch Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      911 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Catch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cecil.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1065 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Celeritas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1232 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Celum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    24473 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Censhare.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    29873 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CentOS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      836 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Centra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2903 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chabokan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      879 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chakra UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chameleon system.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1069 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chameleon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chamilo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1331 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Channel.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1076 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChannelAdvisor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2567 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChannelApe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2004 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chaport.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChargeAfter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6939 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chargebee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      783 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chart.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chartbeat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChatStack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1361 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChatWith.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chatango.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1751 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chatbase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1827 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chatra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      698 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chatwoot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Checkfront.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Checkly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      864 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Checkout.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4732 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chekkit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      635 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cherokee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CherryPy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1997 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chevereto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9748 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chicago Boss.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1162 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chili Piper.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chinese Menu Online.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1169 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chitika.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      574 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Choices.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chord.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chorus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Chronopost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      968 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ChurnZero.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      897 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ciklik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1097 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Circle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1424 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/City Hive.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4077 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CityMail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1692 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CiviCRM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      361 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ckan.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      887 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clarip.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Claris.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   188901 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Classeh.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2464 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClearSale.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3602 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clearbit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clerk.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2550 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clerk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1409 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CleverTap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cleverbridge.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2081 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Click & Pledge.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5974 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClickCease.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1221 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClickDimensions.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5520 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClickFunnels.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      434 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClickHeat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1153 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClickTale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2898 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clickbank.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1869 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clicky.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2642 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClientJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1387 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClientXCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      242 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clinch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      524 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Clipboard.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6066 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CloudCannon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1067 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CloudFlare.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2676 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CloudSuite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1611 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudbeds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      697 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudera.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5088 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudflare Workers.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      897 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudify.store.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20441 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudimage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4598 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudinary.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudrexx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      819 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloudways.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3715 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cloverly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cluep.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10882 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ClustrMaps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      840 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoConstruct.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2425 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoRover.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2039 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cococart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3975 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoconutSoftware.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2130 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cocos2d.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CodeIgniter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      179 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CodeMirror.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      258 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CodeSandbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Coin Currency Converter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoinHive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1220 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Coinbase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      310 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Colibri WP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      859 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Colis Prive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Colorlib.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Combahton.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Combeenation.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Combodo iTop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1340 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Comm100.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2329 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Commanders Act.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Commerce Server.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1159 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Commerce7.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Community Funded.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2082 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Complianz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Concrete CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1306 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Conekta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Confer With.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1490 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Conferbot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2488 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Confiant.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Congressus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Conjured.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Connectif.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2031 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Constant Contact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2760 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contabo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3158 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contact Form 7.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1986 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Container Media Group.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1134 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contao.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      205 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contenido.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contensis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ContentBox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1339 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ContentStudio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      923 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contentful.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contently.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contentsquare.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10132 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contentstack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      651 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Contlo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1105 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Conversant.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Conversio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Convert.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2042 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ConvertFlow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ConvertKit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      898 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Convertcart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Convertr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2057 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Convertri.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      806 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ConveyThis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      997 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cookie Information.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      809 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cookie Notice.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1294 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cookie Seal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1462 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CookieFirst.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1612 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CookieHub.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2359 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CookieScript.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cookiebot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19150 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cooladata.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      220 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Coppermine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3405 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Copypoison.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cordial.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoreMedia Content Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1566 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoreUI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1639 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Corebine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Correos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      236 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cosmoshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      520 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cotonti.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CouchDB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Countly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Coureon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      598 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Coveo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20198 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CoverManager.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Covet.pics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2871 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cowboy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2779 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cozy AntiTheft.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2850 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CppCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Craft CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Craftum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      257 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cratejoy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crazy Egg.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crealive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CreateJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1197 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Creatium.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1305 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Creativ.eMail.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crikle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crisp Live Chat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      386 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Criteo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1584 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crobox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      591 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crocoblock.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cross Pixel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2226 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CrossBox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      622 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CrossSell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      582 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CrownPeak.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2609 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cryout Creations.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      458 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crypto-Loot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      568 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Crystallize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      734 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CubeCart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      312 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cubyn.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2513 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cufon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      902 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Custom Fonts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1701 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Customer.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2953 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Customily.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1544 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cwicly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Cxense.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2594 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/CyberChimps.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Czater.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1328 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/D3.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      716 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DDoS-Guard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1056 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DHL.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      345 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DHTMLX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1216 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DM Polopoly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      657 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DNN.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DPD.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DPlayer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DTScout.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1708 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DX1.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dachser.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2400 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Daily Deals.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1874 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DailyKarma.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dailymotion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1127 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DanDomain.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      794 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dancer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Danneo CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2292 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2001 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DataDome.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DataLife Engine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1572 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DataMilk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2667 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DataPower.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2922 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DataTables.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5338 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Datadog.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7187 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Datatrics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      693 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DatoCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3634 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Day.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dealer Spike.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Debian.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1109 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Decibel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      834 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DedeCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Delacon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      974 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Deliverr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2381 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Depict.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2030 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DerakCloud.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DeskPro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4576 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Detectify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1022 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Deutsche Post.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      521 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Devisto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1295 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DiamondCDN.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dianomi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1095 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DigiCert.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18847 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DigiFi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      564 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Digismoothie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    69367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Digistore24.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      247 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Digital Factory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1584 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Digital Showroom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DigitalOcean.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16835 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DigitalRiver.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1335 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Digizuite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      389 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DirectAdmin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3214 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Directus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1916 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Discourse.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2282 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Discuz X.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      596 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Disqus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      736 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/District M.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dito.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      511 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Divhunt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    31445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Divi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1227 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DivideBuy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Divido.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1442 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Django CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      529 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Django.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13403 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DocFX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1446 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DocSearch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10478 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Docker.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Docsify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      563 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DocuSign.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      247 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dojo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6722 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dokan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      644 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dokeos.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2944 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DokuWiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      578 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DomainFactory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1045 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dominate.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DonorPerfect.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2293 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Donorbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3253 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Doofinder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      811 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Doppler.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      992 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DorikAI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      247 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dotclear.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   356122 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dotdigital.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Doteasy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1603 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dotser.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DoubleClick.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1592 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DoubleVerify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1210 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dovetale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Download Monitor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      115 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Doxygen.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Draftpress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1154 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dragon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2413 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drapr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DreamApply.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      865 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DreamHost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      649 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DreamWeaver.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dreamdata.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drift.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1395 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drop A Hint.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DropInBlog.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dropbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      986 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dropzone.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Droxit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      714 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Droz.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1716 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drubbit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      830 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drupal Commerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1736 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Drupal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      917 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Duda.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      701 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Duel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1091 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dukaan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1052 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Duopana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1551 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/DynamicYield.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1052 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dynamicweb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2486 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dynatrace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      401 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Dyte.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4139 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/E-Com Plus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1111 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/E-monsite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      820 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EC-CUBE.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      817 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EKM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      203 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ELOG.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      651 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EPrints.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      355 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ERPNext.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1423 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ESW.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1253 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EWWW Image Optimizer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EX.CO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1772 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Easy Hide PayPal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1000 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Easy Orders.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Easy Redirects.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EasyDigitalDownloads.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2856 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EasyEngine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      786 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EasyGift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5529 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EasyStore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6903 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ebasnet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1420 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EcForce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ecovium.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EdgeCast.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   429538 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Edgio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1323 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Editor.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   176262 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Effector.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Effiliation.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Efilli.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1197 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eggplant.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6971 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ElasticAPM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ElasticSuite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1637 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elasticsearch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1319 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elcodi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1124 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eleanor CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ElementUI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2457 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elementor Header & Footer Builder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      817 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elementor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1995 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elevar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eleventy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1901 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elfsight.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4618 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Elixir.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ElkArte.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      905 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ellucian CRM Recruit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eloomi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EmailJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      397 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Emarsys.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3700 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ematic Solutions.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      629 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EmbedPlus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      955 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EmbedSocial.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Embedly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Embedthis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1735 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ember.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Emotion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1279 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Emotive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      625 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Empretienda.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1164 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Enable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1150 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Engagio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      642 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Enjin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1470 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Enlistly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ensi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Envialia.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      300 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Envo Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3553 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Envoy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1793 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Envybox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      197 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Enyo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      728 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Epom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2993 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EqualWeb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1425 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EraofEcom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Erlang.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1342 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Errorception.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2558 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Essent.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Essential Addons for Elementor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    22550 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EstoreCompare.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13806 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EstoreShopserve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      858 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ethers.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2715 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EthicalAds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1512 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eticex.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Etix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1234 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Etracker.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Etsy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      366 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Everflow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/EveryAction.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    21518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Eveve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2621 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Evidon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18449 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExactMetrics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1071 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Exemptify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      611 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Exhibit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1157 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExitIntel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1458 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExoClick.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1120 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExpertRec.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      766 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Expivi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Exponea.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1352 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Express.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExpressionEngine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1376 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExtJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ExtendThemes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1345 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Extole.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ezoic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2378 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/F5.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FAST ESP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      548 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FAST Search for SharePoint.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2070 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fabric.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1118 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Facebook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Facil-iti.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       92 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fact Finder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1187 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FalguniThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FameThemes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FancyBox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1805 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fanplayr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1437 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FaraPy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    36345 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FareHarbor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      919 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Farfetch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fast Bundle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      364 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fast Checkout.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      625 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FastComet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2731 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fastcommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1083 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fasterize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   465602 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fastly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fat-Free Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1048 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FatherShops.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fathom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1229 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fbits.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)  1007779 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FeatherX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2777 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Featurebase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1613 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FedEx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1173 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fedora.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      793 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Feefo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3067 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fenicio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2870 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fera.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1030 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Financeads.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6883 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Findify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      580 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Findmeashoe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fing.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1363 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FingerprintJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      717 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FintechOS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2570 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FireApps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5992 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Firebase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      739 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fireblade.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1459 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Firepush.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3661 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FirstHive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      937 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FirstImpression.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1957 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FirstPromoter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      710 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fit Analytics.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      779 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FlagSmith.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flask.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      702 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flat UI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2035 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flazio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1543 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fleksa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FlexCMP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      740 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FlexSlider.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2114 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FlippingBook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      834 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flits.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flocktory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1569 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flourish.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      567 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flowbite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flowplayer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1778 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flutter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FluxBB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1361 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fly.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4458 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flying Pages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6217 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FlyingPress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      350 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Flyspray.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      596 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fomo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      735 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Font Awesome.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      606 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FontServer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      947 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fontify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8371 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FooPlugins.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1677 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Food-Ordering.co.uk.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FoodBooking.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2622 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Foodomaa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3250 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Forethought Solve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      804 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fork Awesome.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1836 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ForkCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1950 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FormAssembly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      189 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FormBold.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1292 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Formaloo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Formidable Form.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      793 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Formitable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1192 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Formli.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5677 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ForoshGostar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    38934 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Forte.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4969 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Forter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      695 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fortinet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2307 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fortune3.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Four.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      433 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Foursixty.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      637 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fourthwall.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      250 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Framer Sites.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frames.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      950 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/France Express.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      283 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frappe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1630 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FraudLabs Pro.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FreakOut.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2512 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FreeBSD.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      657 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FreeTextBox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Freespee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frequently Bought Together.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fresh.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      963 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Freshchat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      616 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Freshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      830 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Freshteam.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2017 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Freshworks CRM.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Friendbuy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1099 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FriendlyCaptcha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4054 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frizbit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Froala.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1400 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Front Chat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      357 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FrontPage.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4391 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frontastic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3626 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frontify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      775 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Frosmo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FullCalendar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1093 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FullContact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1588 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FullStory.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fundiin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      620 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fundraise Up.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1344 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FunnelCockpit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2122 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Funnelforms.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1287 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Funnelish.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2474 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Funraise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/FurnitureDealer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      240 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fusion Ads.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1392 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Futurio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Fynd Platform.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9002 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GEODIS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2501 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GEOvendas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1282 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GLPI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GLS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3046 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GPT AI Power.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      687 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GTranslate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      681 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GX WebManager.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      596 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gallery.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      730 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gambio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gameball.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gatsby.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      156 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gauges.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1448 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gcore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GeeTest.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GemPages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      730 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gemius.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GeneXus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2359 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GenerateBlocks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      569 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Genesis theme.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Genesys Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1559 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Geniee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1910 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gentoo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Geo Targetly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Get Satisfaction.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1483 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetButton.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1038 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetFeedback.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetMeAShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      889 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetResponse.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      213 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetSimple CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1322 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetSocial.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      628 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GetYourGuide.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Getintent.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      578 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Getsitecontrol.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ghost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1054 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gigalixir.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      616 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gist.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GitBook.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2130 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GitHub.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      649 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GitLab CI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1395 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GitLab.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      924 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GiveCampus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2187 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GiveSmart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8203 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GiveWP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1085 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GivingFuel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gladly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GlassFish.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glassbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glide.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glider.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12591 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glitch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      733 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Global-e.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1430 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GlobalShopex.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Globo apps.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2391 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glofox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1165 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glopal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      251 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Glyphicons.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3454 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Go Instore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Go.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3047 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoAffPro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoAhead.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2321 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoCache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2154 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoCertify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2146 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoDaddy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5894 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5354 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoKwik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1904 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoMage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      787 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GoStats.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4181 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Godot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3013 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Goftino.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1762 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gomag.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1406 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google AdSense.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      706 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Ads.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      384 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Analytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      895 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google App Engine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      551 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Charts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2410 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Developers.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Font API.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1997 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Forms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1456 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Maps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      943 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Optimize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2528 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google PageSpeed.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2055 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Sites.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      975 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Tag Manager for WordPress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      906 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Tag Manager.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1116 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Wallet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1970 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google Web Toolkit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1018 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Google.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      621 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gorgias.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GotiPath.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5719 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Govalo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3186 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Grab.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9982 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Grafana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      385 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Graffiti CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7655 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GrandNode.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1809 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GrapesJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      626 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GraphCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1223 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GraphQL.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1256 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Graphene Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1210 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Grasp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Grav.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1243 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gravatar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1427 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gravitec.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2051 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GreatPages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      330 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Green Valley CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2105 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Greenhouse.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1733 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Griddo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2856 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gridsome.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Grin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      854 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GrocerKey.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Groupby.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Growave.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GrowingIO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    21870 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Guestonline.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GuideIT.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1586 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/GumGum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      715 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gumlet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gumroad.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      539 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gumstack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2362 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Gutenberg.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2002 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HCL Commerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      529 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HCL Domino.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1006 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HHVM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      719 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2151 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HTTP2.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2053 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HTTP3.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1581 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Halo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3322 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hamechio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2022 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hammer.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9708 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Handlebars.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Handtalk.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hansel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      731 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Happy Returns.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      692 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HappyFox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Haptik.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9434 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Haravan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6297 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Harbor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1464 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HashThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      558 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hashtag Labs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Haskell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2598 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hasura.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3152 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hatena.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1285 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HeadJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)  1035130 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Header Bidding Ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2831 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Headless UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      305 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Heap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    23026 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Heartland Payment Systems.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      926 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Helhost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HelixUltimate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1189 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Helixo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      322 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hello Bar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      617 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hello Elementor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      844 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Help Scout.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1868 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HelpDocs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4376 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hermes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1218 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hero.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1910 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HetrixTools.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      529 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hetzner.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      361 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hexo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      866 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hextom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hi Platform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      493 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hiawatha.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2352 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HighLevel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Highcharts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      772 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Highlight.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2954 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HikeOrders.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1321 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hireology.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      257 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Histats.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hocalwire.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      869 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HockeyStack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hoefler&Co.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      365 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hogan.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3558 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Homerr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      824 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Homestead.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      456 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hono.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1424 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HostEurope.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3161 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostens.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    36642 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostgator.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      364 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hosting Ukraine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostinger.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1174 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostiq.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    69138 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostmeapp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      420 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hostpoint.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      599 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hotaru CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hotjar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12590 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Howler.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5862 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HrFlow.ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3044 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Htmx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HubSpot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hubalz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1412 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Huberway.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1252 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Huddle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1804 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hugo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/HulkApps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1467 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Humm.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    23131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hund.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      559 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hushly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hydra-Shield.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      940 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hydrogen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1178 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hyperspeed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      294 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hypervisual.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1263 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hypestyle CSS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      662 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hyros.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      710 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Hyva Themes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IBM.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14421 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ID5.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/INFOnline.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      506 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IONOS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1408 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IP2Location.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      217 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IPB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IPFS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IPInfoDB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1954 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IPinfo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2283 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ISAY.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      677 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Iamport.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1166 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ibexa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1165 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IconScout.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1039 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ideasoft.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Identrust.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      919 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ikas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      755 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Iluria.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4089 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Image Relay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3746 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ImageEngine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1426 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imagely.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imber.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1764 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imgix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Immutable.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Impact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imperva.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      408 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ImpressCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ImpressPages.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imunify360.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1414 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Imweb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      838 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/In Cart Upsell & Cross-Sell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1071 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InMoment.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1314 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InSyncai.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      335 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Inblog.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1025 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Incapsula.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1206 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Incident.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2193 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Includable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      457 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Index Exchange.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Indi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Indico.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      609 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Inertia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1149 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InfernoJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Infogram.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      753 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Infolinks.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      312 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Infomaniak.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Infoset.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Insider.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1913 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Insightly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1497 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instabot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1079 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instafeed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2847 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instant.page.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InstantCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1582 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InstantClick.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5528 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/InstantGeo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1252 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instapage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      883 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Instatus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2285 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Integral Ad Science.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      604 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Intel Active Management Technology.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2506 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Intelligems.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Intellimize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      717 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IntenseDebate.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Interact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Intercom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1081 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Internet Brands.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      952 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Intershop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1317 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Invenio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Inventrue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      795 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Inveon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1263 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Invoca.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1923 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ionic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ionicons.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1219 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/IrisLMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Isotope.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      982 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Issuu.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1688 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Iterable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      964 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Izooto.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      928 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JANet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      454 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JAlbum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1772 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JBoss Application Server.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1194 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JBoss Web.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1166 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JET Enterprise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      271 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JS Charts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      586 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JSEcoin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      892 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JSS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6679 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1414 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JTL Shop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2110 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JUST.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JW Player.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1154 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JahiaDX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      246 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jalios.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Java.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JavaScript Infovis Toolkit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      183 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JavaServer Faces.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3837 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jekyll.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2000 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jenkins.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jetpack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jetshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      672 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jetty.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      679 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jibres.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jilt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      758 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jimdo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jirafe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2093 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jitsi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jive.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      728 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JivoChat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jivox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      366 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JobAdder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      252 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JobberBase.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1073 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jobvite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3263 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JoomShopping.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3462 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Joomla.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4423 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JouwWeb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JsObservable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1441 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JsRender.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2031 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JsViews.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1136 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Judge.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2234 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/JuicyAds.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      983 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jumbo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1258 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jumio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16866 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Jumpseller.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/June.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      656 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Junip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1104 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Juo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      819 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Justo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Justuno.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      620 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/K2.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10858 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KAMAR.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KISSmetrics.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KMK.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1457 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KQS.store.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KaTeX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kadence WP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1104 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kaira.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kajabi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      363 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kakao.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kaltura.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1866 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kameleoon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9993 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kamva.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2602 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kapix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1253 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kapture CRM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Karma.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Karte.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      698 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kartra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1767 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kasada.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      538 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Keap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Keen Delivery.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1073 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KelonCloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      634 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kendo UI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2786 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kentico CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1044 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Keptify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      314 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ketch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3473 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kevel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1661 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KeyCDN.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7543 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Keybase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1225 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kibo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      800 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kicksite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2135 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kiliba.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kindful.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1176 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KineticJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      809 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kintone.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      698 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kirby.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      435 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kirki Customizer Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1066 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kitcart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1757 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kiwi Sizing.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1056 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klarna.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      902 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klaro.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      907 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klasha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      244 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klaviyo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klevu.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2152 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KlickPages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1227 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Klickly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      690 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Knak.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5894 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Knockout.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2443 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ko-fi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koa.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koala Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koala.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2900 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kobimaster.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1839 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kohana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1141 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koishi.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koken.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      214 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Komodo CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1329 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Konduto.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      862 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kong.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      956 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kontent.ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      475 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Koobi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1659 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kooboo CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kooomo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kosmos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1703 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kotisivukone.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kotlin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      784 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kount.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ktor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10937 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kubernetes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2600 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/KueskiPay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4236 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kustomer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1402 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Kwai.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LEPTON.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1000 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LGC.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LINE.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1804 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LKQD.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LOU.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/La Poste.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1164 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LandingPress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2767 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LangShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1780 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Laravel Echo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Laravel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2737 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LatitudePay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LaunchDarkly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Launchrock.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9438 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lawpay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1586 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LayBuy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1811 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LayoutHub.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Layui.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2138 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lazada.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4807 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LeadChat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      469 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LeadDyno.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      720 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leadfeeder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1353 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leadinfo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2314 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leadster.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1301 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leaflet platform.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leaflet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2320 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leanplum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LearnDash.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3450 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LearnWorlds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2539 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leaseweb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Legal Monster.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1330 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lemon Squeezy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lengow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lenis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3901 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Leptos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7594 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Less.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      278 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Letro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2134 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lets Encrypt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Levar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1036 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Level 5.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1477 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lever.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lexity.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Liberapay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2967 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lieferando.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1087 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Liferay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      734 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      684 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LightMon Engine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      158 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lightbox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1708 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lightning.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      510 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lightspeed.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LimeChat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1075 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LimeSpot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Limepay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Limit Login Attempts Reloaded.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2557 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Linen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1270 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Linguise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      149 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LinkMink.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      609 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Linkedin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1575 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Linx.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7823 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Liquid Web.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/List.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2264 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Listrak.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiteSpeed.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1528 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lithium.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1897 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Litmus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Littledata.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1517 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveAgent.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2309 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveCanvas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveChat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      892 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveHelp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      689 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveIntent.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveJournal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1961 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LivePerson.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveRamp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2316 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveSession.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveStory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      743 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveStreet CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LiveZilla.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Livefyre.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      633 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Liveinternet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      426 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Livescale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5563 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Livewire.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2060 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LlamaLink.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2163 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loadable-Components.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1564 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loadify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1245 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LocalFocus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Localised.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2256 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Locksmith.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LocomotiveCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lodash.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2103 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LogRocket.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loggly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LogiCommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1791 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LoginRadius.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loglib.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LogoiX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      933 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loja Integrada.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2446 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loja Mestre.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15001 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loja Virtual.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    22347 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loja2.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      795 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loop Web.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      265 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      850 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loop54.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1870 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lootly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1425 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      382 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Loqate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1515 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LottieFiles.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LoyaltyLion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1029 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lua.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      932 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Luana.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1585 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lucene.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      726 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lucide.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      832 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lucky Orange.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1421 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Luigisbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4490 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lume.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Luna.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1949 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/LyraThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      712 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Lytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      741 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MAAK.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MAJIN.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1116 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MDBootstrap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MDS Brand.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      965 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MDUI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      614 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MGID.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1141 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MGPanel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1768 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MIYN.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      659 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MODX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1936 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MRW.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MSHOP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1360 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MTCaptcha.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3803 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MUI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Macaron.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1144 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MachoThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MadAdsMedia.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2330 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MadCap Software.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2566 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Magazord.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      561 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MageWorx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      435 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Magento.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      662 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Magisto.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Magixite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      681 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Magnolia CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1342 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MailChimp for WordPress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2375 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MailerLite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      979 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mailgun.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      483 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mailjet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3550 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mailman.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mailmunch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1765 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MainAd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Make-Sense.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      301 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MakeShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MakeShopKorea.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1215 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Malomo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      763 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mambo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8935 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mangeznotez.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mantine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1851 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MantisBT.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ManyChat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ManyContacts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      750 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MapLibre.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1483 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mapbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1246 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mapp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mapplic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1497 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Maptalks.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19114 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marchex.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1837 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marfeel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marionette.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marked.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2101 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marker.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12181 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marketo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1009 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marketpath CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      656 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Marko.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      943 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mastercard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2330 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Masterking32.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1397 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mastodon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      832 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Matajer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      404 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Material Design Lite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2705 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Materialize CSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1051 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MathJax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    26524 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Matomo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      735 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MaxCDN.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      635 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MaxMind.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      772 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MaxSite CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Maxemail.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1650 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Measured.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      429 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Medallia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2791 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Media.net.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MediaElement.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19255 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MediaWiki.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2709 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mediavine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      520 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Medium.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      129 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Meebo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1251 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Meeting Scheduler.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Megagroup.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2509 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Meilisearch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      774 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MemberSpace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1126 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MemberStack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      274 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mention Me.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      998 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Menufy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8039 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mercado Shops.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      495 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MetaSlider.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1775 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Meteor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Methode.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5652 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Metrilo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      490 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mews.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft 365.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft ASP.NET.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    66972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft Clarity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3761 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft Excel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3581 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft PowerPoint.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3647 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft Publisher.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      753 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft SharePoint.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9374 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft Visual Studio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3112 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft Word.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      541 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Microsoft.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Miestro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1541 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mighty Network.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Milestone.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Milligram.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1998 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MinMaxify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    57624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MindBody.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      316 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mindbox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      348 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mint.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1411 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mintlify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      696 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Miso.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3808 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Misskey.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mithril.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      688 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mittwald.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mixin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mixpanel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      853 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MizbanCloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1095 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MoEngage.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2251 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MobX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2021 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mobicred.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      662 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mobify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MochiKit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      925 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Modern Campus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2118 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Modernizr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ModiFace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1797 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moguta.CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MoinMoin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      655 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mojolicious.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1753 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mokka.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      794 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mollie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      371 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mollom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moment.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      634 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mondial Relay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mondo Media.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moneris.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Monetate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      762 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MongoDB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      977 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mongrel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2722 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Monkey HTTP Server.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mono.net.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mono.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Monsido.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2738 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MonsterInsights.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MooTools.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1213 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moodle.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1505 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moove.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mopinion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Moshimo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4463 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Motherhost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      931 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MotoCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4015 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mouseflow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1175 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Movable Ink.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7916 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Movable Type.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mozard Suite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mudblazor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3402 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mulberry.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2167 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mura CMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mustache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      558 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Muuri.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1477 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/My Flying Box.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    30397 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/My Food Link.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1381 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyBB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      701 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyBlogLog.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyFonts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2608 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyLiveChat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      710 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyOnlineStore.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2823 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MySQL.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      441 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MySiteNow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      545 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MyWebsite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2651 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Myhkw player.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mynetcap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Mysitefy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/MysteryThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NACEX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4113 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NSW Design System.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      876 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NVD3.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2026 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nacelle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      710 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NagaCommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nagich.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1801 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NagishLi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Naive UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1168 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Najva.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2433 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NamelessMC.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1046 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Narrativ.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      862 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Narvar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2295 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NationBuilder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nativo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      862 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Navegg.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7217 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Naver Analytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   233353 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Naver Maps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      469 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Naver.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15017 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Navidium.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Neat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3339 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Neon One.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      547 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Neos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nestify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NetSuite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1454 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Netcore Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1049 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Netdeal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Netlify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2573 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Neto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1680 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nette Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Network for Good.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      447 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/New Relic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      374 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NewStore.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2267 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NewspackLogo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5444 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nexive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Next Total.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1962 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Next-Auth.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1110 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Next.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1889 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NextGEN Gallery.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1973 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NextUI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1347 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nextcloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      859 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nextdoor Ads.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1030 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nextra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3425 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nextsale.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1083 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NexusPHP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1052 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NexusPIPE.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nginx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Niagahoster.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nicepage.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1810 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ninja Forms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   100963 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NitroPack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      467 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NoFraud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1043 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Noddus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    22140 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Node.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1809 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NodeBB.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      304 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/NodePing.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nogin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      807 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Northbeam.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2307 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Norton Shopping Guarantee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1095 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nosto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1342 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Notifly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1637 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Notion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1378 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nudgify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nukeviet CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1430 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nuqlium.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4063 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nuvemshop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      780 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Nuxt.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OTYS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      560 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OVHcloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1033 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OWL Carousel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OXID eShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      979 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Obsidian Publish.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1439 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Obsidian.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Obviyo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1541 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Occasion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1236 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OceanWP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3438 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ochanoko.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oct8ne.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4409 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Octane AI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      700 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/October CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1204 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ocuco.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1108 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Odoo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      932 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oh Dear.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2390 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Okendo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4029 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Okta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      546 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Olapic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      869 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Olark.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1316 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omeka.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ometria.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14573 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1040 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omniconvert.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1041 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omnisend.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2080 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omny Studio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1532 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Omurga Sistemi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      466 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OnUniverse.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      244 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/One.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1353 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneAPM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      964 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneAll.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1233 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneCause.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OnePress Social Locker.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1928 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneSignal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      909 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneStat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14461 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OneTrust.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oney.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Onfido.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Onshop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      569 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ookla.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1874 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oopy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    86800 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open AdStream.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1602 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open Classifieds.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1911 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open Graph.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open Journal Systems.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      158 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open Web Analytics.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      905 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Open eShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    66670 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenBSD httpd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2609 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenCV.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1432 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenCart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1960 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenCms.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2073 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenElement.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      427 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenGrok.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      961 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenLayers.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      245 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenNemas.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   257608 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenResty.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      488 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenSSL.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   796121 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenStreetMap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      901 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenSwoole.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1819 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenTable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      392 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenText Web Solutions.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1600 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenUI5.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5148 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenWeb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpenX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      985 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OperateBeyond.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11626 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Opigno LMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      963 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OpinionLab.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2792 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OptiMonk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1098 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Optimise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1591 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Optimizely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      525 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Optimove.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1977 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OptinMonster.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      689 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oracle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1614 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Orankl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16561 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OrbitFox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1780 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Orchard Core.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2572 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Orckestra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Order Deadline.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1021 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OrderCast.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1687 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OrderLogic app.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OrderYOYO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      331 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ordersify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1139 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Osano.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1458 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OutSystems.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      235 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OutTheBoxThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5996 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Outbrain.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1747 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Outlook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2274 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oxatis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1552 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/OxiSocialLogin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Oxygen.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      874 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PCI Proxy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1232 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PCRecruiter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      995 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PDF.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1059 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PHP-Nuke.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PHP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7547 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PHPFusion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      960 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PIXIjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      568 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/POLi Payment.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2362 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/POWR.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1045 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PRONOTE.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      844 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PWA Studio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1127 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PWA.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2899 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1013 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Packlink.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      935 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paddle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3995 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PagSeguro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      916 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pagar.me.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1125 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Page Builder Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pagefai.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      129 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pagekit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1652 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pagevamp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1705 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paidy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2010 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paloma.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2040 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PandaCSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1076 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Panelbear.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pantheon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      767 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paradox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2238 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Parcel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1681 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Parcelforce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      734 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ParkingCrew.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1832 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Parmin Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4802 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Parse.ly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1757 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Partially.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1956 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Partnerize.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      886 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Partnero.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1638 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Parttrap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8764 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Partytown.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2981 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Passage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      414 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Patreon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1617 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pay It Later.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PayBright.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1179 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PayGreen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      875 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PayJustNow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PayKickStart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3883 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PayPal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1515 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Payfast.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      610 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Payflex.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1740 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Payl8r.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paylocity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      675 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Paymenter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Payplug.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PebblePost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16082 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Peek.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PeerBoard.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2586 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PeerTube.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      503 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PencilBlue.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      224 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pendo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1103 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pepperjam.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Peraichi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      308 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Percussion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1205 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PerfectApps Swift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      837 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Perfex CRM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3012 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Perfmatters.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1405 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Performance Lab.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10729 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PerimeterX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3022 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Periodic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1109 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Peripl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Perl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      794 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Permutive.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16114 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PersonaClick.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2236 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Personio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4227 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Personizely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2151 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Perzonalization.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      939 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phabricator.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      327 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phaser.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9052 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phenomic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7645 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Philomena.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1512 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phlox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3567 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phoenix Framework.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      946 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phoenix Site.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3987 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Photo Gallery.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PhotoShelter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      761 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PhotoSwipe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1839 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Photoslurp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2306 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Phusion Passenger.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      151 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Piano.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2288 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PickyStory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      804 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pico CSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1987 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Picreel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Picturepark.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1482 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Piman.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2633 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pingdom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pingoteam.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5667 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pinia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PinnacleCart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pinterest.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      766 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pipedrive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Piwigo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1032 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Piwik PRO Core.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pixc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PixelFed.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PixelYourSite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pixelee TurnTo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1238 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pixieset.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8561 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pixnet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PizzaNetz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1395 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plaid.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Planet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2687 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plasmic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plataforma NEO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PlatformOS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      591 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Platforma LP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1181 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PlatinMarket.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      788 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Platter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3002 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plausible.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      493 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Play.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1866 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plaza.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1278 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pleroma.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plesk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8264 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pligg.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5656 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plone.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plotly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plug and Pay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      399 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Plyr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Po.st.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1967 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Podia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2006 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Podigee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      337 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Podium.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      587 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Podsights.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1020 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pojo.me.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Poloriz.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4368 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Polylang.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1516 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Polymer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4931 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Popmenu.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9543 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Popper.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1276 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PopularFX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1815 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Popup Maker.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2009 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Post AG.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Post Affiliate Pro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3451 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PostHog.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PostNL.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5673 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Poste Italiane.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      260 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Posterous.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1021 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PostgreSQL.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Postpay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    26169 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Postscript.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    23054 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Potions.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1791 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PowerReviews.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PowerSchool.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      668 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Powergap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      968 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Preact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1038 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prebid.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prediggo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      489 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prefix-Free.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      712 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Preline UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      949 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Premio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      706 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prepr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Press.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PressMaximum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    62783 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PrestaShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      925 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pretty Links.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      876 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PriceSpider.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PrimeNG.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3998 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PrimeReact.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PrimeVue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Primis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Printful.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3287 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Priority Hints.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prism.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3159 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prismic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1329 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Privy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ProcessWire.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      897 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Product Hunt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Product Personalizer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      914 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ProfilePress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Profitwell.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      738 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Progress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1894 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Project Wonderful.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1565 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PromoBuilding.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Proton Mail.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Prototype.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7780 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ProvenExpert.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1495 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Provide Support.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1840 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Proximis Omnichannel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2582 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Proxmox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ptengine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pterodactyl Panel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2084 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PubGuru.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      788 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PubLive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      155 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PubMatic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Public CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1104 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PulseSecure.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pure CSS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1192 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pure Chat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      766 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PureCars.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    44875 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PurpleAds.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      857 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PushDaddy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1531 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PushEngage.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PushOwl.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1082 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PushPushGo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pushnami.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      850 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Pushpay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2470 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PyData Sphinx Theme.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   318318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PyScript.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1033 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PyroCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      755 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Python.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9695 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/PythonAnywhere.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      979 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Q4.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2650 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/QUIC.cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2553 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qgiv.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      837 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qikify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qstomizer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1755 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qualaroo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2065 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qualified.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qualtrics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      762 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quanta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      899 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quantcast.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1239 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quantummetric.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3023 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quasar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1027 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qubit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      501 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Queue-it.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      250 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quick.CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      250 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quick.Cart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2811 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/QuickSell.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1611 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quickblog.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1009 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quickbutik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1924 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quicklink.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1081 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quicq.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quill.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quintype.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1320 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quoli.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15216 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Quora.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3243 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Qwik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      343 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RBS Change.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      439 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      521 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RD Station.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      408 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RDoc.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1112 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/REDAXO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2464 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/REG.RU.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RND.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      977 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      165 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RTB House.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1498 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RXWeb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      204 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RackCache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      451 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Radix UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3727 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rain.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RainLoop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1245 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RaiseDonors.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      589 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raisely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raku-uru Cart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rakuten Advertising.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rakuten.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      631 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RakutenDigitalCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ramda.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      549 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RankMath SEO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1105 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raphael.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5778 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RapidSec.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3077 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RapidSpike.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raptor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5498 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raspbian.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1264 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RateParity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rawabit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3144 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Raygun.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1878 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rayo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      395 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Razorpay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1561 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Re-amaze.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReCaptcha v2 for Contact Form 7.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3124 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReConvert.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      950 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/React Bricks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3897 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/React Flow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1743 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/React Router.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4822 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/React.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reactive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1492 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReadSpeaker.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1517 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Readymag.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Really Simple CAPTCHA.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18473 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RebelMouse.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2748 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rebuy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      797 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recapture.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3467 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1519 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recent Posts Widget With Thumbnails.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      918 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recharge.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1182 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recharts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1778 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recite Me.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      714 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recomify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1062 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RecoverMyCart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3549 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recruitee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      400 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recurate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3105 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Recurly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1890 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Red Hat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4063 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Red je Pakketje.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7306 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RedCart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      889 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RedShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2201 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reddit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2599 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Redis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2599 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RedisObjectCache.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      687 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Redmine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Redonner.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      404 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Redux Framework.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Redux.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RedwoodJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      739 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reelevant.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2498 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reevoo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReferralCandy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Refersion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reflektion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Refundid.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    31949 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Regiondo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      707 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reinvigorate.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3243 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Relais Colis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2085 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Relewise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1980 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Remarkable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      707 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Remix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1843 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Remotion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Render.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7296 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Replicache.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      688 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Replit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2401 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reputon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      857 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RequireJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20182 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ResDiary.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9134 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Resengo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reserve In-Store.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reservio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      772 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Resin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Resmio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1048 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Resova.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    21476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ResponsiveVoice.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2714 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Resy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1564 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Retail Rocket.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      868 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Retention.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      746 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Retool.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReturnGO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1573 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Returnly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      548 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RevJet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RevLifter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1362 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Revel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RevenueHunt.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2948 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Revieve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ReviewSolicitors.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2259 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Reviews.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RevolverMaps.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Revv.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Revy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      962 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rewardful.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6096 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rezdy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12703 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rezgo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      936 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rich Plugins.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1020 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RichRelevance.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3532 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Richpanel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1689 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RightJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      439 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Riot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rise.ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Riskified.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      245 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RiteCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1211 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6140 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RoadRunner.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      421 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Roadiz CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2411 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Robin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1459 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RockRMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      240 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rockerbox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3730 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rocket.Chat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2437 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rocketfy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rokt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      961 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rollbar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1328 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rosti.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1327 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rotic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2108 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RoundCube.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2534 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Royal Mail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1195 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rubicon Project.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ruby Receptionists.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2575 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ruby on Rails.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ruby.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1207 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rudderstack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      855 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rumble.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5978 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Rust.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1527 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/RxJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1049 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ryviu.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14335 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/S-COREpion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SALESmanago.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SAP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SDL Tridion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1548 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SEMrush.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3744 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SEOmatic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2421 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SHE Media.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SIDEARM Sports.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1749 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SIMsite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19066 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SNO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      149 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SOBI 2.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      674 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SPDY.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      239 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SQL Buddy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      627 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SQLite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1070 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/STN Video.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1208 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/STUDIO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SUSE.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1820 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SVG Support.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SWFObject.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2469 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SaaSquatch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1483 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Saba.Host.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1271 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SabaVision.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1978 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Saber.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      236 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sails.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      739 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sailthru.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1324 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sakai.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      975 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sakura Internet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Saleor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      812 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SalesFire.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2515 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SalesReps.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      852 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salesforce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salesloft.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1335 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salesnauts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1384 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salla.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1779 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salonist.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12713 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Salsify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Saly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1819 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sana Commerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1104 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sanity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sapper.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      982 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sapren.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sarka-SPIP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4869 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sass.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Satori Studio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      348 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Satori.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8786 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sazito.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1012 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scala.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1010 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scalapay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scalefast.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ScandiPWA.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Schedule Engine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      749 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SchemaPlus.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      171 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scientific Linux.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      176 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scissor Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      682 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scoop.it.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scorpion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scrivito.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1446 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ScrollMagic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Scully.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2347 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SeQura.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Seal Subscriptions.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1704 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SeamlessCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SearchFit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      987 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Searchanise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2948 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SearchiQ.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Searchspring.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Secomapp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sectigo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1363 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sections-Design.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1018 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SeedProd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Segmanta.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2009 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Segment.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1624 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SegmentStream.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3469 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Segmentify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1295 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Seko OmniReturns.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1776 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Select2.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      895 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Selectize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sellacious.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1950 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Selldone.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1216 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SellersCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1381 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Selless.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2272 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sellfy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2489 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sellingo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sellix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2744 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sellsy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Selly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      936 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Semantic-ui.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10290 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sematext.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6029 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Semplice.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sencha Touch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1969 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SendGrid.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SendPulse.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2976 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sendinblue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2529 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sensors Data.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2189 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sentry.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4629 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Seravo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      744 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Serendipity.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Service Management Group.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1075 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Service Provider Pro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      774 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ServiceNow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Setmore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9919 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SevenRooms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2141 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sezzle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      501 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShadCnSvelte.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shaka Player.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5387 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shanon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      923 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shapecss.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      667 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShareThis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      836 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sharethrough.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sharetribe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SharpSpring.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1129 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SheerID.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      234 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShellInABox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      712 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shift4Shop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2219 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shiny.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      222 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShinyStat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3459 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShipStation.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShipTection.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1141 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShippyPro.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4258 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoefitr.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4759 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoelace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7127 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shogun Frontend.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1572 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shogun Page Builder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1178 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shop Pay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShopBase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17906 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShopGold.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1765 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShopPad.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1462 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShopWired.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9748 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopaholic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1819 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopapps.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopatron.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2233 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopcada.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5161 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoper.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2042 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopery.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5666 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopfa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14126 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShopiMind.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2449 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopify Geolocation App.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1682 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1176 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopistry.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      547 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoplazza.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopline.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3838 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoplo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2143 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopmatic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1878 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoporama.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1510 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoppiko.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShoppingFeeder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1750 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShoppingGives.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1854 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoppub.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4707 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoppy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoprenter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      693 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoprunner.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      216 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shoptet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shopware.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9211 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShortPixel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shortcodes Ultimate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Shortly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ShoutOut.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Showit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10347 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sift.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1811 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Signifyd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      872 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SilverStripe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      795 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simpl.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      252 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simple Analytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      255 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simple Machines Forum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      565 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simple.css.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      566 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simple.ink.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16042 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simplebo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1250 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simplero.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      259 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simplifi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1206 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simplio Upsells.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2782 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simplo7.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1282 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SimplyBook.me.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      233 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Simvoly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1133 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sinatra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1604 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sirclo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sirdata.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      505 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sirge.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      975 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sirvoy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      382 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Site Meter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4491 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Site Search 360.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2892 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Site24x7.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteEdit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteGuard WP Plugin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1590 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteJabber.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1999 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteManager.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1376 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteMinder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteOrigin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1889 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SitePad.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      885 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteSpect.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1069 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteVibes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1401 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SiteW.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sitecore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      485 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sitefinity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Siteglide.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Siteimprove.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1091 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sitepark.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sitevision CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1435 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sivuviidakko.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SixCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4700 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sizebay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      642 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sizmek.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      757 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1272 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skedify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      489 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skilldo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1468 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skimlinks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skolengo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sky-Shop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1384 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SkyVerge.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      796 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skyflow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Skynet Technologies.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1262 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sleeknote.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sleekplan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6164 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slice.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    34385 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slick.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1986 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SlickStack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1211 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slider Revolution.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1309 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slimbox 2.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1309 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Slimbox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      579 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smart Ad Server.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4460 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smart Slider 3.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      994 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SmartRecruiters.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      387 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SmartSite.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      726 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SmartWeb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2451 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smarter Click.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5124 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartling.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7973 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartlook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1099 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartocto.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartstore.biz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1310 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartstore.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5294 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smartsupp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1111 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smash Balloon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1572 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Smile.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SmugMug.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5141 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snap Pixel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1680 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snap.svg.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SnapEngage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SnapWidget.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1424 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snipcart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SniperFast.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sniply.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snoobi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2366 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Snowplow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SobiPro.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1604 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Social9.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      703 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SocialJuice.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1584 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SocialLadder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2049 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Societe des Avis Garantis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Socket.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      667 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Softr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Soisy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SolidJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SolidPixels.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      199 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Solodev.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      951 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Solr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2323 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Solusquare.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Solve Media.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Solvemate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      901 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sonobi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2675 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Soocommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      500 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sortable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      697 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sorted.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    20813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SoteShop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8873 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sotel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3967 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sotoon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2609 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SoundCloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SoundManager.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3676 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sourcepoint.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sovrn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      849 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SparkPost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      965 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spatie Media Library Pro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2463 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spatie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      852 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spectra.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Speed Kit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3224 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpeedCurve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8068 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpeedSize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5434 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Speedimize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1882 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spektrix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2733 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sphinx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      683 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpiceThemes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2128 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spin-a-Sale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spinnakr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1259 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpiritShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1063 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Splide.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1178 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Split.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SplitIt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SplittyPay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      216 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Splunk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1072 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpotHopper.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1381 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpotX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1164 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spotify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spotii.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18611 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spree.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6217 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sprig plugin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1060 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sprig.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1370 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spring for creators.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2333 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spring.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9479 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SprintHub.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5200 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Spryker.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      886 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SpurIT.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      982 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sqreen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2062 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Squadata.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Squadded.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      879 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Square.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Squarespace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Squeezely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SquirrelMail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      699 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Squiz Matrix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stack Analytix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1918 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StackPath.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2705 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stackable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stackcommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1369 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StackerHQ.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stackify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1477 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stage Try.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2457 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stamped.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2849 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Starhost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Starlet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1524 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statamic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1091 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statcounter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statically.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1670 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statping.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1312 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statsig.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1287 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Status.io.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1678 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StatusCast.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1306 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Statuspal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1413 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stay22.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      226 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Staytus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SteelHouse.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stencil.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2057 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stimulus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stitches.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stoplight.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1629 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StoreHippo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1510 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Storefront UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1920 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Storeino.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1331 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Storeplum.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1354 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StorifyMe.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      422 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StoryStream.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Storyblok.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      943 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Strapi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    10601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Strato.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1645 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Strikingly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      526 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stripe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      392 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/StrutFit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6509 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Stylitics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1588 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sub2Tech.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      814 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Subbly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sublime.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      802 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SublimeVideo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      906 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Subrion.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Substack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1157 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Suiteshare.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2026 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sulu.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SummerCart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2375 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Summernote.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15334 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sumo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Suncel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1355 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Supabase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      758 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Super Builder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1820 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Super Socializer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2305 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SuperLemon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      292 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Supersized.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    17066 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Superspeed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Support Hero.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1931 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Survicate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Svelte.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5400 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swagger UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1167 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swagify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1835 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SweetAlert.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    24482 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SweetAlert2.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swell.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      978 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swiffy Slider.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1128 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swiftype.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3369 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swiper.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      965 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swup.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1128 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Swym.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      547 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Sylius.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2406 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Symfony.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1185 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Syndeca.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      442 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Synerise.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Synology DiskStation.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/SyntaxHighlighter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1579 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Systeme.io.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1922 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Syte.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2548 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/T1 Comercios.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1309 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/T1 Envios.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1460 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/T1 Paginas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/T1 Pagos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2049 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TCAdmin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2152 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TDesign.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      312 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/THG Ingenuity.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/THRON.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TRISOshop.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      313 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TRUENDO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1679 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TVSquared.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      317 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TWiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TYPO3.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1495 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tabarnapp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1399 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tabby.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TableBooker.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12405 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TableCheck.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1370 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TablePress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Taboola.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    30514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tachyons.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1911 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tada.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1357 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TagPro.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      513 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tagboard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tagembed.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1227 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Taggbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1719 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Taiga.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4764 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tail.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      902 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TakeDrop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1091 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Talkable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2086 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tallentor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16751 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tally.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4274 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tamago.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1051 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tamara.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      853 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tap Payments.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tapad.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1377 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tapcart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1396 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tapfiliate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1143 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Target2Sell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      369 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tatari.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TawkTo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Teachable.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4829 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Teads.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      324 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tealium.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1359 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TeamBrain.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4166 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TeamCity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      881 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TeamUp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tebex.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Telescope.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2148 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tencent Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3831 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tencent QQ.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1089 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TencentWaterproofWall.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1914 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tengine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      654 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tern.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5269 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TerriaJS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8794 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TestFreaks.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      407 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Texthelp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1768 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Textpattern CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6683 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The Arena Group.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      412 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The Church Co.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1829 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The Events Calendar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1342 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The Hotels Network.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1996 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The SEO Framework.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2000 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The Theme Foundry.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3243 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/The.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9178 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Theatre.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    31558 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thefork.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      355 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thelia.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1664 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Theme Freesia.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      942 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Theme Horse.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1185 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Theme Vision.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Theme4Press.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1492 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThemeGrill.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1784 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThemeIsle.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThemeZee.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1151 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Themeansar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Themebeez.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Themegraphy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      826 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Themes4Wp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1001 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThemezHut.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1474 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Themonic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      378 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thesis.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1845 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThimPress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      592 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thimatic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2288 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Think Up Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1833 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThinkPHP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      591 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thinkific.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      960 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Three.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2478 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Threekit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2899 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Thrive.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7610 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ThriveCart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1927 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ticimax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      843 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TiddlyWiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1172 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tidio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1096 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiendanube.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1504 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiiny Host.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TikTok.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiki Wiki CMS Groupware.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiktak Pro.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1644 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tilda.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiledesk.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Timeplot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Timify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      878 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TinyMCE.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tinybird.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16288 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tippy.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5084 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tipsa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tiqets.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3115 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tistory.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      152 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Titan.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    27490 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tolt.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4648 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TomTom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      196 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TomatoCart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      784 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TornadoServer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3704 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TotalCode.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2301 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Totango.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Totara.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6412 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Touch2Success.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1815 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trac.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      761 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Track123.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TrackJs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trackify X.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      778 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tradedoubler.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1206 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Traek.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      663 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TrafficStars.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11998 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Transcend.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2026 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Transcy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1296 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Transistor.fm.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2258 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trbo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Treasure Data.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2184 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trengo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1074 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Triggerbee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      692 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trinity Audio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2738 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tripadviser.Widget.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TripleLift.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tritac.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TruValidate.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1113 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/True Fit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2027 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Truecommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1375 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trumba.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2028 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trunkrs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TrustArc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13562 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TrustYou.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   393228 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trusted Shops.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      885 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trustindex.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      295 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trustpilot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1060 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trustspot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2357 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Trustvox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1059 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TryNow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      533 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tsoft.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      456 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tumblr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Turbo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      180 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TurfJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1132 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TweenMax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      674 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TwicPics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      507 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      468 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twikoo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      426 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twilight CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TwistPHP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      394 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TwistedWeb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      656 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twitch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twitter Flight.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      411 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twitter typeahead.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      851 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Twitter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1006 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TypeDoc.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      629 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TypePad.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2728 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/TypeScript.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1028 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Typeform.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Typekit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      541 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Typof.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2162 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Tyslo EasySell.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      245 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/U-KOMI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      525 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UIKit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2160 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UK Mail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UKFast.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1224 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UMI.CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1599 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UNIX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2608 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UPS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1083 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/USPS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      733 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/USWDS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      826 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ubercart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1594 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ubiliz.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2215 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ubuntu.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1078 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ueeshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1324 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ultimate Addons for Elementor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1336 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ultimate GDPR & CCPA.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2722 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UltimatelySocial.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2545 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UltraCart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1154 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Umbraco.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1063 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UmiJs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3025 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Umso.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unas.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1314 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unbounce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unbxd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      110 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Underscore.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1737 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Understrap.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UniFi_OS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1205 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uniconsent.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      606 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unicorn Platform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1038 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UnoCSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      664 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unpkg.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      509 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unpoly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      731 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Unruly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1304 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UpSellit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UpSolution.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9143 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Upfluence.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      540 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uploadcare.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Upptime.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1735 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Upserve.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      625 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UptimeRobot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uptrends.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1292 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UsableNet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1859 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uscreen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/User Accessibility.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2753 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/User1st.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserLike.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1423 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserReport.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      831 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserRules.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2053 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserVoice.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1962 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserWay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1713 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/UserZoom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      656 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Userback.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Usercentrics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1277 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Userflow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3401 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Userpilot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2760 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ushahidi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1061 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Usizy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      797 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uvodo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1233 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Uzerly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1095 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VAPTCHA.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1320 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VDX.tv.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      218 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VIVVO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      248 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VP-ASP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1383 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VTEX.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1030 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VWO.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1178 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vaadin.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1060 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ValueCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vanco.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1948 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vanilla.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vant.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1063 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Variti.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      633 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Varnish.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1153 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ve Global.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      589 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vendre.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1502 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Venly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      688 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Venmo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1517 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VentraIP.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1462 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Veoxa.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      579 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Verifone.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VerifyPass.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      230 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Verizon Media.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      851 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Verloop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      337 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VerticalScope.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1588 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Very Good Security.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1327 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vev.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2520 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ViaBill.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      240 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vidazoo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1686 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Video Greet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1536 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VideoJS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vignette.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      485 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vimeo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Viqeo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9732 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Viral Loops.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1535 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virgool.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1486 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virtooal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      888 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virtuagym.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virtual Chat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1721 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VirtualSpirits.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1878 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VirtueMart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      360 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virtuous.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      324 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Virtusize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      347 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      792 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visual Portfolio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visual Quiz Builder.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   120921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visualsoft.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      947 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Visx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8723 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vitals.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vitrin.me.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      917 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vizury.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      222 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vnda.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1726 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vntana.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      771 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Volusion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      595 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vonage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1231 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Voog.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      717 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Voracio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      940 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vouchley.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4387 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vtiger.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2066 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VuFind.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vue.ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6631 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/VuePress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      368 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vuetify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8683 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Vultr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      508 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/W3 Total Cache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/W3.CSS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1003 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/W3C.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1693 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/W3Counter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1584 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WEBXPAY.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WEN Themes.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1175 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WHMCS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1858 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Automatic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6169 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Courseware.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2993 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Fastest Cache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2320 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Google Map Embed.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      847 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Google Map Plugin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2184 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Job Openings.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1498 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Maintenance Mode.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1004 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Portfolio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2154 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Puzzle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP Rocket.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1021 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP-Optimize.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      255 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP-PageNavi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP-Royal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5370 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP-Statistics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WPCacheOn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    16093 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WPForms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1546 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WPML.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1123 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WPMU DEV.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WPS Visitor Counter.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1510 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WP_Featherlight.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2610 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wagtail.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wair.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      399 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Waitlist.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1891 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wakav Performance Monitoring.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WalkMe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      791 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wangsu.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1037 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Warp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1669 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wask.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      770 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Waveme.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1183 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WayForPay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8704 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WeWeb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1448 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Weaver Xtreme.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1804 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Web Shop Manager.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1235 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Web-Stories.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      133 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Web2py.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1003 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebAssembly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      754 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebEngage.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      981 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebFactory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1973 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebGUI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1336 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebHostUK.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1978 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebMetric.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      711 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebNode.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2634 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebRTC.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      596 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebSite X5.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      598 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebSocket.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1158 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebToffee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2267 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebWave.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5749 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webasyst Shop-Script.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      890 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webeyez.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4876 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webgains.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1926 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Weblication.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Weblium.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1484 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webmin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1573 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webolytics.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      918 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webpack.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      618 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webriti.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      363 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebsPlanet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      531 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Websale.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      603 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebsiteBaker.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    31494 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebsiteBuilder.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WebsiteCreator.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      849 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webtrends.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2889 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webx.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3015 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webyn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2214 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webzi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2615 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Webzie.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Weebly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1190 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Weglot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Welcart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5959 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WeltPixel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      542 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Whatfix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3489 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WhatsApp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wheelio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      454 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Whistl.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      511 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Whooshkaa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      973 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WideBundle.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1382 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Widen.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WidgetWhats.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1106 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wigzo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1939 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wiki.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      667 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WikkaWiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1133 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WildJar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1387 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WindowsServer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      383 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WineDirect.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      436 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wink.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      416 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wirecard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1111 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wisepops.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1299 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wishlist King.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wistia.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/With Reach.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wix Answers.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18870 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2194 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WiziShop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1616 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wizpay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2339 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wolf CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1646 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wolfeo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3071 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Woltlab Community Framework.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1126 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WooCommerce Blocks.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1219 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WooCommerce Multilingual.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1065 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WooCommerce PayPal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1075 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WooCommerce Stripe Payment Gateway.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1563 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WooCommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Woopra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1452 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Woostify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WoowUp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      224 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WordAds.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      969 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WordPress Popular Posts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1505 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WordPress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2472 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wordfence.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1147 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Workable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1488 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Workarea.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      296 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/World4You.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3921 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WorldPay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Worldz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      925 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wufoo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1195 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wuilt.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1285 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wunderkind.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1975 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Wurfl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2534 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/WysiBB.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1254 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/X-Cart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1117 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/X.ai.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XAMPP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1847 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XGen Ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      697 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XMB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      615 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XOOPS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XRegExp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      893 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xajax.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      465 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xanario.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      290 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XenForo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      175 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xitami.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1148 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xiuno BBS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2029 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/XpressEngine.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1452 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xpresslane.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      691 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xretail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xserver.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1763 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xtime.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1145 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xtra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1290 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Xtremepush.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      709 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YMQ Product Options Variant Option.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1189 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YNAP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1287 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YUI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      357 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YaBB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      697 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yahoo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1815 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YalinHost.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1582 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yampi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8852 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yandex.Cloud.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2031 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yandex.Direct.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   116742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yandex.Messenger.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1113 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yandex.Metrika.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      574 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yapla.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yaws.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      393 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ycode.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2538 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yektanet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    25346 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yelp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YesWiki.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yett.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1441 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yext.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yieldify.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1823 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yieldlab.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3690 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yii.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yoast SEO.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      768 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yola.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      604 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YooMoney.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2495 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yoori.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      356 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yotpo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    14089 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Yottaa.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2286 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouCam Makeup.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      896 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouCan Pay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      151 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouCan.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1011 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouPay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1522 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouTrack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      570 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YouTube.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6765 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/YunoHost.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      398 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ZK.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      353 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ZURB Foundation.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      125 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zabbix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      960 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zakeke.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      599 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zakra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zanox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1221 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zeald.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      938 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zen Cart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      397 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zen Planner.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zend.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      429 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zendesk Chat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      671 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zendesk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      634 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zenfolio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1307 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zeotap.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2358 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zepto.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1481 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ZestMoney.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   285671 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zeus Technology.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zid.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1201 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Ziggy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zimbra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      686 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ZingChart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zinnia.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1285 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zinrelo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      431 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zipify OCU.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      467 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zipify Pages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1575 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zipkin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1961 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zipteams.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1492 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zmags Creator.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1644 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zocdoc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      409 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zoey.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2463 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zoho Commerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1698 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zoho.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1981 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zoko.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      635 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zola.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19863 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zonos.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      956 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ZoodPay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1783 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zoominfo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      574 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zope.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1828 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zozo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1630 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/Zuppler.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1129 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/_hyperscript.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      816 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/a-blog cms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/a3.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      336 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/aThemes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      944 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/abicart.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3166 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/abp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2054 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-campaign-factory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1944 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-cdp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-cloud-ide.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      956 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-cloud-platform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2273 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-cloud.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5107 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-content-hub.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-personalization.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1834 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-site-factory.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1474 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/acquia-site-studio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1458 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/actionhero.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3378 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/addi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      742 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/adminer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1433 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/adobedtm.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1487 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/adrecover.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1362 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/afterpay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      492 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ahrefs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1988 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/aimeos.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1463 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/aircall.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/akaunting.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/akinon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      778 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/akka-http.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3046 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/amCharts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/amber.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1854 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/amex.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1710 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/amoCRM.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9148 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/anime.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    11559 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/apexcharts.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3423 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/arcgis_icon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2095 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/arsys.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/aspnetboilerplate.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1298 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/atome.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      730 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/atws.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1370 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/augmented-ui.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      689 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/authorize.net.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1153 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/autoComplete.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1429 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/automatad.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5167 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bSecure.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    15451 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bablic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1014 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/babylonjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    29666 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/basilcss.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/basket.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4089 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bdok.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1912 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bizweb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      579 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/blitzjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1756 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bokeh.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bookly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2578 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/boom.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      655 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/boomerang.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/brimble.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1825 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/bubble.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1718 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/butter-cms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      539 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cPanel.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cState.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1887 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/caddy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5636 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/canvasjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2455 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cashew.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1740 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ccvshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      543 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cdnjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1887 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cendyn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12042 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/centminmod.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      115 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cgit.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4904 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/citruspay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      647 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/civic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2195 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/civictheme.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1476 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/clarity.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3590 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/classy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1150 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/clickio.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1239 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cloudcart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1036 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/clutch.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cnzz.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1019 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/coaster-cms.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      580 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/coinhave.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1530 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/coinimp.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1201 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/colbass.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      900 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/colormeshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      432 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/comScore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2762 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/comeet.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1534 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/commercejs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1826 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/commercelayer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2143 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/commercetools.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/conviva.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      448 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cookieyes.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2860 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/core-js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2102 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cosmicjs.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2417 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/cybersource.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2803 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/daisyUI.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      762 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/daphne.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      794 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/db-ip.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      749 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/decimal.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/deepminer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      326 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/default.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1567 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/demandbase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1990 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/deno.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1016 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/deta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1958 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/didomi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3698 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/distributor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    13355 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/docusaurus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      502 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/draftjs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      521 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/e-goi.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      574 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/e107.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2097 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eBay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1648 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eCaupo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      956 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eClass.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1399 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eDokan.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6034 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eKomi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1491 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eNamad.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1099 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ePages.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      907 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eSSENTIAL Accessibility.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4629 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eShop eCommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1318 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eShopCRM.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1410 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eSputnik.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eSyndiCat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1750 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eZ.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    54631 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ebis.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2858 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ebisumart.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1290 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/echarts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12443 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ecwid.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      715 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ef.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/elasticpress.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1934 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/elcom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1765 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/elementio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5075 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/elementskit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/elm.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/emBlue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8357 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/endurance-cache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      601 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/enduro.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1588 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/engintron.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1120 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ensighten.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      468 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/etherpad.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2979 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/etika.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eucookie.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1581 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eventon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1453 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/eway.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1394 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/experiencedCMS_Logo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1094 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/fastspring.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      435 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/fatzebra.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      619 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/feedback-fish.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4664 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/filepond.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      713 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/flarum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6903 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/flywheel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1325 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/foswiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2349 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/foxyio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/front-commerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1520 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/frontity.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/fullPage.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      618 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/fun_captcha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1257 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/fusion_charts.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2652 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/futureshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1428 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/generatepress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3267 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/genezio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gerrit.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4252 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gist_live_chat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1678 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/git.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5715 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gitea.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3420 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gluster.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6803 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/goanywhere.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1045 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/goatcounter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4004 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gogs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1378 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/google-cloud-cdn.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      943 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/google-cloud-storage.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      763 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/google-cloud-trace.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3783 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/govCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      662 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/govuk.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3496 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/granicus.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1284 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gravityforms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1651 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/gunicorn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4440 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hCaptcha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2939 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hantana.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5047 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hashnode.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1100 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hcl-dx.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/here.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      494 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/heroku.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1961 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hinza_advanced_cms.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1499 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hirschmann_OS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/honey-badger.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1185 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hoolah.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3731 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/human_presence.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1097 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/hypercorn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2060 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/i-MSCP.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1685 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/i-mobile.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      805 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iAdvize.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2880 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iEXExchanger.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      610 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iHomefinder IDX.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    22125 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iPresta.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      971 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iSina Chat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3637 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iThemes Security.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3258 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iWeb.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/idCloudHost.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2676 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/idosellshop.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      986 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ikiwiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/imperiaCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1102 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/inSales.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/inSided.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2311 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/inspectlet.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1402 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/instamojo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1727 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ip-api.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      989 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipapi.co.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1069 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipapi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2445 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipbase.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2137 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipdata.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1734 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipgeolocation.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1412 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1332 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iplabel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2012 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ipstack.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1119 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/irroba.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      776 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iubenda.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2194 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ivory_searc.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1972 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/iyzico.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      703 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/j2store.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1155 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jComponent.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      829 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jPlayer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      884 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jQTouch.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1223 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jQuery Mobile.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jQuery Modal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jQuery UI.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3983 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jQuery.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      592 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jqPlot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5899 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/jsdelivr-icon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/juspay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      652 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/k-eCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/keen-slider.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      967 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/keep. archeevo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      814 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kemalcr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5480 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kestrel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      651 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kibana.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7968 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kinsta.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      878 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kobalte.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1561 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/koha.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1644 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/kudobuzz.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1919 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/lagoon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5541 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/landbot.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1280 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/langify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      987 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/laterpay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5249 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/lede.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2229 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/libravatar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2241 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/libwww-perl-daemon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      713 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/lighttpd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2390 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/litespeed-cache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      904 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mParticle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8850 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mailchimp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4760 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mariadb.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1790 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/master_slider.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      346 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/math.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1195 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mattermost.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1419 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mautic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3314 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mdBook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2920 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/melis-platform.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2115 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/metomic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1104 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/microCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      124 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mini_httpd.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      744 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mirrAR.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1540 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/miva.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      271 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mkdocs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1992 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mobirise.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      372 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mod_perl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      607 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mod_python.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      488 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mod_ssl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      199 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mod_wsgi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1035 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/model-viewer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      263 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/modified.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1474 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/moon.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1653 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/mycashflow.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2592 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/nepso.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1830 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/nexcess.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1505 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/noibu.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      736 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/nopCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1291 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/nopStation.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3409 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/novomind.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      773 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ocStore.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      267 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/octopress.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/onpublix.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2113 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/openpay.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/openxchange.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1015 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ordergroove.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/orocommerce.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1647 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/osCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1024 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/osTicket.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1282 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/otrs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ownCloud.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      345 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/p5.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1751 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pagefly.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1491 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pagely.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      391 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/papaya CMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3114 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/parselecom.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      373 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/paysafe.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3560 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/paywhirl.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1597 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pelican.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1813 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/percona.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      443 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpAlbum.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1240 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpBB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      367 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpDocumentor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      468 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpMyAdmin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpPgAdmin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      359 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpSQLiteCMS.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3621 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpdebugbar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      467 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/phpwind.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      466 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pico.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      477 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pimcore.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2952 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pinoox.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3159 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pinpayments.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1351 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pirobaseCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1233 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/platformsh.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1971 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/plentyShop LTS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1971 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/plentymarkets.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pocket.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      303 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/polyfill.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9386 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/powerboutique.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1335 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pressable.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      131 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/prettyPhoto.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/projesoft.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      631 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pubsub-js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      295 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/punBB.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1789 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/pygments.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5302 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/qiankun.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1058 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/question2answer.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1821 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/raychat.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      610 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/reCAPTCHA.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3088 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/readme.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      659 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/redoc.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2050 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/remixd.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2134 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/renderbetter.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      383 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/replo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1848 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/return-prime.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      214 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/retype.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1084 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/reveal.js.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1108 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ripple.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1010 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/roistat.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/route.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      108 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sIFR.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      266 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sNews.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    22534 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/salecycle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1008 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/salesfloor.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2703 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sazito-phoenix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      542 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/script.aculo.us.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      920 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/scrollreveal.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1089 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sectionio.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1565 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/seersco.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7323 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/shadcn-ui.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1052 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/shareaholic.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      929 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/signal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      800 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/siimple.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1345 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/simbel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1853 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/siteground.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3044 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/skilljar.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6021 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/snigel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1234 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/softtr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3780 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/solvvy.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      724 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sonar.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5652 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/spip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     4503 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/splitbee.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3096 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/stimulus-reflex-logo.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2518 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/storeden.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1877 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/stores.jp.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      913 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/storybook.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      316 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/strapdown.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      694 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/strattic-icon.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    38966 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/styled-components.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1121 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sucuri.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2649 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/superpwa.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1255 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/svbtle.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     5472 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/swc.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3237 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/sympa.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1537 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/syncfusion.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      931 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tailwindcss.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1103 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tajs.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2090 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/teamtailor.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      399 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/termly.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1076 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tessitura.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/theTradeDesk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2498 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/threatmetrix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      124 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/thttpd.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      799 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tictail.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2344 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tnsi.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1583 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/toastr.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      944 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/total.js.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    32038 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/townnews.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      232 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/trading_view.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1271 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/transifex.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1677 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/tray.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8212 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/triplewhale.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1107 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/trix.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2511 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/trove.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7566 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/truepush.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1259 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/twilio_authy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2579 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/typecho.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2017 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uKnowva.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1032 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uLogin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6457 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uMarketingSuite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2093 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uPlot.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7688 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uPortal.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      439 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/umami.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      863 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/unbox.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6550 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/upvoty.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      262 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/user.com.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/utterances.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1745 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/uvicorn.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2841 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/v4Guard.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1808 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vBulletin.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1640 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/varbase.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1107 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vcita.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1554 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vectary.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2886 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/ventry_shield.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      183 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vercel.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/viafoura.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1012 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vibecommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2769 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vigbo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1126 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/visualcomposer.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1523 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vite.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2205 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vk.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1379 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vue-storefront.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      261 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vue.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1621 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vuukle.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1752 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/vxe-table.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      633 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wBuy.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      334 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wap.store.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2281 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wazimo.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1144 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/web-vitals.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      418 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/webEdition.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2665 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/webdev.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      514 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/webflow.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1152 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/webpushr.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1641 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wikinggruppen.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2414 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wisyCMS.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3994 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/worldshopping.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      934 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wowza.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2874 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wpBakery.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1539 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wpCache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      785 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wp_super_cache.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1289 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wpengine.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3188 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/wpvip.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1869 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/xeora.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1406 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/xonic.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1092 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/xtCommerce.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1672 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/xwiki.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      838 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/yandex_smartcaptcha.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1700 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/yellow.ai.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     2429 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/yepcomm.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1687 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/yoast-seo-shopify.png
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      404 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/zeabur.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      380 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/zip_pay.svg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1603 2024-02-23 08:38:41.000000 webinspectra-1.0.2/webinspectra/data/icons/zotabox.png
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.941020 webinspectra-1.0.2/webinspectra/data/technologies/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7019 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/_.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   150822 2024-04-11 20:50:07.000000 webinspectra-1.0.2/webinspectra/data/technologies/a.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    77630 2024-04-21 20:43:56.000000 webinspectra-1.0.2/webinspectra/data/technologies/b.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   126409 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/c.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    58160 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/d.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    61359 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/e.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    67058 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/f.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    70996 2024-05-26 20:53:51.000000 webinspectra-1.0.2/webinspectra/data/technologies/g.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    49916 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/h.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    47057 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/i.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    28225 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/j.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    36178 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/k.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    57764 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/l.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    95231 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/m.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    35143 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/n.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    55592 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/o.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   107248 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/p.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    12872 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/q.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    68363 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/r.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)   198382 2024-04-13 20:05:15.000000 webinspectra-1.0.2/webinspectra/data/technologies/s.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    97757 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/t.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    29092 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/u.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    37725 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/v.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    70528 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/w.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     8424 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/x.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    21025 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/y.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    19055 2024-03-25 18:37:02.000000 webinspectra-1.0.2/webinspectra/data/technologies/z.json
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18871 2024-05-29 19:57:27.000000 webinspectra-1.0.2/webinspectra/inspectra.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:43:32.941020 webinspectra-1.0.2/webinspectra/utils/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 16:38:14.000000 webinspectra-1.0.2/webinspectra/utils/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3312 2024-04-17 19:29:48.000000 webinspectra-1.0.2/webinspectra/utils/selenium_utils.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6701 2024-05-27 19:29:48.000000 webinspectra-1.0.2/webinspectra/utils/signature_utils.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9060 2024-05-27 19:30:04.000000 webinspectra-1.0.2/webinspectra/webpage.py
```

### Comparing `webinspectra-1.0.1/LICENSE` & `webinspectra-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/PKG-INFO` & `webinspectra-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebInspectra
-Version: 1.0.1
+Version: 1.0.2
 Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 Home-page: https://github.com/insafm/WebInspectra
 Author: Mohammed Insaf M (insafm)
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `webinspectra-1.0.1/README.md` & `webinspectra-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/WebInspectra.egg-info/PKG-INFO` & `webinspectra-1.0.2/WebInspectra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebInspectra
-Version: 1.0.1
+Version: 1.0.2
 Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 Home-page: https://github.com/insafm/WebInspectra
 Author: Mohammed Insaf M (insafm)
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `webinspectra-1.0.1/setup.py` & `webinspectra-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name="WebInspectra",
-    version="1.0.1",
+    version="1.0.2",
     description="WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Mohammed Insaf M (insafm)",
     url="https://github.com/insafm/WebInspectra",
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `webinspectra-1.0.1/tests/test_webinspectra.py` & `webinspectra-1.0.2/tests/test_webinspectra.py`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/webinspectra/__main__.py` & `webinspectra-1.0.2/webinspectra/__main__.py`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/webinspectra/inspectra.py` & `webinspectra-1.0.2/webinspectra/inspectra.py`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/webinspectra/utils/selenium_utils.py` & `webinspectra-1.0.2/webinspectra/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/webinspectra/utils/signature_utils.py` & `webinspectra-1.0.2/webinspectra/utils/signature_utils.py`

 * *Files identical despite different names*

### Comparing `webinspectra-1.0.1/webinspectra/webpage.py` & `webinspectra-1.0.2/webinspectra/webpage.py`

 * *Files identical despite different names*

