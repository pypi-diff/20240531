# Comparing `tmp/slthcore-0.0.4.tar.gz` & `tmp/slthcore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slthcore-0.0.4.tar", last modified: Sun May 26 11:59:36 2024, max compression
+gzip compressed data, was "slthcore-0.0.5.tar", last modified: Fri May 31 15:22:50 2024, max compression
```

## Comparing `slthcore-0.0.4.tar` & `slthcore-0.0.5.tar`

### file list

```diff
@@ -1,93 +1,99 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.365379 slthcore-0.0.4/
--rw-r--r--   0 breno      (501) staff       (20)      127 2024-05-25 14:10:00.000000 slthcore-0.0.4/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      572 2024-05-26 11:59:36.365157 slthcore-0.0.4/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-26 11:59:36.365438 slthcore-0.0.4/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      819 2024-05-26 11:59:12.000000 slthcore-0.0.4/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.346592 slthcore-0.0.4/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 slthcore-0.0.4/slth/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.337820 slthcore-0.0.4/slth/cmd/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.346896 slthcore-0.0.4/slth/cmd/init/
--rw-r--r--   0 breno      (501) staff       (20)      910 2024-04-27 22:48:44.000000 slthcore-0.0.4/slth/cmd/init/__main__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.349748 slthcore-0.0.4/slth/cmd/init/boilerplate/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-27 15:58:06.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)      103 2024-04-09 12:50:34.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/.gitignore
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.351498 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.354069 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-03-07 12:24:57.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)      383 2024-05-25 23:50:12.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/asgi.py
--rw-r--r--   0 breno      (501) staff       (20)       27 2024-05-25 20:45:27.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)       39 2024-04-09 15:58:59.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/models.py
--rw-r--r--   0 breno      (501) staff       (20)     4970 2024-05-25 20:20:18.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/settings.py
--rw-r--r--   0 breno      (501) staff       (20)      244 2024-04-13 21:08:07.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      443 2024-05-18 08:02:28.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/urls.py
--rw-r--r--   0 breno      (501) staff       (20)      383 2024-05-25 23:50:11.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/wsgi.py
--rw-r--r--   0 breno      (501) staff       (20)     1213 2024-05-25 19:49:40.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/application.yml
--rwxr-xr-x   0 breno      (501) staff       (20)      112 2024-05-25 23:48:32.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/entrypoint.sh
--rwxr-xr-x   0 breno      (501) staff       (20)      659 2024-05-25 19:49:17.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/manage.py
--rw-r--r--   0 breno      (501) staff       (20)       16 2024-05-25 19:50:51.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/backend/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)      323 2024-04-28 13:48:53.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/base.env
--rw-r--r--   0 breno      (501) staff       (20)     1334 2024-05-25 23:51:38.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/docker-compose.yml
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.354759 slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/
--rw-rw-r--   0 breno      (501) staff       (20)      435 2024-04-27 16:00:09.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/package.json
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.355036 slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/src/
--rw-r--r--   0 breno      (501) staff       (20)      397 2024-04-27 19:45:33.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/src/main.jsx
--rw-rw-r--   0 breno      (501) staff       (20)      659 2024-05-25 19:51:33.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/vite.config.js
--rw-r--r--   0 breno      (501) staff       (20)      107 2024-04-24 17:59:56.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/local.env
--rwxr-xr-x   0 breno      (501) staff       (20)       75 2024-04-27 23:12:22.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/run.sh
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.355381 slthcore-0.0.4/slth/cmd/init/boilerplate/selenium/
--rwxr-xr-x   0 breno      (501) staff       (20)       50 2024-04-14 10:48:25.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/selenium/run.sh
--rwxr-xr-x   0 breno      (501) staff       (20)      211 2024-04-27 19:54:03.000000 slthcore-0.0.4/slth/cmd/init/boilerplate/test.sh
--rw-r--r--   0 breno      (501) staff       (20)     9973 2024-05-23 09:22:14.000000 slthcore-0.0.4/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.356106 slthcore-0.0.4/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 slthcore-0.0.4/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 slthcore-0.0.4/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    25289 2024-05-23 12:47:50.000000 slthcore-0.0.4/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 slthcore-0.0.4/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 slthcore-0.0.4/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26979 2024-05-23 09:31:15.000000 slthcore-0.0.4/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.356406 slthcore-0.0.4/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.4/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.357074 slthcore-0.0.4/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.4/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 slthcore-0.0.4/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 slthcore-0.0.4/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.360070 slthcore-0.0.4/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 slthcore-0.0.4/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 slthcore-0.0.4/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 slthcore-0.0.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 slthcore-0.0.4/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 slthcore-0.0.4/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 slthcore-0.0.4/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.4/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6762 2024-05-23 12:24:55.000000 slthcore-0.0.4/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      561 2024-05-23 12:20:56.000000 slthcore-0.0.4/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 slthcore-0.0.4/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 slthcore-0.0.4/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-26 01:07:41.000000 slthcore-0.0.4/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 slthcore-0.0.4/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.360572 slthcore-0.0.4/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 slthcore-0.0.4/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 slthcore-0.0.4/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15969 2024-05-21 20:16:17.000000 slthcore-0.0.4/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.360910 slthcore-0.0.4/slth/static/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-25 13:08:29.000000 slthcore-0.0.4/slth/static/.DS_Store
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.361544 slthcore-0.0.4/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 slthcore-0.0.4/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 slthcore-0.0.4/slth/static/css/slth.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.363086 slthcore-0.0.4/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-26 11:56:30.000000 slthcore-0.0.4/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-26 11:56:30.000000 slthcore-0.0.4/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102724 2024-05-26 11:56:30.000000 slthcore-0.0.4/slth/static/js/slth.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 slthcore-0.0.4/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.364081 slthcore-0.0.4/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3094 2024-05-25 14:20:50.000000 slthcore-0.0.4/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 slthcore-0.0.4/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5572 2024-05-26 01:06:28.000000 slthcore-0.0.4/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 slthcore-0.0.4/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 slthcore-0.0.4/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 slthcore-0.0.4/slth/views.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-26 11:59:36.364899 slthcore-0.0.4/slthcore.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      572 2024-05-26 11:59:36.000000 slthcore-0.0.4/slthcore.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     2242 2024-05-26 11:59:36.000000 slthcore-0.0.4/slthcore.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-26 11:59:36.000000 slthcore-0.0.4/slthcore.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-26 11:59:36.000000 slthcore-0.0.4/slthcore.egg-info/top_level.txt
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.921746 slthcore-0.0.5/
+-rw-r--r--   0 breno      (501) staff       (20)      127 2024-05-25 14:10:00.000000 slthcore-0.0.5/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      572 2024-05-31 15:22:50.921513 slthcore-0.0.5/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-31 15:22:50.921810 slthcore-0.0.5/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      819 2024-05-31 11:16:05.000000 slthcore-0.0.5/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.895325 slthcore-0.0.5/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     6992 2024-05-30 14:16:05.000000 slthcore-0.0.5/slth/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.885126 slthcore-0.0.5/slth/cmd/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.895644 slthcore-0.0.5/slth/cmd/configure/
+-rw-r--r--   0 breno      (501) staff       (20)     2550 2024-05-26 15:00:15.000000 slthcore-0.0.5/slth/cmd/configure/__main__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.895967 slthcore-0.0.5/slth/cmd/init/
+-rw-r--r--   0 breno      (501) staff       (20)      910 2024-04-27 22:48:44.000000 slthcore-0.0.5/slth/cmd/init/__main__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.898727 slthcore-0.0.5/slth/cmd/init/boilerplate/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-27 15:58:06.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)      103 2024-04-09 12:50:34.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/.gitignore
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.900539 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.902928 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-03-07 12:24:57.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)      383 2024-05-25 23:50:12.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/asgi.py
+-rw-r--r--   0 breno      (501) staff       (20)       27 2024-05-25 20:45:27.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)       39 2024-04-09 15:58:59.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/models.py
+-rw-r--r--   0 breno      (501) staff       (20)     4970 2024-05-25 20:20:18.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/settings.py
+-rw-r--r--   0 breno      (501) staff       (20)      244 2024-04-13 21:08:07.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      443 2024-05-18 08:02:28.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)      383 2024-05-25 23:50:11.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/wsgi.py
+-rw-r--r--   0 breno      (501) staff       (20)     1213 2024-05-25 19:49:40.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/application.yml
+-rwxr-xr-x   0 breno      (501) staff       (20)      112 2024-05-25 23:48:32.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/entrypoint.sh
+-rwxr-xr-x   0 breno      (501) staff       (20)      659 2024-05-25 19:49:17.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/manage.py
+-rw-r--r--   0 breno      (501) staff       (20)       16 2024-05-25 19:50:51.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/backend/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)      323 2024-04-28 13:48:53.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/base.env
+-rw-r--r--   0 breno      (501) staff       (20)     1334 2024-05-25 23:51:38.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/docker-compose.yml
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.904061 slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/
+-rw-rw-r--   0 breno      (501) staff       (20)      435 2024-04-27 16:00:09.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/package.json
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.904386 slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/src/
+-rw-r--r--   0 breno      (501) staff       (20)      397 2024-04-27 19:45:33.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/src/main.jsx
+-rw-rw-r--   0 breno      (501) staff       (20)      659 2024-05-25 19:51:33.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/vite.config.js
+-rw-r--r--   0 breno      (501) staff       (20)      107 2024-04-24 17:59:56.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/local.env
+-rwxr-xr-x   0 breno      (501) staff       (20)       75 2024-04-27 23:12:22.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/run.sh
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.904837 slthcore-0.0.5/slth/cmd/init/boilerplate/selenium/
+-rwxr-xr-x   0 breno      (501) staff       (20)       50 2024-04-14 10:48:25.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/selenium/run.sh
+-rwxr-xr-x   0 breno      (501) staff       (20)      211 2024-04-27 19:54:03.000000 slthcore-0.0.5/slth/cmd/init/boilerplate/test.sh
+-rw-r--r--   0 breno      (501) staff       (20)     9973 2024-05-26 23:03:30.000000 slthcore-0.0.5/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.905979 slthcore-0.0.5/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 slthcore-0.0.5/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     3297 2024-05-28 19:33:36.000000 slthcore-0.0.5/slth/db/generic.py
+-rw-r--r--   0 breno      (501) staff       (20)     5213 2024-05-30 22:36:23.000000 slthcore-0.0.5/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    28123 2024-05-30 21:14:36.000000 slthcore-0.0.5/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 slthcore-0.0.5/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4443 2024-05-28 21:16:27.000000 slthcore-0.0.5/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    27072 2024-05-30 12:31:23.000000 slthcore-0.0.5/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.906290 slthcore-0.0.5/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.5/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.906984 slthcore-0.0.5/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.5/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 slthcore-0.0.5/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 slthcore-0.0.5/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.916367 slthcore-0.0.5/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 slthcore-0.0.5/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 slthcore-0.0.5/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 slthcore-0.0.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 slthcore-0.0.5/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 slthcore-0.0.5/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 slthcore-0.0.5/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)     2269 2024-05-30 14:07:26.000000 slthcore-0.0.5/slth/migrations/0007_deletion_log.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 slthcore-0.0.5/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11292 2024-05-30 22:37:17.000000 slthcore-0.0.5/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      561 2024-05-23 12:20:56.000000 slthcore-0.0.5/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 slthcore-0.0.5/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 slthcore-0.0.5/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    20517 2024-05-30 22:49:16.000000 slthcore-0.0.5/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 slthcore-0.0.5/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.916847 slthcore-0.0.5/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 slthcore-0.0.5/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 slthcore-0.0.5/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    16170 2024-05-30 12:52:14.000000 slthcore-0.0.5/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.917165 slthcore-0.0.5/slth/static/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-25 13:08:29.000000 slthcore-0.0.5/slth/static/.DS_Store
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.917785 slthcore-0.0.5/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 slthcore-0.0.5/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 slthcore-0.0.5/slth/static/css/slth.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.919196 slthcore-0.0.5/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-31 15:21:40.000000 slthcore-0.0.5/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-31 15:21:40.000000 slthcore-0.0.5/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   103598 2024-05-31 15:21:40.000000 slthcore-0.0.5/slth/static/js/slth.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 slthcore-0.0.5/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     1774 2024-05-28 20:37:31.000000 slthcore-0.0.5/slth/tasks.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.920396 slthcore-0.0.5/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3094 2024-05-25 14:20:50.000000 slthcore-0.0.5/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 slthcore-0.0.5/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5572 2024-05-26 01:06:28.000000 slthcore-0.0.5/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)       41 2024-05-29 01:55:22.000000 slthcore-0.0.5/slth/threadlocal.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 slthcore-0.0.5/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1172 2024-05-26 13:58:05.000000 slthcore-0.0.5/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2920 2024-05-30 19:58:36.000000 slthcore-0.0.5/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-31 15:22:50.921247 slthcore-0.0.5/slthcore.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      572 2024-05-31 15:22:50.000000 slthcore-0.0.5/slthcore.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     2363 2024-05-31 15:22:50.000000 slthcore-0.0.5/slthcore.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-31 15:22:50.000000 slthcore-0.0.5/slthcore.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-31 15:22:50.000000 slthcore-0.0.5/slthcore.egg-info/top_level.txt
```

### Comparing `slthcore-0.0.4/PKG-INFO` & `slthcore-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slthcore
-Version: 0.0.4
+Version: 0.0.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `slthcore-0.0.4/setup.py` & `slthcore-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = []
 
 setup(
     name='slthcore',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=install_requires,
     include_package_data=True,
     license='BSD License',
     description='API generator based on yml file',
     long_description='',
     url='https://github.com/brenokcc',
```

