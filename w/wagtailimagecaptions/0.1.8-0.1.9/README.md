# Comparing `tmp/wagtailimagecaptions-0.1.8.tar.gz` & `tmp/wagtailimagecaptions-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailimagecaptions-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtailimagecaptions-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtailimagecaptions-0.1.8.tar` & `wagtailimagecaptions-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.8/LICENSE
--rw-r--r--   0        0        0     1783 2024-02-20 12:22:58.817708 wagtailimagecaptions-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.8/media/.gitkeep
--rw-r--r--   0        0        0     1203 2023-11-29 14:29:06.682894 wagtailimagecaptions-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.8/setup.cfg
--rw-r--r--   0        0        0      164 2024-02-20 12:22:53.078964 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/__init__.py
--rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/apps.py
--rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0001_initial.py
--rw-r--r--   0        0        0      352 2023-07-19 11:10:26.633109 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0002_rename_extendedrendition_captionedrendition.py
--rw-r--r--   0        0        0     1569 2023-11-21 17:30:03.855636 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0003_captionedimage_byline_and_more.py
--rw-r--r--   0        0        0      573 2023-11-21 17:30:03.855830 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0004_auto_20231121_1134.py
--rw-r--r--   0        0        0      450 2023-12-01 16:21:13.645173 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0005_auto_20231121_1134.py
--rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/__init__.py
--rw-r--r--   0        0        0     4194 2024-02-20 12:22:58.818208 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/models.py
--rw-r--r--   0        0        0     3592 2023-11-21 17:30:03.857266 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/services.py
--rw-r--r--   0        0        0     1952 2023-12-01 16:21:13.645663 wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/signals.py
--rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.8/test_project/__init__.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.8/test_project/asgi.py
--rw-r--r--   0        0        0     3910 2024-02-20 12:22:58.818856 wagtailimagecaptions-0.1.8/test_project/settings.py
--rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.8/test_project/urls.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.8/test_project/wsgi.py
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1783 2024-02-20 12:22:58.817708 wagtailimagecaptions-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512372 wagtailimagecaptions-0.1.9/media/.gitkeep
+-rw-r--r--   0        0        0     1203 2023-11-29 14:29:06.682894 wagtailimagecaptions-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.9/setup.cfg
+-rw-r--r--   0        0        0      164 2024-05-31 14:18:51.343085 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/apps.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0001_initial.py
+-rw-r--r--   0        0        0      352 2023-07-19 11:10:26.633109 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0002_rename_extendedrendition_captionedrendition.py
+-rw-r--r--   0        0        0     1569 2023-11-21 17:30:03.855636 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0003_captionedimage_byline_and_more.py
+-rw-r--r--   0        0        0      573 2023-11-21 17:30:03.855830 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0004_auto_20231121_1134.py
+-rw-r--r--   0        0        0      450 2023-12-01 16:21:13.645173 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0005_auto_20231121_1134.py
+-rw-r--r--   0        0        0      521 2024-05-31 14:18:51.343322 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0006_alter_captionedimage_options.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/__init__.py
+-rw-r--r--   0        0        0     4446 2024-05-31 14:18:51.343840 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/models.py
+-rw-r--r--   0        0        0     3592 2023-11-21 17:30:03.857266 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/services.py
+-rw-r--r--   0        0        0     1952 2023-12-01 16:21:13.645663 wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/signals.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.9/test_project/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936483 wagtailimagecaptions-0.1.9/test_project/asgi.py
+-rw-r--r--   0        0        0     3912 2024-05-31 14:18:51.344268 wagtailimagecaptions-0.1.9/test_project/settings.py
+-rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.9/test_project/urls.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939985 wagtailimagecaptions-0.1.9/test_project/wsgi.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.9/PKG-INFO
```

### Comparing `wagtailimagecaptions-0.1.8/LICENSE` & `wagtailimagecaptions-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/README.md` & `wagtailimagecaptions-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/pyproject.toml` & `wagtailimagecaptions-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/setup.cfg` & `wagtailimagecaptions-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0001_initial.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0003_captionedimage_byline_and_more.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0003_captionedimage_byline_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/migrations/0004_auto_20231121_1134.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/migrations/0004_auto_20231121_1134.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/models.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import uuid
 
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
 from wagtail.coreutils import string_to_ascii
 from wagtail.fields import RichTextField
 from wagtail.images.models import AbstractImage, AbstractRendition, Image
 from wagtail.search import index
 
 
 class CaptionedImage(AbstractImage):
@@ -50,14 +51,21 @@
     )
 
     search_fields = AbstractImage.search_fields + [
         index.SearchField("uuid"),
         index.SearchField("caption"),
     ]
 
+    class Meta(AbstractImage.Meta):
+        verbose_name = _("image")
+        verbose_name_plural = _("images")
+        permissions = [
+            ("choose_image", "Can choose image"),
+        ]
+
     def default_alt_text(self):
         """Return our stored alt value, otherwise Wagtail defaults to the title."""
         if self.alt:
             return self.alt
         return super().default_alt_text
 
     def get_upload_to(self, filename):
```

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/services.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/services.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/src/wagtailimagecaptions/signals.py` & `wagtailimagecaptions-0.1.9/src/wagtailimagecaptions/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/test_project/settings.py` & `wagtailimagecaptions-0.1.9/test_project/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "wagtail.contrib.routable_page",
     "wagtail.contrib.forms",
     "wagtail.contrib.redirects",
-    "wagtail.contrib.modeladmin",
+    # "wagtail.contrib.modeladmin",
     "wagtail.contrib.settings",
     "wagtail.embeds",
     "wagtail.sites",
     "wagtail.users",
     "wagtail.snippets",
     "wagtail.documents",
     "wagtail.images",
```

### Comparing `wagtailimagecaptions-0.1.8/test_project/urls.py` & `wagtailimagecaptions-0.1.9/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.8/PKG-INFO` & `wagtailimagecaptions-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailimagecaptions
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app for extending the Wagtail Image model to add captions and alt fields as
 Author-email: Stephan Rohde <appsupport@newshour.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

