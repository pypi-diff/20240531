# Comparing `tmp/django_jalali_date-1.1.1.tar.gz` & `tmp/django_jalali_date-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jalali_date-1.1.1.tar", last modified: Tue May 28 06:09:22 2024, max compression
+gzip compressed data, was "django_jalali_date-1.1.2.tar", last modified: Fri May 31 07:19:37 2024, max compression
```

## Comparing `django_jalali_date-1.1.1.tar` & `django_jalali_date-1.1.2.tar`

### file list

```diff
@@ -1,59 +1,69 @@
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/
--rw-rw-r--   0 arman     (1000) arman     (1000)     1070 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/LICENSE
--rw-rw-r--   0 arman     (1000) arman     (1000)       99 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/MANIFEST.in
--rw-r--r--   0 arman     (1000) arman     (1000)     7115 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)     6166 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/README.md
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/django_jalali_date.egg-info/
--rw-r--r--   0 arman     (1000) arman     (1000)     7115 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)     2234 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/SOURCES.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/dependency_links.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/not-zip-safe
--rw-rw-r--   0 arman     (1000) arman     (1000)       17 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/requires.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       12 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/top_level.txt
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/
--rw-rw-r--   0 arman     (1000) arman     (1000)      523 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     3401 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/admin.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1930 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/fields.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1277 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/settings.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/
--rw-rw-r--   0 arman     (1000) arman     (1000)     9386 2024-05-28 05:49:47.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
--rw-rw-r--   0 arman     (1000) arman     (1000)    45960 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
--rw-rw-r--   0 arman     (1000) arman     (1000)     3991 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
--rw-rw-r--   0 arman     (1000) arman     (1000)    93107 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
--rw-rw-r--   0 arman     (1000) arman     (1000)   140036 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
--rw-rw-r--   0 arman     (1000) arman     (1000)     8198 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
--rw-rw-r--   0 arman     (1000) arman     (1000)     4296 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
--rw-rw-r--   0 arman     (1000) arman     (1000)    77969 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
--rw-rw-r--   0 arman     (1000) arman     (1000)     6992 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)     6988 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)     6999 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)     6299 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
--rw-rw-r--   0 arman     (1000) arman     (1000)    19200 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/static/admin/js/
--rw-rw-r--   0 arman     (1000) arman     (1000)   254920 2024-05-28 05:45:55.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali..js
--rw-rw-r--   0 arman     (1000) arman     (1000)   139578 2024-05-28 05:49:08.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali.min.js
--rw-rw-r--   0 arman     (1000) arman     (1000)      338 2024-05-28 05:45:58.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/main.js
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/templates/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/templates/admin/
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/
--rw-rw-r--   0 arman     (1000) arman     (1000)     2365 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html
--rw-rw-r--   0 arman     (1000) arman     (1000)     4301 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templates/admin/includes/
--rw-rw-r--   0 arman     (1000) arman     (1000)     2232 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/includes/jalali_fieldset.html
--rw-rw-r--   0 arman     (1000) arman     (1000)      191 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/jalali_change_form.html
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templates/admin/widgets/
--rw-rw-r--   0 arman     (1000) arman     (1000)      234 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/widgets/jalali_split_datetime.html
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templatetags/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templatetags/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     2002 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templatetags/jalali_tags.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     2055 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/widgets.py
--rw-rw-r--   0 arman     (1000) arman     (1000)       76 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/setup.cfg
--rw-rw-r--   0 arman     (1000) arman     (1000)     1335 2024-05-28 05:57:42.000000 django_jalali_date-1.1.1/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1070 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)       99 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/MANIFEST.in
+-rw-r--r--   0 arman     (1000) arman     (1000)     7771 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6464 2024-05-31 07:13:03.000000 django_jalali_date-1.1.2/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/django_jalali_date.egg-info/
+-rw-r--r--   0 arman     (1000) arman     (1000)     7771 2024-05-31 07:19:37.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2522 2024-05-31 07:19:37.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-31 07:19:37.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-28 06:09:22.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/not-zip-safe
+-rw-rw-r--   0 arman     (1000) arman     (1000)       17 2024-05-31 07:19:37.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       18 2024-05-31 07:19:37.000000 django_jalali_date-1.1.2/django_jalali_date.egg-info/top_level.txt
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.452564 django_jalali_date-1.1.2/jalali_date/
+-rw-rw-r--   0 arman     (1000) arman     (1000)      523 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3401 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/admin.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1930 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/fields.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1277 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/settings.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.448564 django_jalali_date-1.1.2/jalali_date/static/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.448564 django_jalali_date-1.1.2/jalali_date/static/admin/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.452564 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     9386 2024-05-28 05:49:47.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.452564 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    45960 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3991 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)    93107 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)   140036 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8198 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4296 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)    77969 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.448564 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.452564 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.456564 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6992 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6988 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6999 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6299 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)    19200 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.456564 django_jalali_date-1.1.2/jalali_date/static/admin/js/
+-rw-rw-r--   0 arman     (1000) arman     (1000)   254920 2024-05-28 05:45:55.000000 django_jalali_date-1.1.2/jalali_date/static/admin/js/django_jalali..js
+-rw-rw-r--   0 arman     (1000) arman     (1000)   139578 2024-05-28 05:49:08.000000 django_jalali_date-1.1.2/jalali_date/static/admin/js/django_jalali.min.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)      338 2024-05-28 05:45:58.000000 django_jalali_date-1.1.2/jalali_date/static/admin/js/main.js
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.448564 django_jalali_date-1.1.2/jalali_date/templates/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/jalali_date/templates/admin/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/jalali_date/templates/admin/edit_inline/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2365 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templates/admin/edit_inline/jalali_stacked.html
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4301 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templates/admin/edit_inline/jalali_tabular.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/jalali_date/templates/admin/includes/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2232 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templates/admin/includes/jalali_fieldset.html
+-rw-rw-r--   0 arman     (1000) arman     (1000)      191 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templates/admin/jalali_change_form.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/jalali_date/templates/admin/widgets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)      234 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templates/admin/widgets/jalali_split_datetime.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/jalali_date/templatetags/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/templatetags/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2381 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/jalali_date/templatetags/jalali_tags.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2055 2024-05-28 05:21:27.000000 django_jalali_date-1.1.2/jalali_date/widgets.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)       76 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1686 2024-05-31 07:18:50.000000 django_jalali_date-1.1.2/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)       63 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/test_settings.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/tests/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/tests/__init__.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-31 07:19:37.460564 django_jalali_date-1.1.2/tests/tests/templatetags/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/tests/templatetags/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3040 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/tests/templatetags/test_jalali_admin_safe_readonly_template_tag.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1765 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/tests/templatetags/test_jalali_now_template_tag.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2167 2024-05-31 06:46:08.000000 django_jalali_date-1.1.2/tests/tests/templatetags/test_to_jalali_template_tag.py
```

### Comparing `django_jalali_date-1.1.1/LICENSE` & `django_jalali_date-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/PKG-INFO` & `django_jalali_date-1.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 Metadata-Version: 2.1
 Name: django-jalali-date
