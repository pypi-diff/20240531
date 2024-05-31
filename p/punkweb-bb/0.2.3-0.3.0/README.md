# Comparing `tmp/punkweb_bb-0.2.3.tar.gz` & `tmp/punkweb_bb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.2.3.tar", last modified: Wed May 29 23:14:11 2024, max compression
+gzip compressed data, was "punkweb_bb-0.3.0.tar", last modified: Thu May 30 22:50:22 2024, max compression
```

## Comparing `punkweb_bb-0.2.3.tar` & `punkweb_bb-0.3.0.tar`

### file list

```diff
@@ -1,290 +1,368 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.724864 punkweb_bb-0.2.3/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.3/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.3/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4441 2024-05-29 05:09:26.000000 punkweb_bb-0.2.3/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.3/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     4182 2024-05-29 19:50:24.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3531 2024-05-29 19:49:57.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    15478 2024-05-29 22:03:33.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 21:18:38.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1591 2024-05-29 22:23:50.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/sitemap.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2057 2024-05-29 21:02:46.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    25244 2024-05-29 22:01:21.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2821 2024-05-29 19:50:23.000000 punkweb_bb-0.2.3/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1372 2024-05-29 19:49:56.000000 punkweb_bb-0.2.3/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.3/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.3/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.3/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.3/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.3/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.3/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0003_alter_thread_options.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/0004_groupstyle.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.3/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     7072 2024-05-29 22:03:32.000000 punkweb_bb-0.2.3/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.3/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.3/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.3/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 21:18:30.000000 punkweb_bb-0.2.3/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.3/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.704864 punkweb_bb-0.2.3/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/category-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1686 2024-05-29 21:11:17.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.712864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.716864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10526 2024-05-29 20:04:35.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2886 2024-05-29 22:07:52.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3198 2024-05-29 22:08:57.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      802 2024-05-29 22:33:12.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     5893 2024-05-29 22:09:31.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10838 2024-05-29 22:11:05.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.720864 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 21:01:58.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_delete.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_edit.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/can_post.py
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 21:01:50.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/styled_group_name.py
--rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.2.3/punkweb_bb/templatetags/styled_username.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.3/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.3/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1200 2024-05-29 21:02:45.000000 punkweb_bb-0.2.3/punkweb_bb/utils.py
--rw-r--r--   0 pork      (1000) pork      (1000)    17383 2024-05-29 22:01:20.000000 punkweb_bb-0.2.3/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.3/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 23:14:11.708864 punkweb_bb-0.2.3/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    14850 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 23:14:11.000000 punkweb_bb-0.2.3/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 23:14:11.724864 punkweb_bb-0.2.3/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 23:13:37.000000 punkweb_bb-0.2.3/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.3.0/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.3.0/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     6172 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     5518 2024-05-30 22:33:15.000000 punkweb_bb-0.3.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.3.0/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3883 2024-05-30 20:51:38.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3605 2024-05-30 22:34:17.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6735 2024-05-30 20:41:21.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    15480 2024-05-30 20:40:50.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1111 2024-05-30 20:23:01.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1591 2024-05-29 22:23:50.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51701 2024-05-30 22:31:44.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3686 2024-05-30 02:32:29.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2794 2024-05-30 22:36:26.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    26364 2024-05-30 02:49:07.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2640 2024-05-30 22:36:37.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2686 2024-05-30 20:51:37.000000 punkweb_bb-0.3.0/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1414 2024-05-30 22:34:16.000000 punkweb_bb-0.3.0/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.3.0/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.3.0/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.3.0/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     3130 2024-05-30 20:41:20.000000 punkweb_bb-0.3.0/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.3.0/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.3.0/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0003_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0004_groupstyle.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      638 2024-05-30 02:25:42.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0005_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1699 2024-05-30 21:37:11.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      885 2024-05-30 02:25:45.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1901 2024-05-30 21:37:24.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.3.0/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     7053 2024-05-30 20:40:49.000000 punkweb_bb-0.3.0/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.3.0/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.3.0/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.3.0/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      609 2024-05-30 20:14:52.000000 punkweb_bb-0.3.0/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.3.0/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.476752 punkweb_bb-0.3.0/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     2032 2024-05-30 02:38:15.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-30 21:26:55.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      571 2024-05-30 22:36:33.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/markdown-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)      345 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.eslintrc.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1625 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore
+-rw-r--r--   0 pork      (1000) pork      (1000)        3 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.prettierrc.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1078 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)    30065 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md
+-rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/babel.config.json
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/
+-rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3749 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   454032 2024-05-30 22:21:37.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2855 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    50144 2024-05-30 22:21:37.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    41346 2024-05-30 22:21:38.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/
+-rw-r--r--   0 pork      (1000) pork      (1000)       26 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_config.yml
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/
+-rw-r--r--   0 pork      (1000) pork      (1000)     2333 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     6061 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md
+-rw-r--r--   0 pork      (1000) pork      (1000)     2919 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts
+-rw-r--r--   0 pork      (1000) pork      (1000)     5976 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/
+-rw-r--r--   0 pork      (1000) pork      (1000)    24077 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4321 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    20160 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1284 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     5645 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/
+-rw-r--r--   0 pork      (1000) pork      (1000)       40 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      300 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/server.js
+-rw-r--r--   0 pork      (1000) pork      (1000)       23 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/setup.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3506 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      141 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest-puppeteer.config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      226 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest.config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   602599 2024-05-30 20:58:03.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1983 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/
+-rw-r--r--   0 pork      (1000) pork      (1000)    69517 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8504 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1494 2024-05-30 22:21:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     2218 2024-05-30 21:33:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)       48 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    16351 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/
+-rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      107 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/index.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/
+-rw-r--r--   0 pork      (1000) pork      (1000)      557 2024-05-30 21:15:44.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      351 2024-05-30 21:10:59.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/bold.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      230 2024-05-30 21:13:22.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/clear_formatting.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 21:13:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/code.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      215 2024-05-30 21:13:44.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h1.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      305 2024-05-30 21:13:54.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h2.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      149 2024-05-30 21:14:11.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/hr.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      327 2024-05-30 21:14:18.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/image.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      192 2024-05-30 21:14:25.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/italic.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      380 2024-05-30 21:14:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/link.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:14:50.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ol.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      214 2024-05-30 21:15:26.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/strikethrough.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)     4350 2024-05-30 22:21:36.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:15:12.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ul.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)       49 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/tiny.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.476752 punkweb_bb-0.3.0/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      422 2024-05-30 02:43:33.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base_delete_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10519 2024-05-30 22:46:56.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2886 2024-05-29 22:07:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-05-30 02:46:54.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      216 2024-05-30 02:45:15.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      220 2024-05-30 02:45:33.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      246 2024-05-30 02:45:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      224 2024-05-30 02:43:57.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      746 2024-05-30 02:36:40.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/thread_move.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3203 2024-05-30 22:47:03.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-05-30 22:47:12.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5893 2024-05-30 02:20:28.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    11201 2024-05-30 22:46:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-30 21:41:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-30 21:41:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/widgets/
+-rw-r--r--   0 pork      (1000) pork      (1000)       99 2024-05-30 22:19:14.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/widgets/markdown-editor.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1858 2024-05-30 20:32:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2478 2024-05-30 22:08:38.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/render.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      945 2024-05-30 21:47:56.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1255 2024-05-30 22:35:40.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/shoutbox_render.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 21:01:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1194 2024-05-30 22:08:37.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/render.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      591 2024-05-30 22:35:38.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/shoutbox_render.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 21:01:50.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/styled_group_name.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/styled_username.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26298 2024-05-30 22:31:43.000000 punkweb_bb-0.3.0/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2673 2024-05-30 02:32:28.000000 punkweb_bb-0.3.0/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1651 2024-05-30 22:36:26.000000 punkweb_bb-0.3.0/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    18191 2024-05-30 02:49:06.000000 punkweb_bb-0.3.0/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1502 2024-05-30 22:36:36.000000 punkweb_bb-0.3.0/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6172 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    19738 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       63 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1030 2024-05-30 22:48:58.000000 punkweb_bb-0.3.0/setup.py
```

### Comparing `punkweb_bb-0.2.3/LICENSE` & `punkweb_bb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/PKG-INFO` & `punkweb_bb-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.2.3
+Version: 0.3.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -24,28 +24,43 @@
 
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
+- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
+- [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
-- Django 4.2+
+- Django 4.0+
 - django-precise-bbcode 1.2+
+- markdown 3.6+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
+## BBCode or Markdown?
+
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+
+BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+
+```python
+PUNKWEB_BB = {
+  "RENDERER": "markdown",
+}
+```
+
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
 Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
@@ -54,24 +69,15 @@
 INSTALLED_APPS = [
     ...
     "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required. It must be installed before `punkweb_bb`.
-
-Add the following middleware to your `MIDDLEWARE` setting:
-
-```python
-MIDDLEWARE = [
-    ...
-    "punkweb_bb.middleware.ProfileOnlineCacheMiddleware",
-]
-```
+_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
 
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
@@ -106,14 +112,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
+  "RENDERER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
@@ -130,43 +137,50 @@
 HTML:
 
 ```bash
 coverage run && coverage html
 ```
 
 ```bash
-Found 57 test(s).
+Found 59 test(s).
 Creating test database for alias 'default'...
 System check identified no issues (0 silenced).
-.........................................................
+...........................................................
 ----------------------------------------------------------------------
-Ran 57 tests in 8.824s
+Ran 59 tests in 9.166s
 
 OK
 Destroying test database for alias 'default'...
-Name                                         Stmts   Miss  Cover
-----------------------------------------------------------------
-punkweb_bb/__init__.py                           0      0   100%
-punkweb_bb/admin.py                             41      1    98%
-punkweb_bb/admin_forms.py                       28      0   100%
-punkweb_bb/apps.py                               6      0   100%
-punkweb_bb/bbcode_tags.py                      115      3    97%
-punkweb_bb/context_processors.py                 3      0   100%
-punkweb_bb/forms.py                             35      0   100%
-punkweb_bb/middleware.py                        10      0   100%
-punkweb_bb/mixins.py                            11      0   100%
-punkweb_bb/models.py                           124      0   100%
-punkweb_bb/pagination.py                        11      4    64%
-punkweb_bb/parsers.py                           50      2    96%
-punkweb_bb/response.py                           3      0   100%
-punkweb_bb/settings.py                           6      0   100%
-punkweb_bb/signals.py                            9      0   100%
-punkweb_bb/templatetags/__init__.py              0      0   100%
-punkweb_bb/templatetags/humanize_int.py          9      5    44%
-punkweb_bb/templatetags/shoutbox_bbcode.py       9      0   100%
-punkweb_bb/tests.py                            410      0   100%
-punkweb_bb/urls.py                               4      0   100%
-punkweb_bb/views.py                            174     17    90%
-punkweb_bb/widgets.py                            8      0   100%
-----------------------------------------------------------------
-TOTAL                                         1066     32    97%
+Name                                           Stmts   Miss  Cover
+------------------------------------------------------------------
+punkweb_bb/__init__.py                             0      0   100%
+punkweb_bb/admin.py                               43      0   100%
+punkweb_bb/admin_forms.py                         34      0   100%
+punkweb_bb/apps.py                                 6      0   100%
+punkweb_bb/context_processors.py                   3      0   100%
+punkweb_bb/forms.py                               47      0   100%
+punkweb_bb/guests.py                              13      0   100%
+punkweb_bb/middleware.py                          14      0   100%
+punkweb_bb/mixins.py                              11      0   100%
+punkweb_bb/models.py                             153      1    99%
+punkweb_bb/pagination.py                          11      4    64%
+punkweb_bb/parsers.py                             50     36    28%
+punkweb_bb/response.py                             3      0   100%
+punkweb_bb/settings.py                            11      0   100%
+punkweb_bb/signals.py                              9      0   100%
+punkweb_bb/templatetags/__init__.py                0      0   100%
+punkweb_bb/templatetags/can_delete.py              5      0   100%
+punkweb_bb/templatetags/can_edit.py                5      0   100%
+punkweb_bb/templatetags/can_post.py                5      0   100%
+punkweb_bb/templatetags/humanize_int.py            9      5    44%
+punkweb_bb/templatetags/render.py                 36     12    67%
+punkweb_bb/templatetags/shoutbox_render.py        18      2    89%
+punkweb_bb/templatetags/styled_group_name.py       7      1    86%
+punkweb_bb/templatetags/styled_username.py         6      0   100%
+punkweb_bb/tests.py                              418      0   100%
+punkweb_bb/urls.py                                 4      0   100%
+punkweb_bb/utils.py                               42     24    43%
+punkweb_bb/views.py                              304    118    61%
+punkweb_bb/widgets.py                             16      0   100%
+------------------------------------------------------------------
+TOTAL                                           1283    203    84%
 ```
```

### Comparing `punkweb_bb-0.2.3/README.md` & `punkweb_bb-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,43 @@
 
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
+- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
+- [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
-- Django 4.2+
+- Django 4.0+
 - django-precise-bbcode 1.2+
+- markdown 3.6+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
+## BBCode or Markdown?
+
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+
+BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+
+```python
+PUNKWEB_BB = {
+  "RENDERER": "markdown",
+}
+```
+
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
 Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
@@ -36,24 +51,15 @@
 INSTALLED_APPS = [
     ...
     "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required. It must be installed before `punkweb_bb`.
-
-Add the following middleware to your `MIDDLEWARE` setting:
-
-```python
-MIDDLEWARE = [
-    ...
-    "punkweb_bb.middleware.ProfileOnlineCacheMiddleware",
-]
-```
+_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
 
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
@@ -88,14 +94,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
+  "RENDERER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
@@ -112,43 +119,50 @@
 HTML:
 
 ```bash
 coverage run && coverage html
 ```
 
 ```bash
-Found 57 test(s).
+Found 59 test(s).
 Creating test database for alias 'default'...
 System check identified no issues (0 silenced).
-.........................................................
+...........................................................
 ----------------------------------------------------------------------
-Ran 57 tests in 8.824s
+Ran 59 tests in 9.166s
 
 OK
 Destroying test database for alias 'default'...
-Name                                         Stmts   Miss  Cover
-----------------------------------------------------------------
-punkweb_bb/__init__.py                           0      0   100%
-punkweb_bb/admin.py                             41      1    98%
-punkweb_bb/admin_forms.py                       28      0   100%
-punkweb_bb/apps.py                               6      0   100%
-punkweb_bb/bbcode_tags.py                      115      3    97%
-punkweb_bb/context_processors.py                 3      0   100%
-punkweb_bb/forms.py                             35      0   100%
-punkweb_bb/middleware.py                        10      0   100%
-punkweb_bb/mixins.py                            11      0   100%
-punkweb_bb/models.py                           124      0   100%
-punkweb_bb/pagination.py                        11      4    64%
-punkweb_bb/parsers.py                           50      2    96%
-punkweb_bb/response.py                           3      0   100%
-punkweb_bb/settings.py                           6      0   100%
-punkweb_bb/signals.py                            9      0   100%
-punkweb_bb/templatetags/__init__.py              0      0   100%
-punkweb_bb/templatetags/humanize_int.py          9      5    44%
-punkweb_bb/templatetags/shoutbox_bbcode.py       9      0   100%
-punkweb_bb/tests.py                            410      0   100%
-punkweb_bb/urls.py                               4      0   100%
-punkweb_bb/views.py                            174     17    90%
-punkweb_bb/widgets.py                            8      0   100%
-----------------------------------------------------------------
-TOTAL                                         1066     32    97%
+Name                                           Stmts   Miss  Cover
+------------------------------------------------------------------
+punkweb_bb/__init__.py                             0      0   100%
+punkweb_bb/admin.py                               43      0   100%
+punkweb_bb/admin_forms.py                         34      0   100%
+punkweb_bb/apps.py                                 6      0   100%
+punkweb_bb/context_processors.py                   3      0   100%
+punkweb_bb/forms.py                               47      0   100%
+punkweb_bb/guests.py                              13      0   100%
+punkweb_bb/middleware.py                          14      0   100%
+punkweb_bb/mixins.py                              11      0   100%
+punkweb_bb/models.py                             153      1    99%
+punkweb_bb/pagination.py                          11      4    64%
+punkweb_bb/parsers.py                             50     36    28%
+punkweb_bb/response.py                             3      0   100%
+punkweb_bb/settings.py                            11      0   100%
+punkweb_bb/signals.py                              9      0   100%
+punkweb_bb/templatetags/__init__.py                0      0   100%
+punkweb_bb/templatetags/can_delete.py              5      0   100%
+punkweb_bb/templatetags/can_edit.py                5      0   100%
+punkweb_bb/templatetags/can_post.py                5      0   100%
+punkweb_bb/templatetags/humanize_int.py            9      5    44%
+punkweb_bb/templatetags/render.py                 36     12    67%
+punkweb_bb/templatetags/shoutbox_render.py        18      2    89%
+punkweb_bb/templatetags/styled_group_name.py       7      1    86%
+punkweb_bb/templatetags/styled_username.py         6      0   100%
+punkweb_bb/tests.py                              418      0   100%
+punkweb_bb/urls.py                                 4      0   100%
+punkweb_bb/utils.py                               42     24    43%
+punkweb_bb/views.py                              304    118    61%
+punkweb_bb/widgets.py                             16      0   100%
+------------------------------------------------------------------
+TOTAL                                           1283    203    84%
 ```
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xff865766 (Wed May 29 19:50:23 2024 UTC)
-files sz: 2821
+moddate:  0xd9e65866 (Thu May 30 20:51:37 2024 UTC)
+files sz: 2686
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -100,161 +100,161 @@
                150 CALL                     3
    
     23         160 PRECALL                  0
                164 CALL                     0
    
     24         174 STORE_NAME              21 (BoardProfileModelAdmin)
    
-    43         176 PUSH_NULL
+    39         176 PUSH_NULL
                178 LOAD_NAME                1 (admin)
                180 LOAD_ATTR               19 (register)
                190 LOAD_NAME               13 (Category)
                192 PRECALL                  1
                196 CALL                     1
    
-    44         206 PUSH_NULL
+    40         206 PUSH_NULL
                208 LOAD_BUILD_CLASS
-               210 LOAD_CONST               7 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 43>)
+               210 LOAD_CONST               7 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 39>)
                212 MAKE_FUNCTION            0
                214 LOAD_CONST               8 ('CategoryModelAdmin')
                216 LOAD_NAME                1 (admin)
                218 LOAD_ATTR               20 (ModelAdmin)
                228 PRECALL                  3
                232 CALL                     3
    
-    43         242 PRECALL                  0
+    39         242 PRECALL                  0
                246 CALL                     0
    
-    44         256 STORE_NAME              22 (CategoryModelAdmin)
+    40         256 STORE_NAME              22 (CategoryModelAdmin)
    
-    57         258 PUSH_NULL
+    53         258 PUSH_NULL
                260 LOAD_NAME                1 (admin)
                262 LOAD_ATTR               19 (register)
                272 LOAD_NAME               17 (Subcategory)
                274 PRECALL                  1
                278 CALL                     1
    
-    58         288 PUSH_NULL
+    54         288 PUSH_NULL
                290 LOAD_BUILD_CLASS
-               292 LOAD_CONST               9 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 57>)
+               292 LOAD_CONST               9 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 53>)
                294 MAKE_FUNCTION            0
                296 LOAD_CONST              10 ('SubcategoryModelAdmin')
                298 LOAD_NAME                1 (admin)
                300 LOAD_ATTR               20 (ModelAdmin)
                310 PRECALL                  3
                314 CALL                     3
    
-    57         324 PRECALL                  0
+    53         324 PRECALL                  0
                328 CALL                     0
    
-    58         338 STORE_NAME              23 (SubcategoryModelAdmin)
+    54         338 STORE_NAME              23 (SubcategoryModelAdmin)
    
-    73         340 PUSH_NULL
+    69         340 PUSH_NULL
                342 LOAD_NAME                1 (admin)
                344 LOAD_ATTR               19 (register)
                354 LOAD_NAME               18 (Thread)
                356 PRECALL                  1
                360 CALL                     1
    
-    74         370 PUSH_NULL
+    70         370 PUSH_NULL
                372 LOAD_BUILD_CLASS
-               374 LOAD_CONST              11 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 73>)
+               374 LOAD_CONST              11 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 69>)
                376 MAKE_FUNCTION            0
                378 LOAD_CONST              12 ('ThreadModelAdmin')
                380 LOAD_NAME                1 (admin)
                382 LOAD_ATTR               20 (ModelAdmin)
                392 PRECALL                  3
                396 CALL                     3
    
-    73         406 PRECALL                  0
+    69         406 PRECALL                  0
                410 CALL                     0
    
-    74         420 STORE_NAME              24 (ThreadModelAdmin)
+    70         420 STORE_NAME              24 (ThreadModelAdmin)
    
-   100         422 PUSH_NULL
+    96         422 PUSH_NULL
                424 LOAD_NAME                1 (admin)
                426 LOAD_ATTR               19 (register)
                436 LOAD_NAME               15 (Post)
                438 PRECALL                  1
                442 CALL                     1
    
-   101         452 PUSH_NULL
+    97         452 PUSH_NULL
                454 LOAD_BUILD_CLASS
-               456 LOAD_CONST              13 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 100>)
+               456 LOAD_CONST              13 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 96>)
                458 MAKE_FUNCTION            0
                460 LOAD_CONST              14 ('PostModelAdmin')
                462 LOAD_NAME                1 (admin)
                464 LOAD_ATTR               20 (ModelAdmin)
                474 PRECALL                  3
                478 CALL                     3
    
-   100         488 PRECALL                  0
+    96         488 PRECALL                  0
                492 CALL                     0
    
-   101         502 STORE_NAME              25 (PostModelAdmin)
+    97         502 STORE_NAME              25 (PostModelAdmin)
    
-   115         504 PUSH_NULL
+   111         504 PUSH_NULL
                506 LOAD_NAME                1 (admin)
                508 LOAD_ATTR               19 (register)
                518 LOAD_NAME               16 (Shout)
                520 PRECALL                  1
                524 CALL                     1
    
-   116         534 PUSH_NULL
+   112         534 PUSH_NULL
                536 LOAD_BUILD_CLASS
-               538 LOAD_CONST              15 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 115>)
+               538 LOAD_CONST              15 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 111>)
                540 MAKE_FUNCTION            0
                542 LOAD_CONST              16 ('ShoutModelAdmin')
                544 LOAD_NAME                1 (admin)
                546 LOAD_ATTR               20 (ModelAdmin)
                556 PRECALL                  3
                560 CALL                     3
    
-   115         570 PRECALL                  0
+   111         570 PRECALL                  0
                574 CALL                     0
    
-   116         584 STORE_NAME              26 (ShoutModelAdmin)
+   112         584 STORE_NAME              26 (ShoutModelAdmin)
    
-   128         586 PUSH_NULL
+   124         586 PUSH_NULL
                588 LOAD_NAME                1 (admin)
                590 LOAD_ATTR               19 (register)
                600 LOAD_NAME               14 (GroupStyle)
                602 PRECALL                  1
                606 CALL                     1
    
-   129         616 PUSH_NULL
+   125         616 PUSH_NULL
                618 LOAD_BUILD_CLASS
-               620 LOAD_CONST              17 (<code object GroupStyleModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 128>)
+               620 LOAD_CONST              17 (<code object GroupStyleModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 124>)
                622 MAKE_FUNCTION            0
                624 LOAD_CONST              18 ('GroupStyleModelAdmin')
                626 LOAD_NAME                1 (admin)
                628 LOAD_ATTR               20 (ModelAdmin)
                638 PRECALL                  3
                642 CALL                     3
    
-   128         652 PRECALL                  0
+   124         652 PRECALL                  0
                656 CALL                     0
    