### Comparing `slthcore-0.0.4/slth/cmd/init/__main__.py` & `slthcore-0.0.5/slth/cmd/init/__main__.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/.DS_Store` & `slthcore-0.0.5/slth/cmd/init/boilerplate/.DS_Store`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/backend/api/settings.py` & `slthcore-0.0.5/slth/cmd/init/boilerplate/backend/api/settings.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/backend/application.yml` & `slthcore-0.0.5/slth/cmd/init/boilerplate/backend/application.yml`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/backend/manage.py` & `slthcore-0.0.5/slth/cmd/init/boilerplate/backend/manage.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/docker-compose.yml` & `slthcore-0.0.5/slth/cmd/init/boilerplate/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/cmd/init/boilerplate/frontend/vite.config.js` & `slthcore-0.0.5/slth/cmd/init/boilerplate/frontend/vite.config.js`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/components.py` & `slthcore-0.0.5/slth/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
 class Scheduler(dict):
     INTERVALS = {1: ["00"], 2: ["00", "30"]}
 
     def __init__(
         self,
         start_time=7,
-        end_time=20,
+        end_time=23,
         chucks=2,
         start_day=None,
         days=14,
         single_selection=False,
         input_name="schedule",
         readonly=False,
     ):
```

### Comparing `slthcore-0.0.4/slth/db/models.py` & `slthcore-0.0.5/slth/db/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from uuid import uuid1
 from django.db.models import Model as DjangoModel
 from django.db.models import *
 from django.utils.translation import gettext_lazy as _
+from . import generic
 from .. import ModelMixin
 
+GenericField = generic.GenericField
+
 class CharField(CharField):
     def __init__(self, *args, **kwargs):
         self.mask = kwargs.pop('mask', None)
         kwargs.setdefault('max_length', 255)
         super().__init__(*args, **kwargs)
 
     def formfield(self, *args, **kwargs):
@@ -134,7 +137,15 @@
         filename = '{}.{}'.format(uuid1().hex, filename.split('.')[-1].lower())
         print(filename)
         return super().generate_filename(instance, filename)
 
 class Model(DjangoModel, ModelMixin):
     class Meta:
         abstract = True
+
+class Filter:
+
+    def get_label(self):
+        return None
+    
+    def choices(self, queryset):
+        return queryset
```

### Comparing `slthcore-0.0.4/slth/endpoints.py` & `slthcore-0.0.5/slth/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import json
 import types
 import inspect
-from .models import Token
+
+from .models import Token, Role, Log, Deletion
 from django.apps import apps
 from typing import TypeVar, Generic
 from django.core.cache import cache
 from django.conf import settings
 from django.utils.text import slugify
 from django.db import models
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .factory import FormFactory
 from django.core.exceptions import ValidationError
 from slth import forms
+from django.db.models import Model
+from datetime import datetime
 from django.contrib.auth import authenticate
 from .forms import ModelForm, Form
 from .serializer import serialize, Serializer
 from .components import (
     Application as Application_,
     Navbar,
     Menu,
     Footer,
     Response,
     Boxes,
     IconSet,
 )
 from .exceptions import JsonResponseException
 from .utils import build_url, append_url
-from .models import PushSubscription, Profile, User
+from .models import PushSubscription, Profile, User, Log
 from slth.queryset import QuerySet
 from slth import APPLICATON, ENDPOINTS
 from . import oauth
+from .tasks import Task, TaskRunner
+from .threadlocal import tl
 
 
 T = TypeVar("T")
 
 
 class ApiResponse(JsonResponse):
     def __init__(self, *args, **kwargs):
@@ -110,21 +115,28 @@
         self.request = request
         return self
 
     def objects(self, model):
         return apps.get_model(model).objects
 
     def get(self):
-        return {}
+        fields = []
+        for name in dir(self):
+            if isinstance(getattr(self, name), forms.Field):
+                fields.append(name)
+        return self.formfactory().fields(*fields) if fields else {}
 
     def post(self):
         return Response(message="Ação realizada com sucesso")
 
     def check_permission(self):
         return self.request.user.is_superuser
+    
+    def contribute(self, entrypoint):
+        return True
 
     def check_role(self, *names, superuser=True):
         if self.request.user.is_superuser and superuser:
             return True
         for name in names:
             if (
                 self.objects("slth.role")
@@ -165,15 +177,19 @@
         elif isinstance(data, Form) or isinstance(data, ModelForm):
             data = data.settitle(title)
         elif self.request.method == "POST" and not data:
             return self.post()
         return data
 
     def serialize(self):
-        return serialize(self.process())
+        output = self.process()
+        if isinstance(output, Task):
+            TaskRunner(output).start()
+            output = Response(f'Tarefa {output.key} iniciada.', task=output.key)
+        return serialize(output)
 
     def to_response(self):
         return ApiResponse(self.serialize(), safe=False)
 
     def formfactory(self, instance=None, method="POST") -> FormFactory:
         return FormFactory(instance, method=method)
 
@@ -221,15 +237,15 @@
         return len(inspect.getfullargspec(cls.__init__).args) > 1
 
     @classmethod
     def get_api_url_pattern(cls):
         args = inspect.getfullargspec(cls.__init__).args[1:]
         pattern = "{}/".format(cls.get_api_name())
         for arg in args:
-            pattern = "{}{}/".format(pattern, "<int:{}>".format(arg))
+            pattern = "{}{}/".format(pattern, "<str:{}>".format(arg))
         return pattern
 
     @classmethod
     def get_api_metadata(cls, request, base_url, pk=None):
         action_name = cls.get_metadata("verbose_name")
         icon = cls.get_metadata("icon")
         modal = cls.get_metadata("modal")
@@ -265,15 +281,37 @@
                     or issubclass(cls, Endpoint)
                     or issubclass(cls, ChildEndpoint)
                 )
         return default if value is None else value
 
     def get_verbose_name(self):
         return self.get_metadata("verbose_name")
+    
+    def get_instance(self):
+        return None
+    
+    def start_audit_trail(self):
+        instance = self.get_instance()
+        pk = instance.pk if isinstance(instance, Model) else None
+        tl.context = dict(
+            endpoint = self.get_api_name(), model=None, pk=pk,
+            datetime=datetime.now().strftime('%d/%m/%Y %H:%M:%S'),
+            user=self.request.user.username if self.request.user.is_authenticated else None,
+            url=self.request.get_full_path(), logs=[]
+        )
 
+    def finish_audit_trail(self):
+        if hasattr(tl, 'context') and tl.context['logs']:
+            pk = tl.context['pk']
+            instance = self.get_instance()
+            print(tl.context)
+            if pk or isinstance(instance, Model):
+                model = '{}.{}'.format(instance._meta.app_label, instance._meta.model_name)
+                tl.context.update(model=model, pk=pk or instance.pk)
+            Log.objects.create(data=tl.context)
 
 class PublicEndpoint(Endpoint):
     def check_permission(self):
         return True
 
 
 class ModelEndpoint(Endpoint):
@@ -304,27 +342,30 @@
     
     def check_delete_permission(self):
         return self.check_permission()
 
 
 class ListEndpoint(Generic[T], ModelEndpoint):
     def get(self) -> QuerySet:
-        return self.model.objects.contextualize(self.request)
+        return self.model.objects#.contextualize(self.request)
 
 
 class AddEndpoint(Generic[T], ModelEndpoint):
     def __init__(self):
         super().__init__()
         self.instance = self.model()
 
     def get(self) -> FormFactory:
-        return self.model().formfactory()
+        return self.formfactory()
 
     def get_instance(self):
         return self.instance
+    
+    def formfactory(self):
+        return self.instance.formfactory()
 
 
 class ModelInstanceEndpoint(ModelEndpoint):
     def __init__(self, pk):
         super().__init__()
         self.instance = self.model.objects.get(pk=pk)
 
@@ -361,15 +402,15 @@
 
 
 class DeleteEndpoint(Generic[T], ModelInstanceEndpoint):
     def get(self) -> FormFactory:
         return self.formfactory(self.get_instance()).fields()
 
     def post(self):
-        self.get_instance().delete()
+        self.get_instance().safe_delete(self.request.user.username)
         return super().post()
 
 
 class ChildEndpoint(Endpoint):
 
     @classmethod
     def is_child(cls):
@@ -463,15 +504,15 @@
             username=self.cleaned_data.get("username"),
             password=self.cleaned_data.get("password"),
         )
         if user:
             token = Token.objects.create(user=user)
             return Response(
                 message="Bem-vindo!",
-                redirect="/api/dashboard/",
+                redirect=self.request.GET.get("next", "/api/dashboard/"),
                 store=dict(token=token.key, application=None),
             )
         else:
             raise ValidationError("Login e senha não conferem")
 
 
 class Logout(Endpoint):
@@ -489,21 +530,66 @@
     def check_permission(self):
         return self.request.user.is_authenticated
 
 
 class Icons(PublicEndpoint):
     class Meta:
         modal = True
-        verbose_name = "Icons"
+        verbose_name = "Ícones"
 
     def get(self):
         return IconSet()
 
     def check_permission(self):
         return settings.DEBUG
+    
+    def contribute(self, entrypoint):
+        return self.request.user.is_authenticated
+    
+
+class Roles(ListEndpoint[Role]):
+    class Meta:
+        modal = False
+        verbose_name = 'Papéis dos Usuários'
+    
+    def get(self):
+        return super().get().all()
+
+class Logs(ListEndpoint[Log]):
+    class Meta:
+        modal = False
+        verbose_name = 'Histórico de Alterações'
+    
+    def get(self):
+        return super().get().all()
+    
+
+class Deletions(ListEndpoint[Deletion]):
+    class Meta:
+        modal = False
+        verbose_name = 'Exclusões'
+    
+    def get(self):
+        return super().get().all()
+
+
+class RestoreDeletion(InstanceEndpoint[Deletion]):
+    class Meta:
+        verbose_name = 'Restaurar'
+
+    def get(self):
+        return (super().formfactory().fields())
+    
+    def post(self):
+        self.instance.restore()
+        return super().post()
+    
+    def check_permission(self):
+        return super().check_permission() and not self.instance.restored
+
 
 
 class Search(Endpoint):
     def get(self):
         key = "_options_"
         options = self.cache.get(key, [])
         term = self.request.GET.get("term")
@@ -586,46 +672,43 @@
 
 
 class Dashboard(Endpoint):
     class Meta:
         verbose_name = ""
 
     def get(self):
-        if self.request.user.is_authenticated:
-            serializer = Serializer(request=self.request)
-            if APPLICATON["dashboard"]["boxes"]:
-                boxes = Boxes("Acesso Rápido")
-                for endpoint in APPLICATON["dashboard"]["boxes"]:
-                    cls = ENDPOINTS[endpoint]
-                    if cls().contextualize(self.request).check_permission():
-                        icon = cls.get_metadata("icon", "check")
-                        label = cls.get_metadata("verbose_name")
-                        url = build_url(self.request, cls.get_api_url())
-                        boxes.append(icon, label, url)
-                serializer.append("Acesso Rápido", boxes)
-            if APPLICATON["dashboard"]["top"]:
-                group = serializer.group("Top")
-                for endpoint in APPLICATON["dashboard"]["top"]:
-                    cls = ENDPOINTS[endpoint]
-                    if cls.instantiate(
-                        self.request, self.request.user
-                    ).check_permission():
-                        group.endpoint(
-                            cls.get_metadata("verbose_name"), cls, wrap=False
-                        )
-                group.parent()
-            if APPLICATON["dashboard"]["center"]:
-                for endpoint in APPLICATON["dashboard"]["center"]:
-                    cls = ENDPOINTS[endpoint]
-                    serializer.endpoint(
+        serializer = Serializer(request=self.request)
+        if APPLICATON["dashboard"]["boxes"]:
+            boxes = Boxes("Acesso Rápido")
+            for endpoint in APPLICATON["dashboard"]["boxes"]:
+                cls = ENDPOINTS[endpoint]
+                if cls().contextualize(self.request).check_permission():
+                    icon = cls.get_metadata("icon", "check")
+                    label = cls.get_metadata("verbose_name")
+                    url = build_url(self.request, cls.get_api_url())
+                    boxes.append(icon, label, url)
+            serializer.append("Acesso Rápido", boxes)
+        if APPLICATON["dashboard"]["top"]:
+            group = serializer.group("Top")
+            for endpoint in APPLICATON["dashboard"]["top"]:
+                cls = ENDPOINTS[endpoint]
+                if cls.instantiate(
+                    self.request, self.request.user
+                ).check_permission():
+                    group.endpoint(
                         cls.get_metadata("verbose_name"), cls, wrap=False
                     )
-            return serializer
-        else:
-            self.redirect("/api/login/")
+            group.parent()
+        if APPLICATON["dashboard"]["center"]:
+            for endpoint in APPLICATON["dashboard"]["center"]:
+                cls = ENDPOINTS[endpoint]
+                serializer.endpoint(
+                    cls.get_metadata("verbose_name"), cls, wrap=False
+                )
+        return serializer
 
     def check_permission(self):
         return self.request.user.is_authenticated
 
 
 class Application(PublicEndpoint):
     def get(self):
@@ -642,22 +725,24 @@
             logo=logo,
             user=user,
             search=False,
             roles=' | '.join((str(role) for role in self.objects('slth.role').filter(username=self.request.user.username)))
         )
         for entrypoint in ["actions", "usermenu", "adder", "settings", "tools", "toolbar"]:
             if APPLICATON["dashboard"][entrypoint]:
