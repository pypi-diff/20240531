# Comparing `tmp/django_headless_cms-0.2.1.tar.gz` & `tmp/django_headless_cms-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_headless_cms-0.2.1.tar", max compression
+gzip compressed data, was "django_headless_cms-0.2.2.tar", max compression
```

## Comparing `django_headless_cms-0.2.1.tar` & `django_headless_cms-0.2.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1521 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/LICENSE
--rw-r--r--   0        0        0      925 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/__init__.py
--rw-r--r--   0        0        0    14062 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/admin.py
--rw-r--r--   0        0        0       71 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/__init__.py
--rw-r--r--   0        0        0     4029 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/base_translate.py
--rw-r--r--   0        0        0     3617 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/openai_translate.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/__init__.py
--rw-r--r--   0        0        0      376 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/admin.py
--rw-r--r--   0        0        0     9496 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/__init__.py
--rw-r--r--   0        0        0     2695 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/__init__.py
--rw-r--r--   0        0        0      365 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/admin.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/commands/__init__.py
--rw-r--r--   0        0        0     1115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/commands/populate_aw_data.py
--rw-r--r--   0        0        0    11108 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py
--rw-r--r--   0        0        0    12374 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/__init__.py
--rw-r--r--   0        0        0     6212 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/models.py
--rw-r--r--   0        0        0     1327 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/views.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/__init__.py
--rw-r--r--   0        0        0      277 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/admin.py
--rw-r--r--   0        0        0    10936 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/__init__.py
--rw-r--r--   0        0        0     2413 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/models.py
--rw-r--r--   0        0        0      638 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py
--rw-r--r--   0        0        0      369 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/urls.py
--rw-r--r--   0        0        0     2093 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/views.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/__init__.py
--rw-r--r--   0        0        0     1859 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py
--rw-r--r--   0        0        0    75728 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/__init__.py
--rw-r--r--   0        0        0    15115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/shared/__init__.py
--rw-r--r--   0        0        0      226 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/shared/serializers.py
--rw-r--r--   0        0        0      736 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/urls.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2558 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/clean_outdated_drafts.py
--rw-r--r--   0        0        0     3912 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/export_cms_data.py
--rw-r--r--   0        0        0     5165 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/import_cms_data.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/__init__.py
--rw-r--r--   0        0        0     3003 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
--rw-r--r--   0        0        0     1633 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/admin/change_form.html
--rw-r--r--   0        0        0       67 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
--rw-r--r--   0        0        0       67 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
--rw-r--r--   0        0        0      689 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
--rw-r--r--   0        0        0     2115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/object_history.html
--rw-r--r--   0        0        0     1245 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/revision_form.html
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/boolean_field.py
--rw-r--r--   0        0        0      559 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/martor_field.py
--rw-r--r--   0        0        0      753 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/slug_field.py
--rw-r--r--   0        0        0       89 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/url_field.py
--rw-r--r--   0        0        0      452 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/forms.py
--rw-r--r--   0        0        0      302 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/mixins.py
--rw-r--r--   0        0        0     7213 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/models.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/__init__.py
--rw-r--r--   0        0        0      490 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/auto_schema.py
--rw-r--r--   0        0        0      314 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/preprocessing_hooks.py
--rw-r--r--   0        0        0      831 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/urls.py
--rw-r--r--   0        0        0      285 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/views.py
--rw-r--r--   0        0        0      883 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/serializer_fields.py
--rw-r--r--   0        0        0     5802 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/serializers.py
--rw-r--r--   0        0        0     1028 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/settings.py
--rw-r--r--   0        0        0        0 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/__init__.py
--rw-r--r--   0        0        0     1954 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/custom_import_export.py
--rw-r--r--   0        0        0     1003 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/markdown.py
--rw-r--r--   0        0        0     2033 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/martor_custom_upload.py
--rw-r--r--   0        0        0     2449 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/relations.py
--rw-r--r--   0        0        0     5424 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/widgets.py
--rw-r--r--   0        0        0     3909 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 django_headless_cms-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/LICENSE
+-rw-r--r--   0        0        0      925 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/__init__.py
+-rw-r--r--   0        0        0    18821 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/admin.py
+-rw-r--r--   0        0        0       71 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/auto_translate/__init__.py
+-rw-r--r--   0        0        0     4029 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/auto_translate/base_translate.py
+-rw-r--r--   0        0        0     3617 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/auto_translate/openai_translate.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/admin.py
+-rw-r--r--   0        0        0     9496 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/migrations/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/models.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/admin.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/management/commands/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/management/commands/populate_aw_data.py
+-rw-r--r--   0        0        0    11108 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py
+-rw-r--r--   0        0        0    12374 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.501924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/migrations/__init__.py
+-rw-r--r--   0        0        0     6212 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/models.py
+-rw-r--r--   0        0        0     1327 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/views.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/admin.py
+-rw-r--r--   0        0        0    10936 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/migrations/__init__.py
+-rw-r--r--   0        0        0     2413 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/models.py
+-rw-r--r--   0        0        0      638 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/serializers.py
+-rw-r--r--   0        0        0      369 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/urls.py
+-rw-r--r--   0        0        0     2093 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/views.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/admin.py
+-rw-r--r--   0        0        0    75728 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/migrations/__init__.py
+-rw-r--r--   0        0        0    15115 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/models.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/shared/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/shared/serializers.py
+-rw-r--r--   0        0        0      736 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/contrib/astrowind/urls.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2558 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/management/commands/clean_outdated_drafts.py
+-rw-r--r--   0        0        0     3912 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/management/commands/export_cms_data.py
+-rw-r--r--   0        0        0     5165 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/core/management/commands/import_cms_data.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/__init__.py
+-rw-r--r--   0        0        0     3003 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
+-rw-r--r--   0        0        0     1633 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/admin/change_form.html
+-rw-r--r--   0        0        0       67 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
+-rw-r--r--   0        0        0       67 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
+-rw-r--r--   0        0        0      689 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
+-rw-r--r--   0        0        0     2115 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/reversion/object_history.html
+-rw-r--r--   0        0        0     1245 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/enhances/templates/reversion/revision_form.html
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/fields/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/fields/boolean_field.py
+-rw-r--r--   0        0        0      559 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/fields/martor_field.py
+-rw-r--r--   0        0        0      753 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/fields/slug_field.py
+-rw-r--r--   0        0        0       89 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/fields/url_field.py
+-rw-r--r--   0        0        0      452 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/forms.py
+-rw-r--r--   0        0        0     1434 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/mixins.py
+-rw-r--r--   0        0        0    14624 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/models.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/schema/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/schema/auto_schema.py
+-rw-r--r--   0        0        0      314 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/schema/preprocessing_hooks.py
+-rw-r--r--   0        0        0      831 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/schema/urls.py
+-rw-r--r--   0        0        0      285 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/schema/views.py
+-rw-r--r--   0        0        0      893 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/serializer_fields.py
+-rw-r--r--   0        0        0     9390 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/serializers.py
+-rw-r--r--   0        0        0     1028 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/settings.py
+-rw-r--r--   0        0        0        0 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/utils/__init__.py
+-rw-r--r--   0        0        0     1954 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/utils/custom_import_export.py
+-rw-r--r--   0        0        0     1003 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/utils/markdown.py
+-rw-r--r--   0        0        0     2033 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/utils/martor_custom_upload.py
+-rw-r--r--   0        0        0     2449 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/utils/relations.py
+-rw-r--r--   0        0        0     5424 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/headless_cms/widgets.py
+-rw-r--r--   0        0        0     3931 2024-05-31 06:05:49.505924 django_headless_cms-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 django_headless_cms-0.2.2/PKG-INFO
```

### Comparing `django_headless_cms-0.2.1/LICENSE` & `django_headless_cms-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/README.md` & `django_headless_cms-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/admin.py` & `django_headless_cms-0.2.2/headless_cms/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,31 +33,52 @@
     M2MSortedOrderThrough,
     SortableGenericBaseModel,
 )
 from headless_cms.utils.custom_import_export import override_modelresource_factory
 
 
 class PublishStatusInlineMixin:
-    show_change_link = True
+    """
+    Mixin to show the publish status of related objects in inline admin.
+    """
 
+    show_change_link = True
     readonly_fields = ("publish_status",)
 
     def _get_publish_status(self, obj):
+        """
+        Get the publish status of an object.
+
+        Args:
+            obj (models.Model): The object to check.
+
+        Returns:
+            str: The publish status.
+        """
         published_state = "unpublished"
         if obj.published_version:
             last_ver = Version.objects.get_for_object(obj).first()
             if last_ver.id == obj.published_version.id:
                 published_state = "published (latest)"
             else:
                 published_state = "published (outdated)"
         return published_state
 
-    def publish_status(self, obj):  # noqa: C901
+    def publish_status(self, obj):
+        """
+        Get the publish status of an object for display in the admin.
+
+        Args:
+            obj (models.Model): The object to check.
+
+        Returns:
+            str: The publish status.
+        """
         published_state = "unpublished"
-        if hasattr(obj, "is_through_table") and obj.is_through_table:
+        if isinstance(obj, M2MSortedOrderThrough):
             fields = obj._meta.get_fields()
             for field in fields:
                 rel_model = field.related_model
                 if not rel_model or not issubclass(
                     rel_model, LocalizedPublicationModel
                 ):
                     continue