-   129         666 STORE_NAME              27 (GroupStyleModelAdmin)
+   125         666 STORE_NAME              27 (GroupStyleModelAdmin)
                668 LOAD_CONST              19 (None)
                670 RETURN_VALUE
    consts
       0
       ('admin',)
       ('mark_safe',)
       ('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm')
       ('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
-            0x970065005a0164005a0265035a0464015a0564025a0664035a0764045a
-            08640584005a0964065300
+            0x970065005a0164005a0265035a0464015a0564025a0664035a07640453
+            00
           23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfileModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
           25          10 LOAD_NAME                3 (BoardProfileAdminModelForm)
@@ -264,90 +264,55 @@
                       16 STORE_NAME               5 (list_display)
          
           27          18 LOAD_CONST               2 (('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser'))
                       20 STORE_NAME               6 (list_filter)
          
           33          22 LOAD_CONST               3 (('user__username', 'user__email'))
                       24 STORE_NAME               7 (search_fields)
-         
-          37          26 LOAD_CONST               4 (('signature_rendered',))
-                      28 STORE_NAME               8 (readonly_fields)
-         
-          39          30 LOAD_CONST               5 (<code object signature_rendered, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 39>)
-                      32 MAKE_FUNCTION            0
-                      34 STORE_NAME               9 (signature_rendered)
-                      36 LOAD_CONST               6 (None)
-                      38 RETURN_VALUE
+                      26 LOAD_CONST               4 (None)
+                      28 RETURN_VALUE
          consts
             'BoardProfileModelAdmin'
             ('user',)
             ('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser')
             ('user__username', 'user__email')
-            ('signature_rendered',)
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 3
-               flags     : 3
-               code
-                  0x97007401000000000000000000007c016a0100000000000000006a0200
-                  00000000000000a6010000ab0100000000000000005300
-                39           0 RESUME                   0
-               
-                40           2 LOAD_GLOBAL              1 (NULL + mark_safe)
-                            14 LOAD_FAST                1 (obj)
-                            16 LOAD_ATTR                1 (signature)
-                            26 LOAD_ATTR                2 (rendered)
-                            36 PRECALL                  1
-                            40 CALL                     1
-                            50 RETURN_VALUE
-               consts
-                  None
-               names      ('mark_safe', 'signature', 'rendered')
-               varnames   ('self', 'obj')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
-               name       'signature_rendered'
-               firstlineno 39
-               lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'BoardProfileAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields', 'readonly_fields', 'signature_rendered')
+         names      ('__name__', '__module__', '__qualname__', 'BoardProfileAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'BoardProfileModelAdmin'
          firstlineno 23
-         lnotab 0x0a0204010401040604040402
+         lnotab 0x0a02040104010406
       'BoardProfileModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a066403640469015a
             0764055300
-          43           0 RESUME                   0
+          39           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          45          10 LOAD_NAME                3 (CategoryAdminModelForm)
+          41          10 LOAD_NAME                3 (CategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          46          14 LOAD_CONST               1 (('name', 'order'))
+          42          14 LOAD_CONST               1 (('name', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          50          18 LOAD_CONST               2 (('name', 'description'))
+          46          18 LOAD_CONST               2 (('name', 'description'))
                       20 STORE_NAME               6 (search_fields)
          
-          54          22 LOAD_CONST               3 ('slug')
+          50          22 LOAD_CONST               3 ('slug')
                       24 LOAD_CONST               4 (('name',))
                       26 BUILD_MAP                1
                       28 STORE_NAME               7 (prepopulated_fields)
                       30 LOAD_CONST               5 (None)
                       32 RETURN_VALUE
          consts
             'CategoryModelAdmin'
@@ -358,44 +323,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'CategoryAdminModelForm', 'form', 'list_display', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'CategoryModelAdmin'
-         firstlineno 43
+         firstlineno 39
          lnotab 0x0a02040104040404
       'CategoryModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a07640464
             0569015a0864065300
-          57           0 RESUME                   0
+          53           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SubcategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          59          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
+          55          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          60          14 LOAD_CONST               1 (('name', 'category', 'order'))
+          56          14 LOAD_CONST               1 (('name', 'category', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          65          18 LOAD_CONST               2 (('category',))
+          61          18 LOAD_CONST               2 (('category',))
                       20 STORE_NAME               6 (list_filter)
          
-          66          22 LOAD_CONST               3 (('name', 'description'))
+          62          22 LOAD_CONST               3 (('name', 'description'))
                       24 STORE_NAME               7 (search_fields)
          
-          70          26 LOAD_CONST               4 ('slug')
+          66          26 LOAD_CONST               4 ('slug')
                       28 LOAD_CONST               5 (('name',))
                       30 BUILD_MAP                1
                       32 STORE_NAME               8 (prepopulated_fields)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'SubcategoryModelAdmin'
@@ -407,41 +372,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'SubcategoryAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'SubcategoryModelAdmin'
-         firstlineno 57
+         firstlineno 53
          lnotab 0x0a020401040504010404
       'SubcategoryModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a07640453
             00
-          73           0 RESUME                   0
+          69           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          75          10 LOAD_NAME                3 (ThreadAdminModelForm)
+          71          10 LOAD_NAME                3 (ThreadAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          76          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          72          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       16 STORE_NAME               5 (list_display)
          
-          85          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          81          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       20 STORE_NAME               6 (list_filter)
          
-          92          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
+          88          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
                       24 STORE_NAME               7 (search_fields)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'ThreadModelAdmin'
             ('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
             ('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
@@ -449,127 +414,127 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'ThreadAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'ThreadModelAdmin'
-         firstlineno 73
+         firstlineno 69
          lnotab 0x0a02040104090407
       'ThreadModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0265035a0464015a0564025a0664035300
-         100           0 RESUME                   0
+          96           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         102          10 LOAD_NAME                3 (PostAdminModelForm)
+          98          10 LOAD_NAME                3 (PostAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-         103          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
+          99          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
                       16 STORE_NAME               5 (list_display)
          
-         108          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         104          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
                       20 STORE_NAME               6 (search_fields)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'PostModelAdmin'
             ('thread', 'user', 'created_at')
             ('user__username', 'user__email', 'content')
             None
          names      ('__name__', '__module__', '__qualname__', 'PostAdminModelForm', 'form', 'list_display', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'PostModelAdmin'
-         firstlineno 100
+         firstlineno 96
          lnotab 0x0a0204010405
       'PostModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a0464035300
-         115           0 RESUME                   0
+         111           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ShoutModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         117          10 LOAD_CONST               1 (('user', 'created_at'))
+         113          10 LOAD_CONST               1 (('user', 'created_at'))
                       12 STORE_NAME               3 (list_display)
          
-         121          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         117          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
                       16 STORE_NAME               4 (search_fields)
                       18 LOAD_CONST               3 (None)
                       20 RETURN_VALUE
          consts
             'ShoutModelAdmin'
             ('user', 'created_at')
             ('user__username', 'user__email', 'content')
             None
          names      ('__name__', '__module__', '__qualname__', 'list_display', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'ShoutModelAdmin'
-         firstlineno 115
+         firstlineno 111
          lnotab 0x0a020404
       'ShoutModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0265035a0464015a0564025a0664035300
-         128           0 RESUME                   0
+         124           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupStyleModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         130          10 LOAD_NAME                3 (GroupStyleAdminModelForm)
+         126          10 LOAD_NAME                3 (GroupStyleAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-         131          14 LOAD_CONST               1 (('group', 'priority'))
+         127          14 LOAD_CONST               1 (('group', 'priority'))
                       16 STORE_NAME               5 (list_display)
          
-         135          18 LOAD_CONST               2 (('group__name', 'username_style'))
+         131          18 LOAD_CONST               2 (('group__name', 'username_style'))
                       20 STORE_NAME               6 (search_fields)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'GroupStyleModelAdmin'
             ('group', 'priority')
             ('group__name', 'username_style')
             None
          names      ('__name__', '__module__', '__qualname__', 'GroupStyleAdminModelForm', 'form', 'list_display', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'GroupStyleModelAdmin'
-         firstlineno 128
+         firstlineno 124
          lnotab 0x0a0204010404
       'GroupStyleModelAdmin'
       None
    names      ('django.contrib', 'admin', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.admin_forms', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread', 'register', 'ModelAdmin', 'BoardProfileModelAdmin', 'CategoryModelAdmin', 'SubcategoryModelAdmin', 'ThreadModelAdmin', 'PostModelAdmin', 'ShoutModelAdmin', 'GroupStyleModelAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c022008240b1e0124ff0e0102131e0124ff0e01020d1e
+      0x00ff02010c010c022008240b1e0124ff0e01020f1e0124ff0e01020d1e
       0124ff0e01020f1e0124ff0e01021a1e0124ff0e01020e1e0124ff0e0102
       0c1e0124ff0e01
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,27 @@
 magic:    0xa70d0d0a
-moddate:  0xe4865766 (Wed May 29 19:49:56 2024 UTC)
-files sz: 1372
+moddate:  0xe8fe5866 (Thu May 30 22:34:16 2024 UTC)
+files sz: 1414
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a066d075a076d085a080100640064036c096d0a5a0a010002
-      00470064048400640565016a0b0000000000000000a6030000ab03000000
-      00000000005a0c0200470064068400640765016a0b0000000000000000a6
-      030000ab0300000000000000005a0d0200470064088400640965016a0b00
-      00000000000000a6030000ab0300000000000000005a0e02004700640a84
-      00640b65016a0b0000000000000000a6030000ab0300000000000000005a
-      0f02004700640c8400640d65016a0b0000000000000000a6030000ab0300
-      000000000000005a1002004700640e8400640f65016a0b00000000000000
-      00a6030000ab0300000000000000005a1164105300
+      055a056d065a066d075a076d085a080100640064036c096d0a5a0a010064
+      0064046c0b6d0c5a0c01000200470064058400640665016a0d0000000000
+      000000a6030000ab0300000000000000005a0e0200470064078400640865
+      016a0d0000000000000000a6030000ab0300000000000000005a0f020047
+      0064098400640a65016a0d0000000000000000a6030000ab030000000000
+      0000005a1002004700640b8400640c65016a0d0000000000000000a60300
+      00ab0300000000000000005a1102004700640d8400640e65016a0d000000
+      0000000000a6030000ab0300000000000000005a1202004700640f840064
+      1065016a0d0000000000000000a6030000ab0300000000000000005a1364
+      115300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('forms',))
                  6 IMPORT_NAME              0 (django)
                  8 IMPORT_FROM              1 (forms)
                 10 STORE_NAME               1 (forms)
@@ -40,109 +41,117 @@
                 36 IMPORT_FROM              7 (Subcategory)
                 38 STORE_NAME               7 (Subcategory)
                 40 IMPORT_FROM              8 (Thread)
                 42 STORE_NAME               8 (Thread)
                 44 POP_TOP
    
     11          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               3 (('BBCodeEditorWidget',))
-                50 IMPORT_NAME              9 (punkweb_bb.widgets)
-                52 IMPORT_FROM             10 (BBCodeEditorWidget)
-                54 STORE_NAME              10 (BBCodeEditorWidget)
+                48 LOAD_CONST               3 (('get_editor_widget',))
+                50 IMPORT_NAME              9 (punkweb_bb.utils)
+                52 IMPORT_FROM             10 (get_editor_widget)
+                54 STORE_NAME              10 (get_editor_widget)
                 56 POP_TOP
    
-    14          58 PUSH_NULL
-                60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               4 (<code object BoardProfileAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 14>)
-                64 MAKE_FUNCTION            0
-                66 LOAD_CONST               5 ('BoardProfileAdminModelForm')
-                68 LOAD_NAME                1 (forms)
-                70 LOAD_ATTR               11 (ModelForm)
-                80 PRECALL                  3
-                84 CALL                     3
-                94 STORE_NAME              12 (BoardProfileAdminModelForm)
+    12          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               4 (('BBCodeEditorWidget',))
+                62 IMPORT_NAME             11 (punkweb_bb.widgets)
+                64 IMPORT_FROM             12 (BBCodeEditorWidget)
+                66 STORE_NAME              12 (BBCodeEditorWidget)
+                68 POP_TOP
    
-    23          96 PUSH_NULL
-                98 LOAD_BUILD_CLASS
-               100 LOAD_CONST               6 (<code object CategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 23>)
-               102 MAKE_FUNCTION            0
-               104 LOAD_CONST               7 ('CategoryAdminModelForm')
-               106 LOAD_NAME                1 (forms)
-               108 LOAD_ATTR               11 (ModelForm)
-               118 PRECALL                  3
-               122 CALL                     3
-               132 STORE_NAME              13 (CategoryAdminModelForm)
+    15          70 PUSH_NULL
+                72 LOAD_BUILD_CLASS
+                74 LOAD_CONST               5 (<code object BoardProfileAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 15>)
+                76 MAKE_FUNCTION            0
+                78 LOAD_CONST               6 ('BoardProfileAdminModelForm')
+                80 LOAD_NAME                1 (forms)
+                82 LOAD_ATTR               13 (ModelForm)
+                92 PRECALL                  3
+                96 CALL                     3
+               106 STORE_NAME              14 (BoardProfileAdminModelForm)
    
-    32         134 PUSH_NULL
-               136 LOAD_BUILD_CLASS
-               138 LOAD_CONST               8 (<code object SubcategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 32>)
-               140 MAKE_FUNCTION            0
-               142 LOAD_CONST               9 ('SubcategoryAdminModelForm')
-               144 LOAD_NAME                1 (forms)
-               146 LOAD_ATTR               11 (ModelForm)
-               156 PRECALL                  3
-               160 CALL                     3
-               170 STORE_NAME              14 (SubcategoryAdminModelForm)
+    24         108 PUSH_NULL
+               110 LOAD_BUILD_CLASS
+               112 LOAD_CONST               7 (<code object CategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 24>)
+               114 MAKE_FUNCTION            0
+               116 LOAD_CONST               8 ('CategoryAdminModelForm')
+               118 LOAD_NAME                1 (forms)
+               120 LOAD_ATTR               13 (ModelForm)
+               130 PRECALL                  3
+               134 CALL                     3
+               144 STORE_NAME              15 (CategoryAdminModelForm)
    
-    41         172 PUSH_NULL
-               174 LOAD_BUILD_CLASS
-               176 LOAD_CONST              10 (<code object ThreadAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 41>)
-               178 MAKE_FUNCTION            0
-               180 LOAD_CONST              11 ('ThreadAdminModelForm')
-               182 LOAD_NAME                1 (forms)
-               184 LOAD_ATTR               11 (ModelForm)
-               194 PRECALL                  3
-               198 CALL                     3
-               208 STORE_NAME              15 (ThreadAdminModelForm)
+    33         146 PUSH_NULL
+               148 LOAD_BUILD_CLASS
+               150 LOAD_CONST               9 (<code object SubcategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 33>)
+               152 MAKE_FUNCTION            0
+               154 LOAD_CONST              10 ('SubcategoryAdminModelForm')
+               156 LOAD_NAME                1 (forms)
+               158 LOAD_ATTR               13 (ModelForm)
+               168 PRECALL                  3
+               172 CALL                     3
+               182 STORE_NAME              16 (SubcategoryAdminModelForm)
    
-    50         210 PUSH_NULL
-               212 LOAD_BUILD_CLASS
-               214 LOAD_CONST              12 (<code object PostAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 50>)
-               216 MAKE_FUNCTION            0
-               218 LOAD_CONST              13 ('PostAdminModelForm')
-               220 LOAD_NAME                1 (forms)
-               222 LOAD_ATTR               11 (ModelForm)
-               232 PRECALL                  3
-               236 CALL                     3
-               246 STORE_NAME              16 (PostAdminModelForm)
+    42         184 PUSH_NULL
+               186 LOAD_BUILD_CLASS
+               188 LOAD_CONST              11 (<code object ThreadAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 42>)
+               190 MAKE_FUNCTION            0
+               192 LOAD_CONST              12 ('ThreadAdminModelForm')
+               194 LOAD_NAME                1 (forms)
+               196 LOAD_ATTR               13 (ModelForm)
+               206 PRECALL                  3
+               210 CALL                     3
+               220 STORE_NAME              17 (ThreadAdminModelForm)
    
-    59         248 PUSH_NULL
-               250 LOAD_BUILD_CLASS
-               252 LOAD_CONST              14 (<code object GroupStyleAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 59>)
-               254 MAKE_FUNCTION            0
-               256 LOAD_CONST              15 ('GroupStyleAdminModelForm')
-               258 LOAD_NAME                1 (forms)
-               260 LOAD_ATTR               11 (ModelForm)
-               270 PRECALL                  3
-               274 CALL                     3
-               284 STORE_NAME              17 (GroupStyleAdminModelForm)
-               286 LOAD_CONST              16 (None)
-               288 RETURN_VALUE
+    51         222 PUSH_NULL
+               224 LOAD_BUILD_CLASS
+               226 LOAD_CONST              13 (<code object PostAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 51>)
+               228 MAKE_FUNCTION            0
+               230 LOAD_CONST              14 ('PostAdminModelForm')
+               232 LOAD_NAME                1 (forms)
+               234 LOAD_ATTR               13 (ModelForm)
+               244 PRECALL                  3
+               248 CALL                     3
+               258 STORE_NAME              18 (PostAdminModelForm)
+   
+    60         260 PUSH_NULL
+               262 LOAD_BUILD_CLASS
+               264 LOAD_CONST              15 (<code object GroupStyleAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 60>)
+               266 MAKE_FUNCTION            0
+               268 LOAD_CONST              16 ('GroupStyleAdminModelForm')
+               270 LOAD_NAME                1 (forms)
+               272 LOAD_ATTR               13 (ModelForm)
+               282 PRECALL                  3
+               286 CALL                     3
+               296 STORE_NAME              19 (GroupStyleAdminModelForm)
+               298 LOAD_CONST              17 (None)
+               300 RETURN_VALUE
    consts
       0
       ('forms',)
       ('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread')
+      ('get_editor_widget',)
       ('BBCodeEditorWidget',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          14           0 RESUME                   0
+          15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfileAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          15          10 PUSH_NULL
+          16          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 15>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 16>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -152,77 +161,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                15           0 RESUME                   0
+                16           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfileAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                16          10 LOAD_NAME                3 (BoardProfile)
+                17          10 LOAD_NAME                3 (BoardProfile)
                             12 STORE_NAME               4 (model)
                
-                17          14 LOAD_CONST               1 ('__all__')
+                18          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                19          18 LOAD_CONST               2 ('signature')
+                20          18 LOAD_CONST               2 ('signature')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                18          38 BUILD_MAP                1
+                19          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'BoardProfileAdminModelForm.Meta'
                   '__all__'
                   'signature'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'BoardProfile', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'BoardProfile', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 15
+               firstlineno 16
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'BoardProfileAdminModelForm'
-         firstlineno 14
+         firstlineno 15
          lnotab 0x0a01
       'BoardProfileAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          23           0 RESUME                   0
+          24           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CategoryAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          24          10 PUSH_NULL
+          25          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 24>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 25>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -232,77 +241,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                24           0 RESUME                   0
+                25           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('CategoryAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                25          10 LOAD_NAME                3 (Category)
+                26          10 LOAD_NAME                3 (Category)
                             12 STORE_NAME               4 (model)
                
-                26          14 LOAD_CONST               1 ('__all__')
+                27          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                28          18 LOAD_CONST               2 ('description')
+                29          18 LOAD_CONST               2 ('description')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                27          38 BUILD_MAP                1
+                28          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'CategoryAdminModelForm.Meta'
                   '__all__'
                   'description'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Category', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Category', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'CategoryAdminModelForm'
-         firstlineno 23
+         firstlineno 24
          lnotab 0x0a01
       'CategoryAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          32           0 RESUME                   0
+          33           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SubcategoryAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          33          10 PUSH_NULL
+          34          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 33>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 34>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -312,77 +321,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                33           0 RESUME                   0
+                34           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('SubcategoryAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                34          10 LOAD_NAME                3 (Subcategory)
+                35          10 LOAD_NAME                3 (Subcategory)
                             12 STORE_NAME               4 (model)
                
-                35          14 LOAD_CONST               1 ('__all__')
+                36          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                37          18 LOAD_CONST               2 ('description')
+                38          18 LOAD_CONST               2 ('description')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                36          38 BUILD_MAP                1
+                37          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'SubcategoryAdminModelForm.Meta'
                   '__all__'
                   'description'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Subcategory', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Subcategory', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 33
+               firstlineno 34
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'SubcategoryAdminModelForm'
-         firstlineno 32
+         firstlineno 33
          lnotab 0x0a01
       'SubcategoryAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          41           0 RESUME                   0
+          42           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          42          10 PUSH_NULL
+          43          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 42>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 43>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -392,77 +401,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                42           0 RESUME                   0
+                43           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ThreadAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                43          10 LOAD_NAME                3 (Thread)
+                44          10 LOAD_NAME                3 (Thread)
                             12 STORE_NAME               4 (model)
                
-                44          14 LOAD_CONST               1 ('__all__')
+                45          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                46          18 LOAD_CONST               2 ('content')
+                47          18 LOAD_CONST               2 ('content')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                45          38 BUILD_MAP                1
+                46          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'ThreadAdminModelForm.Meta'
                   '__all__'
                   'content'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Thread', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Thread', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 42
+               firstlineno 43
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'ThreadAdminModelForm'
-         firstlineno 41
+         firstlineno 42
          lnotab 0x0a01
       'ThreadAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          50           0 RESUME                   0
+          51           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          51          10 PUSH_NULL
+          52          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 51>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 52>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -472,77 +481,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                51           0 RESUME                   0
+                52           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('PostAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                52          10 LOAD_NAME                3 (Post)
+                53          10 LOAD_NAME                3 (Post)
                             12 STORE_NAME               4 (model)
                
-                53          14 LOAD_CONST               1 ('__all__')
+                54          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                55          18 LOAD_CONST               2 ('content')
+                56          18 LOAD_CONST               2 ('content')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                54          38 BUILD_MAP                1
+                55          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'PostAdminModelForm.Meta'
                   '__all__'
                   'content'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Post', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Post', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 51
+               firstlineno 52
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'PostAdminModelForm'
-         firstlineno 50
+         firstlineno 51
          lnotab 0x0a01
       'PostAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          59           0 RESUME                   0
+          60           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupStyleAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          60          10 PUSH_NULL
+          61          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 60>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 61>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -552,62 +561,62 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                60           0 RESUME                   0
+                61           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('GroupStyleAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                61          10 LOAD_NAME                3 (GroupStyle)
+                62          10 LOAD_NAME                3 (GroupStyle)
                             12 STORE_NAME               4 (model)
                
-                62          14 LOAD_CONST               1 ('__all__')
+                63          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                64          18 LOAD_CONST               2 ('username_style')
+                65          18 LOAD_CONST               2 ('username_style')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                63          38 BUILD_MAP                1
+                64          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'GroupStyleAdminModelForm.Meta'
                   '__all__'
                   'username_style'
                   None
                names      ('__name__', '__module__', '__qualname__', 'GroupStyle', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 60
+               firstlineno 61
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'GroupStyleAdminModelForm'
-         firstlineno 59
+         firstlineno 60
          lnotab 0x0a01
       'GroupStyleAdminModelForm'
       None
-   names      ('django', 'forms', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'ModelForm', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'PostAdminModelForm', 'GroupStyleAdminModelForm')
+   names      ('django', 'forms', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread', 'punkweb_bb.utils', 'get_editor_widget', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'ModelForm', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'PostAdminModelForm', 'GroupStyleAdminModelForm')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0220080c0326092609260926092609
+   lnotab 0x00ff02010c0220080c010c0326092609260926092609
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x074f5666 (Tue May 28 21:39:19 2024 UTC)
-files sz: 2907
+moddate:  0x70e45866 (Thu May 30 20:41:20 2024 UTC)
+files sz: 3130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -14,16 +14,17 @@
       0300000000000000005a0f0200470064098400640a65016a100000000000
       000000a6030000ab0300000000000000005a1102004700640b8400640c65
       016a100000000000000000a6030000ab0300000000000000005a12020047
       00640d8400640e65016a100000000000000000a6030000ab030000000000
       0000005a1302004700640f8400641065016a100000000000000000a60300
       00ab0300000000000000005a140200470064118400641265016a10000000
       0000000000a6030000ab0300000000000000005a15020047006413840064
-      1465016a100000000000000000a6030000ab0300000000000000005a1664
-      155300
+      1465016a100000000000000000a6030000ab0300000000000000005a1602
+      00470064158400641665016a170000000000000000a6030000ab03000000
+      00000000005a1864175300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('forms',))
                  6 IMPORT_NAME              0 (django)
                  8 IMPORT_FROM              1 (forms)
                 10 STORE_NAME               1 (forms)
@@ -52,18 +53,18 @@
                 52 IMPORT_FROM             10 (Subcategory)
                 54 STORE_NAME              10 (Subcategory)
                 56 IMPORT_FROM             11 (Thread)
                 58 STORE_NAME              11 (Thread)
                 60 POP_TOP
    
      5          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               4 (('BBCodeEditorWidget',))
-                66 IMPORT_NAME             12 (punkweb_bb.widgets)
-                68 IMPORT_FROM             13 (BBCodeEditorWidget)
-                70 STORE_NAME              13 (BBCodeEditorWidget)
+                64 LOAD_CONST               4 (('get_editor_widget',))
+                66 IMPORT_NAME             12 (punkweb_bb.utils)
+                68 IMPORT_FROM             13 (get_editor_widget)
+                70 STORE_NAME              13 (get_editor_widget)
                 72 POP_TOP
    
      8          74 PUSH_NULL
                 76 LOAD_BUILD_CLASS
                 78 LOAD_CONST               5 (<code object LoginForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py", line 8>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               6 ('LoginForm')
@@ -143,22 +144,33 @@
                326 MAKE_FUNCTION            0
                328 LOAD_CONST              20 ('ThreadModelForm')
                330 LOAD_NAME                1 (forms)
                332 LOAD_ATTR               16 (ModelForm)
                342 PRECALL                  3
                346 CALL                     3
                356 STORE_NAME              22 (ThreadModelForm)
-               358 LOAD_CONST              21 (None)
-               360 RETURN_VALUE
+   
+   110         358 PUSH_NULL
+               360 LOAD_BUILD_CLASS
+               362 LOAD_CONST              21 (<code object ThreadMoveForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py", line 110>)
+               364 MAKE_FUNCTION            0
+               366 LOAD_CONST              22 ('ThreadMoveForm')
+               368 LOAD_NAME                1 (forms)
+               370 LOAD_ATTR               23 (Form)
+               380 PRECALL                  3
+               384 CALL                     3
+               394 STORE_NAME              24 (ThreadMoveForm)
+               396 LOAD_CONST              23 (None)
+               398 RETURN_VALUE
    consts
       0
       ('forms',)
       ('AuthenticationForm', 'UserCreationForm')
       ('BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread')
-      ('BBCodeEditorWidget',)
+      ('get_editor_widget',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
@@ -449,28 +461,28 @@
                             12 STORE_NAME               4 (model)
                
                 37          14 LOAD_CONST               1 (('image', 'signature'))
                             16 STORE_NAME               5 (fields)
                
                 42          18 LOAD_CONST               2 ('signature')
                             20 PUSH_NULL
-                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            22 LOAD_NAME                6 (get_editor_widget)
                             24 PRECALL                  0
                             28 CALL                     0
                
                 41          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'BoardProfileModelForm.Meta'
                   ('image', 'signature')
                   'signature'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'BoardProfile', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'BoardProfile', 'model', 'fields', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
                name       'Meta'
                firstlineno 35
                lnotab 0x0a010401040514ff
@@ -643,29 +655,29 @@
                             20 LOAD_CONST               3 ('')
                
                 65          22 BUILD_MAP                1
                             24 STORE_NAME               6 (labels)
                
                 69          26 LOAD_CONST               2 ('content')
                             28 PUSH_NULL
-                            30 LOAD_NAME                7 (BBCodeEditorWidget)
+                            30 LOAD_NAME                7 (get_editor_widget)
                             32 PRECALL                  0
                             36 CALL                     0
                
                 68          46 BUILD_MAP                1
                             48 STORE_NAME               8 (widgets)
                             50 LOAD_CONST               4 (None)
                             52 RETURN_VALUE
                consts
                   'PostModelForm.Meta'
                   ('content',)
                   'content'
                   ''
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Post', 'model', 'fields', 'labels', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Post', 'model', 'fields', 'labels', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
                name       'Meta'
                firstlineno 62
                lnotab 0x0a010401040204ff040414ff
@@ -805,15 +817,15 @@
                             36 LOAD_CONST               4 (('autofocus', 'class'))
                             38 BUILD_CONST_KEY_MAP      2
                             40 KW_NAMES                 5
                             42 PRECALL                  1
                             46 CALL                     1
                
                 90          56 PUSH_NULL
-                            58 LOAD_NAME                8 (BBCodeEditorWidget)
+                            58 LOAD_NAME                8 (get_editor_widget)
                             60 PRECALL                  0
                             64 CALL                     0
                
                 91          74 PUSH_NULL
                             76 LOAD_NAME                6 (forms)
                             78 LOAD_ATTR                7 (TextInput)
                
@@ -840,15 +852,15 @@
                   ('autofocus', 'class')
                   ('attrs',)
                   '0'
                   'number'
                   ('class', 'min', 'type')
                   ('name', 'description', 'order')
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Subcategory', 'model', 'fields', 'forms', 'TextInput', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Subcategory', 'model', 'fields', 'forms', 'TextInput', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
                name       'Meta'
                firstlineno 80
                lnotab 0x0a0104010407260112010e010aff10fd
@@ -918,15 +930,15 @@
                             36 LOAD_CONST               4 (('autofocus', 'class'))
                             38 BUILD_CONST_KEY_MAP      2
                             40 KW_NAMES                 5
                             42 PRECALL                  1
                             46 CALL                     1
                
                106          56 PUSH_NULL
-                            58 LOAD_NAME                8 (BBCodeEditorWidget)
+                            58 LOAD_NAME                8 (get_editor_widget)
                             60 PRECALL                  0
                             64 CALL                     0
                
                104          74 LOAD_CONST               1 (('title', 'content'))
                             76 BUILD_CONST_KEY_MAP      2
                             78 STORE_NAME               9 (widgets)
                             80 LOAD_CONST               6 (None)
@@ -935,15 +947,15 @@
                   'ThreadModelForm.Meta'
                   ('title', 'content')
                   True
                   'pw-input'
                   ('autofocus', 'class')
                   ('attrs',)
                   None
-               names      ('__name__', '__module__', '__qualname__', 'Thread', 'model', 'fields', 'forms', 'TextInput', 'BBCodeEditorWidget', 'widgets')
+               names      ('__name__', '__module__', '__qualname__', 'Thread', 'model', 'fields', 'forms', 'TextInput', 'get_editor_widget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
                name       'Meta'
                firstlineno 98
                lnotab 0x0a0104010405260112fe
@@ -954,16 +966,78 @@
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
          name       'ThreadModelForm'
          firstlineno 97
          lnotab 0x0a01
       'ThreadModelForm'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 8
+         flags     : 0
+         code
+            0x970065005a0164005a02020065036a04000000000000000065056a0600
+            00000000000000a0070000000000000000000000000000000000000000a6
+            000000ab0000000000000000006401020065036a08000000000000000064
+            0264036901ac04a6010000ab010000000000000000ac05a6030000ab0300
+            000000000000005a0964065300
+         110           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('ThreadMoveForm')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         111          10 PUSH_NULL
+                      12 LOAD_NAME                3 (forms)
+                      14 LOAD_ATTR                4 (ModelChoiceField)
+         
+         112          24 LOAD_NAME                5 (Subcategory)
+                      26 LOAD_ATTR                6 (objects)
+                      36 LOAD_METHOD              7 (all)
+                      58 PRECALL                  0
+                      62 CALL                     0
+         
+         113          72 LOAD_CONST               1 ('Select a subcategory')
+         
+         114          74 PUSH_NULL
+                      76 LOAD_NAME                3 (forms)
+                      78 LOAD_ATTR                8 (Select)
+                      88 LOAD_CONST               2 ('class')
+                      90 LOAD_CONST               3 ('pw-input')
+                      92 BUILD_MAP                1
+                      94 KW_NAMES                 4
+                      96 PRECALL                  1
+                     100 CALL                     1
+         
+         111         110 KW_NAMES                 5
+                     112 PRECALL                  3
+                     116 CALL                     3
+                     126 STORE_NAME               9 (subcategory)
+                     128 LOAD_CONST               6 (None)
+                     130 RETURN_VALUE
+         consts
+            'ThreadMoveForm'
+            'Select a subcategory'
+            'class'
+            'pw-input'
+            ('attrs',)
+            ('queryset', 'empty_label', 'widget')
+            None
+         names      ('__name__', '__module__', '__qualname__', 'forms', 'ModelChoiceField', 'Subcategory', 'objects', 'all', 'Select', 'subcategory')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
+         name       'ThreadMoveForm'
+         firstlineno 110
+         lnotab 0x0a010e013001020124fd
+      'ThreadMoveForm'
       None
-   names      ('django', 'forms', 'django.contrib.auth.forms', 'AuthenticationForm', 'UserCreationForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'LoginForm', 'SignUpForm', 'ModelForm', 'BoardProfileModelForm', 'CategoryModelForm', 'PostModelForm', 'ShoutModelForm', 'SubcategoryModelForm', 'ThreadModelForm')
+   names      ('django', 'forms', 'django.contrib.auth.forms', 'AuthenticationForm', 'UserCreationForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.utils', 'get_editor_widget', 'LoginForm', 'SignUpForm', 'ModelForm', 'BoardProfileModelForm', 'CategoryModelForm', 'PostModelForm', 'ShoutModelForm', 'SubcategoryModelForm', 'ThreadModelForm', 'Form', 'ThreadMoveForm')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/forms.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c01100220010c031c0f1c0b260c260f260c26062612
+   lnotab 0x00ff02010c01100220010c031c0f1c0b260c260f260c26062612260d
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0x34a65766 (Wed May 29 22:03:32 2024 UTC)
-files sz: 7072
+moddate:  0x51e45866 (Thu May 30 20:40:49 2024 UTC)
+files sz: 7053
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
       00640064036c046d055a050100640064046c066d075a070100640064056c
       086d095a090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d01
-      00640064086c0e6d0f5a0f0100640064096c106d115a1101006400640a6c
-      126d135a136d145a1401006400640b6c156d165a166d175a170100020065
-      03a6000000ab0000000000000000005a18640c84005a1902004700640d84
-      00640e65146513a6040000ab0400000000000000005a1a02004700640f84
-      00641065146513a6040000ab0400000000000000005a1b02004700641184
-      00641265146513a6040000ab0400000000000000005a1c02004700641384
-      00641465146513a6040000ab0400000000000000005a1d02004700641584
-      00641665146513a6040000ab0400000000000000005a1e02004700641784
-      00641865146513a6040000ab0400000000000000005a1f02004700641984
-      00641a65146513a6040000ab0400000000000000005a2064015300
+      00640064086c0e6d0f5a0f0100640064096c106d115a116d125a12010064
+      00640a6c136d145a146d155a15010002006503a6000000ab000000000000
+      0000005a16640b84005a1702004700640c8400640d65126511a6040000ab
+      0400000000000000005a1802004700640e8400640f65126511a6040000ab
+      0400000000000000005a190200470064108400641165126511a6040000ab
+      0400000000000000005a1a0200470064128400641365126511a6040000ab
+      0400000000000000005a1b0200470064148400641565126511a6040000ab
+      0400000000000000005a1c0200470064168400641765126511a6040000ab
+      0400000000000000005a1d0200470064188400641965126511a6040000ab
+      0400000000000000005a1e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (math)
                  8 STORE_NAME               0 (math)
    
@@ -77,163 +77,155 @@
     10          90 LOAD_CONST               0 (0)
                 92 LOAD_CONST               8 (('timezone',))
                 94 IMPORT_NAME             14 (django.utils)
                 96 IMPORT_FROM             15 (timezone)
                 98 STORE_NAME              15 (timezone)
                100 POP_TOP
    
-    11         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               9 (('BBCodeTextField',))
-               106 IMPORT_NAME             16 (precise_bbcode.fields)
-               108 IMPORT_FROM             17 (BBCodeTextField)
-               110 STORE_NAME              17 (BBCodeTextField)
-               112 POP_TOP
-   
-    13         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST              10 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
-               118 IMPORT_NAME             18 (punkweb_bb.mixins)
-               120 IMPORT_FROM             19 (TimestampMixin)
-               122 STORE_NAME              19 (TimestampMixin)
-               124 IMPORT_FROM             20 (UUIDPrimaryKeyMixin)
-               126 STORE_NAME              20 (UUIDPrimaryKeyMixin)
-               128 POP_TOP
-   
-    14         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              11 (('get_highest_priority_group', 'get_styled_username'))
-               134 IMPORT_NAME             21 (punkweb_bb.utils)
-               136 IMPORT_FROM             22 (get_highest_priority_group)
-               138 STORE_NAME              22 (get_highest_priority_group)
-               140 IMPORT_FROM             23 (get_styled_username)
-               142 STORE_NAME              23 (get_styled_username)
-               144 POP_TOP
-   
-    16         146 PUSH_NULL
-               148 LOAD_NAME                3 (get_user_model)
-               150 PRECALL                  0
-               154 CALL                     0
-               164 STORE_NAME              24 (User)
-   
-    19         166 LOAD_CONST              12 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 19>)
-               168 MAKE_FUNCTION            0
-               170 STORE_NAME              25 (profile_image_upload_to)
-   
-    24         172 PUSH_NULL
-               174 LOAD_BUILD_CLASS
-               176 LOAD_CONST              13 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 24>)
-               178 MAKE_FUNCTION            0
-               180 LOAD_CONST              14 ('BoardProfile')
-               182 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               184 LOAD_NAME               19 (TimestampMixin)
-               186 PRECALL                  4
-               190 CALL                     4
-               200 STORE_NAME              26 (BoardProfile)
-   
-    55         202 PUSH_NULL
-               204 LOAD_BUILD_CLASS
-               206 LOAD_CONST              15 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 55>)
-               208 MAKE_FUNCTION            0
-               210 LOAD_CONST              16 ('Category')
-               212 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               214 LOAD_NAME               19 (TimestampMixin)
-               216 PRECALL                  4
-               220 CALL                     4
-               230 STORE_NAME              27 (Category)
-   
-    73         232 PUSH_NULL
-               234 LOAD_BUILD_CLASS
-               236 LOAD_CONST              17 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 73>)
-               238 MAKE_FUNCTION            0
-               240 LOAD_CONST              18 ('Subcategory')
-               242 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               244 LOAD_NAME               19 (TimestampMixin)
-               246 PRECALL                  4
-               250 CALL                     4
-               260 STORE_NAME              28 (Subcategory)
-   
-   113         262 PUSH_NULL
-               264 LOAD_BUILD_CLASS
-               266 LOAD_CONST              19 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 113>)
-               268 MAKE_FUNCTION            0
-               270 LOAD_CONST              20 ('Thread')
-               272 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               274 LOAD_NAME               19 (TimestampMixin)
-               276 PRECALL                  4
-               280 CALL                     4
-               290 STORE_NAME              29 (Thread)
-   
-   160         292 PUSH_NULL
-               294 LOAD_BUILD_CLASS
-               296 LOAD_CONST              21 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 160>)
-               298 MAKE_FUNCTION            0
-               300 LOAD_CONST              22 ('Post')
-               302 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               304 LOAD_NAME               19 (TimestampMixin)
-               306 PRECALL                  4
-               310 CALL                     4
-               320 STORE_NAME              30 (Post)
-   
-   205         322 PUSH_NULL
-               324 LOAD_BUILD_CLASS
-               326 LOAD_CONST              23 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 205>)
-               328 MAKE_FUNCTION            0
-               330 LOAD_CONST              24 ('Shout')
-               332 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               334 LOAD_NAME               19 (TimestampMixin)
-               336 PRECALL                  4
-               340 CALL                     4
-               350 STORE_NAME              31 (Shout)
-   
-   219         352 PUSH_NULL
-               354 LOAD_BUILD_CLASS
-               356 LOAD_CONST              25 (<code object GroupStyle, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 219>)
-               358 MAKE_FUNCTION            0
-               360 LOAD_CONST              26 ('GroupStyle')
-               362 LOAD_NAME               20 (UUIDPrimaryKeyMixin)
-               364 LOAD_NAME               19 (TimestampMixin)
-               366 PRECALL                  4
-               370 CALL                     4
-               380 STORE_NAME              32 (GroupStyle)
-               382 LOAD_CONST               1 (None)
-               384 RETURN_VALUE
+    12         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               9 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
+               106 IMPORT_NAME             16 (punkweb_bb.mixins)
+               108 IMPORT_FROM             17 (TimestampMixin)
+               110 STORE_NAME              17 (TimestampMixin)
+               112 IMPORT_FROM             18 (UUIDPrimaryKeyMixin)
+               114 STORE_NAME              18 (UUIDPrimaryKeyMixin)
+               116 POP_TOP
+   
+    13         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST              10 (('get_highest_priority_group', 'get_styled_username'))
+               122 IMPORT_NAME             19 (punkweb_bb.utils)
+               124 IMPORT_FROM             20 (get_highest_priority_group)
+               126 STORE_NAME              20 (get_highest_priority_group)
+               128 IMPORT_FROM             21 (get_styled_username)
+               130 STORE_NAME              21 (get_styled_username)
+               132 POP_TOP
+   
+    15         134 PUSH_NULL
+               136 LOAD_NAME                3 (get_user_model)
+               138 PRECALL                  0
+               142 CALL                     0
+               152 STORE_NAME              22 (User)
+   
+    18         154 LOAD_CONST              11 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 18>)
+               156 MAKE_FUNCTION            0
+               158 STORE_NAME              23 (profile_image_upload_to)
+   
+    23         160 PUSH_NULL
+               162 LOAD_BUILD_CLASS
+               164 LOAD_CONST              12 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 23>)
+               166 MAKE_FUNCTION            0
+               168 LOAD_CONST              13 ('BoardProfile')
+               170 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               172 LOAD_NAME               17 (TimestampMixin)
+               174 PRECALL                  4
+               178 CALL                     4
+               188 STORE_NAME              24 (BoardProfile)
+   
+    54         190 PUSH_NULL
+               192 LOAD_BUILD_CLASS
+               194 LOAD_CONST              14 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 54>)
+               196 MAKE_FUNCTION            0
+               198 LOAD_CONST              15 ('Category')
+               200 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               202 LOAD_NAME               17 (TimestampMixin)
+               204 PRECALL                  4
+               208 CALL                     4
+               218 STORE_NAME              25 (Category)
+   
+    72         220 PUSH_NULL
+               222 LOAD_BUILD_CLASS
+               224 LOAD_CONST              16 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 72>)
+               226 MAKE_FUNCTION            0
+               228 LOAD_CONST              17 ('Subcategory')
+               230 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               232 LOAD_NAME               17 (TimestampMixin)
+               234 PRECALL                  4
+               238 CALL                     4
+               248 STORE_NAME              26 (Subcategory)
+   
+   112         250 PUSH_NULL
+               252 LOAD_BUILD_CLASS
+               254 LOAD_CONST              18 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 112>)
+               256 MAKE_FUNCTION            0
+               258 LOAD_CONST              19 ('Thread')
+               260 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               262 LOAD_NAME               17 (TimestampMixin)
+               264 PRECALL                  4
+               268 CALL                     4
+               278 STORE_NAME              27 (Thread)
+   
+   160         280 PUSH_NULL
+               282 LOAD_BUILD_CLASS
+               284 LOAD_CONST              20 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 160>)
+               286 MAKE_FUNCTION            0
+               288 LOAD_CONST              21 ('Post')
+               290 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               292 LOAD_NAME               17 (TimestampMixin)
+               294 PRECALL                  4
+               298 CALL                     4
+               308 STORE_NAME              28 (Post)
+   
+   205         310 PUSH_NULL
+               312 LOAD_BUILD_CLASS
+               314 LOAD_CONST              22 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 205>)
+               316 MAKE_FUNCTION            0
+               318 LOAD_CONST              23 ('Shout')
+               320 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               322 LOAD_NAME               17 (TimestampMixin)
+               324 PRECALL                  4
+               328 CALL                     4
+               338 STORE_NAME              29 (Shout)
+   
+   219         340 PUSH_NULL
+               342 LOAD_BUILD_CLASS
+               344 LOAD_CONST              24 (<code object GroupStyle, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 219>)
+               346 MAKE_FUNCTION            0
+               348 LOAD_CONST              25 ('GroupStyle')
+               350 LOAD_NAME               18 (UUIDPrimaryKeyMixin)
+               352 LOAD_NAME               17 (TimestampMixin)
+               354 PRECALL                  4
+               358 CALL                     4
+               368 STORE_NAME              30 (GroupStyle)
+               370 LOAD_CONST               1 (None)
+               372 RETURN_VALUE
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
-      ('BBCodeTextField',)
       ('TimestampMixin', 'UUIDPrimaryKeyMixin')
       ('get_highest_priority_group', 'get_styled_username')
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
-          19           0 RESUME                   0
+          18           0 RESUME                   0
          
-          20           2 LOAD_GLOBAL              0 (os)
+          19           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (splitext)
                       46 LOAD_FAST                1 (filename)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_CONST               1 (-1)
                       64 BINARY_SUBSCR
                       74 STORE_FAST               2 (ext)
          
-          21          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
+          20          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
                       78 LOAD_FAST                0 (instance)
                       80 LOAD_ATTR                3 (user)
                       90 LOAD_ATTR                4 (username)
                      100 FORMAT_VALUE             0
                      102 LOAD_CONST               3 ('/image')
                      104 LOAD_FAST                2 (ext)
                      106 FORMAT_VALUE             0
@@ -246,286 +238,286 @@
             '/image'
          names      ('os', 'path', 'splitext', 'user', 'username')
          varnames   ('instance', 'filename', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'profile_image_upload_to'
-         firstlineno 19
+         firstlineno 18
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
-            00000000005a0a0200650b640564036403ac06a6030000ab030000000000
-            0000005a0c02004700640784006408a6020000ab0200000000000000005a
-            0d650e64098400a6000000ab0000000000000000005a0f650e640a8400a6
-            000000ab0000000000000000005a10650e640b8400a6000000ab00000000
-            00000000005a11650e640c8400a6000000ab0000000000000000005a1264
-            0d84005a13640e5300
-          24           0 RESUME                   0
+            00000000005a0a020065036a0b000000000000000064056403ac06a60200
+            00ab0200000000000000005a0c02004700640784006408a6020000ab0200
+            000000000000005a0d650e64098400a6000000ab0000000000000000005a
+            0f650e640a8400a6000000ab0000000000000000005a10650e640b8400a6
+            000000ab0000000000000000005a11650e640c8400a6000000ab00000000
+            00000000005a12640d84005a13640e5300
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfile')
                        8 STORE_NAME               2 (__qualname__)
          
-          25          10 PUSH_NULL
+          24          10 PUSH_NULL
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
          
-          26          58 PUSH_NULL
+          25          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (ImageField)
                       72 LOAD_NAME                9 (profile_image_upload_to)
                       74 LOAD_CONST               3 (True)
                       76 LOAD_CONST               3 (True)
                       78 KW_NAMES                 4
                       80 PRECALL                  3
                       84 CALL                     3
                       94 STORE_NAME              10 (image)
          
-          27          96 PUSH_NULL
-                      98 LOAD_NAME               11 (BBCodeTextField)
-                     100 LOAD_CONST               5 (1024)
-                     102 LOAD_CONST               3 (True)
-                     104 LOAD_CONST               3 (True)
-                     106 KW_NAMES                 6
-                     108 PRECALL                  3
-                     112 CALL                     3
-                     122 STORE_NAME              12 (signature)
-         
-          29         124 PUSH_NULL
-                     126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 29>)
-                     130 MAKE_FUNCTION            0
-                     132 LOAD_CONST               8 ('Meta')
-                     134 PRECALL                  2
-                     138 CALL                     2
-                     148 STORE_NAME              13 (Meta)
+          26          96 PUSH_NULL
+                      98 LOAD_NAME                3 (models)
+                     100 LOAD_ATTR               11 (TextField)
+                     110 LOAD_CONST               5 (1024)
+                     112 LOAD_CONST               3 (True)
+                     114 KW_NAMES                 6
+                     116 PRECALL                  2
+                     120 CALL                     2
+                     130 STORE_NAME              12 (signature)
+         
+          28         132 PUSH_NULL
+                     134 LOAD_BUILD_CLASS
+                     136 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 28>)
+                     138 MAKE_FUNCTION            0
+                     140 LOAD_CONST               8 ('Meta')
+                     142 PRECALL                  2
+                     146 CALL                     2
+                     156 STORE_NAME              13 (Meta)
          
-          32         150 LOAD_NAME               14 (property)
+          31         158 LOAD_NAME               14 (property)
          
-          33         152 LOAD_CONST               9 (<code object priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 32>)
-                     154 MAKE_FUNCTION            0
+          32         160 LOAD_CONST               9 (<code object priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 31>)
+                     162 MAKE_FUNCTION            0
          
-          32         156 PRECALL                  0
-                     160 CALL                     0
+          31         164 PRECALL                  0
+                     168 CALL                     0
          
-          33         170 STORE_NAME              15 (priority_group)
+          32         178 STORE_NAME              15 (priority_group)
          
-          36         172 LOAD_NAME               14 (property)
+          35         180 LOAD_NAME               14 (property)
          
-          37         174 LOAD_CONST              10 (<code object styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 36>)
-                     176 MAKE_FUNCTION            0
+          36         182 LOAD_CONST              10 (<code object styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 35>)
+                     184 MAKE_FUNCTION            0
          
-          36         178 PRECALL                  0
-                     182 CALL                     0
+          35         186 PRECALL                  0
+                     190 CALL                     0
          
-          37         192 STORE_NAME              16 (styled_username)
+          36         200 STORE_NAME              16 (styled_username)
          
-          40         194 LOAD_NAME               14 (property)
+          39         202 LOAD_NAME               14 (property)
          
-          41         196 LOAD_CONST              11 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 40>)
-                     198 MAKE_FUNCTION            0
+          40         204 LOAD_CONST              11 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 39>)
+                     206 MAKE_FUNCTION            0
          
-          40         200 PRECALL                  0
-                     204 CALL                     0
+          39         208 PRECALL                  0
+                     212 CALL                     0
          
-          41         214 STORE_NAME              17 (is_online)
+          40         222 STORE_NAME              17 (is_online)
          
-          47         216 LOAD_NAME               14 (property)
+          46         224 LOAD_NAME               14 (property)
          
-          48         218 LOAD_CONST              12 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 47>)
-                     220 MAKE_FUNCTION            0
+          47         226 LOAD_CONST              12 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 46>)
+                     228 MAKE_FUNCTION            0
          
-          47         222 PRECALL                  0
-                     226 CALL                     0
+          46         230 PRECALL                  0
+                     234 CALL                     0
          
-          48         236 STORE_NAME              18 (post_count)
+          47         244 STORE_NAME              18 (post_count)
          
-          51         238 LOAD_CONST              13 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 51>)
-                     240 MAKE_FUNCTION            0
-                     242 STORE_NAME              19 (__str__)
-                     244 LOAD_CONST              14 (None)
-                     246 RETURN_VALUE
+          50         246 LOAD_CONST              13 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 50>)
+                     248 MAKE_FUNCTION            0
+                     250 STORE_NAME              19 (__str__)
+                     252 LOAD_CONST              14 (None)
+                     254 RETURN_VALUE
          consts
             'BoardProfile'
             'profile'
             ('related_name', 'on_delete')
             True
             ('upload_to', 'blank', 'null')
             1024
-            ('max_length', 'blank', 'null')
+            ('max_length', 'blank')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                29           0 RESUME                   0
+                28           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfile.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                30          10 LOAD_CONST               1 (('user__username',))
+                29          10 LOAD_CONST               1 (('user__username',))
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
-               firstlineno 29
+               firstlineno 28
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
-                32           0 RESUME                   0
+                31           0 RESUME                   0
                
-                34           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
+                33           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (user)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('get_highest_priority_group', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'priority_group'
-               firstlineno 32
+               firstlineno 31
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                36           0 RESUME                   0
+                35           0 RESUME                   0
                
-                38           2 LOAD_GLOBAL              1 (NULL + get_styled_username)
+                37           2 LOAD_GLOBAL              1 (NULL + get_styled_username)
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
-               firstlineno 36
+               firstlineno 35
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
                   0000000000000000007c017407000000000000000000006a050000000000
                   0000006402ac03a6010000ab0100000000000000007a0000006b00000000
                   00530064045300
-                40           0 RESUME                   0
+                39           0 RESUME                   0
                
-                42           2 LOAD_GLOBAL              1 (NULL + cache)
+                41           2 LOAD_GLOBAL              1 (NULL + cache)
                             14 LOAD_ATTR                1 (get)
                             24 LOAD_CONST               1 ('profile_online_')
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (id)
                             38 FORMAT_VALUE             0
                             40 BUILD_STRING             2
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               1 (last_seen)
                
-                43          58 LOAD_FAST                1 (last_seen)
+                42          58 LOAD_FAST                1 (last_seen)
                             60 POP_JUMP_FORWARD_IF_FALSE    45 (to 152)
                
-                44          62 LOAD_GLOBAL              7 (NULL + timezone)
+                43          62 LOAD_GLOBAL              7 (NULL + timezone)
                             74 LOAD_ATTR                4 (now)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 LOAD_FAST                1 (last_seen)
                            100 LOAD_GLOBAL              7 (NULL + timezone)
                            112 LOAD_ATTR                5 (timedelta)
                            122 LOAD_CONST               2 (5)
                            124 KW_NAMES                 3
                            126 PRECALL                  1
                            130 CALL                     1
                            140 BINARY_OP                0 (+)
                            144 COMPARE_OP               0 (<)
                            150 RETURN_VALUE
                
-                45     >>  152 LOAD_CONST               4 (False)
+                44     >>  152 LOAD_CONST               4 (False)
                            154 RETURN_VALUE
                consts
                   None
                   'profile_online_'
                   5
                   ('minutes',)
                   False
                names      ('cache', 'get', 'id', 'timezone', 'now', 'timedelta')
                varnames   ('self', 'last_seen')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'is_online'
-               firstlineno 40
+               firstlineno 39
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
-                47           0 RESUME                   0
+                46           0 RESUME                   0
                
-                49           2 LOAD_FAST                0 (self)
+                48           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (threads)
                             24 LOAD_METHOD              2 (count)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                0 (user)
@@ -539,110 +531,110 @@
                   None
                names      ('user', 'threads', 'count', 'posts')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 47
+               firstlineno 46
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                51           0 RESUME                   0
+                50           0 RESUME                   0
                
-                52           2 LOAD_FAST                0 (self)
+                51           2 LOAD_FAST                0 (self)
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
-               firstlineno 51
+               firstlineno 50
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'priority_group', 'styled_username', 'is_online', 'post_count', '__str__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'TextField', 'signature', 'Meta', 'property', 'priority_group', 'styled_username', 'is_online', 'post_count', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'BoardProfile'
-         firstlineno 24
+         firstlineno 23
          lnotab
-            0x0a01300126011c021a03020104ff0e010203020104ff0e010203020104
+            0x0a013001260124021a03020104ff0e010203020104ff0e010203020104
             ff0e010206020104ff0e010203
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
-          55           0 RESUME                   0
+          54           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Category')
                        8 STORE_NAME               2 (__qualname__)
          
-          56          10 PUSH_NULL
+          55          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (255)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (name)
          
-          57          44 PUSH_NULL
+          56          44 PUSH_NULL
                       46 LOAD_NAME                3 (models)
                       48 LOAD_ATTR                6 (SlugField)
                       58 LOAD_CONST               3 (1024)
                       60 LOAD_CONST               4 (True)
                       62 KW_NAMES                 5
                       64 PRECALL                  2
                       68 CALL                     2
                       78 STORE_NAME               7 (slug)
          
-          58          80 PUSH_NULL
+          57          80 PUSH_NULL
                       82 LOAD_NAME                3 (models)
                       84 LOAD_ATTR                8 (PositiveIntegerField)
                       94 LOAD_CONST               6 (0)
                       96 KW_NAMES                 7
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_NAME               9 (order)
          
-          60         114 PUSH_NULL
+          59         114 PUSH_NULL
                      116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 60>)
+                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 59>)
                      120 MAKE_FUNCTION            0
                      122 LOAD_CONST               9 ('Meta')
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_NAME              10 (Meta)
          
-          65         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 65>)
+          64         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 64>)
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              11 (__str__)
          
-          68         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 68>)
+          67         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 67>)
                      148 MAKE_FUNCTION            0
                      150 STORE_NAME              12 (get_absolute_url)
                      152 LOAD_CONST              12 (None)
                      154 RETURN_VALUE
          consts
             'Category'
             255