-Version: 1.1.1
+Version: 1.1.2
 Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
 Home-page: http://github.com/a-roomana/django-jalali-date
 Download-URL: https://pypi.python.org/pypi/django-jalali-date/
 Author: Arman Roomana
 Author-email: roomana.arman@gmail.com
 License: MIT
 Keywords: django jalali date
 Platform: any
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: jdatetime
 
 
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+[![Github Tests](https://github.com/a-roomana/django-jalali-date/workflows/Tests/badge.svg?branch=master)](https://github.com/a-roomana/django-jalali-date/actions)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
 [![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+
 # django-jalali-date
 
 Jalali Date support for user interface. Easy conversion of DateTimeField to JalaliDateTimeField within the admin site, view and templates.
 
 
 ## Dependency
```

### Comparing `django_jalali_date-1.1.1/README.md` & `django_jalali_date-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+[![Github Tests](https://github.com/a-roomana/django-jalali-date/workflows/Tests/badge.svg?branch=master)](https://github.com/a-roomana/django-jalali-date/actions)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
 [![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+
 # django-jalali-date
 
 Jalali Date support for user interface. Easy conversion of DateTimeField to JalaliDateTimeField within the admin site, view and templates.
 
 
 ## Dependency
```

### Comparing `django_jalali_date-1.1.1/django_jalali_date.egg-info/PKG-INFO` & `django_jalali_date-1.1.2/django_jalali_date.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 Metadata-Version: 2.1
 Name: django-jalali-date
-Version: 1.1.1
+Version: 1.1.2
 Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
 Home-page: http://github.com/a-roomana/django-jalali-date
 Download-URL: https://pypi.python.org/pypi/django-jalali-date/
 Author: Arman Roomana
 Author-email: roomana.arman@gmail.com
 License: MIT
 Keywords: django jalali date
 Platform: any
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: jdatetime
 
 
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+[![Github Tests](https://github.com/a-roomana/django-jalali-date/workflows/Tests/badge.svg?branch=master)](https://github.com/a-roomana/django-jalali-date/actions)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
 [![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+
 # django-jalali-date
 
 Jalali Date support for user interface. Easy conversion of DateTimeField to JalaliDateTimeField within the admin site, view and templates.
 
 
 ## Dependency
```

### Comparing `django_jalali_date-1.1.1/django_jalali_date.egg-info/SOURCES.txt` & `django_jalali_date-1.1.2/django_jalali_date.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -34,8 +34,15 @@
 jalali_date/static/admin/js/main.js
 jalali_date/templates/admin/jalali_change_form.html
 jalali_date/templates/admin/edit_inline/jalali_stacked.html
 jalali_date/templates/admin/edit_inline/jalali_tabular.html
 jalali_date/templates/admin/includes/jalali_fieldset.html
 jalali_date/templates/admin/widgets/jalali_split_datetime.html
 jalali_date/templatetags/__init__.py
-jalali_date/templatetags/jalali_tags.py
+jalali_date/templatetags/jalali_tags.py
+tests/__init__.py
+tests/test_settings.py
+tests/tests/__init__.py
+tests/tests/templatetags/__init__.py
+tests/tests/templatetags/test_jalali_admin_safe_readonly_template_tag.py
+tests/tests/templatetags/test_jalali_now_template_tag.py
+tests/tests/templatetags/test_to_jalali_template_tag.py
```

### Comparing `django_jalali_date-1.1.1/jalali_date/__init__.py` & `django_jalali_date-1.1.2/jalali_date/__init__.py`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/admin.py` & `django_jalali_date-1.1.2/jalali_date/admin.py`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/fields.py` & `django_jalali_date-1.1.2/jalali_date/fields.py`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/settings.py` & `django_jalali_date-1.1.2/jalali_date/settings.py`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css` & `django_jalali_date-1.1.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali..js` & `django_jalali_date-1.1.2/jalali_date/static/admin/js/django_jalali..js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali.min.js` & `django_jalali_date-1.1.2/jalali_date/static/admin/js/django_jalali.min.js`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html` & `django_jalali_date-1.1.2/jalali_date/templates/admin/edit_inline/jalali_stacked.html`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html` & `django_jalali_date-1.1.2/jalali_date/templates/admin/edit_inline/jalali_tabular.html`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/templates/admin/includes/jalali_fieldset.html` & `django_jalali_date-1.1.2/jalali_date/templates/admin/includes/jalali_fieldset.html`

 * *Files identical despite different names*

### Comparing `django_jalali_date-1.1.1/jalali_date/templatetags/jalali_tags.py` & `django_jalali_date-1.1.2/jalali_date/templatetags/jalali_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,23 +23,33 @@
 	def __str__(self):
 		return self.value
 
 	def contents(self):
 		return self.value
 
 
+def normalize_strftime(strftime):
+	"""
+	Normalize strftime values to make sure their usable for datetime libraries.
+	"""
+	if not isinstance(strftime, str):
+		# Convert non-str values to str to support stuff like "lazy_translations".
+		strftime = str(strftime)
+	return strftime
+
+
 @register.filter
 def to_jalali(g_date, strftime=None):
 	if g_date is None:
 		return '-'
 	elif isinstance(g_date, datetime):
-		strftime = strftime if strftime else DEFAULTS['Strftime']['datetime']
+		strftime = normalize_strftime(strftime if strftime else DEFAULTS['Strftime']['datetime'])
 		return datetime2jalali(g_date).strftime(strftime)
 	elif isinstance(g_date, date):
-		strftime = strftime if strftime else DEFAULTS['Strftime']['date']
+		strftime = normalize_strftime(strftime if strftime else DEFAULTS['Strftime']['date'])
 		return date2jalali(g_date).strftime(strftime)
 	return '-'
 
 
 @register.filter
 def jalali_admin_safe_readonly(readonly_field, strftime=None):
 	"""
@@ -51,22 +61,22 @@
 	field_name = readonly_field.field['field']
 
 	if not hasattr(instance, field_name):
 		return readonly_field
 
 	field = getattr(instance, field_name)
 	if isinstance(field, datetime):
-		strftime = strftime if strftime else DEFAULTS['Strftime']['datetime']
+		strftime = normalize_strftime(strftime if strftime else DEFAULTS['Strftime']['datetime'])
 		return ObjectContents(datetime2jalali(field).strftime(strftime))
 	elif isinstance(field, date):
-		strftime = strftime if strftime else DEFAULTS['Strftime']['date']
+		strftime = normalize_strftime(strftime if strftime else DEFAULTS['Strftime']['date'])
 		return ObjectContents(date2jalali(field).strftime(strftime))
 	elif field is None:
 		return ObjectContents('-')
 
 	return readonly_field
 
 
 @register.simple_tag
 def jalali_now(strftime=None):
-	strftime = strftime if strftime else DEFAULTS['Strftime']['datetime']
+	strftime = normalize_strftime(strftime if strftime else DEFAULTS['Strftime']['datetime'])
 	return datetime2jalali(datetime.now()).strftime(strftime)
```

### Comparing `django_jalali_date-1.1.1/jalali_date/widgets.py` & `django_jalali_date-1.1.2/jalali_date/widgets.py`

 * *Files identical despite different names*