@@ -84,76 +105,140 @@
         return published_state
 
 
 class BaseGenericAdmin(
     PublishStatusInlineMixin,
     GenericStackedInline,
 ):
+    """
+    Base class for generic inlines with publish status.
+    """
+
     extra = 0
 
 
 class BaseSortableGenericAdmin(
     SortableGenericInlineAdminMixin,
     SortableStackedInline,
     BaseGenericAdmin,
 ):
+    """
+    Base class for sortable generic inlines with publish status.
+    """
+
     extra = 0
 
 
 @admin.action(description="Publish selected")
 def publish(modeladmin, request, queryset):
+    """
+    Admin action to publish selected objects.
+
+    Args:
+        modeladmin (ModelAdmin): The model admin.
+        request (HttpRequest): The request object.
+        queryset (QuerySet): The selected objects.
+    """
     obj: LocalizedPublicationModel
 
     for obj in queryset.all():
         obj.publish(request.user)
 
 
 @admin.action(description="Unpublish selected")
 def unpublish(modeladmin, request, queryset):
+    """
+    Admin action to unpublish selected objects.
+
+    Args:
+        modeladmin (ModelAdmin): The model admin.
+        request (HttpRequest): The request object.
+        queryset (QuerySet): The selected objects.
+    """
     obj: LocalizedPublicationModel
 
     for obj in queryset.all():
         obj.unpublish(request.user)
 
 
 @admin.action(description="Translate untranslated contents")
 def translate_missing(modeladmin, request, queryset):
+    """
+    Admin action to translate missing content for selected objects.
+
+    Args:
+        modeladmin (ModelAdmin): The model admin.
+        request (HttpRequest): The request object.
+        queryset (QuerySet): The selected objects.
+    """
     obj: LocalizedPublicationModel
 
     for obj in queryset.all():
         obj.translate(request.user)
 
 
 @admin.action(description="Force translate (override old translation)")
 def force_translate(modeladmin, request, queryset):
+    """
+    Admin action to force translate selected objects, overriding old translations.
+
+    Args:
+        modeladmin (ModelAdmin): The model admin.
+        request (HttpRequest): The request object.
+        queryset (QuerySet): The selected objects.
+    """
     obj: LocalizedPublicationModel
 
     for obj in queryset.all():
         obj.translate(request.user, force=True)
 
 
 FORCE_TRANSLATE = {"_force_translate", "_recursively_force_translate"}
 RECURSIVELY_TRANSLATE = {"_recursively_translate", "_recursively_force_translate"}
 TRANSLATE_ACTIONS = {"_translate"} | FORCE_TRANSLATE | RECURSIVELY_TRANSLATE
 
 
 class EnhancedLocalizedVersionAdmin(
     ImportExportActionModelAdmin, LocalizedFieldsAdminMixin, VersionAdmin
 ):