@@ -654,27 +646,27 @@
             ('default',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                60           0 RESUME                   0
+                59           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Category.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                61          10 LOAD_CONST               1 ('category')
+                60          10 LOAD_CONST               1 ('category')
                             12 STORE_NAME               3 (verbose_name)
                
-                62          14 LOAD_CONST               2 ('categories')
+                61          14 LOAD_CONST               2 ('categories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                63          18 LOAD_CONST               3 (('order',))
+                62          18 LOAD_CONST               3 (('order',))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Category.Meta'
                   'category'
                   'categories'
@@ -682,28 +674,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 60
+               firstlineno 59
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
-                65           0 RESUME                   0
+                64           0 RESUME                   0
                
-                66           2 LOAD_FAST                0 (self)
+                65           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (order)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('. ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (name)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -713,34 +705,34 @@
                   '. '
                names      ('order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 65
+               firstlineno 64
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
-                68           0 RESUME                   0
+                67           0 RESUME                   0
                
-                69           2 LOAD_GLOBAL              1 (NULL + reverse)
+                68           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:index')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               1 (index_url)
                
-                70          32 LOAD_FAST                1 (index_url)
+                69          32 LOAD_FAST                1 (index_url)
                             34 FORMAT_VALUE             0
                             36 LOAD_CONST               2 ('#')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                1 (slug)
                             50 FORMAT_VALUE             0
                             52 LOAD_CONST               3 ('.')
                             54 LOAD_FAST                0 (self)
@@ -755,194 +747,194 @@
                   '.'
                names      ('reverse', 'slug', 'order')
                varnames   ('self', 'index_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 68
+               firstlineno 67
                lnotab 0x02011e01
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'SlugField', 'slug', 'PositiveIntegerField', 'order', 'Meta', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Category'
-         firstlineno 55
+         firstlineno 54
          lnotab 0x0a012201240122021a050603
       'Category'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a0800000000000000006403ac04a6010000ab0100000000000000
             005a09020065036a0a000000000000000064056406ac07a6020000ab0200
-            000000000000005a0b0200650c64066406ac08a6020000ab020000000000
-            0000005a0d020065036a0e00000000000000006409ac0aa6010000ab0100
-            000000000000005a0f020065036a100000000000000000640bac0aa60100
-            00ab0100000000000000005a1102004700640c8400640da6020000ab0200
-            000000000000005a12640e84005a136514640f8400a6000000ab00000000
-            00000000005a15651464108400a6000000ab0000000000000000005a1665
-            1464118400a6000000ab0000000000000000005a17641284005a18641384
-            005a1964145300
-          73           0 RESUME                   0
+            000000000000005a0b020065036a0c00000000000000006406ac08a60100
+            00ab0100000000000000005a0d020065036a0e00000000000000006409ac
+            0aa6010000ab0100000000000000005a0f020065036a1000000000000000
+            00640bac0aa6010000ab0100000000000000005a1102004700640c840064
+            0da6020000ab0200000000000000005a12640e84005a136514640f8400a6
+            000000ab0000000000000000005a15651464108400a6000000ab00000000
+            00000000005a16651464118400a6000000ab0000000000000000005a1764
+            1284005a18641384005a1964145300
+          72           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Subcategory')
                        8 STORE_NAME               2 (__qualname__)
          
-          74          10 PUSH_NULL
+          73          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-          75          24 LOAD_NAME                5 (Category)
+          74          24 LOAD_NAME                5 (Category)
                       26 LOAD_CONST               1 ('subcategories')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-          74          40 KW_NAMES                 2
+          73          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (category)
          
-          77          58 PUSH_NULL
+          76          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (CharField)
                       72 LOAD_CONST               3 (255)
                       74 KW_NAMES                 4
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_NAME               9 (name)
          
-          78          92 PUSH_NULL
+          77          92 PUSH_NULL
                       94 LOAD_NAME                3 (models)
                       96 LOAD_ATTR               10 (SlugField)
                      106 LOAD_CONST               5 (1024)
                      108 LOAD_CONST               6 (True)
                      110 KW_NAMES                 7
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_NAME              11 (slug)
          
-          79         128 PUSH_NULL
-                     130 LOAD_NAME               12 (BBCodeTextField)
-                     132 LOAD_CONST               6 (True)
-                     134 LOAD_CONST               6 (True)
-                     136 KW_NAMES                 8
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 STORE_NAME              13 (description)
-         
-          80         154 PUSH_NULL
-                     156 LOAD_NAME                3 (models)
-                     158 LOAD_ATTR               14 (PositiveIntegerField)
-                     168 LOAD_CONST               9 (0)
-                     170 KW_NAMES                10
-                     172 PRECALL                  1
-                     176 CALL                     1
-                     186 STORE_NAME              15 (order)
-         
-          81         188 PUSH_NULL
-                     190 LOAD_NAME                3 (models)
-                     192 LOAD_ATTR               16 (BooleanField)
-                     202 LOAD_CONST              11 (False)
-                     204 KW_NAMES                10
-                     206 PRECALL                  1
-                     210 CALL                     1
-                     220 STORE_NAME              17 (staff_post_only)
-         
-          83         222 PUSH_NULL
-                     224 LOAD_BUILD_CLASS
-                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 83>)
-                     228 MAKE_FUNCTION            0
-                     230 LOAD_CONST              13 ('Meta')
-                     232 PRECALL                  2
-                     236 CALL                     2
-                     246 STORE_NAME              18 (Meta)
-         
-          91         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
-                     250 MAKE_FUNCTION            0
-                     252 STORE_NAME              19 (can_post)
-         
-          94         254 LOAD_NAME               20 (property)
+          78         128 PUSH_NULL
+                     130 LOAD_NAME                3 (models)
+                     132 LOAD_ATTR               12 (TextField)
+                     142 LOAD_CONST               6 (True)
+                     144 KW_NAMES                 8
+                     146 PRECALL                  1
+                     150 CALL                     1
+                     160 STORE_NAME              13 (description)
+         
+          79         162 PUSH_NULL
+                     164 LOAD_NAME                3 (models)
+                     166 LOAD_ATTR               14 (PositiveIntegerField)
+                     176 LOAD_CONST               9 (0)
+                     178 KW_NAMES                10
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 STORE_NAME              15 (order)
+         
+          80         196 PUSH_NULL
+                     198 LOAD_NAME                3 (models)
+                     200 LOAD_ATTR               16 (BooleanField)
+                     210 LOAD_CONST              11 (False)
+                     212 KW_NAMES                10
+                     214 PRECALL                  1
+                     218 CALL                     1
+                     228 STORE_NAME              17 (staff_post_only)
+         
+          82         230 PUSH_NULL
+                     232 LOAD_BUILD_CLASS
+                     234 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 82>)
+                     236 MAKE_FUNCTION            0
+                     238 LOAD_CONST              13 ('Meta')
+                     240 PRECALL                  2
+                     244 CALL                     2
+                     254 STORE_NAME              18 (Meta)
          
-          95         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 94>)
+          90         256 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 90>)
                      258 MAKE_FUNCTION            0
+                     260 STORE_NAME              19 (can_post)
          
-          94         260 PRECALL                  0
-                     264 CALL                     0
+          93         262 LOAD_NAME               20 (property)
          
-          95         274 STORE_NAME              21 (thread_count)
+          94         264 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 93>)
+                     266 MAKE_FUNCTION            0
          
-          98         276 LOAD_NAME               20 (property)
+          93         268 PRECALL                  0
+                     272 CALL                     0
          
-          99         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 98>)
-                     280 MAKE_FUNCTION            0
+          94         282 STORE_NAME              21 (thread_count)
          
-          98         282 PRECALL                  0
-                     286 CALL                     0
+          97         284 LOAD_NAME               20 (property)
          
-          99         296 STORE_NAME              22 (post_count)
+          98         286 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
+                     288 MAKE_FUNCTION            0
          
-         102         298 LOAD_NAME               20 (property)
+          97         290 PRECALL                  0
+                     294 CALL                     0
          
-         103         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 102>)
-                     302 MAKE_FUNCTION            0
+          98         304 STORE_NAME              22 (post_count)
          
-         102         304 PRECALL                  0
-                     308 CALL                     0
+         101         306 LOAD_NAME               20 (property)
          
-         103         318 STORE_NAME              23 (latest_thread)
+         102         308 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 101>)
+                     310 MAKE_FUNCTION            0
          
-         106         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 106>)
-                     322 MAKE_FUNCTION            0
-                     324 STORE_NAME              24 (__str__)
+         101         312 PRECALL                  0
+                     316 CALL                     0
          
-         109         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 109>)
-                     328 MAKE_FUNCTION            0
-                     330 STORE_NAME              25 (get_absolute_url)
-                     332 LOAD_CONST              20 (None)
-                     334 RETURN_VALUE
+         102         326 STORE_NAME              23 (latest_thread)
+         
+         105         328 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 105>)
+                     330 MAKE_FUNCTION            0
+                     332 STORE_NAME              24 (__str__)
+         
+         108         334 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 108>)
+                     336 MAKE_FUNCTION            0
+                     338 STORE_NAME              25 (get_absolute_url)
+                     340 LOAD_CONST              20 (None)
+                     342 RETURN_VALUE
          consts
             'Subcategory'
             'subcategories'
             ('related_name', 'on_delete')
             255
             ('max_length',)
             1024
             True
             ('max_length', 'unique')
-            ('blank', 'null')
+            ('blank',)
             0
             ('default',)
             False
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                83           0 RESUME                   0
+                82           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Subcategory.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                84          10 LOAD_CONST               1 ('subcategory')
+                83          10 LOAD_CONST               1 ('subcategory')
                             12 STORE_NAME               3 (verbose_name)
                
-                85          14 LOAD_CONST               2 ('subcategories')
+                84          14 LOAD_CONST               2 ('subcategories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                86          18 LOAD_CONST               3 (('category__order', 'order'))
+                85          18 LOAD_CONST               3 (('category__order', 'order'))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Subcategory.Meta'
                   'subcategory'
                   'subcategories'
@@ -950,84 +942,84 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 83
+               firstlineno 82
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
-                91           0 RESUME                   0
+                90           0 RESUME                   0
                
-                92           2 LOAD_FAST                0 (self)
+                91           2 LOAD_FAST                0 (self)
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
-               firstlineno 91
+               firstlineno 90
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-                94           0 RESUME                   0
+                93           0 RESUME                   0
                
-                96           2 LOAD_FAST                0 (self)
+                95           2 LOAD_FAST                0 (self)
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
-               firstlineno 94
+               firstlineno 93
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
-                98           0 RESUME                   0
+                97           0 RESUME                   0
                
-               100           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 100>)
+                99           2 LOAD_GLOBAL              1 (NULL + sum)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 99>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (threads)
                             30 LOAD_METHOD              2 (all)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
@@ -1040,15 +1032,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     100           0 RESUME                   0
+                      99           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (thread)
                                   10 LOAD_FAST                1 (thread)
                                   12 LOAD_ATTR                0 (post_count)
                                   22 LIST_APPEND              2
@@ -1057,37 +1049,37 @@
                      consts
                      names      ('post_count',)
                      varnames   ('.0', 'thread')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                      name       '<listcomp>'
-                     firstlineno 100
+                     firstlineno 99
                      lnotab 0x
                names      ('sum', 'threads', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 98
+               firstlineno 97
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
-               102           0 RESUME                   0
+               101           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               103           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-last_post_created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1098,27 +1090,27 @@
                   '-last_post_created_at'
                names      ('threads', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_thread'
-               firstlineno 102
+               firstlineno 101
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064027c006a0200000000000000009b009d055300
-               106           0 RESUME                   0
+               105           0 RESUME                   0
                
-               107           2 LOAD_FAST                0 (self)
+               106           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (category)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (order)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               2 ('. ')
@@ -1133,27 +1125,27 @@
                   '. '
                names      ('category', 'order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 106
+               firstlineno 105
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               109           0 RESUME                   0
+               108           0 RESUME                   0
                
-               110           2 LOAD_GLOBAL              1 (NULL + reverse)
+               109           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:subcategory')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (slug)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1164,181 +1156,182 @@
                   ('args',)
                names      ('reverse', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 109
+               firstlineno 108
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'can_post', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'TextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'can_post', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Subcategory'
-         firstlineno 73
+         firstlineno 72
          lnotab
-            0x0a010e0110ff1203220124011a01220122021a080603020104ff0e0102
+            0x0a010e0110ff1203220124012201220122021a080603020104ff0e0102
             03020104ff0e010203020104ff0e0102030603
       'Subcategory'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a0400000000000000006508640165036a060000000000000000ac
             02a6030000ab0300000000000000005a09020065036a0a00000000000000
-            006403ac04a6010000ab0100000000000000005a0b0200650ca6000000ab
-            0000000000000000005a0d020065036a0e00000000000000006405ac06a6
-            010000ab0100000000000000005a0f020065036a0e000000000000000064
-            05ac06a6010000ab0100000000000000005a10020065036a110000000000
-            0000006407ac08a6010000ab0100000000000000005a12020065036a1300
-            000000000000006409ac06a6010000ab0100000000000000005a14020047
-            00640a8400640ba6020000ab0200000000000000005a15640c84005a1664
-            0d84005a17640e84005a18640f84005a19651a64108400a6000000ab0000
-            000000000000005a1b651a64118400a6000000ab0000000000000000005a
-            1c641284005a1d64135300
-         113           0 RESUME                   0
+            006403ac04a6010000ab0100000000000000005a0b020065036a0c000000
+            0000000000a6000000ab0000000000000000005a0d020065036a0e000000
+            00000000006405ac06a6010000ab0100000000000000005a0f020065036a
+            0e00000000000000006405ac06a6010000ab0100000000000000005a1002
+            0065036a1100000000000000006407ac08a6010000ab0100000000000000
+            005a12020065036a1300000000000000006409ac06a6010000ab01000000
+            00000000005a1402004700640a8400640ba6020000ab0200000000000000
+            005a15640c84005a16640d84005a17640e84005a18640f84005a19651a64
+            108400a6000000ab0000000000000000005a1b651a64118400a6000000ab
+            0000000000000000005a1c641284005a1d64135300
+         112           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Thread')
                        8 STORE_NAME               2 (__qualname__)
          
-         114          10 PUSH_NULL
+         113          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         115          24 LOAD_NAME                5 (Subcategory)
+         114          24 LOAD_NAME                5 (Subcategory)
                       26 LOAD_CONST               1 ('threads')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-         114          40 KW_NAMES                 2
+         113          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (subcategory)
          
-         117          58 PUSH_NULL
+         116          58 PUSH_NULL
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
          
-         118         106 PUSH_NULL
+         117         106 PUSH_NULL
                      108 LOAD_NAME                3 (models)
                      110 LOAD_ATTR               10 (CharField)
                      120 LOAD_CONST               3 (255)
                      122 KW_NAMES                 4
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_NAME              11 (title)
          
-         119         140 PUSH_NULL
-                     142 LOAD_NAME               12 (BBCodeTextField)
-                     144 PRECALL                  0
-                     148 CALL                     0
-                     158 STORE_NAME              13 (content)
-         
-         120         160 PUSH_NULL
-                     162 LOAD_NAME                3 (models)
-                     164 LOAD_ATTR               14 (BooleanField)
-                     174 LOAD_CONST               5 (False)
-                     176 KW_NAMES                 6
-                     178 PRECALL                  1
-                     182 CALL                     1
-                     192 STORE_NAME              15 (is_pinned)
-         
-         121         194 PUSH_NULL
-                     196 LOAD_NAME                3 (models)
-                     198 LOAD_ATTR               14 (BooleanField)
-                     208 LOAD_CONST               5 (False)
-                     210 KW_NAMES                 6
-                     212 PRECALL                  1
-                     216 CALL                     1
-                     226 STORE_NAME              16 (is_closed)
-         
-         122         228 PUSH_NULL
-                     230 LOAD_NAME                3 (models)
-                     232 LOAD_ATTR               17 (DateTimeField)
-                     242 LOAD_CONST               7 (True)
-                     244 KW_NAMES                 8
-                     246 PRECALL                  1
-                     250 CALL                     1
-                     260 STORE_NAME              18 (last_post_created_at)
-         
-         123         262 PUSH_NULL
-                     264 LOAD_NAME                3 (models)
-                     266 LOAD_ATTR               19 (PositiveIntegerField)
-                     276 LOAD_CONST               9 (0)
-                     278 KW_NAMES                 6
-                     280 PRECALL                  1
-                     284 CALL                     1
-                     294 STORE_NAME              20 (view_count)
-         
-         125         296 PUSH_NULL
-                     298 LOAD_BUILD_CLASS
-                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 125>)
-                     302 MAKE_FUNCTION            0
-                     304 LOAD_CONST              11 ('Meta')
-                     306 PRECALL                  2
-                     310 CALL                     2
-                     320 STORE_NAME              21 (Meta)
-         
-         136         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
-                     324 MAKE_FUNCTION            0
-                     326 STORE_NAME              22 (__str__)
-         
-         139         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
-                     330 MAKE_FUNCTION            0
-                     332 STORE_NAME              23 (can_edit)
-         
-         142         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 142>)
-                     336 MAKE_FUNCTION            0
-                     338 STORE_NAME              24 (can_delete)
-         
-         145         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 145>)
-                     342 MAKE_FUNCTION            0
-                     344 STORE_NAME              25 (can_post)
-         
-         148         346 LOAD_NAME               26 (property)
-         
-         149         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 148>)
-                     350 MAKE_FUNCTION            0
-         
-         148         352 PRECALL                  0
-                     356 CALL                     0
-         
-         149         366 STORE_NAME              27 (post_count)
-         
-         152         368 LOAD_NAME               26 (property)
-         
-         153         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
-                     372 MAKE_FUNCTION            0
-         
-         152         374 PRECALL                  0
-                     378 CALL                     0
-         
-         153         388 STORE_NAME              28 (latest_post)
-         
-         156         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
-                     392 MAKE_FUNCTION            0
-                     394 STORE_NAME              29 (get_absolute_url)
-                     396 LOAD_CONST              19 (None)
-                     398 RETURN_VALUE
+         118         140 PUSH_NULL
+                     142 LOAD_NAME                3 (models)
+                     144 LOAD_ATTR               12 (TextField)
+                     154 PRECALL                  0
+                     158 CALL                     0
+                     168 STORE_NAME              13 (content)
+         
+         119         170 PUSH_NULL
+                     172 LOAD_NAME                3 (models)
+                     174 LOAD_ATTR               14 (BooleanField)
+                     184 LOAD_CONST               5 (False)
+                     186 KW_NAMES                 6
+                     188 PRECALL                  1
+                     192 CALL                     1
+                     202 STORE_NAME              15 (is_pinned)
+         
+         120         204 PUSH_NULL
+                     206 LOAD_NAME                3 (models)
+                     208 LOAD_ATTR               14 (BooleanField)
+                     218 LOAD_CONST               5 (False)
+                     220 KW_NAMES                 6
+                     222 PRECALL                  1
+                     226 CALL                     1
+                     236 STORE_NAME              16 (is_closed)
+         
+         121         238 PUSH_NULL
+                     240 LOAD_NAME                3 (models)
+                     242 LOAD_ATTR               17 (DateTimeField)
+                     252 LOAD_CONST               7 (True)
+                     254 KW_NAMES                 8
+                     256 PRECALL                  1
+                     260 CALL                     1
+                     270 STORE_NAME              18 (last_post_created_at)
+         
+         122         272 PUSH_NULL
+                     274 LOAD_NAME                3 (models)
+                     276 LOAD_ATTR               19 (PositiveIntegerField)
+                     286 LOAD_CONST               9 (0)
+                     288 KW_NAMES                 6
+                     290 PRECALL                  1
+                     294 CALL                     1
+                     304 STORE_NAME              20 (view_count)
+         
+         124         306 PUSH_NULL
+                     308 LOAD_BUILD_CLASS
+                     310 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 124>)
+                     312 MAKE_FUNCTION            0
+                     314 LOAD_CONST              11 ('Meta')
+                     316 PRECALL                  2
+                     320 CALL                     2
+                     330 STORE_NAME              21 (Meta)
+         
+         136         332 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
+                     334 MAKE_FUNCTION            0
+                     336 STORE_NAME              22 (__str__)
+         
+         139         338 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
+                     340 MAKE_FUNCTION            0
+                     342 STORE_NAME              23 (can_edit)
+         
+         142         344 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 142>)
+                     346 MAKE_FUNCTION            0
+                     348 STORE_NAME              24 (can_delete)
+         
+         145         350 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 145>)
+                     352 MAKE_FUNCTION            0
+                     354 STORE_NAME              25 (can_post)
+         
+         148         356 LOAD_NAME               26 (property)
+         
+         149         358 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 148>)
+                     360 MAKE_FUNCTION            0
+         
+         148         362 PRECALL                  0
+                     366 CALL                     0
+         
+         149         376 STORE_NAME              27 (post_count)
+         
+         152         378 LOAD_NAME               26 (property)
+         
+         153         380 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
+                     382 MAKE_FUNCTION            0
+         
+         152         384 PRECALL                  0
+                     388 CALL                     0
+         
+         153         398 STORE_NAME              28 (latest_post)
+         
+         156         400 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
+                     402 MAKE_FUNCTION            0
+                     404 STORE_NAME              29 (get_absolute_url)
+                     406 LOAD_CONST              19 (None)
+                     408 RETURN_VALUE
          consts
             'Thread'
             'threads'
             ('related_name', 'on_delete')
             255
             ('max_length',)
             False
@@ -1348,39 +1341,39 @@
             0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035300
-               125           0 RESUME                   0
+               124           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               126          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
+               125          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
                
-               131          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
+               130          14 LOAD_CONST               2 ((('move_thread', 'Can move thread'), ('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
                             16 STORE_NAME               4 (permissions)
                             18 LOAD_CONST               3 (None)
                             20 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
-                  (('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread'))
+                  (('move_thread', 'Can move thread'), ('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread'))
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 125
+               firstlineno 124
                lnotab 0x0a010405
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
@@ -1576,40 +1569,40 @@
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
                firstlineno 156
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'TextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
-         firstlineno 113
+         firstlineno 112
          lnotab
-            0x0a010e0110ff120330012201140122012201220122021a0b0603060306
+            0x0a010e0110ff1203300122011e0122012201220122021a0c0603060306
             030603020104ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a02020065036a040000000000000000650564
             0165036a060000000000000000ac02a6030000ab0300000000000000005a
             07020065036a0400000000000000006508640165036a0600000000000000
-            00ac02a6030000ab0300000000000000005a090200650aa6000000ab0000
-            000000000000005a0b02004700640384006404a6020000ab020000000000
-            0000005a0c640584005a0d640684005a0e640784005a0f651064088400a6
-            000000ab0000000000000000005a11651064098400a6000000ab00000000
-            00000000005a12640a84005a1388006601640b84085a14880078015a1553
-            00
+            00ac02a6030000ab0300000000000000005a09020065036a0a0000000000
+            000000a6000000ab0000000000000000005a0b02004700640384006404a6
+            020000ab0200000000000000005a0c640584005a0d640684005a0e640784
+            005a0f651064088400a6000000ab0000000000000000005a116510640984
+            00a6000000ab0000000000000000005a12640a84005a1388006601640b84
+            085a14880078015a155300
                        0 MAKE_CELL                0 (__class__)
          
          160           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
@@ -1635,73 +1628,74 @@
                       80 LOAD_ATTR                6 (CASCADE)
                       90 KW_NAMES                 2
                       92 PRECALL                  3
                       96 CALL                     3
                      106 STORE_NAME               9 (user)
          
          163         108 PUSH_NULL
-                     110 LOAD_NAME               10 (BBCodeTextField)
-                     112 PRECALL                  0
-                     116 CALL                     0
-                     126 STORE_NAME              11 (content)
-         
-         165         128 PUSH_NULL
-                     130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
-                     134 MAKE_FUNCTION            0
-                     136 LOAD_CONST               4 ('Meta')
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 STORE_NAME              12 (Meta)
-         
-         168         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
-                     156 MAKE_FUNCTION            0
-                     158 STORE_NAME              13 (__str__)
+                     110 LOAD_NAME                3 (models)
+                     112 LOAD_ATTR               10 (TextField)
+                     122 PRECALL                  0
+                     126 CALL                     0
+                     136 STORE_NAME              11 (content)
          
-         171         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 171>)
-                     162 MAKE_FUNCTION            0
-                     164 STORE_NAME              14 (can_edit)
+         165         138 PUSH_NULL
+                     140 LOAD_BUILD_CLASS
+                     142 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
+                     144 MAKE_FUNCTION            0
+                     146 LOAD_CONST               4 ('Meta')
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 STORE_NAME              12 (Meta)
          
-         174         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
-                     168 MAKE_FUNCTION            0
-                     170 STORE_NAME              15 (can_delete)
+         168         164 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
+                     166 MAKE_FUNCTION            0
+                     168 STORE_NAME              13 (__str__)
          
-         177         172 LOAD_NAME               16 (property)
+         171         170 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 171>)
+                     172 MAKE_FUNCTION            0
+                     174 STORE_NAME              14 (can_edit)
          
-         178         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 177>)
-                     176 MAKE_FUNCTION            0
+         174         176 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
+                     178 MAKE_FUNCTION            0
+                     180 STORE_NAME              15 (can_delete)
          
-         177         178 PRECALL                  0
-                     182 CALL                     0
+         177         182 LOAD_NAME               16 (property)
          
-         178         192 STORE_NAME              17 (index)
+         178         184 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 177>)
+                     186 MAKE_FUNCTION            0
          
-         185         194 LOAD_NAME               16 (property)
+         177         188 PRECALL                  0
+                     192 CALL                     0
          
-         186         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 185>)
-                     198 MAKE_FUNCTION            0
+         178         202 STORE_NAME              17 (index)
          
-         185         200 PRECALL                  0
-                     204 CALL                     0
+         185         204 LOAD_NAME               16 (property)
          
-         186         214 STORE_NAME              18 (page_number)
+         186         206 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 185>)
+                     208 MAKE_FUNCTION            0
          
-         189         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 189>)
-                     218 MAKE_FUNCTION            0
-                     220 STORE_NAME              19 (get_absolute_url)
+         185         210 PRECALL                  0
+                     214 CALL                     0
          
-         196         222 LOAD_CLOSURE             0 (__class__)
-                     224 BUILD_TUPLE              1
-                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
-                     228 MAKE_FUNCTION            8 (closure)
-                     230 STORE_NAME              20 (save)
-                     232 LOAD_CLOSURE             0 (__class__)
-                     234 COPY                     1
-                     236 STORE_NAME              21 (__classcell__)
-                     238 RETURN_VALUE
+         186         224 STORE_NAME              18 (page_number)
+         
+         189         226 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 189>)
+                     228 MAKE_FUNCTION            0
+                     230 STORE_NAME              19 (get_absolute_url)
+         
+         196         232 LOAD_CLOSURE             0 (__class__)
+                     234 BUILD_TUPLE              1
+                     236 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
+                     238 MAKE_FUNCTION            8 (closure)
+                     240 STORE_NAME              20 (save)
+                     242 LOAD_CLOSURE             0 (__class__)
+                     244 COPY                     1
+                     246 STORE_NAME              21 (__classcell__)
+                     248 RETURN_VALUE
          consts
             'Post'
             'posts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
@@ -2043,23 +2037,23 @@
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
                firstlineno 196
                lnotab 0x040118011e0118013a013201
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'TextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
          firstlineno 160
          lnotab
-            0x0c013001300114021a03060306030603020104ff0e010207020104ff0e
+            0x0c01300130011e021a03060306030603020104ff0e010207020104ff0e
             0102030607
       'Post'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -2223,17 +2217,17 @@
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a08000000000000000064036404ac05a6020000ab020000000000
-            0000005a090200650aa6000000ab0000000000000000005a0b0200470064
-            0684006407a6020000ab0200000000000000005a0c640884005a0d640953
-            00
+            0000005a09020065036a0a0000000000000000a6000000ab000000000000
+            0000005a0b02004700640684006407a6020000ab0200000000000000005a
+            0c640884005a0d64095300
          219           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupStyle')
                        8 STORE_NAME               2 (__qualname__)
          
          220          10 PUSH_NULL
@@ -2258,33 +2252,34 @@
          
          221          76 KW_NAMES                 5
                       78 PRECALL                  2
                       82 CALL                     2
                       92 STORE_NAME               9 (priority)
          
          225          94 PUSH_NULL
-                      96 LOAD_NAME               10 (BBCodeTextField)
-                      98 PRECALL                  0
-                     102 CALL                     0
-                     112 STORE_NAME              11 (username_style)
+                      96 LOAD_NAME                3 (models)
+                      98 LOAD_ATTR               10 (TextField)
+                     108 PRECALL                  0
+                     112 CALL                     0
+                     122 STORE_NAME              11 (username_style)
          
-         227         114 PUSH_NULL
-                     116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               6 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 227>)
-                     120 MAKE_FUNCTION            0
-                     122 LOAD_CONST               7 ('Meta')
-                     124 PRECALL                  2
-                     128 CALL                     2
-                     138 STORE_NAME              12 (Meta)
+         227         124 PUSH_NULL
+                     126 LOAD_BUILD_CLASS
+                     128 LOAD_CONST               6 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 227>)
+                     130 MAKE_FUNCTION            0
+                     132 LOAD_CONST               7 ('Meta')
+                     134 PRECALL                  2
+                     138 CALL                     2
+                     148 STORE_NAME              12 (Meta)
          
-         230         140 LOAD_CONST               8 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 230>)
-                     142 MAKE_FUNCTION            0
-                     144 STORE_NAME              13 (__str__)
-                     146 LOAD_CONST               9 (None)
-                     148 RETURN_VALUE
+         230         150 LOAD_CONST               8 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 230>)
+                     152 MAKE_FUNCTION            0
+                     154 STORE_NAME              13 (__str__)
+                     156 LOAD_CONST               9 (None)
+                     158 RETURN_VALUE
          consts
             'GroupStyle'
             'style'
             ('related_name', 'on_delete')
             0
             'Highest priority is displayed'
             ('default', 'help_text')
@@ -2344,26 +2339,26 @@
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
                firstlineno 230
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'Group', 'CASCADE', 'group', 'PositiveIntegerField', 'priority', 'BBCodeTextField', 'username_style', 'Meta', '__str__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'Group', 'CASCADE', 'group', 'PositiveIntegerField', 'priority', 'TextField', 'username_style', 'Meta', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'GroupStyle'
          firstlineno 219
-         lnotab 0x0a0130010e01020102fe120414021a03
+         lnotab 0x0a0130010e01020102fe12041e021a03
       'GroupStyle'
-   names      ('math', 'os', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'punkweb_bb.utils', 'get_highest_priority_group', 'get_styled_username', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout', 'GroupStyle')
+   names      ('math', 'os', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'punkweb_bb.utils', 'get_highest_priority_group', 'get_styled_username', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout', 'GroupStyle')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108020c010c010c010c010c010c010c010c021001100214
-      0306051e1f1e121e281e2f1e2d1e0e
+      0x00ff0201080108020c010c010c010c010c010c010c0210011002140306
+      051e1f1e121e281e301e2d1e0e
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa69b5766 (Wed May 29 21:18:30 2024 UTC)
-files sz: 561
+moddate:  0x3cde5866 (Thu May 30 20:14:52 2024 UTC)
+files sz: 609
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a01010002006502650164026900a6030000ab
@@ -15,16 +15,17 @@
       00000064076408a6020000ab0200000000000000005a076503a004000000
       00000000000000000000000000000000006409640aa6020000ab02000000
       00000000005a086503a00400000000000000000000000000000000000000
       00640b640ca6020000ab0200000000000000005a096503a0040000000000
       000000000000000000000000000000640d640ea6020000ab020000000000
       0000005a0a6503a004000000000000000000000000000000000000000064
       0f6410a6020000ab0200000000000000005a0b6503a00400000000000000
-      000000000000000000000000006411640aa6020000ab0200000000000000
-      005a0c640a5300
+      0000000000000000000000000064116412a6020000ab0200000000000000
+      005a0c6503a0040000000000000000000000000000000000000000641364
+      0ca6020000ab0200000000000000005a0d640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('settings',))
                  6 IMPORT_NAME              0 (django.conf)
                  8 IMPORT_FROM              1 (settings)
                 10 STORE_NAME               1 (settings)
@@ -53,81 +54,91 @@
                110 LOAD_CONST               6 ('PunkwebBB')
                112 PRECALL                  2
                116 CALL                     2
                126 STORE_NAME               6 (SITE_TITLE)
    
      7         128 LOAD_NAME                3 (PUNKWEB_BB)
                130 LOAD_METHOD              4 (get)
-               152 LOAD_CONST               7 ('FAVICON')
-               154 LOAD_CONST               8 ('punkweb_bb/favicon.ico')
+               152 LOAD_CONST               7 ('RENDERER')
+               154 LOAD_CONST               8 ('bbcode')
                156 PRECALL                  2
                160 CALL                     2
-               170 STORE_NAME               7 (FAVICON)
+               170 STORE_NAME               7 (RENDERER)
    
      8         172 LOAD_NAME                3 (PUNKWEB_BB)
                174 LOAD_METHOD              4 (get)
-               196 LOAD_CONST               9 ('OG_IMAGE')
-               198 LOAD_CONST              10 (None)
+               196 LOAD_CONST               9 ('FAVICON')
+               198 LOAD_CONST              10 ('punkweb_bb/favicon.ico')
                200 PRECALL                  2
                204 CALL                     2
-               214 STORE_NAME               8 (OG_IMAGE)
+               214 STORE_NAME               8 (FAVICON)
    
      9         216 LOAD_NAME                3 (PUNKWEB_BB)
                218 LOAD_METHOD              4 (get)
-               240 LOAD_CONST              11 ('SHOUTBOX_ENABLED')
-               242 LOAD_CONST              12 (True)
+               240 LOAD_CONST              11 ('OG_IMAGE')
+               242 LOAD_CONST              12 (None)
                244 PRECALL                  2
                248 CALL                     2
-               258 STORE_NAME               9 (SHOUTBOX_ENABLED)
+               258 STORE_NAME               9 (OG_IMAGE)
    
     10         260 LOAD_NAME                3 (PUNKWEB_BB)
                262 LOAD_METHOD              4 (get)
-               284 LOAD_CONST              13 ('DISCORD_WIDGET_ENABLED')
-               286 LOAD_CONST              14 (False)
+               284 LOAD_CONST              13 ('SHOUTBOX_ENABLED')
+               286 LOAD_CONST              14 (True)
                288 PRECALL                  2
                292 CALL                     2
-               302 STORE_NAME              10 (DISCORD_WIDGET_ENABLED)
+               302 STORE_NAME              10 (SHOUTBOX_ENABLED)
    
     11         304 LOAD_NAME                3 (PUNKWEB_BB)
                306 LOAD_METHOD              4 (get)
-               328 LOAD_CONST              15 ('DISCORD_WIDGET_THEME')
-               330 LOAD_CONST              16 ('dark')
+               328 LOAD_CONST              15 ('DISCORD_WIDGET_ENABLED')
+               330 LOAD_CONST              16 (False)
                332 PRECALL                  2
                336 CALL                     2
-               346 STORE_NAME              11 (DISCORD_WIDGET_THEME)
+               346 STORE_NAME              11 (DISCORD_WIDGET_ENABLED)
    
     12         348 LOAD_NAME                3 (PUNKWEB_BB)
                350 LOAD_METHOD              4 (get)
-               372 LOAD_CONST              17 ('DISCORD_SERVER_ID')
-               374 LOAD_CONST              10 (None)
+               372 LOAD_CONST              17 ('DISCORD_WIDGET_THEME')
+               374 LOAD_CONST              18 ('dark')
                376 PRECALL                  2
                380 CALL                     2
-               390 STORE_NAME              12 (DISCORD_SERVER_ID)
-               392 LOAD_CONST              10 (None)
-               394 RETURN_VALUE
+               390 STORE_NAME              12 (DISCORD_WIDGET_THEME)
+   
+    13         392 LOAD_NAME                3 (PUNKWEB_BB)
+               394 LOAD_METHOD              4 (get)
+               416 LOAD_CONST              19 ('DISCORD_SERVER_ID')
+               418 LOAD_CONST              12 (None)
+               420 PRECALL                  2
+               424 CALL                     2
+               434 STORE_NAME              13 (DISCORD_SERVER_ID)
+               436 LOAD_CONST              12 (None)
+               438 RETURN_VALUE
    consts
       0
       ('settings',)
       'PUNKWEB_BB'
       'SITE_NAME'
       'PUNKWEB'
       'SITE_TITLE'
       'PunkwebBB'
+      'RENDERER'
+      'bbcode'
       'FAVICON'
       'punkweb_bb/favicon.ico'
       'OG_IMAGE'
       None
       'SHOUTBOX_ENABLED'
       True
       'DISCORD_WIDGET_ENABLED'
       False
       'DISCORD_WIDGET_THEME'
       'dark'
       'DISCORD_SERVER_ID'
-   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'FAVICON', 'OG_IMAGE', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
+   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'RENDERER', 'FAVICON', 'OG_IMAGE', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/settings.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021a022c012c012c012c012c012c012c01
+   lnotab 0x00ff02010c021a022c012c012c012c012c012c012c012c01
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/sitemap.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x114e5666 (Tue May 28 21:35:13 2024 UTC)
-files sz: 26338
+moddate:  0x4ffe5866 (Thu May 30 22:31:43 2024 UTC)
+files sz: 26298
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -4079,15 +4079,15 @@
                   007c016a0600000000000000006401a6020000ab02000000000000000001
                   007c006a000000000000000000a007000000000000000000000000000000
                   00000000007c006a040000000000000000640264036901a6020000ab0200
                   0000000000000001007c006a0200000000000000006a0800000000000000
                   00a0090000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001007c00a0050000000000000000000000000000000000
                   0000007c006a0200000000000000006a0800000000000000006a0a000000
-                  00000000006404a6020000ab02000000000000000001007c00a005000000
+                  00000000006403a6020000ab02000000000000000001007c00a005000000
                   00000000000000000000000000000000007c016a06000000000000000064
                   01a6020000ab020000000000000000010064005300
                411           0 RESUME                   0
                
                412           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
@@ -4140,16 +4140,16 @@
                            306 POP_TOP
                
                425         308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              5 (assertEqual)
                            332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR                2 (user)
                            344 LOAD_ATTR                8 (profile)
-                           354 LOAD_ATTR               10 (_signature_rendered)
-                           364 LOAD_CONST               4 ('<strong>test</strong>')
+                           354 LOAD_ATTR               10 (signature)
+                           364 LOAD_CONST               3 ('[b]test[/b]')
                            366 PRECALL                  2
                            370 CALL                     2
                            380 POP_TOP
                
                427         382 LOAD_FAST                0 (self)
                            384 LOAD_METHOD              5 (assertEqual)
                            406 LOAD_FAST                1 (response)
@@ -4161,16 +4161,15 @@
                            436 LOAD_CONST               0 (None)
                            438 RETURN_VALUE
                consts
                   None
                   200
                   'signature'
                   '[b]test[/b]'
-                  '<strong>test</strong>'
-               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'profile', 'refresh_from_db', '_signature_rendered')
+               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'profile', 'refresh_from_db', 'signature')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_settings'
                firstlineno 411
                lnotab 0x02013e013e02360222010c0204ff02fe10073c014a02