-                for endpoint in APPLICATON["dashboard"][entrypoint]:
-                    cls = ENDPOINTS[endpoint]
-                    if cls().instantiate(self.request, self).check_permission():
+                for endpoint_name in APPLICATON["dashboard"][entrypoint]:
+                    cls = ENDPOINTS[endpoint_name]
+                    endpoint = cls().instantiate(self.request, self)
+                    if endpoint.check_permission() and endpoint.contribute(entrypoint):
                         label = cls.get_metadata("verbose_name")
                         url = build_url(self.request, cls.get_api_url())
                         modal = cls.get_metadata("modal", False)
                         icon = cls.get_metadata("icon", None)
                         navbar.add_action(entrypoint, label, url, modal, icon=icon)
+        
         if APPLICATON["menu"]:
             items = []
 
             def get_item(k, v):
                 if isinstance(v, dict):
                     icon, label = k.split(":") if ":" in k else (None, k)
                     subitems = []
@@ -666,15 +751,16 @@
                         if subitem:
                             subitems.append(subitem)
                     if subitems:
                         return dict(dict(icon=icon, label=label, items=subitems))
                 else:
                     cls = ENDPOINTS.get(v)
                     if cls:
-                        if cls().instantiate(self.request, self).check_permission():
+                        endpoint = cls().instantiate(self.request, self)
+                        if endpoint.check_permission() and endpoint.contribute("menu"):
                             icon, label = k.split(":") if ":" in k else (None, k)
                             url = build_url(self.request, cls.get_api_url())
                             return dict(dict(label=label, url=url, icon=icon))
                     else:
                         print(v)
 
             for k, v in APPLICATON["menu"].items():
@@ -802,7 +888,17 @@
     def check_permission(self):
         return self.request.user.is_authenticated
 
 
 class About(PublicEndpoint):
     def get(self):
         return dict(version=APPLICATON["version"])
+    
+class TaskProgress(PublicEndpoint):
+
+    def __init__(self, key):
+        self.key = key
+        super().__init__()
+
+    def get(self):
+        return cache.get(self.key)
+
```

### Comparing `slthcore-0.0.4/slth/factory.py` & `slthcore-0.0.5/slth/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         
         if isinstance(self._instance, Model):
             fieldlist = [field.name for field in type(self._instance)._meta.get_fields() if field.name in self._fieldlist]
             class Form(ModelForm):
                 class Meta:
                     model = type(self._instance)
                     fields = () if self._empty else (fieldlist if self._fieldlist else '__all__')
-                
+        
         form = Form(instance=self._instance, endpoint=endpoint, initial=self._initial)
         form._key = endpoint.get_api_name()
         form._title = self._title
         form._method = self._method
         form._info = self._info
         form._actions = self._actions
         form._message = self._message
```

### Comparing `slthcore-0.0.4/slth/forms.py` & `slthcore-0.0.5/slth/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
                             else None
                         )
                         if pk < 0:
                             setattr(instance, "deleting", True)
                         inline_form = inline_field.form(
                             data=inline_form_data,
                             instance=instance,
-                            request=self.request,
+                            endpoint=self._endpoint,
                         )
                         if inline_form.is_valid():
                             if isinstance(inline_form, DjangoModelForm):
                                 data[inline_field_name].append(inline_form.instance)
                             else:
                                 data[inline_field_name].append(inline_form.cleaned_data)
                         else:
@@ -465,28 +465,30 @@
                     for field_name in self.fields
                     if field_name not in inline_fields
                 }
             )
             with transaction.atomic():
                 self.cleaned_data = data
                 if isinstance(self, DjangoModelForm):
+                    self.instance.pre_save()
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             obj.save()
                             # set one-to-one
                             if hasattr(self.instance, f"{inline_field_name}_id"):
                                 if hasattr(obj, "deleting"):
                                     setattr(self.instance, inline_field_name, None)
                                 else:
                                     setattr(self.instance, inline_field_name, obj)
                     self.save()
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             if hasattr(obj, "deleting"):
                                 obj.delete()
+                    self.instance.post_save()
                 return self.cleaned_data
 
     def settitle(self, title):
         self._title = title
         return self
 
     def setvalue(self, **kwargs):
@@ -514,15 +516,14 @@
         self._key = self._title.lower()
 
         self.fieldsets = {}
         self.fields = {}
         self.request = endpoint.request
         self.controller = FormController(self)
         self.instance = kwargs.pop("instance", None)
-
         self.parse_json()
         if "data" not in kwargs:
             if self.request.method.upper() == "GET":
                 data = self.request.GET or None
             elif self.request.method.upper() == "POST":
                 data = self.request.POST or {}
         else:
```

### Comparing `slthcore-0.0.4/slth/management/commands/integration_test.py` & `slthcore-0.0.5/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/management/commands/sync.py` & `slthcore-0.0.5/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/migrations/0001_initial.py` & `slthcore-0.0.5/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/migrations/0002_email_role_pushsubscription_error.py` & `slthcore-0.0.5/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `slthcore-0.0.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/migrations/0006_user.py` & `slthcore-0.0.5/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/notifications.py` & `slthcore-0.0.5/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/oauth.py` & `slthcore-0.0.5/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/permissions.py` & `slthcore-0.0.5/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/queryset.py` & `slthcore-0.0.5/slth/queryset.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,17 @@
         return self
 
     def search(self, *names):
         if 'search' not in self.metadata:
             self.metadata['search'] = [name if '__' in name else '{}__icontains'.format(name) for name in names]
         return self
 
-    def filters(self, *names):
+    def filters(self, *names, **kwargs):
         self.metadata['filters'] = names
+        self.metadata['custom_filters'] = kwargs
         return self
 
     def actions(self, *names, **replacement):
         if 'actions' not in self.metadata:
             self.metadata['actions'] = []
         self.metadata['actions'].extend(names)
         for k, v in replacement.items():
@@ -157,39 +158,38 @@
             if cls.get_api_name() in actions:
                 source = self.model.objects.get(pk=pk) if pk else self
                 endpoint = cls.instantiate(self.request, source)
                 if endpoint.check_permission():
                     raise JsonResponseException(endpoint.serialize())
                 raise Exception()
 
+        
         filters = qs.metadata.get('filters', ())
         for lookup in filters:
-            if lookup.endswith('userrole'):
-                from api.models import Role
-                rolename = qs.parameter('userrole')
-                if rolename:
-                    qs = qs.filter(
-                        **{'{}__in'.format(lookup[0:-10]):
-                        Role.objects.filter(name=rolename).values_list('username', flat=True)}
-                    )
-            elif request and lookup in request.GET and lookup != choices_field_name:
+            if request and lookup in request.GET and lookup != choices_field_name:
                 qs = qs.apply_filter(lookup, request.GET[lookup])
+        custom_filters = qs.metadata.get('custom_filters', {})
+        for lookup in custom_filters:
+            if request and lookup in request.GET and lookup != choices_field_name:
+                qs = custom_filters[lookup].filter(qs, request.GET[lookup])
         search = qs.metadata.get('search', ())
         if request and search and 'q' in request.GET:
             qs = qs.apply_search(request.GET['q'], search)
 
         if choices_field_name:
-            field = qs.model.get_field(choices_field_name)
-            choices = field.related_model.objects.filter(pk__in=qs.values_list(choices_field_name, flat=True))
             term = self.request.GET.get('term')
-            if term:
-                choices = choices.apply_search(term)
+            if choices_field_name in custom_filters:
+                choices = custom_filters[choices_field_name].choices(self, term)
+            else:
+                field = qs.model.get_field(choices_field_name)
+                choices = field.related_model.objects.filter(pk__in=qs.values_list(choices_field_name, flat=True))
+                if term:
+                    choices = choices.apply_search(term)
             raise JsonResponseException([dict(id=obj.id, value=str(obj).strip()) for obj in choices[0:20]])
 
-
         return qs
 
     def apply_filter(self, lookup, value):
         booleans = dict(true=True, false=False, null=None)
         if len(value) == 10 and '-' in value:
             value = datetime.strptime(value, '%Y-%m-%d');
         if value in booleans:
@@ -276,21 +276,22 @@
             qs, calendar = qs.to_calendar(qs.metadata['calendar'])
         template = self.metadata.get('template')
 
         for name in qs.metadata.get('search', ()):
             search.append(name)
 
         for lookup in qs.metadata.get('filters', ()):
-            if lookup.endswith('userrole'):
-                field = self.role_filter_field()
-            else:
-                field = self.filter_field(lookup, base_url)
+            field = self.filter_field(lookup, base_url)
             if field:
                 filters.append(field)
-
+        for filtername, filter in qs.metadata.get('custom_filters', {}).items():
+            field = self.custom_filter_field(filtername, filter, base_url)
+            if field:
+                filters.append(field)
+        
         total = qs.count()
         for name in self.metadata.get('subsets', ()):
             attr = getattr(self, name)
             label = getattr(attr, 'verbose_name', name.title())
             subsets.append(dict(name=name, label=label, count=attr().count()))
         if subsets:
             subsets.insert(0, dict(name=None, label='Tudo', count=total))
@@ -385,19 +386,26 @@
                 )
             )
             data.update(count=count, data=objs, pagination=pagination)
         if debug:
             print(json.dumps(data, indent=2, ensure_ascii=False))
         return data
     
-    def role_filter_field(self):
-        value = self.parameter('userrole')
-        choices = [{'id': '', 'text': ''}]
-        choices.extend({'id': k, 'text': v} for k, v in ['adm', 'Administrador'])
-        return dict(name='userrole', type='choice', value=value, label='Papel', required=False, mask=None, choices=choices)
+    def custom_filter_field(self, name, filter, base_url):
+        options = filter.choices(self)
+        value = self.parameter(name)
+        if isinstance(options, list) or isinstance(options, tuple):
+            field_type = 'choice'
+            choices = [{'id': '', 'value':''}]
+            choices.extend([{'id': k, 'value': v} for k, v in options])
+            choices.append({'id': 'null', 'value':'Nulo'})
+        else:
+            field_type = 'choice'
+            choices = append_url(base_url, f'choices={name}')
+        return dict(name=name, type=field_type, value=value, label=filter.get_label(), required=False, mask=None, choices=choices)
 
     def filter_field(self, lookups, base_url):
         name = lookups.strip()
         suffix = None
         choices = None
         field = None
         value = None
```

### Comparing `slthcore-0.0.4/slth/roles.py` & `slthcore-0.0.5/slth/roles.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/selenium/__init__.py` & `slthcore-0.0.5/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/selenium/browser.py` & `slthcore-0.0.5/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/serializer.py` & `slthcore-0.0.5/slth/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return getattr(obj, args[0])
 
 
 def to_snake_case(name):
     return slugify(name).replace('-', '_')
 
 
-def serialize(obj, primitive=False, request=None):
+def serialize(obj, primitive=False, request=None, logging=False):
     if obj is None:
         return None
     elif isinstance(obj, dict):
         if request:
             if isinstance(obj, Image):
                 if isinstance(obj['src'], ImageFieldFile):
                     obj['src'] = build_url(request, obj['src'].url) if obj['src'] else None
@@ -50,17 +50,23 @@
     elif isinstance(obj, bool):
         return obj
     if isinstance(obj, Decimal) or isinstance(obj, float):
         return str(obj).replace('.', ',')
     elif isinstance(obj, list):
         return [serialize(obj) for obj in obj]
     elif isinstance(obj, Model):
-        return str(obj) if primitive else dict(pk=obj.pk, str=str(obj))
+        if logging:
+            return f'{obj.pk}:{str(obj)}'
+        else:
+            return str(obj) if primitive else dict(pk=obj.pk, str=str(obj))
     elif isinstance(obj, QuerySet) or isinstance(obj, Manager) or type(obj).__name__ == 'ManyRelatedManager':
-        return [str(obj) for obj in obj.filter()] if primitive else obj.serialize()
+        if logging:
+            return [f'{obj.pk}:{str(obj)}' for obj in obj.filter()]
+        else:
+            return [str(obj) for obj in obj.filter()] if primitive else obj.serialize()
     elif isinstance(obj, ImageFieldFile) or isinstance(obj, FieldFile):
         return str(obj)
     elif hasattr(obj, 'serialize'):
         return obj.serialize()
     return str(obj)
 
 def getfield(obj, name_or_names, request=None):
```

### Comparing `slthcore-0.0.4/slth/static/.DS_Store` & `slthcore-0.0.5/slth/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/static/css/.DS_Store` & `slthcore-0.0.5/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/static/css/slth.css` & `slthcore-0.0.5/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/static/js/index.min.js` & `slthcore-0.0.5/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/static/js/react.min.js` & `slthcore-0.0.5/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/static/js/slth.min.js` & `slthcore-0.0.5/slth/static/js/slth.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
     c as H,
     r as D,
     R as Te
 } from "./react.min.js";
