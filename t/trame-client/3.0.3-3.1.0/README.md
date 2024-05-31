# Comparing `tmp/trame-client-3.0.3.tar.gz` & `tmp/trame-client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-3.0.3.tar", last modified: Thu May 16 18:26:26 2024, max compression
+gzip compressed data, was "trame-client-3.1.0.tar", last modified: Fri May 31 20:40:42 2024, max compression
```

## Comparing `trame-client-3.0.3.tar` & `trame-client-3.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.674174 trame-client-3.0.3/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-05-16 18:25:57.000000 trame-client-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-16 18:25:57.000000 trame-client-3.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3539 2024-05-16 18:26:26.674174 trame-client-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2024-05-16 18:25:57.000000 trame-client-3.0.3/README.rst
--rw-r--r--   0 root         (0) root         (0)      935 2024-05-16 18:26:26.674174 trame-client-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 18:25:57.000000 trame-client-3.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.662174 trame-client-3.0.3/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.662174 trame-client-3.0.3/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.670174 trame-client-3.0.3/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    26057 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/js/app.7d0e64a7.js
--rw-r--r--   0 root         (0) root         (0)   156057 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
--rw-r--r--   0 root         (0) root         (0)     2890 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2024-05-16 18:26:17.000000 trame-client-3.0.3/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.670174 trame-client-3.0.3/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.670174 trame-client-3.0.3/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   102131 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/assets/index-75032529.js
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/assets/index-e80c1ba5.css
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     2890 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   147534 2024-05-16 18:26:23.000000 trame-client-3.0.3/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.670174 trame-client-3.0.3/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.670174 trame-client-3.0.3/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9369 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.674174 trame-client-3.0.3/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1134 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/formatter.py
--rw-r--r--   0 root         (0) root         (0)      343 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     3816 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/testing.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/version.py
--rw-r--r--   0 root         (0) root         (0)     3190 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/utils/web_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.674174 trame-client-3.0.3/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22879 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     9071 2024-05-16 18:25:57.000000 trame-client-3.0.3/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 18:26:26.666174 trame-client-3.0.3/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3539 2024-05-16 18:26:26.000000 trame-client-3.0.3/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-16 18:26:26.000000 trame-client-3.0.3/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 18:26:26.000000 trame-client-3.0.3/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-16 18:26:26.000000 trame-client-3.0.3/trame_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-16 18:26:26.000000 trame-client-3.0.3/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.138555 trame-client-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-05-31 20:40:12.000000 trame-client-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-31 20:40:12.000000 trame-client-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-05-31 20:40:42.138555 trame-client-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-05-31 20:40:12.000000 trame-client-3.1.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      935 2024-05-31 20:40:42.138555 trame-client-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 20:40:12.000000 trame-client-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.126555 trame-client-3.1.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.126555 trame-client-3.1.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.126555 trame-client-3.1.0/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.126555 trame-client-3.1.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.126555 trame-client-3.1.0/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    26057 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/js/app.7d0e64a7.js
+-rw-r--r--   0 root         (0) root         (0)   156057 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2024-05-31 20:40:33.000000 trame-client-3.1.0/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.134555 trame-client-3.1.0/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.134555 trame-client-3.1.0/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   102131 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/assets/index-75032529.js
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/assets/index-e80c1ba5.css
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   147534 2024-05-31 20:40:38.000000 trame-client-3.1.0/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.134555 trame-client-3.1.0/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.134555 trame-client-3.1.0/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.134555 trame-client-3.1.0/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/formatter.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/testing.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/version.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/utils/web_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.138555 trame-client-3.1.0/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23244 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-05-31 20:40:12.000000 trame-client-3.1.0/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 20:40:42.130555 trame-client-3.1.0/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-05-31 20:40:42.000000 trame-client-3.1.0/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-31 20:40:42.000000 trame-client-3.1.0/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 20:40:42.000000 trame-client-3.1.0/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 20:40:42.000000 trame-client-3.1.0/trame_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-31 20:40:42.000000 trame-client-3.1.0/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-3.0.3/LICENSE` & `trame-client-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/PKG-INFO` & `trame-client-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.3
+Version: 3.1.0
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.3/README.rst` & `trame-client-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/setup.cfg` & `trame-client-3.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 3.0.3
+version = 3.1.0
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-3.0.3/trame_client/LICENSE` & `trame-client-3.1.0/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/encoders/numpy.py` & `trame-client-3.1.0/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-3.1.0/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/index.html` & `trame-client-3.1.0/trame_client/module/vue2-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/js/app.7d0e64a7.js` & `trame-client-3.1.0/trame_client/module/vue2-www/js/app.7d0e64a7.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js` & `trame-client-3.1.0/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/loading.tpl` & `trame-client-3.1.0/trame_client/module/vue2-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/logo.png` & `trame-client-3.1.0/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue2-www/vue.global.js` & `trame-client-3.1.0/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/assets/index-75032529.js` & `trame-client-3.1.0/trame_client/module/vue3-www/assets/index-75032529.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/assets/index-e80c1ba5.css` & `trame-client-3.1.0/trame_client/module/vue3-www/assets/index-e80c1ba5.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/index.html` & `trame-client-3.1.0/trame_client/module/vue3-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/loading.tpl` & `trame-client-3.1.0/trame_client/module/vue3-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/logo.png` & `trame-client-3.1.0/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/module/vue3-www/vue.global.js` & `trame-client-3.1.0/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/resources/attributes.json` & `trame-client-3.1.0/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/resources/vue.json` & `trame-client-3.1.0/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/ui/core.py` & `trame-client-3.1.0/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/ui/html.py` & `trame-client-3.1.0/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/utils/formatter.py` & `trame-client-3.1.0/trame_client/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/utils/testing.py` & `trame-client-3.1.0/trame_client/utils/testing.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/utils/version.py` & `trame-client-3.1.0/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/utils/web_module.py` & `trame-client-3.1.0/trame_client/utils/web_module.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/widgets/core.py` & `trame-client-3.1.0/trame_client/widgets/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -337,14 +337,29 @@
         """Return the associated server"""
         return self._server
 
     def set_server(self, v):
         """Update the associated server"""
         self._server = v
 
+    @property
+    def state(self):
+        """Return the associated server state"""
+        return self.server.state
+
+    @property
+    def ctrl(self):
+        """Return the associated server controller"""
+        return self.server.controller
+
+    @property
+    def ctx(self):
+        """Return the associated server context"""
+        return self.server.context
+
     # -------------------------------------------------------------------------
     # Buildin API
     # -------------------------------------------------------------------------
 
     def __getitem__(self, name):
         return self._py_attr[name]
```

### Comparing `trame-client-3.0.3/trame_client/widgets/generator.py` & `trame-client-3.1.0/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/widgets/html.py` & `trame-client-3.1.0/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client/widgets/trame.py` & `trame-client-3.1.0/trame_client/widgets/trame.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.3/trame_client.egg-info/PKG-INFO` & `trame-client-3.1.0/trame_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.3
+Version: 3.1.0
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.3/trame_client.egg-info/SOURCES.txt` & `trame-client-3.1.0/trame_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