+    """
+    Enhanced admin class for localized versioned models.
+
+    Includes support for import/export, localization, and versioning.
+    """
+
     actions = [publish, unpublish, translate_missing, force_translate]
     formfield_overrides = {
         models.TextField: {"widget": AdminMartorWidget},
     }
 
     def get_list_display(self, request):
+        """
+        Get the list display fields for the admin changelist.
+
+        Args:
+            request (HttpRequest): The request object.
+
+        Returns:
+            tuple: The list display fields.
+        """
         list_display = super().get_list_display(request)
         return list_display + ("published_state",)
 
     def render_change_form(self, request, context, *args, **kwargs):
-        """We need to update the context to show the button."""
+        """
+        Render the change form for the admin.
+
+        Args:
+            request (HttpRequest): The request object.
+            context (dict): The context for the form.
+
+        Returns:
+            HttpResponse: The rendered change form.
+        """
         obj = kwargs.get("obj")
         if obj and not context.get("revert"):
             show_publish = True
             show_unpublish = False
             show_recursively_publish = any(
                 f.is_relation
                 and not f.auto_created
@@ -181,24 +266,46 @@
                     "show_translate": True,
                 }
             )
 
         return super().render_change_form(request, context, *args, **kwargs)
 
     def changelist_view(self, request, extra_context=None):
+        """
+        Render the changelist view for the admin.
+
+        Args:
+            request (HttpRequest): The request object.
+            extra_context (dict, optional): Extra context for the view.
+
+        Returns:
+            HttpResponse: The rendered changelist view.
+        """
         if request.POST and "action" in request.POST:
             context = {
                 "has_change_permission": self.has_change_permission(request),
             }
             context.update(extra_context or {})
             return super(VersionAdmin, self).changelist_view(request, context)
         else:
             return super().changelist_view(request, extra_context)
 
     def change_view(self, request, object_id, form_url="", extra_context=None):
+        """
+        Render the change view for the admin.
+
+        Args:
+            request (HttpRequest): The request object.
+            object_id (str): The ID of the object being changed.
+            form_url (str, optional): The form URL.
+            extra_context (dict, optional): Extra context for the view.
+
+        Returns:
+            HttpResponse: The rendered change view.
+        """
         res = super().change_view(request, object_id, form_url, extra_context)
 
         obj: LocalizedPublicationModel = self.get_object(request, unquote(object_id))
 
         request_post_keys = set(request.POST.keys())
         if "_unpublish" in request_post_keys:
             obj.unpublish(request.user)
@@ -212,14 +319,24 @@
             if recursively:
                 obj.recursively_translate(request.user, force)
             else:
                 obj.translate(request.user, force)
         return res
 
     def response_change(self, request, obj):
+        """
+        Handle the response after saving the object in the admin.
+
+        Args:
+            request (HttpRequest): The request object.
+            obj (models.Model): The object being saved.
+
+        Returns:
+            HttpResponse: The response.
+        """
         opts = self.opts
         preserved_filters = self.get_preserved_filters(request)
 
         msg_dict = {
             "name": opts.verbose_name,
             "obj": format_html('<a href="{}">{}</a>', urlquote(request.path), obj),
         }
@@ -265,15 +382,26 @@
         redirect_url = request.path
         redirect_url = add_preserved_filters(
             {"preserved_filters": preserved_filters, "opts": opts}, redirect_url
         )
         return HttpResponseRedirect(redirect_url)
 
     def revision_view(self, request, object_id, version_id, extra_context=None):
