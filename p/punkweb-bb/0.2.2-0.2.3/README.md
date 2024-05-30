# Comparing `tmp/punkweb_bb-0.2.2.tar.gz` & `tmp/punkweb_bb-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.2.2.tar", last modified: Wed May 29 20:22:44 2024, max compression
+gzip compressed data, was "punkweb_bb-0.2.3.tar", last modified: Wed May 29 23:14:11 2024, max compression
```

## Comparing `punkweb_bb-0.2.2.tar` & `punkweb_bb-0.2.3.tar`

### file list

```diff
@@ -1,289 +1,290 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.2/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.2/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4441 2024-05-29 05:09:26.000000 punkweb_bb-0.2.2/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.2/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     4182 2024-05-29 19:50:24.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3531 2024-05-29 19:49:57.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    15235 2024-05-29 20:18:30.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 04:36:57.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2086 2024-05-29 20:11:36.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    25276 2024-05-29 01:17:40.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2821 2024-05-29 19:50:23.000000 punkweb_bb-0.2.2/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1372 2024-05-29 19:49:56.000000 punkweb_bb-0.2.2/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.2/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.2/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.2/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.2/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.2/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.2/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0003_alter_thread_options.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0004_groupstyle.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.2/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     6962 2024-05-29 20:18:29.000000 punkweb_bb-0.2.2/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.2/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.2/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.2/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 04:36:54.000000 punkweb_bb-0.2.2/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.2/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.388550 punkweb_bb-0.2.2/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/category-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1870 2024-05-29 20:15:36.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.388550 punkweb_bb-0.2.2/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10526 2024-05-29 20:04:35.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2804 2024-05-29 20:04:57.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3035 2024-05-29 20:06:01.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      759 2024-05-29 20:07:16.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     5842 2024-05-29 20:09:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10390 2024-05-29 20:13:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 20:12:20.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_delete.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_edit.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_post.py
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 20:12:14.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/styled_group_name.py
--rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/styled_username.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.2/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.2/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1223 2024-05-29 20:11:35.000000 punkweb_bb-0.2.2/punkweb_bb/utils.py
--rw-r--r--   0 pork      (1000) pork      (1000)    17400 2024-05-29 01:17:40.000000 punkweb_bb-0.2.2/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    14803 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 20:22:30.000000 punkweb_bb-0.2.2/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.724864 punkweb_bb-0.2.3/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.3/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.3/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4441 2024-05-29 05:09:26.000000 punkweb_bb-0.2.3/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.3/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     4182 2024-05-29 19:50:24.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3531 2024-05-29 19:49:57.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    15478 2024-05-29 22:03:33.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 21:18:38.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1591 2024-05-29 22:23:50.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/sitemap.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2057 2024-05-29 21:02:46.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    25244 2024-05-29 22:01:21.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2821 2024-05-29 19:50:23.000000 punkweb_bb-0.2.3/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1372 2024-05-29 19:49:56.000000 punkweb_bb-0.2.3/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.3/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.3/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.3/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.3/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.3/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.3/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0003_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0004_groupstyle.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.3/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     7072 2024-05-29 22:03:32.000000 punkweb_bb-0.2.3/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.3/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.3/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.3/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 21:18:30.000000 punkweb_bb-0.2.3/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.3/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.704864 punkweb_bb-0.2.3/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1686 2024-05-29 21:11:17.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10526 2024-05-29 20:04:35.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2886 2024-05-29 22:07:52.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3198 2024-05-29 22:08:57.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      802 2024-05-29 22:33:12.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5893 2024-05-29 22:09:31.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10838 2024-05-29 22:11:05.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 21:01:58.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 21:01:50.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/styled_group_name.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/styled_username.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.3/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.3/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1200 2024-05-29 21:02:45.000000 punkweb_bb-0.2.3/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    17383 2024-05-29 22:01:20.000000 punkweb_bb-0.2.3/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    14850 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 23:14:11.724864 punkweb_bb-0.2.3/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 23:13:37.000000 punkweb_bb-0.2.3/setup.py
```

### Comparing `punkweb_bb-0.2.2/LICENSE` & `punkweb_bb-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/PKG-INFO` & `punkweb_bb-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.2.2
+Version: 0.2.3
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `punkweb_bb-0.2.2/README.md` & `punkweb_bb-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,243 +1,239 @@
 magic:    0xa70d0d0a
-moddate:  0x958d5766 (Wed May 29 20:18:29 2024 UTC)
-files sz: 6962
+moddate:  0x34a65766 (Wed May 29 22:03:32 2024 UTC)
+files sz: 7072
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      026c036d045a040100640064036c056d065a060100640064046c076d085a
-      080100640064056c096d0a5a0a0100640064066c0b6d0c5a0c0100640064
-      076c0d6d0e5a0e0100640064086c0f6d105a100100640064096c116d125a
-      1201006400640a6c136d145a146d155a1501006400640b6c166d175a1701
-      0002006504a6000000ab0000000000000000005a18640c84005a19020047
-      00640d8400640e65156514a6040000ab0400000000000000005a1a020047
-      00640f8400641065156514a6040000ab0400000000000000005a1b020047
-      0064118400641265156514a6040000ab0400000000000000005a1c020047
-      0064138400641465156514a6040000ab0400000000000000005a1d020047
-      0064158400641665156514a6040000ab0400000000000000005a1e020047
-      0064178400641865156514a6040000ab0400000000000000005a1f020047
-      0064198400641a65156514a6040000ab0400000000000000005a20640153
-      00
+      0x9700640064016c005a00640064016c015a01640064026c026d035a0301
+      00640064036c046d055a050100640064046c066d075a070100640064056c
+      086d095a090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d01
+      00640064086c0e6d0f5a0f0100640064096c106d115a1101006400640a6c
+      126d135a136d145a1401006400640b6c156d165a166d175a170100020065
+      03a6000000ab0000000000000000005a18640c84005a1902004700640d84
+      00640e65146513a6040000ab0400000000000000005a1a02004700640f84
+      00641065146513a6040000ab0400000000000000005a1b02004700641184
+      00641265146513a6040000ab0400000000000000005a1c02004700641384
+      00641465146513a6040000ab0400000000000000005a1d02004700641584
+      00641665146513a6040000ab0400000000000000005a1e02004700641784
+      00641865146513a6040000ab0400000000000000005a1f02004700641984
+      00641a65146513a6040000ab0400000000000000005a2064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (datetime)
-                 8 STORE_NAME               0 (datetime)
+                 6 IMPORT_NAME              0 (math)
+                 8 STORE_NAME               0 (math)
    
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (math)
-                16 STORE_NAME               1 (math)
+                14 IMPORT_NAME              1 (os)
+                16 STORE_NAME               1 (os)
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              2 (os)
-                24 STORE_NAME               2 (os)
-   
-     5          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               2 (('get_user_model',))
-                30 IMPORT_NAME              3 (django.contrib.auth)
-                32 IMPORT_FROM              4 (get_user_model)
-                34 STORE_NAME               4 (get_user_model)
-                36 POP_TOP
-   
-     6          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('Group',))
-                42 IMPORT_NAME              5 (django.contrib.auth.models)
-                44 IMPORT_FROM              6 (Group)
-                46 STORE_NAME               6 (Group)
-                48 POP_TOP
-   
-     7          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('cache',))
-                54 IMPORT_NAME              7 (django.core.cache)
-                56 IMPORT_FROM              8 (cache)
-                58 STORE_NAME               8 (cache)
-                60 POP_TOP
-   
-     8          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('models',))
-                66 IMPORT_NAME              9 (django.db)
-                68 IMPORT_FROM             10 (models)
-                70 STORE_NAME              10 (models)
-                72 POP_TOP
-   
-     9          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('ValidationError',))
-                78 IMPORT_NAME             11 (django.forms)
-                80 IMPORT_FROM             12 (ValidationError)
-                82 STORE_NAME              12 (ValidationError)
-                84 POP_TOP
-   
-    10          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('reverse',))
-                90 IMPORT_NAME             13 (django.urls)
-                92 IMPORT_FROM             14 (reverse)
-                94 STORE_NAME              14 (reverse)
-                96 POP_TOP
-   
-    11          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('timezone',))
-               102 IMPORT_NAME             15 (django.utils)
-               104 IMPORT_FROM             16 (timezone)
-               106 STORE_NAME              16 (timezone)
-               108 POP_TOP
-   
-    12         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('BBCodeTextField',))
-               114 IMPORT_NAME             17 (precise_bbcode.fields)
-               116 IMPORT_FROM             18 (BBCodeTextField)
-               118 STORE_NAME              18 (BBCodeTextField)
-               120 POP_TOP
-   
-    14         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST              10 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
-               126 IMPORT_NAME             19 (punkweb_bb.mixins)
-               128 IMPORT_FROM             20 (TimestampMixin)
-               130 STORE_NAME              20 (TimestampMixin)
-               132 IMPORT_FROM             21 (UUIDPrimaryKeyMixin)
-               134 STORE_NAME              21 (UUIDPrimaryKeyMixin)
-               136 POP_TOP
-   
-    15         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              11 (('get_styled_username',))
-               142 IMPORT_NAME             22 (punkweb_bb.utils)
-               144 IMPORT_FROM             23 (get_styled_username)
-               146 STORE_NAME              23 (get_styled_username)
-               148 POP_TOP
-   
-    17         150 PUSH_NULL
-               152 LOAD_NAME                4 (get_user_model)
-               154 PRECALL                  0
-               158 CALL                     0
-               168 STORE_NAME              24 (User)
-   
-    20         170 LOAD_CONST              12 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 20>)
-               172 MAKE_FUNCTION            0
-               174 STORE_NAME              25 (profile_image_upload_to)
-   
-    25         176 PUSH_NULL
-               178 LOAD_BUILD_CLASS
-               180 LOAD_CONST              13 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 25>)
-               182 MAKE_FUNCTION            0
-               184 LOAD_CONST              14 ('BoardProfile')
-               186 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               188 LOAD_NAME               20 (TimestampMixin)
-               190 PRECALL                  4
-               194 CALL                     4
-               204 STORE_NAME              26 (BoardProfile)
-   
-    52         206 PUSH_NULL
-               208 LOAD_BUILD_CLASS
-               210 LOAD_CONST              15 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 52>)
-               212 MAKE_FUNCTION            0
-               214 LOAD_CONST              16 ('Category')
-               216 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               218 LOAD_NAME               20 (TimestampMixin)
-               220 PRECALL                  4
-               224 CALL                     4
-               234 STORE_NAME              27 (Category)
-   
-    70         236 PUSH_NULL
-               238 LOAD_BUILD_CLASS
-               240 LOAD_CONST              17 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 70>)
-               242 MAKE_FUNCTION            0
-               244 LOAD_CONST              18 ('Subcategory')
-               246 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               248 LOAD_NAME               20 (TimestampMixin)
-               250 PRECALL                  4
-               254 CALL                     4
-               264 STORE_NAME              28 (Subcategory)
-   
-   110         266 PUSH_NULL
-               268 LOAD_BUILD_CLASS
-               270 LOAD_CONST              19 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 110>)
-               272 MAKE_FUNCTION            0
-               274 LOAD_CONST              20 ('Thread')
-               276 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               278 LOAD_NAME               20 (TimestampMixin)
-               280 PRECALL                  4
-               284 CALL                     4
-               294 STORE_NAME              29 (Thread)
-   
-   157         296 PUSH_NULL
-               298 LOAD_BUILD_CLASS
-               300 LOAD_CONST              21 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 157>)
-               302 MAKE_FUNCTION            0
-               304 LOAD_CONST              22 ('Post')
-               306 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               308 LOAD_NAME               20 (TimestampMixin)
-               310 PRECALL                  4
-               314 CALL                     4
-               324 STORE_NAME              30 (Post)
-   
-   202         326 PUSH_NULL
-               328 LOAD_BUILD_CLASS
-               330 LOAD_CONST              23 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 202>)
-               332 MAKE_FUNCTION            0
-               334 LOAD_CONST              24 ('Shout')
-               336 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               338 LOAD_NAME               20 (TimestampMixin)
-               340 PRECALL                  4
-               344 CALL                     4
-               354 STORE_NAME              31 (Shout)
-   
-   216         356 PUSH_NULL
-               358 LOAD_BUILD_CLASS
-               360 LOAD_CONST              25 (<code object GroupStyle, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 216>)
-               362 MAKE_FUNCTION            0
-               364 LOAD_CONST              26 ('GroupStyle')
-               366 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
-               368 LOAD_NAME               20 (TimestampMixin)
-               370 PRECALL                  4
-               374 CALL                     4
-               384 STORE_NAME              32 (GroupStyle)
-               386 LOAD_CONST               1 (None)
-               388 RETURN_VALUE
+     4          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('get_user_model',))
+                22 IMPORT_NAME              2 (django.contrib.auth)
+                24 IMPORT_FROM              3 (get_user_model)
+                26 STORE_NAME               3 (get_user_model)
+                28 POP_TOP
+   
+     5          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('Group',))
+                34 IMPORT_NAME              4 (django.contrib.auth.models)
+                36 IMPORT_FROM              5 (Group)
+                38 STORE_NAME               5 (Group)
+                40 POP_TOP
+   
+     6          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('cache',))
+                46 IMPORT_NAME              6 (django.core.cache)
+                48 IMPORT_FROM              7 (cache)
+                50 STORE_NAME               7 (cache)
+                52 POP_TOP
+   
+     7          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('models',))
+                58 IMPORT_NAME              8 (django.db)
+                60 IMPORT_FROM              9 (models)
+                62 STORE_NAME               9 (models)
+                64 POP_TOP
+   
+     8          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               6 (('ValidationError',))
+                70 IMPORT_NAME             10 (django.forms)
+                72 IMPORT_FROM             11 (ValidationError)
+                74 STORE_NAME              11 (ValidationError)
+                76 POP_TOP
+   
+     9          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               7 (('reverse',))
+                82 IMPORT_NAME             12 (django.urls)
+                84 IMPORT_FROM             13 (reverse)
+                86 STORE_NAME              13 (reverse)
+                88 POP_TOP
+   
+    10          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               8 (('timezone',))
+                94 IMPORT_NAME             14 (django.utils)
+                96 IMPORT_FROM             15 (timezone)
+                98 STORE_NAME              15 (timezone)
+               100 POP_TOP
+   
+    11         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               9 (('BBCodeTextField',))
+               106 IMPORT_NAME             16 (precise_bbcode.fields)
+               108 IMPORT_FROM             17 (BBCodeTextField)
+               110 STORE_NAME              17 (BBCodeTextField)
+               112 POP_TOP
+   
+    13         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST              10 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
+               118 IMPORT_NAME             18 (punkweb_bb.mixins)
+               120 IMPORT_FROM             19 (TimestampMixin)
+               122 STORE_NAME              19 (TimestampMixin)
+               124 IMPORT_FROM             20 (UUIDPrimaryKeyMixin)
+               126 STORE_NAME              20 (UUIDPrimaryKeyMixin)
+               128 POP_TOP
+   
+    14         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              11 (('get_highest_priority_group', 'get_styled_username'))
+               134 IMPORT_NAME             21 (punkweb_bb.utils)
+               136 IMPORT_FROM             22 (get_highest_priority_group)
+               138 STORE_NAME              22 (get_highest_priority_group)
+               140 IMPORT_FROM             23 (get_styled_username)
+               142 STORE_NAME              23 (get_styled_username)
+               144 POP_TOP
+   
+    16         146 PUSH_NULL
+               148 LOAD_NAME                3 (get_user_model)
+               150 PRECALL                  0
+               154 CALL                     0
+               164 STORE_NAME              24 (User)
+   
+    19         166 LOAD_CONST              12 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 19>)
+               168 MAKE_FUNCTION            0
+               170 STORE_NAME              25 (profile_image_upload_to)
+   
+    24         172 PUSH_NULL
+               174 LOAD_BUILD_CLASS
+               176 LOAD_CONST              13 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 24>)
+               178 MAKE_FUNCTION            0
+               180 LOAD_CONST              14 ('BoardProfile')
+               182 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               184 LOAD_NAME               19 (TimestampMixin)
+               186 PRECALL                  4
+               190 CALL                     4
+               200 STORE_NAME              26 (BoardProfile)
+   
+    55         202 PUSH_NULL
+               204 LOAD_BUILD_CLASS
+               206 LOAD_CONST              15 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 55>)
+               208 MAKE_FUNCTION            0
+               210 LOAD_CONST              16 ('Category')
+               212 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               214 LOAD_NAME               19 (TimestampMixin)
+               216 PRECALL                  4
+               220 CALL                     4
+               230 STORE_NAME              27 (Category)
+   
+    73         232 PUSH_NULL
+               234 LOAD_BUILD_CLASS
+               236 LOAD_CONST              17 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 73>)
+               238 MAKE_FUNCTION            0
+               240 LOAD_CONST              18 ('Subcategory')
+               242 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               244 LOAD_NAME               19 (TimestampMixin)
+               246 PRECALL                  4
+               250 CALL                     4
+               260 STORE_NAME              28 (Subcategory)
+   
+   113         262 PUSH_NULL
+               264 LOAD_BUILD_CLASS
+               266 LOAD_CONST              19 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 113>)
+               268 MAKE_FUNCTION            0
+               270 LOAD_CONST              20 ('Thread')
+               272 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               274 LOAD_NAME               19 (TimestampMixin)
+               276 PRECALL                  4
+               280 CALL                     4
+               290 STORE_NAME              29 (Thread)
+   
+   160         292 PUSH_NULL
+               294 LOAD_BUILD_CLASS
+               296 LOAD_CONST              21 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 160>)
+               298 MAKE_FUNCTION            0
+               300 LOAD_CONST              22 ('Post')
+               302 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               304 LOAD_NAME               19 (TimestampMixin)
+               306 PRECALL                  4
+               310 CALL                     4
+               320 STORE_NAME              30 (Post)
+   
+   205         322 PUSH_NULL
+               324 LOAD_BUILD_CLASS
+               326 LOAD_CONST              23 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 205>)
+               328 MAKE_FUNCTION            0
+               330 LOAD_CONST              24 ('Shout')
+               332 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               334 LOAD_NAME               19 (TimestampMixin)
+               336 PRECALL                  4
+               340 CALL                     4
+               350 STORE_NAME              31 (Shout)
+   
+   219         352 PUSH_NULL
+               354 LOAD_BUILD_CLASS
+               356 LOAD_CONST              25 (<code object GroupStyle, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 219>)
+               358 MAKE_FUNCTION            0
+               360 LOAD_CONST              26 ('GroupStyle')
+               362 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
+               364 LOAD_NAME               19 (TimestampMixin)
+               366 PRECALL                  4
+               370 CALL                     4
+               380 STORE_NAME              32 (GroupStyle)
+               382 LOAD_CONST               1 (None)
+               384 RETURN_VALUE
    consts
       0
       None
       ('get_user_model',)
       ('Group',)
       ('cache',)
       ('models',)
       ('ValidationError',)
       ('reverse',)
       ('timezone',)
       ('BBCodeTextField',)
       ('TimestampMixin', 'UUIDPrimaryKeyMixin')
-      ('get_styled_username',)
+      ('get_highest_priority_group', 'get_styled_username')
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c01a6010000ab010000000000
             0000006401190000000000000000007d0264027c006a0300000000000000
             006a0400000000000000009b0064037c029b009d045300
-          20           0 RESUME                   0
+          19           0 RESUME                   0
          
-          21           2 LOAD_GLOBAL              0 (os)
+          20           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (splitext)
                       46 LOAD_FAST                1 (filename)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_CONST               1 (-1)
                       64 BINARY_SUBSCR
                       74 STORE_FAST               2 (ext)
          
-          22          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
+          21          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
                       78 LOAD_FAST                0 (instance)
                       80 LOAD_ATTR                3 (user)
                       90 LOAD_ATTR                4 (username)
                      100 FORMAT_VALUE             0
                      102 LOAD_CONST               3 ('/image')
                      104 LOAD_FAST                2 (ext)
                      106 FORMAT_VALUE             0
@@ -250,249 +246,286 @@
             '/image'
          names      ('os', 'path', 'splitext', 'user', 'username')
          varnames   ('instance', 'filename', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'profile_image_upload_to'
-         firstlineno 20
+         firstlineno 19
          lnotab 0x02014a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000650964036403ac04a6030000ab03000000
             00000000005a0a0200650b640564036403ac06a6030000ab030000000000
             0000005a0c02004700640784006408a6020000ab0200000000000000005a
             0d650e64098400a6000000ab0000000000000000005a0f650e640a8400a6
             000000ab0000000000000000005a10650e640b8400a6000000ab00000000
-            00000000005a11640c84005a12640d5300
-          25           0 RESUME                   0
+            00000000005a11650e640c8400a6000000ab0000000000000000005a1264
+            0d84005a13640e5300
+          24           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfile')
                        8 STORE_NAME               2 (__qualname__)
          
-          26          10 PUSH_NULL
+          25          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (OneToOneField)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('profile')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-          27          58 PUSH_NULL
+          26          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (ImageField)
                       72 LOAD_NAME                9 (profile_image_upload_to)
                       74 LOAD_CONST               3 (True)
                       76 LOAD_CONST               3 (True)
                       78 KW_NAMES                 4
                       80 PRECALL                  3
                       84 CALL                     3
                       94 STORE_NAME              10 (image)
          
-          28          96 PUSH_NULL
+          27          96 PUSH_NULL
                       98 LOAD_NAME               11 (BBCodeTextField)
                      100 LOAD_CONST               5 (1024)
                      102 LOAD_CONST               3 (True)
                      104 LOAD_CONST               3 (True)
                      106 KW_NAMES                 6
                      108 PRECALL                  3
                      112 CALL                     3
                      122 STORE_NAME              12 (signature)
          
-          30         124 PUSH_NULL
+          29         124 PUSH_NULL
                      126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 30>)
+                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 29>)
                      130 MAKE_FUNCTION            0
                      132 LOAD_CONST               8 ('Meta')
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_NAME              13 (Meta)
          
-          33         150 LOAD_NAME               14 (property)
+          32         150 LOAD_NAME               14 (property)
          
-          34         152 LOAD_CONST               9 (<code object styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 33>)
+          33         152 LOAD_CONST               9 (<code object priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 32>)
                      154 MAKE_FUNCTION            0
          
-          33         156 PRECALL                  0
+          32         156 PRECALL                  0
                      160 CALL                     0
          
-          34         170 STORE_NAME              15 (styled_username)
+          33         170 STORE_NAME              15 (priority_group)
          
-          37         172 LOAD_NAME               14 (property)
+          36         172 LOAD_NAME               14 (property)
          
-          38         174 LOAD_CONST              10 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 37>)
+          37         174 LOAD_CONST              10 (<code object styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 36>)
                      176 MAKE_FUNCTION            0
          
-          37         178 PRECALL                  0
+          36         178 PRECALL                  0
                      182 CALL                     0
          
-          38         192 STORE_NAME              16 (is_online)
+          37         192 STORE_NAME              16 (styled_username)
          
-          44         194 LOAD_NAME               14 (property)
+          40         194 LOAD_NAME               14 (property)
          
-          45         196 LOAD_CONST              11 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 44>)
+          41         196 LOAD_CONST              11 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 40>)
                      198 MAKE_FUNCTION            0
          
-          44         200 PRECALL                  0
+          40         200 PRECALL                  0
                      204 CALL                     0
          
-          45         214 STORE_NAME              17 (post_count)
+          41         214 STORE_NAME              17 (is_online)
          
-          48         216 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 48>)
-                     218 MAKE_FUNCTION            0
-                     220 STORE_NAME              18 (__str__)
-                     222 LOAD_CONST              13 (None)
-                     224 RETURN_VALUE
+          47         216 LOAD_NAME               14 (property)
+         
+          48         218 LOAD_CONST              12 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 47>)
+                     220 MAKE_FUNCTION            0
+         
+          47         222 PRECALL                  0
+                     226 CALL                     0
+         
+          48         236 STORE_NAME              18 (post_count)
+         
+          51         238 LOAD_CONST              13 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 51>)
+                     240 MAKE_FUNCTION            0
+                     242 STORE_NAME              19 (__str__)
+                     244 LOAD_CONST              14 (None)
+                     246 RETURN_VALUE
          consts
             'BoardProfile'
             'profile'
             ('related_name', 'on_delete')
             True
             ('upload_to', 'blank', 'null')
             1024
             ('max_length', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                30           0 RESUME                   0
+                29           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfile.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                31          10 LOAD_CONST               1 (('user__username',))
+                30          10 LOAD_CONST               1 (('user__username',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'BoardProfile.Meta'
                   ('user__username',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 30
+               firstlineno 29
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                33           0 RESUME                   0
+                32           0 RESUME                   0
                
-                35           2 LOAD_GLOBAL              1 (NULL + get_styled_username)
+                34           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (user)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 RETURN_VALUE
+               consts
+                  None
+               names      ('get_highest_priority_group', 'user')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'priority_group'
+               firstlineno 32
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab0100000000000000005300
+                36           0 RESUME                   0
+               
+                38           2 LOAD_GLOBAL              1 (NULL + get_styled_username)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (user)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('get_styled_username', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'styled_username'
-               firstlineno 33
+               firstlineno 36
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c006a
                   0200000000000000009b009d02a6010000ab0100000000000000007d017c
                   01722d7407000000000000000000006a040000000000000000a6000000ab
-                  0000000000000000007c01740b000000000000000000006a060000000000
+                  0000000000000000007c017407000000000000000000006a050000000000
                   0000006402ac03a6010000ab0100000000000000007a0000006b00000000
                   00530064045300
-                37           0 RESUME                   0
+                40           0 RESUME                   0
                
-                39           2 LOAD_GLOBAL              1 (NULL + cache)
+                42           2 LOAD_GLOBAL              1 (NULL + cache)
                             14 LOAD_ATTR                1 (get)
                             24 LOAD_CONST               1 ('profile_online_')
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (id)
                             38 FORMAT_VALUE             0
                             40 BUILD_STRING             2
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               1 (last_seen)
                
-                40          58 LOAD_FAST                1 (last_seen)
+                43          58 LOAD_FAST                1 (last_seen)
                             60 POP_JUMP_FORWARD_IF_FALSE    45 (to 152)
                
-                41          62 LOAD_GLOBAL              7 (NULL + timezone)
+                44          62 LOAD_GLOBAL              7 (NULL + timezone)
                             74 LOAD_ATTR                4 (now)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 LOAD_FAST                1 (last_seen)
-                           100 LOAD_GLOBAL             11 (NULL + datetime)
-                           112 LOAD_ATTR                6 (timedelta)
+                           100 LOAD_GLOBAL              7 (NULL + timezone)
+                           112 LOAD_ATTR                5 (timedelta)
                            122 LOAD_CONST               2 (5)
                            124 KW_NAMES                 3
                            126 PRECALL                  1
                            130 CALL                     1
                            140 BINARY_OP                0 (+)
                            144 COMPARE_OP               0 (<)
                            150 RETURN_VALUE
                
-                42     >>  152 LOAD_CONST               4 (False)
+                45     >>  152 LOAD_CONST               4 (False)
                            154 RETURN_VALUE
                consts
                   None
                   'profile_online_'
                   5
                   ('minutes',)
                   False
-               names      ('cache', 'get', 'id', 'timezone', 'now', 'datetime', 'timedelta')
+               names      ('cache', 'get', 'id', 'timezone', 'now', 'timedelta')
                varnames   ('self', 'last_seen')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'is_online'
-               firstlineno 37
+               firstlineno 40
                lnotab 0x0202380104015a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   007c006a0000000000000000006a030000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab0000000000000000007a
                   0000005300
-                44           0 RESUME                   0
+                47           0 RESUME                   0
                
-                46           2 LOAD_FAST                0 (self)
+                49           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (threads)
                             24 LOAD_METHOD              2 (count)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                0 (user)
@@ -506,110 +539,110 @@
                   None
                names      ('user', 'threads', 'count', 'posts')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 44
+               firstlineno 47
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                48           0 RESUME                   0
+                51           0 RESUME                   0
                
-                49           2 LOAD_FAST                0 (self)
+                52           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (username)
                             24 RETURN_VALUE
                consts
                   None
                names      ('user', 'username')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 48
+               firstlineno 51
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'styled_username', 'is_online', 'post_count', '__str__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'priority_group', 'styled_username', 'is_online', 'post_count', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'BoardProfile'
-         firstlineno 25
+         firstlineno 24
          lnotab
-            0x0a01300126011c021a03020104ff0e010203020104ff0e010206020104
-            ff0e010203
+            0x0a01300126011c021a03020104ff0e010203020104ff0e010203020104
+            ff0e010206020104ff0e010203
       'BoardProfile'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006401ac02a6
             010000ab0100000000000000005a05020065036a06000000000000000064
             036404ac05a6020000ab0200000000000000005a07020065036a08000000
             00000000006406ac07a6010000ab0100000000000000005a090200470064
             0884006409a6020000ab0200000000000000005a0a640a84005a0b640b84
             005a0c640c5300
-          52           0 RESUME                   0
+          55           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Category')
                        8 STORE_NAME               2 (__qualname__)
          
-          53          10 PUSH_NULL
+          56          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (255)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (name)
          
-          54          44 PUSH_NULL
+          57          44 PUSH_NULL
                       46 LOAD_NAME                3 (models)
                       48 LOAD_ATTR                6 (SlugField)
                       58 LOAD_CONST               3 (1024)
                       60 LOAD_CONST               4 (True)
                       62 KW_NAMES                 5
                       64 PRECALL                  2
                       68 CALL                     2
                       78 STORE_NAME               7 (slug)
          
-          55          80 PUSH_NULL
+          58          80 PUSH_NULL
                       82 LOAD_NAME                3 (models)
                       84 LOAD_ATTR                8 (PositiveIntegerField)
                       94 LOAD_CONST               6 (0)
                       96 KW_NAMES                 7
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_NAME               9 (order)
          
-          57         114 PUSH_NULL
+          60         114 PUSH_NULL
                      116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 57>)
+                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 60>)
                      120 MAKE_FUNCTION            0
                      122 LOAD_CONST               9 ('Meta')
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_NAME              10 (Meta)
          
-          62         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 62>)
+          65         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 65>)
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              11 (__str__)
          
-          65         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 65>)
+          68         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 68>)
                      148 MAKE_FUNCTION            0
                      150 STORE_NAME              12 (get_absolute_url)
                      152 LOAD_CONST              12 (None)
                      154 RETURN_VALUE
          consts
             'Category'
             255
@@ -621,27 +654,27 @@
             ('default',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                57           0 RESUME                   0
+                60           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Category.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                58          10 LOAD_CONST               1 ('category')
+                61          10 LOAD_CONST               1 ('category')
                             12 STORE_NAME               3 (verbose_name)
                
-                59          14 LOAD_CONST               2 ('categories')
+                62          14 LOAD_CONST               2 ('categories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                60          18 LOAD_CONST               3 (('order',))
+                63          18 LOAD_CONST               3 (('order',))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Category.Meta'
                   'category'
                   'categories'
@@ -649,28 +682,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 57
+               firstlineno 60
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-                62           0 RESUME                   0
+                65           0 RESUME                   0
                
-                63           2 LOAD_FAST                0 (self)
+                66           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (order)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('. ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (name)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -680,34 +713,34 @@
                   '. '
                names      ('order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 62
+               firstlineno 65
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   007d017c019b0064027c006a0100000000000000009b0064037c006a0200
                   000000000000009b009d055300
-                65           0 RESUME                   0
+                68           0 RESUME                   0
                
-                66           2 LOAD_GLOBAL              1 (NULL + reverse)
+                69           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:index')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               1 (index_url)
                
-                67          32 LOAD_FAST                1 (index_url)
+                70          32 LOAD_FAST                1 (index_url)
                             34 FORMAT_VALUE             0
                             36 LOAD_CONST               2 ('#')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                1 (slug)
                             50 FORMAT_VALUE             0
                             52 LOAD_CONST               3 ('.')
                             54 LOAD_FAST                0 (self)
@@ -722,24 +755,24 @@
                   '.'
                names      ('reverse', 'slug', 'order')
                varnames   ('self', 'index_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 65
+               firstlineno 68
                lnotab 0x02011e01
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'SlugField', 'slug', 'PositiveIntegerField', 'order', 'Meta', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Category'
-         firstlineno 52
+         firstlineno 55
          lnotab 0x0a012201240122021a050603
       'Category'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -752,128 +785,128 @@
             0000005a0d020065036a0e00000000000000006409ac0aa6010000ab0100
             000000000000005a0f020065036a100000000000000000640bac0aa60100
             00ab0100000000000000005a1102004700640c8400640da6020000ab0200
             000000000000005a12640e84005a136514640f8400a6000000ab00000000
             00000000005a15651464108400a6000000ab0000000000000000005a1665
             1464118400a6000000ab0000000000000000005a17641284005a18641384
             005a1964145300
-          70           0 RESUME                   0
+          73           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Subcategory')
                        8 STORE_NAME               2 (__qualname__)
          
-          71          10 PUSH_NULL
+          74          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-          72          24 LOAD_NAME                5 (Category)
+          75          24 LOAD_NAME                5 (Category)
                       26 LOAD_CONST               1 ('subcategories')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-          71          40 KW_NAMES                 2
+          74          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (category)
          
-          74          58 PUSH_NULL
+          77          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (CharField)
                       72 LOAD_CONST               3 (255)
                       74 KW_NAMES                 4
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_NAME               9 (name)
          
-          75          92 PUSH_NULL
+          78          92 PUSH_NULL
                       94 LOAD_NAME                3 (models)
                       96 LOAD_ATTR               10 (SlugField)
                      106 LOAD_CONST               5 (1024)
                      108 LOAD_CONST               6 (True)
                      110 KW_NAMES                 7
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_NAME              11 (slug)
          
-          76         128 PUSH_NULL
+          79         128 PUSH_NULL
                      130 LOAD_NAME               12 (BBCodeTextField)
                      132 LOAD_CONST               6 (True)
                      134 LOAD_CONST               6 (True)
                      136 KW_NAMES                 8
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              13 (description)
          
-          77         154 PUSH_NULL
+          80         154 PUSH_NULL
                      156 LOAD_NAME                3 (models)
                      158 LOAD_ATTR               14 (PositiveIntegerField)
                      168 LOAD_CONST               9 (0)
                      170 KW_NAMES                10
                      172 PRECALL                  1
                      176 CALL                     1
                      186 STORE_NAME              15 (order)
          
-          78         188 PUSH_NULL
+          81         188 PUSH_NULL
                      190 LOAD_NAME                3 (models)
                      192 LOAD_ATTR               16 (BooleanField)
                      202 LOAD_CONST              11 (False)
                      204 KW_NAMES                10
                      206 PRECALL                  1
                      210 CALL                     1
                      220 STORE_NAME              17 (staff_post_only)
          
-          80         222 PUSH_NULL
+          83         222 PUSH_NULL
                      224 LOAD_BUILD_CLASS
-                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 80>)
+                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 83>)
                      228 MAKE_FUNCTION            0
                      230 LOAD_CONST              13 ('Meta')
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_NAME              18 (Meta)
          
-          88         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 88>)
+          91         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
                      250 MAKE_FUNCTION            0
                      252 STORE_NAME              19 (can_post)
          
-          91         254 LOAD_NAME               20 (property)
+          94         254 LOAD_NAME               20 (property)
          
-          92         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
+          95         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 94>)
                      258 MAKE_FUNCTION            0
          
-          91         260 PRECALL                  0
+          94         260 PRECALL                  0
                      264 CALL                     0
          
-          92         274 STORE_NAME              21 (thread_count)
+          95         274 STORE_NAME              21 (thread_count)
          
-          95         276 LOAD_NAME               20 (property)
+          98         276 LOAD_NAME               20 (property)
          
-          96         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 95>)
+          99         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 98>)
                      280 MAKE_FUNCTION            0
          
-          95         282 PRECALL                  0
+          98         282 PRECALL                  0
                      286 CALL                     0
          
-          96         296 STORE_NAME              22 (post_count)
+          99         296 STORE_NAME              22 (post_count)
          
-          99         298 LOAD_NAME               20 (property)
+         102         298 LOAD_NAME               20 (property)
          
-         100         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 99>)
+         103         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 102>)
                      302 MAKE_FUNCTION            0
          
-          99         304 PRECALL                  0
+         102         304 PRECALL                  0
                      308 CALL                     0
          
-         100         318 STORE_NAME              23 (latest_thread)
+         103         318 STORE_NAME              23 (latest_thread)
          
-         103         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 103>)
+         106         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 106>)
                      322 MAKE_FUNCTION            0
                      324 STORE_NAME              24 (__str__)
          
-         106         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 106>)
+         109         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 109>)
                      328 MAKE_FUNCTION            0
                      330 STORE_NAME              25 (get_absolute_url)
                      332 LOAD_CONST              20 (None)
                      334 RETURN_VALUE
          consts
             'Subcategory'
             'subcategories'
@@ -889,27 +922,27 @@
             False
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                80           0 RESUME                   0
+                83           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Subcategory.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                81          10 LOAD_CONST               1 ('subcategory')
+                84          10 LOAD_CONST               1 ('subcategory')
                             12 STORE_NAME               3 (verbose_name)
                
-                82          14 LOAD_CONST               2 ('subcategories')
+                85          14 LOAD_CONST               2 ('subcategories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                83          18 LOAD_CONST               3 (('category__order', 'order'))
+                86          18 LOAD_CONST               3 (('category__order', 'order'))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Subcategory.Meta'
                   'subcategory'
                   'subcategories'
@@ -917,84 +950,84 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 80
+               firstlineno 83
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code
                   0x97007c006a0000000000000000000c0070067c016a0100000000000000
                   005300
-                88           0 RESUME                   0
+                91           0 RESUME                   0
                
-                89           2 LOAD_FAST                0 (self)
+                92           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (staff_post_only)
                             14 UNARY_NOT
                             16 JUMP_IF_TRUE_OR_POP      6 (to 30)
                             18 LOAD_FAST                1 (user)
                             20 LOAD_ATTR                1 (is_staff)
                        >>   30 RETURN_VALUE
                consts
                   None
                names      ('staff_post_only', 'is_staff')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_post'
-               firstlineno 88
+               firstlineno 91
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-                91           0 RESUME                   0
+                94           0 RESUME                   0
                
-                93           2 LOAD_FAST                0 (self)
+                96           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('threads', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'thread_count'
-               firstlineno 91
+               firstlineno 94
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000005300
-                95           0 RESUME                   0
+                98           0 RESUME                   0
                
-                97           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
+               100           2 LOAD_GLOBAL              1 (NULL + sum)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 100>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (threads)
                             30 LOAD_METHOD              2 (all)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
@@ -1007,15 +1040,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                      97           0 RESUME                   0
+                     100           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (thread)
                                   10 LOAD_FAST                1 (thread)
                                   12 LOAD_ATTR                0 (post_count)
                                   22 LIST_APPEND              2
@@ -1024,37 +1057,37 @@
                      consts
                      names      ('post_count',)
                      varnames   ('.0', 'thread')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                      name       '<listcomp>'
-                     firstlineno 97
+                     firstlineno 100
                      lnotab 0x
                names      ('sum', 'threads', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 95
+               firstlineno 98
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-                99           0 RESUME                   0
+               102           0 RESUME                   0
                
-               101           2 LOAD_FAST                0 (self)
+               104           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-last_post_created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1065,27 +1098,27 @@
                   '-last_post_created_at'
                names      ('threads', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_thread'
-               firstlineno 99
+               firstlineno 102
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064027c006a0200000000000000009b009d055300
-               103           0 RESUME                   0
+               106           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               107           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (category)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (order)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               2 ('. ')
@@ -1100,27 +1133,27 @@
                   '. '
                names      ('category', 'order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 103
+               firstlineno 106
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               106           0 RESUME                   0
+               109           0 RESUME                   0
                
-               107           2 LOAD_GLOBAL              1 (NULL + reverse)
+               110           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:subcategory')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (slug)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1131,24 +1164,24 @@
                   ('args',)
                names      ('reverse', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 106
+               firstlineno 109
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'can_post', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Subcategory'
-         firstlineno 70
+         firstlineno 73
          lnotab
             0x0a010e0110ff1203220124011a01220122021a080603020104ff0e0102
             03020104ff0e010203020104ff0e0102030603
       'Subcategory'
       code
          argcount  : 0
          nlocals   : 0
@@ -1165,143 +1198,143 @@
             05ac06a6010000ab0100000000000000005a10020065036a110000000000
             0000006407ac08a6010000ab0100000000000000005a12020065036a1300
             000000000000006409ac06a6010000ab0100000000000000005a14020047
             00640a8400640ba6020000ab0200000000000000005a15640c84005a1664
             0d84005a17640e84005a18640f84005a19651a64108400a6000000ab0000
             000000000000005a1b651a64118400a6000000ab0000000000000000005a
             1c641284005a1d64135300
-         110           0 RESUME                   0
+         113           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Thread')
                        8 STORE_NAME               2 (__qualname__)
          
-         111          10 PUSH_NULL
+         114          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         112          24 LOAD_NAME                5 (Subcategory)
+         115          24 LOAD_NAME                5 (Subcategory)
                       26 LOAD_CONST               1 ('threads')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-         111          40 KW_NAMES                 2
+         114          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (subcategory)
          
-         114          58 PUSH_NULL
+         117          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                4 (ForeignKey)
                       72 LOAD_NAME                8 (User)
                       74 LOAD_CONST               1 ('threads')
                       76 LOAD_NAME                3 (models)
                       78 LOAD_ATTR                6 (CASCADE)
                       88 KW_NAMES                 2
                       90 PRECALL                  3
                       94 CALL                     3
                      104 STORE_NAME               9 (user)
          
-         115         106 PUSH_NULL
+         118         106 PUSH_NULL
                      108 LOAD_NAME                3 (models)
                      110 LOAD_ATTR               10 (CharField)
                      120 LOAD_CONST               3 (255)
                      122 KW_NAMES                 4
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_NAME              11 (title)
          
-         116         140 PUSH_NULL
+         119         140 PUSH_NULL
                      142 LOAD_NAME               12 (BBCodeTextField)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 STORE_NAME              13 (content)
          
-         117         160 PUSH_NULL
+         120         160 PUSH_NULL
                      162 LOAD_NAME                3 (models)
                      164 LOAD_ATTR               14 (BooleanField)
                      174 LOAD_CONST               5 (False)
                      176 KW_NAMES                 6
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_NAME              15 (is_pinned)
          
-         118         194 PUSH_NULL
+         121         194 PUSH_NULL
                      196 LOAD_NAME                3 (models)
                      198 LOAD_ATTR               14 (BooleanField)
                      208 LOAD_CONST               5 (False)
                      210 KW_NAMES                 6
                      212 PRECALL                  1
                      216 CALL                     1
                      226 STORE_NAME              16 (is_closed)
          
-         119         228 PUSH_NULL
+         122         228 PUSH_NULL
                      230 LOAD_NAME                3 (models)
                      232 LOAD_ATTR               17 (DateTimeField)
                      242 LOAD_CONST               7 (True)
                      244 KW_NAMES                 8
                      246 PRECALL                  1
                      250 CALL                     1
                      260 STORE_NAME              18 (last_post_created_at)
          
-         120         262 PUSH_NULL
+         123         262 PUSH_NULL
                      264 LOAD_NAME                3 (models)
                      266 LOAD_ATTR               19 (PositiveIntegerField)
                      276 LOAD_CONST               9 (0)
                      278 KW_NAMES                 6
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_NAME              20 (view_count)
          
-         122         296 PUSH_NULL
+         125         296 PUSH_NULL
                      298 LOAD_BUILD_CLASS
-                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 122>)
+                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 125>)
                      302 MAKE_FUNCTION            0
                      304 LOAD_CONST              11 ('Meta')
                      306 PRECALL                  2
                      310 CALL                     2
                      320 STORE_NAME              21 (Meta)
          
-         133         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 133>)
+         136         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
                      324 MAKE_FUNCTION            0
                      326 STORE_NAME              22 (__str__)
          
-         136         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
+         139         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
                      330 MAKE_FUNCTION            0
                      332 STORE_NAME              23 (can_edit)
          
-         139         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
+         142         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 142>)
                      336 MAKE_FUNCTION            0
                      338 STORE_NAME              24 (can_delete)
          
-         142         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 142>)
+         145         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 145>)
                      342 MAKE_FUNCTION            0
                      344 STORE_NAME              25 (can_post)
          
-         145         346 LOAD_NAME               26 (property)
+         148         346 LOAD_NAME               26 (property)
          
-         146         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 145>)
+         149         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 148>)
                      350 MAKE_FUNCTION            0
          
-         145         352 PRECALL                  0
+         148         352 PRECALL                  0
                      356 CALL                     0
          
-         146         366 STORE_NAME              27 (post_count)
+         149         366 STORE_NAME              27 (post_count)
          
-         149         368 LOAD_NAME               26 (property)
+         152         368 LOAD_NAME               26 (property)
          
-         150         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 149>)
+         153         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
                      372 MAKE_FUNCTION            0
          
-         149         374 PRECALL                  0
+         152         374 PRECALL                  0
                      378 CALL                     0
          
-         150         388 STORE_NAME              28 (latest_post)
+         153         388 STORE_NAME              28 (latest_post)
          
-         153         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 153>)
+         156         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
                      392 MAKE_FUNCTION            0
                      394 STORE_NAME              29 (get_absolute_url)
                      396 LOAD_CONST              19 (None)
                      398 RETURN_VALUE
          consts
             'Thread'
             'threads'
@@ -1315,75 +1348,75 @@
             0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035300
-               122           0 RESUME                   0
+               125           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               123          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
+               126          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
                
-               128          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
+               131          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
                             16 STORE_NAME               4 (permissions)
                             18 LOAD_CONST               3 (None)
                             20 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
                   (('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread'))
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 122
+               firstlineno 125
                lnotab 0x0a010405
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               133           0 RESUME                   0
+               136           0 RESUME                   0
                
-               134           2 LOAD_FAST                0 (self)
+               137           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 FORMAT_VALUE             0
                             16 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 133
+               firstlineno 136
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               136           0 RESUME                   0
+               139           0 RESUME                   0
                
-               137           2 LOAD_FAST                1 (user)
+               140           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_thread')
@@ -1395,28 +1428,28 @@
                   'punkweb_bb.change_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 136
+               firstlineno 139
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               139           0 RESUME                   0
+               142           0 RESUME                   0
                
-               140           2 LOAD_FAST                1 (user)
+               143           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_thread')
@@ -1428,77 +1461,77 @@
                   'punkweb_bb.delete_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 139
+               firstlineno 142
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000000c005300
-               142           0 RESUME                   0
+               145           0 RESUME                   0
                
-               143           2 LOAD_FAST                0 (self)
+               146           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (is_closed)
                             14 UNARY_NOT
                             16 RETURN_VALUE
                consts
                   None
                names      ('is_closed',)
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_post'
-               firstlineno 142
+               firstlineno 145
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               145           0 RESUME                   0
+               148           0 RESUME                   0
                
-               147           2 LOAD_FAST                0 (self)
+               150           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('posts', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 145
+               firstlineno 148
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-               149           0 RESUME                   0
+               152           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (self)
+               154           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1509,27 +1542,27 @@
                   '-created_at'
                names      ('posts', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_post'
-               firstlineno 149
+               firstlineno 152
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               153           0 RESUME                   0
+               156           0 RESUME                   0
                
-               154           2 LOAD_GLOBAL              1 (NULL + reverse)
+               157           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (id)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1540,24 +1573,24 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 153
+               firstlineno 156
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
-         firstlineno 110
+         firstlineno 113
          lnotab
             0x0a010e0110ff120330012201140122012201220122021a0b0603060306
             030603020104ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
@@ -1571,98 +1604,98 @@
             000000000000005a0b02004700640384006404a6020000ab020000000000
             0000005a0c640584005a0d640684005a0e640784005a0f651064088400a6
             000000ab0000000000000000005a11651064098400a6000000ab00000000
             00000000005a12640a84005a1388006601640b84085a14880078015a1553
             00
                        0 MAKE_CELL                0 (__class__)
          
-         157           2 RESUME                   0
+         160           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
          
-         158          12 PUSH_NULL
+         161          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (ForeignKey)
                       26 LOAD_NAME                5 (Thread)
                       28 LOAD_CONST               1 ('posts')
                       30 LOAD_NAME                3 (models)
                       32 LOAD_ATTR                6 (CASCADE)
                       42 KW_NAMES                 2
                       44 PRECALL                  3
                       48 CALL                     3
                       58 STORE_NAME               7 (thread)
          
-         159          60 PUSH_NULL
+         162          60 PUSH_NULL
                       62 LOAD_NAME                3 (models)
                       64 LOAD_ATTR                4 (ForeignKey)
                       74 LOAD_NAME                8 (User)
                       76 LOAD_CONST               1 ('posts')
                       78 LOAD_NAME                3 (models)
                       80 LOAD_ATTR                6 (CASCADE)
                       90 KW_NAMES                 2
                       92 PRECALL                  3
                       96 CALL                     3
                      106 STORE_NAME               9 (user)
          
-         160         108 PUSH_NULL
+         163         108 PUSH_NULL
                      110 LOAD_NAME               10 (BBCodeTextField)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_NAME              11 (content)
          
-         162         128 PUSH_NULL
+         165         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 162>)
+                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST               4 ('Meta')
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              12 (Meta)
          
-         165         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
+         168         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
                      156 MAKE_FUNCTION            0
                      158 STORE_NAME              13 (__str__)
          
-         168         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
+         171         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 171>)
                      162 MAKE_FUNCTION            0
                      164 STORE_NAME              14 (can_edit)
          
-         171         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 171>)
+         174         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
                      168 MAKE_FUNCTION            0
                      170 STORE_NAME              15 (can_delete)
          
-         174         172 LOAD_NAME               16 (property)
+         177         172 LOAD_NAME               16 (property)
          
-         175         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
+         178         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 177>)
                      176 MAKE_FUNCTION            0
          
-         174         178 PRECALL                  0
+         177         178 PRECALL                  0
                      182 CALL                     0
          
-         175         192 STORE_NAME              17 (index)
+         178         192 STORE_NAME              17 (index)
          
-         182         194 LOAD_NAME               16 (property)
+         185         194 LOAD_NAME               16 (property)
          
-         183         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 182>)
+         186         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 185>)
                      198 MAKE_FUNCTION            0
          
-         182         200 PRECALL                  0
+         185         200 PRECALL                  0
                      204 CALL                     0
          
-         183         214 STORE_NAME              18 (page_number)
+         186         214 STORE_NAME              18 (page_number)
          
-         186         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 186>)
+         189         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 189>)
                      218 MAKE_FUNCTION            0
                      220 STORE_NAME              19 (get_absolute_url)
          
-         193         222 LOAD_CLOSURE             0 (__class__)
+         196         222 LOAD_CLOSURE             0 (__class__)
                      224 BUILD_TUPLE              1
-                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 193>)
+                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
                      228 MAKE_FUNCTION            8 (closure)
                      230 STORE_NAME              20 (save)
                      232 LOAD_CLOSURE             0 (__class__)
                      234 COPY                     1
                      236 STORE_NAME              21 (__classcell__)
                      238 RETURN_VALUE
          consts
@@ -1671,48 +1704,48 @@
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               162           0 RESUME                   0
+               165           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Post.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               163          10 LOAD_CONST               1 (('created_at',))
+               166          10 LOAD_CONST               1 (('created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Post.Meta'
                   ('created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 162
+               firstlineno 165
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064017c006a0200000000000000009b009d055300
-               165           0 RESUME                   0
+               168           0 RESUME                   0
                
-               166           2 LOAD_FAST                0 (self)
+               169           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (user)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 (' > ')
@@ -1726,28 +1759,28 @@
                   ' > '
                names      ('thread', 'user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 165
+               firstlineno 168
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               168           0 RESUME                   0
+               171           0 RESUME                   0
                
-               169           2 LOAD_FAST                1 (user)
+               172           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_post')
@@ -1759,28 +1792,28 @@
                   'punkweb_bb.change_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 168
+               firstlineno 171
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               171           0 RESUME                   0
+               174           0 RESUME                   0
                
-               172           2 LOAD_FAST                1 (user)
+               175           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_post')
@@ -1792,41 +1825,41 @@
                   'punkweb_bb.delete_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 171
+               firstlineno 174
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000006401a6010000ab010000000000
                   0000007d017407000000000000000000007c01a004000000000000000000
                   000000000000000000000064026403ac04a6020000ab0200000000000000
                   00a6010000ab010000000000000000a00500000000000000000000000000
                   000000000000007c006a060000000000000000a6010000ab010000000000
                   0000007d027c0264057a0000005300
-               174           0 RESUME                   0
+               177           0 RESUME                   0
                
-               178           2 LOAD_FAST                0 (self)
+               181           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 LOAD_ATTR                1 (posts)
                             24 LOAD_METHOD              2 (order_by)
                             46 LOAD_CONST               1 ('created_at')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (qs)
                
-               179          64 LOAD_GLOBAL              7 (NULL + list)
+               182          64 LOAD_GLOBAL              7 (NULL + list)
                             76 LOAD_FAST                1 (qs)
                             78 LOAD_METHOD              4 (values_list)
                            100 LOAD_CONST               2 ('id')
                            102 LOAD_CONST               3 (True)
                            104 KW_NAMES                 4
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1835,15 +1868,15 @@
                            134 LOAD_METHOD              5 (index)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                6 (id)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 STORE_FAST               2 (index)
                
-               180         184 LOAD_FAST                2 (index)
+               183         184 LOAD_FAST                2 (index)
                            186 LOAD_CONST               5 (1)
                            188 BINARY_OP                0 (+)
                            192 RETURN_VALUE
                consts
                   None
                   'created_at'
                   'id'
@@ -1852,27 +1885,27 @@
                   1
                names      ('thread', 'posts', 'order_by', 'list', 'values_list', 'index', 'id')
                varnames   ('self', 'qs', 'index')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'index'
-               firstlineno 174
+               firstlineno 177
                lnotab 0x02043e017801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   0000000000000064017a0b0000a6010000ab0100000000000000005300
-               182           0 RESUME                   0
+               185           0 RESUME                   0
                
-               184           2 LOAD_GLOBAL              1 (NULL + math)
+               187           2 LOAD_GLOBAL              1 (NULL + math)
                             14 LOAD_ATTR                1 (ceil)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (index)
                             36 LOAD_CONST               1 (10)
                             38 BINARY_OP               11 (/)
                             42 PRECALL                  1
                             46 CALL                     1
@@ -1882,67 +1915,67 @@
                   10
                names      ('math', 'ceil', 'index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'page_number'
-               firstlineno 182
+               firstlineno 185
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a0100000000000000006a
                   0200000000000000006701ac02a6020000ab0200000000000000007d017c
                   0164037c006a0300000000000000009b0064047c006a0200000000000000
                   009b009d047a0d00007d017c015300
-               186           0 RESUME                   0
+               189           0 RESUME                   0
                
-               187           2 LOAD_GLOBAL              1 (NULL + reverse)
+               190           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (thread)
                             28 LOAD_ATTR                2 (id)
                             38 BUILD_LIST               1
                             40 KW_NAMES                 2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_FAST               1 (thread_url)
                
-               189          58 LOAD_FAST                1 (thread_url)
+               192          58 LOAD_FAST                1 (thread_url)
                             60 LOAD_CONST               3 ('?page=')
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (page_number)
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 ('#post-')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                2 (id)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             4
                             94 BINARY_OP               13 (+=)
                             98 STORE_FAST               1 (thread_url)
                
-               191         100 LOAD_FAST                1 (thread_url)
+               194         100 LOAD_FAST                1 (thread_url)
                            102 RETURN_VALUE
                consts
                   None
                   'punkweb_bb:thread'
                   ('args',)
                   '?page='
                   '#post-'
                names      ('reverse', 'thread', 'id', 'page_number')
                varnames   ('self', 'thread_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 186
+               firstlineno 189
                lnotab 0x020138022a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
@@ -1953,48 +1986,48 @@
                   006a0000000000000000005f0700000000000000007c006a000000000000
                   000000a0080000000000000000000000000000000000000000a6000000ab
                   00000000000000000001000200741300000000000000000000a6000000ab
                   0000000000000000006a0800000000000000007c0169007c02a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               193           2 RESUME                   0
+               196           2 RESUME                   0
                
-               194           4 LOAD_FAST                0 (self)
+               197           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (thread)
                             16 LOAD_ATTR                1 (is_closed)
                             26 POP_JUMP_FORWARD_IF_FALSE    15 (to 58)
                
-               195          28 LOAD_GLOBAL              5 (NULL + ValidationError)
+               198          28 LOAD_GLOBAL              5 (NULL + ValidationError)
                             40 LOAD_CONST               1 ('Cannot add posts to a closed thread.')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 RAISE_VARARGS            1
                
-               196     >>   58 LOAD_FAST                0 (self)
+               199     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                3 (_state)
                             70 LOAD_ATTR                4 (adding)
                             80 POP_JUMP_FORWARD_IF_FALSE    54 (to 190)
                
-               197          82 LOAD_GLOBAL             11 (NULL + timezone)
+               200          82 LOAD_GLOBAL             11 (NULL + timezone)
                             94 LOAD_ATTR                6 (now)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                0 (thread)
                            130 STORE_ATTR               7 (last_post_created_at)
                
-               198         140 LOAD_FAST                0 (self)
+               201         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                0 (thread)
                            152 LOAD_METHOD              8 (save)
                            174 PRECALL                  0
                            178 CALL                     0
                            188 POP_TOP
                
-               199     >>  190 PUSH_NULL
+               202     >>  190 PUSH_NULL
                            192 LOAD_GLOBAL             19 (NULL + super)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_ATTR                8 (save)
                            228 LOAD_FAST                1 (args)
                            230 BUILD_MAP                0
                            232 LOAD_FAST                2 (kwargs)
@@ -2008,23 +2041,23 @@
                   'Cannot add posts to a closed thread.'
                names      ('thread', 'is_closed', 'ValidationError', '_state', 'adding', 'timezone', 'now', 'last_post_created_at', 'save', 'super')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
-               firstlineno 193
+               firstlineno 196
                lnotab 0x040118011e0118013a013201
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
-         firstlineno 157
+         firstlineno 160
          lnotab
             0x0c013001300114021a03060306030603020104ff0e010207020104ff0e
             0102030607
       'Post'
       code
          argcount  : 0
          nlocals   : 0
@@ -2032,101 +2065,101 @@
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000a6000000ab0000000000000000005a0902
             004700640384006404a6020000ab0200000000000000005a0a640584005a
             0b640684005a0c64075300
-         202           0 RESUME                   0
+         205           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Shout')
                        8 STORE_NAME               2 (__qualname__)
          
-         203          10 PUSH_NULL
+         206          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('shouts')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-         204          58 PUSH_NULL
+         207          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (TextField)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 STORE_NAME               9 (content)
          
-         206          88 PUSH_NULL
+         209          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
-                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 206>)
+                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 209>)
                       94 MAKE_FUNCTION            0
                       96 LOAD_CONST               4 ('Meta')
                       98 PRECALL                  2
                      102 CALL                     2
                      112 STORE_NAME              10 (Meta)
          
-         209         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 209>)
+         212         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 212>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              11 (__str__)
          
-         212         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 212>)
+         215         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 215>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              12 (can_delete)
                      126 LOAD_CONST               7 (None)
                      128 RETURN_VALUE
          consts
             'Shout'
             'shouts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               206           0 RESUME                   0
+               209           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Shout.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               207          10 LOAD_CONST               1 (('-created_at',))
+               210          10 LOAD_CONST               1 (('-created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Shout.Meta'
                   ('-created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 206
+               firstlineno 209
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               209           0 RESUME                   0
+               212           0 RESUME                   0
                
-               210           2 LOAD_FAST                0 (self)
+               213           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (created_at)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -2136,28 +2169,28 @@
                   ' > '
                names      ('user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 209
+               firstlineno 212
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               212           0 RESUME                   0
+               215           0 RESUME                   0
                
-               213           2 LOAD_FAST                1 (user)
+               216           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_shout')
@@ -2169,85 +2202,85 @@
                   'punkweb_bb.delete_shout'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 212
+               firstlineno 215
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__', 'can_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Shout'
-         firstlineno 202
+         firstlineno 205
          lnotab 0x0a0130011e021a030603
       'Shout'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a08000000000000000064036404ac05a6020000ab020000000000
             0000005a090200650aa6000000ab0000000000000000005a0b0200470064
             0684006407a6020000ab0200000000000000005a0c640884005a0d640953
             00
-         216           0 RESUME                   0
+         219           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupStyle')
                        8 STORE_NAME               2 (__qualname__)
          
-         217          10 PUSH_NULL
+         220          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (OneToOneField)
                       24 LOAD_NAME                5 (Group)
                       26 LOAD_CONST               1 ('style')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (group)
          
-         218          58 PUSH_NULL
+         221          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (PositiveIntegerField)
          
-         219          72 LOAD_CONST               3 (0)
+         222          72 LOAD_CONST               3 (0)
          
-         220          74 LOAD_CONST               4 ('Highest priority is displayed')
+         223          74 LOAD_CONST               4 ('Highest priority is displayed')
          
-         218          76 KW_NAMES                 5
+         221          76 KW_NAMES                 5
                       78 PRECALL                  2
                       82 CALL                     2
                       92 STORE_NAME               9 (priority)
          
-         222          94 PUSH_NULL
+         225          94 PUSH_NULL
                       96 LOAD_NAME               10 (BBCodeTextField)
                       98 PRECALL                  0
                      102 CALL                     0
                      112 STORE_NAME              11 (username_style)
          
-         224         114 PUSH_NULL
+         227         114 PUSH_NULL
                      116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               6 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 224>)
+                     118 LOAD_CONST               6 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 227>)
                      120 MAKE_FUNCTION            0
                      122 LOAD_CONST               7 ('Meta')
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_NAME              12 (Meta)
          
-         227         140 LOAD_CONST               8 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 227>)
+         230         140 LOAD_CONST               8 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 230>)
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              13 (__str__)
                      146 LOAD_CONST               9 (None)
                      148 RETURN_VALUE
          consts
             'GroupStyle'
             'style'
@@ -2257,48 +2290,48 @@
             ('default', 'help_text')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               224           0 RESUME                   0
+               227           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('GroupStyle.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               225          10 LOAD_CONST               1 (('-priority',))
+               228          10 LOAD_CONST               1 (('-priority',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'GroupStyle.Meta'
                   ('-priority',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 224
+               firstlineno 227
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               227           0 RESUME                   0
+               230           0 RESUME                   0
                
-               228           2 LOAD_FAST                0 (self)
+               231           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (group)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (priority)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -2308,29 +2341,29 @@
                   ' > '
                names      ('group', 'priority')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 227
+               firstlineno 230
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'Group', 'CASCADE', 'group', 'PositiveIntegerField', 'priority', 'BBCodeTextField', 'username_style', 'Meta', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'GroupStyle'
-         firstlineno 216
+         firstlineno 219
          lnotab 0x0a0130010e01020102fe120414021a03
       'GroupStyle'
-   names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'punkweb_bb.utils', 'get_styled_username', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout', 'GroupStyle')
+   names      ('math', 'os', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'punkweb_bb.utils', 'get_highest_priority_group', 'get_styled_username', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout', 'GroupStyle')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108020c010c010c010c010c010c010c010c0210010c
-      02140306051e1b1e121e281e2f1e2d1e0e
+      0x00ff0201080108020c010c010c010c010c010c010c010c021001100214
+      0306051e1f1e121e281e2f1e2d1e0e
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe6b05666 (Wed May 29 04:36:54 2024 UTC)
+moddate:  0xa69b5766 (Wed May 29 21:18:30 2024 UTC)
 files sz: 561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/utils.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/utils.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf78b5766 (Wed May 29 20:11:35 2024 UTC)
-files sz: 1223
+moddate:  0xf5975766 (Wed May 29 21:02:45 2024 UTC)
+files sz: 1200
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640384
@@ -25,25 +25,25 @@
                 22 STORE_NAME               3 (slugify)
                 24 POP_TOP
    
      5          26 LOAD_CONST               3 (<code object get_unique_slug, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 5>)
                 28 MAKE_FUNCTION            0
                 30 STORE_NAME               4 (get_unique_slug)
    
-    21          32 LOAD_CONST               4 (<code object get_user_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 21>)
+    21          32 LOAD_CONST               4 (<code object get_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 21>)
                 34 MAKE_FUNCTION            0
-                36 STORE_NAME               5 (get_user_highest_priority_group)
+                36 STORE_NAME               5 (get_highest_priority_group)
    
     30          38 LOAD_CONST               5 (<code object get_styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 30>)
                 40 MAKE_FUNCTION            0
                 42 STORE_NAME               6 (get_styled_username)
    
-    41          44 LOAD_CONST               6 (<code object get_group_name_styled, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 41>)
+    41          44 LOAD_CONST               6 (<code object get_styled_group_name, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 41>)
                 46 MAKE_FUNCTION            0
-                48 STORE_NAME               7 (get_group_name_styled)
+                48 STORE_NAME               7 (get_styled_group_name)
                 50 LOAD_CONST               7 (None)
                 52 RETURN_VALUE
    consts
       0
       ('Group',)
       ('slugify',)
       code
@@ -126,81 +126,79 @@
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_unique_slug'
          firstlineno 5
          lnotab 0x02011e0104010402040104015a010e010c0204fb0407
       code
          argcount  : 1
          nlocals   : 2
-         stacksize : 4
+         stacksize : 3
          flags     : 3
          code
-            0x97007400000000000000000000006a010000000000000000a002000000
-            00000000000000000000000000000000007c006401ac02a6020000ab0200
-            000000000000007d017c01a0030000000000000000000000000000000000
-            000000a6000000ab00000000000000000072277c01a00400000000000000
-            000000000000000000000000006403a6010000ab010000000000000000a0
-            050000000000000000000000000000000000000000a6000000ab00000000
-            0000000000530064005300
+            0x97007c006a000000000000000000a00100000000000000000000000000
+            000000000000006401ac02a6010000ab0100000000000000007d017c01a0
+            020000000000000000000000000000000000000000a6000000ab00000000
+            000000000072277c01a00300000000000000000000000000000000000000
+            006403a6010000ab010000000000000000a0040000000000000000000000
+            000000000000000000a6000000ab000000000000000000530064005300
           21           0 RESUME                   0
          
-          22           2 LOAD_GLOBAL              0 (Group)
-                      14 LOAD_ATTR                1 (objects)
-                      24 LOAD_METHOD              2 (filter)
-                      46 LOAD_FAST                0 (user)
-                      48 LOAD_CONST               1 (False)
-                      50 KW_NAMES                 2
-                      52 PRECALL                  2
-                      56 CALL                     2
-                      66 STORE_FAST               1 (groups)
-         
-          24          68 LOAD_FAST                1 (groups)
-                      70 LOAD_METHOD              3 (exists)
-                      92 PRECALL                  0
-                      96 CALL                     0
-                     106 POP_JUMP_FORWARD_IF_FALSE    39 (to 186)
-         
-          25         108 LOAD_FAST                1 (groups)
-                     110 LOAD_METHOD              4 (order_by)
-                     132 LOAD_CONST               3 ('-style__priority')
-                     134 PRECALL                  1
-                     138 CALL                     1
-                     148 LOAD_METHOD              5 (first)
-                     170 PRECALL                  0
-                     174 CALL                     0
-                     184 RETURN_VALUE
+          22           2 LOAD_FAST                0 (user)
+                       4 LOAD_ATTR                0 (groups)
+                      14 LOAD_METHOD              1 (filter)
+                      36 LOAD_CONST               1 (False)
+                      38 KW_NAMES                 2
+                      40 PRECALL                  1
+                      44 CALL                     1
+                      54 STORE_FAST               1 (groups)
+         
+          24          56 LOAD_FAST                1 (groups)
+                      58 LOAD_METHOD              2 (exists)
+                      80 PRECALL                  0
+                      84 CALL                     0
+                      94 POP_JUMP_FORWARD_IF_FALSE    39 (to 174)
+         
+          25          96 LOAD_FAST                1 (groups)
+                      98 LOAD_METHOD              3 (order_by)
+                     120 LOAD_CONST               3 ('-style__priority')
+                     122 PRECALL                  1
+                     126 CALL                     1
+                     136 LOAD_METHOD              4 (first)
+                     158 PRECALL                  0
+                     162 CALL                     0
+                     172 RETURN_VALUE
          
-          27     >>  186 LOAD_CONST               0 (None)
-                     188 RETURN_VALUE
+          27     >>  174 LOAD_CONST               0 (None)
+                     176 RETURN_VALUE
          consts
             None
             False
-            ('user', 'style__isnull')
+            ('style__isnull',)
             '-style__priority'
-         names      ('Group', 'objects', 'filter', 'exists', 'order_by', 'first')
+         names      ('groups', 'filter', 'exists', 'order_by', 'first')
          varnames   ('user', 'groups')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
-         name       'get_user_highest_priority_group'
+         name       'get_highest_priority_group'
          firstlineno 21
-         lnotab 0x0201420228014e02
+         lnotab 0x0201360228014e02
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007d017c01722e7c016a0100000000000000006a0200000000000000007d
             027c026a030000000000000000a004000000000000000000000000000000
             000000000064017c006a050000000000000000a6020000ab020000000000
             0000007d037c0353007c006a0500000000000000005300
           30           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              1 (NULL + get_user_highest_priority_group)
+          31           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
                       14 LOAD_FAST                0 (user)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (group)
          
           33          32 LOAD_FAST                1 (group)
                       34 POP_JUMP_FORWARD_IF_FALSE    46 (to 128)
@@ -225,15 +223,15 @@
          
           38     >>  128 LOAD_FAST                0 (user)
                      130 LOAD_ATTR                5 (username)
                      140 RETURN_VALUE
          consts
             None
             '{USER}'
-         names      ('get_user_highest_priority_group', 'style', 'username_style', 'rendered', 'replace', 'username')
+         names      ('get_highest_priority_group', 'style', 'username_style', 'rendered', 'replace', 'username')
          varnames   ('user', 'group', 'username_style', 'styled_username')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_styled_username'
          firstlineno 30
          lnotab 0x02011e020401180140010402
@@ -279,19 +277,19 @@
             None
             '{USER}'
          names      ('style', 'name', 'username_style', 'rendered', 'replace')
          varnames   ('group', 'username_style', 'styled_group_name')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
-         name       'get_group_name_styled'
+         name       'get_styled_group_name'
          firstlineno 41
          lnotab 0x02010e010e0218014001
       None
-   names      ('django.contrib.auth.models', 'Group', 'django.utils.text', 'slugify', 'get_unique_slug', 'get_user_highest_priority_group', 'get_styled_username', 'get_group_name_styled')
+   names      ('django.contrib.auth.models', 'Group', 'django.utils.text', 'slugify', 'get_unique_slug', 'get_highest_priority_group', 'get_styled_username', 'get_styled_group_name')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c0306100609060b
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,470 +1,464 @@
 magic:    0xa70d0d0a
-moddate:  0x34825666 (Wed May 29 01:17:40 2024 UTC)
-files sz: 17400
+moddate:  0xb0a55766 (Wed May 29 22:01:20 2024 UTC)
+files sz: 17383
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
-      055a050100640064036c066d075a070100640064046c086d095a09010064
-      0064056c0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00640064076c106d115a110100640064086c126d135a136d145a146d155a
-      156d165a166d175a176d185a186d195a196d1a5a1a0100640064096c1b6d
-      1c5a1c01006400640a6c1d6d1e5a1e6d1f5a1f6d205a206d215a216d225a
-      2201006400640b6c236d245a2401006400640c6c256d265a260100640064
-      0d6c276d285a28010002006503a6000000ab0000000000000000005a2964
-      0e84005a2a640f84005a2b641084005a2c641184005a2d641284005a2e64
-      1384005a2f020065076414ac15a6010000ab010000000000000000641684
-      00a6000000ab0000000000000000005a30020065076414ac15a6010000ab
-      01000000000000000064178400a6000000ab0000000000000000005a3102
-      0065076414ac15a6010000ab01000000000000000064188400a6000000ab
-      0000000000000000005a32020065076414ac15a6010000ab010000000000
-      00000064198400a6000000ab0000000000000000005a33641a84005a3402
-      0065076414ac15a6010000ab010000000000000000641b8400a6000000ab
-      0000000000000000005a35020065076414ac15a6010000ab010000000000
-      000000641c8400a6000000ab0000000000000000005a36020065076414ac
-      15a6010000ab010000000000000000641d8400a6000000ab000000000000
-      0000005a37020065076414ac15a6010000ab010000000000000000641e84
-      00a6000000ab0000000000000000005a38641f84005a39020065076414ac
-      15a6010000ab01000000000000000064208400a6000000ab000000000000
-      0000005a3a020065076414ac15a6010000ab010000000000000000642184
-      00a6000000ab0000000000000000005a3b020065076414ac15a6010000ab
-      01000000000000000064228400a6000000ab0000000000000000005a3c02
-      0065076414ac15a6010000ab01000000000000000064238400a6000000ab
-      0000000000000000005a3d020065076414ac15a6010000ab010000000000
-      00000064248400a6000000ab0000000000000000005a3e020065076414ac
-      15a6010000ab01000000000000000064258400a6000000ab000000000000
-      0000005a3f020065076414ac15a6010000ab010000000000000000642684
-      00a6000000ab0000000000000000005a40642784005a41642884005a4264
-      2984005a43020065076414ac15a6010000ab010000000000000000642a84
-      00a6000000ab0000000000000000005a44642b84005a4564015300
+      0x9700640064016c006d015a016d025a026d035a036d045a040100640064
+      026c056d065a060100640064036c076d085a080100640064046c096d0a5a
+      0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
+      105a100100640064076c116d125a126d135a136d145a146d155a156d165a
+      166d175a176d185a186d195a190100640064086c1a6d1b5a1b0100640064
+      096c1c6d1d5a1d6d1e5a1e6d1f5a1f6d205a206d215a2101006400640a6c
+      226d235a2301006400640b6c246d255a2501006400640c6c266d275a2701
+      0002006502a6000000ab0000000000000000005a28640d84005a29640e84
+      005a2a640f84005a2b641084005a2c641184005a2d641284005a2e020065
+      066413ac14a6010000ab01000000000000000064158400a6000000ab0000
+      000000000000005a2f020065066413ac14a6010000ab0100000000000000
+      0064168400a6000000ab0000000000000000005a30020065066413ac14a6
+      010000ab01000000000000000064178400a6000000ab0000000000000000
+      005a31020065066413ac14a6010000ab01000000000000000064188400a6
+      000000ab0000000000000000005a32641984005a33020065066413ac14a6
+      010000ab010000000000000000641a8400a6000000ab0000000000000000
+      005a34020065066413ac14a6010000ab010000000000000000641b8400a6
+      000000ab0000000000000000005a35020065066413ac14a6010000ab0100
+      00000000000000641c8400a6000000ab0000000000000000005a36020065
+      066413ac14a6010000ab010000000000000000641d8400a6000000ab0000
+      000000000000005a37641e84005a38020065066413ac14a6010000ab0100
+      00000000000000641f8400a6000000ab0000000000000000005a39020065
+      066413ac14a6010000ab01000000000000000064208400a6000000ab0000
+      000000000000005a3a020065066413ac14a6010000ab0100000000000000
+      0064218400a6000000ab0000000000000000005a3b020065066413ac14a6
+      010000ab01000000000000000064228400a6000000ab0000000000000000
+      005a3c020065066413ac14a6010000ab01000000000000000064238400a6
+      000000ab0000000000000000005a3d020065066413ac14a6010000ab0100
+      0000000000000064248400a6000000ab0000000000000000005a3e020065
+      066413ac14a6010000ab01000000000000000064258400a6000000ab0000
+      000000000000005a3f642684005a40642784005a41642884005a42020065
+      066413ac14a6010000ab01000000000000000064298400a6000000ab0000
+      000000000000005a43642a84005a44642b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (datetime)
-                 8 STORE_NAME               0 (datetime)
-   
-     3          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('authenticate', 'get_user_model', 'login', 'logout'))
-                14 IMPORT_NAME              1 (django.contrib.auth)
-                16 IMPORT_FROM              2 (authenticate)
-                18 STORE_NAME               2 (authenticate)
-                20 IMPORT_FROM              3 (get_user_model)
-                22 STORE_NAME               3 (get_user_model)
-                24 IMPORT_FROM              4 (login)
-                26 STORE_NAME               4 (login)
-                28 IMPORT_FROM              5 (logout)
-                30 STORE_NAME               5 (logout)
-                32 POP_TOP
-   
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('login_required',))
-                38 IMPORT_NAME              6 (django.contrib.auth.decorators)
-                40 IMPORT_FROM              7 (login_required)
-                42 STORE_NAME               7 (login_required)
-                44 POP_TOP
-   
-     5          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('HttpResponseForbidden',))
-                50 IMPORT_NAME              8 (django.http)
-                52 IMPORT_FROM              9 (HttpResponseForbidden)
-                54 STORE_NAME               9 (HttpResponseForbidden)
-                56 POP_TOP
-   
-     6          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('get_object_or_404', 'redirect', 'render'))
-                62 IMPORT_NAME             10 (django.shortcuts)
-                64 IMPORT_FROM             11 (get_object_or_404)
-                66 STORE_NAME              11 (get_object_or_404)
-                68 IMPORT_FROM             12 (redirect)
-                70 STORE_NAME              12 (redirect)
-                72 IMPORT_FROM             13 (render)
-                74 STORE_NAME              13 (render)
-                76 POP_TOP
-   
-     7          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('reverse',))
-                82 IMPORT_NAME             14 (django.urls)
-                84 IMPORT_FROM             15 (reverse)
-                86 STORE_NAME              15 (reverse)
-                88 POP_TOP
-   
-     8          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('timezone',))
-                94 IMPORT_NAME             16 (django.utils)
-                96 IMPORT_FROM             17 (timezone)
-                98 STORE_NAME              17 (timezone)
-               100 POP_TOP
-   
-    10         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm'))
-               106 IMPORT_NAME             18 (punkweb_bb.forms)
-               108 IMPORT_FROM             19 (BoardProfileModelForm)
-               110 STORE_NAME              19 (BoardProfileModelForm)
-               112 IMPORT_FROM             20 (CategoryModelForm)
-               114 STORE_NAME              20 (CategoryModelForm)
-               116 IMPORT_FROM             21 (LoginForm)
-               118 STORE_NAME              21 (LoginForm)
-               120 IMPORT_FROM             22 (PostModelForm)
-               122 STORE_NAME              22 (PostModelForm)
-               124 IMPORT_FROM             23 (ShoutModelForm)
-               126 STORE_NAME              23 (ShoutModelForm)
-               128 IMPORT_FROM             24 (SignUpForm)
-               130 STORE_NAME              24 (SignUpForm)
-               132 IMPORT_FROM             25 (SubcategoryModelForm)
-               134 STORE_NAME              25 (SubcategoryModelForm)
-               136 IMPORT_FROM             26 (ThreadModelForm)
-               138 STORE_NAME              26 (ThreadModelForm)
-               140 POP_TOP
-   
-    20         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST               9 (('guest_list',))
-               146 IMPORT_NAME             27 (punkweb_bb.guests)
-               148 IMPORT_FROM             28 (guest_list)
-               150 STORE_NAME              28 (guest_list)
-               152 POP_TOP
-   
-    21         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST              10 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
-               158 IMPORT_NAME             29 (punkweb_bb.models)
-               160 IMPORT_FROM             30 (Category)
-               162 STORE_NAME              30 (Category)
-               164 IMPORT_FROM             31 (Post)
-               166 STORE_NAME              31 (Post)
-               168 IMPORT_FROM             32 (Shout)
-               170 STORE_NAME              32 (Shout)
-               172 IMPORT_FROM             33 (Subcategory)
-               174 STORE_NAME              33 (Subcategory)
-               176 IMPORT_FROM             34 (Thread)
-               178 STORE_NAME              34 (Thread)
-               180 POP_TOP
-   
-    22         182 LOAD_CONST               0 (0)
-               184 LOAD_CONST              11 (('paginate_qs',))
-               186 IMPORT_NAME             35 (punkweb_bb.pagination)
-               188 IMPORT_FROM             36 (paginate_qs)
-               190 STORE_NAME              36 (paginate_qs)
-               192 POP_TOP
-   
-    23         194 LOAD_CONST               0 (0)
-               196 LOAD_CONST              12 (('htmx_redirect',))
-               198 IMPORT_NAME             37 (punkweb_bb.response)
-               200 IMPORT_FROM             38 (htmx_redirect)
-               202 STORE_NAME              38 (htmx_redirect)
-               204 POP_TOP
-   
-    24         206 LOAD_CONST               0 (0)
-               208 LOAD_CONST              13 (('get_unique_slug',))
-               210 IMPORT_NAME             39 (punkweb_bb.utils)
-               212 IMPORT_FROM             40 (get_unique_slug)
-               214 STORE_NAME              40 (get_unique_slug)
-               216 POP_TOP
-   
-    26         218 PUSH_NULL
-               220 LOAD_NAME                3 (get_user_model)
-               222 PRECALL                  0
-               226 CALL                     0
-               236 STORE_NAME              41 (User)
-   
-    29         238 LOAD_CONST              14 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 29>)
-               240 MAKE_FUNCTION            0
-               242 STORE_NAME              42 (signup_view)
-   
-    49         244 LOAD_CONST              15 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 49>)
-               246 MAKE_FUNCTION            0
-               248 STORE_NAME              43 (login_view)
-   
-    75         250 LOAD_CONST              16 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 75>)
-               252 MAKE_FUNCTION            0
-               254 STORE_NAME              44 (logout_view)
-   
-    80         256 LOAD_CONST              17 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 80>)
-               258 MAKE_FUNCTION            0
-               260 STORE_NAME              45 (index_view)
-   
-   112         262 LOAD_CONST              18 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 112>)
-               264 MAKE_FUNCTION            0
-               266 STORE_NAME              46 (profile_view)
-   
-   121         268 LOAD_CONST              19 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 121>)
-               270 MAKE_FUNCTION            0
-               272 STORE_NAME              47 (members_view)
-   
-   132         274 PUSH_NULL
-               276 LOAD_NAME                7 (login_required)
-               278 LOAD_CONST              20 ('/login/')
-               280 KW_NAMES                21
-               282 PRECALL                  1
-               286 CALL                     1
-   
-   133         296 LOAD_CONST              22 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 132>)
-               298 MAKE_FUNCTION            0
-   
-   132         300 PRECALL                  0
-               304 CALL                     0
-   
-   133         314 STORE_NAME              48 (settings_view)
-   
-   155         316 PUSH_NULL
-               318 LOAD_NAME                7 (login_required)
-               320 LOAD_CONST              20 ('/login/')
-               322 KW_NAMES                21
-               324 PRECALL                  1
-               328 CALL                     1
-   
-   156         338 LOAD_CONST              23 (<code object category_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 155>)
-               340 MAKE_FUNCTION            0
-   
-   155         342 PRECALL                  0
-               346 CALL                     0
-   
-   156         356 STORE_NAME              49 (category_create_view)
-   
-   178         358 PUSH_NULL
-               360 LOAD_NAME                7 (login_required)
-               362 LOAD_CONST              20 ('/login/')
-               364 KW_NAMES                21
-               366 PRECALL                  1
-               370 CALL                     1
-   
-   179         380 LOAD_CONST              24 (<code object category_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 178>)
-               382 MAKE_FUNCTION            0
-   
-   178         384 PRECALL                  0
-               388 CALL                     0
-   
-   179         398 STORE_NAME              50 (category_update_view)
-   
-   202         400 PUSH_NULL
-               402 LOAD_NAME                7 (login_required)
-               404 LOAD_CONST              20 ('/login/')
-               406 KW_NAMES                21
-               408 PRECALL                  1
-               412 CALL                     1
-   
-   203         422 LOAD_CONST              25 (<code object category_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 202>)
-               424 MAKE_FUNCTION            0
-   
-   202         426 PRECALL                  0
-               430 CALL                     0
-   
-   203         440 STORE_NAME              51 (category_delete_view)
-   
-   221         442 LOAD_CONST              26 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 221>)
-               444 MAKE_FUNCTION            0
-               446 STORE_NAME              52 (subcategory_view)
-   
-   233         448 PUSH_NULL
-               450 LOAD_NAME                7 (login_required)
-               452 LOAD_CONST              20 ('/login/')
-               454 KW_NAMES                21
-               456 PRECALL                  1
-               460 CALL                     1
-   
-   234         470 LOAD_CONST              27 (<code object subcategory_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 233>)
-               472 MAKE_FUNCTION            0
-   
-   233         474 PRECALL                  0
-               478 CALL                     0
-   
-   234         488 STORE_NAME              53 (subcategory_create_view)
-   
-   262         490 PUSH_NULL
-               492 LOAD_NAME                7 (login_required)
-               494 LOAD_CONST              20 ('/login/')
-               496 KW_NAMES                21
-               498 PRECALL                  1
-               502 CALL                     1
-   
-   263         512 LOAD_CONST              28 (<code object subcategory_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 262>)
-               514 MAKE_FUNCTION            0
-   
-   262         516 PRECALL                  0
-               520 CALL                     0
-   
-   263         530 STORE_NAME              54 (subcategory_update_view)
-   
-   288         532 PUSH_NULL
-               534 LOAD_NAME                7 (login_required)
-               536 LOAD_CONST              20 ('/login/')
-               538 KW_NAMES                21
-               540 PRECALL                  1
-               544 CALL                     1
-   
-   289         554 LOAD_CONST              29 (<code object subcategory_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 288>)
-               556 MAKE_FUNCTION            0
-   
-   288         558 PRECALL                  0
-               562 CALL                     0
-   
-   289         572 STORE_NAME              55 (subcategory_delete_view)
-   
-   311         574 PUSH_NULL
-               576 LOAD_NAME                7 (login_required)
-               578 LOAD_CONST              20 ('/login/')
-               580 KW_NAMES                21
-               582 PRECALL                  1
-               586 CALL                     1
-   
-   312         596 LOAD_CONST              30 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 311>)
-               598 MAKE_FUNCTION            0
-   
-   311         600 PRECALL                  0
-               604 CALL                     0
-   
-   312         614 STORE_NAME              56 (thread_create_view)
-   
-   340         616 LOAD_CONST              31 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 340>)
-               618 MAKE_FUNCTION            0
-               620 STORE_NAME              57 (thread_view)
-   
-   362         622 PUSH_NULL
-               624 LOAD_NAME                7 (login_required)
-               626 LOAD_CONST              20 ('/login/')
-               628 KW_NAMES                21
-               630 PRECALL                  1
-               634 CALL                     1
-   
-   363         644 LOAD_CONST              32 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 362>)
-               646 MAKE_FUNCTION            0
-   
-   362         648 PRECALL                  0
-               652 CALL                     0
-   
-   363         662 STORE_NAME              58 (thread_update_view)
-   
-   388         664 PUSH_NULL
-               666 LOAD_NAME                7 (login_required)
-               668 LOAD_CONST              20 ('/login/')
-               670 KW_NAMES                21
-               672 PRECALL                  1
-               676 CALL                     1
-   
-   389         686 LOAD_CONST              33 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 388>)
-               688 MAKE_FUNCTION            0
-   
-   388         690 PRECALL                  0
-               694 CALL                     0
-   
-   389         704 STORE_NAME              59 (thread_delete_view)
-   
-   409         706 PUSH_NULL
-               708 LOAD_NAME                7 (login_required)
-               710 LOAD_CONST              20 ('/login/')
-               712 KW_NAMES                21
-               714 PRECALL                  1
-               718 CALL                     1
-   
-   410         728 LOAD_CONST              34 (<code object thread_pin_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 409>)
-               730 MAKE_FUNCTION            0
-   
-   409         732 PRECALL                  0
-               736 CALL                     0
-   
-   410         746 STORE_NAME              60 (thread_pin_view)
-   
-   422         748 PUSH_NULL
-               750 LOAD_NAME                7 (login_required)
-               752 LOAD_CONST              20 ('/login/')
-               754 KW_NAMES                21
-               756 PRECALL                  1
-               760 CALL                     1
-   
-   423         770 LOAD_CONST              35 (<code object thread_close_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 422>)
-               772 MAKE_FUNCTION            0
-   
-   422         774 PRECALL                  0
-               778 CALL                     0
-   
-   423         788 STORE_NAME              61 (thread_close_view)
-   
-   435         790 PUSH_NULL
-               792 LOAD_NAME                7 (login_required)
-               794 LOAD_CONST              20 ('/login/')
-               796 KW_NAMES                21
-               798 PRECALL                  1
-               802 CALL                     1
-   
-   436         812 LOAD_CONST              36 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 435>)
-               814 MAKE_FUNCTION            0
-   
-   435         816 PRECALL                  0
-               820 CALL                     0
-   
-   436         830 STORE_NAME              62 (post_create_view)
-   
-   455         832 PUSH_NULL
-               834 LOAD_NAME                7 (login_required)
-               836 LOAD_CONST              20 ('/login/')
-               838 KW_NAMES                21
-               840 PRECALL                  1
-               844 CALL                     1
-   
-   456         854 LOAD_CONST              37 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 455>)
-               856 MAKE_FUNCTION            0
-   
-   455         858 PRECALL                  0
-               862 CALL                     0
-   
-   456         872 STORE_NAME              63 (post_update_view)
-   
-   480         874 PUSH_NULL
-               876 LOAD_NAME                7 (login_required)
-               878 LOAD_CONST              20 ('/login/')
-               880 KW_NAMES                21
-               882 PRECALL                  1
-               886 CALL                     1
-   
-   481         896 LOAD_CONST              38 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 480>)
-               898 MAKE_FUNCTION            0
-   
-   480         900 PRECALL                  0
-               904 CALL                     0
-   
-   481         914 STORE_NAME              64 (post_delete_view)
-   
-   499         916 LOAD_CONST              39 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 499>)
-               918 MAKE_FUNCTION            0
-               920 STORE_NAME              65 (current_shouts)
-   
-   505         922 LOAD_CONST              40 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 505>)
-               924 MAKE_FUNCTION            0
-               926 STORE_NAME              66 (shout_list_view)
-   
-   514         928 LOAD_CONST              41 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 514>)
-               930 MAKE_FUNCTION            0
-               932 STORE_NAME              67 (shout_create_view)
-   
-   537         934 PUSH_NULL
-               936 LOAD_NAME                7 (login_required)
-               938 LOAD_CONST              20 ('/login/')
-               940 KW_NAMES                21
-               942 PRECALL                  1
-               946 CALL                     1
-   
-   538         956 LOAD_CONST              42 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 537>)
-               958 MAKE_FUNCTION            0
-   
-   537         960 PRECALL                  0
-               964 CALL                     0
-   
-   538         974 STORE_NAME              68 (shout_delete_view)
-   
-   556         976 LOAD_CONST              43 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 556>)
-               978 MAKE_FUNCTION            0
-               980 STORE_NAME              69 (bbcode_view)
-               982 LOAD_CONST               1 (None)
-               984 RETURN_VALUE
+                 4 LOAD_CONST               1 (('authenticate', 'get_user_model', 'login', 'logout'))
+                 6 IMPORT_NAME              0 (django.contrib.auth)
+                 8 IMPORT_FROM              1 (authenticate)
+                10 STORE_NAME               1 (authenticate)
+                12 IMPORT_FROM              2 (get_user_model)
+                14 STORE_NAME               2 (get_user_model)
+                16 IMPORT_FROM              3 (login)
+                18 STORE_NAME               3 (login)
+                20 IMPORT_FROM              4 (logout)
+                22 STORE_NAME               4 (logout)
+                24 POP_TOP
+   
+     2          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               2 (('login_required',))
+                30 IMPORT_NAME              5 (django.contrib.auth.decorators)
+                32 IMPORT_FROM              6 (login_required)
+                34 STORE_NAME               6 (login_required)
+                36 POP_TOP
+   
+     3          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               3 (('HttpResponseForbidden',))
+                42 IMPORT_NAME              7 (django.http)
+                44 IMPORT_FROM              8 (HttpResponseForbidden)
+                46 STORE_NAME               8 (HttpResponseForbidden)
+                48 POP_TOP
+   
+     4          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               4 (('get_object_or_404', 'redirect', 'render'))
+                54 IMPORT_NAME              9 (django.shortcuts)
+                56 IMPORT_FROM             10 (get_object_or_404)
+                58 STORE_NAME              10 (get_object_or_404)
+                60 IMPORT_FROM             11 (redirect)
+                62 STORE_NAME              11 (redirect)
+                64 IMPORT_FROM             12 (render)
+                66 STORE_NAME              12 (render)
+                68 POP_TOP
+   
+     5          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('reverse',))
+                74 IMPORT_NAME             13 (django.urls)
+                76 IMPORT_FROM             14 (reverse)
+                78 STORE_NAME              14 (reverse)
+                80 POP_TOP
+   
+     6          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('timezone',))
+                86 IMPORT_NAME             15 (django.utils)
+                88 IMPORT_FROM             16 (timezone)
+                90 STORE_NAME              16 (timezone)
+                92 POP_TOP
+   
+     8          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               7 (('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm'))
+                98 IMPORT_NAME             17 (punkweb_bb.forms)
+               100 IMPORT_FROM             18 (BoardProfileModelForm)
+               102 STORE_NAME              18 (BoardProfileModelForm)
+               104 IMPORT_FROM             19 (CategoryModelForm)
+               106 STORE_NAME              19 (CategoryModelForm)
+               108 IMPORT_FROM             20 (LoginForm)
+               110 STORE_NAME              20 (LoginForm)
+               112 IMPORT_FROM             21 (PostModelForm)
+               114 STORE_NAME              21 (PostModelForm)
+               116 IMPORT_FROM             22 (ShoutModelForm)
+               118 STORE_NAME              22 (ShoutModelForm)
+               120 IMPORT_FROM             23 (SignUpForm)
+               122 STORE_NAME              23 (SignUpForm)
+               124 IMPORT_FROM             24 (SubcategoryModelForm)
+               126 STORE_NAME              24 (SubcategoryModelForm)
+               128 IMPORT_FROM             25 (ThreadModelForm)
+               130 STORE_NAME              25 (ThreadModelForm)
+               132 POP_TOP
+   
+    18         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST               8 (('guest_list',))
+               138 IMPORT_NAME             26 (punkweb_bb.guests)
+               140 IMPORT_FROM             27 (guest_list)
+               142 STORE_NAME              27 (guest_list)
+               144 POP_TOP
+   
+    19         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST               9 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
+               150 IMPORT_NAME             28 (punkweb_bb.models)
+               152 IMPORT_FROM             29 (Category)
+               154 STORE_NAME              29 (Category)
+               156 IMPORT_FROM             30 (Post)
+               158 STORE_NAME              30 (Post)
+               160 IMPORT_FROM             31 (Shout)
+               162 STORE_NAME              31 (Shout)
+               164 IMPORT_FROM             32 (Subcategory)
+               166 STORE_NAME              32 (Subcategory)
+               168 IMPORT_FROM             33 (Thread)
+               170 STORE_NAME              33 (Thread)
+               172 POP_TOP
+   
+    20         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST              10 (('paginate_qs',))
+               178 IMPORT_NAME             34 (punkweb_bb.pagination)
+               180 IMPORT_FROM             35 (paginate_qs)
+               182 STORE_NAME              35 (paginate_qs)
+               184 POP_TOP
+   
+    21         186 LOAD_CONST               0 (0)
+               188 LOAD_CONST              11 (('htmx_redirect',))
+               190 IMPORT_NAME             36 (punkweb_bb.response)
+               192 IMPORT_FROM             37 (htmx_redirect)
+               194 STORE_NAME              37 (htmx_redirect)
+               196 POP_TOP
+   
+    22         198 LOAD_CONST               0 (0)
+               200 LOAD_CONST              12 (('get_unique_slug',))
+               202 IMPORT_NAME             38 (punkweb_bb.utils)
+               204 IMPORT_FROM             39 (get_unique_slug)
+               206 STORE_NAME              39 (get_unique_slug)
+               208 POP_TOP
+   
+    24         210 PUSH_NULL
+               212 LOAD_NAME                2 (get_user_model)
+               214 PRECALL                  0
+               218 CALL                     0
+               228 STORE_NAME              40 (User)
+   
+    27         230 LOAD_CONST              13 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 27>)
+               232 MAKE_FUNCTION            0
+               234 STORE_NAME              41 (signup_view)
+   
+    47         236 LOAD_CONST              14 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 47>)
+               238 MAKE_FUNCTION            0
+               240 STORE_NAME              42 (login_view)
+   
+    73         242 LOAD_CONST              15 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 73>)
+               244 MAKE_FUNCTION            0
+               246 STORE_NAME              43 (logout_view)
+   
+    78         248 LOAD_CONST              16 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 78>)
+               250 MAKE_FUNCTION            0
+               252 STORE_NAME              44 (index_view)
+   
+   110         254 LOAD_CONST              17 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 110>)
+               256 MAKE_FUNCTION            0
+               258 STORE_NAME              45 (profile_view)
+   
+   119         260 LOAD_CONST              18 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 119>)
+               262 MAKE_FUNCTION            0
+               264 STORE_NAME              46 (members_view)
+   
+   130         266 PUSH_NULL
+               268 LOAD_NAME                6 (login_required)
+               270 LOAD_CONST              19 ('/login/')
+               272 KW_NAMES                20
+               274 PRECALL                  1
+               278 CALL                     1
+   
+   131         288 LOAD_CONST              21 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 130>)
+               290 MAKE_FUNCTION            0
+   
+   130         292 PRECALL                  0
+               296 CALL                     0
+   
+   131         306 STORE_NAME              47 (settings_view)
+   
+   153         308 PUSH_NULL
+               310 LOAD_NAME                6 (login_required)
+               312 LOAD_CONST              19 ('/login/')
+               314 KW_NAMES                20
+               316 PRECALL                  1
+               320 CALL                     1
+   
+   154         330 LOAD_CONST              22 (<code object category_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 153>)
+               332 MAKE_FUNCTION            0
+   
+   153         334 PRECALL                  0
+               338 CALL                     0
+   
+   154         348 STORE_NAME              48 (category_create_view)
+   
+   176         350 PUSH_NULL
+               352 LOAD_NAME                6 (login_required)
+               354 LOAD_CONST              19 ('/login/')
+               356 KW_NAMES                20
+               358 PRECALL                  1
+               362 CALL                     1
+   
+   177         372 LOAD_CONST              23 (<code object category_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 176>)
+               374 MAKE_FUNCTION            0
+   
+   176         376 PRECALL                  0
+               380 CALL                     0
+   
+   177         390 STORE_NAME              49 (category_update_view)
+   
+   200         392 PUSH_NULL
+               394 LOAD_NAME                6 (login_required)
+               396 LOAD_CONST              19 ('/login/')
+               398 KW_NAMES                20
+               400 PRECALL                  1
+               404 CALL                     1
+   
+   201         414 LOAD_CONST              24 (<code object category_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 200>)
+               416 MAKE_FUNCTION            0
+   
+   200         418 PRECALL                  0
+               422 CALL                     0
+   
+   201         432 STORE_NAME              50 (category_delete_view)
+   
+   219         434 LOAD_CONST              25 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 219>)
+               436 MAKE_FUNCTION            0
+               438 STORE_NAME              51 (subcategory_view)
+   
+   231         440 PUSH_NULL
+               442 LOAD_NAME                6 (login_required)
+               444 LOAD_CONST              19 ('/login/')
+               446 KW_NAMES                20
+               448 PRECALL                  1
+               452 CALL                     1
+   
+   232         462 LOAD_CONST              26 (<code object subcategory_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 231>)
+               464 MAKE_FUNCTION            0
+   
+   231         466 PRECALL                  0
+               470 CALL                     0
+   
+   232         480 STORE_NAME              52 (subcategory_create_view)
+   
+   260         482 PUSH_NULL
+               484 LOAD_NAME                6 (login_required)
+               486 LOAD_CONST              19 ('/login/')
+               488 KW_NAMES                20
+               490 PRECALL                  1
+               494 CALL                     1
+   
+   261         504 LOAD_CONST              27 (<code object subcategory_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 260>)
+               506 MAKE_FUNCTION            0
+   
+   260         508 PRECALL                  0
+               512 CALL                     0
+   
+   261         522 STORE_NAME              53 (subcategory_update_view)
+   
+   286         524 PUSH_NULL
+               526 LOAD_NAME                6 (login_required)
+               528 LOAD_CONST              19 ('/login/')
+               530 KW_NAMES                20
+               532 PRECALL                  1
+               536 CALL                     1
+   
+   287         546 LOAD_CONST              28 (<code object subcategory_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 286>)
+               548 MAKE_FUNCTION            0
+   
+   286         550 PRECALL                  0
+               554 CALL                     0
+   
+   287         564 STORE_NAME              54 (subcategory_delete_view)
+   
+   309         566 PUSH_NULL
+               568 LOAD_NAME                6 (login_required)
+               570 LOAD_CONST              19 ('/login/')
+               572 KW_NAMES                20
+               574 PRECALL                  1
+               578 CALL                     1
+   
+   310         588 LOAD_CONST              29 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 309>)
+               590 MAKE_FUNCTION            0
+   
+   309         592 PRECALL                  0
+               596 CALL                     0
+   
+   310         606 STORE_NAME              55 (thread_create_view)
+   
+   338         608 LOAD_CONST              30 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 338>)
+               610 MAKE_FUNCTION            0
+               612 STORE_NAME              56 (thread_view)
+   
+   360         614 PUSH_NULL
+               616 LOAD_NAME                6 (login_required)
+               618 LOAD_CONST              19 ('/login/')
+               620 KW_NAMES                20
+               622 PRECALL                  1
+               626 CALL                     1
+   
+   361         636 LOAD_CONST              31 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 360>)
+               638 MAKE_FUNCTION            0
+   
+   360         640 PRECALL                  0
+               644 CALL                     0
+   
+   361         654 STORE_NAME              57 (thread_update_view)
+   
+   386         656 PUSH_NULL
+               658 LOAD_NAME                6 (login_required)
+               660 LOAD_CONST              19 ('/login/')
+               662 KW_NAMES                20
+               664 PRECALL                  1
+               668 CALL                     1
+   
+   387         678 LOAD_CONST              32 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 386>)
+               680 MAKE_FUNCTION            0
+   
+   386         682 PRECALL                  0
+               686 CALL                     0
+   
+   387         696 STORE_NAME              58 (thread_delete_view)
+   
+   407         698 PUSH_NULL
+               700 LOAD_NAME                6 (login_required)
+               702 LOAD_CONST              19 ('/login/')
+               704 KW_NAMES                20
+               706 PRECALL                  1
+               710 CALL                     1
+   
+   408         720 LOAD_CONST              33 (<code object thread_pin_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 407>)
+               722 MAKE_FUNCTION            0
+   
+   407         724 PRECALL                  0
+               728 CALL                     0
+   
+   408         738 STORE_NAME              59 (thread_pin_view)
+   
+   420         740 PUSH_NULL
+               742 LOAD_NAME                6 (login_required)
+               744 LOAD_CONST              19 ('/login/')
+               746 KW_NAMES                20
+               748 PRECALL                  1
+               752 CALL                     1
+   
+   421         762 LOAD_CONST              34 (<code object thread_close_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 420>)
+               764 MAKE_FUNCTION            0
+   
+   420         766 PRECALL                  0
+               770 CALL                     0
+   
+   421         780 STORE_NAME              60 (thread_close_view)
+   
+   433         782 PUSH_NULL
+               784 LOAD_NAME                6 (login_required)
+               786 LOAD_CONST              19 ('/login/')
+               788 KW_NAMES                20
+               790 PRECALL                  1
+               794 CALL                     1
+   
+   434         804 LOAD_CONST              35 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 433>)
+               806 MAKE_FUNCTION            0
+   
+   433         808 PRECALL                  0
+               812 CALL                     0
+   
+   434         822 STORE_NAME              61 (post_create_view)
+   
+   453         824 PUSH_NULL
+               826 LOAD_NAME                6 (login_required)
+               828 LOAD_CONST              19 ('/login/')
+               830 KW_NAMES                20
+               832 PRECALL                  1
+               836 CALL                     1
+   
+   454         846 LOAD_CONST              36 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 453>)
+               848 MAKE_FUNCTION            0
+   
+   453         850 PRECALL                  0
+               854 CALL                     0
+   
+   454         864 STORE_NAME              62 (post_update_view)
+   
+   478         866 PUSH_NULL
+               868 LOAD_NAME                6 (login_required)
+               870 LOAD_CONST              19 ('/login/')
+               872 KW_NAMES                20
+               874 PRECALL                  1
+               878 CALL                     1
+   
+   479         888 LOAD_CONST              37 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 478>)
+               890 MAKE_FUNCTION            0
+   
+   478         892 PRECALL                  0
+               896 CALL                     0
+   
+   479         906 STORE_NAME              63 (post_delete_view)
+   
+   497         908 LOAD_CONST              38 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 497>)
+               910 MAKE_FUNCTION            0
+               912 STORE_NAME              64 (current_shouts)
+   
+   503         914 LOAD_CONST              39 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 503>)
+               916 MAKE_FUNCTION            0
+               918 STORE_NAME              65 (shout_list_view)
+   
+   512         920 LOAD_CONST              40 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 512>)
+               922 MAKE_FUNCTION            0
+               924 STORE_NAME              66 (shout_create_view)
+   
+   535         926 PUSH_NULL
+               928 LOAD_NAME                6 (login_required)
+               930 LOAD_CONST              19 ('/login/')
+               932 KW_NAMES                20
+               934 PRECALL                  1
+               938 CALL                     1
+   
+   536         948 LOAD_CONST              41 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 535>)
+               950 MAKE_FUNCTION            0
+   
+   535         952 PRECALL                  0
+               956 CALL                     0
+   
+   536         966 STORE_NAME              67 (shout_delete_view)
+   
+   554         968 LOAD_CONST              42 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 554>)
+               970 MAKE_FUNCTION            0
+               972 STORE_NAME              68 (bbcode_view)
+               974 LOAD_CONST              43 (None)
+               976 RETURN_VALUE
    consts
       0
-      None
       ('authenticate', 'get_user_model', 'login', 'logout')
       ('login_required',)
       ('HttpResponseForbidden',)
       ('get_object_or_404', 'redirect', 'render')
       ('reverse',)
       ('timezone',)
       ('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm')
@@ -486,72 +480,72 @@
             01a0060000000000000000000000000000000000000000a6000000ab0000
             0000000000000072237c01a0070000000000000000000000000000000000
             000000a6000000ab00000000000000000001007405000000000000000000
             006403a6010000ab01000000000000000053006e0e740900000000000000
             000000a6000000ab0000000000000000007d0164047c0169017d02741100
             0000000000000000007c0064057c02a6030000ab03000000000000000053
             00
-          29           0 RESUME                   0
+          27           0 RESUME                   0
          
-          30           2 LOAD_FAST                0 (request)
+          28           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          31          26 LOAD_GLOBAL              5 (NULL + redirect)
+          29          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          33     >>   56 LOAD_FAST                0 (request)
+          31     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE    76 (to 230)
          
-          34          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
+          32          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_ATTR                5 (POST)
                      102 PRECALL                  1
                      106 CALL                     1
                      116 STORE_FAST               1 (form)
          
-          36         118 LOAD_FAST                1 (form)
+          34         118 LOAD_FAST                1 (form)
                      120 LOAD_METHOD              6 (is_valid)
                      142 PRECALL                  0
                      146 CALL                     0
                      156 POP_JUMP_FORWARD_IF_FALSE    35 (to 228)
          
-          37         158 LOAD_FAST                1 (form)
+          35         158 LOAD_FAST                1 (form)
                      160 LOAD_METHOD              7 (save)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-          39         198 LOAD_GLOBAL              5 (NULL + redirect)
+          37         198 LOAD_GLOBAL              5 (NULL + redirect)
                      210 LOAD_CONST               3 ('punkweb_bb:login')
                      212 PRECALL                  1
                      216 CALL                     1
                      226 RETURN_VALUE
          
-          36     >>  228 JUMP_FORWARD            14 (to 258)
+          34     >>  228 JUMP_FORWARD            14 (to 258)
          
-          41     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
+          39     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
                      242 PRECALL                  0
                      246 CALL                     0
                      256 STORE_FAST               1 (form)
          
-          44     >>  258 LOAD_CONST               4 ('form')
+          42     >>  258 LOAD_CONST               4 ('form')
                      260 LOAD_FAST                1 (form)
          
-          43         262 BUILD_MAP                1
+          41         262 BUILD_MAP                1
                      264 STORE_FAST               2 (context)
          
-          46         266 LOAD_GLOBAL             17 (NULL + render)
+          44         266 LOAD_GLOBAL             17 (NULL + render)
                      278 LOAD_FAST                0 (request)
                      280 LOAD_CONST               5 ('punkweb_bb/signup.html')
                      282 LOAD_FAST                2 (context)
                      284 PRECALL                  3
                      288 CALL                     3
                      298 RETURN_VALUE
          consts
@@ -563,15 +557,15 @@
             'punkweb_bb/signup.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'SignUpForm', 'POST', 'is_valid', 'save', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'signup_view'
-         firstlineno 29
+         firstlineno 27
          lnotab 0x020118011e0216012802280128021efd02051c0304ff0403
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -584,97 +578,97 @@
             00000000007d027c016a0700000000000000006404190000000000000000
             007d037411000000000000000000007c007c027c03ac05a6030000ab0300
             000000000000007d047c04811f7413000000000000000000007c007c04a6
             020000ab02000000000000000001007405000000000000000000006401a6
             010000ab01000000000000000053006e0e740900000000000000000000a6
             000000ab0000000000000000007d0164067c0169017d0574150000000000
             00000000007c0064077c05a6030000ab0300000000000000005300
-          49           0 RESUME                   0
+          47           0 RESUME                   0
          
-          50           2 LOAD_FAST                0 (request)
+          48           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          51          26 LOAD_GLOBAL              5 (NULL + redirect)
+          49          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          53     >>   56 LOAD_FAST                0 (request)
+          51     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE   119 (to 316)
          
-          54          78 LOAD_GLOBAL              9 (NULL + LoginForm)
+          52          78 LOAD_GLOBAL              9 (NULL + LoginForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 PRECALL                  2
                      108 CALL                     2
                      118 STORE_FAST               1 (form)
          
-          56         120 LOAD_FAST                1 (form)
+          54         120 LOAD_FAST                1 (form)
                      122 LOAD_METHOD              6 (is_valid)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 POP_JUMP_FORWARD_IF_FALSE    77 (to 314)
          
-          57         160 LOAD_FAST                1 (form)
+          55         160 LOAD_FAST                1 (form)
                      162 LOAD_ATTR                7 (cleaned_data)
                      172 LOAD_CONST               3 ('username')
                      174 BINARY_SUBSCR
                      184 STORE_FAST               2 (username)
          
-          58         186 LOAD_FAST                1 (form)
+          56         186 LOAD_FAST                1 (form)
                      188 LOAD_ATTR                7 (cleaned_data)
                      198 LOAD_CONST               4 ('password')
                      200 BINARY_SUBSCR
                      210 STORE_FAST               3 (password)
          
-          60         212 LOAD_GLOBAL             17 (NULL + authenticate)
+          58         212 LOAD_GLOBAL             17 (NULL + authenticate)
                      224 LOAD_FAST                0 (request)
                      226 LOAD_FAST                2 (username)
                      228 LOAD_FAST                3 (password)
                      230 KW_NAMES                 5
                      232 PRECALL                  3
                      236 CALL                     3
                      246 STORE_FAST               4 (user)
          
-          62         248 LOAD_FAST                4 (user)
+          60         248 LOAD_FAST                4 (user)
                      250 POP_JUMP_FORWARD_IF_NONE    31 (to 314)
          
-          63         252 LOAD_GLOBAL             19 (NULL + login)
+          61         252 LOAD_GLOBAL             19 (NULL + login)
                      264 LOAD_FAST                0 (request)
                      266 LOAD_FAST                4 (user)
                      268 PRECALL                  2
                      272 CALL                     2
                      282 POP_TOP
          
-          65         284 LOAD_GLOBAL              5 (NULL + redirect)
+          63         284 LOAD_GLOBAL              5 (NULL + redirect)
                      296 LOAD_CONST               1 ('punkweb_bb:index')
                      298 PRECALL                  1
                      302 CALL                     1
                      312 RETURN_VALUE
                  >>  314 JUMP_FORWARD            14 (to 344)
          
-          67     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
+          65     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
                      328 PRECALL                  0
                      332 CALL                     0
                      342 STORE_FAST               1 (form)
          
-          70     >>  344 LOAD_CONST               6 ('form')
+          68     >>  344 LOAD_CONST               6 ('form')
                      346 LOAD_FAST                1 (form)
          
-          69         348 BUILD_MAP                1
+          67         348 BUILD_MAP                1
                      350 STORE_FAST               5 (context)
          
-          72         352 LOAD_GLOBAL             21 (NULL + render)
+          70         352 LOAD_GLOBAL             21 (NULL + render)
                      364 LOAD_FAST                0 (request)
                      366 LOAD_CONST               7 ('punkweb_bb/login.html')
                      368 LOAD_FAST                5 (context)
                      370 PRECALL                  3
                      374 CALL                     3
                      384 RETURN_VALUE
          consts
@@ -688,50 +682,50 @@
             'punkweb_bb/login.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'LoginForm', 'POST', 'is_valid', 'cleaned_data', 'authenticate', 'login', 'render')
          varnames   ('request', 'form', 'username', 'password', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'login_view'
-         firstlineno 49
+         firstlineno 47
          lnotab
             0x020118011e0216012a0228011a011a0224020401200220021c0304ff04
             03
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             0001007403000000000000000000006401a6010000ab0100000000000000
             005300
-          75           0 RESUME                   0
+          73           0 RESUME                   0
          
-          76           2 LOAD_GLOBAL              1 (NULL + logout)
+          74           2 LOAD_GLOBAL              1 (NULL + logout)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          77          32 LOAD_GLOBAL              3 (NULL + redirect)
+          75          32 LOAD_GLOBAL              3 (NULL + redirect)
                       44 LOAD_CONST               1 ('punkweb_bb:login')
                       46 PRECALL                  1
                       50 CALL                     1
                       60 RETURN_VALUE
          consts
             None
             'punkweb_bb:login'
          names      ('logout', 'redirect')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'logout_view'
-         firstlineno 75
+         firstlineno 73
          lnotab 0x02011e01
       code
          argcount  : 1
          nlocals   : 13
          stacksize : 11
          flags     : 3
          code
@@ -755,141 +749,141 @@
             0000000000000000007d08640784007c074400a6000000ab000000000000
             0000007d097415000000000000000000006a0b0000000000000000a60000
             00ab0000000000000000007d0a7419000000000000000000007c08a60100
             00ab0100000000000000007419000000000000000000007c09a6010000ab
             0100000000000000007a0000007c0a7a0000007d0b7c017c027c037c047c
             057c067c087c097c0a7c0b64089c0a7d0c741b000000000000000000007c
             0064097c0cac0aa6030000ab0300000000000000005300
-          80           0 RESUME                   0
+          78           0 RESUME                   0
          
-          81           2 LOAD_GLOBAL              0 (Category)
+          79           2 LOAD_GLOBAL              0 (Category)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (all)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               1 (categories)
          
-          83          62 LOAD_GLOBAL              6 (Thread)
+          81          62 LOAD_GLOBAL              6 (Thread)
                       74 LOAD_ATTR                1 (objects)
                       84 LOAD_METHOD              2 (all)
                      106 PRECALL                  0
                      110 CALL                     0
                      120 LOAD_METHOD              4 (order_by)
                      142 LOAD_CONST               1 ('-created_at')
                      144 PRECALL                  1
                      148 CALL                     1
                      158 LOAD_CONST               0 (None)
                      160 LOAD_CONST               2 (5)
                      162 BUILD_SLICE              2
                      164 BINARY_SUBSCR
                      174 STORE_FAST               2 (recent_threads)
          
-          85         176 LOAD_GLOBAL              6 (Thread)
+          83         176 LOAD_GLOBAL              6 (Thread)
                      188 LOAD_ATTR                1 (objects)
                      198 LOAD_METHOD              5 (count)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 STORE_FAST               3 (thread_count)
          
-          86         236 LOAD_GLOBAL             12 (Post)
+          84         236 LOAD_GLOBAL             12 (Post)
                      248 LOAD_ATTR                1 (objects)
                      258 LOAD_METHOD              5 (count)
                      280 PRECALL                  0
                      284 CALL                     0
                      294 STORE_FAST               4 (post_count)
          
-          88         296 LOAD_GLOBAL             14 (User)
+          86         296 LOAD_GLOBAL             14 (User)
                      308 LOAD_ATTR                1 (objects)
                      318 LOAD_METHOD              8 (select_related)
                      340 LOAD_CONST               3 ('profile')
                      342 PRECALL                  1
                      346 CALL                     1
                      356 LOAD_METHOD              2 (all)
                      378 PRECALL                  0
                      382 CALL                     0
                      392 STORE_FAST               5 (users)
          
-          89         394 LOAD_FAST                5 (users)
+          87         394 LOAD_FAST                5 (users)
                      396 LOAD_METHOD              4 (order_by)
                      418 LOAD_CONST               4 ('-profile__created_at')
                      420 PRECALL                  1
                      424 CALL                     1
                      434 LOAD_METHOD              9 (first)
                      456 PRECALL                  0
                      460 CALL                     0
                      470 STORE_FAST               6 (newest_user)
          
-          91         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 91>)
+          89         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 89>)
                      474 MAKE_FUNCTION            0
                      476 LOAD_FAST                5 (users)
                      478 GET_ITER
                      480 PRECALL                  0
                      484 CALL                     0
                      494 STORE_FAST               7 (users_online)
          
-          92         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 92>)
+          90         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 90>)
                      498 MAKE_FUNCTION            0
                      500 LOAD_FAST                7 (users_online)
                      502 GET_ITER
                      504 PRECALL                  0
                      508 CALL                     0
                      518 STORE_FAST               8 (members_online)
          
-          93         520 LOAD_CONST               7 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 93>)
+          91         520 LOAD_CONST               7 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 91>)
                      522 MAKE_FUNCTION            0
                      524 LOAD_FAST                7 (users_online)
                      526 GET_ITER
                      528 PRECALL                  0
                      532 CALL                     0
                      542 STORE_FAST               9 (staff_online)
          
-          94         544 LOAD_GLOBAL             21 (NULL + guest_list)
+          92         544 LOAD_GLOBAL             21 (NULL + guest_list)
                      556 LOAD_ATTR               11 (length)
                      566 PRECALL                  0
                      570 CALL                     0
                      580 STORE_FAST              10 (guests_online)
          
-          95         582 LOAD_GLOBAL             25 (NULL + len)
+          93         582 LOAD_GLOBAL             25 (NULL + len)
                      594 LOAD_FAST                8 (members_online)
                      596 PRECALL                  1
                      600 CALL                     1
                      610 LOAD_GLOBAL             25 (NULL + len)
                      622 LOAD_FAST                9 (staff_online)
                      624 PRECALL                  1
                      628 CALL                     1
                      638 BINARY_OP                0 (+)
                      642 LOAD_FAST               10 (guests_online)
                      644 BINARY_OP                0 (+)
                      648 STORE_FAST              11 (total_online)
          
-          98         650 LOAD_FAST                1 (categories)
+          96         650 LOAD_FAST                1 (categories)
          
-          99         652 LOAD_FAST                2 (recent_threads)
+          97         652 LOAD_FAST                2 (recent_threads)
          
-         100         654 LOAD_FAST                3 (thread_count)
+          98         654 LOAD_FAST                3 (thread_count)
          
-         101         656 LOAD_FAST                4 (post_count)
+          99         656 LOAD_FAST                4 (post_count)
          
-         102         658 LOAD_FAST                5 (users)
+         100         658 LOAD_FAST                5 (users)
          
-         103         660 LOAD_FAST                6 (newest_user)
+         101         660 LOAD_FAST                6 (newest_user)
          
-         104         662 LOAD_FAST                8 (members_online)
+         102         662 LOAD_FAST                8 (members_online)
          
-         105         664 LOAD_FAST                9 (staff_online)
+         103         664 LOAD_FAST                9 (staff_online)
          
-         106         666 LOAD_FAST               10 (guests_online)
+         104         666 LOAD_FAST               10 (guests_online)
          
-         107         668 LOAD_FAST               11 (total_online)
+         105         668 LOAD_FAST               11 (total_online)
          
-          97         670 LOAD_CONST               8 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online'))
+          95         670 LOAD_CONST               8 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online'))
                      672 BUILD_CONST_KEY_MAP     10
                      674 STORE_FAST              12 (context)
          
-         109         676 LOAD_GLOBAL             27 (NULL + render)
+         107         676 LOAD_GLOBAL             27 (NULL + render)
                      688 LOAD_FAST                0 (request)
                      690 LOAD_CONST               9 ('punkweb_bb/index.html')
                      692 LOAD_FAST               12 (context)
                      694 KW_NAMES                10
                      696 PRECALL                  3
                      700 CALL                     3
                      710 RETURN_VALUE
@@ -903,15 +897,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d107d017c016a0000000000000000006a010000000000
                   000000af0e7c0191028c115300
-                91           0 RESUME                   0
+                89           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                16 (to 40)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (profile)
                             22 LOAD_ATTR                1 (is_online)
@@ -923,25 +917,25 @@
                consts
                names      ('profile', 'is_online')
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 91
+               firstlineno 89
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d0b7d017c016a000000000000000000b0097c0191028c
                   0c5300
-                92           0 RESUME                   0
+                90           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                11 (to 30)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (is_staff)
                             22 POP_JUMP_BACKWARD_IF_TRUE     9 (to 6)
@@ -952,25 +946,25 @@
                consts
                names      ('is_staff',)
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 92
+               firstlineno 90
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d0b7d017c016a000000000000000000af097c0191028c
                   0c5300
-                93           0 RESUME                   0
+                91           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                11 (to 30)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (is_staff)
                             22 POP_JUMP_BACKWARD_IF_FALSE     9 (to 6)
@@ -981,56 +975,56 @@
                consts
                names      ('is_staff',)
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 93
+               firstlineno 91
                lnotab 0x
             ('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online')
             'punkweb_bb/index.html'
             ('context',)
          names      ('Category', 'objects', 'all', 'Thread', 'order_by', 'count', 'Post', 'User', 'select_related', 'first', 'guest_list', 'length', 'len', 'render')
          varnames   ('request', 'categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'users_online', 'members_online', 'staff_online', 'guests_online', 'total_online', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'index_view'
-         firstlineno 80
+         firstlineno 78
          lnotab
             0x02013c0272023c013c0262014e02180118011801260144030201020102
             0102010201020102010201020102f6060c
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d0264027c0269017d037405000000
             000000000000007c0064037c03ac04a6030000ab03000000000000000053
             00
-         112           0 RESUME                   0
+         110           0 RESUME                   0
          
-         113           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         111           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (User)
                       26 LOAD_FAST                1 (user_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (user)
          
-         116          46 LOAD_CONST               2 ('user')
+         114          46 LOAD_CONST               2 ('user')
                       48 LOAD_FAST                2 (user)
          
-         115          50 BUILD_MAP                1
+         113          50 BUILD_MAP                1
                       52 STORE_FAST               3 (context)
          
-         118          54 LOAD_GLOBAL              5 (NULL + render)
+         116          54 LOAD_GLOBAL              5 (NULL + render)
                       66 LOAD_FAST                0 (request)
                       68 LOAD_CONST               3 ('punkweb_bb/profile.html')
                       70 LOAD_FAST                3 (context)
                       72 KW_NAMES                 4
                       74 PRECALL                  3
                       78 CALL                     3
                       88 RETURN_VALUE
@@ -1042,55 +1036,55 @@
             ('context',)
          names      ('get_object_or_404', 'User', 'render')
          varnames   ('request', 'user_id', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'profile_view'
-         firstlineno 112
+         firstlineno 110
          lnotab 0x02012c0304ff0403
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c007402000000000000000000006a
             020000000000000000a00300000000000000000000000000000000000000
             006401a6010000ab010000000000000000a0040000000000000000000000
             0000000000000000006402a6010000ab010000000000000000a6020000ab
             0200000000000000007d0164037c0169017d02740b000000000000000000
             007c0064047c02ac05a6030000ab0300000000000000005300
-         121           0 RESUME                   0
+         119           0 RESUME                   0
          
-         122           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
+         120           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
          
-         123          14 LOAD_FAST                0 (request)
+         121          14 LOAD_FAST                0 (request)
                       16 LOAD_GLOBAL              2 (User)
                       28 LOAD_ATTR                2 (objects)
                       38 LOAD_METHOD              3 (select_related)
                       60 LOAD_CONST               1 ('profile')
                       62 PRECALL                  1
                       66 CALL                     1
                       76 LOAD_METHOD              4 (order_by)
                       98 LOAD_CONST               2 ('username')
                      100 PRECALL                  1
                      104 CALL                     1
          
-         122         114 PRECALL                  2
+         120         114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (users)
          
-         127         130 LOAD_CONST               3 ('users')
+         125         130 LOAD_CONST               3 ('users')
                      132 LOAD_FAST                1 (users)
          
-         126         134 BUILD_MAP                1
+         124         134 BUILD_MAP                1
                      136 STORE_FAST               2 (context)
          
-         129         138 LOAD_GLOBAL             11 (NULL + render)
+         127         138 LOAD_GLOBAL             11 (NULL + render)
                      150 LOAD_FAST                0 (request)
                      152 LOAD_CONST               4 ('punkweb_bb/members.html')
                      154 LOAD_FAST                2 (context)
                      156 KW_NAMES                 5
                      158 PRECALL                  3
                      162 CALL                     3
                      172 RETURN_VALUE
@@ -1103,15 +1097,15 @@
             ('context',)
          names      ('paginate_qs', 'User', 'objects', 'select_related', 'order_by', 'render')
          varnames   ('request', 'users', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'members_view'
-         firstlineno 121
+         firstlineno 119
          lnotab 0x02010c0164ff100504ff0403
       '/login/'
       ('login_url',)
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -1125,82 +1119,82 @@
             000000000000000000000000000000a6000000ab00000000000000000001
             007411000000000000000000006403a6010000ab01000000000000000053
             007413000000000000000000007c00640464057c016901ac06a6030000ab
             03000000000000000053007403000000000000000000007c006a04000000
             00000000006a050000000000000000ac02a6010000ab0100000000000000
             007d0164057c0169017d027413000000000000000000007c0064047c02ac
             06a6030000ab0300000000000000005300
-         132           0 RESUME                   0
+         130           0 RESUME                   0
          
-         134           2 LOAD_FAST                0 (request)
+         132           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('POST')
                       16 COMPARE_OP               2 (==)
                       22 POP_JUMP_FORWARD_IF_FALSE   113 (to 250)
          
-         135          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         133          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
          
-         136          36 LOAD_FAST                0 (request)
+         134          36 LOAD_FAST                0 (request)
                       38 LOAD_ATTR                2 (POST)
                       48 LOAD_FAST                0 (request)
                       50 LOAD_ATTR                3 (FILES)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                4 (user)
                       72 LOAD_ATTR                5 (profile)
          
-         135          82 KW_NAMES                 2
+         133          82 KW_NAMES                 2
                       84 PRECALL                  3
                       88 CALL                     3
                       98 STORE_FAST               1 (form)
          
-         139         100 LOAD_FAST                1 (form)
+         137         100 LOAD_FAST                1 (form)
                      102 LOAD_METHOD              6 (is_valid)
                      124 PRECALL                  0
                      128 CALL                     0
                      138 POP_JUMP_FORWARD_IF_FALSE    35 (to 210)
          
-         140         140 LOAD_FAST                1 (form)
+         138         140 LOAD_FAST                1 (form)
                      142 LOAD_METHOD              7 (save)
                      164 PRECALL                  0
                      168 CALL                     0
                      178 POP_TOP
          
-         142         180 LOAD_GLOBAL             17 (NULL + redirect)
+         140         180 LOAD_GLOBAL             17 (NULL + redirect)
                      192 LOAD_CONST               3 ('punkweb_bb:settings')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RETURN_VALUE
          
-         144     >>  210 LOAD_GLOBAL             19 (NULL + render)
+         142     >>  210 LOAD_GLOBAL             19 (NULL + render)
                      222 LOAD_FAST                0 (request)
                      224 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      226 LOAD_CONST               5 ('form')
                      228 LOAD_FAST                1 (form)
                      230 BUILD_MAP                1
                      232 KW_NAMES                 6
                      234 PRECALL                  3
                      238 CALL                     3
                      248 RETURN_VALUE
          
-         146     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         144     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
                      262 LOAD_FAST                0 (request)
                      264 LOAD_ATTR                4 (user)
                      274 LOAD_ATTR                5 (profile)
                      284 KW_NAMES                 2
                      286 PRECALL                  1
                      290 CALL                     1
                      300 STORE_FAST               1 (form)
          
-         149         302 LOAD_CONST               5 ('form')
+         147         302 LOAD_CONST               5 ('form')
                      304 LOAD_FAST                1 (form)
          
-         148         306 BUILD_MAP                1
+         146         306 BUILD_MAP                1
                      308 STORE_FAST               2 (context)
          
-         152         310 LOAD_GLOBAL             19 (NULL + render)
+         150         310 LOAD_GLOBAL             19 (NULL + render)
                      322 LOAD_FAST                0 (request)
                      324 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      326 LOAD_FAST                2 (context)
                      328 KW_NAMES                 6
                      330 PRECALL                  3
                      334 CALL                     3
                      344 RETURN_VALUE
@@ -1214,15 +1208,15 @@
             ('context',)
          names      ('method', 'BoardProfileModelForm', 'POST', 'FILES', 'user', 'profile', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'settings_view'
-         firstlineno 132
+         firstlineno 130
          lnotab 0x020216010c012eff1204280128021e022802340304ff0404
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1237,92 +1231,92 @@
             0000007412000000000000000000007c026a0a0000000000000000a60200
             00ab0200000000000000007c025f0b00000000000000007c02a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0001007419000000000000000000007c02a6010000ab0100000000000000
             0053006e0e740900000000000000000000a6000000ab0000000000000000
             007d0164067c0169017d03741b000000000000000000007c0064077c03ac
             08a6030000ab0300000000000000005300
-         155           0 RESUME                   0
+         153           0 RESUME                   0
          
-         157           2 LOAD_FAST                0 (request)
+         155           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.add_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         158          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         156          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to create categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         160     >>   84 LOAD_FAST                0 (request)
+         158     >>   84 LOAD_FAST                0 (request)
                       86 LOAD_ATTR                3 (method)
                       96 LOAD_CONST               3 ('POST')
                       98 COMPARE_OP               2 (==)
                      104 POP_JUMP_FORWARD_IF_FALSE   129 (to 364)
          
-         161         106 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
+         159         106 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
                      118 LOAD_FAST                0 (request)
                      120 LOAD_ATTR                5 (POST)
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_FAST               1 (form)
          
-         163         146 LOAD_FAST                1 (form)
+         161         146 LOAD_FAST                1 (form)
                      148 LOAD_METHOD              6 (is_valid)
                      170 PRECALL                  0
                      174 CALL                     0
                      184 POP_JUMP_FORWARD_IF_FALSE    88 (to 362)
          
-         164         186 LOAD_FAST                1 (form)
+         162         186 LOAD_FAST                1 (form)
                      188 LOAD_METHOD              7 (save)
                      210 LOAD_CONST               4 (False)
                      212 KW_NAMES                 5
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (category)
          
-         165         230 LOAD_GLOBAL             17 (NULL + get_unique_slug)
+         163         230 LOAD_GLOBAL             17 (NULL + get_unique_slug)
                      242 LOAD_GLOBAL             18 (Category)
                      254 LOAD_FAST                2 (category)
                      256 LOAD_ATTR               10 (name)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 LOAD_FAST                2 (category)
                      282 STORE_ATTR              11 (slug)
          
-         166         292 LOAD_FAST                2 (category)
+         164         292 LOAD_FAST                2 (category)
                      294 LOAD_METHOD              7 (save)
                      316 PRECALL                  0
                      320 CALL                     0
                      330 POP_TOP
          
-         168         332 LOAD_GLOBAL             25 (NULL + redirect)
+         166         332 LOAD_GLOBAL             25 (NULL + redirect)
                      344 LOAD_FAST                2 (category)
                      346 PRECALL                  1
                      350 CALL                     1
                      360 RETURN_VALUE
          
-         163     >>  362 JUMP_FORWARD            14 (to 392)
+         161     >>  362 JUMP_FORWARD            14 (to 392)
          
-         170     >>  364 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
+         168     >>  364 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
                      376 PRECALL                  0
                      380 CALL                     0
                      390 STORE_FAST               1 (form)
          
-         173     >>  392 LOAD_CONST               6 ('form')
+         171     >>  392 LOAD_CONST               6 ('form')
                      394 LOAD_FAST                1 (form)
          
-         172         396 BUILD_MAP                1
+         170         396 BUILD_MAP                1
                      398 STORE_FAST               3 (context)
          
-         175         400 LOAD_GLOBAL             27 (NULL + render)
+         173         400 LOAD_GLOBAL             27 (NULL + render)
                      412 LOAD_FAST                0 (request)
                      414 LOAD_CONST               7 ('punkweb_bb/category_create.html')
                      416 LOAD_FAST                3 (context)
                      418 KW_NAMES                 8
                      420 PRECALL                  3
                      424 CALL                     3
                      434 RETURN_VALUE
@@ -1338,15 +1332,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'method', 'CategoryModelForm', 'POST', 'is_valid', 'save', 'get_unique_slug', 'Category', 'name', 'slug', 'redirect', 'render')
          varnames   ('request', 'form', 'category', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_create_view'
-         firstlineno 155
+         firstlineno 153
          lnotab 0x020234011e021601280228012c013e0128021efb02071c0304ff0403
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1359,89 +1353,89 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac05a6010000ab0100
             000000000000007d037c027c0364069c027d047417000000000000000000
             007c0064077c04ac08a6030000ab0300000000000000005300
-         178           0 RESUME                   0
+         176           0 RESUME                   0
          
-         180           2 LOAD_FAST                0 (request)
+         178           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.change_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         181          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         179          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to change categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         183     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         181     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         185         128 LOAD_FAST                0 (request)
+         183         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         186         150 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
+         184         150 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (category)
                      176 KW_NAMES                 5
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         188         194 LOAD_FAST                3 (form)
+         186         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         189         234 LOAD_FAST                3 (form)
+         187         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (category)
          
-         191         274 LOAD_GLOBAL             21 (NULL + redirect)
+         189         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (category)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         188     >>  304 JUMP_FORWARD            16 (to 338)
+         186     >>  304 JUMP_FORWARD            16 (to 338)
          
-         193     >>  306 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
+         191     >>  306 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
                      318 LOAD_FAST                2 (category)
                      320 KW_NAMES                 5
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         196     >>  338 LOAD_FAST                2 (category)
+         194     >>  338 LOAD_FAST                2 (category)
          
-         197         340 LOAD_FAST                3 (form)
+         195         340 LOAD_FAST                3 (form)
          
-         195         342 LOAD_CONST               6 (('category', 'form'))
+         193         342 LOAD_CONST               6 (('category', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         199         348 LOAD_GLOBAL             23 (NULL + render)
+         197         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               7 ('punkweb_bb/category_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 8
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -1457,15 +1451,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'CategoryModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'category_slug', 'category', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_update_view'
-         firstlineno 178
+         firstlineno 176
          lnotab 0x020234011e022c0216012c02280128021efd02052003020102fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1475,66 +1469,66 @@
             000000000000007408000000000000000000007c01ac03a6020000ab0200
             000000000000007d027c006a05000000000000000064046b020000000072
             307c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f0000000000000000000074110000000000
             00000000006405a6010000ab010000000000000000a6010000ab01000000
             0000000000530064067c0269017d037413000000000000000000007c0064
             077c03ac08a6030000ab0300000000000000005300
-         202           0 RESUME                   0
+         200           0 RESUME                   0
          
-         204           2 LOAD_FAST                0 (request)
+         202           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.delete_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         205          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         203          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to delete categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         207     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         205     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         209         128 LOAD_FAST                0 (request)
+         207         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    48 (to 246)
          
-         210         150 LOAD_FAST                2 (category)
+         208         150 LOAD_FAST                2 (category)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         212         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         210         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_GLOBAL             17 (NULL + reverse)
                      214 LOAD_CONST               5 ('punkweb_bb:index')
                      216 PRECALL                  1
                      220 CALL                     1
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         215     >>  246 LOAD_CONST               6 ('category')
+         213     >>  246 LOAD_CONST               6 ('category')
                      248 LOAD_FAST                2 (category)
          
-         214         250 BUILD_MAP                1
+         212         250 BUILD_MAP                1
                      252 STORE_FAST               3 (context)
          
-         218         254 LOAD_GLOBAL             19 (NULL + render)
+         216         254 LOAD_GLOBAL             19 (NULL + render)
                      266 LOAD_FAST                0 (request)
                      268 LOAD_CONST               7 ('punkweb_bb/partials/category_delete.html')
                      270 LOAD_FAST                3 (context)
                      272 KW_NAMES                 8
                      274 PRECALL                  3
                      278 CALL                     3
                      288 RETURN_VALUE
@@ -1550,58 +1544,58 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'delete', 'htmx_redirect', 'reverse', 'render')
          varnames   ('request', 'category_slug', 'category', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_delete_view'
-         firstlineno 202
+         firstlineno 200
          lnotab 0x020234011e022c0216012802380304ff0404
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d027405000000000000000000007c
             007c026a030000000000000000a004000000000000000000000000000000
             0000000000a6000000ab000000000000000000a6020000ab020000000000
             0000007d037c027c0364029c027d04740b000000000000000000007c0064
             037c04ac04a6030000ab0300000000000000005300
-         221           0 RESUME                   0
+         219           0 RESUME                   0
          
-         222           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         220           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         224          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         222          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (subcategory)
                       62 LOAD_ATTR                3 (threads)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (threads)
          
-         227         124 LOAD_FAST                2 (subcategory)
+         225         124 LOAD_FAST                2 (subcategory)
          
-         228         126 LOAD_FAST                3 (threads)
+         226         126 LOAD_FAST                3 (threads)
          
-         226         128 LOAD_CONST               2 (('subcategory', 'threads'))
+         224         128 LOAD_CONST               2 (('subcategory', 'threads'))
                      130 BUILD_CONST_KEY_MAP      2
                      132 STORE_FAST               4 (context)
          
-         230         134 LOAD_GLOBAL             11 (NULL + render)
+         228         134 LOAD_GLOBAL             11 (NULL + render)
                      146 LOAD_FAST                0 (request)
                      148 LOAD_CONST               3 ('punkweb_bb/subcategory.html')
                      150 LOAD_FAST                4 (context)
                      152 KW_NAMES                 4
                      154 PRECALL                  3
                      158 CALL                     3
                      168 RETURN_VALUE
@@ -1613,15 +1607,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'paginate_qs', 'threads', 'all', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_view'
-         firstlineno 221
+         firstlineno 219
          lnotab 0x02012c024e03020102fe0604
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1638,108 +1632,108 @@
             007418000000000000000000007c046a0d0000000000000000a6020000ab
             0200000000000000007c045f0e00000000000000007c04a0090000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00741f000000000000000000007c04a6010000ab01000000000000000053
             006e0e740d00000000000000000000a6000000ab0000000000000000007d
             037c027c0364079c027d057421000000000000000000007c0064087c05ac
             09a6030000ab0300000000000000005300
-         233           0 RESUME                   0
+         231           0 RESUME                   0
          
-         235           2 LOAD_FAST                0 (request)
+         233           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.add_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         236          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         234          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         237          66 LOAD_CONST               2 ('You do not have permission to create subcategories.')
+         235          66 LOAD_CONST               2 ('You do not have permission to create subcategories.')
          
-         236          68 PRECALL                  1
+         234          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         240     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         238     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         242         128 LOAD_FAST                0 (request)
+         240         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE   136 (to 422)
          
-         243         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         241         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 STORE_FAST               3 (form)
          
-         245         190 LOAD_FAST                3 (form)
+         243         190 LOAD_FAST                3 (form)
                      192 LOAD_METHOD              8 (is_valid)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 POP_JUMP_FORWARD_IF_FALSE    95 (to 420)
          
-         246         230 LOAD_FAST                3 (form)
+         244         230 LOAD_FAST                3 (form)
                      232 LOAD_METHOD              9 (save)
                      254 LOAD_CONST               5 (False)
                      256 KW_NAMES                 6
                      258 PRECALL                  1
                      262 CALL                     1
                      272 STORE_FAST               4 (subcategory)
          
-         247         274 LOAD_FAST                2 (category)
+         245         274 LOAD_FAST                2 (category)
                      276 LOAD_FAST                4 (subcategory)
                      278 STORE_ATTR              10 (category)
          
-         248         288 LOAD_GLOBAL             23 (NULL + get_unique_slug)
+         246         288 LOAD_GLOBAL             23 (NULL + get_unique_slug)
                      300 LOAD_GLOBAL             24 (Subcategory)
                      312 LOAD_FAST                4 (subcategory)
                      314 LOAD_ATTR               13 (name)
                      324 PRECALL                  2
                      328 CALL                     2
                      338 LOAD_FAST                4 (subcategory)
                      340 STORE_ATTR              14 (slug)
          
-         249         350 LOAD_FAST                4 (subcategory)
+         247         350 LOAD_FAST                4 (subcategory)
                      352 LOAD_METHOD              9 (save)
                      374 PRECALL                  0
                      378 CALL                     0
                      388 POP_TOP
          
-         251         390 LOAD_GLOBAL             31 (NULL + redirect)
+         249         390 LOAD_GLOBAL             31 (NULL + redirect)
                      402 LOAD_FAST                4 (subcategory)
                      404 PRECALL                  1
                      408 CALL                     1
                      418 RETURN_VALUE
          
-         245     >>  420 JUMP_FORWARD            14 (to 450)
+         243     >>  420 JUMP_FORWARD            14 (to 450)
          
-         253     >>  422 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         251     >>  422 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      434 PRECALL                  0
                      438 CALL                     0
                      448 STORE_FAST               3 (form)
          
-         256     >>  450 LOAD_FAST                2 (category)
+         254     >>  450 LOAD_FAST                2 (category)
          
-         257         452 LOAD_FAST                3 (form)
+         255         452 LOAD_FAST                3 (form)
          
-         255         454 LOAD_CONST               7 (('category', 'form'))
+         253         454 LOAD_CONST               7 (('category', 'form'))
                      456 BUILD_CONST_KEY_MAP      2
                      458 STORE_FAST               5 (context)
          
-         259         460 LOAD_GLOBAL             33 (NULL + render)
+         257         460 LOAD_GLOBAL             33 (NULL + render)
                      472 LOAD_FAST                0 (request)
                      474 LOAD_CONST               8 ('punkweb_bb/subcategory_create.html')
                      476 LOAD_FAST                5 (context)
                      478 KW_NAMES                 9
                      480 PRECALL                  3
                      484 CALL                     3
                      494 RETURN_VALUE
@@ -1756,15 +1750,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'SubcategoryModelForm', 'POST', 'is_valid', 'save', 'category', 'get_unique_slug', 'Subcategory', 'name', 'slug', 'redirect', 'render')
          varnames   ('request', 'category_slug', 'category', 'form', 'subcategory', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_create_view'
-         firstlineno 233
+         firstlineno 231
          lnotab
             0x020234010c0102ff10042c021601280228012c010e013e0128021efa02
             081c03020102fe0604
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
@@ -1779,91 +1773,91 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac05a6010000ab0100
             000000000000007d037c027c0364069c027d047417000000000000000000
             007c0064077c04ac08a6030000ab0300000000000000005300
-         262           0 RESUME                   0
+         260           0 RESUME                   0
          
-         264           2 LOAD_FAST                0 (request)
+         262           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.change_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         265          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         263          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         266          66 LOAD_CONST               2 ('You do not have permission to change subcategories.')
+         264          66 LOAD_CONST               2 ('You do not have permission to change subcategories.')
          
-         265          68 PRECALL                  1
+         263          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         269     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         267     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Subcategory)
                      108 LOAD_FAST                1 (subcategory_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (subcategory)
          
-         271         128 LOAD_FAST                0 (request)
+         269         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         272         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         270         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (subcategory)
                      176 KW_NAMES                 5
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         274         194 LOAD_FAST                3 (form)
+         272         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         275         234 LOAD_FAST                3 (form)
+         273         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (subcategory)
          
-         277         274 LOAD_GLOBAL             21 (NULL + redirect)
+         275         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (subcategory)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         274     >>  304 JUMP_FORWARD            16 (to 338)
+         272     >>  304 JUMP_FORWARD            16 (to 338)
          
-         279     >>  306 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         277     >>  306 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      318 LOAD_FAST                2 (subcategory)
                      320 KW_NAMES                 5
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         282     >>  338 LOAD_FAST                2 (subcategory)
+         280     >>  338 LOAD_FAST                2 (subcategory)
          
-         283         340 LOAD_FAST                3 (form)
+         281         340 LOAD_FAST                3 (form)
          
-         281         342 LOAD_CONST               6 (('subcategory', 'form'))
+         279         342 LOAD_CONST               6 (('subcategory', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         285         348 LOAD_GLOBAL             23 (NULL + render)
+         283         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               7 ('punkweb_bb/subcategory_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 8
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -1879,15 +1873,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Subcategory', 'method', 'SubcategoryModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_update_view'
-         firstlineno 262
+         firstlineno 260
          lnotab
             0x020234010c0102ff10042c0216012c02280128021efd02052003020102
             fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -1900,75 +1894,75 @@
             000000000000007d027c006a05000000000000000064046b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064057c
             0269017d037415000000000000000000007c0064067c03ac07a6030000ab
             0300000000000000005300
-         288           0 RESUME                   0
+         286           0 RESUME                   0
          
-         290           2 LOAD_FAST                0 (request)
+         288           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.delete_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         291          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         289          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         292          66 LOAD_CONST               2 ('You do not have permission to delete subcategories.')
+         290          66 LOAD_CONST               2 ('You do not have permission to delete subcategories.')
          
-         291          68 PRECALL                  1
+         289          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         295     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         293     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Subcategory)
                      108 LOAD_FAST                1 (subcategory_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (subcategory)
          
-         297         128 LOAD_FAST                0 (request)
+         295         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         298         150 LOAD_FAST                2 (subcategory)
+         296         150 LOAD_FAST                2 (subcategory)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         300         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         298         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (subcategory)
                      204 LOAD_ATTR                8 (category)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         303     >>  266 LOAD_CONST               5 ('subcategory')
+         301     >>  266 LOAD_CONST               5 ('subcategory')
                      268 LOAD_FAST                2 (subcategory)
          
-         302         270 BUILD_MAP                1
+         300         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         306         274 LOAD_GLOBAL             21 (NULL + render)
+         304         274 LOAD_GLOBAL             21 (NULL + render)
          
-         307         286 LOAD_FAST                0 (request)
+         305         286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               6 ('punkweb_bb/partials/subcategory_delete.html')
                      290 LOAD_FAST                3 (context)
          
-         306         292 KW_NAMES                 7
+         304         292 KW_NAMES                 7
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
          consts
             None
             'punkweb_bb.delete_subcategory'
             'You do not have permission to delete subcategories.'
@@ -1979,15 +1973,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Subcategory', 'method', 'delete', 'htmx_redirect', 'category', 'get_absolute_url', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_delete_view'
-         firstlineno 288
+         firstlineno 286
          lnotab 0x020234010c0102ff10042c02160128024c0304ff04040c0106ff
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -2003,104 +1997,104 @@
             0000007d047c027c045f0a00000000000000007c006a0300000000000000
             007c045f0300000000000000007c04a00900000000000000000000000000
             00000000000000a6000000ab000000000000000000010074170000000000
             00000000007c04a6010000ab01000000000000000053006e0e740d000000
             00000000000000a6000000ab0000000000000000007d037c027c0364069c
             027d057419000000000000000000007c0064077c05ac08a6030000ab0300
             000000000000005300
-         311           0 RESUME                   0
+         309           0 RESUME                   0
          
-         313           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         311           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         315          46 LOAD_FAST                2 (subcategory)
+         313          46 LOAD_FAST                2 (subcategory)
                       48 LOAD_METHOD              2 (can_post)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         316          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         314          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         317         110 LOAD_CONST               2 ('You do not have permission to post in this subcategory.')
+         315         110 LOAD_CONST               2 ('You do not have permission to post in this subcategory.')
          
-         316         112 PRECALL                  1
+         314         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         320     >>  128 LOAD_FAST                0 (request)
+         318     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE   117 (to 384)
          
-         321         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         319         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 STORE_FAST               3 (form)
          
-         323         190 LOAD_FAST                3 (form)
+         321         190 LOAD_FAST                3 (form)
                      192 LOAD_METHOD              8 (is_valid)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 POP_JUMP_FORWARD_IF_FALSE    76 (to 382)
          
-         324         230 LOAD_FAST                3 (form)
+         322         230 LOAD_FAST                3 (form)
                      232 LOAD_METHOD              9 (save)
                      254 LOAD_CONST               4 (False)
                      256 KW_NAMES                 5
                      258 PRECALL                  1
                      262 CALL                     1
                      272 STORE_FAST               4 (thread)
          
-         325         274 LOAD_FAST                2 (subcategory)
+         323         274 LOAD_FAST                2 (subcategory)
                      276 LOAD_FAST                4 (thread)
                      278 STORE_ATTR              10 (subcategory)
          
-         326         288 LOAD_FAST                0 (request)
+         324         288 LOAD_FAST                0 (request)
                      290 LOAD_ATTR                3 (user)
                      300 LOAD_FAST                4 (thread)
                      302 STORE_ATTR               3 (user)
          
-         327         312 LOAD_FAST                4 (thread)
+         325         312 LOAD_FAST                4 (thread)
                      314 LOAD_METHOD              9 (save)
                      336 PRECALL                  0
                      340 CALL                     0
                      350 POP_TOP
          
-         329         352 LOAD_GLOBAL             23 (NULL + redirect)
+         327         352 LOAD_GLOBAL             23 (NULL + redirect)
                      364 LOAD_FAST                4 (thread)
                      366 PRECALL                  1
                      370 CALL                     1
                      380 RETURN_VALUE
          
-         323     >>  382 JUMP_FORWARD            14 (to 412)
+         321     >>  382 JUMP_FORWARD            14 (to 412)
          
-         331     >>  384 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         329     >>  384 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      396 PRECALL                  0
                      400 CALL                     0
                      410 STORE_FAST               3 (form)
          
-         334     >>  412 LOAD_FAST                2 (subcategory)
+         332     >>  412 LOAD_FAST                2 (subcategory)
          
-         335         414 LOAD_FAST                3 (form)
+         333         414 LOAD_FAST                3 (form)
          
-         333         416 LOAD_CONST               6 (('subcategory', 'form'))
+         331         416 LOAD_CONST               6 (('subcategory', 'form'))
                      418 BUILD_CONST_KEY_MAP      2
                      420 STORE_FAST               5 (context)
          
-         337         422 LOAD_GLOBAL             25 (NULL + render)
+         335         422 LOAD_GLOBAL             25 (NULL + render)
                      434 LOAD_FAST                0 (request)
                      436 LOAD_CONST               7 ('punkweb_bb/thread_create.html')
                      438 LOAD_FAST                5 (context)
                      440 KW_NAMES                 8
                      442 PRECALL                  3
                      446 CALL                     3
                      456 RETURN_VALUE
@@ -2116,15 +2110,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'can_post', 'user', 'HttpResponseForbidden', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'subcategory', 'redirect', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_create_view'
-         firstlineno 311
+         firstlineno 309
          lnotab
             0x02022c0234010c0102ff10041601280228012c010e01180128021efa02
             081c03020102fe0604
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 5
@@ -2139,88 +2133,88 @@
             0000000000000064026700a6020000ab0200000000000000007d057c017c
             05760172327c0278016a08000000000000000064037a0d000063025f0800
             000000000000007c02a00900000000000000000000000000000000000000
             00a6000000ab00000000000000000001007c057c0167017a0000007c006a
             06000000000000000064023c0000007c027c037c0464049c037d06741500
             0000000000000000007c0064057c06ac06a6030000ab0300000000000000
             005300
-         340           0 RESUME                   0
+         338           0 RESUME                   0
          
-         341           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         339           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         343          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         341          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (thread)
                       62 LOAD_ATTR                3 (posts)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (posts)
          
-         345         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         343         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 STORE_FAST               4 (post_form)
          
-         348         152 LOAD_FAST                0 (request)
+         346         152 LOAD_FAST                0 (request)
                      154 LOAD_ATTR                6 (session)
                      164 LOAD_METHOD              7 (get)
                      186 LOAD_CONST               2 ('viewed_threads')
                      188 BUILD_LIST               0
                      190 PRECALL                  2
                      194 CALL                     2
                      204 STORE_FAST               5 (viewed_threads)
          
-         349         206 LOAD_FAST                1 (thread_id)
+         347         206 LOAD_FAST                1 (thread_id)
                      208 LOAD_FAST                5 (viewed_threads)
                      210 CONTAINS_OP              1
                      212 POP_JUMP_FORWARD_IF_FALSE    50 (to 314)
          
-         350         214 LOAD_FAST                2 (thread)
+         348         214 LOAD_FAST                2 (thread)
                      216 COPY                     1
                      218 LOAD_ATTR                8 (view_count)
                      228 LOAD_CONST               3 (1)
                      230 BINARY_OP               13 (+=)
                      234 SWAP                     2
                      236 STORE_ATTR               8 (view_count)
          
-         351         246 LOAD_FAST                2 (thread)
+         349         246 LOAD_FAST                2 (thread)
                      248 LOAD_METHOD              9 (save)
                      270 PRECALL                  0
                      274 CALL                     0
                      284 POP_TOP
          
-         352         286 LOAD_FAST                5 (viewed_threads)
+         350         286 LOAD_FAST                5 (viewed_threads)
                      288 LOAD_FAST                1 (thread_id)
                      290 BUILD_LIST               1
                      292 BINARY_OP                0 (+)
                      296 LOAD_FAST                0 (request)
                      298 LOAD_ATTR                6 (session)
                      308 LOAD_CONST               2 ('viewed_threads')
                      310 STORE_SUBSCR
          
-         355     >>  314 LOAD_FAST                2 (thread)
+         353     >>  314 LOAD_FAST                2 (thread)
          
-         356         316 LOAD_FAST                3 (posts)
+         354         316 LOAD_FAST                3 (posts)
          
-         357         318 LOAD_FAST                4 (post_form)
+         355         318 LOAD_FAST                4 (post_form)
          
-         354         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
+         352         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
                      322 BUILD_CONST_KEY_MAP      3
                      324 STORE_FAST               6 (context)
          
-         359         326 LOAD_GLOBAL             21 (NULL + render)
+         357         326 LOAD_GLOBAL             21 (NULL + render)
                      338 LOAD_FAST                0 (request)
                      340 LOAD_CONST               5 ('punkweb_bb/thread.html')
                      342 LOAD_FAST                6 (context)
                      344 KW_NAMES                 6
                      346 PRECALL                  3
                      350 CALL                     3
                      360 RETURN_VALUE
@@ -2234,15 +2228,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'paginate_qs', 'posts', 'all', 'PostModelForm', 'session', 'get', 'view_count', 'save', 'render')
          varnames   ('request', 'thread_id', 'thread', 'posts', 'post_form', 'viewed_threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_view'
-         firstlineno 340
+         firstlineno 338
          lnotab 0x02012c024e021c0336010801200128011c030201020102fd0605
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2255,91 +2249,91 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac04a6010000ab0100
             000000000000007d037c027c0364059c027d047417000000000000000000
             007c0064067c04ac07a6030000ab0300000000000000005300
-         362           0 RESUME                   0
+         360           0 RESUME                   0
          
-         364           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         362           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         366          46 LOAD_FAST                2 (thread)
+         364          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_edit)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         367          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         365          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         368         110 LOAD_CONST               2 ('You do not have permission to change this thread.')
+         366         110 LOAD_CONST               2 ('You do not have permission to change this thread.')
          
-         367         112 PRECALL                  1
+         365         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         371     >>  128 LOAD_FAST                0 (request)
+         369     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         372         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         370         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (thread)
                      176 KW_NAMES                 4
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         374         194 LOAD_FAST                3 (form)
+         372         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         375         234 LOAD_FAST                3 (form)
+         373         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (thread)
          
-         377         274 LOAD_GLOBAL             21 (NULL + redirect)
+         375         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (thread)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         374     >>  304 JUMP_FORWARD            16 (to 338)
+         372     >>  304 JUMP_FORWARD            16 (to 338)
          
-         379     >>  306 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         377     >>  306 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      318 LOAD_FAST                2 (thread)
                      320 KW_NAMES                 4
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         382     >>  338 LOAD_FAST                2 (thread)
+         380     >>  338 LOAD_FAST                2 (thread)
          
-         383         340 LOAD_FAST                3 (form)
+         381         340 LOAD_FAST                3 (form)
          
-         381         342 LOAD_CONST               5 (('thread', 'form'))
+         379         342 LOAD_CONST               5 (('thread', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         385         348 LOAD_GLOBAL             23 (NULL + render)
+         383         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               6 ('punkweb_bb/thread_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 7
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -2354,15 +2348,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'can_edit', 'user', 'HttpResponseForbidden', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'thread_id', 'thread', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_update_view'
-         firstlineno 362
+         firstlineno 360
          lnotab
             0x02022c0234010c0102ff100416012c02280128021efd02052003020102
             fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -2375,69 +2369,69 @@
             0000000000000053007c006a05000000000000000064036b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064047c
             0269017d037415000000000000000000007c0064057c03ac06a6030000ab
             0300000000000000005300
-         388           0 RESUME                   0
+         386           0 RESUME                   0
          
-         390           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         388           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         392          46 LOAD_FAST                2 (thread)
+         390          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         393          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         391          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         394         110 LOAD_CONST               2 ('You do not have permission to delete this thread.')
+         392         110 LOAD_CONST               2 ('You do not have permission to delete this thread.')
          
-         393         112 PRECALL                  1
+         391         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         397     >>  128 LOAD_FAST                0 (request)
+         395     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         398         150 LOAD_FAST                2 (thread)
+         396         150 LOAD_FAST                2 (thread)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         400         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         398         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (thread)
                      204 LOAD_ATTR                8 (subcategory)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         403     >>  266 LOAD_CONST               4 ('thread')
+         401     >>  266 LOAD_CONST               4 ('thread')
                      268 LOAD_FAST                2 (thread)
          
-         402         270 BUILD_MAP                1
+         400         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         406         274 LOAD_GLOBAL             21 (NULL + render)
+         404         274 LOAD_GLOBAL             21 (NULL + render)
                      286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               5 ('punkweb_bb/partials/thread_delete.html')
                      290 LOAD_FAST                3 (context)
                      292 KW_NAMES                 6
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
@@ -2451,15 +2445,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'subcategory', 'get_absolute_url', 'render')
          varnames   ('request', 'thread_id', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_delete_view'
-         firstlineno 388
+         firstlineno 386
          lnotab 0x02022c0234010c0102ff1004160128024c0304ff0404
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
@@ -2468,51 +2462,51 @@
             0300000000000000000000000000000000000000006402a6010000ab0100
             00000000000000730f7409000000000000000000006403a6010000ab0100
             0000000000000053007c026a0500000000000000000c007c025f05000000
             00000000007c02a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000000100740f000000000000000000007c02a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6010000ab0100000000000000005300
-         409           0 RESUME                   0
+         407           0 RESUME                   0
          
-         411           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         409           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         413          46 LOAD_FAST                0 (request)
+         411          46 LOAD_FAST                0 (request)
                       48 LOAD_ATTR                2 (user)
                       58 LOAD_METHOD              3 (has_perm)
                       80 LOAD_CONST               2 ('punkweb_bb.pin_thread')
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         414          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         412          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               3 ('You do not have permission to pin threads.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         416     >>  128 LOAD_FAST                2 (thread)
+         414     >>  128 LOAD_FAST                2 (thread)
                      130 LOAD_ATTR                5 (is_pinned)
                      140 UNARY_NOT
                      142 LOAD_FAST                2 (thread)
                      144 STORE_ATTR               5 (is_pinned)
          
-         417         154 LOAD_FAST                2 (thread)
+         415         154 LOAD_FAST                2 (thread)
                      156 LOAD_METHOD              6 (save)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-         419         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         417         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      206 LOAD_FAST                2 (thread)
                      208 LOAD_METHOD              8 (get_absolute_url)
                      230 PRECALL                  0
                      234 CALL                     0
                      244 PRECALL                  1
                      248 CALL                     1
                      258 RETURN_VALUE
@@ -2523,15 +2517,15 @@
             'You do not have permission to pin threads.'
          names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_pinned', 'save', 'htmx_redirect', 'get_absolute_url')
          varnames   ('request', 'thread_id', 'thread')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_pin_view'
-         firstlineno 409
+         firstlineno 407
          lnotab 0x02022c0234011e021a012802
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
@@ -2540,51 +2534,51 @@
             0300000000000000000000000000000000000000006402a6010000ab0100
             00000000000000730f7409000000000000000000006403a6010000ab0100
             0000000000000053007c026a0500000000000000000c007c025f05000000
             00000000007c02a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000000100740f000000000000000000007c02a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6010000ab0100000000000000005300
-         422           0 RESUME                   0
+         420           0 RESUME                   0
          
-         424           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         422           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         426          46 LOAD_FAST                0 (request)
+         424          46 LOAD_FAST                0 (request)
                       48 LOAD_ATTR                2 (user)
                       58 LOAD_METHOD              3 (has_perm)
                       80 LOAD_CONST               2 ('punkweb_bb.close_thread')
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         427          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         425          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               3 ('You do not have permission to close threads.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         429     >>  128 LOAD_FAST                2 (thread)
+         427     >>  128 LOAD_FAST                2 (thread)
                      130 LOAD_ATTR                5 (is_closed)
                      140 UNARY_NOT
                      142 LOAD_FAST                2 (thread)
                      144 STORE_ATTR               5 (is_closed)
          
-         430         154 LOAD_FAST                2 (thread)
+         428         154 LOAD_FAST                2 (thread)
                      156 LOAD_METHOD              6 (save)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-         432         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         430         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      206 LOAD_FAST                2 (thread)
                      208 LOAD_METHOD              8 (get_absolute_url)
                      230 PRECALL                  0
                      234 CALL                     0
                      244 PRECALL                  1
                      248 CALL                     1
                      258 RETURN_VALUE
@@ -2595,15 +2589,15 @@
             'You do not have permission to close threads.'
          names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_closed', 'save', 'htmx_redirect', 'get_absolute_url')
          varnames   ('request', 'thread_id', 'thread')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_close_view'
-         firstlineno 422
+         firstlineno 420
          lnotab 0x02022c0234011e021a012802
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
@@ -2616,97 +2610,97 @@
             00000000000000000000000000a6000000ab000000000000000000724c7c
             03a00800000000000000000000000000000000000000006403ac04a60100
             00ab0100000000000000007d047c027c045f0900000000000000007c006a
             0300000000000000007c045f0300000000000000007c04a0080000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             007415000000000000000000007c04a6010000ab01000000000000000053
             0064005300
-         435           0 RESUME                   0
+         433           0 RESUME                   0
          
-         437           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         435           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         439          46 LOAD_FAST                2 (thread)
+         437          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_post)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         440          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         438          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         441         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
+         439         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
          
-         440         112 PRECALL                  1
+         438         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         444     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         442     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      140 LOAD_FAST                0 (request)
                      142 LOAD_ATTR                6 (POST)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               3 (form)
          
-         446         168 LOAD_FAST                3 (form)
+         444         168 LOAD_FAST                3 (form)
                      170 LOAD_METHOD              7 (is_valid)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 POP_JUMP_FORWARD_IF_FALSE    76 (to 360)
          
-         447         208 LOAD_FAST                3 (form)
+         445         208 LOAD_FAST                3 (form)
                      210 LOAD_METHOD              8 (save)
                      232 LOAD_CONST               3 (False)
                      234 KW_NAMES                 4
                      236 PRECALL                  1
                      240 CALL                     1
                      250 STORE_FAST               4 (post)
          
-         448         252 LOAD_FAST                2 (thread)
+         446         252 LOAD_FAST                2 (thread)
                      254 LOAD_FAST                4 (post)
                      256 STORE_ATTR               9 (thread)
          
-         449         266 LOAD_FAST                0 (request)
+         447         266 LOAD_FAST                0 (request)
                      268 LOAD_ATTR                3 (user)
                      278 LOAD_FAST                4 (post)
                      280 STORE_ATTR               3 (user)
          
-         450         290 LOAD_FAST                4 (post)
+         448         290 LOAD_FAST                4 (post)
                      292 LOAD_METHOD              8 (save)
                      314 PRECALL                  0
                      318 CALL                     0
                      328 POP_TOP
          
-         452         330 LOAD_GLOBAL             21 (NULL + redirect)
+         450         330 LOAD_GLOBAL             21 (NULL + redirect)
                      342 LOAD_FAST                4 (post)
                      344 PRECALL                  1
                      348 CALL                     1
                      358 RETURN_VALUE
          
-         446     >>  360 LOAD_CONST               0 (None)
+         444     >>  360 LOAD_CONST               0 (None)
                      362 RETURN_VALUE
          consts
             None
             ('pk',)
             'You do not have permission to post in this thread.'
             False
             ('commit',)
          names      ('get_object_or_404', 'Thread', 'can_post', 'user', 'HttpResponseForbidden', 'PostModelForm', 'POST', 'is_valid', 'save', 'thread', 'redirect')
          varnames   ('request', 'thread_id', 'thread', 'form', 'post')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_create_view'
-         firstlineno 435
+         firstlineno 433
          lnotab 0x02022c0234010c0102ff1004280228012c010e01180128021efa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2719,87 +2713,87 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             0000005300740d000000000000000000007c02ac04a6010000ab01000000
             00000000007d037c027c0364059c027d047417000000000000000000007c
             0064067c04ac07a6030000ab0300000000000000005300
-         455           0 RESUME                   0
+         453           0 RESUME                   0
          
-         457           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         455           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         459          46 LOAD_FAST                2 (post)
+         457          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_edit)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         460          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         458          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to change this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         462     >>  128 LOAD_FAST                0 (request)
+         460     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    77 (to 304)
          
-         463         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         461         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (post)
                      176 KW_NAMES                 4
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         465         194 LOAD_FAST                3 (form)
+         463         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         466         234 LOAD_FAST                3 (form)
+         464         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (post)
          
-         468         274 LOAD_GLOBAL             21 (NULL + redirect)
+         466         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (post)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         470     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         468     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      316 LOAD_FAST                2 (post)
                      318 KW_NAMES                 4
                      320 PRECALL                  1
                      324 CALL                     1
                      334 STORE_FAST               3 (form)
          
-         473         336 LOAD_FAST                2 (post)
+         471         336 LOAD_FAST                2 (post)
          
-         474         338 LOAD_FAST                3 (form)
+         472         338 LOAD_FAST                3 (form)
          
-         472         340 LOAD_CONST               5 (('post', 'form'))
+         470         340 LOAD_CONST               5 (('post', 'form'))
                      342 BUILD_CONST_KEY_MAP      2
                      344 STORE_FAST               4 (context)
          
-         477         346 LOAD_GLOBAL             23 (NULL + render)
+         475         346 LOAD_GLOBAL             23 (NULL + render)
                      358 LOAD_FAST                0 (request)
                      360 LOAD_CONST               6 ('punkweb_bb/partials/post_update.html')
                      362 LOAD_FAST                4 (context)
                      364 KW_NAMES                 7
                      366 PRECALL                  3
                      370 CALL                     3
                      380 RETURN_VALUE
@@ -2814,15 +2808,15 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_edit', 'user', 'HttpResponseForbidden', 'method', 'PostModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'post_id', 'post', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_update_view'
-         firstlineno 455
+         firstlineno 453
          lnotab 0x02022c0234011e0216012c02280128021e022003020102fe0605
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -2833,67 +2827,67 @@
             0000000000000053007c006a05000000000000000064036b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064047c
             0269017d037415000000000000000000007c0064057c03ac06a6030000ab
             0300000000000000005300
-         480           0 RESUME                   0
+         478           0 RESUME                   0
          
-         482           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         480           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         484          46 LOAD_FAST                2 (post)
+         482          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         485          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         483          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         487     >>  128 LOAD_FAST                0 (request)
+         485     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         488         150 LOAD_FAST                2 (post)
+         486         150 LOAD_FAST                2 (post)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         490         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         488         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (post)
                      204 LOAD_ATTR                8 (thread)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         493     >>  266 LOAD_CONST               4 ('post')
+         491     >>  266 LOAD_CONST               4 ('post')
                      268 LOAD_FAST                2 (post)
          
-         492         270 BUILD_MAP                1
+         490         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         496         274 LOAD_GLOBAL             21 (NULL + render)
+         494         274 LOAD_GLOBAL             21 (NULL + render)
                      286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               5 ('punkweb_bb/partials/post_delete.html')
                      290 LOAD_FAST                3 (context)
                      292 KW_NAMES                 6
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
@@ -2907,94 +2901,94 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'thread', 'get_absolute_url', 'render')
          varnames   ('request', 'post_id', 'post', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_delete_view'
-         firstlineno 480
+         firstlineno 478
          lnotab 0x02022c0234011e02160128024c0304ff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007407000000000000000000006a
-            040000000000000000a6000000ab000000000000000000740b0000000000
-            00000000006a0600000000000000006401ac02a6010000ab010000000000
-            0000007a0a0000ac03a6010000ab010000000000000000a0070000000000
+            040000000000000000a6000000ab00000000000000000074070000000000
+            00000000006a0500000000000000006401ac02a6010000ab010000000000
+            0000007a0a0000ac03a6010000ab010000000000000000a0060000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             005300
-         499           0 RESUME                   0
+         497           0 RESUME                   0
          
-         500           2 LOAD_GLOBAL              0 (Shout)
+         498           2 LOAD_GLOBAL              0 (Shout)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (filter)
          
-         501          46 LOAD_GLOBAL              7 (NULL + timezone)
+         499          46 LOAD_GLOBAL              7 (NULL + timezone)
                       58 LOAD_ATTR                4 (now)
                       68 PRECALL                  0
                       72 CALL                     0
-                      82 LOAD_GLOBAL             11 (NULL + datetime)
-                      94 LOAD_ATTR                6 (timedelta)
+                      82 LOAD_GLOBAL              7 (NULL + timezone)
+                      94 LOAD_ATTR                5 (timedelta)
                      104 LOAD_CONST               1 (12)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 BINARY_OP               10 (-)
          
-         500         126 KW_NAMES                 3
+         498         126 KW_NAMES                 3
                      128 PRECALL                  1
                      132 CALL                     1
          
-         502         142 LOAD_METHOD              7 (order_by)
+         500         142 LOAD_METHOD              6 (order_by)
                      164 LOAD_CONST               4 ('created_at')
                      166 PRECALL                  1
                      170 CALL                     1
          
-         500         180 RETURN_VALUE
+         498         180 RETURN_VALUE
          consts
             None
             12
             ('hours',)
             ('created_at__gt',)
             'created_at'
-         names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'datetime', 'timedelta', 'order_by')
+         names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'timedelta', 'order_by')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'current_shouts'
-         firstlineno 499
+         firstlineno 497
          lnotab 0x02012c0150ff100226fe
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             0164017c0169017d027403000000000000000000007c0064027c02ac03a6
             030000ab0300000000000000005300
-         505           0 RESUME                   0
+         503           0 RESUME                   0
          
-         506           2 LOAD_GLOBAL              1 (NULL + current_shouts)
+         504           2 LOAD_GLOBAL              1 (NULL + current_shouts)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (shouts)
          
-         509          30 LOAD_CONST               1 ('shouts')
+         507          30 LOAD_CONST               1 ('shouts')
                       32 LOAD_FAST                1 (shouts)
          
-         508          34 BUILD_MAP                1
+         506          34 BUILD_MAP                1
                       36 STORE_FAST               2 (context)
          
-         511          38 LOAD_GLOBAL              3 (NULL + render)
+         509          38 LOAD_GLOBAL              3 (NULL + render)
                       50 LOAD_FAST                0 (request)
                       52 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       54 LOAD_FAST                2 (context)
                       56 KW_NAMES                 3
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -3005,15 +2999,15 @@
             ('context',)
          names      ('current_shouts', 'render')
          varnames   ('request', 'shouts', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_list_view'
-         firstlineno 505
+         firstlineno 503
          lnotab 0x02011c0304ff0403
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -3026,99 +3020,99 @@
             00a6000000ab000000000000000000725a7c02a008000000000000000000
             00000000000000000000006405ac06a6010000ab0100000000000000007d
             037c006a0000000000000000007c035f0000000000000000007c03a00800
             00000000000000000000000000000000000000a6000000ab000000000000
             00000001006401740500000000000000000000a6000000ab000000000000
             00000069017d017407000000000000000000007c0064027c01ac03a60300
             00ab03000000000000000053006400530064005300
-         514           0 RESUME                   0
+         512           0 RESUME                   0
          
-         515           2 LOAD_FAST                0 (request)
+         513           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_TRUE    34 (to 94)
          
-         517          26 LOAD_CONST               1 ('shouts')
+         515          26 LOAD_CONST               1 ('shouts')
                       28 LOAD_GLOBAL              5 (NULL + current_shouts)
                       40 PRECALL                  0
                       44 CALL                     0
          
-         516          54 BUILD_MAP                1
+         514          54 BUILD_MAP                1
                       56 STORE_FAST               1 (context)
          
-         519          58 LOAD_GLOBAL              7 (NULL + render)
+         517          58 LOAD_GLOBAL              7 (NULL + render)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       74 LOAD_FAST                1 (context)
                       76 KW_NAMES                 3
                       78 PRECALL                  3
                       82 CALL                     3
                       92 RETURN_VALUE
          
-         521     >>   94 LOAD_FAST                0 (request)
+         519     >>   94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                4 (method)
                      106 LOAD_CONST               4 ('POST')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE   128 (to 372)
          
-         522         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
+         520         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
                      128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                6 (POST)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (form)
          
-         524         156 LOAD_FAST                2 (form)
+         522         156 LOAD_FAST                2 (form)
                      158 LOAD_METHOD              7 (is_valid)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_JUMP_FORWARD_IF_FALSE    90 (to 376)
          
-         525         196 LOAD_FAST                2 (form)
+         523         196 LOAD_FAST                2 (form)
                      198 LOAD_METHOD              8 (save)
                      220 LOAD_CONST               5 (False)
                      222 KW_NAMES                 6
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (shout)
          
-         526         240 LOAD_FAST                0 (request)
+         524         240 LOAD_FAST                0 (request)
                      242 LOAD_ATTR                0 (user)
                      252 LOAD_FAST                3 (shout)
                      254 STORE_ATTR               0 (user)
          
-         527         264 LOAD_FAST                3 (shout)
+         525         264 LOAD_FAST                3 (shout)
                      266 LOAD_METHOD              8 (save)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 POP_TOP
          
-         530         304 LOAD_CONST               1 ('shouts')
+         528         304 LOAD_CONST               1 ('shouts')
                      306 LOAD_GLOBAL              5 (NULL + current_shouts)
                      318 PRECALL                  0
                      322 CALL                     0
          
-         529         332 BUILD_MAP                1
+         527         332 BUILD_MAP                1
                      334 STORE_FAST               1 (context)
          
-         532         336 LOAD_GLOBAL              7 (NULL + render)
+         530         336 LOAD_GLOBAL              7 (NULL + render)
          
-         533         348 LOAD_FAST                0 (request)
+         531         348 LOAD_FAST                0 (request)
                      350 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                      352 LOAD_FAST                1 (context)
          
-         532         354 KW_NAMES                 3
+         530         354 KW_NAMES                 3
                      356 PRECALL                  3
                      360 CALL                     3
                      370 RETURN_VALUE
          
-         521     >>  372 LOAD_CONST               0 (None)
+         519     >>  372 LOAD_CONST               0 (None)
                      374 RETURN_VALUE
          
-         524     >>  376 LOAD_CONST               0 (None)
+         522     >>  376 LOAD_CONST               0 (None)
                      378 RETURN_VALUE
          consts
             None
             'shouts'
             'punkweb_bb/shoutbox/shout_list.html'
             ('context',)
             'POST'
@@ -3126,15 +3120,15 @@
             ('commit',)
          names      ('user', 'is_authenticated', 'current_shouts', 'render', 'method', 'ShoutModelForm', 'POST', 'is_valid', 'save')
          varnames   ('request', 'context', 'form', 'shout')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_create_view'
-         firstlineno 514
+         firstlineno 512
          lnotab
             0x020118021cff040324021601280228012c01180128031cff04030c0106
             ff12f50403
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -3146,66 +3140,66 @@
             00000000000000730f7409000000000000000000006402a6010000ab0100
             0000000000000053007c006a05000000000000000064036b020000000072
             307c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f0000000000000000000074110000000000
             00000000006404a6010000ab010000000000000000a6010000ab01000000
             0000000000530064057c0269017d037413000000000000000000007c0064
             067c03ac07a6030000ab0300000000000000005300
-         537           0 RESUME                   0
+         535           0 RESUME                   0
          
-         539           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         537           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Shout)
                       26 LOAD_FAST                1 (shout_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (shout)
          
-         541          46 LOAD_FAST                2 (shout)
+         539          46 LOAD_FAST                2 (shout)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         542          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         540          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this shout.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         544     >>  128 LOAD_FAST                0 (request)
+         542     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    48 (to 246)
          
-         545         150 LOAD_FAST                2 (shout)
+         543         150 LOAD_FAST                2 (shout)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         547         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         545         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_GLOBAL             17 (NULL + reverse)
                      214 LOAD_CONST               4 ('punkweb_bb:index')
                      216 PRECALL                  1
                      220 CALL                     1
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         550     >>  246 LOAD_CONST               5 ('shout')
+         548     >>  246 LOAD_CONST               5 ('shout')
                      248 LOAD_FAST                2 (shout)
          
-         549         250 BUILD_MAP                1
+         547         250 BUILD_MAP                1
                      252 STORE_FAST               3 (context)
          
-         553         254 LOAD_GLOBAL             19 (NULL + render)
+         551         254 LOAD_GLOBAL             19 (NULL + render)
                      266 LOAD_FAST                0 (request)
                      268 LOAD_CONST               6 ('punkweb_bb/partials/shout_delete.html')
                      270 LOAD_FAST                3 (context)
                      272 KW_NAMES                 7
                      274 PRECALL                  3
                      278 CALL                     3
                      288 RETURN_VALUE
@@ -3220,36 +3214,36 @@
             ('context',)
          names      ('get_object_or_404', 'Shout', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'reverse', 'render')
          varnames   ('request', 'shout_id', 'shout', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_delete_view'
-         firstlineno 537
+         firstlineno 535
          lnotab 0x02022c0234011e0216012802380304ff0404
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
-         556           0 RESUME                   0
+         554           0 RESUME                   0
          
-         557           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         555           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         611           6 LOAD_CONST               2 ('codes')
+         609           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         610          10 BUILD_MAP                1
+         608          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         614          14 LOAD_GLOBAL              1 (NULL + render)
+         612          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
@@ -3261,24 +3255,25 @@
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
-         firstlineno 556
+         firstlineno 554
          lnotab 0x0201043604ff0404
-   names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
+      None
+   names      ('django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080218010c010c0114010c010c02280a0c011c010c010c010c
-      0214030614061a060506200609060b160104ff0e010216160104ff0e0102
-      16160104ff0e010217160104ff0e010212060c160104ff0e01021c160104
-      ff0e010219160104ff0e010216160104ff0e01021c0616160104ff0e0102
-      19160104ff0e010214160104ff0e01020c160104ff0e01020c160104ff0e
-      010213160104ff0e010218160104ff0e010212060606090617160104ff0e
-      010212
+      0x00ff020118010c010c0114010c010c02280a0c011c010c010c010c0214
+      030614061a060506200609060b160104ff0e010216160104ff0e01021616
+      0104ff0e010217160104ff0e010212060c160104ff0e01021c160104ff0e
+      010219160104ff0e010216160104ff0e01021c0616160104ff0e01021916
+      0104ff0e010214160104ff0e01020c160104ff0e01020c160104ff0e0102
+      13160104ff0e010218160104ff0e010212060606090617160104ff0e0102
+      12
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/admin.py` & `punkweb_bb-0.2.3/punkweb_bb/admin.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/admin_forms.py` & `punkweb_bb-0.2.3/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.2.3/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/forms.py` & `punkweb_bb-0.2.3/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/middleware.py` & `punkweb_bb-0.2.3/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.2.3/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/0003_alter_thread_options.py` & `punkweb_bb-0.2.3/punkweb_bb/migrations/0003_alter_thread_options.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/0004_groupstyle.py` & `punkweb_bb-0.2.3/punkweb_bb/migrations/0004_groupstyle.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/models.py` & `punkweb_bb-0.2.3/punkweb_bb/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import datetime
 import math
 import os
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
 from django.core.cache import cache
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
 from django.utils import timezone
 from precise_bbcode.fields import BBCodeTextField
 
 from punkweb_bb.mixins import TimestampMixin, UUIDPrimaryKeyMixin
-from punkweb_bb.utils import get_styled_username
+from punkweb_bb.utils import get_highest_priority_group, get_styled_username
 
 User = get_user_model()
 
 
 def profile_image_upload_to(instance, filename):
     ext = os.path.splitext(filename)[-1]
     return f"punkweb_bb/board_profiles/{instance.user.username}/image{ext}"
@@ -27,22 +26,26 @@
     image = models.ImageField(upload_to=profile_image_upload_to, blank=True, null=True)
     signature = BBCodeTextField(max_length=1024, blank=True, null=True)
 
     class Meta:
         ordering = ("user__username",)
 
     @property
+    def priority_group(self):
+        return get_highest_priority_group(self.user)
+
+    @property
     def styled_username(self):
         return get_styled_username(self.user)
 
     @property
     def is_online(self):
         last_seen = cache.get(f"profile_online_{self.id}")
         if last_seen:
-            return timezone.now() < last_seen + datetime.timedelta(minutes=5)
+            return timezone.now() < last_seen + timezone.timedelta(minutes=5)
         return False
 
     @property
     def post_count(self):
         return self.user.threads.count() + self.user.posts.count()
 
     def __str__(self):
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/parsers.py` & `punkweb_bb-0.2.3/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/settings.py` & `punkweb_bb-0.2.3/punkweb_bb/settings.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/shoutbox.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files 7% similar despite different names*

```diff
@@ -24,84 +24,77 @@
   display: flex;
   flex: 0 0 16rem;
   flex-direction: column;
   gap: 1rem;
   padding: 1rem;
 }
 