@@ -5231,29 +5230,29 @@
                            446 CALL                     2
                            456 POP_TOP
                
                549         458 LOAD_FAST                0 (self)
                            460 LOAD_METHOD              5 (assertEqual)
                            482 LOAD_FAST                0 (self)
                            484 LOAD_ATTR                9 (thread)
-                           494 LOAD_ATTR               13 (_content_rendered)
+                           494 LOAD_ATTR               13 (content)
                            504 LOAD_CONST               2 ('edit')
                            506 PRECALL                  2
                            510 CALL                     2
                            520 POP_TOP
                            522 LOAD_CONST               0 (None)
                            524 RETURN_VALUE
                consts
                   None
                   200
                   'edit'
                   ('title', 'content')
                   True
                   ('follow',)
-               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'thread', 'get_absolute_url', 'refresh_from_db', 'title', '_content_rendered')
+               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'thread', 'get_absolute_url', 'refresh_from_db', 'title', 'content')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_update'
                firstlineno 531
                lnotab 0x02013e013e02360222010c02020102fe040402fa12095a0132014001
@@ -6418,29 +6417,29 @@
                            380 CALL                     0
                            390 POP_TOP
                
                678         392 LOAD_FAST                0 (self)
                            394 LOAD_METHOD              5 (assertEqual)
                            416 LOAD_FAST                0 (self)
                            418 LOAD_ATTR                7 (post)
-                           428 LOAD_ATTR               11 (_content_rendered)
+                           428 LOAD_ATTR               11 (content)
                            438 LOAD_CONST               3 ('edit')
                            440 PRECALL                  2
                            444 CALL                     2
                            454 POP_TOP
                            456 LOAD_CONST               0 (None)
                            458 RETURN_VALUE
                consts
                   None
                   200
                   'content'
                   'edit'
                   True
                   ('follow',)
-               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'get_absolute_url', 'refresh_from_db', '_content_rendered')
+               names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'get_absolute_url', 'refresh_from_db', 'content')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_post_update'
                firstlineno 662
                lnotab 0x02013e013e02360222010c0204ff020302fb12085a013201
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,14 +1,14 @@
 magic:    0xa70d0d0a
-moddate:  0x95815666 (Wed May 29 01:15:01 2024 UTC)
-files sz: 2587
+moddate:  0x3ce55766 (Thu May 30 02:32:28 2024 UTC)
+files sz: 2673
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 31
+   stacksize : 32
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a03010064035a
       0402006501640465036a0500000000000000006405ac06a6030000ab0300
       0000000000000002006501640765036a0600000000000000006408ac06a6
       030000ab03000000000000000002006501640965036a0700000000000000
       00640aac06a6030000ab03000000000000000002006501640b65036a0800
@@ -36,15 +36,16 @@
       0000000000000002006501642f65036a1a00000000000000006430ac06a6
       030000ab03000000000000000002006501643165036a1b00000000000000
       006432ac06a6030000ab03000000000000000002006501643365036a1c00
       000000000000006434ac06a6030000ab0300000000000000000200650164
       3565036a1d00000000000000006436ac06a6030000ab0300000000000000
       0002006501643765036a1e00000000000000006438ac06a6030000ab0300
       0000000000000002006501643965036a1f0000000000000000643aac06a6
-      030000ab030000000000000000671b5a20643b5300
+      030000ab03000000000000000002006501643b65036a2000000000000000
+      00643cac06a6030000ab030000000000000000671c5a21643d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('path',))
                  6 IMPORT_NAME              0 (django.urls)
                  8 IMPORT_FROM              1 (path)
                 10 STORE_NAME               1 (path)
@@ -304,76 +305,86 @@
                768 LOAD_CONST              46 ('thread_close')
                770 KW_NAMES                 6
                772 PRECALL                  3
                776 CALL                     3
    
     64         786 PUSH_NULL
                788 LOAD_NAME                1 (path)
-               790 LOAD_CONST              47 ('post/<str:post_id>/delete/')
+               790 LOAD_CONST              47 ('thread/<str:thread_id>/move/')
                792 LOAD_NAME                3 (views)
-               794 LOAD_ATTR               26 (post_delete_view)
-               804 LOAD_CONST              48 ('post_delete')
+               794 LOAD_ATTR               26 (thread_move_view)
+               804 LOAD_CONST              48 ('thread_move')
                806 KW_NAMES                 6
                808 PRECALL                  3
                812 CALL                     3
    
     65         822 PUSH_NULL
                824 LOAD_NAME                1 (path)
-               826 LOAD_CONST              49 ('post/<str:post_id>/update/')
+               826 LOAD_CONST              49 ('post/<str:post_id>/delete/')
                828 LOAD_NAME                3 (views)
-               830 LOAD_ATTR               27 (post_update_view)
-               840 LOAD_CONST              50 ('post_update')
+               830 LOAD_ATTR               27 (post_delete_view)
+               840 LOAD_CONST              50 ('post_delete')
                842 KW_NAMES                 6
                844 PRECALL                  3
                848 CALL                     3
    
     66         858 PUSH_NULL
                860 LOAD_NAME                1 (path)
-               862 LOAD_CONST              51 ('shout-list/')
+               862 LOAD_CONST              51 ('post/<str:post_id>/update/')
                864 LOAD_NAME                3 (views)
-               866 LOAD_ATTR               28 (shout_list_view)
-               876 LOAD_CONST              52 ('shout_list')
+               866 LOAD_ATTR               28 (post_update_view)
+               876 LOAD_CONST              52 ('post_update')
                878 KW_NAMES                 6
                880 PRECALL                  3
                884 CALL                     3
    
     67         894 PUSH_NULL
                896 LOAD_NAME                1 (path)
-               898 LOAD_CONST              53 ('shout-create/')
+               898 LOAD_CONST              53 ('shout-list/')
                900 LOAD_NAME                3 (views)
-               902 LOAD_ATTR               29 (shout_create_view)
-               912 LOAD_CONST              54 ('shout_create')
+               902 LOAD_ATTR               29 (shout_list_view)
+               912 LOAD_CONST              54 ('shout_list')
                914 KW_NAMES                 6
                916 PRECALL                  3
                920 CALL                     3
    
     68         930 PUSH_NULL
                932 LOAD_NAME                1 (path)
-               934 LOAD_CONST              55 ('shout/<str:shout_id>/delete/')
+               934 LOAD_CONST              55 ('shout-create/')
                936 LOAD_NAME                3 (views)
-               938 LOAD_ATTR               30 (shout_delete_view)
-               948 LOAD_CONST              56 ('shout_delete')
+               938 LOAD_ATTR               30 (shout_create_view)
+               948 LOAD_CONST              56 ('shout_create')
                950 KW_NAMES                 6
                952 PRECALL                  3
                956 CALL                     3
    
     69         966 PUSH_NULL
                968 LOAD_NAME                1 (path)
-               970 LOAD_CONST              57 ('bbcode/')
+               970 LOAD_CONST              57 ('shout/<str:shout_id>/delete/')
                972 LOAD_NAME                3 (views)
-               974 LOAD_ATTR               31 (bbcode_view)
-               984 LOAD_CONST              58 ('bbcode')
+               974 LOAD_ATTR               31 (shout_delete_view)
+               984 LOAD_CONST              58 ('shout_delete')
                986 KW_NAMES                 6
                988 PRECALL                  3
                992 CALL                     3
    
-     6        1002 BUILD_LIST              27
-              1004 STORE_NAME              32 (urlpatterns)
-              1006 LOAD_CONST              59 (None)
-              1008 RETURN_VALUE
+    70        1002 PUSH_NULL
+              1004 LOAD_NAME                1 (path)
+              1006 LOAD_CONST              59 ('bbcode/')
+              1008 LOAD_NAME                3 (views)
+              1010 LOAD_ATTR               32 (bbcode_view)
+              1020 LOAD_CONST              60 ('bbcode')
+              1022 KW_NAMES                 6
+              1024 PRECALL                  3
+              1028 CALL                     3
+   
+     6        1038 BUILD_LIST              28
+              1040 STORE_NAME              33 (urlpatterns)
+              1042 LOAD_CONST              61 (None)
+              1044 RETURN_VALUE
    consts
       0
       ('path',)
       ('views',)
       'punkweb_bb'
       ''
       'index'
@@ -414,33 +425,35 @@
       'thread_update'
       'thread/<str:thread_id>/create-post/'
       'post_create'
       'thread/<str:thread_id>/pin/'
       'thread_pin'
       'thread/<str:thread_id>/close/'
       'thread_close'
+      'thread/<str:thread_id>/move/'
+      'thread_move'
       'post/<str:post_id>/delete/'
       'post_delete'
       'post/<str:post_id>/update/'
       'post_update'
       'shout-list/'
       'shout_list'
       'shout-create/'
       'shout_create'
       'shout/<str:shout_id>/delete/'
       'shout_delete'
       'bbcode/'
       'bbcode'
       None
-   names      ('django.urls', 'path', 'punkweb_bb', 'views', 'app_name', 'index_view', 'signup_view', 'login_view', 'logout_view', 'settings_view', 'members_view', 'profile_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_delete_view', 'thread_update_view', 'post_create_view', 'thread_pin_view', 'thread_close_view', 'post_delete_view', 'post_update_view', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view', 'urlpatterns')
+   names      ('django.urls', 'path', 'punkweb_bb', 'views', 'app_name', 'index_view', 'signup_view', 'login_view', 'logout_view', 'settings_view', 'members_view', 'profile_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_delete_view', 'thread_update_view', 'post_create_view', 'thread_pin_view', 'thread_close_view', 'thread_move_view', 'post_delete_view', 'post_update_view', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view', 'urlpatterns')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/urls.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020c02040224012401240124012401240124012401040102
       010c0102fd1005040102010c0102fd1005040102010c0102fd1005040102
       010c0102fd1005040102010c0102fd1005040102010c0102fd1005040102
       010c0102fd10052401040110ff1003040110ff1003040102010c0102fd10
-      05240124012401240124012401240124c1
+      052401240124012401240124012401240124c0
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/utils.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/utils.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,295 +1,397 @@
 magic:    0xa70d0d0a
-moddate:  0xf5975766 (Wed May 29 21:02:45 2024 UTC)
-files sz: 1200
+moddate:  0x6aff5866 (Thu May 30 22:36:26 2024 UTC)
+files sz: 1651
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100640384
-      005a04640484005a05640584005a06640684005a0764075300
+      0x9700640064016c006d015a010100640064026c026d035a030100640064
+      036c046d055a050100640484005a06640584005a07640684005a08640784
+      005a09640884005a0a64095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Group',))
-                 6 IMPORT_NAME              0 (django.contrib.auth.models)
-                 8 IMPORT_FROM              1 (Group)
-                10 STORE_NAME               1 (Group)
+                 4 LOAD_CONST               1 (('slugify',))
+                 6 IMPORT_NAME              0 (django.utils.text)
+                 8 IMPORT_FROM              1 (slugify)
+                10 STORE_NAME               1 (slugify)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('slugify',))
-                18 IMPORT_NAME              2 (django.utils.text)
-                20 IMPORT_FROM              3 (slugify)
-                22 STORE_NAME               3 (slugify)
+                16 LOAD_CONST               2 (('get_parser',))
+                18 IMPORT_NAME              2 (precise_bbcode.bbcode)
+                20 IMPORT_FROM              3 (get_parser)
+                22 STORE_NAME               3 (get_parser)
                 24 POP_TOP
    
-     5          26 LOAD_CONST               3 (<code object get_unique_slug, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 5>)
-                28 MAKE_FUNCTION            0
-                30 STORE_NAME               4 (get_unique_slug)
+     3          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('RENDERER',))
+                30 IMPORT_NAME              4 (punkweb_bb.settings)
+                32 IMPORT_FROM              5 (RENDERER)
+                34 STORE_NAME               5 (RENDERER)
+                36 POP_TOP
    
-    21          32 LOAD_CONST               4 (<code object get_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 21>)
-                34 MAKE_FUNCTION            0
-                36 STORE_NAME               5 (get_highest_priority_group)
-   
-    30          38 LOAD_CONST               5 (<code object get_styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 30>)
+     6          38 LOAD_CONST               4 (<code object get_editor_widget, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 6>)
                 40 MAKE_FUNCTION            0
-                42 STORE_NAME               6 (get_styled_username)
+                42 STORE_NAME               6 (get_editor_widget)
    
-    41          44 LOAD_CONST               6 (<code object get_styled_group_name, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 41>)
+    19          44 LOAD_CONST               5 (<code object get_unique_slug, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 19>)
                 46 MAKE_FUNCTION            0
-                48 STORE_NAME               7 (get_styled_group_name)
-                50 LOAD_CONST               7 (None)
-                52 RETURN_VALUE
+                48 STORE_NAME               7 (get_unique_slug)
+   
+    35          50 LOAD_CONST               6 (<code object get_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 35>)
+                52 MAKE_FUNCTION            0
+                54 STORE_NAME               8 (get_highest_priority_group)
+   
+    44          56 LOAD_CONST               7 (<code object get_styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 44>)
+                58 MAKE_FUNCTION            0
+                60 STORE_NAME               9 (get_styled_username)
+   
+    56          62 LOAD_CONST               8 (<code object get_styled_group_name, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 56>)
+                64 MAKE_FUNCTION            0
+                66 STORE_NAME              10 (get_styled_group_name)
+                68 LOAD_CONST               9 (None)
+                70 RETURN_VALUE
    consts
       0
-      ('Group',)
       ('slugify',)
+      ('get_parser',)
+      ('RENDERER',)
+      code
+         argcount  : 0
+         nlocals   : 2
+         stacksize : 3
+         flags     : 3
+         code
+            0x970074000000000000000000000064016b02000000007210640264036c
+            016d027d00010002007c00a6000000ab0000000000000000005300740000
+            00000000000000000064046b02000000007210640264056c016d037d0101
+            0002007c01a6000000ab0000000000000000005300740900000000000000
+            0000006406a6010000ab0100000000000000008201
+           6           0 RESUME                   0
+         
+           7           2 LOAD_GLOBAL              0 (RENDERER)
+                      14 LOAD_CONST               1 ('bbcode')
+                      16 COMPARE_OP               2 (==)
+                      22 POP_JUMP_FORWARD_IF_FALSE    16 (to 56)
+         
+           8          24 LOAD_CONST               2 (0)
+                      26 LOAD_CONST               3 (('BBCodeEditorWidget',))
+                      28 IMPORT_NAME              1 (punkweb_bb.widgets)
+                      30 IMPORT_FROM              2 (BBCodeEditorWidget)
+                      32 STORE_FAST               0 (BBCodeEditorWidget)
+                      34 POP_TOP
+         
+          10          36 PUSH_NULL
+                      38 LOAD_FAST                0 (BBCodeEditorWidget)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 RETURN_VALUE
+         
+          11     >>   56 LOAD_GLOBAL              0 (RENDERER)
+                      68 LOAD_CONST               4 ('markdown')
+                      70 COMPARE_OP               2 (==)
+                      76 POP_JUMP_FORWARD_IF_FALSE    16 (to 110)
+         
+          12          78 LOAD_CONST               2 (0)
+                      80 LOAD_CONST               5 (('MarkdownEditorWidget',))
+                      82 IMPORT_NAME              1 (punkweb_bb.widgets)
+                      84 IMPORT_FROM              3 (MarkdownEditorWidget)
+                      86 STORE_FAST               1 (MarkdownEditorWidget)
+                      88 POP_TOP
+         
+          14          90 PUSH_NULL
+                      92 LOAD_FAST                1 (MarkdownEditorWidget)
+                      94 PRECALL                  0
+                      98 CALL                     0
+                     108 RETURN_VALUE
+         
+          16     >>  110 LOAD_GLOBAL              9 (NULL + ValueError)
+                     122 LOAD_CONST               6 ('Invalid renderer')
+                     124 PRECALL                  1
+                     128 CALL                     1
+                     138 RAISE_VARARGS            1
+         consts
+            None
+            'bbcode'
+            0
+            ('BBCodeEditorWidget',)
+            'markdown'
+            ('MarkdownEditorWidget',)
+            'Invalid renderer'
+         names      ('RENDERER', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'MarkdownEditorWidget', 'ValueError')
+         varnames   ('BBCodeEditorWidget', 'MarkdownEditorWidget')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
+         name       'get_editor_widget'
+         firstlineno 6
+         lnotab 0x020116010c02140116010c021402
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c01a6010000ab0100000000000000
             007d027c027d0364017d0464027d057c04723e7c006a0100000000000000
             00a00200000000000000000000000000000000000000007c03ac03a60100
             00ab010000000000000000a0030000000000000000000000000000000000
             000000a6000000ab000000000000000000720d7c029b0064047c059b009d
             037d037c0564027a0d00007d056e0264057d047c04b03e7c035300
-           5           0 RESUME                   0
+          19           0 RESUME                   0
          
-           6           2 LOAD_GLOBAL              1 (NULL + slugify)
+          20           2 LOAD_GLOBAL              1 (NULL + slugify)
                       14 LOAD_FAST                1 (field)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               2 (base_slug)
          
-           7          32 LOAD_FAST                2 (base_slug)
+          21          32 LOAD_FAST                2 (base_slug)
                       34 STORE_FAST               3 (slug)
          
-           8          36 LOAD_CONST               1 (True)
+          22          36 LOAD_CONST               1 (True)
                       38 STORE_FAST               4 (unique_slug_exists)
          
-          10          40 LOAD_CONST               2 (1)
+          24          40 LOAD_CONST               2 (1)
                       42 STORE_FAST               5 (counter)
          
-          11          44 LOAD_FAST                4 (unique_slug_exists)
+          25          44 LOAD_FAST                4 (unique_slug_exists)
                       46 POP_JUMP_FORWARD_IF_FALSE    62 (to 172)
          
-          12     >>   48 LOAD_FAST                0 (model)
+          26     >>   48 LOAD_FAST                0 (model)
                       50 LOAD_ATTR                1 (objects)
                       60 LOAD_METHOD              2 (filter)
                       82 LOAD_FAST                3 (slug)
                       84 KW_NAMES                 3
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_METHOD              3 (exists)
                      122 PRECALL                  0
                      126 CALL                     0
                      136 POP_JUMP_FORWARD_IF_FALSE    13 (to 164)
          
-          13         138 LOAD_FAST                2 (base_slug)
+          27         138 LOAD_FAST                2 (base_slug)
                      140 FORMAT_VALUE             0
                      142 LOAD_CONST               4 ('-')
                      144 LOAD_FAST                5 (counter)
                      146 FORMAT_VALUE             0
                      148 BUILD_STRING             3
                      150 STORE_FAST               3 (slug)
          
-          14         152 LOAD_FAST                5 (counter)
+          28         152 LOAD_FAST                5 (counter)
                      154 LOAD_CONST               2 (1)
                      156 BINARY_OP               13 (+=)
                      160 STORE_FAST               5 (counter)
                      162 JUMP_FORWARD             2 (to 168)
          
-          16     >>  164 LOAD_CONST               5 (False)
+          30     >>  164 LOAD_CONST               5 (False)
                      166 STORE_FAST               4 (unique_slug_exists)
          
-          11     >>  168 LOAD_FAST                4 (unique_slug_exists)
+          25     >>  168 LOAD_FAST                4 (unique_slug_exists)
                      170 POP_JUMP_BACKWARD_IF_TRUE    62 (to 48)
          
-          18     >>  172 LOAD_FAST                3 (slug)
+          32     >>  172 LOAD_FAST                3 (slug)
                      174 RETURN_VALUE
          consts
             None
             True
             1
             ('slug',)
             '-'
             False
          names      ('slugify', 'objects', 'filter', 'exists')
          varnames   ('model', 'field', 'base_slug', 'slug', 'unique_slug_exists', 'counter')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_unique_slug'
-         firstlineno 5
+         firstlineno 19
          lnotab 0x02011e0104010402040104015a010e010c0204fb0407
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             000000000000006401ac02a6010000ab0100000000000000007d017c01a0
             020000000000000000000000000000000000000000a6000000ab00000000
             000000000072277c01a00300000000000000000000000000000000000000
             006403a6010000ab010000000000000000a0040000000000000000000000
             000000000000000000a6000000ab000000000000000000530064005300
-          21           0 RESUME                   0
+          35           0 RESUME                   0
          
-          22           2 LOAD_FAST                0 (user)
+          36           2 LOAD_FAST                0 (user)
                        4 LOAD_ATTR                0 (groups)
                       14 LOAD_METHOD              1 (filter)
                       36 LOAD_CONST               1 (False)
                       38 KW_NAMES                 2
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_FAST               1 (groups)
          
-          24          56 LOAD_FAST                1 (groups)
+          38          56 LOAD_FAST                1 (groups)
                       58 LOAD_METHOD              2 (exists)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 POP_JUMP_FORWARD_IF_FALSE    39 (to 174)
          
-          25          96 LOAD_FAST                1 (groups)
+          39          96 LOAD_FAST                1 (groups)
                       98 LOAD_METHOD              3 (order_by)
                      120 LOAD_CONST               3 ('-style__priority')
                      122 PRECALL                  1
                      126 CALL                     1
                      136 LOAD_METHOD              4 (first)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 RETURN_VALUE
          
-          27     >>  174 LOAD_CONST               0 (None)
+          41     >>  174 LOAD_CONST               0 (None)
                      176 RETURN_VALUE
          consts
             None
             False
             ('style__isnull',)
             '-style__priority'
          names      ('groups', 'filter', 'exists', 'order_by', 'first')
          varnames   ('user', 'groups')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_highest_priority_group'
-         firstlineno 21
+         firstlineno 35
          lnotab 0x0201360228014e02
       code
          argcount  : 1
-         nlocals   : 4
-         stacksize : 4
+         nlocals   : 5
+         stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
-            007d017c01722e7c016a0100000000000000006a0200000000000000007d
-            027c026a030000000000000000a004000000000000000000000000000000
-            000000000064017c006a050000000000000000a6020000ab020000000000
-            0000007d037c0353007c006a0500000000000000005300
-          30           0 RESUME                   0
+            007d017c01724a740300000000000000000000a6000000ab000000000000
+            0000007d027c016a0200000000000000006a0300000000000000007d037c
+            02a00400000000000000000000000000000000000000007c03a005000000
+            000000000000000000000000000000000064017c006a0600000000000000
+            00a6020000ab020000000000000000a6010000ab0100000000000000007d
+            047c0453007c006a0600000000000000005300
+          44           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
+          45           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
                       14 LOAD_FAST                0 (user)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (group)
          
-          33          32 LOAD_FAST                1 (group)
-                      34 POP_JUMP_FORWARD_IF_FALSE    46 (to 128)
+          47          32 LOAD_FAST                1 (group)
+                      34 POP_JUMP_FORWARD_IF_FALSE    74 (to 184)
          
-          34          36 LOAD_FAST                1 (group)
-                      38 LOAD_ATTR                1 (style)
-                      48 LOAD_ATTR                2 (username_style)
-                      58 STORE_FAST               2 (username_style)
-         
-          35          60 LOAD_FAST                2 (username_style)
-                      62 LOAD_ATTR                3 (rendered)
-                      72 LOAD_METHOD              4 (replace)
-                      94 LOAD_CONST               1 ('{USER}')
-                      96 LOAD_FAST                0 (user)
-                      98 LOAD_ATTR                5 (username)
-                     108 PRECALL                  2
-                     112 CALL                     2
-                     122 STORE_FAST               3 (styled_username)
-         
-          36         124 LOAD_FAST                3 (styled_username)
-                     126 RETURN_VALUE
-         
-          38     >>  128 LOAD_FAST                0 (user)
-                     130 LOAD_ATTR                5 (username)
-                     140 RETURN_VALUE
+          48          36 LOAD_GLOBAL              3 (NULL + get_parser)
+                      48 PRECALL                  0
+                      52 CALL                     0
+                      62 STORE_FAST               2 (parser)
+         
+          49          64 LOAD_FAST                1 (group)
+                      66 LOAD_ATTR                2 (style)
+                      76 LOAD_ATTR                3 (username_style)
+                      86 STORE_FAST               3 (username_style)
+         
+          50          88 LOAD_FAST                2 (parser)
+                      90 LOAD_METHOD              4 (render)
+                     112 LOAD_FAST                3 (username_style)
+                     114 LOAD_METHOD              5 (replace)
+                     136 LOAD_CONST               1 ('{USER}')
+                     138 LOAD_FAST                0 (user)
+                     140 LOAD_ATTR                6 (username)
+                     150 PRECALL                  2
+                     154 CALL                     2
+                     164 PRECALL                  1
+                     168 CALL                     1
+                     178 STORE_FAST               4 (styled_username)
+         
+          51         180 LOAD_FAST                4 (styled_username)
+                     182 RETURN_VALUE
+         
+          53     >>  184 LOAD_FAST                0 (user)
+                     186 LOAD_ATTR                6 (username)
+                     196 RETURN_VALUE
          consts
             None
             '{USER}'
-         names      ('get_highest_priority_group', 'style', 'username_style', 'rendered', 'replace', 'username')
-         varnames   ('user', 'group', 'username_style', 'styled_username')
+         names      ('get_highest_priority_group', 'get_parser', 'style', 'username_style', 'render', 'replace', 'username')
+         varnames   ('user', 'group', 'parser', 'username_style', 'styled_username')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_styled_username'
-         firstlineno 30
-         lnotab 0x02011e020401180140010402
+         firstlineno 44
+         lnotab 0x02011e0204011c0118015c010402
       code
          argcount  : 1
-         nlocals   : 3
-         stacksize : 4
+         nlocals   : 4
+         stacksize : 6
          flags     : 3
          code
             0x97007c006a00000000000000000080077c006a01000000000000000053
-            007c006a0000000000000000006a0200000000000000007d017c016a0300
-            00000000000000a004000000000000000000000000000000000000000064
-            017c006a010000000000000000a6020000ab0200000000000000007d027c
-            025300
-          41           0 RESUME                   0
+            00740500000000000000000000a6000000ab0000000000000000007d017c
+            006a0000000000000000006a0300000000000000007d027c01a004000000
+            00000000000000000000000000000000007c02a005000000000000000000
+            000000000000000000000064017c006a010000000000000000a6020000ab
+            020000000000000000a6010000ab0100000000000000007d037c035300
+          56           0 RESUME                   0
          
-          42           2 LOAD_FAST                0 (group)
+          57           2 LOAD_FAST                0 (group)
                        4 LOAD_ATTR                0 (style)
                       14 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 30)
          
-          43          16 LOAD_FAST                0 (group)
+          58          16 LOAD_FAST                0 (group)
                       18 LOAD_ATTR                1 (name)
                       28 RETURN_VALUE
          
-          45     >>   30 LOAD_FAST                0 (group)
-                      32 LOAD_ATTR                0 (style)
-                      42 LOAD_ATTR                2 (username_style)
-                      52 STORE_FAST               1 (username_style)
-         
-          46          54 LOAD_FAST                1 (username_style)
-                      56 LOAD_ATTR                3 (rendered)
-                      66 LOAD_METHOD              4 (replace)
-                      88 LOAD_CONST               1 ('{USER}')
-                      90 LOAD_FAST                0 (group)
-                      92 LOAD_ATTR                1 (name)
-                     102 PRECALL                  2
-                     106 CALL                     2
-                     116 STORE_FAST               2 (styled_group_name)
+          60     >>   30 LOAD_GLOBAL              5 (NULL + get_parser)
+                      42 PRECALL                  0
+                      46 CALL                     0
+                      56 STORE_FAST               1 (parser)
+         
+          61          58 LOAD_FAST                0 (group)
+                      60 LOAD_ATTR                0 (style)
+                      70 LOAD_ATTR                3 (username_style)
+                      80 STORE_FAST               2 (username_style)
+         
+          62          82 LOAD_FAST                1 (parser)
+                      84 LOAD_METHOD              4 (render)
+                     106 LOAD_FAST                2 (username_style)
+                     108 LOAD_METHOD              5 (replace)
+                     130 LOAD_CONST               1 ('{USER}')
+                     132 LOAD_FAST                0 (group)
+                     134 LOAD_ATTR                1 (name)
+                     144 PRECALL                  2
+                     148 CALL                     2
+                     158 PRECALL                  1
+                     162 CALL                     1
+                     172 STORE_FAST               3 (styled_group_name)
          
-          47         118 LOAD_FAST                2 (styled_group_name)
-                     120 RETURN_VALUE
+          63         174 LOAD_FAST                3 (styled_group_name)
+                     176 RETURN_VALUE
          consts
             None
             '{USER}'
-         names      ('style', 'name', 'username_style', 'rendered', 'replace')
-         varnames   ('group', 'username_style', 'styled_group_name')
+         names      ('style', 'name', 'get_parser', 'username_style', 'render', 'replace')
+         varnames   ('group', 'parser', 'username_style', 'styled_group_name')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_styled_group_name'
-         firstlineno 41
-         lnotab 0x02010e010e0218014001
+         firstlineno 56
+         lnotab 0x02010e010e021c0118015c01
       None
-   names      ('django.contrib.auth.models', 'Group', 'django.utils.text', 'slugify', 'get_unique_slug', 'get_highest_priority_group', 'get_styled_username', 'get_styled_group_name')
+   names      ('django.utils.text', 'slugify', 'precise_bbcode.bbcode', 'get_parser', 'punkweb_bb.settings', 'RENDERER', 'get_editor_widget', 'get_unique_slug', 'get_highest_priority_group', 'get_styled_username', 'get_styled_group_name')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0306100609060b
+   lnotab 0x00ff02010c010c010c03060d06100609060c
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,49 +1,51 @@
 magic:    0xa70d0d0a
-moddate:  0xb0a55766 (Wed May 29 22:01:20 2024 UTC)
-files sz: 17383
+moddate:  0x22e95766 (Thu May 30 02:49:06 2024 UTC)
+files sz: 18191
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a040100640064
       026c056d065a060100640064036c076d085a080100640064046c096d0a5a
       0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
       105a100100640064076c116d125a126d135a136d145a146d155a156d165a
-      166d175a176d185a186d195a190100640064086c1a6d1b5a1b0100640064
-      096c1c6d1d5a1d6d1e5a1e6d1f5a1f6d205a206d215a2101006400640a6c
-      226d235a2301006400640b6c246d255a2501006400640c6c266d275a2701
-      0002006502a6000000ab0000000000000000005a28640d84005a29640e84
-      005a2a640f84005a2b641084005a2c641184005a2d641284005a2e020065
-      066413ac14a6010000ab01000000000000000064158400a6000000ab0000
-      000000000000005a2f020065066413ac14a6010000ab0100000000000000
-      0064168400a6000000ab0000000000000000005a30020065066413ac14a6
-      010000ab01000000000000000064178400a6000000ab0000000000000000
-      005a31020065066413ac14a6010000ab01000000000000000064188400a6
-      000000ab0000000000000000005a32641984005a33020065066413ac14a6
-      010000ab010000000000000000641a8400a6000000ab0000000000000000
-      005a34020065066413ac14a6010000ab010000000000000000641b8400a6
-      000000ab0000000000000000005a35020065066413ac14a6010000ab0100
-      00000000000000641c8400a6000000ab0000000000000000005a36020065
-      066413ac14a6010000ab010000000000000000641d8400a6000000ab0000
-      000000000000005a37641e84005a38020065066413ac14a6010000ab0100
-      00000000000000641f8400a6000000ab0000000000000000005a39020065
-      066413ac14a6010000ab01000000000000000064208400a6000000ab0000
-      000000000000005a3a020065066413ac14a6010000ab0100000000000000
-      0064218400a6000000ab0000000000000000005a3b020065066413ac14a6
-      010000ab01000000000000000064228400a6000000ab0000000000000000
-      005a3c020065066413ac14a6010000ab01000000000000000064238400a6
-      000000ab0000000000000000005a3d020065066413ac14a6010000ab0100
-      0000000000000064248400a6000000ab0000000000000000005a3e020065
-      066413ac14a6010000ab01000000000000000064258400a6000000ab0000
-      000000000000005a3f642684005a40642784005a41642884005a42020065
-      066413ac14a6010000ab01000000000000000064298400a6000000ab0000
-      000000000000005a43642a84005a44642b5300
+      166d175a176d185a186d195a196d1a5a1a0100640064086c1b6d1c5a1c01
+      00640064096c1d6d1e5a1e6d1f5a1f6d205a206d215a216d225a22010064
+      00640a6c236d245a2401006400640b6c256d265a2601006400640c6c276d
+      285a28010002006502a6000000ab0000000000000000005a29640d84005a
+      2a640e84005a2b640f84005a2c641084005a2d641184005a2e641284005a
+      2f020065066413ac14a6010000ab01000000000000000064158400a60000
+      00ab0000000000000000005a30020065066413ac14a6010000ab01000000
+      000000000064168400a6000000ab0000000000000000005a310200650664
+      13ac14a6010000ab01000000000000000064178400a6000000ab00000000
+      00000000005a32020065066413ac14a6010000ab01000000000000000064
+      188400a6000000ab0000000000000000005a33641984005a340200650664
+      13ac14a6010000ab010000000000000000641a8400a6000000ab00000000
+      00000000005a35020065066413ac14a6010000ab01000000000000000064
+      1b8400a6000000ab0000000000000000005a36020065066413ac14a60100
+      00ab010000000000000000641c8400a6000000ab0000000000000000005a
+      37020065066413ac14a6010000ab010000000000000000641d8400a60000
+      00ab0000000000000000005a38641e84005a39020065066413ac14a60100
+      00ab010000000000000000641f8400a6000000ab0000000000000000005a
+      3a020065066413ac14a6010000ab01000000000000000064208400a60000
+      00ab0000000000000000005a3b020065066413ac14a6010000ab01000000
+      000000000064218400a6000000ab0000000000000000005a3c0200650664
+      13ac14a6010000ab01000000000000000064228400a6000000ab00000000
+      00000000005a3d020065066413ac14a6010000ab01000000000000000064
+      238400a6000000ab0000000000000000005a3e020065066413ac14a60100
+      00ab01000000000000000064248400a6000000ab0000000000000000005a
+      3f020065066413ac14a6010000ab01000000000000000064258400a60000
+      00ab0000000000000000005a40020065066413ac14a6010000ab01000000
+      000000000064268400a6000000ab0000000000000000005a41642784005a
+      42642884005a43642984005a44020065066413ac14a6010000ab01000000
+      0000000000642a8400a6000000ab0000000000000000005a45642b84005a
+      46642c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('authenticate', 'get_user_model', 'login', 'logout'))
                  6 IMPORT_NAME              0 (django.contrib.auth)
                  8 IMPORT_FROM              1 (authenticate)
                 10 STORE_NAME               1 (authenticate)
