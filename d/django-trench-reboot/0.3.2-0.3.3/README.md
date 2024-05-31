# Comparing `tmp/django_trench_reboot-0.3.2.tar.gz` & `tmp/django_trench_reboot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trench_reboot-0.3.2.tar", last modified: Wed May 29 21:48:46 2024, max compression
+gzip compressed data, was "django_trench_reboot-0.3.3.tar", last modified: Fri May 31 15:15:23 2024, max compression
```

## Comparing `django_trench_reboot-0.3.2.tar` & `django_trench_reboot-0.3.3.tar`

### file list

```diff
@@ -1,96 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-29 21:48:46.000000 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 21:48:46.000000 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:48:46.000000 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-29 21:48:46.000000 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 21:48:46.000000 django_trench_reboot-0.3.2/django_trench_reboot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.973859 django_trench_reboot-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.973859 django_trench_reboot-0.3.2/trench/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.973859 django_trench_reboot-0.3.2/trench/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/basic_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/sms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/backends/yubikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.977859 django_trench_reboot-0.3.2/trench/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/activate_mfa_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/authenticate_second_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/authenticate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/create_mfa_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/create_otp.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/create_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/deactivate_mfa_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/generate_backup_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/remove_backup_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/replace_mfa_method_backup_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/set_primary_mfa_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/command/validate_backup_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.977859 django_trench_reboot-0.3.2/trench/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.977859 django_trench_reboot-0.3.2/trench/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.977859 django_trench_reboot-0.3.2/trench/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.977859 django_trench_reboot-0.3.2/trench/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/0002_auto_20190111_1403.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/0003_auto_20190213_2330.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/0004_alter_mfamethod_id_mfamethod_unique_user_is_primary_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/0005_remove_mfamethod_primary_is_active_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/trench/query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/query/get_mfa_config_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/templates/trench/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.969859 django_trench_reboot-0.3.2/trench/templates/trench/backends/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/trench/templates/trench/backends/email/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/templates/trench/backends/email/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/templates/trench/backends/email/code.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/trench/urls/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/urls/authtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/urls/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/urls/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:48:46.981859 django_trench_reboot-0.3.2/trench/views/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/views/authtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 21:48:43.000000 django_trench_reboot-0.3.2/trench/views/jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.277374 django_trench_reboot-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-31 15:15:23.277374 django_trench_reboot-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-31 15:15:23.000000 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-31 15:15:23.000000 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:15:23.000000 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-31 15:15:23.000000 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 15:15:23.000000 django_trench_reboot-0.3.3/django_trench_reboot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.265374 django_trench_reboot-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-31 15:15:23.277374 django_trench_reboot-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.269374 django_trench_reboot-0.3.3/trench/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.269374 django_trench_reboot-0.3.3/trench/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/basic_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/sms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/backends/yubikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/activate_mfa_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/authenticate_second_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/authenticate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/create_mfa_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/create_otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/create_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/deactivate_mfa_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/generate_backup_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/remove_backup_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/replace_mfa_method_backup_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/set_primary_mfa_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/command/validate_backup_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.261374 django_trench_reboot-0.3.3/trench/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.261374 django_trench_reboot-0.3.3/trench/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.261374 django_trench_reboot-0.3.3/trench/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.261374 django_trench_reboot-0.3.3/trench/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/migrations/0002_auto_20190111_1403.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/migrations/0003_auto_20190213_2330.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/query/get_mfa_config_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.265374 django_trench_reboot-0.3.3/trench/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.265374 django_trench_reboot-0.3.3/trench/templates/trench/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.265374 django_trench_reboot-0.3.3/trench/templates/trench/backends/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/templates/trench/backends/email/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/templates/trench/backends/email/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/templates/trench/backends/email/code.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/urls/authtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/urls/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/urls/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:15:23.273374 django_trench_reboot-0.3.3/trench/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/views/authtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-31 15:15:13.000000 django_trench_reboot-0.3.3/trench/views/jwt.py
```

### Comparing `django_trench_reboot-0.3.2/LICENSE` & `django_trench_reboot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/PKG-INFO` & `django_trench_reboot-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-trench-reboot
-Version: 0.3.2
+Version: 0.3.3
 Summary: REST Multi-factor authentication package for Django
 Home-page: https://github.com/Panevo/django-trench
 Author: Karlo Krakan
 Author-email: karlo.krakan@panevo.com
 License: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django_trench_reboot-0.3.2/README.rst` & `django_trench_reboot-0.3.3/README.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -149,8 +149,8 @@
     To do so you need to install the :code:`pytest-xdist` package and run the tests
     with additional parameter of :code:`-n 8` where :code:`8` stands for the number
     of threads that will be spawned for executing the tests. Depending on the machine
     you're using using this tool can speed up the test execution process up to 5 times.
 
     .. code-block:: shell
 