-        """Displays the contents of the given revision."""
+        """
+        Displays the contents of the given revision.
+
+        Args:
+            request (HttpRequest): The request object.
+            object_id (str): The ID of the object being changed.
+            version_id (str): The ID of the version to display.
+            extra_context (dict, optional): Extra context for the view.
+
+        Returns:
+            HttpResponse: The rendered revision view.
+        """
         object_id = unquote(object_id)  # Underscores in primary key get quoted to "_5F"
         version = get_object_or_404(Version, pk=version_id, object_id=object_id)
         context = {
             "title": _("Revert %(name)s") % {"name": version.object_repr},
             "revert": True,
             "is_published": (
                 version.object.published_version
@@ -288,14 +416,26 @@
             or self._reversion_get_template_list("revision_form.html"),
             context,
         )
 
     def _reversion_revisionform_view(
         self, request, version, template_name, extra_context=None
     ):
+        """
+        Helper method for rendering the revision form view.
+
+        Args:
+            request (HttpRequest): The request object.
+            version (Version): The version to display.
+            template_name (str): The template name.
+            extra_context (dict, optional): Extra context for the view.
+
+        Returns:
+            HttpResponse: The rendered revision form view.
+        """
         old_published_version = (
             version.object.published_version if version.object else None
         )
         res = super()._reversion_revisionform_view(
             request, version, template_name, extra_context
         )
 
@@ -305,21 +445,38 @@
                     version.refresh_from_db()
                     version.object.published_version_id = old_published_version
                     version.object.save()
 
         return res
 
     def get_resource_classes(self, *args, **kwargs):
+        """
+        Get the resource classes for import/export.
+
+        Returns:
+            list: The resource classes.
+        """
         if not self.resource_classes:
             return [override_modelresource_factory(self.model)]
         return super().get_resource_classes(*args, **kwargs)
 
 
 @lru_cache(maxsize=0)
 def create_m2m_inline_admin(model, sortable=False, fk_name=None):
+    """
+    Create an inline admin class for a many-to-many relationship.
+
+    Args:
+        model (models.Model): The model for the inline admin.
+        sortable (bool, optional): Whether the inline is sortable.
+        fk_name (str, optional): The foreign key name.
+
+    Returns:
+        type: The inline admin class.
+    """
     body = {"extra": 0, "model": model}
     if fk_name is not None:
         body["fk_name"] = fk_name
     return type(
         model.__name__ + "Inline",
         (
             PublishStatusInlineMixin,
@@ -327,24 +484,40 @@
         ),
         body,
     )
 
 
 @lru_cache(maxsize=0)
 def create_generic_inline_admin(model, sortable=False):
+    """
+    Create an inline admin class for a generic relationship.
+
+    Args:
+        model (models.Model): The model for the inline admin.
+        sortable (bool, optional): Whether the inline is sortable.
+
+    Returns:
+        type: The inline admin class.
+    """
     return type(
         model.__name__ + "Inline",
         (BaseSortableGenericAdmin if sortable else BaseGenericAdmin,),
         {"model": model},
     )
 
 
 def auto_admins(
     model_list: list[type[models.Model]],
 ):
+    """
+    Automatically register admin classes for a list of models.
+
+    Args:
+        model_list (list): The list of models to register.
+    """
     for model in model_list:
         admin_attrs = {"history_latest_first": True}
         inlines = []
         exclude = []
         model_fields = model._meta.get_fields()
         has_sortable_base = False
         for field in model_fields:
```

### Comparing `django_headless_cms-0.2.1/headless_cms/auto_translate/base_translate.py` & `django_headless_cms-0.2.2/headless_cms/auto_translate/base_translate.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/auto_translate/openai_translate.py` & `django_headless_cms-0.2.2/headless_cms/auto_translate/openai_translate.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_metadata/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/commands/populate_aw_data.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/management/commands/populate_aw_data.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/models.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/views.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_pages/views.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/models.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/serializers.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/views.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_posts/views.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/admin.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/astrowind_widgets/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/urls.py` & `django_headless_cms-0.2.2/headless_cms/contrib/astrowind/urls.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/core/management/commands/clean_outdated_drafts.py` & `django_headless_cms-0.2.2/headless_cms/core/management/commands/clean_outdated_drafts.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/core/management/commands/export_cms_data.py` & `django_headless_cms-0.2.2/headless_cms/core/management/commands/export_cms_data.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/core/management/commands/import_cms_data.py` & `django_headless_cms-0.2.2/headless_cms/core/management/commands/import_cms_data.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js` & `django_headless_cms-0.2.2/headless_cms/enhances/static/localized_fields/localized-fields-admin.js`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/enhances/templates/admin/change_form.html` & `django_headless_cms-0.2.2/headless_cms/enhances/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html` & `django_headless_cms-0.2.2/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/object_history.html` & `django_headless_cms-0.2.2/headless_cms/enhances/templates/reversion/object_history.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/revision_form.html` & `django_headless_cms-0.2.2/headless_cms/enhances/templates/reversion/revision_form.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/fields/boolean_field.py` & `django_headless_cms-0.2.2/headless_cms/fields/boolean_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/fields/martor_field.py` & `django_headless_cms-0.2.2/headless_cms/fields/martor_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/fields/slug_field.py` & `django_headless_cms-0.2.2/headless_cms/fields/slug_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/schema/urls.py` & `django_headless_cms-0.2.2/headless_cms/schema/urls.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/serializer_fields.py` & `django_headless_cms-0.2.2/headless_cms/serializer_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,10 +19,10 @@
             return value
 
         language_code = translation.get_language() or settings.LANGUAGE_CODE
 
         return f"/{language_code}" + value
 
 
-class LocalizedMartorField(CharField):
+class LocalizedMartorFieldSerializer(CharField):
     def to_representation(self, value):
         return replace_placeholder(str(value), False)
```

### Comparing `django_headless_cms-0.2.1/headless_cms/settings.py` & `django_headless_cms-0.2.2/headless_cms/settings.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/utils/custom_import_export.py` & `django_headless_cms-0.2.2/headless_cms/utils/custom_import_export.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/utils/markdown.py` & `django_headless_cms-0.2.2/headless_cms/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/utils/martor_custom_upload.py` & `django_headless_cms-0.2.2/headless_cms/utils/martor_custom_upload.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/utils/relations.py` & `django_headless_cms-0.2.2/headless_cms/utils/relations.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/headless_cms/widgets.py` & `django_headless_cms-0.2.2/headless_cms/widgets.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.2.1/pyproject.toml` & `django_headless_cms-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -82,32 +82,32 @@
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
 version_provider = "poetry"
 version_scheme = "pep440"
 
 [tool.commitizen.customize]
-bump_map = {build = "PATCH", ci = "PATCH", feat = "MINOR", fix = "PATCH", perf = "PATCH", refactor = "PATCH"}
-bump_pattern = '^(feat|fix|ci|build|perf|refactor)'
-schema_pattern = '^(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump|my_custom_one)(\(\S+\))?\:?\s.*'
+bump_map = {build = "PATCH", ci = "PATCH", docs = "PATCH", feat = "MINOR", fix = "PATCH", perf = "PATCH", refactor = "PATCH"}
+bump_pattern = '^(feat|fix|ci|build|perf|refactor|docs)'
+schema_pattern = '^(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump)(\(\S+\))?\:?\s.*'
 
 [tool.coverage.run]
 omit = [
   "headless_cms/contrib/*",
   "headless_cms/fields/boolean_field.py",  # Just a small fix
   "headless_cms/utils/martor_custom_upload.py",
   "tests/*"
 ]
 
 [tool.poetry]
 name = 'headless_cms'
 packages = [
   {include = "headless_cms"}
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.27.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = ">=7.0.0,<8"
 sphinx_rtd_theme = "*"
@@ -147,14 +147,15 @@
   "PL",  # pylint
   "Q",  # flake8-quotes
   "UP",  # pyupgrade
   "W"  # pycodestyle warnings
 ]
 
 [tool.ruff.lint.per-file-ignores]
+"*" = ['C901']
 "tests/*" = ["PLR0913", "PLR2004"]
 "tests/test_utils/base.py" = ["N802"]
 
 [tool.tomlsort]
 all = true
 in_place = true
 spaces_before_inline_comment = 2
```

### Comparing `django_headless_cms-0.2.1/PKG-INFO` & `django_headless_cms-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-headless-cms
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple django-based headless CMS.
 Home-page: https://github.com/huynguyengl99/django-headless-cms
 License: Copyright © 2024-present, Huy Nguyen <danghuy1999@gmail.com>.
          
          All rights reserved.
          
          Redistribution and use in source and binary forms, with or without
```