@@ -91,15 +93,15 @@
                 84 LOAD_CONST               6 (('timezone',))
                 86 IMPORT_NAME             15 (django.utils)
                 88 IMPORT_FROM             16 (timezone)
                 90 STORE_NAME              16 (timezone)
                 92 POP_TOP
    
      8          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               7 (('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm'))
+                96 LOAD_CONST               7 (('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'ThreadMoveForm'))
                 98 IMPORT_NAME             17 (punkweb_bb.forms)
                100 IMPORT_FROM             18 (BoardProfileModelForm)
                102 STORE_NAME              18 (BoardProfileModelForm)
                104 IMPORT_FROM             19 (CategoryModelForm)
                106 STORE_NAME              19 (CategoryModelForm)
                108 IMPORT_FROM             20 (LoginForm)
                110 STORE_NAME              20 (LoginForm)
@@ -109,363 +111,380 @@
                118 STORE_NAME              22 (ShoutModelForm)
                120 IMPORT_FROM             23 (SignUpForm)
                122 STORE_NAME              23 (SignUpForm)
                124 IMPORT_FROM             24 (SubcategoryModelForm)
                126 STORE_NAME              24 (SubcategoryModelForm)
                128 IMPORT_FROM             25 (ThreadModelForm)
                130 STORE_NAME              25 (ThreadModelForm)
-               132 POP_TOP
-   
-    18         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST               8 (('guest_list',))
-               138 IMPORT_NAME             26 (punkweb_bb.guests)
-               140 IMPORT_FROM             27 (guest_list)
-               142 STORE_NAME              27 (guest_list)
-               144 POP_TOP
-   
-    19         146 LOAD_CONST               0 (0)
-               148 LOAD_CONST               9 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
-               150 IMPORT_NAME             28 (punkweb_bb.models)
-               152 IMPORT_FROM             29 (Category)
-               154 STORE_NAME              29 (Category)
-               156 IMPORT_FROM             30 (Post)
-               158 STORE_NAME              30 (Post)
-               160 IMPORT_FROM             31 (Shout)
-               162 STORE_NAME              31 (Shout)
-               164 IMPORT_FROM             32 (Subcategory)
-               166 STORE_NAME              32 (Subcategory)
-               168 IMPORT_FROM             33 (Thread)
-               170 STORE_NAME              33 (Thread)
-               172 POP_TOP
-   
-    20         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              10 (('paginate_qs',))
-               178 IMPORT_NAME             34 (punkweb_bb.pagination)
-               180 IMPORT_FROM             35 (paginate_qs)
-               182 STORE_NAME              35 (paginate_qs)
-               184 POP_TOP
-   
-    21         186 LOAD_CONST               0 (0)
-               188 LOAD_CONST              11 (('htmx_redirect',))
-               190 IMPORT_NAME             36 (punkweb_bb.response)
-               192 IMPORT_FROM             37 (htmx_redirect)
-               194 STORE_NAME              37 (htmx_redirect)
-               196 POP_TOP
-   
-    22         198 LOAD_CONST               0 (0)
-               200 LOAD_CONST              12 (('get_unique_slug',))
-               202 IMPORT_NAME             38 (punkweb_bb.utils)
-               204 IMPORT_FROM             39 (get_unique_slug)
-               206 STORE_NAME              39 (get_unique_slug)
-               208 POP_TOP
-   
-    24         210 PUSH_NULL
-               212 LOAD_NAME                2 (get_user_model)
-               214 PRECALL                  0
-               218 CALL                     0
-               228 STORE_NAME              40 (User)
-   
-    27         230 LOAD_CONST              13 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 27>)
-               232 MAKE_FUNCTION            0
-               234 STORE_NAME              41 (signup_view)
-   
-    47         236 LOAD_CONST              14 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 47>)
-               238 MAKE_FUNCTION            0
-               240 STORE_NAME              42 (login_view)
-   
-    73         242 LOAD_CONST              15 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 73>)
-               244 MAKE_FUNCTION            0
-               246 STORE_NAME              43 (logout_view)
-   
-    78         248 LOAD_CONST              16 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 78>)
-               250 MAKE_FUNCTION            0
-               252 STORE_NAME              44 (index_view)
-   
-   110         254 LOAD_CONST              17 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 110>)
-               256 MAKE_FUNCTION            0
-               258 STORE_NAME              45 (profile_view)
-   
-   119         260 LOAD_CONST              18 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 119>)
-               262 MAKE_FUNCTION            0
-               264 STORE_NAME              46 (members_view)
-   
-   130         266 PUSH_NULL
-               268 LOAD_NAME                6 (login_required)
-               270 LOAD_CONST              19 ('/login/')
-               272 KW_NAMES                20
-               274 PRECALL                  1
-               278 CALL                     1
-   
-   131         288 LOAD_CONST              21 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 130>)
-               290 MAKE_FUNCTION            0
-   
-   130         292 PRECALL                  0
-               296 CALL                     0
-   
-   131         306 STORE_NAME              47 (settings_view)
-   
-   153         308 PUSH_NULL
-               310 LOAD_NAME                6 (login_required)
-               312 LOAD_CONST              19 ('/login/')
-               314 KW_NAMES                20
-               316 PRECALL                  1
-               320 CALL                     1
-   
-   154         330 LOAD_CONST              22 (<code object category_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 153>)
-               332 MAKE_FUNCTION            0
-   
-   153         334 PRECALL                  0
-               338 CALL                     0
-   
-   154         348 STORE_NAME              48 (category_create_view)
-   
-   176         350 PUSH_NULL
-               352 LOAD_NAME                6 (login_required)
-               354 LOAD_CONST              19 ('/login/')
-               356 KW_NAMES                20
-               358 PRECALL                  1
-               362 CALL                     1
-   
-   177         372 LOAD_CONST              23 (<code object category_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 176>)
-               374 MAKE_FUNCTION            0
-   
-   176         376 PRECALL                  0
-               380 CALL                     0
-   
-   177         390 STORE_NAME              49 (category_update_view)
-   
-   200         392 PUSH_NULL
-               394 LOAD_NAME                6 (login_required)
-               396 LOAD_CONST              19 ('/login/')
-               398 KW_NAMES                20
-               400 PRECALL                  1
-               404 CALL                     1
-   
-   201         414 LOAD_CONST              24 (<code object category_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 200>)
-               416 MAKE_FUNCTION            0
-   
-   200         418 PRECALL                  0
-               422 CALL                     0
-   
-   201         432 STORE_NAME              50 (category_delete_view)
-   
-   219         434 LOAD_CONST              25 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 219>)
-               436 MAKE_FUNCTION            0
-               438 STORE_NAME              51 (subcategory_view)
-   
-   231         440 PUSH_NULL
-               442 LOAD_NAME                6 (login_required)
-               444 LOAD_CONST              19 ('/login/')
-               446 KW_NAMES                20
-               448 PRECALL                  1
-               452 CALL                     1
-   
-   232         462 LOAD_CONST              26 (<code object subcategory_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 231>)
-               464 MAKE_FUNCTION            0
-   
-   231         466 PRECALL                  0
-               470 CALL                     0
-   
-   232         480 STORE_NAME              52 (subcategory_create_view)
-   
-   260         482 PUSH_NULL
-               484 LOAD_NAME                6 (login_required)
-               486 LOAD_CONST              19 ('/login/')
-               488 KW_NAMES                20
-               490 PRECALL                  1
-               494 CALL                     1
-   
-   261         504 LOAD_CONST              27 (<code object subcategory_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 260>)
-               506 MAKE_FUNCTION            0
-   
-   260         508 PRECALL                  0
-               512 CALL                     0
-   
-   261         522 STORE_NAME              53 (subcategory_update_view)
-   
-   286         524 PUSH_NULL
-               526 LOAD_NAME                6 (login_required)
-               528 LOAD_CONST              19 ('/login/')
-               530 KW_NAMES                20
-               532 PRECALL                  1
-               536 CALL                     1
-   
-   287         546 LOAD_CONST              28 (<code object subcategory_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 286>)
-               548 MAKE_FUNCTION            0
-   
-   286         550 PRECALL                  0
-               554 CALL                     0
-   
-   287         564 STORE_NAME              54 (subcategory_delete_view)
-   
-   309         566 PUSH_NULL
-               568 LOAD_NAME                6 (login_required)
-               570 LOAD_CONST              19 ('/login/')
-               572 KW_NAMES                20
-               574 PRECALL                  1
-               578 CALL                     1
-   
-   310         588 LOAD_CONST              29 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 309>)
-               590 MAKE_FUNCTION            0
-   
-   309         592 PRECALL                  0
-               596 CALL                     0
-   
-   310         606 STORE_NAME              55 (thread_create_view)
-   
-   338         608 LOAD_CONST              30 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 338>)
-               610 MAKE_FUNCTION            0
-               612 STORE_NAME              56 (thread_view)
-   
-   360         614 PUSH_NULL
-               616 LOAD_NAME                6 (login_required)
-               618 LOAD_CONST              19 ('/login/')
-               620 KW_NAMES                20
-               622 PRECALL                  1
-               626 CALL                     1
-   
-   361         636 LOAD_CONST              31 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 360>)
-               638 MAKE_FUNCTION            0
-   
-   360         640 PRECALL                  0
-               644 CALL                     0
-   
-   361         654 STORE_NAME              57 (thread_update_view)
-   
-   386         656 PUSH_NULL
-               658 LOAD_NAME                6 (login_required)
-               660 LOAD_CONST              19 ('/login/')
-               662 KW_NAMES                20
-               664 PRECALL                  1
-               668 CALL                     1
-   
-   387         678 LOAD_CONST              32 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 386>)
-               680 MAKE_FUNCTION            0
-   
-   386         682 PRECALL                  0
-               686 CALL                     0
-   
-   387         696 STORE_NAME              58 (thread_delete_view)
-   
-   407         698 PUSH_NULL
-               700 LOAD_NAME                6 (login_required)
-               702 LOAD_CONST              19 ('/login/')
-               704 KW_NAMES                20
-               706 PRECALL                  1
-               710 CALL                     1
-   
-   408         720 LOAD_CONST              33 (<code object thread_pin_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 407>)
-               722 MAKE_FUNCTION            0
-   
-   407         724 PRECALL                  0
-               728 CALL                     0
-   
-   408         738 STORE_NAME              59 (thread_pin_view)
-   
-   420         740 PUSH_NULL
-               742 LOAD_NAME                6 (login_required)
-               744 LOAD_CONST              19 ('/login/')
-               746 KW_NAMES                20
-               748 PRECALL                  1
-               752 CALL                     1
-   
-   421         762 LOAD_CONST              34 (<code object thread_close_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 420>)
-               764 MAKE_FUNCTION            0
-   
-   420         766 PRECALL                  0
-               770 CALL                     0
-   
-   421         780 STORE_NAME              60 (thread_close_view)
-   
-   433         782 PUSH_NULL
-               784 LOAD_NAME                6 (login_required)
-               786 LOAD_CONST              19 ('/login/')
-               788 KW_NAMES                20
-               790 PRECALL                  1
-               794 CALL                     1
-   
-   434         804 LOAD_CONST              35 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 433>)
-               806 MAKE_FUNCTION            0
-   
-   433         808 PRECALL                  0
-               812 CALL                     0
-   
-   434         822 STORE_NAME              61 (post_create_view)
-   
-   453         824 PUSH_NULL
-               826 LOAD_NAME                6 (login_required)
-               828 LOAD_CONST              19 ('/login/')
-               830 KW_NAMES                20
-               832 PRECALL                  1
-               836 CALL                     1
-   
-   454         846 LOAD_CONST              36 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 453>)
-               848 MAKE_FUNCTION            0
-   
-   453         850 PRECALL                  0
-               854 CALL                     0
-   
-   454         864 STORE_NAME              62 (post_update_view)
-   
-   478         866 PUSH_NULL
-               868 LOAD_NAME                6 (login_required)
-               870 LOAD_CONST              19 ('/login/')
-               872 KW_NAMES                20
-               874 PRECALL                  1
-               878 CALL                     1
-   
-   479         888 LOAD_CONST              37 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 478>)
-               890 MAKE_FUNCTION            0
-   
-   478         892 PRECALL                  0
-               896 CALL                     0
-   
-   479         906 STORE_NAME              63 (post_delete_view)
-   
-   497         908 LOAD_CONST              38 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 497>)
-               910 MAKE_FUNCTION            0
-               912 STORE_NAME              64 (current_shouts)
-   
-   503         914 LOAD_CONST              39 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 503>)
-               916 MAKE_FUNCTION            0
-               918 STORE_NAME              65 (shout_list_view)
-   
-   512         920 LOAD_CONST              40 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 512>)
-               922 MAKE_FUNCTION            0
-               924 STORE_NAME              66 (shout_create_view)
-   
-   535         926 PUSH_NULL
-               928 LOAD_NAME                6 (login_required)
-               930 LOAD_CONST              19 ('/login/')
-               932 KW_NAMES                20
-               934 PRECALL                  1
-               938 CALL                     1
-   
-   536         948 LOAD_CONST              41 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 535>)
-               950 MAKE_FUNCTION            0
-   
-   535         952 PRECALL                  0
-               956 CALL                     0
-   
-   536         966 STORE_NAME              67 (shout_delete_view)
-   
-   554         968 LOAD_CONST              42 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 554>)
-               970 MAKE_FUNCTION            0
-               972 STORE_NAME              68 (bbcode_view)
-               974 LOAD_CONST              43 (None)
-               976 RETURN_VALUE
+               132 IMPORT_FROM             26 (ThreadMoveForm)
+               134 STORE_NAME              26 (ThreadMoveForm)
+               136 POP_TOP
+   
+    19         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST               8 (('guest_list',))
+               142 IMPORT_NAME             27 (punkweb_bb.guests)
+               144 IMPORT_FROM             28 (guest_list)
+               146 STORE_NAME              28 (guest_list)
+               148 POP_TOP
+   
+    20         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST               9 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
+               154 IMPORT_NAME             29 (punkweb_bb.models)
+               156 IMPORT_FROM             30 (Category)
+               158 STORE_NAME              30 (Category)
+               160 IMPORT_FROM             31 (Post)
+               162 STORE_NAME              31 (Post)
+               164 IMPORT_FROM             32 (Shout)
+               166 STORE_NAME              32 (Shout)
+               168 IMPORT_FROM             33 (Subcategory)
+               170 STORE_NAME              33 (Subcategory)
+               172 IMPORT_FROM             34 (Thread)
+               174 STORE_NAME              34 (Thread)
+               176 POP_TOP
+   
+    21         178 LOAD_CONST               0 (0)
+               180 LOAD_CONST              10 (('paginate_qs',))
+               182 IMPORT_NAME             35 (punkweb_bb.pagination)
+               184 IMPORT_FROM             36 (paginate_qs)
+               186 STORE_NAME              36 (paginate_qs)
+               188 POP_TOP
+   
+    22         190 LOAD_CONST               0 (0)
+               192 LOAD_CONST              11 (('htmx_redirect',))
+               194 IMPORT_NAME             37 (punkweb_bb.response)
+               196 IMPORT_FROM             38 (htmx_redirect)
+               198 STORE_NAME              38 (htmx_redirect)
+               200 POP_TOP
+   
+    23         202 LOAD_CONST               0 (0)
+               204 LOAD_CONST              12 (('get_unique_slug',))
+               206 IMPORT_NAME             39 (punkweb_bb.utils)
+               208 IMPORT_FROM             40 (get_unique_slug)
+               210 STORE_NAME              40 (get_unique_slug)
+               212 POP_TOP
+   
+    25         214 PUSH_NULL
+               216 LOAD_NAME                2 (get_user_model)
+               218 PRECALL                  0
+               222 CALL                     0
+               232 STORE_NAME              41 (User)
+   
+    28         234 LOAD_CONST              13 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 28>)
+               236 MAKE_FUNCTION            0
+               238 STORE_NAME              42 (signup_view)
+   
+    48         240 LOAD_CONST              14 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 48>)
+               242 MAKE_FUNCTION            0
+               244 STORE_NAME              43 (login_view)
+   
+    74         246 LOAD_CONST              15 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 74>)
+               248 MAKE_FUNCTION            0
+               250 STORE_NAME              44 (logout_view)
+   
+    79         252 LOAD_CONST              16 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 79>)
+               254 MAKE_FUNCTION            0
+               256 STORE_NAME              45 (index_view)
+   
+   111         258 LOAD_CONST              17 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 111>)
+               260 MAKE_FUNCTION            0
+               262 STORE_NAME              46 (profile_view)
+   
+   120         264 LOAD_CONST              18 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 120>)
+               266 MAKE_FUNCTION            0
+               268 STORE_NAME              47 (members_view)
+   
+   131         270 PUSH_NULL
+               272 LOAD_NAME                6 (login_required)
+               274 LOAD_CONST              19 ('/login/')
+               276 KW_NAMES                20
+               278 PRECALL                  1
+               282 CALL                     1
+   
+   132         292 LOAD_CONST              21 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 131>)
+               294 MAKE_FUNCTION            0
+   
+   131         296 PRECALL                  0
+               300 CALL                     0
+   
+   132         310 STORE_NAME              48 (settings_view)
+   
+   154         312 PUSH_NULL
+               314 LOAD_NAME                6 (login_required)
+               316 LOAD_CONST              19 ('/login/')
+               318 KW_NAMES                20
+               320 PRECALL                  1
+               324 CALL                     1
+   
+   155         334 LOAD_CONST              22 (<code object category_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 154>)
+               336 MAKE_FUNCTION            0
+   
+   154         338 PRECALL                  0
+               342 CALL                     0
+   
+   155         352 STORE_NAME              49 (category_create_view)
+   
+   177         354 PUSH_NULL
+               356 LOAD_NAME                6 (login_required)
+               358 LOAD_CONST              19 ('/login/')
+               360 KW_NAMES                20
+               362 PRECALL                  1
+               366 CALL                     1
+   
+   178         376 LOAD_CONST              23 (<code object category_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 177>)
+               378 MAKE_FUNCTION            0
+   
+   177         380 PRECALL                  0
+               384 CALL                     0
+   
+   178         394 STORE_NAME              50 (category_update_view)
+   
+   201         396 PUSH_NULL
+               398 LOAD_NAME                6 (login_required)
+               400 LOAD_CONST              19 ('/login/')
+               402 KW_NAMES                20
+               404 PRECALL                  1
+               408 CALL                     1
+   
+   202         418 LOAD_CONST              24 (<code object category_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 201>)
+               420 MAKE_FUNCTION            0
+   
+   201         422 PRECALL                  0
+               426 CALL                     0
+   
+   202         436 STORE_NAME              51 (category_delete_view)
+   
+   220         438 LOAD_CONST              25 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 220>)
+               440 MAKE_FUNCTION            0
+               442 STORE_NAME              52 (subcategory_view)
+   
+   232         444 PUSH_NULL
+               446 LOAD_NAME                6 (login_required)
+               448 LOAD_CONST              19 ('/login/')
+               450 KW_NAMES                20
+               452 PRECALL                  1
+               456 CALL                     1
+   
+   233         466 LOAD_CONST              26 (<code object subcategory_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 232>)
+               468 MAKE_FUNCTION            0
+   
+   232         470 PRECALL                  0
+               474 CALL                     0
+   
+   233         484 STORE_NAME              53 (subcategory_create_view)
+   
+   261         486 PUSH_NULL
+               488 LOAD_NAME                6 (login_required)
+               490 LOAD_CONST              19 ('/login/')
+               492 KW_NAMES                20
+               494 PRECALL                  1
+               498 CALL                     1
+   
+   262         508 LOAD_CONST              27 (<code object subcategory_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 261>)
+               510 MAKE_FUNCTION            0
+   
+   261         512 PRECALL                  0
+               516 CALL                     0
+   
+   262         526 STORE_NAME              54 (subcategory_update_view)
+   
+   287         528 PUSH_NULL
+               530 LOAD_NAME                6 (login_required)
+               532 LOAD_CONST              19 ('/login/')
+               534 KW_NAMES                20
+               536 PRECALL                  1
+               540 CALL                     1
+   
+   288         550 LOAD_CONST              28 (<code object subcategory_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 287>)
+               552 MAKE_FUNCTION            0
+   
+   287         554 PRECALL                  0
+               558 CALL                     0
+   
+   288         568 STORE_NAME              55 (subcategory_delete_view)
+   
+   310         570 PUSH_NULL
+               572 LOAD_NAME                6 (login_required)
+               574 LOAD_CONST              19 ('/login/')
+               576 KW_NAMES                20
+               578 PRECALL                  1
+               582 CALL                     1
+   
+   311         592 LOAD_CONST              29 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 310>)
+               594 MAKE_FUNCTION            0
+   
+   310         596 PRECALL                  0
+               600 CALL                     0
+   
+   311         610 STORE_NAME              56 (thread_create_view)
+   
+   339         612 LOAD_CONST              30 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 339>)
+               614 MAKE_FUNCTION            0
+               616 STORE_NAME              57 (thread_view)
+   
+   361         618 PUSH_NULL
+               620 LOAD_NAME                6 (login_required)
+               622 LOAD_CONST              19 ('/login/')
+               624 KW_NAMES                20
+               626 PRECALL                  1
+               630 CALL                     1
+   
+   362         640 LOAD_CONST              31 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 361>)
+               642 MAKE_FUNCTION            0
+   
+   361         644 PRECALL                  0
+               648 CALL                     0
+   
+   362         658 STORE_NAME              58 (thread_update_view)
+   
+   387         660 PUSH_NULL
+               662 LOAD_NAME                6 (login_required)
+               664 LOAD_CONST              19 ('/login/')
+               666 KW_NAMES                20
+               668 PRECALL                  1
+               672 CALL                     1
+   
+   388         682 LOAD_CONST              32 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 387>)
+               684 MAKE_FUNCTION            0
+   
+   387         686 PRECALL                  0
+               690 CALL                     0
+   
+   388         700 STORE_NAME              59 (thread_delete_view)
+   
+   408         702 PUSH_NULL
+               704 LOAD_NAME                6 (login_required)
+               706 LOAD_CONST              19 ('/login/')
+               708 KW_NAMES                20
+               710 PRECALL                  1
+               714 CALL                     1
+   
+   409         724 LOAD_CONST              33 (<code object thread_pin_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 408>)
+               726 MAKE_FUNCTION            0
+   
+   408         728 PRECALL                  0
+               732 CALL                     0
+   
+   409         742 STORE_NAME              60 (thread_pin_view)
+   
+   421         744 PUSH_NULL
+               746 LOAD_NAME                6 (login_required)
+               748 LOAD_CONST              19 ('/login/')
+               750 KW_NAMES                20
+               752 PRECALL                  1
+               756 CALL                     1
+   
+   422         766 LOAD_CONST              34 (<code object thread_close_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 421>)
+               768 MAKE_FUNCTION            0
+   
+   421         770 PRECALL                  0
+               774 CALL                     0
+   
+   422         784 STORE_NAME              61 (thread_close_view)
+   
+   434         786 PUSH_NULL
+               788 LOAD_NAME                6 (login_required)
+               790 LOAD_CONST              19 ('/login/')
+               792 KW_NAMES                20
+               794 PRECALL                  1
+               798 CALL                     1
+   
+   435         808 LOAD_CONST              35 (<code object thread_move_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 434>)
+               810 MAKE_FUNCTION            0
+   
+   434         812 PRECALL                  0
+               816 CALL                     0
+   
+   435         826 STORE_NAME              62 (thread_move_view)
+   
+   464         828 PUSH_NULL
+               830 LOAD_NAME                6 (login_required)
+               832 LOAD_CONST              19 ('/login/')
+               834 KW_NAMES                20
+               836 PRECALL                  1
+               840 CALL                     1
+   
+   465         850 LOAD_CONST              36 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 464>)
+               852 MAKE_FUNCTION            0
+   
+   464         854 PRECALL                  0
+               858 CALL                     0
+   
+   465         868 STORE_NAME              63 (post_create_view)
+   
+   484         870 PUSH_NULL
+               872 LOAD_NAME                6 (login_required)
+               874 LOAD_CONST              19 ('/login/')
+               876 KW_NAMES                20
+               878 PRECALL                  1
+               882 CALL                     1
+   
+   485         892 LOAD_CONST              37 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 484>)
+               894 MAKE_FUNCTION            0
+   
+   484         896 PRECALL                  0
+               900 CALL                     0
+   
+   485         910 STORE_NAME              64 (post_update_view)
+   
+   509         912 PUSH_NULL
+               914 LOAD_NAME                6 (login_required)
+               916 LOAD_CONST              19 ('/login/')
+               918 KW_NAMES                20
+               920 PRECALL                  1
+               924 CALL                     1
+   
+   510         934 LOAD_CONST              38 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 509>)
+               936 MAKE_FUNCTION            0
+   
+   509         938 PRECALL                  0
+               942 CALL                     0
+   
+   510         952 STORE_NAME              65 (post_delete_view)
+   
+   528         954 LOAD_CONST              39 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 528>)
+               956 MAKE_FUNCTION            0
+               958 STORE_NAME              66 (current_shouts)
+   
+   534         960 LOAD_CONST              40 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 534>)
+               962 MAKE_FUNCTION            0
+               964 STORE_NAME              67 (shout_list_view)
+   
+   543         966 LOAD_CONST              41 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 543>)
+               968 MAKE_FUNCTION            0
+               970 STORE_NAME              68 (shout_create_view)
+   
+   566         972 PUSH_NULL
+               974 LOAD_NAME                6 (login_required)
+               976 LOAD_CONST              19 ('/login/')
+               978 KW_NAMES                20
+               980 PRECALL                  1
+               984 CALL                     1
+   
+   567         994 LOAD_CONST              42 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 566>)
+               996 MAKE_FUNCTION            0
+   
+   566         998 PRECALL                  0
+              1002 CALL                     0
+   
+   567        1012 STORE_NAME              69 (shout_delete_view)
+   
+   585        1014 LOAD_CONST              43 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 585>)
+              1016 MAKE_FUNCTION            0
+              1018 STORE_NAME              70 (bbcode_view)
+              1020 LOAD_CONST              44 (None)
+              1022 RETURN_VALUE
    consts
       0
       ('authenticate', 'get_user_model', 'login', 'logout')
       ('login_required',)
       ('HttpResponseForbidden',)
       ('get_object_or_404', 'redirect', 'render')
       ('reverse',)
       ('timezone',)
-      ('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm')
+      ('BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'ThreadMoveForm')
       ('guest_list',)
       ('Category', 'Post', 'Shout', 'Subcategory', 'Thread')
       ('paginate_qs',)
       ('htmx_redirect',)
       ('get_unique_slug',)
       code
          argcount  : 1
@@ -480,72 +499,72 @@
             01a0060000000000000000000000000000000000000000a6000000ab0000
             0000000000000072237c01a0070000000000000000000000000000000000
             000000a6000000ab00000000000000000001007405000000000000000000
             006403a6010000ab01000000000000000053006e0e740900000000000000
             000000a6000000ab0000000000000000007d0164047c0169017d02741100
             0000000000000000007c0064057c02a6030000ab03000000000000000053
             00
-          27           0 RESUME                   0
+          28           0 RESUME                   0
          
-          28           2 LOAD_FAST                0 (request)
+          29           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          29          26 LOAD_GLOBAL              5 (NULL + redirect)
+          30          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          31     >>   56 LOAD_FAST                0 (request)
+          32     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE    76 (to 230)
          
-          32          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
+          33          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_ATTR                5 (POST)
                      102 PRECALL                  1
                      106 CALL                     1
                      116 STORE_FAST               1 (form)
          
-          34         118 LOAD_FAST                1 (form)
+          35         118 LOAD_FAST                1 (form)
                      120 LOAD_METHOD              6 (is_valid)
                      142 PRECALL                  0
                      146 CALL                     0
                      156 POP_JUMP_FORWARD_IF_FALSE    35 (to 228)
          
-          35         158 LOAD_FAST                1 (form)
+          36         158 LOAD_FAST                1 (form)
                      160 LOAD_METHOD              7 (save)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-          37         198 LOAD_GLOBAL              5 (NULL + redirect)
+          38         198 LOAD_GLOBAL              5 (NULL + redirect)
                      210 LOAD_CONST               3 ('punkweb_bb:login')
                      212 PRECALL                  1
                      216 CALL                     1
                      226 RETURN_VALUE
          
-          34     >>  228 JUMP_FORWARD            14 (to 258)
+          35     >>  228 JUMP_FORWARD            14 (to 258)
          
-          39     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
+          40     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
                      242 PRECALL                  0
                      246 CALL                     0
                      256 STORE_FAST               1 (form)
          
-          42     >>  258 LOAD_CONST               4 ('form')
+          43     >>  258 LOAD_CONST               4 ('form')
                      260 LOAD_FAST                1 (form)
          
-          41         262 BUILD_MAP                1
+          42         262 BUILD_MAP                1
                      264 STORE_FAST               2 (context)
          
-          44         266 LOAD_GLOBAL             17 (NULL + render)
+          45         266 LOAD_GLOBAL             17 (NULL + render)
                      278 LOAD_FAST                0 (request)
                      280 LOAD_CONST               5 ('punkweb_bb/signup.html')
                      282 LOAD_FAST                2 (context)
                      284 PRECALL                  3
                      288 CALL                     3
                      298 RETURN_VALUE
          consts
@@ -557,15 +576,15 @@
             'punkweb_bb/signup.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'SignUpForm', 'POST', 'is_valid', 'save', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'signup_view'
-         firstlineno 27
+         firstlineno 28
          lnotab 0x020118011e0216012802280128021efd02051c0304ff0403
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -578,97 +597,97 @@
             00000000007d027c016a0700000000000000006404190000000000000000
             007d037411000000000000000000007c007c027c03ac05a6030000ab0300
             000000000000007d047c04811f7413000000000000000000007c007c04a6
             020000ab02000000000000000001007405000000000000000000006401a6
             010000ab01000000000000000053006e0e740900000000000000000000a6
             000000ab0000000000000000007d0164067c0169017d0574150000000000
             00000000007c0064077c05a6030000ab0300000000000000005300
-          47           0 RESUME                   0
+          48           0 RESUME                   0
          
-          48           2 LOAD_FAST                0 (request)
+          49           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          49          26 LOAD_GLOBAL              5 (NULL + redirect)
+          50          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          51     >>   56 LOAD_FAST                0 (request)
+          52     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE   119 (to 316)
          
-          52          78 LOAD_GLOBAL              9 (NULL + LoginForm)
+          53          78 LOAD_GLOBAL              9 (NULL + LoginForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 PRECALL                  2
                      108 CALL                     2
                      118 STORE_FAST               1 (form)
          
-          54         120 LOAD_FAST                1 (form)
+          55         120 LOAD_FAST                1 (form)
                      122 LOAD_METHOD              6 (is_valid)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 POP_JUMP_FORWARD_IF_FALSE    77 (to 314)
          
-          55         160 LOAD_FAST                1 (form)
+          56         160 LOAD_FAST                1 (form)
                      162 LOAD_ATTR                7 (cleaned_data)
                      172 LOAD_CONST               3 ('username')
                      174 BINARY_SUBSCR
                      184 STORE_FAST               2 (username)
          
-          56         186 LOAD_FAST                1 (form)
+          57         186 LOAD_FAST                1 (form)
                      188 LOAD_ATTR                7 (cleaned_data)
                      198 LOAD_CONST               4 ('password')
                      200 BINARY_SUBSCR
                      210 STORE_FAST               3 (password)
          
-          58         212 LOAD_GLOBAL             17 (NULL + authenticate)
+          59         212 LOAD_GLOBAL             17 (NULL + authenticate)
                      224 LOAD_FAST                0 (request)
                      226 LOAD_FAST                2 (username)
                      228 LOAD_FAST                3 (password)
                      230 KW_NAMES                 5
                      232 PRECALL                  3
                      236 CALL                     3
                      246 STORE_FAST               4 (user)
          
-          60         248 LOAD_FAST                4 (user)
+          61         248 LOAD_FAST                4 (user)
                      250 POP_JUMP_FORWARD_IF_NONE    31 (to 314)
          
-          61         252 LOAD_GLOBAL             19 (NULL + login)
+          62         252 LOAD_GLOBAL             19 (NULL + login)
                      264 LOAD_FAST                0 (request)
                      266 LOAD_FAST                4 (user)
                      268 PRECALL                  2
                      272 CALL                     2
                      282 POP_TOP
          
-          63         284 LOAD_GLOBAL              5 (NULL + redirect)
+          64         284 LOAD_GLOBAL              5 (NULL + redirect)
                      296 LOAD_CONST               1 ('punkweb_bb:index')
                      298 PRECALL                  1
                      302 CALL                     1
                      312 RETURN_VALUE
                  >>  314 JUMP_FORWARD            14 (to 344)
          
-          65     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
+          66     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
                      328 PRECALL                  0
                      332 CALL                     0
                      342 STORE_FAST               1 (form)
          
-          68     >>  344 LOAD_CONST               6 ('form')
+          69     >>  344 LOAD_CONST               6 ('form')
                      346 LOAD_FAST                1 (form)
          
-          67         348 BUILD_MAP                1
+          68         348 BUILD_MAP                1
                      350 STORE_FAST               5 (context)
          
-          70         352 LOAD_GLOBAL             21 (NULL + render)
+          71         352 LOAD_GLOBAL             21 (NULL + render)
                      364 LOAD_FAST                0 (request)
                      366 LOAD_CONST               7 ('punkweb_bb/login.html')
                      368 LOAD_FAST                5 (context)
                      370 PRECALL                  3
                      374 CALL                     3
                      384 RETURN_VALUE
          consts
@@ -682,50 +701,50 @@
             'punkweb_bb/login.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'LoginForm', 'POST', 'is_valid', 'cleaned_data', 'authenticate', 'login', 'render')
          varnames   ('request', 'form', 'username', 'password', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'login_view'
-         firstlineno 47
+         firstlineno 48
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
-          73           0 RESUME                   0
+          74           0 RESUME                   0
          
-          74           2 LOAD_GLOBAL              1 (NULL + logout)
+          75           2 LOAD_GLOBAL              1 (NULL + logout)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          75          32 LOAD_GLOBAL              3 (NULL + redirect)
+          76          32 LOAD_GLOBAL              3 (NULL + redirect)
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
-         firstlineno 73
+         firstlineno 74
          lnotab 0x02011e01
       code
          argcount  : 1
          nlocals   : 13
          stacksize : 11
          flags     : 3
          code
@@ -749,141 +768,141 @@
             0000000000000000007d08640784007c074400a6000000ab000000000000
             0000007d097415000000000000000000006a0b0000000000000000a60000
             00ab0000000000000000007d0a7419000000000000000000007c08a60100
             00ab0100000000000000007419000000000000000000007c09a6010000ab
             0100000000000000007a0000007c0a7a0000007d0b7c017c027c037c047c
             057c067c087c097c0a7c0b64089c0a7d0c741b000000000000000000007c
             0064097c0cac0aa6030000ab0300000000000000005300
-          78           0 RESUME                   0
+          79           0 RESUME                   0
          
-          79           2 LOAD_GLOBAL              0 (Category)
+          80           2 LOAD_GLOBAL              0 (Category)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (all)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               1 (categories)
          
-          81          62 LOAD_GLOBAL              6 (Thread)
+          82          62 LOAD_GLOBAL              6 (Thread)
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
          
-          83         176 LOAD_GLOBAL              6 (Thread)
+          84         176 LOAD_GLOBAL              6 (Thread)
                      188 LOAD_ATTR                1 (objects)
                      198 LOAD_METHOD              5 (count)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 STORE_FAST               3 (thread_count)
          
-          84         236 LOAD_GLOBAL             12 (Post)
+          85         236 LOAD_GLOBAL             12 (Post)
                      248 LOAD_ATTR                1 (objects)
                      258 LOAD_METHOD              5 (count)
                      280 PRECALL                  0
                      284 CALL                     0
                      294 STORE_FAST               4 (post_count)
          
-          86         296 LOAD_GLOBAL             14 (User)
+          87         296 LOAD_GLOBAL             14 (User)
                      308 LOAD_ATTR                1 (objects)
                      318 LOAD_METHOD              8 (select_related)
                      340 LOAD_CONST               3 ('profile')
                      342 PRECALL                  1
                      346 CALL                     1
                      356 LOAD_METHOD              2 (all)
                      378 PRECALL                  0
                      382 CALL                     0
                      392 STORE_FAST               5 (users)
          
-          87         394 LOAD_FAST                5 (users)
+          88         394 LOAD_FAST                5 (users)
                      396 LOAD_METHOD              4 (order_by)
                      418 LOAD_CONST               4 ('-profile__created_at')
                      420 PRECALL                  1
                      424 CALL                     1
                      434 LOAD_METHOD              9 (first)
                      456 PRECALL                  0
                      460 CALL                     0
                      470 STORE_FAST               6 (newest_user)
          
-          89         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 89>)
+          90         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 90>)
                      474 MAKE_FUNCTION            0
                      476 LOAD_FAST                5 (users)
                      478 GET_ITER
                      480 PRECALL                  0
                      484 CALL                     0
                      494 STORE_FAST               7 (users_online)
          
-          90         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 90>)
+          91         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 91>)
                      498 MAKE_FUNCTION            0
                      500 LOAD_FAST                7 (users_online)
                      502 GET_ITER
                      504 PRECALL                  0
                      508 CALL                     0
                      518 STORE_FAST               8 (members_online)
          
-          91         520 LOAD_CONST               7 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 91>)
+          92         520 LOAD_CONST               7 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 92>)
                      522 MAKE_FUNCTION            0
                      524 LOAD_FAST                7 (users_online)
                      526 GET_ITER
                      528 PRECALL                  0
                      532 CALL                     0
                      542 STORE_FAST               9 (staff_online)
          
-          92         544 LOAD_GLOBAL             21 (NULL + guest_list)
+          93         544 LOAD_GLOBAL             21 (NULL + guest_list)
                      556 LOAD_ATTR               11 (length)
                      566 PRECALL                  0
                      570 CALL                     0
                      580 STORE_FAST              10 (guests_online)
          
-          93         582 LOAD_GLOBAL             25 (NULL + len)
+          94         582 LOAD_GLOBAL             25 (NULL + len)
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
          