-        pytest -n 8 --cov=testproject/trench testproject/tests/
+        pytest -n 8 --cov=testproject/trench testproject/tests/
```

### Comparing `django_trench_reboot-0.3.2/django_trench_reboot.egg-info/PKG-INFO` & `django_trench_reboot-0.3.3/django_trench_reboot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-trench-reboot
-Version: 0.3.2
+Version: 0.3.3
 Summary: REST Multi-factor authentication package for Django
 Home-page: https://github.com/Panevo/django-trench
 Author: Karlo Krakan
 Author-email: karlo.krakan@panevo.com
 License: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
```

### Comparing `django_trench_reboot-0.3.2/django_trench_reboot.egg-info/SOURCES.txt` & `django_trench_reboot-0.3.3/django_trench_reboot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 trench/models.py
 trench/responses.py
 trench/serializers.py
 trench/settings.py
 trench/utils.py
 trench/backends/__init__.py
 trench/backends/application.py
-trench/backends/aws.py
 trench/backends/base.py
 trench/backends/basic_mail.py
 trench/backends/provider.py
 trench/backends/sms_api.py
 trench/backends/twilio.py
 trench/backends/yubikey.py
 trench/command/__init__.py
@@ -53,16 +52,14 @@
 trench/locale/en/LC_MESSAGES/django.mo
 trench/locale/en/LC_MESSAGES/django.po
 trench/locale/pl/LC_MESSAGES/django.mo
 trench/locale/pl/LC_MESSAGES/django.po
 trench/migrations/0001_initial.py
 trench/migrations/0002_auto_20190111_1403.py
 trench/migrations/0003_auto_20190213_2330.py
-trench/migrations/0004_alter_mfamethod_id_mfamethod_unique_user_is_primary_and_more.py
-trench/migrations/0005_remove_mfamethod_primary_is_active_and_more.py
 trench/migrations/__init__.py
 trench/query/__init__.py
 trench/query/get_mfa_config_by_name.py
 trench/templates/trench/backends/email/code.html
 trench/templates/trench/backends/email/code.txt
 trench/urls/__init__.py
 trench/urls/authtoken.py
```

### Comparing `django_trench_reboot-0.3.2/docs/Makefile` & `django_trench_reboot-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/docs/backends.rst` & `django_trench_reboot-0.3.3/docs/backends.rst`

 * *Files 3% similar despite different names*

```diff
@@ -84,19 +84,15 @@
 
 :SOURCE_FIELD: Defines the field name in your ``AUTH_USER_MODEL`` to be looked up and used as field containing the phone number of the recipient of the OTP code.
 :SMSAPI_ACCESS_TOKEN: Access token obtained from `SMS API`_
 :SMSAPI_FROM_NUMBER: This will be used as the sender's phone number.
 
 Authentication apps
 *******************
