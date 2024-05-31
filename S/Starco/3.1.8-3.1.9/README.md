# Comparing `tmp/Starco-3.1.8.tar.gz` & `tmp/Starco-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Starco-3.1.8.tar", last modified: Fri May 10 20:33:31 2024, max compression
+gzip compressed data, was "Starco-3.1.9.tar", last modified: Fri May 31 08:54:42 2024, max compression
```

## Comparing `Starco-3.1.8.tar` & `Starco-3.1.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/
--rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-10 20:33:31.512654 Starco-3.1.8/PKG-INFO
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/Starco.egg-info/
--rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-10 20:33:31.000000 Starco-3.1.8/Starco.egg-info/PKG-INFO
--rw-rw-r--   0 starco    (1000) starco    (1000)     1274 2024-05-10 20:33:31.000000 Starco-3.1.8/Starco.egg-info/SOURCES.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)        1 2024-05-10 20:33:31.000000 Starco-3.1.8/Starco.egg-info/dependency_links.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)      359 2024-05-10 20:33:31.000000 Starco-3.1.8/Starco.egg-info/requires.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)        7 2024-05-10 20:33:31.000000 Starco-3.1.8/Starco.egg-info/top_level.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)       38 2024-05-10 20:33:31.512654 Starco-3.1.8/setup.cfg
--rw-rw-r--   0 starco    (1000) starco    (1000)      776 2024-05-10 20:07:25.000000 Starco-3.1.8/setup.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/
--rw-rw-r--   0 starco    (1000) starco    (1000)       15 2023-11-10 08:57:48.000000 Starco-3.1.8/starco/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/cloudflare/
--rw-rw-r--   0 starco    (1000) starco    (1000)     4060 2023-12-25 11:56:49.000000 Starco-3.1.8/starco/cloudflare/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/crypto_gates/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-17 13:29:58.000000 Starco-3.1.8/starco/crypto_gates/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/crypto_gates/nowpayments/
--rw-rw-r--   0 starco    (1000) starco    (1000)      586 2023-12-17 13:30:45.000000 Starco-3.1.8/starco/crypto_gates/nowpayments/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/db/
--rw-rw-r--   0 starco    (1000) starco    (1000)     3601 2023-11-27 16:38:44.000000 Starco-3.1.8/starco/db/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/debug/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1051 2023-12-01 08:39:29.000000 Starco-3.1.8/starco/debug/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/gateways/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1426 2023-12-11 14:39:40.000000 Starco-3.1.8/starco/gateways/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/gateways/gates/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-11 12:22:45.000000 Starco-3.1.8/starco/gateways/gates/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1675 2023-12-23 09:24:08.000000 Starco-3.1.8/starco/gateways/gates/aqayepardakht.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     3382 2023-12-23 09:24:40.000000 Starco-3.1.8/starco/gateways/gates/idpay.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1950 2023-12-23 09:24:43.000000 Starco-3.1.8/starco/gateways/gates/nextpay.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1140 2023-12-23 09:24:28.000000 Starco-3.1.8/starco/gateways/gates/utils.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1826 2023-12-23 09:24:48.000000 Starco-3.1.8/starco/gateways/gates/vandar.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1182 2023-12-23 09:24:49.000000 Starco-3.1.8/starco/gateways/gates/zibalpay.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/gui/
--rw-rw-r--   0 starco    (1000) starco    (1000)     9174 2024-03-31 08:39:11.000000 Starco-3.1.8/starco/gui/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    32861 2024-03-16 18:40:57.000000 Starco-3.1.8/starco/gui/utils.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/hetzner/
--rw-rw-r--   0 starco    (1000) starco    (1000)     6113 2023-12-25 18:28:35.000000 Starco-3.1.8/starco/hetzner/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/pkl/
--rw-rw-r--   0 starco    (1000) starco    (1000)     2208 2023-11-10 08:07:45.000000 Starco-3.1.8/starco/pkl/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.508654 Starco-3.1.8/starco/proxy/
--rw-rw-r--   0 starco    (1000) starco    (1000)     2248 2023-12-01 08:40:12.000000 Starco-3.1.8/starco/proxy/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/scraper/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1693 2024-05-03 15:02:33.000000 Starco-3.1.8/starco/scraper/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/tlg/
--rw-rw-r--   0 starco    (1000) starco    (1000)       35 2024-01-09 13:06:48.000000 Starco-3.1.8/starco/tlg/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/tlg/app/
--rw-rw-r--   0 starco    (1000) starco    (1000)    38618 2024-02-24 13:24:00.000000 Starco-3.1.8/starco/tlg/app/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      812 2024-01-09 13:06:48.000000 Starco-3.1.8/starco/tlg/app/utils.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/tlg/bot/
--rw-rw-r--   0 starco    (1000) starco    (1000)     6864 2024-01-16 10:26:32.000000 Starco-3.1.8/starco/tlg/bot/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    47327 2024-01-09 14:36:18.000000 Starco-3.1.8/starco/tlg/bot/base.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     3146 2024-01-09 13:06:48.000000 Starco-3.1.8/starco/tlg/bot/classes.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/tlg/bot/util/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2024-01-09 13:06:48.000000 Starco-3.1.8/starco/tlg/bot/util/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      849 2024-01-11 11:40:27.000000 Starco-3.1.8/starco/tlg/bot/util/enum.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     4701 2024-01-09 13:06:48.000000 Starco-3.1.8/starco/tlg/bot/util/filteres.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     5494 2024-02-24 13:19:42.000000 Starco-3.1.8/starco/tlg/bot/util/functions.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    35667 2024-02-24 13:21:45.000000 Starco-3.1.8/starco/tlg/bot/util/packs.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/utils/
--rw-rw-r--   0 starco    (1000) starco    (1000)      125 2023-12-25 07:41:52.000000 Starco-3.1.8/starco/utils/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      951 2023-12-03 09:46:31.000000 Starco-3.1.8/starco/utils/directories.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1469 2024-02-24 13:20:03.000000 Starco-3.1.8/starco/utils/ext.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1323 2023-12-06 19:14:01.000000 Starco-3.1.8/starco/utils/scheduler.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      823 2024-03-24 07:26:00.000000 Starco-3.1.8/starco/utils/structures.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     2247 2024-01-01 09:30:33.000000 Starco-3.1.8/starco/utils/time.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/wp_api/
--rw-rw-r--   0 starco    (1000) starco    (1000)     4370 2023-12-15 13:34:21.000000 Starco-3.1.8/starco/wp_api/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/wscraper/
--rw-rw-r--   0 starco    (1000) starco    (1000)     6600 2024-05-03 15:02:40.000000 Starco-3.1.8/starco/wscraper/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-10 20:33:31.512654 Starco-3.1.8/starco/xray_connctor/
--rw-rw-r--   0 starco    (1000) starco    (1000)    10800 2024-05-10 20:32:56.000000 Starco-3.1.8/starco/xray_connctor/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/
+-rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-31 08:54:42.902475 Starco-3.1.9/PKG-INFO
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.894475 Starco-3.1.9/Starco.egg-info/
+-rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-31 08:54:42.000000 Starco-3.1.9/Starco.egg-info/PKG-INFO
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1274 2024-05-31 08:54:42.000000 Starco-3.1.9/Starco.egg-info/SOURCES.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)        1 2024-05-31 08:54:42.000000 Starco-3.1.9/Starco.egg-info/dependency_links.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)      359 2024-05-31 08:54:42.000000 Starco-3.1.9/Starco.egg-info/requires.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)        7 2024-05-31 08:54:42.000000 Starco-3.1.9/Starco.egg-info/top_level.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)       38 2024-05-31 08:54:42.902475 Starco-3.1.9/setup.cfg
+-rw-rw-r--   0 starco    (1000) starco    (1000)      776 2024-05-31 08:54:39.000000 Starco-3.1.9/setup.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.894475 Starco-3.1.9/starco/
+-rw-rw-r--   0 starco    (1000) starco    (1000)       15 2023-11-10 08:57:48.000000 Starco-3.1.9/starco/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.894475 Starco-3.1.9/starco/cloudflare/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4060 2023-12-25 11:56:49.000000 Starco-3.1.9/starco/cloudflare/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.894475 Starco-3.1.9/starco/crypto_gates/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-17 13:29:58.000000 Starco-3.1.9/starco/crypto_gates/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/crypto_gates/nowpayments/
+-rw-rw-r--   0 starco    (1000) starco    (1000)      586 2023-12-17 13:30:45.000000 Starco-3.1.9/starco/crypto_gates/nowpayments/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/db/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3601 2023-11-27 16:38:44.000000 Starco-3.1.9/starco/db/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/debug/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1051 2023-12-01 08:39:29.000000 Starco-3.1.9/starco/debug/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/gateways/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1426 2023-12-11 14:39:40.000000 Starco-3.1.9/starco/gateways/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/gateways/gates/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-11 12:22:45.000000 Starco-3.1.9/starco/gateways/gates/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1675 2023-12-23 09:24:08.000000 Starco-3.1.9/starco/gateways/gates/aqayepardakht.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3382 2023-12-23 09:24:40.000000 Starco-3.1.9/starco/gateways/gates/idpay.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1950 2023-12-23 09:24:43.000000 Starco-3.1.9/starco/gateways/gates/nextpay.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1140 2023-12-23 09:24:28.000000 Starco-3.1.9/starco/gateways/gates/utils.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1826 2023-12-23 09:24:48.000000 Starco-3.1.9/starco/gateways/gates/vandar.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1182 2023-12-23 09:24:49.000000 Starco-3.1.9/starco/gateways/gates/zibalpay.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/gui/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     9174 2024-03-31 08:39:11.000000 Starco-3.1.9/starco/gui/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    32861 2024-03-16 18:40:57.000000 Starco-3.1.9/starco/gui/utils.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/hetzner/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     6113 2023-12-25 18:28:35.000000 Starco-3.1.9/starco/hetzner/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.898475 Starco-3.1.9/starco/pkl/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2208 2023-11-10 08:07:45.000000 Starco-3.1.9/starco/pkl/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/proxy/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2248 2023-12-01 08:40:12.000000 Starco-3.1.9/starco/proxy/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/scraper/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1693 2024-05-03 15:02:33.000000 Starco-3.1.9/starco/scraper/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/tlg/
+-rw-rw-r--   0 starco    (1000) starco    (1000)       35 2024-01-09 13:06:48.000000 Starco-3.1.9/starco/tlg/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/tlg/app/
+-rw-rw-r--   0 starco    (1000) starco    (1000)    38618 2024-02-24 13:24:00.000000 Starco-3.1.9/starco/tlg/app/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      812 2024-01-09 13:06:48.000000 Starco-3.1.9/starco/tlg/app/utils.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/tlg/bot/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     6864 2024-01-16 10:26:32.000000 Starco-3.1.9/starco/tlg/bot/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    47327 2024-01-09 14:36:18.000000 Starco-3.1.9/starco/tlg/bot/base.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3146 2024-01-09 13:06:48.000000 Starco-3.1.9/starco/tlg/bot/classes.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/tlg/bot/util/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2024-01-09 13:06:48.000000 Starco-3.1.9/starco/tlg/bot/util/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      849 2024-01-11 11:40:27.000000 Starco-3.1.9/starco/tlg/bot/util/enum.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4701 2024-01-09 13:06:48.000000 Starco-3.1.9/starco/tlg/bot/util/filteres.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     5494 2024-02-24 13:19:42.000000 Starco-3.1.9/starco/tlg/bot/util/functions.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    35667 2024-02-24 13:21:45.000000 Starco-3.1.9/starco/tlg/bot/util/packs.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/utils/
+-rw-rw-r--   0 starco    (1000) starco    (1000)      125 2023-12-25 07:41:52.000000 Starco-3.1.9/starco/utils/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      951 2023-12-03 09:46:31.000000 Starco-3.1.9/starco/utils/directories.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1469 2024-02-24 13:20:03.000000 Starco-3.1.9/starco/utils/ext.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1323 2023-12-06 19:14:01.000000 Starco-3.1.9/starco/utils/scheduler.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      823 2024-03-24 07:26:00.000000 Starco-3.1.9/starco/utils/structures.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2247 2024-01-01 09:30:33.000000 Starco-3.1.9/starco/utils/time.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/wp_api/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4370 2023-12-15 13:34:21.000000 Starco-3.1.9/starco/wp_api/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/wscraper/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     8212 2024-05-25 08:01:27.000000 Starco-3.1.9/starco/wscraper/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 08:54:42.902475 Starco-3.1.9/starco/xray_connctor/
+-rw-rw-r--   0 starco    (1000) starco    (1000)    10800 2024-05-10 20:32:56.000000 Starco-3.1.9/starco/xray_connctor/__init__.py
```

### Comparing `Starco-3.1.8/PKG-INFO` & `Starco-3.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Starco
-Version: 3.1.8
+Version: 3.1.9
 Author: Mojtaba Tahmasbi
 Requires-Dist: cffi==1.15.1
 Requires-Dist: cryptography==41.0.3
 Requires-Dist: pycparser==2.21
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.3
 Requires-Dist: requests==2.31.0