-const j = {
+const w = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -48,15 +48,15 @@
         textAlign: "center",
         cursor: "pointer"
     };
     return t.jsx("div", {
         style: {
             marginTop: 30
         },
-        children: qe.map(r => t.jsxs("div", {
+        children: Le.map(r => t.jsxs("div", {
             className: "icon-box",
             onClick: () => n(r),
             style: a,
             children: [t.jsx("i", {
                 className: "fa-solid fa-fw fa-" + r
             }), t.jsx("div", {
                 className: "icon-text",
@@ -92,35 +92,35 @@
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = j.colors.primary, a.color = "white"), e.default && (a.color = j.colors.primary, a.border = "solid 1px " + j.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = w.colors.primary, a.color = "white"), e.default && (a.color = w.colors.primary, a.border = "solid 1px " + w.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
             children: t.jsx(C, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
-const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
+const Le = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function Be(e) {
+function qe(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : j.colors.success,
+            backgroundColor: e.isError ? "#e52207" : w.colors.success,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
@@ -133,15 +133,15 @@
         })
     }
     return n()
 }
 
 function z(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(Be, {
+    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -150,16 +150,16 @@
         e.remove()
     })
 }
 
 function J(e) {
     function n() {
         const a = {
-            color: j.colors.info,
-            backgroundColor: j.background.info,
+            color: w.colors.info,
+            backgroundColor: w.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -170,36 +170,36 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Le(e) {
+function Be(e) {
     const n = e.data;
     n.store && Object.keys(n.store).map(function(a) {
         n.store[a] ? localStorage.setItem(a, n.store[a]) : localStorage.removeItem(a, n.store[a])
     }), n.redirect && n.redirect.length > 2 ? (n.message && localStorage.setItem("message", n.message), document.location.href = U(n.redirect)) : n.message && z(n.message)
 }
 
-function A(e) {
+function R(e) {
     return e.replace("/app/", "/api/")
 }
 
 function U(e) {
-    return e.replace("/api/", "/app/")
+    return e.replaceAll("/api/", "/app/")
 }
 
-function B(e, n, a, r) {
+function q(e, n, a, r) {
     const i = localStorage.getItem("token");
     var o = {
         Accept: "application/json"
     };
     i && (o.Authorization = "Token " + i);
-    const d = A(n);
+    const d = R(n);
     var c = {
         method: e,
         headers: new Headers(o),
         ajax: 1
     };
     r && (c.body = r);
     var s = null,
@@ -272,25 +272,25 @@
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function se() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
-function pe(e, n) {
+function we(e, n) {
     de(), se(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
-        url: A(e)
+        url: R(e)
     }))
 }
 
 function Ae(e) {
     de(), se(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
-        url: A(e)
+        url: R(e)
     }))
 }
 
 function Y(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
@@ -324,19 +324,19 @@
         style: n
     })
 }
 
 function _e(e) {
     const [n, a] = D.useState(null), [r, i] = D.useState(0);
     D.useEffect(() => {
-        o(A(e.url)), document.querySelector(".layer").style.display = "block"
+        o(R(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function o(s) {
-        B("GET", A(s), function(u) {
+        q("GET", R(s), function(u) {
             a(u), i(r + 1)
         })
     }
 
     function d() {
         const s = {
                 maxWidth: 800
@@ -399,15 +399,15 @@
             children: [t.jsx("div", {
                 style: i,
                 children: t.jsx(C, {
                     icon: "x",
                     onClick: () => Y()
                 })
             }), t.jsx("iframe", {
-                src: A(e.url),
+                src: R(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
@@ -458,26 +458,36 @@
     return t.jsx("dialog", {
         id: n,
         style: i,
         children: a()
     })
 }
 
-function M(e) {
+function E(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
+const xe = {};
+
+function A(e) {
+    let n = "",
+        a = window.document.styleSheets[0];
+    e.split("}").forEach(r => {
+        let i = (r + "}").replace(/\r?\n|\r/g, "");
+        n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && xe[n] == null && (a.insertRule(n, a.cssRules.length), n = "", xe[n] = !0)
+    })
+}
 
 function F(e) {
     const n = e.id || Math.random(),
         [a, r] = D.useState(e.data.name);
 
     function i(c) {
         c.preventDefault();
         var s = e.data.url;
-        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
+        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : we(s)
     }
 
     function o() {
         return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(C, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(C, {
@@ -486,121 +496,126 @@
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
     function d() {
+        A(`
+      .action{
+        padding: 12px;
+        text-decoration: none;
+        white-space: nowrap;
+        border-radius: 5px;
+        margin: 5px;
+        min-width: 50px;
+      }
+    `);
         var c = {
-            padding: 12,
-            textDecoration: "none",
-            whiteSpace: "nowrap",
-            borderRadius: 5,
-            margin: 5,
-            minWidth: 50,
             lineHeight: e.data.icon ? "4rem" : "auto"
         };
-        return e.primary && (c.backgroundColor = j.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + j.colors.primary, c.color = j.colors.primary), e.style && Object.keys(e.style).map(function(s) {
+        return e.primary && (c.backgroundColor = w.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + w.colors.primary, c.color = w.colors.primary), e.style && Object.keys(e.style).map(function(s) {
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
+            className: "action",
             href: U(e.data.url) || "#",
             onClick: i,
             style: c,
-            "data-label": M(e.data.name),
+            "data-label": E(e.data.name),
             children: o()
         })
     }
     return d()
 }
 
 function ee(e) {
     function n(o) {
-        var d = o.target.parentNode.querySelector(".dropdown");
-        return d == null && (d = o.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = o.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
+        var d = o.target.parentNode.querySelector(".dropdown ul");
+        return d == null && (d = o.target.parentNode.parentNode.querySelector(".dropdown ul")), d == null && (d = o.target.parentNode.parentNode.parentNode.querySelector(".dropdown ul")), d
     }
 
     function a(o) {
         const d = n(o);
         if (d.style.display == "block") d.style.display = "none";
         else {
             const c = o.target.getBoundingClientRect();
-            document.querySelectorAll(".dropdown").forEach(s => s.style.display = "none"), d.style.left = c.left - 150 + c.width + "px", d.style.display = "block"
+            document.querySelectorAll(".dropdown ul").forEach(s => s.style.display = "none"), d.style.left = c.left - 150 + c.width + "px", d.style.display = "block"
         }
     }
 
     function r(o) {
         const d = n(o);
         d.style.display = "none"
     }
 
     function i() {
-        const o = {
-                padding: 0,
-                position: "absolute",
-                width: 150,
-                left: 0,
-                textAlign: "center",
-                backgroundColor: "white",
-                boxShadow: "15px 15px 10px -15px #DDD",
-                display: "none"
-            },
-            d = {
-                listStyleType: "none",
-                padding: 10
-            };
-        return t.jsxs(t.Fragment, {
+        return A(`
+      .dropdown > div {
+        cursor: pointer;
+      }
+      .dropdown ul{
+        padding: 0px;
+        position: absolute;
+        width: 150px;
+        left: 0px;
+        text-align: center;
+        background-color: white;
+        box-shadow: 15px 15px 10px -15px #DDD;
+        display: none;
+      }
+      .dropdown li{
+        list-style-type: none;
+        padding: 10px;
+      }
+    `), t.jsxs("div", {
+            className: "dropdown",
             children: [t.jsx("div", {
                 onClick: a,
-                style: {
-                    cursor: "pointer"
-                },
-                "data-label": M(e.dataLabel),
+                "data-label": E(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
-                style: o,
                 onMouseLeave: r,
-                className: "dropdown",
-                children: e.actions.map(c => t.jsx("li", {
-                    style: d,
+                children: e.actions.map(o => t.jsx("li", {
                     children: t.jsx(F, {
-                        data: c,
+                        data: o,
                         style: {
-                            padding: 0
+                            padding: 0,
+                            whiteSpace: "normal"
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
     return i()
 }
 
-function O({
+function _({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: i,
     onClick: o,
     dataLabel: d,
     style: c
 }) {
     const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
-        s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
+        s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? we(s) : r ? Ae(s) : window.load(s))
     }
 
     function l() {
         return t.jsx("a", {
             id: e,
             onClick: o || u,
             href: s || "#",
-            "data-label": M(d),
+            "data-label": E(d),
             style: c,
             children: i
         })
     }
     return l()
 }
 
@@ -615,24 +630,14 @@
         return t.jsx("div", {
             style: r,
             children: e.children
         }, Math.random())
     }
     return n()
 }
-const xe = {};
-
-function _(e) {
-    let n = "",
-        a = window.document.styleSheets[0];
-    e.split("}").forEach(r => {
-        let i = (r + "}").replace(/\r?\n|\r/g, "");
-        n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && xe[n] == null && (a.insertRule(n, a.cssRules.length), n = "", xe[n] = !0)
-    })
-}
 
 function X(e) {
     function n() {
         return e.data.url ? t.jsx(We, {
             data: e.data
         }) : t.jsx(je, {
             data: e.data
@@ -647,15 +652,15 @@
             children: [t.jsx("strong", {
                 children: e.data.label
             }), ":", t.jsx("br", {})]
         })
     }
 
     function a() {
-        return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(O, {
+        return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(_, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
                 children: [W(e.data.value), t.jsx(C, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
@@ -679,15 +684,15 @@
 }
 
 function We(e) {
     const n = Math.random(),
         [a, r] = D.useState(e.data);
 
     function i(d) {
-        B("GET", d, function(c) {
+        q("GET", d, function(c) {
             r(c)
         })
     }
 
     function o() {
         return window[n] = () => i(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
@@ -778,15 +783,15 @@
             children: [n(), a(), r()]
         })
     }
     return i()
 }
 
 function Pe(e) {
-    _(`
+    A(`
     .cards{
       padding: 10px;
       box-shadow: 0 1px 6px rgba( 0, 0, 0 , 0.16 );
       margin: 10px;
       max-width: 300px;
     }
     .cards h3{
@@ -911,15 +916,15 @@
     }
     return o()
 }
 
 function Ge(e) {
     const n = Math.random(),
         [a, r] = D.useState(e.data);
-    _(`
+    A(`
     .object-fieldset{
       margin-top: 10px;
     }
   `);
 
     function i() {
         return t.jsx(ke, {
@@ -957,15 +962,15 @@
             }, Math.random())
         }) : t.jsx(x, {
             data: a.data
         })
     }
 
     function c(u) {
-        B("GET", u, function(l) {
+        q("GET", u, function(l) {
             r(l)
         })
     }
 
     function s() {
         return e.data.url ? (window[n] = () => c(e.data.url), t.jsxs("div", {
             className: e.data.url ? "reloadable object-fieldset" : "object-fieldset",
@@ -985,15 +990,15 @@
 
     function i() {
         const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + c + "only=actions"
     }
 
     function o() {
-        B("GET", i(), function(c) {
+        q("GET", i(), function(c) {
             r(c)
         })
     }
 
     function d() {
         return window[n] = () => o(), t.jsx("div", {
             className: "reloadable",
@@ -1007,31 +1012,31 @@
         })
     }
     return d()
 }
 
 function Xe(e) {
     function n() {
-        return _(`
+        return A(`
       .object-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .object-title h1 {
           margin: 0;
-          color: ${j.colors.primary};
+          color: ${w.colors.primary};
       }
     `), t.jsxs("div", {
             className: "object-title",
             style: {
                 flexDirection: window.innerWidth > 800 ? "row" : "column"
             },
             children: [e.data.title && t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     margin: 10
                 },
                 children: t.jsx(Ye, {
                     data: e.data
@@ -1039,30 +1044,30 @@
             })]
         })
     }
     return n()
 }
 
 function ke(e) {
-    _(`
+    A(`
       .fieldset-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .fieldset-title h2 {
           margin: 0
       }
     `);
 
     function n() {
         return t.jsxs("div", {
             className: "fieldset-title",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(a) {
                     return t.jsx(F, {
                         data: a,
                         default: !0
                     }, Math.random())
@@ -1123,15 +1128,15 @@
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function Je(e) {
-    _(`
+    A(`
     .noscroll::-webkit-scrollbar {
       display: none;
     }
     .noscroll {
       -ms-overflow-style: none;  /* IE and Edge */
       scrollbar-width: none;  /* Firefox */
       min-height: 2rem;
@@ -1147,43 +1152,43 @@
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20,
                 overflowX: "auto"
             },
             children: e.data.map(function(i, o) {
-                return t.jsx(O, {
+                return t.jsx(_, {
                     href: i.url,
                     style: {
                         padding: 5,
                         fontWeight: n == o ? "bold" : "normal",
                         borderBottom: n == o ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
                         d.preventDefault(), a(o), e.loadContent(i.url)
                     },
-                    dataLabel: M(i.title),
+                    dataLabel: E(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Qe(e) {
     var n = Math.random();
     const [a, r] = D.useState(e.data.data[0]);
 
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": M(e.data.title),
+            "data-label": E(e.data.title),
             children: e.data.title
         })
     }
 
     function o() {
         return t.jsx(ae, {
             data: e.data.actions
@@ -1223,15 +1228,15 @@
         };
         return t.jsx("div", {
             style: h
         })
     }
 
     function u(h) {
-        B("GET", h, function(f) {
+        q("GET", h, function(f) {
             r(f)
         })
     }
 
     function l() {
         return window[n] = () => u(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
@@ -1244,15 +1249,15 @@
 
 function Ke() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function R({
+function O({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: i,
     primary: o,
     compact: d,
@@ -1273,29 +1278,34 @@
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
+        A(`
+      .button{
+        padding: 12px;
+        text-decoration: none;
+        white-space: nowrap;
+        border-radius: 5px;
+        margin: 5px;
+        cursor: pointer;
+        width: fit-content;
+        text-wrap: nowrap;
+      }
+    `);
         const l = {
-            padding: 12,
-            textDecoration: "none",
-            whiteSpace: "nowrap",
-            borderRadius: 5,
-            margin: 5,
-            cursor: "pointer",
-            display: i || "block",
-            width: "fit-content",
-            textWrap: "nowrap"
+            display: i || "block"
         };
-        return o ? (l.backgroundColor = j.colors.primary, l.color = "white") : (l.border = "solid 1px " + j.colors.primary, l.color = j.colors.primary), t.jsx("a", {
+        return o ? (l.backgroundColor = w.colors.primary, l.color = "white") : (l.border = "solid 1px " + w.colors.primary, l.color = w.colors.primary), t.jsx("a", {
             id: e,
+            className: "button",
             style: l,
-            "data-label": M(r || a),
+            "data-label": E(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
     return u()
@@ -1356,18 +1366,18 @@
             },
             children: o.number
         })
     }
 
     function a(o) {
         return {
-            border: "3px solid " + j.colors.primary,
+            border: "3px solid " + w.colors.primary,
             borderRadius: "50%",
-            background: o.done ? j.colors.primary : "white",
-            color: o.done ? "white" : j.colors.primary,
+            background: o.done ? w.colors.primary : "white",
+            color: o.done ? "white" : w.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -1440,15 +1450,15 @@
             i = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: j.colors[e.data.style]
+                backgroundColor: w.colors[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
                 style: i,
                 children: t.jsxs("span", {
                     style: r,
@@ -1458,15 +1468,15 @@
         })
     }
     return n()
 }
 
 function rt(e) {
     function n() {
-        return e.data.color = j.colors[e.data.style], t.jsx(Se, {
+        return e.data.color = w.colors[e.data.style], t.jsx(Se, {
             data: e.data
         })
     }
     return n()
 }
 
 function Se(e) {
@@ -1515,34 +1525,34 @@
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
             i = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: j.colors.auxiliary
+                color: w.colors.auxiliary
             },
             o = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: j.colors.primary
+                color: w.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 style: {
-                    color: j.colors.primary
+                    color: w.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
-                children: e.data.items.map(d => t.jsxs(O, {
+                children: e.data.items.map(d => t.jsxs(_, {
                     href: d.url,
                     style: r,
                     dataLabel: d.label,
                     children: [t.jsx("div", {
                         children: t.jsx(C, {
                             style: i,
                             icon: d.icon
@@ -1576,15 +1586,15 @@
         })
     }
     return n()
 }
 
 function lt(e) {
     function n() {
-        return e.data.url ? t.jsx(O, {
+        return e.data.url ? t.jsx(_, {
             href: e.data.url,
             imodal: !!e.data.modal,
             children: e.data.icon ? t.jsx(C, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
@@ -1628,15 +1638,15 @@
     return a()
 }
 
 function ct(e) {
     function n() {
         const a = {
                 color: "white",
-                backgroundColor: j.colors.highlight,
+                backgroundColor: w.colors.highlight,
                 margin: -20,
                 textAlign: "center",
                 paddingTop: 20,
                 paddingBottom: 70
             },
             r = {
                 fontSize: "4rem",
@@ -1648,31 +1658,31 @@
                 maxWidth: 200,
                 margin: "auto"
             };
         if (e.data) return t.jsxs("div", {
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
                 children: e.data.items.map(o => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
                         children: W(o.value)
                     }), t.jsx("div", {
                         style: i,
                         children: o.name
                     })]
                 }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
-                children: e.data.actions.map(o => t.jsx(O, {
-                    href: A(o.url),
+                children: e.data.actions.map(o => t.jsx(_, {
+                    href: R(o.url),
                     label: o.label,
                     modal: o.modal,
                     children: o.label
                 }, Math.random()))
             })]
         })
     }
@@ -1736,16 +1746,16 @@
             deselect: c
         })
     }
 
     function f(m) {
         if (!e.data.readonly && !(e.data.single_selection && y().length > 0 && m.target.style.backgroundColor != i) && a && m.target.style.backgroundColor != o) {
             const I = m.target.dataset.day.split("/"),
-                k = m.target.dataset.time.split(":");
-            new Date(parseInt(I[2], 10), parseInt(I[1], 10) - 1, parseInt(I[0], 10), parseInt(k[0], 10), parseInt(k[1], 10)) > new Date && (m.target.style.backgroundColor == r ? (m.target.style.backgroundColor = i, console.log("MARCOU", m.target.dataset.day, m.target.dataset.time), d.push([m.target.dataset.day, m.target.dataset.time])) : (m.target.style.backgroundColor = r, console.log("DEMARCOU", m.target.dataset.day, m.target.dataset.time), c.push([m.target.dataset.day, m.target.dataset.time])))
+                j = m.target.dataset.time.split(":");
+            new Date(parseInt(I[2], 10), parseInt(I[1], 10) - 1, parseInt(I[0], 10), parseInt(j[0], 10), parseInt(j[1], 10)) > new Date && (m.target.style.backgroundColor == r ? (m.target.style.backgroundColor = i, console.log("MARCOU", m.target.dataset.day, m.target.dataset.time), d.push([m.target.dataset.day, m.target.dataset.time])) : (m.target.style.backgroundColor = r, console.log("DEMARCOU", m.target.dataset.day, m.target.dataset.time), c.push([m.target.dataset.day, m.target.dataset.time])))
         }
     }
 
     function v(m) {
         const I = m.split("/");
         return s[new Date(parseInt(I[2], 10), parseInt(I[1], 10) - 1, parseInt(I[0], 10)).getDay()]
     }
@@ -1753,26 +1763,26 @@
     function y() {
         const m = [];
         return document.getElementById(n).querySelectorAll("td").forEach(function(I) {
             I.style.backgroundColor == i && m.push(I.dataset.day, I.dataset.time)
         }), m
     }
 
-    function p() {
+    function k() {
         const m = {
                 overflowX: "auto"
             },
             I = {
                 width: "100%",
                 borderSpacing: 0,
                 borderCollapse: "collapse",
                 marginTop: 15,
                 marginBottom: 15
             },
-            k = {
+            j = {
                 border: "solid 4px white"
             };
         return t.jsxs("div", {
             id: n,
             style: m,
             children: [t.jsx("input", {
                 id: "input" + n,
@@ -1783,41 +1793,41 @@
                 onMouseDown: l,
                 onMouseUp: h,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: e.data.matrix[0].map(function(N) {
                             return t.jsxs("th", {
                                 className: "bold",
-                                style: k,
+                                style: j,
                                 children: [v(N.text), t.jsx("br", {}), N.text]
                             }, Math.random())
                         })
                     })
                 }), t.jsx("tbody", {
                     children: e.data.matrix.map(function(N, b) {
                         if (b > 0) return t.jsx("tr", {
-                            children: N.map(function(S, E) {
-                                if (E == 0) return t.jsx("th", {
+                            children: N.map(function(S, M) {
+                                if (M == 0) return t.jsx("th", {
                                     className: "bold",
                                     align: "center",
-                                    style: k,
+                                    style: j,
                                     children: S.text
                                 }, Math.random());
                                 {
                                     const g = {
                                         backgroundColor: u(S),
                                         border: "solid 4px white"
                                     };
                                     return console.log(S), t.jsx("td", {
                                         align: "center",
                                         style: g,
                                         onMouseDown: f,
                                         onMouseLeave: f,
                                         onMouseUp: f,
-                                        "data-day": e.data.matrix[0][E].text,
+                                        "data-day": e.data.matrix[0][M].text,
                                         "data-time": N[0].text,
                                         children: S && S.text && t.jsx(mt, {
                                             text: S.text,
                                             children: t.jsx(C, {
                                                 icon: S.icon || "stethoscope",
                                                 style: {
                                                     color: "white",
@@ -1830,28 +1840,28 @@
                             })
                         }, Math.random())
                     })
                 })]
             })]
         })
     }
-    return p()
+    return k()
 }
 
 function mt(e) {
     function n() {
-        return _(`
+        return A(`
       .tooltip {
         position: relative;
         display: inline-block;
       }
       .tooltip .tooltiptext {
         visibility: hidden;
         width: 220px;
-        background-color: ${j.colors.highlight};
+        background-color: ${w.colors.highlight};
         color: #fff;
         text-align: center;
         border-radius: 6px;
         padding: 5px 0;
         position: absolute;
         z-index: 1;
         bottom: 150%;
@@ -1900,15 +1910,15 @@
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
 function V(e, n) {
-    B("GET", Q(n, e.closest("form"), e.name), Ee)
+    q("GET", Q(n, e.closest("form"), e.name), Me)
 }
 
 function xt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -1944,53 +1954,53 @@
                 if (r.options[i].value == n) {
                     r.selectedIndex = i;
                     break
                 }
     }
 }
 
-function Ee(e) {
+function Me(e) {
     if (e) {
         for (var n = 0; n < e.hide.length; n++) xt(e.hide[n]);
         for (var n = 0; n < e.show.length; n++) yt(e.show[n]);
         for (var n = 0; n < e.reload.length; n++) vt(e.reload[n]);
         for (var a in e.set) bt(a, e.set[a])
     }
 }
 
-function wt(e) {
+function pt(e) {
     function n() {
         const a = {
-            color: j.colors.info,
-            backgroundColor: j.background.info,
+            color: w.colors.info,
+            backgroundColor: w.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
                 children: [t.jsx(C, {
                     icon: "circle-check",
                     style: {
-                        color: j.colors.info,
+                        color: w.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function pt(e) {
+function wt(e) {
     function n() {
         const a = {
             color: "white",
             display: "none",
             backgroundColor: "#e52207",
             marginTop: 2,
             marginBottom: 2,
@@ -2063,15 +2073,15 @@
             data: e.data
         }) : t.jsx(Ct, {
             data: e.data
         }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ve, {
             data: e.data
         }) : t.jsx(le, {
             data: e.data
-        }) : t.jsx(Me, {
+        }) : t.jsx(Ee, {
             data: e.data
         }) : e.data.type == "decimal" ? t.jsx(ye, {
             data: e.data
         }) : e.data.type == "boolean" ? t.jsx(St, {
             data: e.data
         }) : e.data.type == "textarea" ? t.jsx(kt, {
             data: e.data
@@ -2080,15 +2090,15 @@
         })) : t.jsx("span", {
             children: e.data.name
         })
     }
 
     function i() {
         return t.jsx("div", {
-            children: t.jsx(pt, {
+            children: t.jsx(wt, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function o() {
         return e.data.help_text && t.jsx(jt, {
@@ -2145,23 +2155,23 @@
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (oe(s.name)) {
                     const v = "display" + a;
                     var l = document.createElement("img");
                     l.id = d.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(y) {
-                        const p = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
+                        const k = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
                         var m = document.createElement("canvas");
                         const I = m.getContext("2d");
                         m.height = m.width * (l.height / l.width);
-                        const k = document.createElement("canvas"),
-                            N = k.getContext("2d");
-                        k.width = l.width * p, k.height = l.height * p, N.drawImage(l, 0, 0, k.width, k.height), I.drawImage(k, 0, 0, k.width * p, k.height * p, 0, 0, m.width, m.height), k.toBlob(function(S) {
-                            const E = new DataTransfer;
-                            E.items.add(new File([S], s.name)), d.target.files = E.files
+                        const j = document.createElement("canvas"),
+                            N = j.getContext("2d");
+                        j.width = l.width * k, j.height = l.height * k, N.drawImage(l, 0, 0, j.width, j.height), I.drawImage(j, 0, 0, j.width * k, j.height * k, 0, 0, m.width, m.height), j.toBlob(function(S) {
+                            const M = new DataTransfer;
+                            M.items.add(new File([S], s.name)), d.target.files = M.files
                         });
                         var b = document.getElementById(v);
                         b == null ? (b = document.createElement("div"), b.id = v) : b.removeChild(b.childNodes[0]), b.appendChild(l), d.target.parentNode.appendChild(b)
                     }, l.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
                 var f = s.size / 1024;
@@ -2193,15 +2203,15 @@
                     },
                     children: [t.jsx("div", {
                         style: u,
                         children: t.jsx(C, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: j.colors.primary
+                                color: w.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
                         children: [e.data.value && oe(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
@@ -2219,25 +2229,25 @@
                             className: "bold",
                             id: "fileinfo" + a,
                             children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
-                        children: t.jsx(R, {
+                        children: t.jsx(O, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: d,
                     name: e.data.name,
                     id: a,
-                    "data-label": M(e.data.label),
+                    "data-label": E(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: i,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
@@ -2250,26 +2260,26 @@
                 ...$
             }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: i,
                 style: s
             })
         }
     }
     return o()
 }
 
-function Me(e) {
+function Ee(e) {
     var n = [];
     Array.isArray(e.data.value) ? e.data.value.forEach(function(b, S) {
         n.push({
             id: b.id,
             value: b.label
         })
     }) : e.data.value != null && n.push({
@@ -2292,42 +2302,42 @@
     function h() {
         const b = document.getElementById(a);
         if (i) {
             const S = {
                     padding: 5,
                     display: "inline"
                 },
-                E = {
+                M = {
                     cursor: "pointer",
                     marginRight: 5
                 },
                 g = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((w, T) => t.jsxs("div", {
+                children: [b == null && n.map((p, T) => t.jsxs("div", {
                     style: S,
                     children: [t.jsx("span", {
-                        onClick: () => k(T),
-                        style: E,
+                        onClick: () => j(T),
+                        style: M,
                         children: t.jsx(C, {
                             icon: "trash-can",
                             style: g
                         })
-                    }), w.value]
-                }, Math.random())), b != null && Array.from(b.options).map((w, T) => t.jsxs("div", {
+                    }), p.value]
+                }, Math.random())), b != null && Array.from(b.options).map((p, T) => t.jsxs("div", {
                     style: S,
                     children: [t.jsx("span", {
-                        onClick: () => k(T),
-                        style: E,
+                        onClick: () => j(T),
+                        style: M,
                         children: t.jsx(C, {
                             icon: "trash-can",
                             style: g
                         })
-                    }), w.innerHTML]
+                    }), p.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function f() {
         return t.jsx("select", {
@@ -2353,113 +2363,113 @@
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto",
                 zIndex: 99999
             };
         S.position = "absolute", S.backgroundColor = "white";
-        const E = document.getElementById(r);
-        if (e.data.icon && (b.paddingLeft = 30), E) {
-            let q = null,
-                K = E,
+        const M = document.getElementById(r);
+        if (e.data.icon && (b.paddingLeft = 30), M) {
+            let L = null,
+                K = M,
                 ie = null;
             for (; !ie && (K = K.parentElement) instanceof HTMLElement;) K.matches("dialog") && (ie = K);
-            q = ie;
-            const Z = E.getBoundingClientRect();
+            L = ie;
+            const Z = M.getBoundingClientRect();
             var g = Z.top + Z.height,
-                w = Z.left;
-            if (q) {
-                const fe = q.getBoundingClientRect();
-                g = g - fe.top, w = w - fe.left
-            } else g += window.scrollY, w += window.scrollX;
-            S.width = Z.width, S.top = g, S.left = w
+                p = Z.left;
+            if (L) {
+                const fe = L.getBoundingClientRect();
+                g = g - fe.top, p = p - fe.left
+            } else g += window.scrollY, p += window.scrollX;
+            S.width = Z.width, S.top = g, S.left = p
         }
         const T = {
                 cursor: "pointer",
                 padding: 10
             },
-            L = !i && n.length > 0 && n[0].value || "";
+            B = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [e.data.icon && t.jsx(C, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: q => {
-                    q.target.select(), m(q)
+                onFocus: L => {
+                    L.target.select(), m(L)
                 },
                 onChange: m,
                 onMouseLeave: y,
                 onBlur: y,
-                defaultValue: L,
+                defaultValue: B,
                 style: b,
-                "data-label": M(e.data.label)
+                "data-label": E(e.data.label)
             }), c && o && t.jsxs("ul", {
                 style: S,
-                onMouseLeave: p,
-                onMouseEnter: function(q) {
+                onMouseLeave: k,
+                onMouseEnter: function(L) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
                     style: T,
                     children: "Nenhuma opção encontrada."
-                }), c.map(q => t.jsx("li", {
+                }), c.map(L => t.jsx("li", {
                     onClick: () => {
-                        d(!1), e.onSelect ? e.onSelect(q) : I(q)
+                        d(!1), e.onSelect ? e.onSelect(L) : I(L)
                     },
                     style: T,
                     className: "autocomplete-item",
-                    "data-label": M(q.value),
-                    children: q.value
+                    "data-label": E(L.value),
+                    children: L.value
                 }, Math.random()))]
             })]
         })
     }
 
     function y(b) {
         u = !1, setTimeout(function() {
-            u || p(b)
+            u || k(b)
         }, 250)
     }
 
-    function p(b) {
+    function k(b) {
         const S = document.getElementById(a);
         if (S) {
-            const E = document.getElementById(r);
-            i || S.options.length > 0 && E.value != S.options[0].innerHTML && (S.innerHTML = "", E.value = "", d(!1), e.data.onchange && V(E, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
+            const M = document.getElementById(r);
+            i || S.options.length > 0 && M.value != S.options[0].innerHTML && (S.innerHTML = "", M.value = "", d(!1), e.data.onchange && V(M, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
     function m(b) {
         clearTimeout(l), l = setTimeout(function() {
             const S = b.target.closest("form"),
-                E = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), B("GET", Q(e.data.choices + E + "term=" + b.target.value, S), function(w) {
-                s(w)
+                M = e.data.choices.indexOf("?") < 0 ? "?" : "&";
+            d(!0), q("GET", Q(e.data.choices + M + "term=" + b.target.value, S), function(p) {
+                s(p)
             })
         }, 1e3)
     }
 
     function I(b, S = !1) {
-        const E = document.getElementById(a),
+        const M = document.getElementById(a),
             g = document.getElementById(r);
-        E.innerHTML == null && (E.innerHTML = ""), Array.isArray(b) ? E.innerHTML = b.map(w => `<option selected value="${w.id}">${w.value}</option>`).join("") : i ? (E.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (E.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !S && V(g, e.data.onchange)
+        M.innerHTML == null && (M.innerHTML = ""), Array.isArray(b) ? M.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (M.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (M.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !S && V(g, e.data.onchange)
     }
 
-    function k(b) {
+    function j(b) {
         const S = document.getElementById(a);
-        var E = Array.from(S.options);
-        S.innerHTML = E.slice(0, b).concat(E.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), s([])
+        var M = Array.from(S.options);
+        S.innerHTML = M.slice(0, b).concat(M.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), s([])
     }
 
     function N() {
         return t.jsxs(t.Fragment, {
             children: [h(), f(), v()]
         })
     }
@@ -2470,15 +2480,15 @@
     function n() {
         var a = {
             ...$
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": M(e.data.label),
+            "data-label": E(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
@@ -2513,15 +2523,15 @@
     function c(u) {
         var l = document.getElementById(u);
         i.checked = l.checked
     }
 
     function s() {
         return window["reload-" + i.name + "-field"] = function() {
-            B("GET", Q(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
+            q("GET", Q(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
                 a(l)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "radio-group " + i.name,
             children: n.map((u, l) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2531,15 +2541,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + l,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
                     defaultChecked: o(u),
-                    "data-label": M(u.value),
+                    "data-label": E(u.value),
                     onClick: function() {
                         d(i.name + r + l)
                     },
                     onMouseEnter: function() {
                         c(i.name + r + l)
                     }
                 }), t.jsx("label", {
@@ -2576,15 +2586,15 @@
 
     function d(s) {
         e.data.onchange && V(s.target, e.data.onchange)
     }
 
     function c() {
         return window["reload-" + i.name + "-field"] = function() {
-            B("GET", Q(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
+            q("GET", Q(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
                 a(u)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "checkbox-group " + i.name,
             children: n.map((s, u) => (s.id || s.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2595,15 +2605,15 @@
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
                     defaultChecked: o(s),
-                    "data-label": M(s.value)
+                    "data-label": E(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
             className: "checkbox-group empty " + i.name,
@@ -2620,44 +2630,44 @@
 function Ct(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": M(n.label),
+            "data-label": E(n.label),
             defaultValue: n.value,
             style: $,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
 
-function Et(e) {
+function Mt(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(J, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(R, {
+                children: [t.jsx(O, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => o(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(R, {
+                }), t.jsx(O, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => o(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
@@ -2692,23 +2702,23 @@
         const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: s,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), i(), d()]
         })
     }
     return c()
 }
 
-function Mt(e) {
+function Et(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
     function r(l, h) {
         const f = n;
         return n += 1, t.jsxs("div", {
@@ -2720,21 +2730,21 @@
                 data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(R, {
+                children: [t.jsx(O, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => o(),
                     id: "extra-add-" + f + "-",
                     display: h
-                }), t.jsx(R, {
+                }), t.jsx(O, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => d(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
@@ -2783,15 +2793,15 @@
     function s() {
         return t.jsx("div", {
             id: "info-" + a,
             children: t.jsx(J, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(R, {
+                children: t.jsx(O, {
                     primary: !0,
                     icon: "add",
                     onClick: () => o(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
@@ -2802,15 +2812,15 @@
         const l = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: l,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
                 children: [s(), e.data.value.map(function(h, f) {
@@ -2820,36 +2830,36 @@
         })
     }
     return u()
 }
 
 function ue(e) {
     D.useEffect(() => {
-        e.data.controls && Ee(e.data.controls)
+        e.data.controls && Me(e.data.controls)
     }, []);
 
     function n(r) {
-        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Et, {
+        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Mt, {
             data: r
-        }, Math.random()) : t.jsx(Mt, {
+        }, Math.random()) : t.jsx(Et, {
             data: r
         }, Math.random()) : t.jsx(te, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": M(r.title),
+                    "data-label": E(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
                     children: i.map(o => t.jsx("div", {
                         className: "form-group " + o.name,
@@ -2868,24 +2878,24 @@
 
 function Tt(e) {
     const n = Math.random();
 
     function a() {
         const h = {
             margin: 0,
-            color: j.colors.primary
+            color: w.colors.primary
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
     function r() {
-        return e.data.info && t.jsx(wt, {
+        return e.data.info && t.jsx(pt, {
             data: {
                 text: e.data.info
             }
         })
     }
 
     function i() {
@@ -2908,20 +2918,20 @@
 
     function d() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(R, {
+            children: [t.jsx(O, {
                 onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(R, {
+            }), t.jsx(O, {
                 onClick: l,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
@@ -2964,43 +2974,53 @@
 
     function l(h) {
         h.preventDefault();
         var f = e.data.url,
             v = document.getElementById(n),
             y = new FormData(v);
         if (v.method.toUpperCase() == "GET") {
-            const p = f.indexOf("?") >= 0 ? "&" : "?";
-            f = f + p + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
+            const k = f.indexOf("?") >= 0 ? "&" : "?";
+            f = f + k + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
         }
-        B(v.method.toUpperCase(), f, function(m) {
-            if (v.querySelectorAll(".error").forEach(k => k.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), m.type == "response") m.store && Object.keys(m.store).map(function(k) {
-                m.store[k] ? localStorage.setItem(k, m.store[k]) : localStorage.removeItem(k, m.store[k])
-            }), m.redirect && m.redirect.length > 2 ? (m.message && localStorage.setItem("message", m.message), document.location.href = U(m.redirect)) : (m.message && z(m.message), m.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : Y()), m.redirect == "." && v.reset(), m.dispose && (v.style.display = "none"), Ke());
+        q(v.method.toUpperCase(), f, function(m) {
+            if (v.querySelectorAll(".error").forEach(j => j.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), m.type == "response")
+                if (m.store && Object.keys(m.store).map(function(j) {
+                        m.store[j] ? localStorage.setItem(j, m.store[j]) : localStorage.removeItem(j, m.store[j])
+                    }), m.redirect && m.redirect.length > 2) m.message && localStorage.setItem("message", m.message), document.location.href = U(m.redirect);
+                else if (m.message && z(m.message), m.task) {
+                let j = function() {
+                    q("GET", "/api/taskprogress/" + m.task + "/", function(S) {
+                        S == null || S.progress == 100 ? h.target.innerHTML = N : (h.target.innerHTML = "Aguarde... (" + S.progress + "%)", setTimeout(j, 5e3))
+                    })
+                };
+                const N = h.target.innerHTML;
+                h.target.innerHTML = "Aguarde... (0%)", j()
+            } else m.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : Y()), m.redirect == "." && v.reset(), m.dispose && (v.style.display = "none"), Ke();
             else if (m.type == "error") {
                 var I = m.text;
-                console.log(m), Object.keys(m.errors).map(function(k) {
-                    if (k == "__all__") I = m.errors[k];
+                console.log(m), Object.keys(m.errors).map(function(j) {
+                    if (j == "__all__") I = m.errors[j];
                     else {
-                        const N = v.querySelector("#" + k + "_error");
-                        N.querySelector("span").innerHTML = m.errors[k], N.style.display = "block"
+                        const N = v.querySelector("#" + j + "_error");
+                        N.querySelector("span").innerHTML = m.errors[j], N.style.display = "block"
                     }
                 }), z(I, !0)
             } else {
-                const k = document.querySelector("#output");
-                k.innerHTML = "", H.createRoot(k.appendChild(document.createElement("div"))).render(t.jsx(x, {
+                const j = document.querySelector("#output");
+                j.innerHTML = "", H.createRoot(j.appendChild(document.createElement("div"))).render(t.jsx(x, {
                     data: m
                 }))
             }
         }, y)
     }
     return s()
 }
 
 function It(e) {
-    _(`
+    A(`
         .calendar table{
             width: 100%;
             border-spacing: 0px;
             border-collapse: collapse;
             margin-top: 15px;
             margin-bottom: 15px;
         }
@@ -3116,15 +3136,15 @@
                                 }) : h.date + h.today
                             }), h.total && t.jsx("div", {
                                 className: "total",
                                 onClick: () => e.onChange(h.date, e.data.month, e.data.year),
                                 children: t.jsx("div", {
                                     className: "number",
                                     style: {
-                                        backgroundColor: j.colors.primary,
+                                        backgroundColor: w.colors.primary,
                                         textDecoration: h.selected ? "underline" : "normal",
                                         display: "inline-block"
                                     },
                                     children: h.total
                                 })
                             }), !h.total && t.jsx("div", {
                                 className: "total",
@@ -3136,15 +3156,15 @@
             })]
         })
     }
     return u()
 }
 
 function Dt(e) {
-    _(`
+    A(`
       .paginator{
         display: flex;
         justify-content: space-between;
         line-height: 4rem;
         align-items: baseline;
       }
       .paginator .inline{
@@ -3202,20 +3222,20 @@
                         },
                         onKeyDown: function(a) {
                             a.key == "Enter" && (a.preventDefault(), e.onChange(a.target.value < 0 ? 1 : Math.min(a.target.value, e.data.page.total)))
                         }
                     }), t.jsx("div", {
                         className: "inline",
                         children: "|"
-                    }), e.data.page.previous && t.jsx(R, {
+                    }), e.data.page.previous && t.jsx(O, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
                         onClick: () => e.onChange(e.data.page.previous)
-                    }), e.data.page.next && t.jsx(R, {
+                    }), e.data.page.next && t.jsx(O, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
                         onClick: () => e.onChange(e.data.page.next)
                     })]
                 })
             })]
@@ -3223,15 +3243,15 @@
     }
     return n()
 }
 
 function Nt(e) {
     function n() {
         const a = {
-            backgroundColor: j.colors.primary,
+            backgroundColor: w.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -3243,16 +3263,16 @@
             style: a,
             children: e.total
         })
     }
     return n()
 }
 
-function qt(e) {
-    _(`
+function Lt(e) {
+    A(`
     .queryset h1, .queryset h2{
       margin: 0px;
     }
     .queryset .title{
       display: flex;
       justify-content: space-between;
       align-items: center;
@@ -3275,18 +3295,18 @@
         text-decoration: none;
     }
   `), e.data.id == null && (e.data.id = Math.random());
     const [n, a] = D.useState(e.data);
 
     function r() {
         return n.attrname ? t.jsx("h2", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: n.title
         }) : t.jsxs("h1", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: [n.title, " ", n.total > 10 && "(" + n.total + ")"]
         })
     }
 
     function i() {
         return t.jsxs("div", {
             className: "title",
@@ -3300,85 +3320,85 @@
     function o(g) {
         document.getElementById("loader-" + e.data.id).style.display = g ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
-            children: n.subsets.map(function(g, w) {
-                var T = n.subset === g.name || !n.subset && w == 0;
-                return t.jsxs(O, {
+            children: n.subsets.map(function(g, p) {
+                var T = n.subset === g.name || !n.subset && p == 0;
+                return t.jsxs(_, {
                     href: "#",
                     style: {
                         borderBottom: T ? "solid 3px #2670e8" : 0,
                         color: "#0c326f"
                     },
-                    onClick: function(L) {
-                        L.preventDefault(), c(g.name)
+                    onClick: function(B) {
+                        B.preventDefault(), c(g.name)
                     },
-                    dataLabel: M(g.label),
+                    dataLabel: E(g.label),
                     children: [g.label, " ", t.jsx(Nt, {
                         total: g.count
                     })]
                 }, Math.random())
             })
         })
     }
 
     function c(g) {
-        const w = document.getElementById("subset-" + e.data.id);
-        w.value = g || "", N()
+        const p = document.getElementById("subset-" + e.data.id);
+        p.value = g || "", N()
     }
 
-    function s(g, w, T) {
-        const L = document.getElementById("form-" + e.data.id);
-        L.querySelector("input[name=" + n.calendar.field + "__day]").value = g || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = w || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = T || "", y(1)
+    function s(g, p, T) {
+        const B = document.getElementById("form-" + e.data.id);
+        B.querySelector("input[name=" + n.calendar.field + "__day]").value = g || "", B.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", B.querySelector("input[name=" + n.calendar.field + "__year]").value = T || "", y(1)
     }
 
     function u() {
         if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
     function l(g) {
-        const w = {
+        const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
-            color: j.colors.primary,
+            color: w.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
             children: [g.map(function(T) {
                 return T.label != "ID" && t.jsx("th", {
-                    style: w,
+                    style: p,
                     className: "bold",
                     children: T.label
                 }, Math.random())
             }), t.jsx("th", {
-                style: w
+                style: p
             })]
         })
     }
 
     function h(g) {
-        const w = {
+        const p = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
             T = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
-                style: w,
+                style: p,
                 children: g.title
             }, Math.random()), t.jsx("td", {
                 style: T,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
@@ -3389,28 +3409,28 @@
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [g.data.map(function(L) {
-                return L.label != "ID" && t.jsx("td", {
-                    style: w,
-                    children: W(L.value)
+            children: [g.data.map(function(B) {
+                return B.label != "ID" && t.jsx("td", {
+                    style: p,
+                    children: W(B.value)
                 }, Math.random())
             }), t.jsx("td", {
                 style: T,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: g.actions.map(function(L) {
+                    children: g.actions.map(function(B) {
                         return t.jsx(F, {
-                            data: L,
+                            data: B,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
@@ -3442,23 +3462,23 @@
     }
 
     function v() {
         const g = {
                 width: "100%",
                 overflowX: "auto"
             },
-            w = {
+            p = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: g,
             children: t.jsxs("table", {
-                style: w,
+                style: p,
                 children: [t.jsx("thead", {
                     children: l(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(T) {
                         return h(T)
                     })
                 })]
@@ -3467,19 +3487,19 @@
     }
 
     function y(g) {
         const T = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
         T && (T.value = g), N(), I()
     }
 
-    function p() {
+    function k() {
         const g = document.getElementById("form-" + e.data.id);
         if (g) {
-            const w = g.querySelector("input[name=page]");
-            w && (w.value = n.pagination.page.current)
+            const p = g.querySelector("input[name=page]");
+            p && (p.value = n.pagination.page.current)
         }
         return t.jsx(Dt, {
             data: n.pagination,
             onChange: y,
             total: n.total
         })
     }
@@ -3504,114 +3524,114 @@
         const g = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
         console.log(g), console.log(e.data.id), window.scrollTo({
             top: g,
             behavior: "smooth"
         })
     }
 
-    function k() {
+    function j() {
         const g = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
-            w = n.search.length > 0,
+            p = n.search.length > 0,
             T = n.filters.length > 0;
-        if ((n.bi || n.data.length >= 0) && (w || T)) {
-            const L = {
+        if ((n.bi || n.data.length >= 0) && (p || T)) {
+            const B = {
                 name: "q",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves",
                 value: n.q
             };
             return t.jsxs("div", {
                 style: g,
                 children: [t.jsxs(P, {
                     width: 250,
-                    children: [w && t.jsx("div", {
+                    children: [p && t.jsx("div", {
                         children: t.jsx(te, {
-                            data: L
+                            data: B
                         })
-                    }), T && n.filters.map(function(q) {
-                        return q.type != "hidden" && t.jsx("div", {
+                    }), T && n.filters.map(function(L) {
+                        return L.type != "hidden" && t.jsx("div", {
                             children: t.jsx(te, {
-                                data: q
+                                data: L
                             })
                         }, Math.random())
                     }), t.jsx("div", {
-                        children: t.jsx(R, {
+                        children: t.jsx(O, {
                             onClick: N,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
-                }), T && n.filters.map(function(q) {
-                    return q.type == "hidden" && t.jsx("div", {
+                }), T && n.filters.map(function(L) {
+                    return L.type == "hidden" && t.jsx("div", {
                         children: t.jsx(te, {
-                            data: q
+                            data: L
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
     function N() {
         o(!0);
         var g;
-        const w = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? g = e.data.url + "&" + w : g = e.data.url + "?" + w, B("GET", g, function(T) {
+        const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
+        e.data.url.indexOf("?") > 0 ? g = e.data.url + "&" + p : g = e.data.url + "?" + p, q("GET", g, function(T) {
             a(T), o(!1)
         })
     }
 
     function b() {
         const g = {
-            color: j.colors.primary
+            color: w.colors.primary
         };
         return e.data.reloadable && t.jsxs("div", {
             align: "center",
             children: [t.jsxs("i", {
                 children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
             }), t.jsx("div", {
-                children: t.jsx(O, {
+                children: t.jsx(_, {
                     style: g,
-                    onClick: w => {
-                        w.preventDefault(), N()
+                    onClick: p => {
+                        p.preventDefault(), N()
                     },
                     children: "Atualizar agora"
                 })
             })]
         })
     }
 
     function S() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [k(), n.bi.map(function(g) {
+            children: [j(), n.bi.map(function(g) {
                 return t.jsx(P, {
                     width: 300,
                     alignItems: "start",
-                    children: g.map(function(w) {
+                    children: g.map(function(p) {
                         return t.jsx("div", {
                             children: t.jsx(x, {
-                                data: w
+                                data: p
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs("div", {
             className: "content",
-            children: [b(), m(), d(), k(), u(), f(), p()]
+            children: [b(), m(), d(), j(), u(), f(), k()]
         })
     }
 
-    function E() {
+    function M() {
         window[e.data.id] = () => N();
         const g = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable queryset",
@@ -3625,15 +3645,15 @@
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
                 }), i(), S()]
             })
         })
     }
-    return E()
+    return M()
 }
 
 function re(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
@@ -3728,23 +3748,23 @@
         return t.jsx(re, {
             option: i
         })
     }
     return r()
 }
 
-function Bt(e) {
+function qt(e) {
     return t.jsx(he, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function Lt(e) {
+function Bt(e) {
     return t.jsx(he, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
@@ -3985,20 +4005,20 @@
         switch (e.type) {
             case "pie":
                 return t.jsx(he, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(Lt, {
+                return t.jsx(Bt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(Bt, {
+                return t.jsx(qt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
                 return t.jsx(At, {
                     headers: e.headers,
                     rows: e.rows
@@ -4058,30 +4078,30 @@
             }), n()]
         })
     }
     return a()
 }
 
 function Pt(e) {
-    _(`
+    A(`
     .statistics .odd {
       background-color: #EEE;
     }
   `);
 
     function n() {
         for (var r = [], i = 0; i < e.data.series.length; i++) r.push([e.data.series[i][0], e.data.series[i][1]]);
         return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
@@ -4117,15 +4137,15 @@
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: i
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: [r && t.jsx("thead", {
@@ -4137,24 +4157,24 @@
                                 padding: 5
                             },
                             children: f
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
                     children: [i.map((f, v) => t.jsx("tr", {
-                        children: f.map((y, p) => p == 0 ? t.jsx("th", {
+                        children: f.map((y, k) => k == 0 ? t.jsx("th", {
                             className: v % 2 == 0 ? "even" : "odd",
                             style: {
                                 textAlign: "left",
                                 padding: 5
                             },
                             children: y
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
-                            className: (p == f.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (v % 2 == 0 ? "even" : "odd"),
+                            className: (k == f.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (v % 2 == 0 ? "even" : "odd"),
                             children: W(y)
                         }, Math.random()))
                     }, Math.random())), d.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {}), d.map(f => t.jsxs("td", {
                             align: "center",
                             className: "bold",
                             children: [W(f), " "]
@@ -4170,25 +4190,25 @@
 function Ut() {
     function e() {
         const o = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: j.colors.success
+            backgroundColor: w.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: o
                 })
             }), t.jsx("div", {
-                children: t.jsx(O, {
+                children: t.jsx(_, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
@@ -4219,41 +4239,41 @@
                 display: d == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 15,
                 paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: j.colors.primary
+                color: w.colors.primary
             },
             s = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return o.url ? t.jsx("li", {
             style: c,
             onClick: n,
             className: "item",
-            children: t.jsxs(O, {
+            children: t.jsxs(_, {
                 href: o.url,
-                dataLabel: M(o.label),
+                dataLabel: E(o.label),
                 style: {
                     textDecoration: "none",
                     display: "block",
                     width: "100%"
                 },
                 children: [d == 0 && t.jsx(C, {
                     icon: o.icon || "dot-circle",
                     style: s
                 }), o.label]
             })
         }, Math.random()) : o.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": M(o.label),
+            "data-label": E(o.label),
             children: [d == 0 && t.jsx(C, {
                 icon: o.icon || "dot-circle",
                 style: s
             }), o.label, t.jsx(C, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
@@ -4317,15 +4337,15 @@
                 o.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: d
                 }).then(function(c) {
                     if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
                         var s = new FormData;
-                        s.append("subscription", n), B("POST", "/api/pushsubscribe/", function(u) {
+                        s.append("subscription", n), q("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
                         }, s)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(c) {
@@ -4339,15 +4359,15 @@
 
     function i() {
         return t.jsx(C, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: j.colors.primary
+                color: w.colors.primary
             }
         })
     }
     return i()
 }
 
 function Yt(e, n) {
@@ -4377,15 +4397,15 @@
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: j.colors.primary,
+                backgroundColor: w.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -4525,15 +4545,19 @@
                         padding: 10
                     },
                     children: t.jsx(ee, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
                         children: t.jsx(C, {
-                            icon: "plus"
+                            icon: "plus",
+                            style: {
+                                cursor: "pointer",
+                                color: w.colors.primary
+                            }
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Gt, {})
@@ -4550,15 +4574,15 @@
                     return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(F, {
                             data: f,
                             primary: !0
                         }, Math.random())
                     }, Math.random())
                 }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
-                    return t.jsx(O, {
+                    return t.jsx(_, {
                         href: f.url,
                         style: {
                             marginRight: 10
                         },
                         children: f.label
                     }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
@@ -4566,53 +4590,61 @@
                         padding: 10
                     },
                     children: t.jsx(ee, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
                         children: t.jsx(C, {
-                            icon: "tools"
+                            icon: "tools",
+                            style: {
+                                cursor: "pointer",
+                                color: w.colors.primary
+                            }
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(ee, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
                         children: t.jsx(C, {
-                            icon: "gear"
+                            icon: "gear",
+                            style: {
+                                cursor: "pointer",
+                                color: w.colors.primary
+                            }
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && e.data.navbar.search && t.jsx("div", {
-                    children: t.jsx(Me, {
+                    children: t.jsx(Ee, {
                         data: h,
                         style: {
                             padding: 10
                         },
                         onSelect: f => document.location.href = U(f.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(ee, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: M(e.data.navbar.user),
+                        dataLabel: E(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: j.colors.primary
+                                backgroundColor: w.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
@@ -4632,20 +4664,20 @@
     function d() {
         const l = {
                 margin: 15,
                 display: "flex",
                 justifyContent: "space-between"
             },
             h = {
-                color: j.colors.primary
+                color: w.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
             style: l,
             children: [t.jsxs("div", {
-                children: [t.jsx(O, {
+                children: [t.jsx(_, {
                     href: "/app/dashboard/",
                     style: {
                         marginRight: 10
                     },
                     children: t.jsx(C, {
                         icon: "home",
                         style: h
@@ -4733,18 +4765,18 @@
 
     function s() {
         console.log("Trying to connect..."), n = new Peer("999123" + e.data.caller.replaceAll(".", "").replaceAll("-", "")), n.on("open", function(y) {
             document.getElementById("callerid").innerHTML = e.data.caller, f(), o = setInterval(function() {
                 i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), f())
             }, 15e3)
         }), n.on("call", function(y) {
-            var p = document.getElementById("video2");
-            p.addEventListener("loadedmetadata", function(m) {
-                p.style.width = this.videoWidth / 4 + "px", p.style.height = this.videoHeight / 4 + "px", p.style.marginLeft = -this.videoWidth / 4 + "px", p.style.visibility = "visible"
-            }, !1), p.srcObject = a, y.answer(a), y.on("stream", function(m) {
+            var k = document.getElementById("video2");
+            k.addEventListener("loadedmetadata", function(m) {
+                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
+            }, !1), k.srcObject = a, y.answer(a), y.on("stream", function(m) {
                 r = m, document.getElementById("video1").srcObject = r, i = !0
             }), y.on("close", function() {
                 console.log("Closed!"), i = !1
             })
         }), n.on("error", function(y) {
             y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? (i = !1, console.log("Problema na conexão do usuário. Tentando novamente em 5 segundos."), setTimeout(s, 5e3)) : y.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
         })
@@ -4752,28 +4784,28 @@
     D.useEffect(() => (s(), function() {
         clearInterval(o), u(), z("Desconectado!")
     }), []);
 
     function u() {
         l(a, "audio"), l(a, "video"), l(r, "audio"), l(r, "video"), a = null, r = null;
         const y = document.getElementById("video1"),
-            p = document.getElementById("video2");
-        y && (y.srcObject = null), p && (p.srcObject = null), console.log("Stopped!"), i = !1
+            k = document.getElementById("video2");
+        y && (y.srcObject = null), k && (k.srcObject = null), console.log("Stopped!"), i = !1
     }
 
-    function l(y, p) {
+    function l(y, k) {
         y != null && y.getTracks().forEach(m => {
-            m.kind === p && m.stop()
+            m.kind === k && m.stop()
         })
     }
 
     function h() {
         var y = n.call("999123" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
-        y && (y.on("stream", function(p) {
-            r = p, document.getElementById("video1").srcObject = r, i = !0
+        y && (y.on("stream", function(k) {
+            r = k, document.getElementById("video1").srcObject = r, i = !0
         }), y.on("close", function() {
             console.log("Closed!"), i = !1
         }))
     }
 
     function f() {
         if (a != null && !i) return h();
@@ -4783,18 +4815,18 @@
                 autoGainControl: !1,
                 echoCancellation: !1,
                 googGainControl: !1,
                 noiseSuppression: !1
             }
         }, function(y) {
             a = y;
-            var p = document.getElementById("video2");
-            p.addEventListener("loadedmetadata", function(m) {
-                p.style.width = this.videoWidth / 4 + "px", p.style.height = this.videoHeight / 4 + "px", p.style.marginLeft = -this.videoWidth / 4 + "px", p.style.visibility = "visible"
-            }, !1), p.srcObject = a, h()
+            var k = document.getElementById("video2");
+            k.addEventListener("loadedmetadata", function(m) {
+                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
+            }, !1), k.srcObject = a, h()
         }, function(y) {
             alert("Failed to get local stream.")
         })
     }
 
     function v() {
         return t.jsx("iframe", {
@@ -4807,15 +4839,15 @@
             allow: "camera; microphone; display-capture"
         })
     }
     return v()
 }
 
 function Qt(e) {
-    _(`
+    A(`
     .container {
         position: relative;
         width: 100%;
         overflow: hidden;
         padding-top: ${window.innerWidth>800?50:100}%;
       }
       .responsive-iframe {
@@ -4859,15 +4891,15 @@
             children: e.data.text
         })
     }
     return a()
 }
 var ne, me = {};
 const Zt = "/api/application/",
-    we = localStorage.getItem("application");
+    pe = localStorage.getItem("application");
 
 function x(e) {
     const n = me[e.data.type];
     return n ? Te.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
@@ -4877,15 +4909,15 @@
     me[n.toLowerCase()] = e
 };
 x.render = function(e) {
     ne = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
 x.register(ht, "Counter");
 x.register(Tt, "Form");
-x.register(qt, "QuerySet");
+x.register(Lt, "QuerySet");
 x.register(Ge, "Fieldset");
 x.register(X, "Field");
 x.register($e, "Object");
 x.register(Ve, "Section");
 x.register(Qe, "Group");
 x.register(Pt, "Statistics");
 x.register(et, "Image");
@@ -4898,15 +4930,15 @@
 x.register(at, "Progress");
 x.register(Ie, "Color");
 x.register(it, "Boxes");
 x.register(ct, "Indicators");
 x.register(ot, "Shell");
 x.register(lt, "FileLink");
 x.register(dt, "FilePreview");
-x.register(Le, "Response");
+x.register(Be, "Response");
 x.register(Vt, "Application");
 x.register(De, "IconSet");
 x.register(ut, "Grid");
 x.register(He, "Rows");
 x.register(Pe, "Cards");
 x.register(Ue, "Timeline");
 x.register(Ce, "Scheduler");
@@ -4914,39 +4946,39 @@
 x.register(Kt, "Text");
 x.register(Qt, "ZoomMeet");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    me[n] ? B("GET", A(e), function(a) {
+    me[n] ? q("GET", R(e), function(a) {
         ne.render(t.jsx(x, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), we ? (window.application = JSON.parse(we), B("GET", A(e), function(a) {
+    }, "", e), pe ? (window.application = JSON.parse(pe), q("GET", R(e), function(a) {
         window.application.content = a, ne.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
-    })) : B("GET", Zt, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", A(e), function(i) {
+    })) : q("GET", Zt, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", R(e), function(i) {
             window.application.content = i, ne.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), B("GET", A(e), function(n) {
+    }, "", e), q("GET", R(e), function(n) {
         window.loaddata(n), window.scrollTo({
             top: 0,
             behavior: "smooth"
         })
     })) : document.location.href = e
 };
 x.render(H.createRoot(document.getElementById("root")));
```

### Comparing `slthcore-0.0.4/slth/statistics.py` & `slthcore-0.0.5/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/templates/index.html` & `slthcore-0.0.5/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/templates/service-worker.js` & `slthcore-0.0.5/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/tests.py` & `slthcore-0.0.5/slth/tests.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/urls.py` & `slthcore-0.0.5/slth/urls.py`

 * *Files identical despite different names*

### Comparing `slthcore-0.0.4/slth/utils.py` & `slthcore-0.0.5/slth/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from django.conf import settings
+from django.template import Template, Context
+from django.template.engine import Engine
+
 
 def build_url(request, path=None):
     return path or request.path if request else ''
 
 def absolute_url(request, *querystrings):
     url = build_url(request)
     if url:
@@ -26,7 +28,11 @@
         if querystring:
             for param in querystring.split('&'):
                 k, v = param.split('=')
                 params[k] = v
     if params:
         url = '{}?{}'.format(url, '&'.join([f'{k}={v}' for k, v in params.items()]))
     return url
+
+
+def parse_string_template(template, **data):
+    return Template(template, engine=Engine()).render(Context(data))
```

### Comparing `slthcore-0.0.4/slth/views.py` & `slthcore-0.0.5/slth/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
+import json
 import sys
 import slth
 import socket
 import traceback
-from django.conf import settings
+
 from .models import Token
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .exceptions import JsonResponseException
 from .serializer import serialize
 from .utils import build_url
 from slth import APPLICATON
 from django.shortcuts import render
 from django.views.decorators.cache import never_cache, cache_control
 
+
 @cache_control(max_age=0, no_cache=True, no_store=True, must_revalidate=True)
 def index(request, path=None):
     vite = not socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect_ex(('127.0.0.1',5173))
     return render(request, 'index.html', dict(vite=vite, application=APPLICATON))
 
 def service_worker(request):
     return render(request, 'service-worker.js', content_type='text/javascript')
@@ -37,22 +39,29 @@
             url = build_url(request, cls.get_api_url())
             return ApiResponse(dict(type='redirect', url=url))
         else:
             cls = slth.ENDPOINTS.get(request.path.split('/')[2])
             if cls:
                 try:
                     endpoint = cls(*kwargs.values()).contextualize(request)
-                    if True or endpoint.check_permission():
+                    if endpoint.check_permission():
+                        endpoint.start_audit_trail()
                         return endpoint.to_response()
-                    return ApiResponse({}, status=403)
+                    else:
+                        url = '/api/login/'
+                        if request.path != '/api/dashboard/':
+                            url = '{}?next={}'.format(url, request.get_full_path())
+                        return ApiResponse(dict(type="redirect", url=url), status=403)
                 except JsonResponseException as e:
                     return ApiResponse(e.data, safe=False)
                 except Exception as e:
                     traceback.print_exc() 
                     return ApiResponse(data=dict(error=str(e)), safe=False, status=500)
+                finally:
+                    endpoint.start_audit_trail()
             else:
                 return ApiResponse({}, status=404)
 
 class ApiResponse(JsonResponse):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self["Access-Control-Allow-Origin"] = "*"
```

### Comparing `slthcore-0.0.4/slthcore.egg-info/PKG-INFO` & `slthcore-0.0.5/slthcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slthcore
-Version: 0.0.4
+Version: 0.0.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `slthcore-0.0.4/slthcore.egg-info/SOURCES.txt` & `slthcore-0.0.5/slthcore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 slth/notifications.py
 slth/oauth.py
 slth/permissions.py
 slth/queryset.py
 slth/roles.py
 slth/serializer.py
 slth/statistics.py
+slth/tasks.py
 slth/tests.py
+slth/threadlocal.py
 slth/urls.py
 slth/utils.py
 slth/views.py
+slth/cmd/configure/__main__.py
 slth/cmd/init/__main__.py
 slth/cmd/init/boilerplate/.DS_Store
 slth/cmd/init/boilerplate/.gitignore
 slth/cmd/init/boilerplate/base.env
 slth/cmd/init/boilerplate/docker-compose.yml
 slth/cmd/init/boilerplate/local.env
 slth/cmd/init/boilerplate/run.sh
@@ -39,25 +42,27 @@
 slth/cmd/init/boilerplate/backend/api/urls.py
 slth/cmd/init/boilerplate/backend/api/wsgi.py
 slth/cmd/init/boilerplate/frontend/package.json
 slth/cmd/init/boilerplate/frontend/vite.config.js
 slth/cmd/init/boilerplate/frontend/src/main.jsx
 slth/cmd/init/boilerplate/selenium/run.sh
 slth/db/__init__.py
+slth/db/generic.py
 slth/db/models.py
 slth/management/__init__.py
 slth/management/commands/__init__.py
 slth/management/commands/integration_test.py
 slth/management/commands/sync.py
 slth/migrations/0001_initial.py
 slth/migrations/0002_email_role_pushsubscription_error.py
 slth/migrations/0003_rename_photo_profile_alter_profile_options.py
 slth/migrations/0004_alter_profile_photo.py
 slth/migrations/0005_alter_profile_photo.py
 slth/migrations/0006_user.py
+slth/migrations/0007_deletion_log.py
 slth/migrations/__init__.py
 slth/selenium/__init__.py
 slth/selenium/browser.py
 slth/static/.DS_Store
 slth/static/css/.DS_Store
 slth/static/css/slth.css
 slth/static/js/index.min.js
```

