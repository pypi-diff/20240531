# Comparing `tmp/punkweb_bb-0.3.0.tar.gz` & `tmp/punkweb_bb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.3.0.tar", last modified: Thu May 30 22:50:22 2024, max compression
+gzip compressed data, was "punkweb_bb-0.4.0.tar", last modified: Fri May 31 08:05:42 2024, max compression
```

## Comparing `punkweb_bb-0.3.0.tar` & `punkweb_bb-0.4.0.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.3.0/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.3.0/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     6172 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     5518 2024-05-30 22:33:15.000000 punkweb_bb-0.3.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.3.0/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3883 2024-05-30 20:51:38.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3605 2024-05-30 22:34:17.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     6735 2024-05-30 20:41:21.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    15480 2024-05-30 20:40:50.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1111 2024-05-30 20:23:01.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1591 2024-05-29 22:23:50.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51701 2024-05-30 22:31:44.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3686 2024-05-30 02:32:29.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2794 2024-05-30 22:36:26.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    26364 2024-05-30 02:49:07.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2640 2024-05-30 22:36:37.000000 punkweb_bb-0.3.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2686 2024-05-30 20:51:37.000000 punkweb_bb-0.3.0/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1414 2024-05-30 22:34:16.000000 punkweb_bb-0.3.0/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.3.0/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.3.0/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.3.0/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     3130 2024-05-30 20:41:20.000000 punkweb_bb-0.3.0/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.3.0/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.3.0/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0003_alter_thread_options.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0004_groupstyle.py
--rw-r--r--   0 pork      (1000) pork      (1000)      638 2024-05-30 02:25:42.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0005_alter_thread_options.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1699 2024-05-30 21:37:11.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      885 2024-05-30 02:25:45.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1901 2024-05-30 21:37:24.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.3.0/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     7053 2024-05-30 20:40:49.000000 punkweb_bb-0.3.0/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.3.0/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.3.0/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.3.0/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      609 2024-05-30 20:14:52.000000 punkweb_bb-0.3.0/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.3.0/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.476752 punkweb_bb-0.3.0/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/category-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     2032 2024-05-30 02:38:15.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-30 21:26:55.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      571 2024-05-30 22:36:33.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/markdown-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.484753 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.488752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/
--rw-r--r--   0 pork      (1000) pork      (1000)      345 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.eslintrc.json
--rw-r--r--   0 pork      (1000) pork      (1000)     1625 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore
--rw-r--r--   0 pork      (1000) pork      (1000)        3 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.prettierrc.json
--rw-r--r--   0 pork      (1000) pork      (1000)     1078 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)    30065 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md
--rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/babel.config.json
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/
--rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3749 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css
--rw-r--r--   0 pork      (1000) pork      (1000)   454032 2024-05-30 22:21:37.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2855 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    50144 2024-05-30 22:21:37.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    41346 2024-05-30 22:21:38.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/
--rw-r--r--   0 pork      (1000) pork      (1000)       26 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_config.yml
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/
--rw-r--r--   0 pork      (1000) pork      (1000)     2333 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html
--rw-r--r--   0 pork      (1000) pork      (1000)     6061 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md
--rw-r--r--   0 pork      (1000) pork      (1000)     2919 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts
--rw-r--r--   0 pork      (1000) pork      (1000)     5976 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/
--rw-r--r--   0 pork      (1000) pork      (1000)    24077 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4321 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js
--rw-r--r--   0 pork      (1000) pork      (1000)    20160 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1284 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js
--rw-r--r--   0 pork      (1000) pork      (1000)     5645 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/
--rw-r--r--   0 pork      (1000) pork      (1000)       40 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/config.js
--rw-r--r--   0 pork      (1000) pork      (1000)      300 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/server.js
--rw-r--r--   0 pork      (1000) pork      (1000)       23 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/setup.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3506 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js
--rw-r--r--   0 pork      (1000) pork      (1000)      141 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest-puppeteer.config.js
--rw-r--r--   0 pork      (1000) pork      (1000)      226 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest.config.js
--rw-r--r--   0 pork      (1000) pork      (1000)   602599 2024-05-30 20:58:03.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json
--rw-r--r--   0 pork      (1000) pork      (1000)     1983 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/
--rw-r--r--   0 pork      (1000) pork      (1000)    69517 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8504 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/
--rw-r--r--   0 pork      (1000) pork      (1000)     1494 2024-05-30 22:21:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)     2218 2024-05-30 21:33:47.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)       48 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)    16351 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/
--rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html
--rw-r--r--   0 pork      (1000) pork      (1000)      107 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/index.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/
--rw-r--r--   0 pork      (1000) pork      (1000)      557 2024-05-30 21:15:44.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      351 2024-05-30 21:10:59.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/bold.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      230 2024-05-30 21:13:22.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/clear_formatting.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 21:13:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/code.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      215 2024-05-30 21:13:44.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h1.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      305 2024-05-30 21:13:54.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h2.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      149 2024-05-30 21:14:11.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/hr.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      327 2024-05-30 21:14:18.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/image.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      192 2024-05-30 21:14:25.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/italic.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      380 2024-05-30 21:14:32.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/link.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:14:50.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ol.svg
--rw-r--r--   0 pork      (1000) pork      (1000)      214 2024-05-30 21:15:26.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/strikethrough.svg
--rw-r--r--   0 pork      (1000) pork      (1000)     4350 2024-05-30 22:21:36.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js
--rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:15:12.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ul.svg
--rw-r--r--   0 pork      (1000) pork      (1000)       49 2024-05-30 20:56:51.000000 punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/tiny.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.476752 punkweb_bb-0.3.0/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      422 2024-05-30 02:43:33.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base_delete_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10519 2024-05-30 22:46:56.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2886 2024-05-29 22:07:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-05-30 02:46:54.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      216 2024-05-30 02:45:15.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      220 2024-05-30 02:45:33.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      246 2024-05-30 02:45:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      224 2024-05-30 02:43:57.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      746 2024-05-30 02:36:40.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/thread_move.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3203 2024-05-30 22:47:03.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-05-30 22:47:12.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     5893 2024-05-30 02:20:28.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    11201 2024-05-30 22:46:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-30 21:41:52.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-30 21:41:47.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.492752 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/widgets/
--rw-r--r--   0 pork      (1000) pork      (1000)       99 2024-05-30 22:19:14.000000 punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/widgets/markdown-editor.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1858 2024-05-30 20:32:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2478 2024-05-30 22:08:38.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/render.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      945 2024-05-30 21:47:56.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1255 2024-05-30 22:35:40.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/shoutbox_render.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 21:01:58.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_delete.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_edit.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/can_post.py
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1194 2024-05-30 22:08:37.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/render.py
--rw-r--r--   0 pork      (1000) pork      (1000)      591 2024-05-30 22:35:38.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/shoutbox_render.py
--rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 21:01:50.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/styled_group_name.py
--rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.3.0/punkweb_bb/templatetags/styled_username.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26298 2024-05-30 22:31:43.000000 punkweb_bb-0.3.0/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2673 2024-05-30 02:32:28.000000 punkweb_bb-0.3.0/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1651 2024-05-30 22:36:26.000000 punkweb_bb-0.3.0/punkweb_bb/utils.py
--rw-r--r--   0 pork      (1000) pork      (1000)    18191 2024-05-30 02:49:06.000000 punkweb_bb-0.3.0/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1502 2024-05-30 22:36:36.000000 punkweb_bb-0.3.0/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-30 22:50:22.480752 punkweb_bb-0.3.0/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     6172 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    19738 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       63 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-30 22:50:22.000000 punkweb_bb-0.3.0/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-30 22:50:22.496752 punkweb_bb-0.3.0/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1030 2024-05-30 22:48:58.000000 punkweb_bb-0.3.0/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.4.0/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)      154 2024-05-31 07:23:06.000000 punkweb_bb-0.4.0/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     5831 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     5177 2024-05-31 07:17:22.000000 punkweb_bb-0.4.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.317769 punkweb_bb-0.4.0/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.4.0/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3810 2024-05-31 06:59:50.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3605 2024-05-31 06:59:53.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6638 2024-05-31 06:57:19.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6735 2024-05-31 07:00:11.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-31 07:00:18.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-05-31 07:00:22.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    15480 2024-05-31 07:00:24.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-05-31 07:00:28.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      160 2024-05-31 02:41:33.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-05-31 07:00:31.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1109 2024-05-31 07:00:34.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-05-31 07:00:35.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1591 2024-05-29 22:23:50.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1052 2024-05-31 05:57:58.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51701 2024-05-31 07:01:04.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3686 2024-05-31 07:00:42.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2823 2024-05-31 07:00:44.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    26263 2024-05-31 07:59:22.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2640 2024-05-31 07:00:54.000000 punkweb_bb-0.4.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2640 2024-05-31 06:59:50.000000 punkweb_bb-0.4.0/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1414 2024-05-31 06:59:53.000000 punkweb_bb-0.4.0/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.4.0/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4983 2024-05-31 06:57:18.000000 punkweb_bb-0.4.0/punkweb_bb/bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.4.0/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     3130 2024-05-31 07:00:10.000000 punkweb_bb-0.4.0/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.4.0/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-31 07:00:17.000000 punkweb_bb-0.4.0/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0003_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0004_groupstyle.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      638 2024-05-30 02:25:42.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0005_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1699 2024-05-30 21:37:11.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      885 2024-05-30 02:25:45.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1901 2024-05-30 21:37:24.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-05-31 07:00:21.000000 punkweb_bb-0.4.0/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     7053 2024-05-31 07:00:23.000000 punkweb_bb-0.4.0/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-05-31 07:00:28.000000 punkweb_bb-0.4.0/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-05-31 07:00:30.000000 punkweb_bb-0.4.0/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      605 2024-05-31 07:00:33.000000 punkweb_bb-0.4.0/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-05-31 07:00:35.000000 punkweb_bb-0.4.0/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.317769 punkweb_bb-0.4.0/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-05-31 07:27:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-05-31 07:55:45.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-31 07:36:33.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-05-31 07:30:00.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     2032 2024-05-31 07:53:00.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-30 21:26:55.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1435 2024-05-31 07:50:39.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      473 2024-05-31 07:46:32.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1061 2024-05-31 07:54:16.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/markdown-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.321769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.325769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)      345 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.eslintrc.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1625 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore
+-rw-r--r--   0 pork      (1000) pork      (1000)        3 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.prettierrc.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1078 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)    30065 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md
+-rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/babel.config.json
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/
+-rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3749 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   454032 2024-05-31 07:20:05.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2855 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    50144 2024-05-31 07:20:05.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    41346 2024-05-31 07:20:06.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/
+-rw-r--r--   0 pork      (1000) pork      (1000)       26 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_config.yml
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/
+-rw-r--r--   0 pork      (1000) pork      (1000)     2333 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     6061 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md
+-rw-r--r--   0 pork      (1000) pork      (1000)     2919 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts
+-rw-r--r--   0 pork      (1000) pork      (1000)     5976 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/
+-rw-r--r--   0 pork      (1000) pork      (1000)    24077 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4321 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    20160 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1284 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     5645 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/
+-rw-r--r--   0 pork      (1000) pork      (1000)       40 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      300 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/server.js
+-rw-r--r--   0 pork      (1000) pork      (1000)       23 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/setup.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3506 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      141 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest-puppeteer.config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      226 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest.config.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   602599 2024-05-31 07:19:44.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json
+-rw-r--r--   0 pork      (1000) pork      (1000)     1983 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/
+-rw-r--r--   0 pork      (1000) pork      (1000)    69517 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8504 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1494 2024-05-30 22:21:32.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     2218 2024-05-30 21:33:47.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)       48 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    16351 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.329769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/
+-rw-r--r--   0 pork      (1000) pork      (1000)      515 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3770 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      107 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/index.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/
+-rw-r--r--   0 pork      (1000) pork      (1000)      557 2024-05-30 21:15:44.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      351 2024-05-30 21:10:59.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/bold.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      230 2024-05-30 21:13:22.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/clear_formatting.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      228 2024-05-30 21:13:32.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/code.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      215 2024-05-30 21:13:44.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h1.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      305 2024-05-30 21:13:54.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/h2.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      149 2024-05-30 21:14:11.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/hr.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      327 2024-05-30 21:14:18.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/image.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      192 2024-05-30 21:14:25.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/italic.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      380 2024-05-30 21:14:32.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/link.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:14:50.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ol.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)      214 2024-05-30 21:15:26.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/strikethrough.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)     4350 2024-05-31 07:20:04.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      495 2024-05-30 21:15:12.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/ul.svg
+-rw-r--r--   0 pork      (1000) pork      (1000)       49 2024-05-30 20:56:51.000000 punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/tiny.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.317769 punkweb_bb-0.4.0/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      422 2024-05-30 02:43:33.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/base_delete_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      390 2024-05-31 06:24:23.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10519 2024-05-31 02:33:21.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2886 2024-05-29 22:07:52.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-05-30 02:46:54.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      216 2024-05-30 02:45:15.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      220 2024-05-30 02:45:33.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      246 2024-05-30 02:45:52.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      224 2024-05-30 02:43:57.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      746 2024-05-30 02:36:40.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/thread_move.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3203 2024-05-30 22:47:03.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-05-31 05:24:25.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5893 2024-05-30 02:20:28.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    11201 2024-05-30 22:46:47.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-30 21:41:52.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-30 21:41:47.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/widgets/
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-05-31 07:40:20.000000 punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/widgets/markdown-editor.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1858 2024-05-30 20:32:58.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1880 2024-05-31 08:02:01.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/render.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      945 2024-05-30 21:47:56.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-05-31 02:47:37.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/shoutbox_render.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 21:01:58.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-05-31 08:02:00.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/render.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 21:01:50.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/styled_group_name.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.4.0/punkweb_bb/templatetags/styled_username.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26298 2024-05-31 07:00:38.000000 punkweb_bb-0.4.0/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2673 2024-05-31 07:00:41.000000 punkweb_bb-0.4.0/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1568 2024-05-31 07:00:44.000000 punkweb_bb-0.4.0/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    18010 2024-05-31 07:59:21.000000 punkweb_bb-0.4.0/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1502 2024-05-31 07:00:53.000000 punkweb_bb-0.4.0/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-31 08:05:42.317769 punkweb_bb-0.4.0/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     5831 2024-05-31 08:05:41.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    19758 2024-05-31 08:05:42.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-31 08:05:41.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       48 2024-05-31 08:05:41.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-31 08:05:41.000000 punkweb_bb-0.4.0/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-31 08:05:42.333769 punkweb_bb-0.4.0/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1015 2024-05-31 08:05:25.000000 punkweb_bb-0.4.0/setup.py
```

### Comparing `punkweb_bb-0.3.0/LICENSE` & `punkweb_bb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/PKG-INFO` & `punkweb_bb-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.3.0
+Version: 0.4.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,69 +16,61 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
-This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
-
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
-- [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
-- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
+- [bbcode](https://pypi.org/project/bbcode/)
+- [Markdown](https://pypi.org/project/Markdown/)
 - [SCEditor](https://www.sceditor.com/)
 - [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
 - Django 4.0+
-- django-precise-bbcode 1.2+
-- markdown 3.6+
-- Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## BBCode or Markdown?
 
-PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which parser you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
 
-BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+BBCode is the default parser, but you can switch to Markdown by setting the following in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
-  "RENDERER": "markdown",
+  "PARSER": "markdown",
 }
 ```
 
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
-Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
+Add `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
 
 ```python
 INSTALLED_APPS = [
     ...
-    "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
-
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
         "OPTIONS": {
@@ -112,15 +104,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
-  "RENDERER": "bbcode", # "bbcode" or "markdown"
+  "PARSER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
```

### Comparing `punkweb_bb-0.3.0/README.md` & `punkweb_bb-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
-This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
-
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
-- [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
-- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
+- [bbcode](https://pypi.org/project/bbcode/)
+- [Markdown](https://pypi.org/project/Markdown/)
 - [SCEditor](https://www.sceditor.com/)
 - [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
 - Django 4.0+
-- django-precise-bbcode 1.2+
-- markdown 3.6+
-- Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## BBCode or Markdown?
 
-PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which parser you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
 
-BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+BBCode is the default parser, but you can switch to Markdown by setting the following in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
-  "RENDERER": "markdown",
+  "PARSER": "markdown",
 }
 ```
 
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
-Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
+Add `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
 
 ```python
 INSTALLED_APPS = [
     ...
-    "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
-
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
         "OPTIONS": {
@@ -94,15 +86,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
-  "RENDERER": "bbcode", # "bbcode" or "markdown"
+  "PARSER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,276 +1,268 @@
 magic:    0xa70d0d0a
-moddate:  0xd9e65866 (Thu May 30 20:51:37 2024 UTC)
-files sz: 2686
+moddate:  0x66755966 (Fri May 31 06:59:50 2024 UTC)
+files sz: 2640
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a056d065a066d075a076d085a086d095a096d0a5a0a010064
-      0064046c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d
-      125a120100020065016a130000000000000000650ca6010000ab01000000
-      00000000000200470064058400640665016a140000000000000000a60300
-      00ab030000000000000000a6000000ab0000000000000000005a15020065
-      016a130000000000000000650da6010000ab010000000000000000020047
-      0064078400640865016a140000000000000000a6030000ab030000000000
-      000000a6000000ab0000000000000000005a16020065016a130000000000
-      0000006511a6010000ab0100000000000000000200470064098400640a65
-      016a140000000000000000a6030000ab030000000000000000a6000000ab
-      0000000000000000005a17020065016a1300000000000000006512a60100
-      00ab01000000000000000002004700640b8400640c65016a140000000000
-      000000a6030000ab030000000000000000a6000000ab0000000000000000
-      005a18020065016a130000000000000000650fa6010000ab010000000000
-      00000002004700640d8400640e65016a140000000000000000a6030000ab
-      030000000000000000a6000000ab0000000000000000005a19020065016a
-      1300000000000000006510a6010000ab0100000000000000000200470064
-      0f8400641065016a140000000000000000a6030000ab0300000000000000
-      00a6000000ab0000000000000000005a1a020065016a1300000000000000
-      00650ea6010000ab0100000000000000000200470064118400641265016a
-      140000000000000000a6030000ab030000000000000000a6000000ab0000
-      000000000000005a1b64135300
+      0x9700640064016c006d015a010100640064026c026d035a036d045a046d
+      055a056d065a066d075a076d085a080100640064036c096d0a5a0a6d0b5a
+      0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a100100020065016a1100
+      00000000000000650aa6010000ab01000000000000000002004700640484
+      00640565016a120000000000000000a6030000ab030000000000000000a6
+      000000ab0000000000000000005a13020065016a11000000000000000065
+      0ba6010000ab0100000000000000000200470064068400640765016a1200
+      00000000000000a6030000ab030000000000000000a6000000ab00000000
+      00000000005a14020065016a110000000000000000650fa6010000ab0100
+      000000000000000200470064088400640965016a120000000000000000a6
+      030000ab030000000000000000a6000000ab0000000000000000005a1502
+      0065016a1100000000000000006510a6010000ab01000000000000000002
+      004700640a8400640b65016a120000000000000000a6030000ab03000000
+      0000000000a6000000ab0000000000000000005a16020065016a11000000
+      0000000000650da6010000ab01000000000000000002004700640c840064
+      0d65016a120000000000000000a6030000ab030000000000000000a60000
+      00ab0000000000000000005a17020065016a110000000000000000650ea6
+      010000ab01000000000000000002004700640e8400640f65016a12000000
+      0000000000a6030000ab030000000000000000a6000000ab000000000000
+      0000005a18020065016a110000000000000000650ca6010000ab01000000
+      00000000000200470064108400641165016a120000000000000000a60300
+      00ab030000000000000000a6000000ab0000000000000000005a19641253
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('admin',))
                  6 IMPORT_NAME              0 (django.contrib)
                  8 IMPORT_FROM              1 (admin)
                 10 STORE_NAME               1 (admin)
                 12 POP_TOP
    
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('mark_safe',))
-                18 IMPORT_NAME              2 (django.utils.safestring)
-                20 IMPORT_FROM              3 (mark_safe)
-                22 STORE_NAME               3 (mark_safe)
-                24 POP_TOP
-   
-     4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm'))
-                30 IMPORT_NAME              4 (punkweb_bb.admin_forms)
-                32 IMPORT_FROM              5 (BoardProfileAdminModelForm)
-                34 STORE_NAME               5 (BoardProfileAdminModelForm)
-                36 IMPORT_FROM              6 (CategoryAdminModelForm)
-                38 STORE_NAME               6 (CategoryAdminModelForm)
-                40 IMPORT_FROM              7 (GroupStyleAdminModelForm)
-                42 STORE_NAME               7 (GroupStyleAdminModelForm)
-                44 IMPORT_FROM              8 (PostAdminModelForm)
-                46 STORE_NAME               8 (PostAdminModelForm)
-                48 IMPORT_FROM              9 (SubcategoryAdminModelForm)
-                50 STORE_NAME               9 (SubcategoryAdminModelForm)
-                52 IMPORT_FROM             10 (ThreadAdminModelForm)
-                54 STORE_NAME              10 (ThreadAdminModelForm)
-                56 POP_TOP
-   
-    12          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               4 (('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread'))
-                62 IMPORT_NAME             11 (punkweb_bb.models)
-                64 IMPORT_FROM             12 (BoardProfile)
-                66 STORE_NAME              12 (BoardProfile)
-                68 IMPORT_FROM             13 (Category)
-                70 STORE_NAME              13 (Category)
-                72 IMPORT_FROM             14 (GroupStyle)
-                74 STORE_NAME              14 (GroupStyle)
-                76 IMPORT_FROM             15 (Post)
-                78 STORE_NAME              15 (Post)
-                80 IMPORT_FROM             16 (Shout)
-                82 STORE_NAME              16 (Shout)
-                84 IMPORT_FROM             17 (Subcategory)
-                86 STORE_NAME              17 (Subcategory)
-                88 IMPORT_FROM             18 (Thread)
-                90 STORE_NAME              18 (Thread)
-                92 POP_TOP
-   
-    23          94 PUSH_NULL
-                96 LOAD_NAME                1 (admin)
-                98 LOAD_ATTR               19 (register)
-               108 LOAD_NAME               12 (BoardProfile)
-               110 PRECALL                  1
-               114 CALL                     1
-   
-    24         124 PUSH_NULL
-               126 LOAD_BUILD_CLASS
-               128 LOAD_CONST               5 (<code object BoardProfileModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 23>)
-               130 MAKE_FUNCTION            0
-               132 LOAD_CONST               6 ('BoardProfileModelAdmin')
-               134 LOAD_NAME                1 (admin)
-               136 LOAD_ATTR               20 (ModelAdmin)
-               146 PRECALL                  3
-               150 CALL                     3
-   
-    23         160 PRECALL                  0
-               164 CALL                     0
-   
-    24         174 STORE_NAME              21 (BoardProfileModelAdmin)
-   
-    39         176 PUSH_NULL
-               178 LOAD_NAME                1 (admin)
-               180 LOAD_ATTR               19 (register)
-               190 LOAD_NAME               13 (Category)
-               192 PRECALL                  1
-               196 CALL                     1
-   
-    40         206 PUSH_NULL
-               208 LOAD_BUILD_CLASS
-               210 LOAD_CONST               7 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 39>)
-               212 MAKE_FUNCTION            0
-               214 LOAD_CONST               8 ('CategoryModelAdmin')
-               216 LOAD_NAME                1 (admin)
-               218 LOAD_ATTR               20 (ModelAdmin)
-               228 PRECALL                  3
-               232 CALL                     3
-   
-    39         242 PRECALL                  0
-               246 CALL                     0
-   
-    40         256 STORE_NAME              22 (CategoryModelAdmin)
-   
-    53         258 PUSH_NULL
-               260 LOAD_NAME                1 (admin)
-               262 LOAD_ATTR               19 (register)
-               272 LOAD_NAME               17 (Subcategory)
-               274 PRECALL                  1
-               278 CALL                     1
-   
-    54         288 PUSH_NULL
-               290 LOAD_BUILD_CLASS
-               292 LOAD_CONST               9 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 53>)
-               294 MAKE_FUNCTION            0
-               296 LOAD_CONST              10 ('SubcategoryModelAdmin')
-               298 LOAD_NAME                1 (admin)
-               300 LOAD_ATTR               20 (ModelAdmin)
-               310 PRECALL                  3
-               314 CALL                     3
-   
-    53         324 PRECALL                  0
-               328 CALL                     0
-   
-    54         338 STORE_NAME              23 (SubcategoryModelAdmin)
-   
-    69         340 PUSH_NULL
-               342 LOAD_NAME                1 (admin)
-               344 LOAD_ATTR               19 (register)
-               354 LOAD_NAME               18 (Thread)
-               356 PRECALL                  1
-               360 CALL                     1
-   
-    70         370 PUSH_NULL
-               372 LOAD_BUILD_CLASS
-               374 LOAD_CONST              11 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 69>)
-               376 MAKE_FUNCTION            0
-               378 LOAD_CONST              12 ('ThreadModelAdmin')
-               380 LOAD_NAME                1 (admin)
-               382 LOAD_ATTR               20 (ModelAdmin)
-               392 PRECALL                  3
-               396 CALL                     3
-   
-    69         406 PRECALL                  0
-               410 CALL                     0
-   
-    70         420 STORE_NAME              24 (ThreadModelAdmin)
-   
-    96         422 PUSH_NULL
-               424 LOAD_NAME                1 (admin)
-               426 LOAD_ATTR               19 (register)
-               436 LOAD_NAME               15 (Post)
-               438 PRECALL                  1
-               442 CALL                     1
-   
-    97         452 PUSH_NULL
-               454 LOAD_BUILD_CLASS
-               456 LOAD_CONST              13 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 96>)
-               458 MAKE_FUNCTION            0
-               460 LOAD_CONST              14 ('PostModelAdmin')
-               462 LOAD_NAME                1 (admin)
-               464 LOAD_ATTR               20 (ModelAdmin)
-               474 PRECALL                  3
-               478 CALL                     3
-   
-    96         488 PRECALL                  0
-               492 CALL                     0
-   
-    97         502 STORE_NAME              25 (PostModelAdmin)
-   
-   111         504 PUSH_NULL
-               506 LOAD_NAME                1 (admin)
-               508 LOAD_ATTR               19 (register)
-               518 LOAD_NAME               16 (Shout)
-               520 PRECALL                  1
-               524 CALL                     1
-   
-   112         534 PUSH_NULL
-               536 LOAD_BUILD_CLASS
-               538 LOAD_CONST              15 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 111>)
-               540 MAKE_FUNCTION            0
-               542 LOAD_CONST              16 ('ShoutModelAdmin')
-               544 LOAD_NAME                1 (admin)
-               546 LOAD_ATTR               20 (ModelAdmin)
-               556 PRECALL                  3
-               560 CALL                     3
-   
-   111         570 PRECALL                  0
-               574 CALL                     0
-   
-   112         584 STORE_NAME              26 (ShoutModelAdmin)
-   
-   124         586 PUSH_NULL
-               588 LOAD_NAME                1 (admin)
-               590 LOAD_ATTR               19 (register)
-               600 LOAD_NAME               14 (GroupStyle)
-               602 PRECALL                  1
-               606 CALL                     1
-   
-   125         616 PUSH_NULL
-               618 LOAD_BUILD_CLASS
-               620 LOAD_CONST              17 (<code object GroupStyleModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 124>)
-               622 MAKE_FUNCTION            0
-               624 LOAD_CONST              18 ('GroupStyleModelAdmin')
-               626 LOAD_NAME                1 (admin)
-               628 LOAD_ATTR               20 (ModelAdmin)
-               638 PRECALL                  3
-               642 CALL                     3
-   
-   124         652 PRECALL                  0
-               656 CALL                     0
-   
-   125         666 STORE_NAME              27 (GroupStyleModelAdmin)
-               668 LOAD_CONST              19 (None)
-               670 RETURN_VALUE
+     3          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm'))
+                18 IMPORT_NAME              2 (punkweb_bb.admin_forms)
+                20 IMPORT_FROM              3 (BoardProfileAdminModelForm)
+                22 STORE_NAME               3 (BoardProfileAdminModelForm)
+                24 IMPORT_FROM              4 (CategoryAdminModelForm)
+                26 STORE_NAME               4 (CategoryAdminModelForm)
+                28 IMPORT_FROM              5 (GroupStyleAdminModelForm)
+                30 STORE_NAME               5 (GroupStyleAdminModelForm)
+                32 IMPORT_FROM              6 (PostAdminModelForm)
+                34 STORE_NAME               6 (PostAdminModelForm)
+                36 IMPORT_FROM              7 (SubcategoryAdminModelForm)
+                38 STORE_NAME               7 (SubcategoryAdminModelForm)
+                40 IMPORT_FROM              8 (ThreadAdminModelForm)
+                42 STORE_NAME               8 (ThreadAdminModelForm)
+                44 POP_TOP
+   
+    11          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               3 (('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread'))
+                50 IMPORT_NAME              9 (punkweb_bb.models)
+                52 IMPORT_FROM             10 (BoardProfile)
+                54 STORE_NAME              10 (BoardProfile)
+                56 IMPORT_FROM             11 (Category)
+                58 STORE_NAME              11 (Category)
+                60 IMPORT_FROM             12 (GroupStyle)
+                62 STORE_NAME              12 (GroupStyle)
+                64 IMPORT_FROM             13 (Post)
+                66 STORE_NAME              13 (Post)
+                68 IMPORT_FROM             14 (Shout)
+                70 STORE_NAME              14 (Shout)
+                72 IMPORT_FROM             15 (Subcategory)
+                74 STORE_NAME              15 (Subcategory)
+                76 IMPORT_FROM             16 (Thread)
+                78 STORE_NAME              16 (Thread)
+                80 POP_TOP
+   
+    22          82 PUSH_NULL
+                84 LOAD_NAME                1 (admin)
+                86 LOAD_ATTR               17 (register)
+                96 LOAD_NAME               10 (BoardProfile)
+                98 PRECALL                  1
+               102 CALL                     1
+   
+    23         112 PUSH_NULL
+               114 LOAD_BUILD_CLASS
+               116 LOAD_CONST               4 (<code object BoardProfileModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 22>)
+               118 MAKE_FUNCTION            0
+               120 LOAD_CONST               5 ('BoardProfileModelAdmin')
+               122 LOAD_NAME                1 (admin)
+               124 LOAD_ATTR               18 (ModelAdmin)
+               134 PRECALL                  3
+               138 CALL                     3
+   
+    22         148 PRECALL                  0
+               152 CALL                     0
+   
+    23         162 STORE_NAME              19 (BoardProfileModelAdmin)
+   
+    38         164 PUSH_NULL
+               166 LOAD_NAME                1 (admin)
+               168 LOAD_ATTR               17 (register)
+               178 LOAD_NAME               11 (Category)
+               180 PRECALL                  1
+               184 CALL                     1
+   
+    39         194 PUSH_NULL
+               196 LOAD_BUILD_CLASS
+               198 LOAD_CONST               6 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 38>)
+               200 MAKE_FUNCTION            0
+               202 LOAD_CONST               7 ('CategoryModelAdmin')
+               204 LOAD_NAME                1 (admin)
+               206 LOAD_ATTR               18 (ModelAdmin)
+               216 PRECALL                  3
+               220 CALL                     3
+   
+    38         230 PRECALL                  0
+               234 CALL                     0
+   
+    39         244 STORE_NAME              20 (CategoryModelAdmin)
+   
+    52         246 PUSH_NULL
+               248 LOAD_NAME                1 (admin)
+               250 LOAD_ATTR               17 (register)
+               260 LOAD_NAME               15 (Subcategory)
+               262 PRECALL                  1
+               266 CALL                     1
+   
+    53         276 PUSH_NULL
+               278 LOAD_BUILD_CLASS
+               280 LOAD_CONST               8 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 52>)
+               282 MAKE_FUNCTION            0
+               284 LOAD_CONST               9 ('SubcategoryModelAdmin')
+               286 LOAD_NAME                1 (admin)
+               288 LOAD_ATTR               18 (ModelAdmin)
+               298 PRECALL                  3
+               302 CALL                     3
+   
+    52         312 PRECALL                  0
+               316 CALL                     0
+   
+    53         326 STORE_NAME              21 (SubcategoryModelAdmin)
+   
+    68         328 PUSH_NULL
+               330 LOAD_NAME                1 (admin)
+               332 LOAD_ATTR               17 (register)
+               342 LOAD_NAME               16 (Thread)
+               344 PRECALL                  1
+               348 CALL                     1
+   
+    69         358 PUSH_NULL
+               360 LOAD_BUILD_CLASS
+               362 LOAD_CONST              10 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 68>)
+               364 MAKE_FUNCTION            0
+               366 LOAD_CONST              11 ('ThreadModelAdmin')
+               368 LOAD_NAME                1 (admin)
+               370 LOAD_ATTR               18 (ModelAdmin)
+               380 PRECALL                  3
+               384 CALL                     3
+   
+    68         394 PRECALL                  0
+               398 CALL                     0
+   
+    69         408 STORE_NAME              22 (ThreadModelAdmin)
+   
+    95         410 PUSH_NULL
+               412 LOAD_NAME                1 (admin)
+               414 LOAD_ATTR               17 (register)
+               424 LOAD_NAME               13 (Post)
+               426 PRECALL                  1
+               430 CALL                     1
+   
+    96         440 PUSH_NULL
+               442 LOAD_BUILD_CLASS
+               444 LOAD_CONST              12 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 95>)
+               446 MAKE_FUNCTION            0
+               448 LOAD_CONST              13 ('PostModelAdmin')
+               450 LOAD_NAME                1 (admin)
+               452 LOAD_ATTR               18 (ModelAdmin)
+               462 PRECALL                  3
+               466 CALL                     3
+   
+    95         476 PRECALL                  0
+               480 CALL                     0
+   
+    96         490 STORE_NAME              23 (PostModelAdmin)
+   
+   110         492 PUSH_NULL
+               494 LOAD_NAME                1 (admin)
+               496 LOAD_ATTR               17 (register)
+               506 LOAD_NAME               14 (Shout)
+               508 PRECALL                  1
+               512 CALL                     1
+   
+   111         522 PUSH_NULL
+               524 LOAD_BUILD_CLASS
+               526 LOAD_CONST              14 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 110>)
+               528 MAKE_FUNCTION            0
+               530 LOAD_CONST              15 ('ShoutModelAdmin')
+               532 LOAD_NAME                1 (admin)
+               534 LOAD_ATTR               18 (ModelAdmin)
+               544 PRECALL                  3
+               548 CALL                     3
+   
+   110         558 PRECALL                  0
+               562 CALL                     0
+   
+   111         572 STORE_NAME              24 (ShoutModelAdmin)
+   
+   123         574 PUSH_NULL
+               576 LOAD_NAME                1 (admin)
+               578 LOAD_ATTR               17 (register)
+               588 LOAD_NAME               12 (GroupStyle)
+               590 PRECALL                  1
+               594 CALL                     1
+   
+   124         604 PUSH_NULL
+               606 LOAD_BUILD_CLASS
+               608 LOAD_CONST              16 (<code object GroupStyleModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 123>)
+               610 MAKE_FUNCTION            0
+               612 LOAD_CONST              17 ('GroupStyleModelAdmin')
+               614 LOAD_NAME                1 (admin)
+               616 LOAD_ATTR               18 (ModelAdmin)
+               626 PRECALL                  3
+               630 CALL                     3
+   
+   123         640 PRECALL                  0
+               644 CALL                     0
+   
+   124         654 STORE_NAME              25 (GroupStyleModelAdmin)
+               656 LOAD_CONST              18 (None)
+               658 RETURN_VALUE
    consts
       0
       ('admin',)
-      ('mark_safe',)
       ('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm')
       ('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a07640453
             00
-          23           0 RESUME                   0
+          22           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfileModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          25          10 LOAD_NAME                3 (BoardProfileAdminModelForm)
+          24          10 LOAD_NAME                3 (BoardProfileAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          26          14 LOAD_CONST               1 (('user',))
+          25          14 LOAD_CONST               1 (('user',))
                       16 STORE_NAME               5 (list_display)
          
-          27          18 LOAD_CONST               2 (('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser'))
+          26          18 LOAD_CONST               2 (('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser'))
                       20 STORE_NAME               6 (list_filter)
          
-          33          22 LOAD_CONST               3 (('user__username', 'user__email'))
+          32          22 LOAD_CONST               3 (('user__username', 'user__email'))
                       24 STORE_NAME               7 (search_fields)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'BoardProfileModelAdmin'
             ('user',)
             ('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser')
@@ -278,41 +270,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'BoardProfileAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'BoardProfileModelAdmin'
-         firstlineno 23
+         firstlineno 22
          lnotab 0x0a02040104010406
       'BoardProfileModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a066403640469015a
             0764055300
-          39           0 RESUME                   0
+          38           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          41          10 LOAD_NAME                3 (CategoryAdminModelForm)
+          40          10 LOAD_NAME                3 (CategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          42          14 LOAD_CONST               1 (('name', 'order'))
+          41          14 LOAD_CONST               1 (('name', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          46          18 LOAD_CONST               2 (('name', 'description'))
+          45          18 LOAD_CONST               2 (('name', 'description'))
                       20 STORE_NAME               6 (search_fields)
          
-          50          22 LOAD_CONST               3 ('slug')
+          49          22 LOAD_CONST               3 ('slug')
                       24 LOAD_CONST               4 (('name',))
                       26 BUILD_MAP                1
                       28 STORE_NAME               7 (prepopulated_fields)
                       30 LOAD_CONST               5 (None)
                       32 RETURN_VALUE
          consts
             'CategoryModelAdmin'
@@ -323,44 +315,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'CategoryAdminModelForm', 'form', 'list_display', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'CategoryModelAdmin'
-         firstlineno 39
+         firstlineno 38
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
-          53           0 RESUME                   0
+          52           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SubcategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          55          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
+          54          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          56          14 LOAD_CONST               1 (('name', 'category', 'order'))
+          55          14 LOAD_CONST               1 (('name', 'category', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          61          18 LOAD_CONST               2 (('category',))
+          60          18 LOAD_CONST               2 (('category',))
                       20 STORE_NAME               6 (list_filter)
          
-          62          22 LOAD_CONST               3 (('name', 'description'))
+          61          22 LOAD_CONST               3 (('name', 'description'))
                       24 STORE_NAME               7 (search_fields)
          
-          66          26 LOAD_CONST               4 ('slug')
+          65          26 LOAD_CONST               4 ('slug')
                       28 LOAD_CONST               5 (('name',))
                       30 BUILD_MAP                1
                       32 STORE_NAME               8 (prepopulated_fields)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'SubcategoryModelAdmin'
@@ -372,41 +364,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'SubcategoryAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'SubcategoryModelAdmin'
-         firstlineno 53
+         firstlineno 52
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
-          69           0 RESUME                   0
+          68           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          71          10 LOAD_NAME                3 (ThreadAdminModelForm)
+          70          10 LOAD_NAME                3 (ThreadAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          72          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          71          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       16 STORE_NAME               5 (list_display)
          
-          81          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          80          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       20 STORE_NAME               6 (list_filter)
          
-          88          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
+          87          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
                       24 STORE_NAME               7 (search_fields)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'ThreadModelAdmin'
             ('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
             ('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
@@ -414,127 +406,127 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'ThreadAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'ThreadModelAdmin'
-         firstlineno 69
+         firstlineno 68
          lnotab 0x0a02040104090407
       'ThreadModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0265035a0464015a0564025a0664035300
-          96           0 RESUME                   0
+          95           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          98          10 LOAD_NAME                3 (PostAdminModelForm)
+          97          10 LOAD_NAME                3 (PostAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          99          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
+          98          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
                       16 STORE_NAME               5 (list_display)
          
-         104          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         103          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
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
-         firstlineno 96
+         firstlineno 95
          lnotab 0x0a0204010405
       'PostModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a0464035300
-         111           0 RESUME                   0
+         110           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ShoutModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         113          10 LOAD_CONST               1 (('user', 'created_at'))
+         112          10 LOAD_CONST               1 (('user', 'created_at'))
                       12 STORE_NAME               3 (list_display)
          
-         117          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         116          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
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
-         firstlineno 111
+         firstlineno 110
          lnotab 0x0a020404
       'ShoutModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0265035a0464015a0564025a0664035300
-         124           0 RESUME                   0
+         123           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupStyleModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         126          10 LOAD_NAME                3 (GroupStyleAdminModelForm)
+         125          10 LOAD_NAME                3 (GroupStyleAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-         127          14 LOAD_CONST               1 (('group', 'priority'))
+         126          14 LOAD_CONST               1 (('group', 'priority'))
                       16 STORE_NAME               5 (list_display)
          
-         131          18 LOAD_CONST               2 (('group__name', 'username_style'))
+         130          18 LOAD_CONST               2 (('group__name', 'username_style'))
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
-         firstlineno 124
+         firstlineno 123
          lnotab 0x0a0204010404
       'GroupStyleModelAdmin'
       None
-   names      ('django.contrib', 'admin', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.admin_forms', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread', 'register', 'ModelAdmin', 'BoardProfileModelAdmin', 'CategoryModelAdmin', 'SubcategoryModelAdmin', 'ThreadModelAdmin', 'PostModelAdmin', 'ShoutModelAdmin', 'GroupStyleModelAdmin')
+   names      ('django.contrib', 'admin', 'punkweb_bb.admin_forms', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread', 'register', 'ModelAdmin', 'BoardProfileModelAdmin', 'CategoryModelAdmin', 'SubcategoryModelAdmin', 'ThreadModelAdmin', 'PostModelAdmin', 'ShoutModelAdmin', 'GroupStyleModelAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c022008240b1e0124ff0e01020f1e0124ff0e01020d1e
-      0124ff0e01020f1e0124ff0e01021a1e0124ff0e01020e1e0124ff0e0102
-      0c1e0124ff0e01
+      0x00ff02010c022008240b1e0124ff0e01020f1e0124ff0e01020d1e0124
+      ff0e01020f1e0124ff0e01021a1e0124ff0e01020e1e0124ff0e01020c1e
+      0124ff0e01
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe8fe5866 (Thu May 30 22:34:16 2024 UTC)
+moddate:  0x69755966 (Fri May 31 06:59:53 2024 UTC)
 files sz: 1414
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x70e45866 (Thu May 30 20:41:20 2024 UTC)
+moddate:  0x7a755966 (Fri May 31 07:00:10 2024 UTC)
 files sz: 3130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x28613c66 (Thu May  9 05:37:44 2024 UTC)
+moddate:  0x81755966 (Fri May 31 07:00:17 2024 UTC)
 files sz: 628
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xf1aa0d66 (Wed Apr  3 19:16:01 2024 UTC)
+moddate:  0x85755966 (Fri May 31 07:00:21 2024 UTC)
 files sz: 395
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x51e45866 (Thu May 30 20:40:49 2024 UTC)
+moddate:  0x87755966 (Fri May 31 07:00:23 2024 UTC)
 files sz: 7053
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x7e021166 (Sat Apr  6 08:06:22 2024 UTC)
+moddate:  0x8c755966 (Fri May 31 07:00:28 2024 UTC)
 files sz: 409
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3cde5866 (Thu May 30 20:14:52 2024 UTC)
-files sz: 609
+moddate:  0x91755966 (Fri May 31 07:00:33 2024 UTC)
+files sz: 605
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a01010002006502650164026900a6030000ab
@@ -54,19 +54,19 @@
                110 LOAD_CONST               6 ('PunkwebBB')
                112 PRECALL                  2
                116 CALL                     2
                126 STORE_NAME               6 (SITE_TITLE)
    
      7         128 LOAD_NAME                3 (PUNKWEB_BB)
                130 LOAD_METHOD              4 (get)
-               152 LOAD_CONST               7 ('RENDERER')
+               152 LOAD_CONST               7 ('PARSER')
                154 LOAD_CONST               8 ('bbcode')
                156 PRECALL                  2
                160 CALL                     2
-               170 STORE_NAME               7 (RENDERER)
+               170 STORE_NAME               7 (PARSER)
    
      8         172 LOAD_NAME                3 (PUNKWEB_BB)
                174 LOAD_METHOD              4 (get)
                196 LOAD_CONST               9 ('FAVICON')
                198 LOAD_CONST              10 ('punkweb_bb/favicon.ico')
                200 PRECALL                  2
                204 CALL                     2
@@ -117,28 +117,28 @@
       0
       ('settings',)
       'PUNKWEB_BB'
       'SITE_NAME'
       'PUNKWEB'
       'SITE_TITLE'
       'PunkwebBB'
-      'RENDERER'
+      'PARSER'
       'bbcode'
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
-   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'RENDERER', 'FAVICON', 'OG_IMAGE', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
+   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'PARSER', 'FAVICON', 'OG_IMAGE', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/settings.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c021a022c012c012c012c012c012c012c012c01
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94ab0d66 (Wed Apr  3 19:18:44 2024 UTC)
+moddate:  0x93755966 (Fri May 31 07:00:35 2024 UTC)
 files sz: 365
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/sitemap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4ffe5866 (Thu May 30 22:31:43 2024 UTC)
+moddate:  0x96755966 (Fri May 31 07:00:38 2024 UTC)
 files sz: 26298
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3ce55766 (Thu May 30 02:32:28 2024 UTC)
+moddate:  0x99755966 (Fri May 31 07:00:41 2024 UTC)
 files sz: 2673
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 32
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/utils.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/utils.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,397 +1,402 @@
 magic:    0xa70d0d0a
-moddate:  0x6aff5866 (Thu May 30 22:36:26 2024 UTC)
-files sz: 1651
+moddate:  0x9c755966 (Fri May 31 07:00:44 2024 UTC)
+files sz: 1568
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a050100640484005a06640584005a07640684005a08640784
-      005a09640884005a0a64095300
+      036c046d055a050100640064046c066d075a070100640064056c086d095a
+      096d0a5a0a0100640684005a0b640784005a0c640884005a0d640984005a
+      0e640a84005a0f640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('slugify',))
-                 6 IMPORT_NAME              0 (django.utils.text)
-                 8 IMPORT_FROM              1 (slugify)
-                10 STORE_NAME               1 (slugify)
+                 4 LOAD_CONST               1 (('Textarea',))
+                 6 IMPORT_NAME              0 (django.forms)
+                 8 IMPORT_FROM              1 (Textarea)
+                10 STORE_NAME               1 (Textarea)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('get_parser',))
-                18 IMPORT_NAME              2 (precise_bbcode.bbcode)
-                20 IMPORT_FROM              3 (get_parser)
-                22 STORE_NAME               3 (get_parser)
+                16 LOAD_CONST               2 (('slugify',))
+                18 IMPORT_NAME              2 (django.utils.text)
+                20 IMPORT_FROM              3 (slugify)
+                22 STORE_NAME               3 (slugify)
                 24 POP_TOP
    
-     3          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('RENDERER',))
-                30 IMPORT_NAME              4 (punkweb_bb.settings)
-                32 IMPORT_FROM              5 (RENDERER)
-                34 STORE_NAME               5 (RENDERER)
+     4          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('get_parser',))
+                30 IMPORT_NAME              4 (punkweb_bb.bbcode)
+                32 IMPORT_FROM              5 (get_parser)
+                34 STORE_NAME               5 (get_parser)
                 36 POP_TOP
    
-     6          38 LOAD_CONST               4 (<code object get_editor_widget, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 6>)
-                40 MAKE_FUNCTION            0
-                42 STORE_NAME               6 (get_editor_widget)
+     5          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('PARSER',))
+                42 IMPORT_NAME              6 (punkweb_bb.settings)
+                44 IMPORT_FROM              7 (PARSER)
+                46 STORE_NAME               7 (PARSER)
+                48 POP_TOP
    
-    19          44 LOAD_CONST               5 (<code object get_unique_slug, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 19>)
-                46 MAKE_FUNCTION            0
-                48 STORE_NAME               7 (get_unique_slug)
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               5 (('BBCodeEditorWidget', 'MarkdownEditorWidget'))
+                54 IMPORT_NAME              8 (punkweb_bb.widgets)
+                56 IMPORT_FROM              9 (BBCodeEditorWidget)
+                58 STORE_NAME               9 (BBCodeEditorWidget)
+                60 IMPORT_FROM             10 (MarkdownEditorWidget)
+                62 STORE_NAME              10 (MarkdownEditorWidget)
+                64 POP_TOP
    
-    35          50 LOAD_CONST               6 (<code object get_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 35>)
-                52 MAKE_FUNCTION            0
-                54 STORE_NAME               8 (get_highest_priority_group)
+     9          66 LOAD_CONST               6 (<code object get_editor_widget, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 9>)
+                68 MAKE_FUNCTION            0
+                70 STORE_NAME              11 (get_editor_widget)
    
-    44          56 LOAD_CONST               7 (<code object get_styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 44>)
-                58 MAKE_FUNCTION            0
-                60 STORE_NAME               9 (get_styled_username)
+    17          72 LOAD_CONST               7 (<code object get_unique_slug, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 17>)
+                74 MAKE_FUNCTION            0
+                76 STORE_NAME              12 (get_unique_slug)
    
-    56          62 LOAD_CONST               8 (<code object get_styled_group_name, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 56>)
-                64 MAKE_FUNCTION            0
-                66 STORE_NAME              10 (get_styled_group_name)
-                68 LOAD_CONST               9 (None)
-                70 RETURN_VALUE
+    33          78 LOAD_CONST               8 (<code object get_highest_priority_group, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 33>)
+                80 MAKE_FUNCTION            0
+                82 STORE_NAME              13 (get_highest_priority_group)
+   
+    42          84 LOAD_CONST               9 (<code object get_styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 42>)
+                86 MAKE_FUNCTION            0
+                88 STORE_NAME              14 (get_styled_username)
+   
+    54          90 LOAD_CONST              10 (<code object get_styled_group_name, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py", line 54>)
+                92 MAKE_FUNCTION            0
+                94 STORE_NAME              15 (get_styled_group_name)
+                96 LOAD_CONST              11 (None)
+                98 RETURN_VALUE
    consts
       0
+      ('Textarea',)
       ('slugify',)
       ('get_parser',)
-      ('RENDERER',)
+      ('PARSER',)
+      ('BBCodeEditorWidget', 'MarkdownEditorWidget')
       code
          argcount  : 0
-         nlocals   : 2
-         stacksize : 3
+         nlocals   : 0
+         stacksize : 4
          flags     : 3
          code
-            0x970074000000000000000000000064016b02000000007210640264036c
-            016d027d00010002007c00a6000000ab0000000000000000005300740000
-            00000000000000000064046b02000000007210640264056c016d037d0101
-            0002007c01a6000000ab0000000000000000005300740900000000000000
-            0000006406a6010000ab0100000000000000008201
-           6           0 RESUME                   0
+            0x970074000000000000000000000064016b0200000000720e7403000000
+            00000000000000a6000000ab000000000000000000530074000000000000
+            000000000064026b0200000000720e740500000000000000000000a60000
+            00ab00000000000000000053007407000000000000000000006403640469
+            01ac05a6010000ab0100000000000000005300
+           9           0 RESUME                   0
          
-           7           2 LOAD_GLOBAL              0 (RENDERER)
+          10           2 LOAD_GLOBAL              0 (PARSER)
                       14 LOAD_CONST               1 ('bbcode')
                       16 COMPARE_OP               2 (==)
-                      22 POP_JUMP_FORWARD_IF_FALSE    16 (to 56)
+                      22 POP_JUMP_FORWARD_IF_FALSE    14 (to 52)
          
-           8          24 LOAD_CONST               2 (0)
-                      26 LOAD_CONST               3 (('BBCodeEditorWidget',))
-                      28 IMPORT_NAME              1 (punkweb_bb.widgets)
-                      30 IMPORT_FROM              2 (BBCodeEditorWidget)
-                      32 STORE_FAST               0 (BBCodeEditorWidget)
-                      34 POP_TOP
-         
-          10          36 PUSH_NULL
-                      38 LOAD_FAST                0 (BBCodeEditorWidget)
-                      40 PRECALL                  0
-                      44 CALL                     0
-                      54 RETURN_VALUE
-         
-          11     >>   56 LOAD_GLOBAL              0 (RENDERER)
-                      68 LOAD_CONST               4 ('markdown')
-                      70 COMPARE_OP               2 (==)
-                      76 POP_JUMP_FORWARD_IF_FALSE    16 (to 110)
-         
-          12          78 LOAD_CONST               2 (0)
-                      80 LOAD_CONST               5 (('MarkdownEditorWidget',))
-                      82 IMPORT_NAME              1 (punkweb_bb.widgets)
-                      84 IMPORT_FROM              3 (MarkdownEditorWidget)
-                      86 STORE_FAST               1 (MarkdownEditorWidget)
-                      88 POP_TOP
-         
-          14          90 PUSH_NULL
-                      92 LOAD_FAST                1 (MarkdownEditorWidget)
-                      94 PRECALL                  0
-                      98 CALL                     0
-                     108 RETURN_VALUE
-         
-          16     >>  110 LOAD_GLOBAL              9 (NULL + ValueError)
-                     122 LOAD_CONST               6 ('Invalid renderer')
-                     124 PRECALL                  1
-                     128 CALL                     1
-                     138 RAISE_VARARGS            1
+          11          24 LOAD_GLOBAL              3 (NULL + BBCodeEditorWidget)
+                      36 PRECALL                  0
+                      40 CALL                     0
+                      50 RETURN_VALUE
+         
+          12     >>   52 LOAD_GLOBAL              0 (PARSER)
+                      64 LOAD_CONST               2 ('markdown')
+                      66 COMPARE_OP               2 (==)
+                      72 POP_JUMP_FORWARD_IF_FALSE    14 (to 102)
+         
+          13          74 LOAD_GLOBAL              5 (NULL + MarkdownEditorWidget)
+                      86 PRECALL                  0
+                      90 CALL                     0
+                     100 RETURN_VALUE
+         
+          14     >>  102 LOAD_GLOBAL              7 (NULL + Textarea)
+                     114 LOAD_CONST               3 ('class')
+                     116 LOAD_CONST               4 ('pw-input')
+                     118 BUILD_MAP                1
+                     120 KW_NAMES                 5
+                     122 PRECALL                  1
+                     126 CALL                     1
+                     136 RETURN_VALUE
          consts
             None
             'bbcode'
-            0
-            ('BBCodeEditorWidget',)
             'markdown'
-            ('MarkdownEditorWidget',)
-            'Invalid renderer'
-         names      ('RENDERER', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'MarkdownEditorWidget', 'ValueError')
-         varnames   ('BBCodeEditorWidget', 'MarkdownEditorWidget')
+            'class'
+            'pw-input'
+            ('attrs',)
+         names      ('PARSER', 'BBCodeEditorWidget', 'MarkdownEditorWidget', 'Textarea')
+         varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_editor_widget'
-         firstlineno 6
-         lnotab 0x020116010c02140116010c021402
+         firstlineno 9
+         lnotab 0x020116011c0116011c01
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
-          19           0 RESUME                   0
+          17           0 RESUME                   0
          
-          20           2 LOAD_GLOBAL              1 (NULL + slugify)
+          18           2 LOAD_GLOBAL              1 (NULL + slugify)
                       14 LOAD_FAST                1 (field)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               2 (base_slug)
          
-          21          32 LOAD_FAST                2 (base_slug)
+          19          32 LOAD_FAST                2 (base_slug)
                       34 STORE_FAST               3 (slug)
          
-          22          36 LOAD_CONST               1 (True)
+          20          36 LOAD_CONST               1 (True)
                       38 STORE_FAST               4 (unique_slug_exists)
          
-          24          40 LOAD_CONST               2 (1)
+          22          40 LOAD_CONST               2 (1)
                       42 STORE_FAST               5 (counter)
          
-          25          44 LOAD_FAST                4 (unique_slug_exists)
+          23          44 LOAD_FAST                4 (unique_slug_exists)
                       46 POP_JUMP_FORWARD_IF_FALSE    62 (to 172)
          
-          26     >>   48 LOAD_FAST                0 (model)
+          24     >>   48 LOAD_FAST                0 (model)
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
          
-          27         138 LOAD_FAST                2 (base_slug)
+          25         138 LOAD_FAST                2 (base_slug)
                      140 FORMAT_VALUE             0
                      142 LOAD_CONST               4 ('-')
                      144 LOAD_FAST                5 (counter)
                      146 FORMAT_VALUE             0
                      148 BUILD_STRING             3
                      150 STORE_FAST               3 (slug)
          
-          28         152 LOAD_FAST                5 (counter)
+          26         152 LOAD_FAST                5 (counter)
                      154 LOAD_CONST               2 (1)
                      156 BINARY_OP               13 (+=)
                      160 STORE_FAST               5 (counter)
                      162 JUMP_FORWARD             2 (to 168)
          
-          30     >>  164 LOAD_CONST               5 (False)
+          28     >>  164 LOAD_CONST               5 (False)
                      166 STORE_FAST               4 (unique_slug_exists)
          
-          25     >>  168 LOAD_FAST                4 (unique_slug_exists)
+          23     >>  168 LOAD_FAST                4 (unique_slug_exists)
                      170 POP_JUMP_BACKWARD_IF_TRUE    62 (to 48)
          
-          32     >>  172 LOAD_FAST                3 (slug)
+          30     >>  172 LOAD_FAST                3 (slug)
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
-         firstlineno 19
+         firstlineno 17
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
-          35           0 RESUME                   0
+          33           0 RESUME                   0
          
-          36           2 LOAD_FAST                0 (user)
+          34           2 LOAD_FAST                0 (user)
                        4 LOAD_ATTR                0 (groups)
                       14 LOAD_METHOD              1 (filter)
                       36 LOAD_CONST               1 (False)
                       38 KW_NAMES                 2
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_FAST               1 (groups)
          
-          38          56 LOAD_FAST                1 (groups)
+          36          56 LOAD_FAST                1 (groups)
                       58 LOAD_METHOD              2 (exists)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 POP_JUMP_FORWARD_IF_FALSE    39 (to 174)
          
-          39          96 LOAD_FAST                1 (groups)
+          37          96 LOAD_FAST                1 (groups)
                       98 LOAD_METHOD              3 (order_by)
                      120 LOAD_CONST               3 ('-style__priority')
                      122 PRECALL                  1
                      126 CALL                     1
                      136 LOAD_METHOD              4 (first)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 RETURN_VALUE
          
-          41     >>  174 LOAD_CONST               0 (None)
+          39     >>  174 LOAD_CONST               0 (None)
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
-         firstlineno 35
+         firstlineno 33
          lnotab 0x0201360228014e02
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007d017c01724a740300000000000000000000a6000000ab000000000000
             0000007d027c016a0200000000000000006a0300000000000000007d037c
             02a00400000000000000000000000000000000000000007c03a005000000
             000000000000000000000000000000000064017c006a0600000000000000
             00a6020000ab020000000000000000a6010000ab0100000000000000007d
             047c0453007c006a0600000000000000005300
-          44           0 RESUME                   0
+          42           0 RESUME                   0
          
-          45           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
+          43           2 LOAD_GLOBAL              1 (NULL + get_highest_priority_group)
                       14 LOAD_FAST                0 (user)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (group)
          
-          47          32 LOAD_FAST                1 (group)
+          45          32 LOAD_FAST                1 (group)
                       34 POP_JUMP_FORWARD_IF_FALSE    74 (to 184)
          
-          48          36 LOAD_GLOBAL              3 (NULL + get_parser)
+          46          36 LOAD_GLOBAL              3 (NULL + get_parser)
                       48 PRECALL                  0
                       52 CALL                     0
                       62 STORE_FAST               2 (parser)
          
-          49          64 LOAD_FAST                1 (group)
+          47          64 LOAD_FAST                1 (group)
                       66 LOAD_ATTR                2 (style)
                       76 LOAD_ATTR                3 (username_style)
                       86 STORE_FAST               3 (username_style)
          
-          50          88 LOAD_FAST                2 (parser)
-                      90 LOAD_METHOD              4 (render)
+          48          88 LOAD_FAST                2 (parser)
+                      90 LOAD_METHOD              4 (format)
                      112 LOAD_FAST                3 (username_style)
                      114 LOAD_METHOD              5 (replace)
                      136 LOAD_CONST               1 ('{USER}')
                      138 LOAD_FAST                0 (user)
                      140 LOAD_ATTR                6 (username)
                      150 PRECALL                  2
                      154 CALL                     2
                      164 PRECALL                  1
                      168 CALL                     1
-                     178 STORE_FAST               4 (styled_username)
+                     178 STORE_FAST               4 (rendered)
          
-          51         180 LOAD_FAST                4 (styled_username)
+          49         180 LOAD_FAST                4 (rendered)
                      182 RETURN_VALUE
          
-          53     >>  184 LOAD_FAST                0 (user)
+          51     >>  184 LOAD_FAST                0 (user)
                      186 LOAD_ATTR                6 (username)
                      196 RETURN_VALUE
          consts
             None
             '{USER}'
-         names      ('get_highest_priority_group', 'get_parser', 'style', 'username_style', 'render', 'replace', 'username')
-         varnames   ('user', 'group', 'parser', 'username_style', 'styled_username')
+         names      ('get_highest_priority_group', 'get_parser', 'style', 'username_style', 'format', 'replace', 'username')
+         varnames   ('user', 'group', 'parser', 'username_style', 'rendered')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_styled_username'
-         firstlineno 44
+         firstlineno 42
          lnotab 0x02011e0204011c0118015c010402
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
-            0x97007c006a00000000000000000080077c006a01000000000000000053
-            00740500000000000000000000a6000000ab0000000000000000007d017c
-            006a0000000000000000006a0300000000000000007d027c01a004000000
-            00000000000000000000000000000000007c02a005000000000000000000
-            000000000000000000000064017c006a010000000000000000a6020000ab
-            020000000000000000a6010000ab0100000000000000007d037c035300
-          56           0 RESUME                   0
+            0x97007c006a000000000000000000814a740300000000000000000000a6
+            000000ab0000000000000000007d017c006a0000000000000000006a0200
+            000000000000007d027c01a0030000000000000000000000000000000000
+            0000007c02a004000000000000000000000000000000000000000064017c
+            006a050000000000000000a6020000ab020000000000000000a6010000ab
+            0100000000000000007d037c0353007c006a0500000000000000005300
+          54           0 RESUME                   0
          
-          57           2 LOAD_FAST                0 (group)
+          55           2 LOAD_FAST                0 (group)
                        4 LOAD_ATTR                0 (style)
-                      14 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 30)
+                      14 POP_JUMP_FORWARD_IF_NONE    74 (to 164)
+         
+          56          16 LOAD_GLOBAL              3 (NULL + get_parser)
+                      28 PRECALL                  0
+                      32 CALL                     0
+                      42 STORE_FAST               1 (parser)
+         
+          57          44 LOAD_FAST                0 (group)
+                      46 LOAD_ATTR                0 (style)
+                      56 LOAD_ATTR                2 (username_style)
+                      66 STORE_FAST               2 (username_style)
+         
+          58          68 LOAD_FAST                1 (parser)
+                      70 LOAD_METHOD              3 (format)
+                      92 LOAD_FAST                2 (username_style)
+                      94 LOAD_METHOD              4 (replace)
+                     116 LOAD_CONST               1 ('{USER}')
+                     118 LOAD_FAST                0 (group)
+                     120 LOAD_ATTR                5 (name)
+                     130 PRECALL                  2
+                     134 CALL                     2
+                     144 PRECALL                  1
+                     148 CALL                     1
+                     158 STORE_FAST               3 (rendered)
          
-          58          16 LOAD_FAST                0 (group)
-                      18 LOAD_ATTR                1 (name)
-                      28 RETURN_VALUE
-         
-          60     >>   30 LOAD_GLOBAL              5 (NULL + get_parser)
-                      42 PRECALL                  0
-                      46 CALL                     0
-                      56 STORE_FAST               1 (parser)
-         
-          61          58 LOAD_FAST                0 (group)
-                      60 LOAD_ATTR                0 (style)
-                      70 LOAD_ATTR                3 (username_style)
-                      80 STORE_FAST               2 (username_style)
-         
-          62          82 LOAD_FAST                1 (parser)
-                      84 LOAD_METHOD              4 (render)
-                     106 LOAD_FAST                2 (username_style)
-                     108 LOAD_METHOD              5 (replace)
-                     130 LOAD_CONST               1 ('{USER}')
-                     132 LOAD_FAST                0 (group)
-                     134 LOAD_ATTR                1 (name)
-                     144 PRECALL                  2
-                     148 CALL                     2
-                     158 PRECALL                  1
-                     162 CALL                     1
-                     172 STORE_FAST               3 (styled_group_name)
+          59         160 LOAD_FAST                3 (rendered)
+                     162 RETURN_VALUE
          
-          63         174 LOAD_FAST                3 (styled_group_name)
+          61     >>  164 LOAD_FAST                0 (group)
+                     166 LOAD_ATTR                5 (name)
                      176 RETURN_VALUE
          consts
             None
             '{USER}'
-         names      ('style', 'name', 'get_parser', 'username_style', 'render', 'replace')
-         varnames   ('group', 'parser', 'username_style', 'styled_group_name')
+         names      ('style', 'get_parser', 'username_style', 'format', 'replace', 'name')
+         varnames   ('group', 'parser', 'username_style', 'rendered')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
          name       'get_styled_group_name'
-         firstlineno 56
-         lnotab 0x02010e010e021c0118015c01
+         firstlineno 54
+         lnotab 0x02010e011c0118015c010402
       None
-   names      ('django.utils.text', 'slugify', 'precise_bbcode.bbcode', 'get_parser', 'punkweb_bb.settings', 'RENDERER', 'get_editor_widget', 'get_unique_slug', 'get_highest_priority_group', 'get_styled_username', 'get_styled_group_name')
+   names      ('django.forms', 'Textarea', 'django.utils.text', 'slugify', 'punkweb_bb.bbcode', 'get_parser', 'punkweb_bb.settings', 'PARSER', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'MarkdownEditorWidget', 'get_editor_widget', 'get_unique_slug', 'get_highest_priority_group', 'get_styled_username', 'get_styled_group_name')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c010c03060d06100609060c
+   lnotab 0x00ff02010c010c020c010c011003060806100609060c
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x22e95766 (Thu May 30 02:49:06 2024 UTC)
-files sz: 18191
+moddate:  0x59835966 (Fri May 31 07:59:21 2024 UTC)
+files sz: 18010
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a040100640064
@@ -3379,45 +3379,45 @@
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
          585           0 RESUME                   0
          
-         586           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         586           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Color', '[color=red]Red Text[/color]'), ('Font', '[font=serif]Serif Text[/font]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Horizontal Rule', '[hr]'), ('Left', '[left]Left Text[/left]'), ('Center', '[center]Centered Text[/center]'), ('Right', '[right]Right Text[/right]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         640           6 LOAD_CONST               2 ('codes')
+         631           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         639          10 BUILD_MAP                1
+         630          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         643          14 LOAD_GLOBAL              1 (NULL + render)
+         634          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
          consts
             None
-            (('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]'))
+            (('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Color', '[color=red]Red Text[/color]'), ('Font', '[font=serif]Serif Text[/font]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Horizontal Rule', '[hr]'), ('Left', '[left]Left Text[/left]'), ('Center', '[center]Centered Text[/center]'), ('Right', '[right]Right Text[/right]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]'))
             'codes'
             'punkweb_bb/bbcode.html'
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
          firstlineno 585
-         lnotab 0x0201043604ff0404
+         lnotab 0x0201042d04ff0404
       None
    names      ('django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'ThreadMoveForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'thread_move_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x74ff5866 (Thu May 30 22:36:36 2024 UTC)
+moddate:  0xa5755966 (Fri May 31 07:00:53 2024 UTC)
 files sz: 1502
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/admin.py` & `punkweb_bb-0.4.0/punkweb_bb/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.contrib import admin
-from django.utils.safestring import mark_safe
 
 from punkweb_bb.admin_forms import (
     BoardProfileAdminModelForm,
     CategoryAdminModelForm,
     GroupStyleAdminModelForm,
     PostAdminModelForm,
     SubcategoryAdminModelForm,
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/admin_forms.py` & `punkweb_bb-0.4.0/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/forms.py` & `punkweb_bb-0.4.0/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/middleware.py` & `punkweb_bb-0.4.0/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.4.0/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/0003_alter_thread_options.py` & `punkweb_bb-0.4.0/punkweb_bb/migrations/0003_alter_thread_options.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/0004_groupstyle.py` & `punkweb_bb-0.4.0/punkweb_bb/migrations/0004_groupstyle.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/0005_alter_thread_options.py` & `punkweb_bb-0.4.0/punkweb_bb/migrations/0005_alter_thread_options.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py` & `punkweb_bb-0.4.0/punkweb_bb/migrations/0006_remove_boardprofile__signature_rendered_and_more.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0005_alter_thread_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/migrations/__pycache__/0006_remove_boardprofile__signature_rendered_and_more.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/models.py` & `punkweb_bb-0.4.0/punkweb_bb/models.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/settings.py` & `punkweb_bb-0.4.0/punkweb_bb/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.conf import settings
 
 PUNKWEB_BB = getattr(settings, "PUNKWEB_BB", {})
 
 SITE_NAME = PUNKWEB_BB.get("SITE_NAME", "PUNKWEB")
 SITE_TITLE = PUNKWEB_BB.get("SITE_TITLE", "PunkwebBB")
-RENDERER = PUNKWEB_BB.get("RENDERER", "bbcode")
+PARSER = PUNKWEB_BB.get("PARSER", "bbcode")
 FAVICON = PUNKWEB_BB.get("FAVICON", "punkweb_bb/favicon.ico")
 OG_IMAGE = PUNKWEB_BB.get("OG_IMAGE", None)
 SHOUTBOX_ENABLED = PUNKWEB_BB.get("SHOUTBOX_ENABLED", True)
 DISCORD_WIDGET_ENABLED = PUNKWEB_BB.get("DISCORD_WIDGET_ENABLED", False)
 DISCORD_WIDGET_THEME = PUNKWEB_BB.get("DISCORD_WIDGET_THEME", "dark")
 DISCORD_SERVER_ID = PUNKWEB_BB.get("DISCORD_SERVER_ID", None)
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 * {
   box-sizing: border-box;
-  margin: 0;
-  padding: 0;
 }
 
 *:before,
 *:after {
   box-sizing: border-box;
 }
 
 /* set body min width to 20rem and reset line height */
 body {
   line-height: 1;
   min-width: 20rem;
+  margin: 0;
+  padding: 0;
 }
 
 /* set cursor to pointer on buttons */
 button,
 input[type="submit"],
 input[type="button"] {
   cursor: pointer;
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .modal {
   align-items: center;
   background-color: rgba(0, 0, 0, 0.5);
   display: flex;
   flex-direction: column;
   justify-content: center;
+  padding: 2rem;
 
   position: fixed;
   top: 0;
   bottom: 0;
   left: 0;
   right: 0;
   z-index: 1000;
@@ -24,14 +25,15 @@
   z-index: -1;
 }
 
 .modal__content {
   border-radius: 0.25rem;
   box-shadow: 0 0.5rem 1rem 0 rgba(0, 0, 0, 0.25);
   background-color: white;
+  overflow: auto;
   position: relative;
   width: fit-content;
 
   animation: zoomIn 150ms ease;
 }
 
 .modal__header {
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 }
 
 .pw-table thead tr th {
   background-color: var(--table-header-bg);
   border-bottom: 1px solid var(--border);
   color: var(--table-header-text);
   font-size: 0.875rem;
-  font-weight: 500;
+  font-weight: 700;
   padding: 0.75rem 1rem;
   text-align: left;
 }
 
 .pw-table tbody tr td {
   padding: 0.75rem 1rem;
 }
@@ -660,15 +660,15 @@
 .pw-input:not(:disabled):active {
   border: 1px solid var(--primary-9);
 }
 
 .pw-input-label {
   display: block;
   font-size: 0.875rem;
-  font-weight: 500;
+  font-weight: 700;
 }
 
 /** Card **/
 
 .pw-card {
   background-color: var(--card-bg);
   border: 1px solid var(--border);
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 .subcategory__header__name {
   align-items: center;
   display: flex;
   gap: 1rem;
 }
 
+.subcategory__header__name h1 {
+  margin: 0;
+}
+
 .subcategory__header__actions {
   align-items: center;
   display: flex;
   gap: 0.5rem;
 }
 
 .thread__title {
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,24 @@
   color: #212529;
   font-family: Arial, Helvetica sans-serif;
   font-size: 16px;
   font-weight: 400;
   line-height: 1.5;
   overflow: visible;
 }
+
 html {
   height: 100%;
 }
 
 * {
   box-sizing: border-box;
+}
+
+body {
   margin: 0;
   padding: 0;
 }
 
 *:before,
 *:after {
   box-sizing: border-box;
@@ -52,19 +56,14 @@
   margin: 1rem 0;
 }
 
 a {
   text-decoration: none;
 }
 
-ul,
-ol {
-  padding-inline-start: 2rem;
-}
-
 code {
   display: block;
   background: #f5f2f0;
   font-family: Consolas, Monaco, "Andale Mono", "Ubuntu Mono", monospace;
   white-space: pre;
   padding: 1em;
   text-align: left;
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/editor/markdown-editor.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/editor/markdown-editor.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,49 @@
-function initMarkdownEditor(element) {
-    var editor = new TinyMDE.Editor({
-        textarea: element,
-    });
+function initMarkdownEditor(containerElement) {
+    var editorElement = containerElement.querySelector(".markdown-editor");
+    var toolbarElement = containerElement.querySelector(
+        "#markdown-editor-toolbar"
+    );
 
-    var toolbarElement = document.createElement("div");
-    toolbarElement.id = "markdown-editor-toolbar";
-    element.parentNode.insertBefore(toolbarElement, element);
+    var editor = null;
 
-    new TinyMDE.CommandBar({
-        element: toolbarElement,
-        editor: editor,
-    });
+    if (!containerElement.querySelector(".TinyMDE")) {
+        editor = new TinyMDE.Editor({
+            textarea: editorElement,
+        });
+    }
+
+    if (editor && !toolbarElement.querySelector(".TMCommandBar")) {
+        var toolbar = new TinyMDE.CommandBar({
+            element: toolbarElement,
+            editor: editor,
+            commands: [
+                "bold",
+                "italic",
+                "strikethrough",
+                "|",
+                "h1",
+                "h2",
+                "|",
+                "ul",
+                "ol",
+                "|",
+                "blockquote",
+                "code",
+                "insertLink",
+                "insertImage",
+                "hr",
+            ],
+        });
+    }
 }
 
 $(function() {
     $(document).ready(function() {
-        var editorElements = document.querySelectorAll(".markdown-editor");
+        var editorElements = document.querySelectorAll(
+            ".markdown-editor-container"
+        );
         editorElements.forEach((element) => {
             initMarkdownEditor(element);
         });
     });
 });
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/.gitignore`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/blank.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/demo.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/dist/tiny-mde.tiny.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/docs/index.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/globals.d.ts`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/gulpfile.mjs`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/block.test.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/commandbar.test.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/inline.test.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/interaction.test.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/setup.test.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/jest/util/test-helpers.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package-lock.json`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/package.json`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDE.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/TinyMDECommandBar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/commandbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/css/editor.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/grammar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/blank.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/html/demo.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/blockquote.svg`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js` & `punkweb_bb-0.4.0/punkweb_bb/static/punkweb_bb/vendor/tiny-markdown-editor/src/svg/svg.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_create.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/category_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/category_update.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/category_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/partials/thread_move.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/partials/thread_move.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.4.0/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/markdown.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc` & `punkweb_bb-0.4.0/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/tests.py` & `punkweb_bb-0.4.0/punkweb_bb/tests.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/urls.py` & `punkweb_bb-0.4.0/punkweb_bb/urls.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb/utils.py` & `punkweb_bb-0.4.0/punkweb_bb/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
+from django.forms import Textarea
 from django.utils.text import slugify
-from precise_bbcode.bbcode import get_parser
-from punkweb_bb.settings import RENDERER
 
+from punkweb_bb.bbcode import get_parser
+from punkweb_bb.settings import PARSER
+from punkweb_bb.widgets import BBCodeEditorWidget, MarkdownEditorWidget
 
-def get_editor_widget():
-    if RENDERER == "bbcode":
-        from punkweb_bb.widgets import BBCodeEditorWidget
 
+def get_editor_widget():
+    if PARSER == "bbcode":
         return BBCodeEditorWidget()
-    elif RENDERER == "markdown":
-        from punkweb_bb.widgets import MarkdownEditorWidget
-
+    elif PARSER == "markdown":
         return MarkdownEditorWidget()
-    else:
-        raise ValueError("Invalid renderer")
+    return Textarea(attrs={"class": "pw-input"})
 
 
 def get_unique_slug(model, field):
     base_slug = slugify(field)
     slug = base_slug
     unique_slug_exists = True
 
@@ -43,21 +41,21 @@
 
 def get_styled_username(user):
     group = get_highest_priority_group(user)
 
     if group:
         parser = get_parser()
         username_style = group.style.username_style
-        styled_username = parser.render(username_style.replace("{USER}", user.username))
-        return styled_username
-    else:
-        return user.username
+        rendered = parser.format(username_style.replace("{USER}", user.username))
+        return rendered
+
+    return user.username
 
 
 def get_styled_group_name(group):
-    if group.style is None:
-        return group.name
-    else:
+    if group.style is not None:
         parser = get_parser()
         username_style = group.style.username_style
-        styled_group_name = parser.render(username_style.replace("{USER}", group.name))
-        return styled_group_name
+        rendered = parser.format(username_style.replace("{USER}", group.name))
+        return rendered
+
+    return group.name
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/views.py` & `punkweb_bb-0.4.0/punkweb_bb/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,24 +584,30 @@
 
 def bbcode_view(request):
     codes = (
         ("Bold", "[b]Bold Text[/b]"),
         ("Italic", "[i]Italic Text[/i]"),
         ("Underline", "[u]Underlined Text[/u]"),
         ("Strikethrough", "[s]Strikethrough Text[/s]"),
-        ("Quote", "[quote=Example]Quoted Text[/quote]"),
-        ("Center", "[center]Centered Text[/center]"),
         ("Color", "[color=red]Red Text[/color]"),
+        ("Font", "[font=serif]Serif Text[/font]"),
+        ("Shadow", "[shadow=red]Red Shadow Text[/shadow]"),
+        ("Size", "[size=7]Size 7 Text[/size]"),
+        ("Superscript", "Sup [sup]Superscript Text[/sup]"),
+        ("Subscript", "Sub [sub]Subscript Text[/sub]"),
+        ("Horizontal Rule", "[hr]"),
+        ("Left", "[left]Left Text[/left]"),
+        ("Center", "[center]Centered Text[/center]"),
+        ("Right", "[right]Right Text[/right]"),
+        ("Quote", "[quote=Example]Quoted Text[/quote]"),
         ("Url", "[url=https://google.com]Link Text[/url]"),
         (
             "Image",
             "[img]https://placehold.co/400[/img]",
         ),
-        # Custom
-        ("Horizontal Rule", "[hr]"),
         (
             "Code",
             """
 [code=python]
 class ThreadModelForm(forms.ModelForm):
     class Meta:
         model = Thread
@@ -612,31 +618,16 @@
         widgets = {
             "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),
             "content": BBCodeEditorWidget(),
         }
 [/code]
 """,
         ),
-        ("Email", "[email=test@example.com]Example[/email]"),
-        ("Font", "[font=serif]Serif Text[/font]"),
         ("Ordered List", "[ol][li]Item 1[/li][li]Item 2[/li][/ol]"),
         ("Unordered List", "[ul][li]Item 1[/li][li]Item 2[/li][/ul]"),
-        ("Shadow", "[shadow=red]Red Shadow Text[/shadow]"),
-        ("Size", "[size=7]Size 7 Text[/size]"),
-        (
-            "Checkbox",
-            """
-[n]Unchecked
-[y]Checked
-            """,
-        ),
-        ("Superscript", "Sup [sup]Superscript Text[/sup]"),
-        ("Subscript", "Sub [sub]Subscript Text[/sub]"),
-        ("Left", "[left]Left Text[/left]"),
-        ("Right", "[right]Right Text[/right]"),
         ("Escape", "[escape][b]Escaped bbcode[/b][/escape]"),
     )
 
     context = {
         "codes": codes,
     }
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb/widgets.py` & `punkweb_bb-0.4.0/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.3.0/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.4.0/punkweb_bb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.3.0
+Version: 0.4.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,69 +16,61 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
-This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
-
 Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
-- [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
-- [Markdown](https://python-markdown.github.io/)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
+- [bbcode](https://pypi.org/project/bbcode/)
+- [Markdown](https://pypi.org/project/Markdown/)
 - [SCEditor](https://www.sceditor.com/)
 - [TinyMDE](https://github.com/jefago/tiny-markdown-editor)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
 - Python 3.9+
 - Django 4.0+
-- django-precise-bbcode 1.2+
-- markdown 3.6+
-- Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## BBCode or Markdown?
 
-PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which renderer you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
+PunkwebBB supports both BBCode and Markdown. You'll want to decide before installing which parser you want to use, as switching between them will cause existing threads, posts, signatures, etc. to render incorrectly! Switching will not affect the database schema, but it will affect the content.
 
-BBCode is the default renderer, but you can switch to Markdown by setting the following in your Django settings module:
+BBCode is the default parser, but you can switch to Markdown by setting the following in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
-  "RENDERER": "markdown",
+  "PARSER": "markdown",
 }
 ```
 
 ## Installation
 
 ```bash
 pip install punkweb-bb
 ```
 
-Add `precise_bbcode` and `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
+Add `punkweb_bb` to your `INSTALLED_APPS` in your Django settings module:
 
 ```python
 INSTALLED_APPS = [
     ...
-    "precise_bbcode",
     "punkweb_bb",
 ]
 ```
 
-_Note_: `precise_bbcode` is required even if using the Markdown renderer! It must be installed before `punkweb_bb`.
-
 Add the following context processor to your `TEMPLATES` setting:
 
 ```python
 TEMPLATES = [
     {
         ...
         "OPTIONS": {
@@ -112,15 +104,15 @@
 
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
-  "RENDERER": "bbcode", # "bbcode" or "markdown"
+  "PARSER": "bbcode", # "bbcode" or "markdown"
   "FAVICON": "punkweb_bb/favicon.ico",
   "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
```

### Comparing `punkweb_bb-0.3.0/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.4.0/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 MANIFEST.in
 README.md
 setup.py
 punkweb_bb/__init__.py
 punkweb_bb/admin.py
 punkweb_bb/admin_forms.py
 punkweb_bb/apps.py
-punkweb_bb/bbcode_tags.py
+punkweb_bb/bbcode.py
 punkweb_bb/context_processors.py
 punkweb_bb/forms.py
 punkweb_bb/guests.py
 punkweb_bb/middleware.py
 punkweb_bb/mixins.py
 punkweb_bb/models.py
 punkweb_bb/pagination.py
-punkweb_bb/parsers.py
 punkweb_bb/response.py
 punkweb_bb/settings.py
 punkweb_bb/signals.py
 punkweb_bb/tests.py
 punkweb_bb/urls.py
 punkweb_bb/utils.py
 punkweb_bb/views.py
@@ -29,27 +28,29 @@
 punkweb_bb.egg-info/not-zip-safe
 punkweb_bb.egg-info/requires.txt
 punkweb_bb.egg-info/top_level.txt
 punkweb_bb/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/__pycache__/admin.cpython-311.pyc
 punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
 punkweb_bb/__pycache__/apps.cpython-311.pyc
+punkweb_bb/__pycache__/bbcode.cpython-311.pyc
 punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
 punkweb_bb/__pycache__/context_processors.cpython-311.pyc
 punkweb_bb/__pycache__/forms.cpython-311.pyc
 punkweb_bb/__pycache__/guests.cpython-311.pyc
 punkweb_bb/__pycache__/middleware.cpython-311.pyc
 punkweb_bb/__pycache__/mixins.cpython-311.pyc
 punkweb_bb/__pycache__/models.cpython-311.pyc
 punkweb_bb/__pycache__/pagination.cpython-311.pyc
 punkweb_bb/__pycache__/parsers.cpython-311.pyc
 punkweb_bb/__pycache__/response.cpython-311.pyc
 punkweb_bb/__pycache__/settings.cpython-311.pyc
 punkweb_bb/__pycache__/signals.cpython-311.pyc
 punkweb_bb/__pycache__/sitemap.cpython-311.pyc
+punkweb_bb/__pycache__/tags.cpython-311.pyc
 punkweb_bb/__pycache__/tests.cpython-311.pyc
 punkweb_bb/__pycache__/urls.cpython-311.pyc
 punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
@@ -299,15 +300,14 @@
 punkweb_bb/templates/punkweb_bb/widgets/markdown-editor.html
 punkweb_bb/templatetags/__init__.py
 punkweb_bb/templatetags/can_delete.py
 punkweb_bb/templatetags/can_edit.py
 punkweb_bb/templatetags/can_post.py
 punkweb_bb/templatetags/humanize_int.py
 punkweb_bb/templatetags/render.py
-punkweb_bb/templatetags/shoutbox_render.py
 punkweb_bb/templatetags/styled_group_name.py
 punkweb_bb/templatetags/styled_username.py
 punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
```

### Comparing `punkweb_bb-0.3.0/setup.py` & `punkweb_bb-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.3.0",
+    version="0.4.0",
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
-        "django-precise-bbcode",
+        "bbcode",
         "markdown",
-        "expiringdict",
         "pillow",
+        "expiringdict",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
```

