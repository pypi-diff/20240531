# Comparing `tmp/pretix-adyen-1.4.3.tar.gz` & `tmp/pretix_adyen-1.4.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-adyen-1.4.3.tar", last modified: Wed Mar 27 08:26:10 2024, max compression
+gzip compressed data, was "pretix_adyen-1.4.4.post2.tar", last modified: Fri May 31 12:04:15 2024, max compression
```

## Comparing `pretix-adyen-1.4.3.tar` & `pretix_adyen-1.4.4.post2.tar`

### file list

```diff
@@ -1,61 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.708039 pretix-adyen-1.4.3/
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1969 2024-03-27 08:26:10.708039 pretix-adyen-1.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6325 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9303 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9223 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6089 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6064 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9559 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6618 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    28349 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/payment.py
--rw-rw-rw-   0 root         (0) root         (0)    19433 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.704039 pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/adyen_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/pretix-adyen.css
--rw-rw-rw-   0 root         (0) root         (0)     5715 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/pretix-adyen.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.700039 pretix-adyen-1.4.3/pretix_adyen/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.708039 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/control.html
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/control_settings.html
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/presale_head.html
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/sca.html
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1715 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9302 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pretix_adyen/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 08:26:10.708039 pretix-adyen-1.4.3/pretix_adyen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1969 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1450 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-27 08:26:10.000000 pretix-adyen-1.4.3/pretix_adyen.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-03-27 08:26:10.708039 pretix-adyen-1.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-03-27 08:25:47.000000 pretix-adyen-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.094661 pretix_adyen-1.4.4.post2/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-05-31 12:04:15.094661 pretix_adyen-1.4.4.post2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-31 12:04:07.000000 pretix_adyen-1.4.4.post2/pretix_adyen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6325 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9303 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 12:04:08.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9559 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6618 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/sk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/sk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10851 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/locale/uk/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    28349 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)    19433 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.090661 pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 12:04:08.000000 pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/adyen_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/pretix-adyen.css
+-rw-rw-rw-   0 root         (0) root         (0)     5715 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/pretix-adyen.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.086661 pretix_adyen-1.4.4.post2/pretix_adyen/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.094661 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 12:04:08.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/control_settings.html
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/presale_head.html
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/sca.html
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9302 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pretix_adyen/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:04:15.094661 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1540 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-31 12:04:15.000000 pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-31 12:04:15.094661 pretix_adyen-1.4.4.post2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-31 12:02:58.000000 pretix_adyen-1.4.4.post2/setup.py
```

### Comparing `pretix-adyen-1.4.3/LICENSE` & `pretix_adyen-1.4.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/PKG-INFO` & `pretix_adyen-1.4.4.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-adyen
-Version: 1.4.3
+Version: 1.4.4.post2
 Summary: This plugin allows to use Adyen as a payment provider
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2020 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-adyen-1.4.3/README.rst` & `pretix_adyen-1.4.4.post2/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/apps.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/cs/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/de/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/django.pot` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/hr/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/nl/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix_adyen-1.4.4.post2/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/payment.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/paymentmethods.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/signals.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/adyen_logo.svg` & `pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/adyen_logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/static/pretix_adyen/pretix-adyen.js` & `pretix_adyen-1.4.4.post2/pretix_adyen/static/pretix_adyen/pretix-adyen.js`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/control.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/control.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/control_settings.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/control_settings.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/pending.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/presale_head.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/presale_head.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/templates/pretix_adyen/sca.html` & `pretix_adyen-1.4.4.post2/pretix_adyen/templates/pretix_adyen/sca.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/utils.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/utils.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen/views.py` & `pretix_adyen-1.4.4.post2/pretix_adyen/views.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/pretix_adyen.egg-info/PKG-INFO` & `pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-adyen
-Version: 1.4.3
+Version: 1.4.4.post2
 Summary: This plugin allows to use Adyen as a payment provider
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2020 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-adyen-1.4.3/pretix_adyen.egg-info/SOURCES.txt` & `pretix_adyen-1.4.4.post2/pretix_adyen.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 pretix_adyen/locale/cs/LC_MESSAGES/django.po
 pretix_adyen/locale/de/LC_MESSAGES/django.po
 pretix_adyen/locale/de_Informal/.gitkeep
 pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
 pretix_adyen/locale/hr/LC_MESSAGES/django.po
 pretix_adyen/locale/nl/LC_MESSAGES/django.po
 pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
+pretix_adyen/locale/sk/LC_MESSAGES/django.po
+pretix_adyen/locale/uk/LC_MESSAGES/django.po
 pretix_adyen/static/pretix_adyen/.gitkeep
 pretix_adyen/static/pretix_adyen/adyen_logo.svg
 pretix_adyen/static/pretix_adyen/pretix-adyen.css
 pretix_adyen/static/pretix_adyen/pretix-adyen.js
 pretix_adyen/templates/pretix_adyen/.gitkeep
 pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
 pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
```

### Comparing `pretix-adyen-1.4.3/pyproject.toml` & `pretix_adyen-1.4.4.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.4.3/setup.cfg` & `pretix_adyen-1.4.4.post2/setup.cfg`

 * *Files identical despite different names*