-          96         650 LOAD_FAST                1 (categories)
+          97         650 LOAD_FAST                1 (categories)
          
-          97         652 LOAD_FAST                2 (recent_threads)
+          98         652 LOAD_FAST                2 (recent_threads)
          
-          98         654 LOAD_FAST                3 (thread_count)
+          99         654 LOAD_FAST                3 (thread_count)
          
-          99         656 LOAD_FAST                4 (post_count)
+         100         656 LOAD_FAST                4 (post_count)
          
-         100         658 LOAD_FAST                5 (users)
+         101         658 LOAD_FAST                5 (users)
          
-         101         660 LOAD_FAST                6 (newest_user)
+         102         660 LOAD_FAST                6 (newest_user)
          
-         102         662 LOAD_FAST                8 (members_online)
+         103         662 LOAD_FAST                8 (members_online)
          
-         103         664 LOAD_FAST                9 (staff_online)
+         104         664 LOAD_FAST                9 (staff_online)
          
-         104         666 LOAD_FAST               10 (guests_online)
+         105         666 LOAD_FAST               10 (guests_online)
          
-         105         668 LOAD_FAST               11 (total_online)
+         106         668 LOAD_FAST               11 (total_online)
          
-          95         670 LOAD_CONST               8 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online'))
+          96         670 LOAD_CONST               8 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online'))
                      672 BUILD_CONST_KEY_MAP     10
                      674 STORE_FAST              12 (context)
          
-         107         676 LOAD_GLOBAL             27 (NULL + render)
+         108         676 LOAD_GLOBAL             27 (NULL + render)
                      688 LOAD_FAST                0 (request)
                      690 LOAD_CONST               9 ('punkweb_bb/index.html')
                      692 LOAD_FAST               12 (context)
                      694 KW_NAMES                10
                      696 PRECALL                  3
                      700 CALL                     3
                      710 RETURN_VALUE
@@ -897,15 +916,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d107d017c016a0000000000000000006a010000000000
                   000000af0e7c0191028c115300
-                89           0 RESUME                   0
+                90           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                16 (to 40)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (profile)
                             22 LOAD_ATTR                1 (is_online)
@@ -917,25 +936,25 @@
                consts
                names      ('profile', 'is_online')
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 89
+               firstlineno 90
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d0b7d017c016a000000000000000000b0097c0191028c
                   0c5300
-                90           0 RESUME                   0
+                91           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                11 (to 30)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (is_staff)
                             22 POP_JUMP_BACKWARD_IF_TRUE     9 (to 6)
@@ -946,25 +965,25 @@
                consts
                names      ('is_staff',)
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 90
+               firstlineno 91
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d0b7d017c016a000000000000000000af097c0191028c
                   0c5300
-                91           0 RESUME                   0
+                92           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                11 (to 30)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (is_staff)
                             22 POP_JUMP_BACKWARD_IF_FALSE     9 (to 6)
@@ -975,56 +994,56 @@
                consts
                names      ('is_staff',)
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 91
+               firstlineno 92
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
-         firstlineno 78
+         firstlineno 79
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
-         110           0 RESUME                   0
+         111           0 RESUME                   0
          