-| This backend returns OTP based QR link to be scanned by apps like Google Authenticator and Authy.
-
-**Important note:** validity period varies between apps. Use the right value you
-find in a given provider's docs. Setting the wrong value will lead to an error with
-validating MFA code.
+| This backend returns OTP based QR link to be scanned by apps like Gooogle Authenticator and Authy.
 
 .. code-block:: python
 
     TRENCH_AUTH = {
         "MFA_METHODS": {
             "app": {
                 "VERBOSE_NAME": _("app"),
```

### Comparing `django_trench_reboot-0.3.2/docs/conf.py` & `django_trench_reboot-0.3.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 project = "django-trench-reboot"
 copyright = "2018, Merixstudio"
 author = "Merixstudio"
 
 # The short X.Y version
 version = "0.3"
 # The full version, including alpha/beta/rc tags
-release = "0.3.2"
+release = "0.3.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
@@ -192,8 +192,8 @@
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {"https://docs.python.org/": None}
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = True
+todo_include_todos = True
```

### Comparing `django_trench_reboot-0.3.2/docs/endpoints.rst` & `django_trench_reboot-0.3.3/docs/endpoints.rst`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/docs/installation.rst` & `django_trench_reboot-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/docs/introduction.rst` & `django_trench_reboot-0.3.3/docs/introduction.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 * Python
 * Django
 * Django REST Framework
 
 Supported versions
 ******************
 
-* Python 3.7, 3.8. 3.9, 3.10
-* Django 2.x, 3.x, 4.x
-* Django REST Framework >= 3.10
+* Python 3.7, 3.8. 3.9
+* Django 2.x, 3.x,
+* Django REST Framework >= 3.9
 
 Quick Start
 -----------
 
 1. Install the package using pip:
 
 .. code-block:: python
```

### Comparing `django_trench_reboot-0.3.2/docs/settings.rst` & `django_trench_reboot-0.3.3/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/setup.cfg` & `django_trench_reboot-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/setup.py` & `django_trench_reboot-0.3.3/setup.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-)
+)
```

### Comparing `django_trench_reboot-0.3.2/trench/backends/application.py` & `django_trench_reboot-0.3.3/trench/backends/application.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import User
 
 import logging
 
 from trench.backends.base import AbstractMessageDispatcher
 from trench.responses import (
     DispatchResponse,
     FailedDispatchResponse,
     SuccessfulDispatchResponse,
 )
 from trench.settings import trench_settings
 
 
-User: AbstractUser = get_user_model()
-
-
 class ApplicationMessageDispatcher(AbstractMessageDispatcher):
     def dispatch_message(self) -> DispatchResponse:
         try:
             qr_link = self._create_qr_link(self._mfa_method.user)
             return SuccessfulDispatchResponse(details=qr_link)
         except Exception as cause:  # pragma: nocover
             logging.error(cause, exc_info=True)  # pragma: nocover
```

### Comparing `django_trench_reboot-0.3.2/trench/backends/aws.py` & `django_trench_reboot-0.3.3/trench/backends/sms_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from django.utils.translation import gettext_lazy as _
 
 import logging
-import boto3
+from smsapi.client import SmsApiPlClient
+from smsapi.exception import SmsApiException
 
 from trench.backends.base import AbstractMessageDispatcher
 from trench.responses import (
     DispatchResponse,
     FailedDispatchResponse,
     SuccessfulDispatchResponse,
 )
-from trench.settings import AWS_ACCESS_KEY, AWS_SECRET_KEY, AWS_REGION
-from botocore.exceptions import ClientError, EndpointConnectionError
+from trench.settings import SMSAPI_ACCESS_TOKEN, SMSAPI_FROM_NUMBER
 
-class AWSMessageDispatcher(AbstractMessageDispatcher):
+
+class SMSAPIMessageDispatcher(AbstractMessageDispatcher):
     _SMS_BODY = _("Your verification code is: ")
     _SUCCESS_DETAILS = _("SMS message with MFA code has been sent.")
 
     def dispatch_message(self) -> DispatchResponse:
         try:
-            client = boto3.client(
-                "sns",
-                aws_access_key_id=self._config.get(AWS_ACCESS_KEY),
-                aws_secret_access_key=self._config.get(AWS_SECRET_KEY),
-                region_name=self._config.get(AWS_REGION),
-            )
-            client.publish(
-                PhoneNumber=self._to,
-                Message=self._SMS_BODY + self.create_code(),
+            client = SmsApiPlClient(access_token=self._config.get(SMSAPI_ACCESS_TOKEN))
+            from_number = self._config.get(SMSAPI_FROM_NUMBER)
+            kwargs = {"from_": from_number} if from_number else {}
+            client.sms.send(
+                message=self._SMS_BODY + self.create_code(),
+                to=self._to,
+                **kwargs,
             )
             return SuccessfulDispatchResponse(details=self._SUCCESS_DETAILS)
-        except ClientError as cause:
-            logging.error(cause, exc_info=True)
-            return FailedDispatchResponse(details=str(cause))
-        except EndpointConnectionError as cause:
+        except SmsApiException as cause:
             logging.error(cause, exc_info=True)
-            return FailedDispatchResponse(details=str(cause))
+            return FailedDispatchResponse(details=cause.message)
```

### Comparing `django_trench_reboot-0.3.2/trench/backends/base.py` & `django_trench_reboot-0.3.3/trench/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         try:
             objects, attr = path.rsplit(".", 1)
             return objects, attr
         except ValueError:
             return None, path
 
     @staticmethod
-    def _get_innermost_object(obj: Model, dotted_path: Optional[str] = None) -> Model:
+    def _get_innermost_object(obj: Model, dotted_path: str = None) -> Model:
         """
         For given object return innermost object.
         """
         if dotted_path is None:
             return obj
         for o in dotted_path.split("."):
             obj = getattr(obj, o)
@@ -73,14 +73,15 @@
         return self.validate_code(code)
 
     def validate_code(self, code: str) -> bool:
         return self._get_otp().verify(otp=code)
 
     def _get_otp(self) -> TOTP:
         return create_otp_command(
-            secret=self._mfa_method.secret, interval=self._get_valid_window()
+            secret=self._mfa_method.secret,
+            interval=self._get_valid_window()
         )
 
     def _get_valid_window(self) -> int:
         return self._config.get(
             VALIDITY_PERIOD, trench_settings.DEFAULT_VALIDITY_PERIOD
         )
```

### Comparing `django_trench_reboot-0.3.2/trench/backends/basic_mail.py` & `django_trench_reboot-0.3.3/trench/backends/basic_mail.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,10 +32,7 @@
                 recipient_list=(self._to,),
                 fail_silently=False,
             )
             return SuccessfulDispatchResponse(details=self._SUCCESS_DETAILS)
         except SMTPException as cause:  # pragma: nocover
             logging.error(cause, exc_info=True)  # pragma: nocover
             return FailedDispatchResponse(details=str(cause))  # pragma: nocover
-        except ConnectionRefusedError as cause:  # pragma: nocover
-            logging.error(cause, exc_info=True)  # pragma: nocover
-            return FailedDispatchResponse(details=str(cause))  # pragma: nocover
```

### Comparing `django_trench_reboot-0.3.2/trench/backends/twilio.py` & `django_trench_reboot-0.3.3/trench/backends/twilio.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/backends/yubikey.py` & `django_trench_reboot-0.3.3/trench/backends/yubikey.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/activate_mfa_method.py` & `django_trench_reboot-0.3.3/trench/command/activate_mfa_method.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/authenticate_second_factor.py` & `django_trench_reboot-0.3.3/trench/command/authenticate_second_factor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import User
 
 from typing import Type
 
 from trench.backends.provider import get_mfa_handler
 from trench.command.remove_backup_code import remove_backup_code_command
 from trench.command.validate_backup_code import validate_backup_code_command
 from trench.exceptions import InvalidCodeError, InvalidTokenError
 from trench.models import MFAMethod
 from trench.utils import get_mfa_model, user_token_generator
 
 
-User: AbstractUser = get_user_model()
-
-
 class AuthenticateSecondFactorCommand:
     def __init__(self, mfa_model: Type[MFAMethod]) -> None:
         self._mfa_model = mfa_model
 
     def execute(self, code: str, ephemeral_token: str) -> User:
         user = user_token_generator.check_token(user=None, token=ephemeral_token)
         if user is None:
```

### Comparing `django_trench_reboot-0.3.2/trench/command/authenticate_user.py` & `django_trench_reboot-0.3.3/trench/command/authenticate_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from django.contrib.auth import authenticate, get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth import authenticate
+from django.contrib.auth.models import User
 
 from rest_framework.request import Request
 
 from trench.exceptions import UnauthenticatedError
 
 
-User: AbstractUser = get_user_model()
-
-
 class AuthenticateUserCommand:
     @staticmethod
     def execute(request: Request, username: str, password: str) -> User:
         user = authenticate(
             request=request,
             username=username,
             password=password,
```

### Comparing `django_trench_reboot-0.3.2/trench/command/create_mfa_method.py` & `django_trench_reboot-0.3.3/trench/command/create_mfa_method.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/create_secret.py` & `django_trench_reboot-0.3.3/trench/command/create_secret.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/deactivate_mfa_method.py` & `django_trench_reboot-0.3.3/trench/command/deactivate_mfa_method.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         ).count()
         if mfa.is_primary and number_of_active_mfa_methods > 1:
             raise DeactivationOfPrimaryMFAMethodError()
         if not mfa.is_active:
             raise MFANotEnabledError()
 
         self._mfa_model.objects.filter(user_id=user_id, name=mfa_method_name).update(
-            is_active=False, is_primary=False
+            is_active=False
         )
 
 
 deactivate_mfa_method_command = DeactivateMFAMethodCommand(
     mfa_model=get_mfa_model()
 ).execute
```

### Comparing `django_trench_reboot-0.3.2/trench/command/generate_backup_codes.py` & `django_trench_reboot-0.3.3/trench/command/generate_backup_codes.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/remove_backup_code.py` & `django_trench_reboot-0.3.3/trench/command/remove_backup_code.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/replace_mfa_method_backup_codes.py` & `django_trench_reboot-0.3.3/trench/command/replace_mfa_method_backup_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
     def execute(self, user_id: int, name: str) -> Set[str]:
         backup_codes = self._codes_generator()
         rows_affected = self._mfa_model.objects.filter(
             user_id=user_id, name=name
         ).update(
             _backup_codes=MFAMethod._BACKUP_CODES_DELIMITER.join(
-                [self._code_hasher(backup_code) for backup_code in backup_codes]
-                if self._requires_encryption
-                else backup_codes
+                [
+                    self._code_hasher(backup_code)
+                    for backup_code in backup_codes
+                ] if self._requires_encryption else backup_codes
             ),
         )
 
         if rows_affected < 1:
             raise MFAMethodDoesNotExistError()
 
         return backup_codes
```

### Comparing `django_trench_reboot-0.3.2/trench/command/set_primary_mfa_method.py` & `django_trench_reboot-0.3.3/trench/command/set_primary_mfa_method.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/command/validate_backup_code.py` & `django_trench_reboot-0.3.3/trench/command/validate_backup_code.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/exceptions.py` & `django_trench_reboot-0.3.3/trench/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,24 +23,14 @@
     def __init__(self) -> None:
         super().__init__(
             detail=_("Code invalid or expired."),
             code="code_invalid_or_expired",
         )
 
 
-class MFASourceFieldDoesNotExistError(MFAValidationError):
-    def __init__(self, source_field: str, model_name: str) -> None:
-        super().__init__(
-            detail=_(
-                f"Field name `{source_field}` is not valid for model `{model_name}`."
-            ),
-            code="source_field_not_exist",
-        )
-
-
 class OTPCodeMissingError(MFAValidationError):
     def __init__(self) -> None:
         super().__init__(detail=_("OTP code not provided."), code="otp_code_missing")
 
 
 class MFAMethodDoesNotExistError(MFAValidationError):
     def __init__(self) -> None:
```

### Comparing `django_trench_reboot-0.3.2/trench/locale/de/LC_MESSAGES/django.po` & `django_trench_reboot-0.3.3/trench/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/locale/en/LC_MESSAGES/django.po` & `django_trench_reboot-0.3.3/trench/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/locale/pl/LC_MESSAGES/django.mo` & `django_trench_reboot-0.3.3/trench/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/locale/pl/LC_MESSAGES/django.po` & `django_trench_reboot-0.3.3/trench/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/migrations/0001_initial.py` & `django_trench_reboot-0.3.3/trench/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/migrations/0002_auto_20190111_1403.py` & `django_trench_reboot-0.3.3/trench/migrations/0002_auto_20190111_1403.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/migrations/0003_auto_20190213_2330.py` & `django_trench_reboot-0.3.3/trench/migrations/0003_auto_20190213_2330.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/models.py` & `django_trench_reboot-0.3.3/trench/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from django.conf import settings
 from django.db.models import (
     CASCADE,
     BooleanField,
     CharField,
-    CheckConstraint,
     ForeignKey,
     Manager,
     Model,
-    Q,
     QuerySet,
     TextField,
-    UniqueConstraint,
 )
 from django.utils.translation import gettext_lazy as _
 
 from typing import Any, Iterable
 
 from trench.exceptions import MFAMethodDoesNotExistError
 
@@ -73,29 +70,14 @@
     is_primary = BooleanField(_("is primary"), default=False)
     is_active = BooleanField(_("is active"), default=False)
     _backup_codes = TextField(_("backup codes"), blank=True)
 
     class Meta:
         verbose_name = _("MFA Method")
         verbose_name_plural = _("MFA Methods")
-        constraints = (
-            UniqueConstraint(
-                fields=("user", "name"),
-                name="unique_user_method_name",
-            ),
-            UniqueConstraint(
-                condition=Q(is_primary=True),
-                fields=("user",),
-                name="unique_user_is_primary",
-            ),
-            CheckConstraint(
-                check=(Q(is_primary=True) & Q(is_active=True)) | Q(is_primary=False),
-                name="primary_is_active",
-            ),
-        )
 
     objects = MFAUserMethodManager()
 
     def __str__(self) -> str:
         return f"{self.name} (User id: {self.user_id})"
 
     @property
```

### Comparing `django_trench_reboot-0.3.2/trench/query/get_mfa_config_by_name.py` & `django_trench_reboot-0.3.3/trench/query/get_mfa_config_by_name.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/responses.py` & `django_trench_reboot-0.3.3/trench/responses.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/serializers.py` & `django_trench_reboot-0.3.3/trench/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import User
 from django.db.models import Model
 
 from abc import abstractmethod
 from rest_framework.authtoken.models import Token
 from rest_framework.fields import CharField, ChoiceField
 from rest_framework.serializers import ModelSerializer, Serializer
-from typing import Any, OrderedDict
+from typing import Any, Iterable, OrderedDict, Type
 
 from trench.backends.provider import get_mfa_handler
 from trench.command.remove_backup_code import remove_backup_code_command
 from trench.command.validate_backup_code import validate_backup_code_command
 from trench.exceptions import (
     CodeInvalidOrExpiredError,
     MFAMethodAlreadyActiveError,
@@ -19,15 +18,24 @@
     OTPCodeMissingError,
 )
 from trench.models import MFAMethod
 from trench.settings import trench_settings
 from trench.utils import available_method_choices, get_mfa_model
 
 
-User: AbstractUser = get_user_model()
+def generate_model_serializer(name: str, model: Model, fields: Iterable[str]) -> Type:
+    meta_subclass = type(
+        "Meta",
+        (object,),
+        {
+            "model": model,
+            "fields": fields,
+        },
+    )
+    return type(name, (ModelSerializer,), {"Meta": meta_subclass})
 
 
 class RequestBodyValidator(Serializer):
     def update(self, instance: Model, validated_data: OrderedDict[str, Any]):
         raise NotImplementedError
 
     def create(self, validated_data: OrderedDict[str, Any]):
@@ -134,23 +142,21 @@
 
 class UserMFAMethodSerializer(ModelSerializer):
     class Meta:
         model = get_mfa_model()
         fields = ("name", "is_primary")
 
 
-class ChangePrimaryMethodCodeValidator(ProtectedActionValidator):
+class ChangePrimaryMethodValidator(ProtectedActionValidator):
+    method = ChoiceField(choices=available_method_choices())
+
     @staticmethod
     def _validate_mfa_method(mfa: MFAMethod) -> None:
         pass
 
 
-class ChangePrimaryMethodValidator(RequestBodyValidator):
-    method = ChoiceField(choices=available_method_choices())
-
-
 class TokenSerializer(ModelSerializer):
     auth_token = CharField(source="key")
 
     class Meta:
         model = Token
         fields = ("auth_token",)
```

### Comparing `django_trench_reboot-0.3.2/trench/settings.py` & `django_trench_reboot-0.3.3/trench/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,17 +48,14 @@
 EMAIL_SUBJECT = "EMAIL_SUBJECT"
 EMAIL_PLAIN_TEMPLATE = "EMAIL_PLAIN_TEMPLATE"
 EMAIL_HTML_TEMPLATE = "EMAIL_HTML_TEMPLATE"
 SMSAPI_ACCESS_TOKEN = "SMSAPI_ACCESS_TOKEN"
 SMSAPI_FROM_NUMBER = "SMSAPI_FROM_NUMBER"
 TWILIO_VERIFIED_FROM_NUMBER = "TWILIO_VERIFIED_FROM_NUMBER"
 YUBICLOUD_CLIENT_ID = "YUBICLOUD_CLIENT_ID"
-AWS_ACCESS_KEY = "AWS_ACCESS_KEY"
-AWS_SECRET_KEY = "AWS_SECRET_KEY"
-AWS_REGION = "AWS_REGION"
 
 DEFAULTS = {
     "USER_MFA_MODEL": "trench.MFAMethod",
     "USER_ACTIVE_FIELD": "is_active",
     "BACKUP_CODES_QUANTITY": 5,
     "BACKUP_CODES_LENGTH": 12,  # keep (quantity * length) under 200
     "BACKUP_CODES_CHARACTERS": (string.ascii_letters + string.digits),
@@ -81,23 +78,14 @@
             VERBOSE_NAME: _("sms_api"),
             VALIDITY_PERIOD: 30,
             HANDLER: "trench.backends.sms_api.SMSAPIMessageDispatcher",
             SOURCE_FIELD: "phone_number",
             SMSAPI_ACCESS_TOKEN: "YOUR SMSAPI TOKEN",
             SMSAPI_FROM_NUMBER: "YOUR REGISTERED NUMBER",
         },
-        "sms_aws": {
-            VERBOSE_NAME: _("sms_aws"),
-            VALIDITY_PERIOD: 30,
-            HANDLER: "trench.backends.aws.AWSMessageDispatcher",
-            SOURCE_FIELD: "phone_number",
-            AWS_ACCESS_KEY: "YOUR AWS ACCESS KEY",
-            AWS_SECRET_KEY: "YOUR AWS SECRET KEY",
-            AWS_REGION: "YOUR AWS REGION",
-        },
         "email": {
             VERBOSE_NAME: _("email"),
             VALIDITY_PERIOD: 30,
             HANDLER: "trench.backends.basic_mail.SendMailMessageDispatcher",
             SOURCE_FIELD: "email",
             EMAIL_SUBJECT: _("Your verification code"),
             EMAIL_PLAIN_TEMPLATE: "trench/backends/email/code.txt",
```

### Comparing `django_trench_reboot-0.3.2/trench/urls/base.py` & `django_trench_reboot-0.3.3/trench/urls/base.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/utils.py` & `django_trench_reboot-0.3.3/trench/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import User
 from django.contrib.auth.tokens import PasswordResetTokenGenerator
 from django.utils.crypto import constant_time_compare, salted_hmac
 from django.utils.http import base36_to_int, int_to_base36
 from django.utils.translation import gettext_lazy as _
 
 from datetime import datetime
 from typing import List, Optional, Tuple, Type
 
 from trench.models import MFAMethod
 from trench.settings import VERBOSE_NAME, trench_settings
 
 
-User: AbstractUser = get_user_model()
-
-
 class UserTokenGenerator(PasswordResetTokenGenerator):
     """
     Custom token generator:
         - user pk in token
         - expires after 15 minutes
         - longer hash (40 instead of 20)
     """
```

### Comparing `django_trench_reboot-0.3.2/trench/views/authtoken.py` & `django_trench_reboot-0.3.3/trench/views/authtoken.py`

 * *Files identical despite different names*

### Comparing `django_trench_reboot-0.3.2/trench/views/base.py` & `django_trench_reboot-0.3.3/trench/views/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import User
 from django.db.models import QuerySet
 from django.utils.translation import gettext_lazy as _
 
 from abc import ABC, abstractmethod
 from rest_framework.generics import ListAPIView
 from rest_framework.permissions import AllowAny, IsAuthenticated
 from rest_framework.request import Request
@@ -21,39 +20,32 @@
 from trench.command.authenticate_user import authenticate_user_command
 from trench.command.create_mfa_method import create_mfa_method_command
 from trench.command.deactivate_mfa_method import deactivate_mfa_method_command
 from trench.command.replace_mfa_method_backup_codes import (
     regenerate_backup_codes_for_mfa_method_command,
 )
 from trench.command.set_primary_mfa_method import set_primary_mfa_method_command
-from trench.exceptions import (
-    MFAMethodDoesNotExistError,
-    MFASourceFieldDoesNotExistError,
-    MFAValidationError,
-)
+from trench.exceptions import MFAMethodDoesNotExistError, MFAValidationError
 from trench.query.get_mfa_config_by_name import get_mfa_config_by_name_query
 from trench.responses import ErrorResponse
 from trench.serializers import (
-    ChangePrimaryMethodCodeValidator,
     ChangePrimaryMethodValidator,
     CodeLoginSerializer,
     LoginSerializer,
     MFAMethodActivationConfirmationValidator,
     MFAMethodBackupCodesGenerationValidator,
     MFAMethodCodeSerializer,
     MFAMethodDeactivationValidator,
     UserMFAMethodSerializer,
+    generate_model_serializer,
 )
 from trench.settings import SOURCE_FIELD, trench_settings
 from trench.utils import available_method_choices, get_mfa_model, user_token_generator
 
 
-User: AbstractUser = get_user_model()
-
-
 class MFAStepMixin(APIView, ABC):
     permission_classes = (AllowAny,)
 
     @abstractmethod
     def _successful_authentication_response(self, user: User) -> Response:
         raise NotImplementedError
 
@@ -103,24 +95,25 @@
 
     @staticmethod
     def post(request: Request, method: str) -> Response:
         try:
             source_field = get_mfa_config_by_name_query(name=method).get(SOURCE_FIELD)
         except MFAMethodDoesNotExistError as cause:
             return ErrorResponse(error=cause)
-        user = request.user
+        if source_field is not None:
+            serializer_class = generate_model_serializer(
+                name="MFAMethodActivationValidator",
+                model=request.user.__class__,
+                fields=(source_field,),
+            )
+            serializer = serializer_class(data=request.data)
+            serializer.is_valid(raise_exception=True)
         try:
-            if source_field is not None and not hasattr(user, source_field):
-                raise MFASourceFieldDoesNotExistError(
-                    source_field,
-                    user.__class__.__name__
-                )
-
             mfa = create_mfa_method_command(
-                user_id=user.id,
+                user_id=request.user.id,
                 name=method,
             )
         except MFAValidationError as cause:
             return ErrorResponse(error=cause)
         return get_mfa_handler(mfa_method=mfa).dispatch_message()
 
 
@@ -234,23 +227,22 @@
 
 
 class MFAPrimaryMethodChangeView(APIView):
     permission_classes = (IsAuthenticated,)
 
     @staticmethod
     def post(request: Request) -> Response:
-        method_serializer = ChangePrimaryMethodValidator(data=request.data)
-        method_serializer.is_valid(raise_exception=True)
-
-        code_serializer = ChangePrimaryMethodCodeValidator(
-            user=request.user,
-            mfa_method_name=method_serializer.validated_data["method"],
-            data=request.data,
+        mfa_model = get_mfa_model()
+        mfa_method_name = mfa_model.objects.get_primary_active_name(
+            user_id=request.user.id
         )
-        code_serializer.is_valid(raise_exception=True)
+        serializer = ChangePrimaryMethodValidator(
+            user=request.user, mfa_method_name=mfa_method_name, data=request.data
+        )
+        serializer.is_valid(raise_exception=True)
         try:
             set_primary_mfa_method_command(
-                user_id=request.user.id, name=method_serializer.validated_data["method"]
+                user_id=request.user.id, name=serializer.validated_data["method"]
             )
             return Response(status=HTTP_204_NO_CONTENT)
         except MFAValidationError as cause:
             return ErrorResponse(error=cause)
```