-.thread__user__usernameContainer {
+.thread__user__info {
   align-items: center;
   display: flex;
+  flex-direction: column;
   gap: 0.25rem;
 }
 
-.thread__user__info {
+.thread__user__username {
+  align-items: center;
+  display: flex;
+  gap: 0.25rem;
+}
+
+.thread__user__group {
+  font-size: 0.75rem;
+  font-weight: 700;
+}
+
+.thread__user__details {
   background-color: var(--oc-gray-0);
   border: 1px solid var(--border);
   border-radius: 0.25rem;
   display: flex;
   flex-direction: column;
   font-size: 0.75rem;
   padding: 0.5rem;
   width: 100%;
 }
 
-.thread__user__info__row {
+.thread__user__details__row {
   align-items: center;
   display: flex;
   justify-content: space-between;
 }
 
-.thread__user__info__label {
+.thread__user__details__label {
   color: var(--body-fg);
 }
 
-.thread__user__groups {
-  display: flex;
-  flex-direction: column;
-  gap: 0.5rem;
-  width: 100%;
-}
-
-.thread__user__group {
-  background-color: var(--oc-gray-0);
-  border: 1px solid var(--border);
-  border-radius: 0.25rem;
-  color: var(--text-on-primary);
-  display: flex;
-  font-size: 0.875rem;
-  justify-content: center;
-  padding: 0.5rem;
-  width: 100%;
-}
-
 .thread__main {
   display: flex;
   flex-direction: column;
   width: 100%;
 }
 
 .thread__content {
   flex: 1;
   padding: 1rem;
 }
 
-.thread__signature {
-  border-top: 1px solid var(--border);
-  padding: 1rem;
-}
-
 .thread__actions {
   align-items: center;
   display: flex;
   justify-content: flex-end;
   gap: 0.25rem;
   padding: 1rem;
 }
 
+.thread__signature {
+  border-top: 1px solid var(--border);
+  padding: 1rem;
+}
+
 .thread__reply__content {
   display: flex;
   flex-direction: column;
   gap: 1rem;
 }
 
 @media screen and (max-width: 1024px) {
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_create.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_update.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,17 @@
         <div class="members__user__stats">
           <div class="members__user__stat">
             Posts:
             <span class="members__user__stat__value">{{user.profile.post_count}}</span>
           </div>
           <div class="members__user__stat">
             Date Joined:
-            <span class="members__user__stat__value">{{user.date_joined | date:'m/d/Y'}}</span>
+            <span class="members__user__stat__value">
+              <time datetime="{{user.date_joined|date:'c'}}">{{user.date_joined | date:'m/d/Y'}}</time>
+            </span>
           </div>
         </div>
       </div>
     </li>
     {% endfor %}
   </ul>
 </div>
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,23 @@
         {% endif %}
       </div>
       <div class="profile__info__details">
         <div class="profile__info__username">{{user|styled_username}}</div>
         <div class="profile__info__stats">
           <div class="profile__info__stat">
             Date Joined:
-            <span class="profile__info__stat__value">{{user.date_joined | date:'m/d/Y'}}</span>
+            <span class="profile__info__stat__value">
+              <time datetime="{{user.date_joined|date:'c'}}">{{user.date_joined | date:'m/d/Y'}}</time>
+            </span>
           </div>
           <div class="profile__info__stat">
             Last Login:
-            <span class="profile__info__stat__value">{{user.last_login | date:'m/d/Y'}}</span>
+            <span class="profile__info__stat__value">
+              <time datetime="{{user.last_login|date:'c'}}">{{user.last_login | date:'m/d/Y'}}</time>
+            </span>
           </div>
           <div class="profile__info__stat">
             Posts:
             <span class="profile__info__stat__value">{{user.profile.post_count}}</span>
           </div>
         </div>
       </div>
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load shoutbox_bbcode can_delete styled_username %}
 
 {% for shout in shouts %}
 <div class="shoutbox__shout">
   <div class="shoutbox__shout__content">
-    <span>{{shout.created_at|date:'g:i A'}}</span>
+    <time datetime="{{shout.created_at|date:'c'}}">{{shout.created_at | date:'g:i A'}}</time>
     <span><a href="{% url 'punkweb_bb:profile' shout.user.id %}">{{shout.user|styled_username}}</a>: </span>
     <span>{{ shout.content | safe | shoutbox_bbcode }}</span>
   </div>
   {% if shout|can_delete:request.user %}
   <div class="shoutbox__shout__actions">
     <button
       class="pw-icon-button default danger sm"
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% load shoutbox_bbcode can_delete styled_username %} {% for shout in shouts %}
-{{shout.created_at|date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}: {
+{{shout.created_at | date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}: {
 { shout.content | safe | shoutbox_bbcode }}
 {% if shout|can_delete:request.user %}
 delete
 {% endif %}
 {% endfor %}
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
               {% endif %}
             </div>
             <div>
               <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
                 {{thread.user|styled_username}}
               </a>
               •
-              {{thread.created_at|date:'M j, Y'}}</div>
+              <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'m j, Y'}}</time>
           </td>
           <td>{{thread.post_count}}</td>
           <td>{{thread.view_count | humanize_int}}</td>
           <td>
             {% if thread.latest_post %}
             <div class="thread__latestPost">
               <div class="thread__latestPost__info">
```

#### html2text {}

```diff
@@ -18,16 +18,16 @@
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                                 {% if thread.latest_post %}
 thread.is_pinned %} keep {%                                            _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
 endif %} {% if                                                         _Y_'_}_}
 thread.is_closed %} lock {%                         {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 endif %}                       {                    {thread.view_count {% if thread.latest_post.user.profile.image
 _{                              {thread.post_count}} | humanize_int}}   %} [{
 _{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}                                         {thread.latest_post.user.profile.image.url}}]
-â¢ {{thread.created_at|date:                                          {% else %} [{% static 'punkweb_bb/img/
-'M j, Y'}}                                                             default-profile-image.png' %}]{% endif %}
+â¢ {{thread.created_at |                                              {% else %} [{% static 'punkweb_bb/img/
+date:'m j, Y'}}                                                        default-profile-image.png' %}]{% endif %}
                                                                        {% else %} No posts {% endif %}
 {% if threads.has_other_pages %}
     * {% if threads.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in threads.paginator.page_range %} {% if
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_create.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_update.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static can_delete can_edit can_post styled_username styled_group_name %}
+{% load static can_delete can_edit can_post styled_username %}
 
 {% block title_prefix %}{{thread.title}} | {% endblock %}
 {% block og_title_prefix %}{{thread.title}} | {% endblock %}
 
 {% block extra_head %}
 <meta name="description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
 <meta property="og:description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
@@ -37,52 +37,56 @@
 </nav>
 
 {% if posts.number == 1 %}
 <h1>{{thread.title}}</h1>
 
 <div class="pw-card fluid margin">
   <div class="pw-card-header">
-    <div class="thread__date">{{thread.created_at|date:'M d, Y'}}</div>
+    <div class="thread__date">
+      <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'M d, Y'}}</time>
+    </div>
   </div>
   <div class="thread">
     <div class="thread__user">
-      {% if thread.user.profile.image %}
-      <img class="pw-avatar" src="{{thread.user.profile.image.url}}" alt="{{thread.user.username}}" />
-      {% else %}
-      <img class="pw-avatar" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" alt="{{thread.user.username}}" />
-      {% endif %}
-      <div class="thread__user__usernameContainer">
-        {% if thread.user.profile.is_online %}
-        <div class="onlineIndicator"></div>
-        {% endif %}
-        <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
-          {{thread.user|styled_username}}
-        </a>
-      </div>
       <div class="thread__user__info">
-        <div class="thread__user__info__row">
-          <div class="thread__user__info__label">Joined:</div>
-          <div class="thread__user__info__value">
-            {{thread.user.date_joined|date:"M d, Y"}}
-          </div>
+        <div class="thread__user__image">
+          {% if thread.user.profile.image %}
+          <img class="pw-avatar" src="{{thread.user.profile.image.url}}" alt="{{thread.user.username}}" />
+          {% else %}
+          <img class="pw-avatar" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" alt="{{thread.user.username}}" />
+          {% endif %}
+        </div>
+        <div class="thread__user__username">
+          {% if thread.user.profile.is_online %}
+          <div class="onlineIndicator"></div>
+          {% endif %}
+          <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
+            {{thread.user|styled_username}}
+          </a>
         </div>
-        <div class="thread__user__info__row">
-          <div class="thread__user__info__label">Posts:</div>
-          <div class="thread__user__info__value">{{thread.user.profile.post_count}}</div>
+        <div class="thread__user__group">
+          {% if thread.user.profile.priority_group %}
+          {{thread.user.profile.priority_group.name}}
+          {% else %}
+          Member
+          {% endif %}
         </div>
       </div>
-      {% if thread.user.groups.all|length > 0 %}
-      <div class="thread__user__groups">
-        {% for group in thread.user.groups.all %}
-        <div class="thread__user__group">
-          {{group|styled_group_name}}
+      <div class="thread__user__details">
+        <div class="thread__user__details__row">
+          <div class="thread__user__details__label">Joined:</div>
+          <div class="thread__user__details__value">
+            <time datetime="{{thread.user.date_joined|date:'c'}}">{{thread.user.date_joined | date:'M d, Y'}}</time>
+          </div>
+        </div>
+        <div class="thread__user__details__row">
+          <div class="thread__user__details__label">Posts:</div>
+          <div class="thread__user__details__value">{{thread.user.profile.post_count}}</div>
         </div>
-        {% endfor %}
       </div>
-      {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{thread.content.rendered}}
       </div>
       {% if thread|can_delete:request.user or thread|can_edit:request.user or perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
       <div class="thread__actions">
@@ -144,57 +148,61 @@
   </div>
 </div>
 {% endif %}
 
 {% for post in posts %}
 <div id="post-{{post.id}}" class="pw-card fluid margin">
   <div class="pw-card-header thread__header">
-    <div class="thread__date">{{post.created_at|date:'M d, Y'}}</div>
+    <div class="thread__date">
+      <time datetime="{{post.created_at|date:'c'}}">{{post.created_at | date:'M d, Y'}}</time>
+    </div>
     <a class="thread__index" href="{{post.get_absolute_url}}">#{{post.index}}</a>
   </div>
   <div class="thread">
     <div class="thread__user">
-      {% if post.user.profile.image %}
-      <div class="thread__user__image">
-        <img class="pw-avatar" src="{{post.user.profile.image.url}}" alt="{{post.user.username}}" />
-      </div>
-      {% else %}
-      <div class="thread__user__image">
-        <img class="pw-avatar" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" alt="{{post.user.username}}" />
-      </div>
-      {% endif %}
-      <div class="thread__user__usernameContainer">
-        {% if post.user.profile.is_online %}
-        <div class="onlineIndicator"></div>
-        {% endif %}
-        <a href="{% url 'punkweb_bb:profile' post.user.id %}">
-          {{post.user|styled_username}}
-        </a>
-      </div>
       <div class="thread__user__info">
-        <div class="thread__user__info__row">
-          <div class="thread__user__info__label">Joined:</div>
-          <div class="thread__user__info__value">
-            {{post.user.date_joined|date:"M d, Y"}}
+        <div class="thread__user__image">
+          {% if post.user.profile.image %}
+          <div class="thread__user__image">
+            <img class="pw-avatar" src="{{post.user.profile.image.url}}" alt="{{post.user.username}}" />
           </div>
+          {% else %}
+          <div class="thread__user__image">
+            <img class="pw-avatar" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" alt="{{post.user.username}}" />
+          </div>
+          {% endif %}
         </div>
-        <div class="thread__user__info__row">
-          <div class="thread__user__info__label">Posts:</div>
-          <div class="thread__user__info__value">{{post.user.profile.post_count}}</div>
+        <div class="thread__user__username">
+          {% if post.user.profile.is_online %}
+          <div class="onlineIndicator"></div>
+          {% endif %}
+          <a href="{% url 'punkweb_bb:profile' post.user.id %}">
+            {{post.user|styled_username}}
+          </a>
         </div>
-      </div>
-      {% if post.user.groups.all|length > 0 %}
-      <div class="thread__user__groups">
-        {% for group in post.user.groups.all %}
         <div class="thread__user__group">
-          {{group|styled_group_name}}
+          {% if post.user.profile.priority_group %}
+          {{post.user.profile.priority_group.name}}
+          {% else %}
+          Member
+          {% endif %}
+        </div>
+      </div>
+      <div class="thread__user__details">
+        <div class="thread__user__details__row">
+          <div class="thread__user__details__label">Joined:</div>
+          <div class="thread__user__details__value">
+            <time datetime="{{post.user.date_joined|date:'c'}}">{{post.user.date_joined | date:'M d, Y'}}</time>
+          </div>
+        </div>
+        <div class="thread__user__details__row">
+          <div class="thread__user__details__label">Posts:</div>
+          <div class="thread__user__details__value">{{post.user.profile.post_count}}</div>
         </div>
-        {% endfor %}
       </div>
-      {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{post.content.rendered}}
       </div>
       {% if post|can_delete:request.user or post|can_edit:request.user %}
       <div class="thread__actions">
```

#### html2text {}

```diff
@@ -1,63 +1,57 @@
 {% extends 'punkweb_bb/base.html' %} {% load static can_delete can_edit
-can_post styled_username styled_group_name %} {% block title_prefix %}{
-{thread.title}} | {% endblock %} {% block og_title_prefix %}{{thread.title}} |
-{% endblock %} {% block extra_head %}
+can_post styled_username %} {% block title_prefix %}{{thread.title}} | {%
+endblock %} {% block og_title_prefix %}{{thread.title}} | {% endblock %} {%
+block extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
 ************ {{{{tthhrreeaadd..ttiittllee}}}} ************
-{{thread.created_at|date:'M d, Y'}}
+{{thread.created_at | date:'M d, Y'}}
 {% if thread.user.profile.image %} [{{thread.user.username}}]{% else %} [{
 {thread.user.username}}]{% endif %}
 {% if thread.user.profile.is_online %}
 {% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
+{% if thread.user.profile.priority_group %} {
+{thread.user.profile.priority_group.name}} {% else %} Member {% endif %}
 Joined:
-{{thread.user.date_joined|date:"M d, Y"}}
+{{thread.user.date_joined | date:'M d, Y'}}
 Posts:
 {{thread.user.profile.post_count}}
-{% if thread.user.groups.all|length > 0 %}
-{% for group in thread.user.groups.all %}
-{{group|styled_group_name}}
-{% endfor %}
-{% endif %}
 {{thread.content.rendered}}
 {% if thread|can_delete:request.user or thread|can_edit:request.user or
 perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
 {% if perms.punkweb_bb.pin_thread %} {% if thread.is_pinned %} keep_off {% else
 %} keep {% endif %} {% endif %} {% if perms.punkweb_bb.close_thread %} {% if
 thread.is_closed %} lock_open {% else %} lock {% endif %} {% endif %} {% if
 thread|can_edit:request.user %} _e_d_i_t_ {% endif %} {% if thread|can_delete:
 request.user %} delete {% endif %}
 {% endif %} {% if thread.user.profile.signature.rendered %}
 {{thread.user.profile.signature.rendered}}
 {% endif %}
 {% endif %} {% for post in posts %}
-{{post.created_at|date:'M d, Y'}}
+{{post.created_at | date:'M d, Y'}}
 _#_{_{_p_o_s_t_._i_n_d_e_x_}_}
 {% if post.user.profile.image %}
 [{{post.user.username}}]
 {% else %}
 [{{post.user.username}}]
 {% endif %}
 {% if post.user.profile.is_online %}
 {% endif %} _{_{_p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
+{% if post.user.profile.priority_group %} {
+{post.user.profile.priority_group.name}} {% else %} Member {% endif %}
 Joined:
-{{post.user.date_joined|date:"M d, Y"}}
+{{post.user.date_joined | date:'M d, Y'}}
 Posts:
 {{post.user.profile.post_count}}
-{% if post.user.groups.all|length > 0 %}
-{% for group in post.user.groups.all %}
-{{group|styled_group_name}}
-{% endfor %}
-{% endif %}
 {{post.content.rendered}}
 {% if post|can_delete:request.user or post|can_edit:request.user %}
 {% if post|can_edit:request.user %} edit {% endif %} {% if post|can_delete:
 request.user %} delete {% endif %}
 {% endif %} {% if post.user.profile.signature.rendered %}
 {{post.user.profile.signature.rendered}}
 {% endif %}
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e8c5766 (Wed May 29 20:12:14 2024 UTC)
+moddate:  0xbe975766 (Wed May 29 21:01:50 2024 UTC)
 files sz: 257
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -24,18 +24,18 @@
                 16 LOAD_CONST               2 (('mark_safe',))
                 18 IMPORT_NAME              2 (django.utils.safestring)
                 20 IMPORT_FROM              3 (mark_safe)
                 22 STORE_NAME               3 (mark_safe)
                 24 POP_TOP
    
      4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('get_group_name_styled',))
+                28 LOAD_CONST               3 (('get_styled_group_name',))
                 30 IMPORT_NAME              4 (punkweb_bb.utils)
-                32 IMPORT_FROM              5 (get_group_name_styled)
-                34 STORE_NAME               5 (get_group_name_styled)
+                32 IMPORT_FROM              5 (get_styled_group_name)
+                34 STORE_NAME               5 (get_styled_group_name)
                 36 POP_TOP
    
      6          38 PUSH_NULL
                 40 LOAD_NAME                1 (template)
                 42 LOAD_ATTR                6 (Library)
                 52 PRECALL                  0
                 56 CALL                     0
@@ -53,45 +53,45 @@
     10          98 STORE_NAME               9 (styled_group_name)
                100 LOAD_CONST               5 (None)
                102 RETURN_VALUE
    consts
       0
       ('template',)
       ('mark_safe',)
-      ('get_group_name_styled',)
+      ('get_styled_group_name',)
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007403000000000000000000007c00a6
             010000ab010000000000000000a6010000ab0100000000000000005300
            9           0 RESUME                   0
          
           11           2 LOAD_GLOBAL              1 (NULL + mark_safe)
-                      14 LOAD_GLOBAL              3 (NULL + get_group_name_styled)
+                      14 LOAD_GLOBAL              3 (NULL + get_styled_group_name)
                       26 LOAD_FAST                0 (group)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 PRECALL                  1
                       46 CALL                     1
                       56 RETURN_VALUE
          consts
             None
-         names      ('mark_safe', 'get_group_name_styled')
+         names      ('mark_safe', 'get_styled_group_name')
          varnames   ('group',)
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/templatetags/styled_group_name.py'
          name       'styled_group_name'
          firstlineno 9
          lnotab 0x0202
       None
-   names      ('django', 'template', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.utils', 'get_group_name_styled', 'Library', 'register', 'filter', 'styled_group_name')
+   names      ('django', 'template', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.utils', 'get_styled_group_name', 'Library', 'register', 'filter', 'styled_group_name')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/templatetags/styled_group_name.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c020c021e030c0104ff0e01
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc` & `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/tests.py` & `punkweb_bb-0.2.3/punkweb_bb/tests.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/urls.py` & `punkweb_bb-0.2.3/punkweb_bb/urls.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb/utils.py` & `punkweb_bb-0.2.3/punkweb_bb/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,34 +14,34 @@
             counter += 1
         else:
             unique_slug_exists = False
 
     return slug
 
 
-def get_user_highest_priority_group(user):
-    groups = Group.objects.filter(user=user, style__isnull=False)
+def get_highest_priority_group(user):
+    groups = user.groups.filter(style__isnull=False)
 
     if groups.exists():
         return groups.order_by("-style__priority").first()
 
     return None
 
 
 def get_styled_username(user):
-    group = get_user_highest_priority_group(user)
+    group = get_highest_priority_group(user)
 
     if group:
         username_style = group.style.username_style
         styled_username = username_style.rendered.replace("{USER}", user.username)
         return styled_username
     else:
         return user.username
 
 
-def get_group_name_styled(group):
+def get_styled_group_name(group):
     if group.style is None:
         return group.name
     else:
         username_style = group.style.username_style
         styled_group_name = username_style.rendered.replace("{USER}", group.name)
         return styled_group_name
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/views.py` & `punkweb_bb-0.2.3/punkweb_bb/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import datetime
-
 from django.contrib.auth import authenticate, get_user_model, login, logout
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseForbidden
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils import timezone
 
@@ -494,15 +492,15 @@
     }
 
     return render(request, "punkweb_bb/partials/post_delete.html", context=context)
 
 
 def current_shouts():
     return Shout.objects.filter(
-        created_at__gt=timezone.now() - datetime.timedelta(hours=12)
+        created_at__gt=timezone.now() - timezone.timedelta(hours=12)
     ).order_by("created_at")
 
 
 def shout_list_view(request):
     shouts = current_shouts()
 
     context = {
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb/widgets.py` & `punkweb_bb-0.2.3/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.2/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.2.3/punkweb_bb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.2.2
+Version: 0.2.3
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `punkweb_bb-0.2.2/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.2.3/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 punkweb_bb/__pycache__/mixins.cpython-311.pyc
 punkweb_bb/__pycache__/models.cpython-311.pyc
 punkweb_bb/__pycache__/pagination.cpython-311.pyc
 punkweb_bb/__pycache__/parsers.cpython-311.pyc
 punkweb_bb/__pycache__/response.cpython-311.pyc
 punkweb_bb/__pycache__/settings.cpython-311.pyc
 punkweb_bb/__pycache__/signals.cpython-311.pyc
+punkweb_bb/__pycache__/sitemap.cpython-311.pyc
 punkweb_bb/__pycache__/tests.cpython-311.pyc
 punkweb_bb/__pycache__/urls.cpython-311.pyc
 punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
```

### Comparing `punkweb_bb-0.2.2/setup.py` & `punkweb_bb-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.2.2",
+    version="0.2.3",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
```