-         111           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         112           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (User)
                       26 LOAD_FAST                1 (user_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (user)
          
-         114          46 LOAD_CONST               2 ('user')
+         115          46 LOAD_CONST               2 ('user')
                       48 LOAD_FAST                2 (user)
          
-         113          50 BUILD_MAP                1
+         114          50 BUILD_MAP                1
                       52 STORE_FAST               3 (context)
          
-         116          54 LOAD_GLOBAL              5 (NULL + render)
+         117          54 LOAD_GLOBAL              5 (NULL + render)
                       66 LOAD_FAST                0 (request)
                       68 LOAD_CONST               3 ('punkweb_bb/profile.html')
                       70 LOAD_FAST                3 (context)
                       72 KW_NAMES                 4
                       74 PRECALL                  3
                       78 CALL                     3
                       88 RETURN_VALUE
@@ -1036,55 +1055,55 @@
             ('context',)
          names      ('get_object_or_404', 'User', 'render')
          varnames   ('request', 'user_id', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'profile_view'
-         firstlineno 110
+         firstlineno 111
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
-         119           0 RESUME                   0
+         120           0 RESUME                   0
          
-         120           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
+         121           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
          
-         121          14 LOAD_FAST                0 (request)
+         122          14 LOAD_FAST                0 (request)
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
          
-         120         114 PRECALL                  2
+         121         114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (users)
          
-         125         130 LOAD_CONST               3 ('users')
+         126         130 LOAD_CONST               3 ('users')
                      132 LOAD_FAST                1 (users)
          
-         124         134 BUILD_MAP                1
+         125         134 BUILD_MAP                1
                      136 STORE_FAST               2 (context)
          
-         127         138 LOAD_GLOBAL             11 (NULL + render)
+         128         138 LOAD_GLOBAL             11 (NULL + render)
                      150 LOAD_FAST                0 (request)
                      152 LOAD_CONST               4 ('punkweb_bb/members.html')
                      154 LOAD_FAST                2 (context)
                      156 KW_NAMES                 5
                      158 PRECALL                  3
                      162 CALL                     3
                      172 RETURN_VALUE
@@ -1097,15 +1116,15 @@
             ('context',)
          names      ('paginate_qs', 'User', 'objects', 'select_related', 'order_by', 'render')
          varnames   ('request', 'users', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'members_view'
-         firstlineno 119
+         firstlineno 120
          lnotab 0x02010c0164ff100504ff0403
       '/login/'
       ('login_url',)
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -1119,82 +1138,82 @@
             000000000000000000000000000000a6000000ab00000000000000000001
             007411000000000000000000006403a6010000ab01000000000000000053
             007413000000000000000000007c00640464057c016901ac06a6030000ab
             03000000000000000053007403000000000000000000007c006a04000000
             00000000006a050000000000000000ac02a6010000ab0100000000000000
             007d0164057c0169017d027413000000000000000000007c0064047c02ac
             06a6030000ab0300000000000000005300
-         130           0 RESUME                   0
+         131           0 RESUME                   0
          
-         132           2 LOAD_FAST                0 (request)
+         133           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('POST')
                       16 COMPARE_OP               2 (==)
                       22 POP_JUMP_FORWARD_IF_FALSE   113 (to 250)
          
-         133          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         134          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
          
-         134          36 LOAD_FAST                0 (request)
+         135          36 LOAD_FAST                0 (request)
                       38 LOAD_ATTR                2 (POST)
                       48 LOAD_FAST                0 (request)
                       50 LOAD_ATTR                3 (FILES)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                4 (user)
                       72 LOAD_ATTR                5 (profile)
          
-         133          82 KW_NAMES                 2
+         134          82 KW_NAMES                 2
                       84 PRECALL                  3
                       88 CALL                     3
                       98 STORE_FAST               1 (form)
          
-         137         100 LOAD_FAST                1 (form)
+         138         100 LOAD_FAST                1 (form)
                      102 LOAD_METHOD              6 (is_valid)
                      124 PRECALL                  0
                      128 CALL                     0
                      138 POP_JUMP_FORWARD_IF_FALSE    35 (to 210)
          
-         138         140 LOAD_FAST                1 (form)
+         139         140 LOAD_FAST                1 (form)
                      142 LOAD_METHOD              7 (save)
                      164 PRECALL                  0
                      168 CALL                     0
                      178 POP_TOP
          
-         140         180 LOAD_GLOBAL             17 (NULL + redirect)
+         141         180 LOAD_GLOBAL             17 (NULL + redirect)
                      192 LOAD_CONST               3 ('punkweb_bb:settings')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RETURN_VALUE
          
-         142     >>  210 LOAD_GLOBAL             19 (NULL + render)
+         143     >>  210 LOAD_GLOBAL             19 (NULL + render)
                      222 LOAD_FAST                0 (request)
                      224 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      226 LOAD_CONST               5 ('form')
                      228 LOAD_FAST                1 (form)
                      230 BUILD_MAP                1
                      232 KW_NAMES                 6
                      234 PRECALL                  3
                      238 CALL                     3
                      248 RETURN_VALUE
          
-         144     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         145     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
                      262 LOAD_FAST                0 (request)
                      264 LOAD_ATTR                4 (user)
                      274 LOAD_ATTR                5 (profile)
                      284 KW_NAMES                 2
                      286 PRECALL                  1
                      290 CALL                     1
                      300 STORE_FAST               1 (form)
          
-         147         302 LOAD_CONST               5 ('form')
+         148         302 LOAD_CONST               5 ('form')
                      304 LOAD_FAST                1 (form)
          
-         146         306 BUILD_MAP                1
+         147         306 BUILD_MAP                1
                      308 STORE_FAST               2 (context)
          
-         150         310 LOAD_GLOBAL             19 (NULL + render)
+         151         310 LOAD_GLOBAL             19 (NULL + render)
                      322 LOAD_FAST                0 (request)
                      324 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      326 LOAD_FAST                2 (context)
                      328 KW_NAMES                 6
                      330 PRECALL                  3
                      334 CALL                     3
                      344 RETURN_VALUE
@@ -1208,15 +1227,15 @@
             ('context',)
          names      ('method', 'BoardProfileModelForm', 'POST', 'FILES', 'user', 'profile', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'settings_view'
-         firstlineno 130
+         firstlineno 131
          lnotab 0x020216010c012eff1204280128021e022802340304ff0404
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1231,92 +1250,92 @@
             0000007412000000000000000000007c026a0a0000000000000000a60200
             00ab0200000000000000007c025f0b00000000000000007c02a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0001007419000000000000000000007c02a6010000ab0100000000000000
             0053006e0e740900000000000000000000a6000000ab0000000000000000
             007d0164067c0169017d03741b000000000000000000007c0064077c03ac
             08a6030000ab0300000000000000005300
-         153           0 RESUME                   0
+         154           0 RESUME                   0
          
-         155           2 LOAD_FAST                0 (request)
+         156           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.add_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         156          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         157          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to create categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         158     >>   84 LOAD_FAST                0 (request)
+         159     >>   84 LOAD_FAST                0 (request)
                       86 LOAD_ATTR                3 (method)
                       96 LOAD_CONST               3 ('POST')
                       98 COMPARE_OP               2 (==)
                      104 POP_JUMP_FORWARD_IF_FALSE   129 (to 364)
          
-         159         106 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
+         160         106 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
                      118 LOAD_FAST                0 (request)
                      120 LOAD_ATTR                5 (POST)
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_FAST               1 (form)
          
-         161         146 LOAD_FAST                1 (form)
+         162         146 LOAD_FAST                1 (form)
                      148 LOAD_METHOD              6 (is_valid)
                      170 PRECALL                  0
                      174 CALL                     0
                      184 POP_JUMP_FORWARD_IF_FALSE    88 (to 362)
          
-         162         186 LOAD_FAST                1 (form)
+         163         186 LOAD_FAST                1 (form)
                      188 LOAD_METHOD              7 (save)
                      210 LOAD_CONST               4 (False)
                      212 KW_NAMES                 5
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (category)
          
-         163         230 LOAD_GLOBAL             17 (NULL + get_unique_slug)
+         164         230 LOAD_GLOBAL             17 (NULL + get_unique_slug)
                      242 LOAD_GLOBAL             18 (Category)
                      254 LOAD_FAST                2 (category)
                      256 LOAD_ATTR               10 (name)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 LOAD_FAST                2 (category)
                      282 STORE_ATTR              11 (slug)
          
-         164         292 LOAD_FAST                2 (category)
+         165         292 LOAD_FAST                2 (category)
                      294 LOAD_METHOD              7 (save)
                      316 PRECALL                  0
                      320 CALL                     0
                      330 POP_TOP
          
-         166         332 LOAD_GLOBAL             25 (NULL + redirect)
+         167         332 LOAD_GLOBAL             25 (NULL + redirect)
                      344 LOAD_FAST                2 (category)
                      346 PRECALL                  1
                      350 CALL                     1
                      360 RETURN_VALUE
          
-         161     >>  362 JUMP_FORWARD            14 (to 392)
+         162     >>  362 JUMP_FORWARD            14 (to 392)
          
-         168     >>  364 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
+         169     >>  364 LOAD_GLOBAL              9 (NULL + CategoryModelForm)
                      376 PRECALL                  0
                      380 CALL                     0
                      390 STORE_FAST               1 (form)
          
-         171     >>  392 LOAD_CONST               6 ('form')
+         172     >>  392 LOAD_CONST               6 ('form')
                      394 LOAD_FAST                1 (form)
          
-         170         396 BUILD_MAP                1
+         171         396 BUILD_MAP                1
                      398 STORE_FAST               3 (context)
          
-         173         400 LOAD_GLOBAL             27 (NULL + render)
+         174         400 LOAD_GLOBAL             27 (NULL + render)
                      412 LOAD_FAST                0 (request)
                      414 LOAD_CONST               7 ('punkweb_bb/category_create.html')
                      416 LOAD_FAST                3 (context)
                      418 KW_NAMES                 8
                      420 PRECALL                  3
                      424 CALL                     3
                      434 RETURN_VALUE
@@ -1332,15 +1351,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'method', 'CategoryModelForm', 'POST', 'is_valid', 'save', 'get_unique_slug', 'Category', 'name', 'slug', 'redirect', 'render')
          varnames   ('request', 'form', 'category', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_create_view'
-         firstlineno 153
+         firstlineno 154
          lnotab 0x020234011e021601280228012c013e0128021efb02071c0304ff0403
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1353,89 +1372,89 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac05a6010000ab0100
             000000000000007d037c027c0364069c027d047417000000000000000000
             007c0064077c04ac08a6030000ab0300000000000000005300
-         176           0 RESUME                   0
+         177           0 RESUME                   0
          
-         178           2 LOAD_FAST                0 (request)
+         179           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.change_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         179          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         180          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to change categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         181     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         182     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         183         128 LOAD_FAST                0 (request)
+         184         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         184         150 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
+         185         150 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (category)
                      176 KW_NAMES                 5
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         186         194 LOAD_FAST                3 (form)
+         187         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         187         234 LOAD_FAST                3 (form)
+         188         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (category)
          
-         189         274 LOAD_GLOBAL             21 (NULL + redirect)
+         190         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (category)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         186     >>  304 JUMP_FORWARD            16 (to 338)
+         187     >>  304 JUMP_FORWARD            16 (to 338)
          
-         191     >>  306 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
+         192     >>  306 LOAD_GLOBAL             13 (NULL + CategoryModelForm)
                      318 LOAD_FAST                2 (category)
                      320 KW_NAMES                 5
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         194     >>  338 LOAD_FAST                2 (category)
+         195     >>  338 LOAD_FAST                2 (category)
          
-         195         340 LOAD_FAST                3 (form)
+         196         340 LOAD_FAST                3 (form)
          
-         193         342 LOAD_CONST               6 (('category', 'form'))
+         194         342 LOAD_CONST               6 (('category', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         197         348 LOAD_GLOBAL             23 (NULL + render)
+         198         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               7 ('punkweb_bb/category_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 8
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -1451,15 +1470,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'CategoryModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'category_slug', 'category', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_update_view'
-         firstlineno 176
+         firstlineno 177
          lnotab 0x020234011e022c0216012c02280128021efd02052003020102fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1469,66 +1488,66 @@
             000000000000007408000000000000000000007c01ac03a6020000ab0200
             000000000000007d027c006a05000000000000000064046b020000000072
             307c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f0000000000000000000074110000000000
             00000000006405a6010000ab010000000000000000a6010000ab01000000
             0000000000530064067c0269017d037413000000000000000000007c0064
             077c03ac08a6030000ab0300000000000000005300
-         200           0 RESUME                   0
+         201           0 RESUME                   0
          
-         202           2 LOAD_FAST                0 (request)
+         203           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.delete_category')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         203          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         204          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
                       66 LOAD_CONST               2 ('You do not have permission to delete categories.')
                       68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         205     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         206     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         207         128 LOAD_FAST                0 (request)
+         208         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    48 (to 246)
          
-         208         150 LOAD_FAST                2 (category)
+         209         150 LOAD_FAST                2 (category)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         210         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         211         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_GLOBAL             17 (NULL + reverse)
                      214 LOAD_CONST               5 ('punkweb_bb:index')
                      216 PRECALL                  1
                      220 CALL                     1
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         213     >>  246 LOAD_CONST               6 ('category')
+         214     >>  246 LOAD_CONST               6 ('category')
                      248 LOAD_FAST                2 (category)
          
-         212         250 BUILD_MAP                1
+         213         250 BUILD_MAP                1
                      252 STORE_FAST               3 (context)
          
-         216         254 LOAD_GLOBAL             19 (NULL + render)
+         217         254 LOAD_GLOBAL             19 (NULL + render)
                      266 LOAD_FAST                0 (request)
                      268 LOAD_CONST               7 ('punkweb_bb/partials/category_delete.html')
                      270 LOAD_FAST                3 (context)
                      272 KW_NAMES                 8
                      274 PRECALL                  3
                      278 CALL                     3
                      288 RETURN_VALUE
@@ -1544,58 +1563,58 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'delete', 'htmx_redirect', 'reverse', 'render')
          varnames   ('request', 'category_slug', 'category', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'category_delete_view'
-         firstlineno 200
+         firstlineno 201
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
-         219           0 RESUME                   0
+         220           0 RESUME                   0
          
-         220           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         221           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         222          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         223          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (subcategory)
                       62 LOAD_ATTR                3 (threads)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (threads)
          
-         225         124 LOAD_FAST                2 (subcategory)
+         226         124 LOAD_FAST                2 (subcategory)
          
-         226         126 LOAD_FAST                3 (threads)
+         227         126 LOAD_FAST                3 (threads)
          
-         224         128 LOAD_CONST               2 (('subcategory', 'threads'))
+         225         128 LOAD_CONST               2 (('subcategory', 'threads'))
                      130 BUILD_CONST_KEY_MAP      2
                      132 STORE_FAST               4 (context)
          
-         228         134 LOAD_GLOBAL             11 (NULL + render)
+         229         134 LOAD_GLOBAL             11 (NULL + render)
                      146 LOAD_FAST                0 (request)
                      148 LOAD_CONST               3 ('punkweb_bb/subcategory.html')
                      150 LOAD_FAST                4 (context)
                      152 KW_NAMES                 4
                      154 PRECALL                  3
                      158 CALL                     3
                      168 RETURN_VALUE
@@ -1607,15 +1626,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'paginate_qs', 'threads', 'all', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_view'
-         firstlineno 219
+         firstlineno 220
          lnotab 0x02012c024e03020102fe0604
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1632,108 +1651,108 @@
             007418000000000000000000007c046a0d0000000000000000a6020000ab
             0200000000000000007c045f0e00000000000000007c04a0090000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00741f000000000000000000007c04a6010000ab01000000000000000053
             006e0e740d00000000000000000000a6000000ab0000000000000000007d
             037c027c0364079c027d057421000000000000000000007c0064087c05ac
             09a6030000ab0300000000000000005300
-         231           0 RESUME                   0
+         232           0 RESUME                   0
          
-         233           2 LOAD_FAST                0 (request)
+         234           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.add_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         234          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         235          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         235          66 LOAD_CONST               2 ('You do not have permission to create subcategories.')
+         236          66 LOAD_CONST               2 ('You do not have permission to create subcategories.')
          
-         234          68 PRECALL                  1
+         235          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         238     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         239     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Category)
                      108 LOAD_FAST                1 (category_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (category)
          
-         240         128 LOAD_FAST                0 (request)
+         241         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE   136 (to 422)
          
-         241         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         242         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 STORE_FAST               3 (form)
          
-         243         190 LOAD_FAST                3 (form)
+         244         190 LOAD_FAST                3 (form)
                      192 LOAD_METHOD              8 (is_valid)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 POP_JUMP_FORWARD_IF_FALSE    95 (to 420)
          
-         244         230 LOAD_FAST                3 (form)
+         245         230 LOAD_FAST                3 (form)
                      232 LOAD_METHOD              9 (save)
                      254 LOAD_CONST               5 (False)
                      256 KW_NAMES                 6
                      258 PRECALL                  1
                      262 CALL                     1
                      272 STORE_FAST               4 (subcategory)
          
-         245         274 LOAD_FAST                2 (category)
+         246         274 LOAD_FAST                2 (category)
                      276 LOAD_FAST                4 (subcategory)
                      278 STORE_ATTR              10 (category)
          
-         246         288 LOAD_GLOBAL             23 (NULL + get_unique_slug)
+         247         288 LOAD_GLOBAL             23 (NULL + get_unique_slug)
                      300 LOAD_GLOBAL             24 (Subcategory)
                      312 LOAD_FAST                4 (subcategory)
                      314 LOAD_ATTR               13 (name)
                      324 PRECALL                  2
                      328 CALL                     2
                      338 LOAD_FAST                4 (subcategory)
                      340 STORE_ATTR              14 (slug)
          
-         247         350 LOAD_FAST                4 (subcategory)
+         248         350 LOAD_FAST                4 (subcategory)
                      352 LOAD_METHOD              9 (save)
                      374 PRECALL                  0
                      378 CALL                     0
                      388 POP_TOP
          
-         249         390 LOAD_GLOBAL             31 (NULL + redirect)
+         250         390 LOAD_GLOBAL             31 (NULL + redirect)
                      402 LOAD_FAST                4 (subcategory)
                      404 PRECALL                  1
                      408 CALL                     1
                      418 RETURN_VALUE
          
-         243     >>  420 JUMP_FORWARD            14 (to 450)
+         244     >>  420 JUMP_FORWARD            14 (to 450)
          
-         251     >>  422 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         252     >>  422 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      434 PRECALL                  0
                      438 CALL                     0
                      448 STORE_FAST               3 (form)
          
-         254     >>  450 LOAD_FAST                2 (category)
+         255     >>  450 LOAD_FAST                2 (category)
          
-         255         452 LOAD_FAST                3 (form)
+         256         452 LOAD_FAST                3 (form)
          
-         253         454 LOAD_CONST               7 (('category', 'form'))
+         254         454 LOAD_CONST               7 (('category', 'form'))
                      456 BUILD_CONST_KEY_MAP      2
                      458 STORE_FAST               5 (context)
          
-         257         460 LOAD_GLOBAL             33 (NULL + render)
+         258         460 LOAD_GLOBAL             33 (NULL + render)
                      472 LOAD_FAST                0 (request)
                      474 LOAD_CONST               8 ('punkweb_bb/subcategory_create.html')
                      476 LOAD_FAST                5 (context)
                      478 KW_NAMES                 9
                      480 PRECALL                  3
                      484 CALL                     3
                      494 RETURN_VALUE
@@ -1750,15 +1769,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Category', 'method', 'SubcategoryModelForm', 'POST', 'is_valid', 'save', 'category', 'get_unique_slug', 'Subcategory', 'name', 'slug', 'redirect', 'render')
          varnames   ('request', 'category_slug', 'category', 'form', 'subcategory', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_create_view'
-         firstlineno 231
+         firstlineno 232
          lnotab
             0x020234010c0102ff10042c021601280228012c010e013e0128021efa02
             081c03020102fe0604
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
@@ -1773,91 +1792,91 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac05a6010000ab0100
             000000000000007d037c027c0364069c027d047417000000000000000000
             007c0064077c04ac08a6030000ab0300000000000000005300
-         260           0 RESUME                   0
+         261           0 RESUME                   0
          
-         262           2 LOAD_FAST                0 (request)
+         263           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.change_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         263          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         264          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         264          66 LOAD_CONST               2 ('You do not have permission to change subcategories.')
+         265          66 LOAD_CONST               2 ('You do not have permission to change subcategories.')
          
-         263          68 PRECALL                  1
+         264          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         267     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         268     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Subcategory)
                      108 LOAD_FAST                1 (subcategory_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (subcategory)
          
-         269         128 LOAD_FAST                0 (request)
+         270         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         270         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         271         150 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (subcategory)
                      176 KW_NAMES                 5
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         272         194 LOAD_FAST                3 (form)
+         273         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         273         234 LOAD_FAST                3 (form)
+         274         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (subcategory)
          
-         275         274 LOAD_GLOBAL             21 (NULL + redirect)
+         276         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (subcategory)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         272     >>  304 JUMP_FORWARD            16 (to 338)
+         273     >>  304 JUMP_FORWARD            16 (to 338)
          
-         277     >>  306 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
+         278     >>  306 LOAD_GLOBAL             13 (NULL + SubcategoryModelForm)
                      318 LOAD_FAST                2 (subcategory)
                      320 KW_NAMES                 5
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         280     >>  338 LOAD_FAST                2 (subcategory)
+         281     >>  338 LOAD_FAST                2 (subcategory)
          
-         281         340 LOAD_FAST                3 (form)
+         282         340 LOAD_FAST                3 (form)
          
-         279         342 LOAD_CONST               6 (('subcategory', 'form'))
+         280         342 LOAD_CONST               6 (('subcategory', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         283         348 LOAD_GLOBAL             23 (NULL + render)
+         284         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               7 ('punkweb_bb/subcategory_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 8
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -1873,15 +1892,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Subcategory', 'method', 'SubcategoryModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_update_view'
-         firstlineno 260
+         firstlineno 261
          lnotab
             0x020234010c0102ff10042c0216012c02280128021efd02052003020102
             fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -1894,75 +1913,75 @@
             000000000000007d027c006a05000000000000000064046b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064057c
             0269017d037415000000000000000000007c0064067c03ac07a6030000ab
             0300000000000000005300
-         286           0 RESUME                   0
+         287           0 RESUME                   0
          
-         288           2 LOAD_FAST                0 (request)
+         289           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_METHOD              1 (has_perm)
                       36 LOAD_CONST               1 ('punkweb_bb.delete_subcategory')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         289          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+         290          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
          
-         290          66 LOAD_CONST               2 ('You do not have permission to delete subcategories.')
+         291          66 LOAD_CONST               2 ('You do not have permission to delete subcategories.')
          
-         289          68 PRECALL                  1
+         290          68 PRECALL                  1
                       72 CALL                     1
                       82 RETURN_VALUE
          
-         293     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+         294     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
                       96 LOAD_GLOBAL              8 (Subcategory)
                      108 LOAD_FAST                1 (subcategory_slug)
                      110 KW_NAMES                 3
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               2 (subcategory)
          
-         295         128 LOAD_FAST                0 (request)
+         296         128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               4 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         296         150 LOAD_FAST                2 (subcategory)
+         297         150 LOAD_FAST                2 (subcategory)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         298         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         299         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (subcategory)
                      204 LOAD_ATTR                8 (category)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         301     >>  266 LOAD_CONST               5 ('subcategory')
+         302     >>  266 LOAD_CONST               5 ('subcategory')
                      268 LOAD_FAST                2 (subcategory)
          
-         300         270 BUILD_MAP                1
+         301         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         304         274 LOAD_GLOBAL             21 (NULL + render)
+         305         274 LOAD_GLOBAL             21 (NULL + render)
          
-         305         286 LOAD_FAST                0 (request)
+         306         286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               6 ('punkweb_bb/partials/subcategory_delete.html')
                      290 LOAD_FAST                3 (context)
          
-         304         292 KW_NAMES                 7
+         305         292 KW_NAMES                 7
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
          consts
             None
             'punkweb_bb.delete_subcategory'
             'You do not have permission to delete subcategories.'
@@ -1973,15 +1992,15 @@
             ('context',)
          names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Subcategory', 'method', 'delete', 'htmx_redirect', 'category', 'get_absolute_url', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_delete_view'
-         firstlineno 286
+         firstlineno 287
          lnotab 0x020234010c0102ff10042c02160128024c0304ff04040c0106ff
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1997,104 +2016,104 @@
             0000007d047c027c045f0a00000000000000007c006a0300000000000000
             007c045f0300000000000000007c04a00900000000000000000000000000
             00000000000000a6000000ab000000000000000000010074170000000000
             00000000007c04a6010000ab01000000000000000053006e0e740d000000
             00000000000000a6000000ab0000000000000000007d037c027c0364069c
             027d057419000000000000000000007c0064077c05ac08a6030000ab0300
             000000000000005300
-         309           0 RESUME                   0
+         310           0 RESUME                   0
          
-         311           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         312           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         313          46 LOAD_FAST                2 (subcategory)
+         314          46 LOAD_FAST                2 (subcategory)
                       48 LOAD_METHOD              2 (can_post)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         314          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         315          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         315         110 LOAD_CONST               2 ('You do not have permission to post in this subcategory.')
+         316         110 LOAD_CONST               2 ('You do not have permission to post in this subcategory.')
          
-         314         112 PRECALL                  1
+         315         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         318     >>  128 LOAD_FAST                0 (request)
+         319     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE   117 (to 384)
          
-         319         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         320         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 STORE_FAST               3 (form)
          
-         321         190 LOAD_FAST                3 (form)
+         322         190 LOAD_FAST                3 (form)
                      192 LOAD_METHOD              8 (is_valid)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 POP_JUMP_FORWARD_IF_FALSE    76 (to 382)
          
-         322         230 LOAD_FAST                3 (form)
+         323         230 LOAD_FAST                3 (form)
                      232 LOAD_METHOD              9 (save)
                      254 LOAD_CONST               4 (False)
                      256 KW_NAMES                 5
                      258 PRECALL                  1
                      262 CALL                     1
                      272 STORE_FAST               4 (thread)
          
-         323         274 LOAD_FAST                2 (subcategory)
+         324         274 LOAD_FAST                2 (subcategory)
                      276 LOAD_FAST                4 (thread)
                      278 STORE_ATTR              10 (subcategory)
          
-         324         288 LOAD_FAST                0 (request)
+         325         288 LOAD_FAST                0 (request)
                      290 LOAD_ATTR                3 (user)
                      300 LOAD_FAST                4 (thread)
                      302 STORE_ATTR               3 (user)
          
-         325         312 LOAD_FAST                4 (thread)
+         326         312 LOAD_FAST                4 (thread)
                      314 LOAD_METHOD              9 (save)
                      336 PRECALL                  0
                      340 CALL                     0
                      350 POP_TOP
          
-         327         352 LOAD_GLOBAL             23 (NULL + redirect)
+         328         352 LOAD_GLOBAL             23 (NULL + redirect)
                      364 LOAD_FAST                4 (thread)
                      366 PRECALL                  1
                      370 CALL                     1
                      380 RETURN_VALUE
          
-         321     >>  382 JUMP_FORWARD            14 (to 412)
+         322     >>  382 JUMP_FORWARD            14 (to 412)
          
-         329     >>  384 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         330     >>  384 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      396 PRECALL                  0
                      400 CALL                     0
                      410 STORE_FAST               3 (form)
          
-         332     >>  412 LOAD_FAST                2 (subcategory)
+         333     >>  412 LOAD_FAST                2 (subcategory)
          
-         333         414 LOAD_FAST                3 (form)
+         334         414 LOAD_FAST                3 (form)
          
-         331         416 LOAD_CONST               6 (('subcategory', 'form'))
+         332         416 LOAD_CONST               6 (('subcategory', 'form'))
                      418 BUILD_CONST_KEY_MAP      2
                      420 STORE_FAST               5 (context)
          
-         335         422 LOAD_GLOBAL             25 (NULL + render)
+         336         422 LOAD_GLOBAL             25 (NULL + render)
                      434 LOAD_FAST                0 (request)
                      436 LOAD_CONST               7 ('punkweb_bb/thread_create.html')
                      438 LOAD_FAST                5 (context)
                      440 KW_NAMES                 8
                      442 PRECALL                  3
                      446 CALL                     3
                      456 RETURN_VALUE
@@ -2110,15 +2129,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'can_post', 'user', 'HttpResponseForbidden', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'subcategory', 'redirect', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_create_view'
-         firstlineno 309
+         firstlineno 310
          lnotab
             0x02022c0234010c0102ff10041601280228012c010e01180128021efa02
             081c03020102fe0604
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 5
@@ -2133,88 +2152,88 @@
             0000000000000064026700a6020000ab0200000000000000007d057c017c
             05760172327c0278016a08000000000000000064037a0d000063025f0800
             000000000000007c02a00900000000000000000000000000000000000000
             00a6000000ab00000000000000000001007c057c0167017a0000007c006a
             06000000000000000064023c0000007c027c037c0464049c037d06741500
             0000000000000000007c0064057c06ac06a6030000ab0300000000000000
             005300
-         338           0 RESUME                   0
+         339           0 RESUME                   0
          
-         339           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         340           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         341          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         342          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (thread)
                       62 LOAD_ATTR                3 (posts)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (posts)
          
-         343         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         344         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 STORE_FAST               4 (post_form)
          
-         346         152 LOAD_FAST                0 (request)
+         347         152 LOAD_FAST                0 (request)
                      154 LOAD_ATTR                6 (session)
                      164 LOAD_METHOD              7 (get)
                      186 LOAD_CONST               2 ('viewed_threads')
                      188 BUILD_LIST               0
                      190 PRECALL                  2
                      194 CALL                     2
                      204 STORE_FAST               5 (viewed_threads)
          
-         347         206 LOAD_FAST                1 (thread_id)
+         348         206 LOAD_FAST                1 (thread_id)
                      208 LOAD_FAST                5 (viewed_threads)
                      210 CONTAINS_OP              1
                      212 POP_JUMP_FORWARD_IF_FALSE    50 (to 314)
          
-         348         214 LOAD_FAST                2 (thread)
+         349         214 LOAD_FAST                2 (thread)
                      216 COPY                     1
                      218 LOAD_ATTR                8 (view_count)
                      228 LOAD_CONST               3 (1)
                      230 BINARY_OP               13 (+=)
                      234 SWAP                     2
                      236 STORE_ATTR               8 (view_count)
          
-         349         246 LOAD_FAST                2 (thread)
+         350         246 LOAD_FAST                2 (thread)
                      248 LOAD_METHOD              9 (save)
                      270 PRECALL                  0
                      274 CALL                     0
                      284 POP_TOP
          
-         350         286 LOAD_FAST                5 (viewed_threads)
+         351         286 LOAD_FAST                5 (viewed_threads)
                      288 LOAD_FAST                1 (thread_id)
                      290 BUILD_LIST               1
                      292 BINARY_OP                0 (+)
                      296 LOAD_FAST                0 (request)
                      298 LOAD_ATTR                6 (session)
                      308 LOAD_CONST               2 ('viewed_threads')
                      310 STORE_SUBSCR
          
-         353     >>  314 LOAD_FAST                2 (thread)
+         354     >>  314 LOAD_FAST                2 (thread)
          
-         354         316 LOAD_FAST                3 (posts)
+         355         316 LOAD_FAST                3 (posts)
          
-         355         318 LOAD_FAST                4 (post_form)
+         356         318 LOAD_FAST                4 (post_form)
          
-         352         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
+         353         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
                      322 BUILD_CONST_KEY_MAP      3
                      324 STORE_FAST               6 (context)
          
-         357         326 LOAD_GLOBAL             21 (NULL + render)
+         358         326 LOAD_GLOBAL             21 (NULL + render)
                      338 LOAD_FAST                0 (request)
                      340 LOAD_CONST               5 ('punkweb_bb/thread.html')
                      342 LOAD_FAST                6 (context)
                      344 KW_NAMES                 6
                      346 PRECALL                  3
                      350 CALL                     3
                      360 RETURN_VALUE
@@ -2228,15 +2247,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'paginate_qs', 'posts', 'all', 'PostModelForm', 'session', 'get', 'view_count', 'save', 'render')
          varnames   ('request', 'thread_id', 'thread', 'posts', 'post_form', 'viewed_threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_view'
-         firstlineno 338
+         firstlineno 339
          lnotab 0x02012c024e021c0336010801200128011c030201020102fd0605
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2249,91 +2268,91 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             00000053006e10740d000000000000000000007c02ac04a6010000ab0100
             000000000000007d037c027c0364059c027d047417000000000000000000
             007c0064067c04ac07a6030000ab0300000000000000005300
-         360           0 RESUME                   0
+         361           0 RESUME                   0
          
-         362           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         363           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         364          46 LOAD_FAST                2 (thread)
+         365          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_edit)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         365          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         366          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         366         110 LOAD_CONST               2 ('You do not have permission to change this thread.')
+         367         110 LOAD_CONST               2 ('You do not have permission to change this thread.')
          
-         365         112 PRECALL                  1
+         366         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         369     >>  128 LOAD_FAST                0 (request)
+         370     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    78 (to 306)
          
-         370         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         371         150 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (thread)
                      176 KW_NAMES                 4
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         372         194 LOAD_FAST                3 (form)
+         373         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         373         234 LOAD_FAST                3 (form)
+         374         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (thread)
          
-         375         274 LOAD_GLOBAL             21 (NULL + redirect)
+         376         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (thread)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         372     >>  304 JUMP_FORWARD            16 (to 338)
+         373     >>  304 JUMP_FORWARD            16 (to 338)
          
-         377     >>  306 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
+         378     >>  306 LOAD_GLOBAL             13 (NULL + ThreadModelForm)
                      318 LOAD_FAST                2 (thread)
                      320 KW_NAMES                 4
                      322 PRECALL                  1
                      326 CALL                     1
                      336 STORE_FAST               3 (form)
          
-         380     >>  338 LOAD_FAST                2 (thread)
+         381     >>  338 LOAD_FAST                2 (thread)
          
-         381         340 LOAD_FAST                3 (form)
+         382         340 LOAD_FAST                3 (form)
          
-         379         342 LOAD_CONST               5 (('thread', 'form'))
+         380         342 LOAD_CONST               5 (('thread', 'form'))
                      344 BUILD_CONST_KEY_MAP      2
                      346 STORE_FAST               4 (context)
          
-         383         348 LOAD_GLOBAL             23 (NULL + render)
+         384         348 LOAD_GLOBAL             23 (NULL + render)
                      360 LOAD_FAST                0 (request)
                      362 LOAD_CONST               6 ('punkweb_bb/thread_update.html')
                      364 LOAD_FAST                4 (context)
                      366 KW_NAMES                 7
                      368 PRECALL                  3
                      372 CALL                     3
                      382 RETURN_VALUE
@@ -2348,15 +2367,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'can_edit', 'user', 'HttpResponseForbidden', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'thread_id', 'thread', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_update_view'
-         firstlineno 360
+         firstlineno 361
          lnotab
             0x02022c0234010c0102ff100416012c02280128021efd02052003020102
             fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -2369,69 +2388,69 @@
             0000000000000053007c006a05000000000000000064036b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064047c
             0269017d037415000000000000000000007c0064057c03ac06a6030000ab
             0300000000000000005300
-         386           0 RESUME                   0
+         387           0 RESUME                   0
          
-         388           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         389           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         390          46 LOAD_FAST                2 (thread)
+         391          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         391          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         392          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         392         110 LOAD_CONST               2 ('You do not have permission to delete this thread.')
+         393         110 LOAD_CONST               2 ('You do not have permission to delete this thread.')
          
-         391         112 PRECALL                  1
+         392         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         395     >>  128 LOAD_FAST                0 (request)
+         396     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         396         150 LOAD_FAST                2 (thread)
+         397         150 LOAD_FAST                2 (thread)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         398         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         399         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (thread)
                      204 LOAD_ATTR                8 (subcategory)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         401     >>  266 LOAD_CONST               4 ('thread')
+         402     >>  266 LOAD_CONST               4 ('thread')
                      268 LOAD_FAST                2 (thread)
          
-         400         270 BUILD_MAP                1
+         401         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         404         274 LOAD_GLOBAL             21 (NULL + render)
+         405         274 LOAD_GLOBAL             21 (NULL + render)
                      286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               5 ('punkweb_bb/partials/thread_delete.html')
                      290 LOAD_FAST                3 (context)
                      292 KW_NAMES                 6
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
@@ -2445,160 +2464,294 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'subcategory', 'get_absolute_url', 'render')
          varnames   ('request', 'thread_id', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_delete_view'
-         firstlineno 386
+         firstlineno 387
          lnotab 0x02022c0234010c0102ff1004160128024c0304ff0404
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
-            0x97007401000000000000000000007402000000000000000000007c01ac
-            01a6020000ab0200000000000000007d027c006a020000000000000000a0
-            0300000000000000000000000000000000000000006402a6010000ab0100
-            00000000000000730f7409000000000000000000006403a6010000ab0100
-            0000000000000053007c026a0500000000000000000c007c025f05000000
+            0x97007c006a000000000000000000a00100000000000000000000000000
+            000000000000006401a6010000ab010000000000000000730f7405000000
+            000000000000006402a6010000ab01000000000000000053007407000000
+            000000000000007408000000000000000000007c01ac03a6020000ab0200
+            000000000000007d027c026a0500000000000000000c007c025f05000000
             00000000007c02a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000000100740f000000000000000000007c02a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6010000ab0100000000000000005300
-         407           0 RESUME                   0
+         408           0 RESUME                   0
          
-         409           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
-                      14 LOAD_GLOBAL              2 (Thread)
-                      26 LOAD_FAST                1 (thread_id)
-                      28 KW_NAMES                 1
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 STORE_FAST               2 (thread)
+         410           2 LOAD_FAST                0 (request)
+                       4 LOAD_ATTR                0 (user)
+                      14 LOAD_METHOD              1 (has_perm)
+                      36 LOAD_CONST               1 ('punkweb_bb.pin_thread')
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         411          46 LOAD_FAST                0 (request)
-                      48 LOAD_ATTR                2 (user)
-                      58 LOAD_METHOD              3 (has_perm)
-                      80 LOAD_CONST               2 ('punkweb_bb.pin_thread')
-                      82 PRECALL                  1
-                      86 CALL                     1
-                      96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
+         411          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+                      66 LOAD_CONST               2 ('You do not have permission to pin threads.')
+                      68 PRECALL                  1
+                      72 CALL                     1
+                      82 RETURN_VALUE
          
-         412          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
-                     110 LOAD_CONST               3 ('You do not have permission to pin threads.')
-                     112 PRECALL                  1
-                     116 CALL                     1
-                     126 RETURN_VALUE
+         413     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+                      96 LOAD_GLOBAL              8 (Thread)
+                     108 LOAD_FAST                1 (thread_id)
+                     110 KW_NAMES                 3
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 STORE_FAST               2 (thread)
          
-         414     >>  128 LOAD_FAST                2 (thread)
+         415         128 LOAD_FAST                2 (thread)
                      130 LOAD_ATTR                5 (is_pinned)
                      140 UNARY_NOT
                      142 LOAD_FAST                2 (thread)
                      144 STORE_ATTR               5 (is_pinned)
          
-         415         154 LOAD_FAST                2 (thread)
+         416         154 LOAD_FAST                2 (thread)
                      156 LOAD_METHOD              6 (save)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-         417         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         418         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      206 LOAD_FAST                2 (thread)
                      208 LOAD_METHOD              8 (get_absolute_url)
                      230 PRECALL                  0
                      234 CALL                     0
                      244 PRECALL                  1
                      248 CALL                     1
                      258 RETURN_VALUE
          consts
             None
-            ('pk',)
             'punkweb_bb.pin_thread'
             'You do not have permission to pin threads.'
-         names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_pinned', 'save', 'htmx_redirect', 'get_absolute_url')
+            ('pk',)
+         names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Thread', 'is_pinned', 'save', 'htmx_redirect', 'get_absolute_url')
          varnames   ('request', 'thread_id', 'thread')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_pin_view'
-         firstlineno 407
-         lnotab 0x02022c0234011e021a012802
+         firstlineno 408
+         lnotab 0x020234011e022c021a012802
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
-            0x97007401000000000000000000007402000000000000000000007c01ac
-            01a6020000ab0200000000000000007d027c006a020000000000000000a0
-            0300000000000000000000000000000000000000006402a6010000ab0100
-            00000000000000730f7409000000000000000000006403a6010000ab0100
-            0000000000000053007c026a0500000000000000000c007c025f05000000
+            0x97007c006a000000000000000000a00100000000000000000000000000
+            000000000000006401a6010000ab010000000000000000730f7405000000
+            000000000000006402a6010000ab01000000000000000053007407000000
+            000000000000007408000000000000000000007c01ac03a6020000ab0200
+            000000000000007d027c026a0500000000000000000c007c025f05000000
             00000000007c02a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000000100740f000000000000000000007c02a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6010000ab0100000000000000005300
-         420           0 RESUME                   0
+         421           0 RESUME                   0
          
-         422           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
-                      14 LOAD_GLOBAL              2 (Thread)
-                      26 LOAD_FAST                1 (thread_id)
-                      28 KW_NAMES                 1
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 STORE_FAST               2 (thread)
+         423           2 LOAD_FAST                0 (request)
+                       4 LOAD_ATTR                0 (user)
+                      14 LOAD_METHOD              1 (has_perm)
+                      36 LOAD_CONST               1 ('punkweb_bb.close_thread')
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
          
-         424          46 LOAD_FAST                0 (request)
-                      48 LOAD_ATTR                2 (user)
-                      58 LOAD_METHOD              3 (has_perm)
-                      80 LOAD_CONST               2 ('punkweb_bb.close_thread')
-                      82 PRECALL                  1
-                      86 CALL                     1
-                      96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
+         424          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+                      66 LOAD_CONST               2 ('You do not have permission to close threads.')
+                      68 PRECALL                  1
+                      72 CALL                     1
+                      82 RETURN_VALUE
          
-         425          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
-                     110 LOAD_CONST               3 ('You do not have permission to close threads.')
-                     112 PRECALL                  1
-                     116 CALL                     1
-                     126 RETURN_VALUE
+         426     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+                      96 LOAD_GLOBAL              8 (Thread)
+                     108 LOAD_FAST                1 (thread_id)
+                     110 KW_NAMES                 3
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 STORE_FAST               2 (thread)
          
-         427     >>  128 LOAD_FAST                2 (thread)
+         428         128 LOAD_FAST                2 (thread)
                      130 LOAD_ATTR                5 (is_closed)
                      140 UNARY_NOT
                      142 LOAD_FAST                2 (thread)
                      144 STORE_ATTR               5 (is_closed)
          
-         428         154 LOAD_FAST                2 (thread)
+         429         154 LOAD_FAST                2 (thread)
                      156 LOAD_METHOD              6 (save)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-         430         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         431         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      206 LOAD_FAST                2 (thread)
                      208 LOAD_METHOD              8 (get_absolute_url)
                      230 PRECALL                  0
                      234 CALL                     0
                      244 PRECALL                  1
                      248 CALL                     1
                      258 RETURN_VALUE
          consts
             None
-            ('pk',)
             'punkweb_bb.close_thread'
             'You do not have permission to close threads.'
-         names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_closed', 'save', 'htmx_redirect', 'get_absolute_url')
+            ('pk',)
+         names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Thread', 'is_closed', 'save', 'htmx_redirect', 'get_absolute_url')
          varnames   ('request', 'thread_id', 'thread')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_close_view'
-         firstlineno 420
-         lnotab 0x02022c0234011e021a012802
+         firstlineno 421
+         lnotab 0x020234011e022c021a012802
+      code
+         argcount  : 2
+         nlocals   : 6
+         stacksize : 5
+         flags     : 3
+         code
+            0x97007c006a000000000000000000a00100000000000000000000000000
+            000000000000006401a6010000ab010000000000000000730f7405000000
+            000000000000006402a6010000ab01000000000000000053007407000000
+            000000000000007408000000000000000000007c01ac03a6020000ab0200
+            000000000000007d027c006a05000000000000000064046b020000000072
+            5d740d000000000000000000007c006a070000000000000000a6010000ab
+            0100000000000000007d037c03a008000000000000000000000000000000
+            0000000000a6000000ab00000000000000000072357c036a090000000000
+            0000006405190000000000000000007c025f0a00000000000000007c02a0
+            0b0000000000000000000000000000000000000000a6000000ab00000000
+            000000000001007419000000000000000000007c02a6010000ab01000000
+            0000000000530064057c026a0a000000000000000069017d04740d000000
+            000000000000007c04ac06a6010000ab0100000000000000007d037c027c
+            0364079c027d05741b000000000000000000007c0064087c05ac09a60300
+            00ab0300000000000000005300
+         434           0 RESUME                   0
+         
+         436           2 LOAD_FAST                0 (request)
+                       4 LOAD_ATTR                0 (user)
+                      14 LOAD_METHOD              1 (has_perm)
+                      36 LOAD_CONST               1 ('punkweb_bb.move_thread')
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 POP_JUMP_FORWARD_IF_TRUE    15 (to 84)
+         
+         437          54 LOAD_GLOBAL              5 (NULL + HttpResponseForbidden)
+                      66 LOAD_CONST               2 ('You do not have permission to move threads.')
+                      68 PRECALL                  1
+                      72 CALL                     1
+                      82 RETURN_VALUE
+         
+         439     >>   84 LOAD_GLOBAL              7 (NULL + get_object_or_404)
+                      96 LOAD_GLOBAL              8 (Thread)
+                     108 LOAD_FAST                1 (thread_id)
+                     110 KW_NAMES                 3
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 STORE_FAST               2 (thread)
+         
+         441         128 LOAD_FAST                0 (request)
+                     130 LOAD_ATTR                5 (method)
+                     140 LOAD_CONST               4 ('POST')
+                     142 COMPARE_OP               2 (==)
+                     148 POP_JUMP_FORWARD_IF_FALSE    93 (to 336)
+         
+         442         150 LOAD_GLOBAL             13 (NULL + ThreadMoveForm)
+                     162 LOAD_FAST                0 (request)
+                     164 LOAD_ATTR                7 (POST)
+                     174 PRECALL                  1
+                     178 CALL                     1
+                     188 STORE_FAST               3 (form)
+         
+         444         190 LOAD_FAST                3 (form)
+                     192 LOAD_METHOD              8 (is_valid)
+                     214 PRECALL                  0
+                     218 CALL                     0
+                     228 POP_JUMP_FORWARD_IF_FALSE    53 (to 336)
+         
+         445         230 LOAD_FAST                3 (form)
+                     232 LOAD_ATTR                9 (cleaned_data)
+                     242 LOAD_CONST               5 ('subcategory')
+                     244 BINARY_SUBSCR
+                     254 LOAD_FAST                2 (thread)
+                     256 STORE_ATTR              10 (subcategory)
+         
+         446         266 LOAD_FAST                2 (thread)
+                     268 LOAD_METHOD             11 (save)
+                     290 PRECALL                  0
+                     294 CALL                     0
+                     304 POP_TOP
+         
+         448         306 LOAD_GLOBAL             25 (NULL + redirect)
+                     318 LOAD_FAST                2 (thread)
+                     320 PRECALL                  1
+                     324 CALL                     1
+                     334 RETURN_VALUE
+         
+         451     >>  336 LOAD_CONST               5 ('subcategory')
+                     338 LOAD_FAST                2 (thread)
+                     340 LOAD_ATTR               10 (subcategory)
+         
+         450         350 BUILD_MAP                1
+                     352 STORE_FAST               4 (initial_data)
+         
+         454         354 LOAD_GLOBAL             13 (NULL + ThreadMoveForm)
+                     366 LOAD_FAST                4 (initial_data)
+                     368 KW_NAMES                 6
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 STORE_FAST               3 (form)
+         
+         457         386 LOAD_FAST                2 (thread)
+         
+         458         388 LOAD_FAST                3 (form)
+         
+         456         390 LOAD_CONST               7 (('thread', 'form'))
+                     392 BUILD_CONST_KEY_MAP      2
+                     394 STORE_FAST               5 (context)
+         
+         461         396 LOAD_GLOBAL             27 (NULL + render)
+                     408 LOAD_FAST                0 (request)
+                     410 LOAD_CONST               8 ('punkweb_bb/partials/thread_move.html')
+                     412 LOAD_FAST                5 (context)
+                     414 KW_NAMES                 9
+                     416 PRECALL                  3
+                     420 CALL                     3
+                     430 RETURN_VALUE
+         consts
+            None
+            'punkweb_bb.move_thread'
+            'You do not have permission to move threads.'
+            ('pk',)
+            'POST'
+            'subcategory'
+            ('data',)
+            ('thread', 'form')
+            'punkweb_bb/partials/thread_move.html'
+            ('context',)
+         names      ('user', 'has_perm', 'HttpResponseForbidden', 'get_object_or_404', 'Thread', 'method', 'ThreadMoveForm', 'POST', 'is_valid', 'cleaned_data', 'subcategory', 'save', 'redirect', 'render')
+         varnames   ('request', 'thread_id', 'thread', 'form', 'initial_data', 'context')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
+         name       'thread_move_view'
+         firstlineno 434
+         lnotab
+            0x020234011e022c02160128022801240128021e030eff04042003020102
+            fe0605
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
@@ -2610,97 +2763,97 @@
             00000000000000000000000000a6000000ab000000000000000000724c7c
             03a00800000000000000000000000000000000000000006403ac04a60100
             00ab0100000000000000007d047c027c045f0900000000000000007c006a
             0300000000000000007c045f0300000000000000007c04a0080000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             007415000000000000000000007c04a6010000ab01000000000000000053
             0064005300
-         433           0 RESUME                   0
+         464           0 RESUME                   0
          
-         435           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         466           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         437          46 LOAD_FAST                2 (thread)
+         468          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_post)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         438          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         469          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         439         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
+         470         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
          
-         438         112 PRECALL                  1
+         469         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         442     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         473     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      140 LOAD_FAST                0 (request)
                      142 LOAD_ATTR                6 (POST)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               3 (form)
          
-         444         168 LOAD_FAST                3 (form)
+         475         168 LOAD_FAST                3 (form)
                      170 LOAD_METHOD              7 (is_valid)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 POP_JUMP_FORWARD_IF_FALSE    76 (to 360)
          
-         445         208 LOAD_FAST                3 (form)
+         476         208 LOAD_FAST                3 (form)
                      210 LOAD_METHOD              8 (save)
                      232 LOAD_CONST               3 (False)
                      234 KW_NAMES                 4
                      236 PRECALL                  1
                      240 CALL                     1
                      250 STORE_FAST               4 (post)
          
-         446         252 LOAD_FAST                2 (thread)
+         477         252 LOAD_FAST                2 (thread)
                      254 LOAD_FAST                4 (post)
                      256 STORE_ATTR               9 (thread)
          
-         447         266 LOAD_FAST                0 (request)
+         478         266 LOAD_FAST                0 (request)
                      268 LOAD_ATTR                3 (user)
                      278 LOAD_FAST                4 (post)
                      280 STORE_ATTR               3 (user)
          
-         448         290 LOAD_FAST                4 (post)
+         479         290 LOAD_FAST                4 (post)
                      292 LOAD_METHOD              8 (save)
                      314 PRECALL                  0
                      318 CALL                     0
                      328 POP_TOP
          
-         450         330 LOAD_GLOBAL             21 (NULL + redirect)
+         481         330 LOAD_GLOBAL             21 (NULL + redirect)
                      342 LOAD_FAST                4 (post)
                      344 PRECALL                  1
                      348 CALL                     1
                      358 RETURN_VALUE
          
-         444     >>  360 LOAD_CONST               0 (None)
+         475     >>  360 LOAD_CONST               0 (None)
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
-         firstlineno 433
+         firstlineno 464
          lnotab 0x02022c0234010c0102ff1004280228012c010e01180128021efa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2713,87 +2866,87 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             0000005300740d000000000000000000007c02ac04a6010000ab01000000
             00000000007d037c027c0364059c027d047417000000000000000000007c
             0064067c04ac07a6030000ab0300000000000000005300
-         453           0 RESUME                   0
+         484           0 RESUME                   0
          
-         455           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         486           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         457          46 LOAD_FAST                2 (post)
+         488          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_edit)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         458          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         489          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to change this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         460     >>  128 LOAD_FAST                0 (request)
+         491     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    77 (to 304)
          
-         461         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         492         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (post)
                      176 KW_NAMES                 4
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         463         194 LOAD_FAST                3 (form)
+         494         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         464         234 LOAD_FAST                3 (form)
+         495         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (post)
          
-         466         274 LOAD_GLOBAL             21 (NULL + redirect)
+         497         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (post)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         468     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         499     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      316 LOAD_FAST                2 (post)
                      318 KW_NAMES                 4
                      320 PRECALL                  1
                      324 CALL                     1
                      334 STORE_FAST               3 (form)
          
-         471         336 LOAD_FAST                2 (post)
+         502         336 LOAD_FAST                2 (post)
          
-         472         338 LOAD_FAST                3 (form)
+         503         338 LOAD_FAST                3 (form)
          
-         470         340 LOAD_CONST               5 (('post', 'form'))
+         501         340 LOAD_CONST               5 (('post', 'form'))
                      342 BUILD_CONST_KEY_MAP      2
                      344 STORE_FAST               4 (context)
          
-         475         346 LOAD_GLOBAL             23 (NULL + render)
+         506         346 LOAD_GLOBAL             23 (NULL + render)
                      358 LOAD_FAST                0 (request)
                      360 LOAD_CONST               6 ('punkweb_bb/partials/post_update.html')
                      362 LOAD_FAST                4 (context)
                      364 KW_NAMES                 7
                      366 PRECALL                  3
                      370 CALL                     3
                      380 RETURN_VALUE
@@ -2808,15 +2961,15 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_edit', 'user', 'HttpResponseForbidden', 'method', 'PostModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'post_id', 'post', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_update_view'
-         firstlineno 453
+         firstlineno 484
          lnotab 0x02022c0234011e0216012c02280128021e022003020102fe0605
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -2827,67 +2980,67 @@
             0000000000000053007c006a05000000000000000064036b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064047c
             0269017d037415000000000000000000007c0064057c03ac06a6030000ab
             0300000000000000005300
-         478           0 RESUME                   0
+         509           0 RESUME                   0
          
-         480           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         511           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         482          46 LOAD_FAST                2 (post)
+         513          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         483          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         514          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         485     >>  128 LOAD_FAST                0 (request)
+         516     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         486         150 LOAD_FAST                2 (post)
+         517         150 LOAD_FAST                2 (post)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         488         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         519         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (post)
                      204 LOAD_ATTR                8 (thread)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         491     >>  266 LOAD_CONST               4 ('post')
+         522     >>  266 LOAD_CONST               4 ('post')
                      268 LOAD_FAST                2 (post)
          
-         490         270 BUILD_MAP                1
+         521         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         494         274 LOAD_GLOBAL             21 (NULL + render)
+         525         274 LOAD_GLOBAL             21 (NULL + render)
                      286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               5 ('punkweb_bb/partials/post_delete.html')
                      290 LOAD_FAST                3 (context)
                      292 KW_NAMES                 6
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
@@ -2901,94 +3054,94 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'thread', 'get_absolute_url', 'render')
          varnames   ('request', 'post_id', 'post', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_delete_view'
-         firstlineno 478
+         firstlineno 509
          lnotab 0x02022c0234011e02160128024c0304ff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007407000000000000000000006a
             040000000000000000a6000000ab00000000000000000074070000000000
             00000000006a0500000000000000006401ac02a6010000ab010000000000
             0000007a0a0000ac03a6010000ab010000000000000000a0060000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             005300
-         497           0 RESUME                   0
+         528           0 RESUME                   0
          
-         498           2 LOAD_GLOBAL              0 (Shout)
+         529           2 LOAD_GLOBAL              0 (Shout)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (filter)
          
-         499          46 LOAD_GLOBAL              7 (NULL + timezone)
+         530          46 LOAD_GLOBAL              7 (NULL + timezone)
                       58 LOAD_ATTR                4 (now)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 LOAD_GLOBAL              7 (NULL + timezone)
                       94 LOAD_ATTR                5 (timedelta)
                      104 LOAD_CONST               1 (12)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 BINARY_OP               10 (-)
          
-         498         126 KW_NAMES                 3
+         529         126 KW_NAMES                 3
                      128 PRECALL                  1
                      132 CALL                     1
          
-         500         142 LOAD_METHOD              6 (order_by)
+         531         142 LOAD_METHOD              6 (order_by)
                      164 LOAD_CONST               4 ('created_at')
                      166 PRECALL                  1
                      170 CALL                     1
          
-         498         180 RETURN_VALUE
+         529         180 RETURN_VALUE
          consts
             None
             12
             ('hours',)
             ('created_at__gt',)
             'created_at'
          names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'timedelta', 'order_by')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'current_shouts'
-         firstlineno 497
+         firstlineno 528
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
-         503           0 RESUME                   0
+         534           0 RESUME                   0
          
-         504           2 LOAD_GLOBAL              1 (NULL + current_shouts)
+         535           2 LOAD_GLOBAL              1 (NULL + current_shouts)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (shouts)
          
-         507          30 LOAD_CONST               1 ('shouts')
+         538          30 LOAD_CONST               1 ('shouts')
                       32 LOAD_FAST                1 (shouts)
          
-         506          34 BUILD_MAP                1
+         537          34 BUILD_MAP                1
                       36 STORE_FAST               2 (context)
          
-         509          38 LOAD_GLOBAL              3 (NULL + render)
+         540          38 LOAD_GLOBAL              3 (NULL + render)
                       50 LOAD_FAST                0 (request)
                       52 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       54 LOAD_FAST                2 (context)
                       56 KW_NAMES                 3
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -2999,15 +3152,15 @@
             ('context',)
          names      ('current_shouts', 'render')
          varnames   ('request', 'shouts', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_list_view'
-         firstlineno 503
+         firstlineno 534
          lnotab 0x02011c0304ff0403
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -3020,99 +3173,99 @@
             00a6000000ab000000000000000000725a7c02a008000000000000000000
             00000000000000000000006405ac06a6010000ab0100000000000000007d
             037c006a0000000000000000007c035f0000000000000000007c03a00800
             00000000000000000000000000000000000000a6000000ab000000000000
             00000001006401740500000000000000000000a6000000ab000000000000
             00000069017d017407000000000000000000007c0064027c01ac03a60300
             00ab03000000000000000053006400530064005300
-         512           0 RESUME                   0
+         543           0 RESUME                   0
          
-         513           2 LOAD_FAST                0 (request)
+         544           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_TRUE    34 (to 94)
          
-         515          26 LOAD_CONST               1 ('shouts')
+         546          26 LOAD_CONST               1 ('shouts')
                       28 LOAD_GLOBAL              5 (NULL + current_shouts)
                       40 PRECALL                  0
                       44 CALL                     0
          
-         514          54 BUILD_MAP                1
+         545          54 BUILD_MAP                1
                       56 STORE_FAST               1 (context)
          
-         517          58 LOAD_GLOBAL              7 (NULL + render)
+         548          58 LOAD_GLOBAL              7 (NULL + render)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       74 LOAD_FAST                1 (context)
                       76 KW_NAMES                 3
                       78 PRECALL                  3
                       82 CALL                     3
                       92 RETURN_VALUE
          
-         519     >>   94 LOAD_FAST                0 (request)
+         550     >>   94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                4 (method)
                      106 LOAD_CONST               4 ('POST')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE   128 (to 372)
          
-         520         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
+         551         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
                      128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                6 (POST)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (form)
          
-         522         156 LOAD_FAST                2 (form)
+         553         156 LOAD_FAST                2 (form)
                      158 LOAD_METHOD              7 (is_valid)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_JUMP_FORWARD_IF_FALSE    90 (to 376)
          
-         523         196 LOAD_FAST                2 (form)
+         554         196 LOAD_FAST                2 (form)
                      198 LOAD_METHOD              8 (save)
                      220 LOAD_CONST               5 (False)
                      222 KW_NAMES                 6
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (shout)
          
-         524         240 LOAD_FAST                0 (request)
+         555         240 LOAD_FAST                0 (request)
                      242 LOAD_ATTR                0 (user)
                      252 LOAD_FAST                3 (shout)
                      254 STORE_ATTR               0 (user)
          
-         525         264 LOAD_FAST                3 (shout)
+         556         264 LOAD_FAST                3 (shout)
                      266 LOAD_METHOD              8 (save)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 POP_TOP
          
-         528         304 LOAD_CONST               1 ('shouts')
+         559         304 LOAD_CONST               1 ('shouts')
                      306 LOAD_GLOBAL              5 (NULL + current_shouts)
                      318 PRECALL                  0
                      322 CALL                     0
          
-         527         332 BUILD_MAP                1
+         558         332 BUILD_MAP                1
                      334 STORE_FAST               1 (context)
          
-         530         336 LOAD_GLOBAL              7 (NULL + render)
+         561         336 LOAD_GLOBAL              7 (NULL + render)
          
-         531         348 LOAD_FAST                0 (request)
+         562         348 LOAD_FAST                0 (request)
                      350 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                      352 LOAD_FAST                1 (context)
          
-         530         354 KW_NAMES                 3
+         561         354 KW_NAMES                 3
                      356 PRECALL                  3
                      360 CALL                     3
                      370 RETURN_VALUE
          
-         519     >>  372 LOAD_CONST               0 (None)
+         550     >>  372 LOAD_CONST               0 (None)
                      374 RETURN_VALUE
          
-         522     >>  376 LOAD_CONST               0 (None)
+         553     >>  376 LOAD_CONST               0 (None)
                      378 RETURN_VALUE
          consts
             None
             'shouts'
             'punkweb_bb/shoutbox/shout_list.html'
             ('context',)
             'POST'
@@ -3120,15 +3273,15 @@
             ('commit',)
          names      ('user', 'is_authenticated', 'current_shouts', 'render', 'method', 'ShoutModelForm', 'POST', 'is_valid', 'save')
          varnames   ('request', 'context', 'form', 'shout')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_create_view'
-         firstlineno 512
+         firstlineno 543
          lnotab
             0x020118021cff040324021601280228012c01180128031cff04030c0106
             ff12f50403
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -3140,66 +3293,66 @@
             00000000000000730f7409000000000000000000006402a6010000ab0100
             0000000000000053007c006a05000000000000000064036b020000000072
             307c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f0000000000000000000074110000000000
             00000000006404a6010000ab010000000000000000a6010000ab01000000
             0000000000530064057c0269017d037413000000000000000000007c0064
             067c03ac07a6030000ab0300000000000000005300
-         535           0 RESUME                   0
+         566           0 RESUME                   0
          
-         537           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         568           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Shout)
                       26 LOAD_FAST                1 (shout_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (shout)
          
-         539          46 LOAD_FAST                2 (shout)
+         570          46 LOAD_FAST                2 (shout)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         540          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         571          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this shout.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         542     >>  128 LOAD_FAST                0 (request)
+         573     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    48 (to 246)
          
-         543         150 LOAD_FAST                2 (shout)
+         574         150 LOAD_FAST                2 (shout)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         545         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         576         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_GLOBAL             17 (NULL + reverse)
                      214 LOAD_CONST               4 ('punkweb_bb:index')
                      216 PRECALL                  1
                      220 CALL                     1
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         548     >>  246 LOAD_CONST               5 ('shout')
+         579     >>  246 LOAD_CONST               5 ('shout')
                      248 LOAD_FAST                2 (shout)
          
-         547         250 BUILD_MAP                1
+         578         250 BUILD_MAP                1
                      252 STORE_FAST               3 (context)
          
-         551         254 LOAD_GLOBAL             19 (NULL + render)
+         582         254 LOAD_GLOBAL             19 (NULL + render)
                      266 LOAD_FAST                0 (request)
                      268 LOAD_CONST               6 ('punkweb_bb/partials/shout_delete.html')
                      270 LOAD_FAST                3 (context)
                      272 KW_NAMES                 7
                      274 PRECALL                  3
                      278 CALL                     3
                      288 RETURN_VALUE
@@ -3214,36 +3367,36 @@
             ('context',)
          names      ('get_object_or_404', 'Shout', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'reverse', 'render')
          varnames   ('request', 'shout_id', 'shout', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_delete_view'
-         firstlineno 535
+         firstlineno 566
          lnotab 0x02022c0234011e0216012802380304ff0404
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
-         554           0 RESUME                   0
+         585           0 RESUME                   0
          
-         555           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         586           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         609           6 LOAD_CONST               2 ('codes')
+         640           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         608          10 BUILD_MAP                1
+         639          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         612          14 LOAD_GLOBAL              1 (NULL + render)
+         643          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
@@ -3255,25 +3408,25 @@
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
-         firstlineno 554
+         firstlineno 585
          lnotab 0x0201043604ff0404
       None
-   names      ('django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
+   names      ('django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'ThreadMoveForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'thread_move_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020118010c010c0114010c010c02280a0c011c010c010c010c0214
+      0x00ff020118010c010c0114010c010c022c0b0c011c010c010c010c0214
       030614061a060506200609060b160104ff0e010216160104ff0e01021616
       0104ff0e010217160104ff0e010212060c160104ff0e01021c160104ff0e
       010219160104ff0e010216160104ff0e01021c0616160104ff0e01021916
       0104ff0e010214160104ff0e01020c160104ff0e01020c160104ff0e0102
-      13160104ff0e010218160104ff0e010212060606090617160104ff0e0102
-      12
+      1d160104ff0e010213160104ff0e010218160104ff0e0102120606060906
+      17160104ff0e010212
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,18 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xe8ab0d66 (Wed Apr  3 19:20:08 2024 UTC)
-files sz: 840
+moddate:  0x74ff5866 (Thu May 30 22:36:36 2024 UTC)
+files sz: 1502
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a0101000200470064028400640365016a0200
-      00000000000000a6030000ab0300000000000000005a0364045300
+      00000000000000a6030000ab0300000000000000005a0302004700640484
+      00640565016a020000000000000000a6030000ab0300000000000000005a
+      0464065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('forms',))
                  6 IMPORT_NAME              0 (django)
                  8 IMPORT_FROM              1 (forms)
                 10 STORE_NAME               1 (forms)
@@ -24,16 +26,27 @@
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('BBCodeEditorWidget')
                 24 LOAD_NAME                1 (forms)
                 26 LOAD_ATTR                2 (Textarea)
                 36 PRECALL                  3
                 40 CALL                     3
                 50 STORE_NAME               3 (BBCodeEditorWidget)
-                52 LOAD_CONST               4 (None)
-                54 RETURN_VALUE
+   
+    25          52 PUSH_NULL
+                54 LOAD_BUILD_CLASS
+                56 LOAD_CONST               4 (<code object MarkdownEditorWidget, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py", line 25>)
+                58 MAKE_FUNCTION            0
+                60 LOAD_CONST               5 ('MarkdownEditorWidget')
+                62 LOAD_NAME                1 (forms)
+                64 LOAD_ATTR                2 (Textarea)
+                74 PRECALL                  3
+                78 CALL                     3
+                88 STORE_NAME               4 (MarkdownEditorWidget)
+                90 LOAD_CONST               6 (None)
+                92 RETURN_VALUE
    consts
       0
       ('forms',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -158,16 +171,150 @@
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py'
          name       'BBCodeEditorWidget'
          firstlineno 4
          lnotab 0x0c010a04
       'BBCodeEditorWidget'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 4
+         flags     : 0
+         code
+            0x8700970065005a0164005a0264015a0388006601640284085a04020047
+            00640384006404a6020000ab0200000000000000005a05880078015a0653
+            00
+                       0 MAKE_CELL                0 (__class__)
+         
+          25           2 RESUME                   0
+                       4 LOAD_NAME                0 (__name__)
+                       6 STORE_NAME               1 (__module__)
+                       8 LOAD_CONST               0 ('MarkdownEditorWidget')
+                      10 STORE_NAME               2 (__qualname__)
+         
+          26          12 LOAD_CONST               1 ('punkweb_bb/widgets/markdown-editor.html')
+                      14 STORE_NAME               3 (template_name)
+         
+          28          16 LOAD_CLOSURE             0 (__class__)
+                      18 BUILD_TUPLE              1
+                      20 LOAD_CONST               2 (<code object __init__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py", line 28>)
+                      22 MAKE_FUNCTION            8 (closure)
+                      24 STORE_NAME               4 (__init__)
+         
+          32          26 PUSH_NULL
+                      28 LOAD_BUILD_CLASS
+                      30 LOAD_CONST               3 (<code object Media, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py", line 32>)
+                      32 MAKE_FUNCTION            0
+                      34 LOAD_CONST               4 ('Media')
+                      36 PRECALL                  2
+                      40 CALL                     2
+                      50 STORE_NAME               5 (Media)
+                      52 LOAD_CLOSURE             0 (__class__)
+                      54 COPY                     1
+                      56 STORE_NAME               6 (__classcell__)
+                      58 RETURN_VALUE
+         consts
+            'MarkdownEditorWidget'
+            'punkweb_bb/widgets/markdown-editor.html'
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x9501970002007401000000000000000000007402000000000000000000
+                  007c00a6020000ab0200000000000000006a0200000000000000007c0169
+                  007c02a4018e01010064017c006a03000000000000000064023c00000064
+                  005300
+                             0 COPY_FREE_VARS           1
+               
+                28           2 RESUME                   0
+               
+                29           4 PUSH_NULL
+                             6 LOAD_GLOBAL              1 (NULL + super)
+                            18 LOAD_GLOBAL              2 (MarkdownEditorWidget)
+                            30 LOAD_FAST                0 (self)
+                            32 PRECALL                  2
+                            36 CALL                     2
+                            46 LOAD_ATTR                2 (__init__)
+                            56 LOAD_FAST                1 (args)
+                            58 BUILD_MAP                0
+                            60 LOAD_FAST                2 (kwargs)
+                            62 DICT_MERGE               1
+                            64 CALL_FUNCTION_EX         1
+                            66 POP_TOP
+               
+                30          68 LOAD_CONST               1 ('markdown-editor')
+                            70 LOAD_FAST                0 (self)
+                            72 LOAD_ATTR                3 (attrs)
+                            82 LOAD_CONST               2 ('class')
+                            84 STORE_SUBSCR
+                            88 LOAD_CONST               0 (None)
+                            90 RETURN_VALUE
+               consts
+                  None
+                  'markdown-editor'
+                  'class'
+               names      ('super', 'MarkdownEditorWidget', '__init__', 'attrs')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py'
+               name       '__init__'
+               firstlineno 28
+               lnotab 0x04014001
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 2
+               flags     : 0
+               code 0x970065005a0164005a026401640269015a0364035a0464045300
+                32           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('MarkdownEditorWidget.Media')
+                             8 STORE_NAME               2 (__qualname__)
+               
+                34          10 LOAD_CONST               1 ('all')
+                            12 LOAD_CONST               2 (('/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css',))
+               
+                33          14 BUILD_MAP                1
+                            16 STORE_NAME               3 (css)
+               
+                38          18 LOAD_CONST               3 (('/static/punkweb_bb/vendor/jquery-3.7.0.min.js', '/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js', '/static/punkweb_bb/editor/markdown-editor.js'))
+                            20 STORE_NAME               4 (js)
+                            22 LOAD_CONST               4 (None)
+                            24 RETURN_VALUE
+               consts
+                  'MarkdownEditorWidget.Media'
+                  'all'
+                  ('/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css',)
+                  ('/static/punkweb_bb/vendor/jquery-3.7.0.min.js', '/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js', '/static/punkweb_bb/editor/markdown-editor.js')
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'css', 'js')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py'
+               name       'Media'
+               firstlineno 32
+               lnotab 0x0a0204ff0405
+            'Media'
+         names      ('__name__', '__module__', '__qualname__', 'template_name', '__init__', 'Media', '__classcell__')
+         varnames   ()
+         freevars   ()
+         cellvars   ('__class__',)
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py'
+         name       'MarkdownEditorWidget'
+         firstlineno 25
+         lnotab 0x0c0104020a04
+      'MarkdownEditorWidget'
       None
-   names      ('django', 'forms', 'Textarea', 'BBCodeEditorWidget')
+   names      ('django', 'forms', 'Textarea', 'BBCodeEditorWidget', 'MarkdownEditorWidget')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/widgets.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c03
+   lnotab 0x00ff02010c032615
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/admin.py` & `punkweb_bb-0.3.0/punkweb_bb/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         "user__is_staff",
         "user__is_superuser",
     )
     search_fields = (
         "user__username",
         "user__email",
     )
-    readonly_fields = ("signature_rendered",)
-
-    def signature_rendered(self, obj):
-        return mark_safe(obj.signature.rendered)
 
 
 @admin.register(Category)
 class CategoryModelAdmin(admin.ModelAdmin):
     form = CategoryAdminModelForm
     list_display = (
         "name",
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.3.0/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/forms.py` & `punkweb_bb-0.3.0/punkweb_bb/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from django.contrib.auth.forms import AuthenticationForm, UserCreationForm
 
 from punkweb_bb.models import BoardProfile, Category, Post, Shout, Subcategory, Thread
-from punkweb_bb.widgets import BBCodeEditorWidget
+from punkweb_bb.utils import get_editor_widget
 
 
 class LoginForm(AuthenticationForm):
     """
     Override the default AuthenticationForm to add CSS classes to the
     username and password fields.
     """
@@ -35,15 +35,15 @@
     class Meta:
         model = BoardProfile
         fields = (
             "image",
             "signature",
         )
         widgets = {
-            "signature": BBCodeEditorWidget(),
+            "signature": get_editor_widget(),
         }
 
 
 class CategoryModelForm(forms.ModelForm):
     class Meta:
         model = Category
         fields = (
@@ -62,15 +62,15 @@
     class Meta:
         model = Post
         fields = ("content",)
         labels = {
             "content": "",
         }
         widgets = {
-            "content": BBCodeEditorWidget(),
+            "content": get_editor_widget(),
         }
 
 
 class ShoutModelForm(forms.ModelForm):
     class Meta:
         model = Shout
         fields = ("content",)
@@ -83,15 +83,15 @@
             "name",
             "description",
             "order",
             "staff_post_only",
         )
         widgets = {
             "name": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),
-            "description": BBCodeEditorWidget(),
+            "description": get_editor_widget(),
             "order": forms.TextInput(
                 attrs={"class": "pw-input", "min": "0", "type": "number"}
             ),
         }
 
 
 class ThreadModelForm(forms.ModelForm):
@@ -99,9 +99,17 @@
         model = Thread
         fields = (
             "title",
             "content",
         )
         widgets = {
             "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),
-            "content": BBCodeEditorWidget(),
+            "content": get_editor_widget(),
         }
+
+
+class ThreadMoveForm(forms.Form):
+    subcategory = forms.ModelChoiceField(
+        queryset=Subcategory.objects.all(),
+        empty_label="Select a subcategory",
+        widget=forms.Select(attrs={"class": "pw-input"}),
+    )
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/middleware.py` & `punkweb_bb-0.3.0/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.3.0/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/0003_alter_thread_options.py` & `punkweb_bb-0.3.0/punkweb_bb/migrations/0003_alter_thread_options.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/0004_groupstyle.py` & `punkweb_bb-0.3.0/punkweb_bb/migrations/0004_groupstyle.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/models.py` & `punkweb_bb-0.3.0/punkweb_bb/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
 from django.core.cache import cache
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
 from django.utils import timezone
-from precise_bbcode.fields import BBCodeTextField
 
 from punkweb_bb.mixins import TimestampMixin, UUIDPrimaryKeyMixin
 from punkweb_bb.utils import get_highest_priority_group, get_styled_username
 
 User = get_user_model()
 
 
@@ -20,15 +19,15 @@
     ext = os.path.splitext(filename)[-1]
     return f"punkweb_bb/board_profiles/{instance.user.username}/image{ext}"
 
 
 class BoardProfile(UUIDPrimaryKeyMixin, TimestampMixin):
     user = models.OneToOneField(User, related_name="profile", on_delete=models.CASCADE)
     image = models.ImageField(upload_to=profile_image_upload_to, blank=True, null=True)
-    signature = BBCodeTextField(max_length=1024, blank=True, null=True)
+    signature = models.TextField(max_length=1024, blank=True)
 
     class Meta:
         ordering = ("user__username",)
 
     @property
     def priority_group(self):
         return get_highest_priority_group(self.user)
@@ -72,15 +71,15 @@
 
 class Subcategory(UUIDPrimaryKeyMixin, TimestampMixin):
     category = models.ForeignKey(
         Category, related_name="subcategories", on_delete=models.CASCADE
     )
     name = models.CharField(max_length=255)
     slug = models.SlugField(max_length=1024, unique=True)
-    description = BBCodeTextField(blank=True, null=True)
+    description = models.TextField(blank=True)
     order = models.PositiveIntegerField(default=0)
     staff_post_only = models.BooleanField(default=False)
 
     class Meta:
         verbose_name = "subcategory"
         verbose_name_plural = "subcategories"
         ordering = (
@@ -112,27 +111,28 @@
 
 class Thread(UUIDPrimaryKeyMixin, TimestampMixin):
     subcategory = models.ForeignKey(
         Subcategory, related_name="threads", on_delete=models.CASCADE
     )
     user = models.ForeignKey(User, related_name="threads", on_delete=models.CASCADE)
     title = models.CharField(max_length=255)
-    content = BBCodeTextField()
+    content = models.TextField()
     is_pinned = models.BooleanField(default=False)
     is_closed = models.BooleanField(default=False)
     last_post_created_at = models.DateTimeField(auto_now_add=True)
     view_count = models.PositiveIntegerField(default=0)
 
     class Meta:
         ordering = (
             "subcategory",
             "-is_pinned",
             "-last_post_created_at",
         )
         permissions = (
+            ("move_thread", "Can move thread"),
             ("pin_thread", "Can pin thread"),
             ("close_thread", "Can close thread"),
         )
 
     def __str__(self):
         return f"{self.title}"
 
@@ -156,15 +156,15 @@
     def get_absolute_url(self):
         return reverse("punkweb_bb:thread", args=[self.id])
 
 
 class Post(UUIDPrimaryKeyMixin, TimestampMixin):
     thread = models.ForeignKey(Thread, related_name="posts", on_delete=models.CASCADE)
     user = models.ForeignKey(User, related_name="posts", on_delete=models.CASCADE)
-    content = BBCodeTextField()
+    content = models.TextField()
 
     class Meta:
         ordering = ("created_at",)
 
     def __str__(self):
         return f"{self.thread} > {self.user} > {self.created_at}"
 
@@ -218,14 +218,14 @@
 
 class GroupStyle(UUIDPrimaryKeyMixin, TimestampMixin):
     group = models.OneToOneField(Group, related_name="style", on_delete=models.CASCADE)
     priority = models.PositiveIntegerField(
         default=0,
         help_text="Highest priority is displayed",
     )
-    username_style = BBCodeTextField()
+    username_style = models.TextField()
 
     class Meta:
         ordering = ("-priority",)
 
     def __str__(self):
         return f"{self.group} > {self.priority}"
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/parsers.py` & `punkweb_bb-0.3.0/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,38 @@
 
 .thread__reply__content {
   display: flex;
   flex-direction: column;
   gap: 1rem;
 }
 
+.threadMoveForm {
+  display: flex;
+  flex-direction: column;
+  gap: 1rem;
+}
+
+.threadMoveForm__field {
+  display: flex;
+  flex-direction: column;
+  gap: 0.5rem;
+}
+
+.threadMoveForm .errorlist {
+  color: var(--oc-red-9);
+  margin: 0;
+}
+
+.threadMoveForm__actions {
+  align-items: center;
+  display: flex;
+  justify-content: flex-end;
+  gap: 1rem;
+}
+
 @media screen and (max-width: 1024px) {
   .thread {
     flex-direction: column;
   }
 
   .thread__user {
     border-right: none;
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_create.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/category_update.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends 'punkweb_bb/base.html' %}
 
-{% load static bbcode_tags styled_username %}
+{% load static render styled_username %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/index.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/shoutbox.css' %}" />
 {% endblock %}
 
 {% block extra_script %}
@@ -71,15 +71,15 @@
             </thead>
             <tbody>
               {% for subcategory in category.subcategories.all %}
               <tr>
                 <td>
                   <a href="{{subcategory.get_absolute_url}}" title="{{subcategory.name}}">{{subcategory.name}}</a>
                   <div>
-                    {{subcategory.description.rendered}}
+                    {{subcategory.description|render}}
                   </div>
                 </td>
                 <td>{{subcategory.thread_count}}</td>
                 <td>{{subcategory.post_count}}</td>
                 <td>
                   {% if subcategory.latest_thread %}
                   {% if subcategory.latest_thread.latest_post %}
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-{% extends 'punkweb_bb/base.html' %} {% load static bbcode_tags styled_username
-%} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static render styled_username %}
+{% block extra_head %}
 {% endblock %} {% block extra_script %}
 {% endblock %} {% block content %}
 {% if punkweb_bb.settings.SHOUTBOX_ENABLED|default:True %} {% include
 'punkweb_bb/shoutbox/shoutbox.html' %} {% endif %} {% for category in
 categories %}
 _{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}} {{%% iiff
-ppeerrmmss..ppuunnkkwweebb__bbbb..aadddd__ssuubbccaatteeggoorryy %%}}
-_aa_dd_dd_ {{%% eennddiiff %%}} {{%% iiff
-ppeerrmmss..ppuunnkkwweebb__bbbb..cchhaannggee__ccaatteeggoorryy %%}} TThhrreeaaddss                     PPoossttss
-_ee_dd_ii_tt_ {{%% eennddiiff %%}} {{%% iiff
-ppeerrmmss..ppuunnkkwweebb__bbbb..ddeelleettee__ccaatteeggoorryy %%}}
-ddeelleettee {{%% eennddiiff %%}}
-                                                                                          {% if subcategory.latest_thread %} {% if
-                                                                                          subcategory.latest_thread.latest_post %}
-                                                                                          {% if subcategory.latest_thread.latest_post.user.profile.image
-                                                                                          %} [{
-                                                                                          {subcategory.latest_thread.latest_post.user.profile.image.url}}]
-                                                                                          {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
-                                                                                          %}]{% endif %}
-                                                                                          _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
-                                                                                          {{subcategory.latest_thread.latest_post.created_at|date:'M j,
-_{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}                                                                      Y'}} at {{subcategory.latest_thread.latest_post.created_at|date:
-{                                   {                           {                         'g:i A'}} â¢ _{
-{subcategory.description.rendered}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
-                                                                                          {% else %}
-                                                                                          {% if subcategory.latest_thread.user.profile.image %} [{
-                                                                                          {subcategory.latest_thread.user.profile.image.url}}]{% else%} [
-                                                                                          {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
-                                                                                          %}
-                                                                                          _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
-                                                                                          {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
-                                                                                          {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
-                                                                                          _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
-                                                                                          {% endif %} {% else %} No threads {% endif %}
+ppeerrmmss..ppuunnkkwweebb__bbbb..aadddd__ssuubbccaatteeggoorryy
+%%}} _aa_dd_dd_ {{%% eennddiiff %%}} {{%% iiff
+ppeerrmmss..ppuunnkkwweebb__bbbb..cchhaannggee__ccaatteeggoorryy  TThhrreeaaddss                     PPoossttss
+%%}} _ee_dd_ii_tt_ {{%% eennddiiff %%}} {{%% iiff
+ppeerrmmss..ppuunnkkwweebb__bbbb..ddeelleettee__ccaatteeggoorryy
+%%}} ddeelleettee {{%% eennddiiff %%}}
+                                                                                        {% if subcategory.latest_thread %} {% if
+                                                                                        subcategory.latest_thread.latest_post %}
+                                                                                        {% if subcategory.latest_thread.latest_post.user.profile.image
+                                                                                        %} [{
+                                                                                        {subcategory.latest_thread.latest_post.user.profile.image.url}}]
+                                                                                        {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
+                                                                                        %}]{% endif %}
+                                                                                        _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
+                                                                                        {{subcategory.latest_thread.latest_post.created_at|date:'M j,
+_{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}                                                                    Y'}} at {{subcategory.latest_thread.latest_post.created_at|date:
+{                                 {                           {                         'g:i A'}} â¢ _{
+{subcategory.description|render}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
+                                                                                        {% else %}
+                                                                                        {% if subcategory.latest_thread.user.profile.image %} [{
+                                                                                        {subcategory.latest_thread.user.profile.image.url}}]{% else%} [
+                                                                                        {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
+                                                                                        %}
+                                                                                        _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
+                                                                                        {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
+                                                                                        {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
+                                                                                        _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
+                                                                                        {% endif %} {% else %} No threads {% endif %}
 {% endfor %} {% if perms.punkweb_bb.add_category %} _a_d_d_ {% endif %}
 Recent threads
 {% for thread in recent_threads %}
 {% if thread.user.profile.image %} [{{thread.user.profile.image.url}}]{% else%}
 [{% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_}
 {{thread.created_at|date:'M j, Y'}} at {{thread.created_at|date:'g:i A'}} â¢ _{
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static styled_username %}
+{% load static render styled_username %}
 
 {% block title_prefix %}{{ user.username }} | {% endblock%}
 {% block og_title_prefix %}{{ user.username }} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/profile.css' %}">
 {% endblock %}
@@ -72,15 +72,15 @@
       {% for thread in user.threads.all %}
         <li class="profile__thread">
           <div class="profile__thread__details">
             <div class="profile__thread__title">
               <a href="{% url 'punkweb_bb:thread' thread.id %}">{{ thread.title }}</a>
             </div>
             <p class="profile__thread__preview">
-              {{ thread.content.rendered|striptags|truncatechars:120 }}
+              {{ thread.content|render|striptags|truncatechars:120 }}
             </p>
             <div class="profile__thread__date">
               <time datetime="{{thread.created_at|date:'c'}}">
                 {{thread.created_at|date:'M j, Y'}} at
                 {{thread.created_at|date:'g:i A'}}
               </time>
               •
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends 'punkweb_bb/base.html' %} {% load static styled_username %} {% block
-title_prefix %}{{ user.username }} | {% endblock%} {% block og_title_prefix %}{
-{ user.username }} | {% endblock %} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static render styled_username %}
+{% block title_prefix %}{{ user.username }} | {% endblock%} {% block
+og_title_prefix %}{{ user.username }} | {% endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _M_e_m_b_e_r_s
     * {{ user.username }}
 {% if user.profile.image %} [{{user.profile.image.url}}]{% else %} [{% static
 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 {{user|styled_username}}
@@ -13,13 +13,13 @@
 Posts: {{user.profile.post_count}}
 Threads
 {% if user.threads.count == 0 %}
 {{ user.username }} has not created any threads.
 {% else %}
     * {% for thread in user.threads.all %}
     * _{_{_ _t_h_r_e_a_d_._t_i_t_l_e_ _}_}
-      {{ thread.content.rendered|striptags|truncatechars:120 }}
+      {{ thread.content|render|striptags|truncatechars:120 }}
       {{thread.created_at|date:'M j, Y'}} at {{thread.created_at|date:'g:i A'}}
       â¢ _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {% endfor %}
 {% endif %}
 {% endblock %}
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-{% load shoutbox_bbcode can_delete styled_username %}
+{% load shoutbox_render styled_username can_delete %}
 
 {% for shout in shouts %}
 <div class="shoutbox__shout">
   <div class="shoutbox__shout__content">
     <time datetime="{{shout.created_at|date:'c'}}">{{shout.created_at | date:'g:i A'}}</time>
     <span><a href="{% url 'punkweb_bb:profile' shout.user.id %}">{{shout.user|styled_username}}</a>: </span>
-    <span>{{ shout.content | safe | shoutbox_bbcode }}</span>
+    <span>{{ shout.content|shoutbox_render }}</span>
   </div>
   {% if shout|can_delete:request.user %}
   <div class="shoutbox__shout__actions">
     <button
       class="pw-icon-button default danger sm"
       title="Delete"
       hx-get="{% url 'punkweb_bb:shout_delete' shout.id %}"
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% load shoutbox_bbcode can_delete styled_username %} {% for shout in shouts %}
+{% load shoutbox_render styled_username can_delete %} {% for shout in shouts %}
 {{shout.created_at | date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}: {
-{ shout.content | safe | shoutbox_bbcode }}
+{ shout.content|shoutbox_render }}
 {% if shout|can_delete:request.user %}
 delete
 {% endif %}
 {% endfor %}
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
               {% endif %}
             </div>
             <div>
               <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
                 {{thread.user|styled_username}}
               </a>
               •
-              <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'m j, Y'}}</time>
+              <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'M j, Y'}}</time>
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
@@ -19,15 +19,15 @@
 thread.is_pinned %} keep {%                                            _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
 endif %} {% if                                                         _Y_'_}_}
 thread.is_closed %} lock {%                         {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 endif %}                       {                    {thread.view_count {% if thread.latest_post.user.profile.image
 _{                              {thread.post_count}} | humanize_int}}   %} [{
 _{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}                                         {thread.latest_post.user.profile.image.url}}]
 â¢ {{thread.created_at |                                              {% else %} [{% static 'punkweb_bb/img/
-date:'m j, Y'}}                                                        default-profile-image.png' %}]{% endif %}
+date:'M j, Y'}}                                                        default-profile-image.png' %}]{% endif %}
                                                                        {% else %} No posts {% endif %}
 {% if threads.has_other_pages %}
     * {% if threads.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in threads.paginator.page_range %} {% if
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_create.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/subcategory_update.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static can_delete can_edit can_post styled_username %}
+{% load static render styled_username can_delete can_edit can_post %}
 
 {% block title_prefix %}{{thread.title}} | {% endblock %}
 {% block og_title_prefix %}{{thread.title}} | {% endblock %}
 
 {% block extra_head %}
-<meta name="description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
-<meta property="og:description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
+<meta name="description" content="{{thread.content|render|striptags|truncatechars:120}}" />
+<meta property="og:description" content="{{thread.content|render|striptags|truncatechars:120}}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/post-form.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread-form.css' %}" />
 {{post_form.media.css}}
 {% endblock %}
 
 {% block extra_script %}
@@ -38,15 +38,15 @@
 
 {% if posts.number == 1 %}
 <h1>{{thread.title}}</h1>
 
 <div class="pw-card fluid margin">
   <div class="pw-card-header">
     <div class="thread__date">
-      <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'M d, Y'}}</time>
+      <time datetime="{{thread.created_at|date:'c'}}">{{thread.created_at | date:'M j, Y'}}</time>
     </div>
   </div>
   <div class="thread">
     <div class="thread__user">
       <div class="thread__user__info">
         <div class="thread__user__image">
           {% if thread.user.profile.image %}
@@ -71,29 +71,39 @@
           {% endif %}
         </div>
       </div>
       <div class="thread__user__details">
         <div class="thread__user__details__row">
           <div class="thread__user__details__label">Joined:</div>
           <div class="thread__user__details__value">
-            <time datetime="{{thread.user.date_joined|date:'c'}}">{{thread.user.date_joined | date:'M d, Y'}}</time>
+            <time datetime="{{thread.user.date_joined|date:'c'}}">{{thread.user.date_joined | date:'M j, Y'}}</time>
           </div>
         </div>
         <div class="thread__user__details__row">
           <div class="thread__user__details__label">Posts:</div>
           <div class="thread__user__details__value">{{thread.user.profile.post_count}}</div>
         </div>
       </div>
     </div>
     <div class="thread__main">
       <div class="thread__content">
-        {{thread.content.rendered}}
+        {{thread.content|render}}
       </div>
-      {% if thread|can_delete:request.user or thread|can_edit:request.user or perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
+      {% if thread|can_delete:request.user or thread|can_edit:request.user or perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread or perms.punkweb_bb.move_thread %}
       <div class="thread__actions">
+        {% if perms.punkweb_bb.move_thread %}
+        <a 
+          class="pw-icon-button default rounded"
+          title="Move"
+          hx-get="{% url 'punkweb_bb:thread_move' thread.id %}"
+          hx-target="#modal-portal"
+        >
+          <span class="material-symbols-outlined">move_item</span>
+        </a>
+        {% endif %}
         {% if perms.punkweb_bb.pin_thread %}
         <a 
           class="pw-icon-button default rounded"
           title="{% if thread.is_pinned %}Unpin{% else %}Pin{% endif %}"
           hx-get="{% url 'punkweb_bb:thread_pin' thread.id %}"
           hx-swap="none"
         >
@@ -135,29 +145,29 @@
           hx-target="#modal-portal"
         >
           <span class="material-symbols-outlined">delete</span>
         </a>
         {% endif %}
       </div>
       {% endif %}
-      {% if thread.user.profile.signature.rendered %}
+      {% if thread.user.profile.signature|render %}
       <div class="thread__signature">
-        {{thread.user.profile.signature.rendered}}
+        {{thread.user.profile.signature|render}}
       </div>
       {% endif %}
     </div>
   </div>
 </div>
 {% endif %}
 
 {% for post in posts %}
 <div id="post-{{post.id}}" class="pw-card fluid margin">
   <div class="pw-card-header thread__header">
     <div class="thread__date">
-      <time datetime="{{post.created_at|date:'c'}}">{{post.created_at | date:'M d, Y'}}</time>
+      <time datetime="{{post.created_at|date:'c'}}">{{post.created_at | date:'M j, Y'}}</time>
     </div>
     <a class="thread__index" href="{{post.get_absolute_url}}">#{{post.index}}</a>
   </div>
   <div class="thread">
     <div class="thread__user">
       <div class="thread__user__info">
         <div class="thread__user__image">
@@ -187,26 +197,26 @@
           {% endif %}
         </div>
       </div>
       <div class="thread__user__details">
         <div class="thread__user__details__row">
           <div class="thread__user__details__label">Joined:</div>
           <div class="thread__user__details__value">
-            <time datetime="{{post.user.date_joined|date:'c'}}">{{post.user.date_joined | date:'M d, Y'}}</time>
+            <time datetime="{{post.user.date_joined|date:'c'}}">{{post.user.date_joined | date:'M j, Y'}}</time>
           </div>
         </div>
         <div class="thread__user__details__row">
           <div class="thread__user__details__label">Posts:</div>
           <div class="thread__user__details__value">{{post.user.profile.post_count}}</div>
         </div>
       </div>
     </div>
     <div class="thread__main">
       <div class="thread__content">
-        {{post.content.rendered}}
+        {{post.content|render}}
       </div>
       {% if post|can_delete:request.user or post|can_edit:request.user %}
       <div class="thread__actions">
         {% if post|can_edit:request.user %}
         <a
           class="pw-icon-button default rounded"
           title="Edit"
@@ -224,17 +234,17 @@
           hx-target="#modal-portal"
         >
           <span class="material-symbols-outlined">delete</span>
         </a>
         {% endif %}
       </div>
       {% endif %}
-      {% if post.user.profile.signature.rendered %}
+      {% if post.user.profile.signature|render %}
       <div class="thread__signature">
-        {{post.user.profile.signature.rendered}}
+        {{post.user.profile.signature|render}}
       </div>
       {% endif %}
     </div>
   </div>
 </div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,63 +1,65 @@
-{% extends 'punkweb_bb/base.html' %} {% load static can_delete can_edit
-can_post styled_username %} {% block title_prefix %}{{thread.title}} | {%
+{% extends 'punkweb_bb/base.html' %} {% load static render styled_username
+can_delete can_edit can_post %} {% block title_prefix %}{{thread.title}} | {%
 endblock %} {% block og_title_prefix %}{{thread.title}} | {% endblock %} {%
 block extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
 ************ {{{{tthhrreeaadd..ttiittllee}}}} ************
-{{thread.created_at | date:'M d, Y'}}
+{{thread.created_at | date:'M j, Y'}}
 {% if thread.user.profile.image %} [{{thread.user.username}}]{% else %} [{
 {thread.user.username}}]{% endif %}
 {% if thread.user.profile.is_online %}
 {% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 {% if thread.user.profile.priority_group %} {
 {thread.user.profile.priority_group.name}} {% else %} Member {% endif %}
 Joined:
-{{thread.user.date_joined | date:'M d, Y'}}
+{{thread.user.date_joined | date:'M j, Y'}}
 Posts:
 {{thread.user.profile.post_count}}
-{{thread.content.rendered}}
+{{thread.content|render}}
 {% if thread|can_delete:request.user or thread|can_edit:request.user or
-perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
-{% if perms.punkweb_bb.pin_thread %} {% if thread.is_pinned %} keep_off {% else
-%} keep {% endif %} {% endif %} {% if perms.punkweb_bb.close_thread %} {% if
+perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread or
+perms.punkweb_bb.move_thread %}
+{% if perms.punkweb_bb.move_thread %} move_item {% endif %} {% if
+perms.punkweb_bb.pin_thread %} {% if thread.is_pinned %} keep_off {% else %}
+keep {% endif %} {% endif %} {% if perms.punkweb_bb.close_thread %} {% if
 thread.is_closed %} lock_open {% else %} lock {% endif %} {% endif %} {% if
 thread|can_edit:request.user %} _e_d_i_t_ {% endif %} {% if thread|can_delete:
 request.user %} delete {% endif %}
-{% endif %} {% if thread.user.profile.signature.rendered %}
-{{thread.user.profile.signature.rendered}}
+{% endif %} {% if thread.user.profile.signature|render %}
+{{thread.user.profile.signature|render}}
 {% endif %}
 {% endif %} {% for post in posts %}
-{{post.created_at | date:'M d, Y'}}
+{{post.created_at | date:'M j, Y'}}
 _#_{_{_p_o_s_t_._i_n_d_e_x_}_}
 {% if post.user.profile.image %}
 [{{post.user.username}}]
 {% else %}
 [{{post.user.username}}]
 {% endif %}
 {% if post.user.profile.is_online %}
 {% endif %} _{_{_p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 {% if post.user.profile.priority_group %} {
 {post.user.profile.priority_group.name}} {% else %} Member {% endif %}
 Joined:
-{{post.user.date_joined | date:'M d, Y'}}
+{{post.user.date_joined | date:'M j, Y'}}
 Posts:
 {{post.user.profile.post_count}}
-{{post.content.rendered}}
+{{post.content|render}}
 {% if post|can_delete:request.user or post|can_edit:request.user %}
 {% if post|can_edit:request.user %} edit {% endif %} {% if post|can_delete:
 request.user %} delete {% endif %}
-{% endif %} {% if post.user.profile.signature.rendered %}
-{{post.user.profile.signature.rendered}}
+{% endif %} {% if post.user.profile.signature|render %}
+{{post.user.profile.signature|render}}
 {% endif %}
 {% endfor %} {% if posts.has_other_pages %}
     * {% if posts.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in posts.paginator.page_range %} {% if posts.number
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc` & `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.3/punkweb_bb/tests.py` & `punkweb_bb-0.3.0/punkweb_bb/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             self.url,
             {
                 "signature": "[b]test[/b]",
             },
         )
 
         self.user.profile.refresh_from_db()
-        self.assertEqual(self.user.profile._signature_rendered, "<strong>test</strong>")
+        self.assertEqual(self.user.profile.signature, "[b]test[/b]")
 
         self.assertEqual(response.status_code, 200)
 
 
 class ThreadCreateViewTestCase(TestCase):
     def setUp(self):
         self.client = Client()
@@ -542,15 +542,15 @@
             },
             follow=True,
         )
 
         self.assertRedirects(response, self.thread.get_absolute_url())
         self.thread.refresh_from_db()
         self.assertEqual(self.thread.title, "edit")
-        self.assertEqual(self.thread._content_rendered, "edit")
+        self.assertEqual(self.thread.content, "edit")
 
 
 class ThreadDeleteViewTestCase(TestCase):
     def setUp(self):
         self.client = Client()
         self.user = User.objects.create_user(username="test", password="test")
         self.other_user = User.objects.create_user(username="other", password="other")
@@ -671,15 +671,15 @@
                 "content": "edit",
             },
             follow=True,
         )
 
         self.assertRedirects(response, self.post.get_absolute_url())
         self.post.refresh_from_db()
-        self.assertEqual(self.post._content_rendered, "edit")
+        self.assertEqual(self.post.content, "edit")
 
 
 class PostDeleteViewTestCase(TestCase):
     def setUp(self):
         self.client = Client()
         self.user = User.objects.create_user(username="test", password="test")
         self.other_user = User.objects.create_user(username="other", password="other")
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/urls.py` & `punkweb_bb-0.3.0/punkweb_bb/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     path(
         "thread/<str:thread_id>/create-post/",
         views.post_create_view,
         name="post_create",
     ),
     path("thread/<str:thread_id>/pin/", views.thread_pin_view, name="thread_pin"),
     path("thread/<str:thread_id>/close/", views.thread_close_view, name="thread_close"),
+    path("thread/<str:thread_id>/move/", views.thread_move_view, name="thread_move"),
     path("post/<str:post_id>/delete/", views.post_delete_view, name="post_delete"),
     path("post/<str:post_id>/update/", views.post_update_view, name="post_update"),
     path("shout-list/", views.shout_list_view, name="shout_list"),
     path("shout-create/", views.shout_create_view, name="shout_create"),
     path("shout/<str:shout_id>/delete/", views.shout_delete_view, name="shout_delete"),
     path("bbcode/", views.bbcode_view, name="bbcode"),
 ]
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb/views.py` & `punkweb_bb-0.3.0/punkweb_bb/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     CategoryModelForm,
     LoginForm,
     PostModelForm,
     ShoutModelForm,
     SignUpForm,
     SubcategoryModelForm,
     ThreadModelForm,
+    ThreadMoveForm,
 )
 from punkweb_bb.guests import guest_list
 from punkweb_bb.models import Category, Post, Shout, Subcategory, Thread
 from punkweb_bb.pagination import paginate_qs
 from punkweb_bb.response import htmx_redirect
 from punkweb_bb.utils import get_unique_slug
 
@@ -402,39 +403,69 @@
     }
 
     return render(request, "punkweb_bb/partials/thread_delete.html", context=context)
 
 
 @login_required(login_url="/login/")
 def thread_pin_view(request, thread_id):
-    thread = get_object_or_404(Thread, pk=thread_id)
-
     if not request.user.has_perm("punkweb_bb.pin_thread"):
         return HttpResponseForbidden("You do not have permission to pin threads.")
 
+    thread = get_object_or_404(Thread, pk=thread_id)
+
     thread.is_pinned = not thread.is_pinned
     thread.save()
 
     return htmx_redirect(thread.get_absolute_url())
 
 
 @login_required(login_url="/login/")
 def thread_close_view(request, thread_id):
-    thread = get_object_or_404(Thread, pk=thread_id)
-
     if not request.user.has_perm("punkweb_bb.close_thread"):
         return HttpResponseForbidden("You do not have permission to close threads.")
 
+    thread = get_object_or_404(Thread, pk=thread_id)
+
     thread.is_closed = not thread.is_closed
     thread.save()
 
     return htmx_redirect(thread.get_absolute_url())
 
 
 @login_required(login_url="/login/")
+def thread_move_view(request, thread_id):
+    if not request.user.has_perm("punkweb_bb.move_thread"):
+        return HttpResponseForbidden("You do not have permission to move threads.")
+
+    thread = get_object_or_404(Thread, pk=thread_id)
+
+    if request.method == "POST":
+        form = ThreadMoveForm(request.POST)
+
+        if form.is_valid():
+            thread.subcategory = form.cleaned_data["subcategory"]
+            thread.save()
+
+            return redirect(thread)
+
+    initial_data = {
+        "subcategory": thread.subcategory,
+    }
+
+    form = ThreadMoveForm(data=initial_data)
+
+    context = {
+        "thread": thread,
+        "form": form,
+    }
+
+    return render(request, "punkweb_bb/partials/thread_move.html", context=context)
+
+
+@login_required(login_url="/login/")
 def post_create_view(request, thread_id):
     thread = get_object_or_404(Thread, pk=thread_id)
 
     if not thread.can_post(request.user):
         return HttpResponseForbidden(
             "You do not have permission to post in this thread."
         )
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.3.0/punkweb_bb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.2.3
+Version: 0.3.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -24,28 +24,43 @@
 
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
+- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
+- [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
-- Django 4.2+
+- Django 4.0+
 - django-precise-bbcode 1.2+
+- markdown 3.6+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
+## BBCode or Markdown?
+
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+
+BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+
+```python
+PUNKWEB_BB = {
+  "RENDERER": "markdown",
+}
+```
+
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
 Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
@@ -54,24 +69,15 @@
 INSTALLED_APPS = [
     ...
     "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required. It must be installed before `punkweb_bb`.
-
-Add the following middleware to your `MIDDLEWARE` setting:
-
-```python
-MIDDLEWARE = [
-    ...
-    "punkweb_bb.middleware.ProfileOnlineCacheMiddleware",
-]
-```
+_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
 
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
@@ -106,14 +112,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
+  "RENDERER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
@@ -130,43 +137,50 @@
 HTML:
 
 ```bash
 coverage run && coverage html
 ```
 
 ```bash
-Found 57 test(s).
+Found 59 test(s).
 Creating test database for alias 'default'...
 System check identified no issues (0 silenced).
-.........................................................
+...........................................................
 ----------------------------------------------------------------------
-Ran 57 tests in 8.824s
+Ran 59 tests in 9.166s
 
 OK
 Destroying test database for alias 'default'...
-Name                                         Stmts   Miss  Cover
-----------------------------------------------------------------
-punkweb_bb/__init__.py                           0      0   100%
-punkweb_bb/admin.py                             41      1    98%
-punkweb_bb/admin_forms.py                       28      0   100%
-punkweb_bb/apps.py                               6      0   100%
-punkweb_bb/bbcode_tags.py                      115      3    97%
-punkweb_bb/context_processors.py                 3      0   100%
-punkweb_bb/forms.py                             35      0   100%
-punkweb_bb/middleware.py                        10      0   100%
-punkweb_bb/mixins.py                            11      0   100%
-punkweb_bb/models.py                           124      0   100%
-punkweb_bb/pagination.py                        11      4    64%
-punkweb_bb/parsers.py                           50      2    96%
-punkweb_bb/response.py                           3      0   100%
-punkweb_bb/settings.py                           6      0   100%
-punkweb_bb/signals.py                            9      0   100%
-punkweb_bb/templatetags/__init__.py              0      0   100%
-punkweb_bb/templatetags/humanize_int.py          9      5    44%
-punkweb_bb/templatetags/shoutbox_bbcode.py       9      0   100%
-punkweb_bb/tests.py                            410      0   100%
-punkweb_bb/urls.py                               4      0   100%
-punkweb_bb/views.py                            174     17    90%
-punkweb_bb/widgets.py                            8      0   100%
-----------------------------------------------------------------
-TOTAL                                         1066     32    97%
+Name                                           Stmts   Miss  Cover
+------------------------------------------------------------------
+punkweb_bb/__init__.py                             0      0   100%
+punkweb_bb/admin.py                               43      0   100%
+punkweb_bb/admin_forms.py                         34      0   100%
+punkweb_bb/apps.py                                 6      0   100%
+punkweb_bb/context_processors.py                   3      0   100%
+punkweb_bb/forms.py                               47      0   100%
+punkweb_bb/guests.py                              13      0   100%
+punkweb_bb/middleware.py                          14      0   100%
+punkweb_bb/mixins.py                              11      0   100%
+punkweb_bb/models.py                             153      1    99%
+punkweb_bb/pagination.py                          11      4    64%
+punkweb_bb/parsers.py                             50     36    28%
+punkweb_bb/response.py                             3      0   100%
+punkweb_bb/settings.py                            11      0   100%
+punkweb_bb/signals.py                              9      0   100%
+punkweb_bb/templatetags/__init__.py                0      0   100%
+punkweb_bb/templatetags/can_delete.py              5      0   100%
+punkweb_bb/templatetags/can_edit.py                5      0   100%
+punkweb_bb/templatetags/can_post.py                5      0   100%
+punkweb_bb/templatetags/humanize_int.py            9      5    44%
+punkweb_bb/templatetags/render.py                 36     12    67%
+punkweb_bb/templatetags/shoutbox_render.py        18      2    89%
+punkweb_bb/templatetags/styled_group_name.py       7      1    86%
+punkweb_bb/templatetags/styled_username.py         6      0   100%
+punkweb_bb/tests.py                              418      0   100%
+punkweb_bb/urls.py                                 4      0   100%
+punkweb_bb/utils.py                               42     24    43%
+punkweb_bb/views.py                              304    118    61%
+punkweb_bb/widgets.py                             16      0   100%
+------------------------------------------------------------------
+TOTAL                                           1283    203    84%
 ```
```

### Comparing `punkweb_bb-0.2.3/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.3.0/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -51,19 +51,23 @@
 punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
 punkweb_bb/migrations/0003_alter_thread_options.py
 punkweb_bb/migrations/0004_groupstyle.py
+punkweb_bb/migrations/0005_alter_thread_options.py
+punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py
 punkweb_bb/migrations/__init__.py
 punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
+punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc
+punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/static/punkweb_bb/favicon.ico
 punkweb_bb/static/punkweb_bb/css/category-form.css
 punkweb_bb/static/punkweb_bb/css/defaults.css
 punkweb_bb/static/punkweb_bb/css/index.css
 punkweb_bb/static/punkweb_bb/css/login.css
 punkweb_bb/static/punkweb_bb/css/members.css
@@ -79,14 +83,15 @@
 punkweb_bb/static/punkweb_bb/css/thread.css
 punkweb_bb/static/punkweb_bb/css/typography.css
 punkweb_bb/static/punkweb_bb/css/variables.css
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+punkweb_bb/static/punkweb_bb/editor/markdown-editor.js
 punkweb_bb/static/punkweb_bb/img/default-profile-image.png
 punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
 punkweb_bb/static/punkweb_bb/js/shoutbox.js
 punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
 punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
 punkweb_bb/static/punkweb_bb/vendor/open-color.css
 punkweb_bb/static/punkweb_bb/vendor/prism.css
@@ -205,15 +210,71 @@
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.eslintrc.json
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.prettierrc.json
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/babel.config.json
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest-puppeteer.config.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest.config.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_config.yml
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/config.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/server.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/setup.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/index.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/tiny.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/index.css
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/bold.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/clear_formatting.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/code.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h1.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h2.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/hr.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/image.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/italic.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/link.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ol.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/strikethrough.svg
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js
+punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ul.svg
 punkweb_bb/templates/punkweb_bb/base.html
+punkweb_bb/templates/punkweb_bb/base_delete_modal.html
 punkweb_bb/templates/punkweb_bb/base_modal.html
 punkweb_bb/templates/punkweb_bb/bbcode.html
 punkweb_bb/templates/punkweb_bb/category_create.html
 punkweb_bb/templates/punkweb_bb/category_update.html
 punkweb_bb/templates/punkweb_bb/index.html
 punkweb_bb/templates/punkweb_bb/login.html
 punkweb_bb/templates/punkweb_bb/members.html
@@ -228,27 +289,33 @@
 punkweb_bb/templates/punkweb_bb/thread_update.html
 punkweb_bb/templates/punkweb_bb/partials/category_delete.html
 punkweb_bb/templates/punkweb_bb/partials/post_delete.html
 punkweb_bb/templates/punkweb_bb/partials/post_update.html
 punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
 punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
 punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+punkweb_bb/templates/punkweb_bb/partials/thread_move.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+punkweb_bb/templates/punkweb_bb/widgets/markdown-editor.html
 punkweb_bb/templatetags/__init__.py
 punkweb_bb/templatetags/can_delete.py
 punkweb_bb/templatetags/can_edit.py
 punkweb_bb/templatetags/can_post.py
 punkweb_bb/templatetags/humanize_int.py
-punkweb_bb/templatetags/shoutbox_bbcode.py
+punkweb_bb/templatetags/render.py
+punkweb_bb/templatetags/shoutbox_render.py
 punkweb_bb/templatetags/styled_group_name.py
 punkweb_bb/templatetags/styled_username.py
 punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/render.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/shoutbox_render.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
```

### Comparing `punkweb_bb-0.2.3/setup.py` & `punkweb_bb-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.2.3",
+    version="0.3.0",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     include_package_data=True,
     package_data={"": ["README.md"]},
     install_requires=[
         "django>=4.0",
         "django-precise-bbcode",
+        "markdown",
         "expiringdict",
         "pillow",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
```