```

### Comparing `Starco-3.1.8/Starco.egg-info/PKG-INFO` & `Starco-3.1.9/Starco.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Starco
-Version: 3.1.8
+Version: 3.1.9
 Author: Mojtaba Tahmasbi
 Requires-Dist: cffi==1.15.1
 Requires-Dist: cryptography==41.0.3
 Requires-Dist: pycparser==2.21
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.3
 Requires-Dist: requests==2.31.0
```

### Comparing `Starco-3.1.8/Starco.egg-info/SOURCES.txt` & `Starco-3.1.9/Starco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/setup.py` & `Starco-3.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
     'selenium==4.17.2',
     'pyperclip==1.8.2',
     
 ]
 
 setup(
     name = 'Starco',long_description='starco project',
-    version='3.1.8',
+    version='3.1.9',
     author='Mojtaba Tahmasbi',
     packages=find_packages(),
     install_requires=requires,
 )
```

### Comparing `Starco-3.1.8/starco/cloudflare/__init__.py` & `Starco-3.1.9/starco/cloudflare/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/crypto_gates/nowpayments/__init__.py` & `Starco-3.1.9/starco/crypto_gates/nowpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/db/__init__.py` & `Starco-3.1.9/starco/db/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/debug/__init__.py` & `Starco-3.1.9/starco/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/__init__.py` & `Starco-3.1.9/starco/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/aqayepardakht.py` & `Starco-3.1.9/starco/gateways/gates/aqayepardakht.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/idpay.py` & `Starco-3.1.9/starco/gateways/gates/idpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/nextpay.py` & `Starco-3.1.9/starco/gateways/gates/nextpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/utils.py` & `Starco-3.1.9/starco/gateways/gates/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/vandar.py` & `Starco-3.1.9/starco/gateways/gates/vandar.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gateways/gates/zibalpay.py` & `Starco-3.1.9/starco/gateways/gates/zibalpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gui/__init__.py` & `Starco-3.1.9/starco/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/gui/utils.py` & `Starco-3.1.9/starco/gui/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/hetzner/__init__.py` & `Starco-3.1.9/starco/hetzner/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/pkl/__init__.py` & `Starco-3.1.9/starco/pkl/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/proxy/__init__.py` & `Starco-3.1.9/starco/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/scraper/__init__.py` & `Starco-3.1.9/starco/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/app/__init__.py` & `Starco-3.1.9/starco/tlg/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/app/utils.py` & `Starco-3.1.9/starco/tlg/app/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/__init__.py` & `Starco-3.1.9/starco/tlg/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/base.py` & `Starco-3.1.9/starco/tlg/bot/base.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/classes.py` & `Starco-3.1.9/starco/tlg/bot/classes.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/util/enum.py` & `Starco-3.1.9/starco/tlg/bot/util/enum.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/util/filteres.py` & `Starco-3.1.9/starco/tlg/bot/util/filteres.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/util/functions.py` & `Starco-3.1.9/starco/tlg/bot/util/functions.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/tlg/bot/util/packs.py` & `Starco-3.1.9/starco/tlg/bot/util/packs.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/utils/directories.py` & `Starco-3.1.9/starco/utils/directories.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/utils/ext.py` & `Starco-3.1.9/starco/utils/ext.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/utils/scheduler.py` & `Starco-3.1.9/starco/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/utils/structures.py` & `Starco-3.1.9/starco/utils/structures.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/utils/time.py` & `Starco-3.1.9/starco/utils/time.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/wp_api/__init__.py` & `Starco-3.1.9/starco/wp_api/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.1.8/starco/xray_connctor/__init__.py` & `Starco-3.1.9/starco/xray_connctor/__init__.py`

 * *Files identical despite different names*

