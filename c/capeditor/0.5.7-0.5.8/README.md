# Comparing `tmp/capeditor-0.5.7.tar.gz` & `tmp/capeditor-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.5.7.tar", last modified: Thu May 16 10:49:15 2024, max compression
+gzip compressed data, was "capeditor-0.5.8.tar", last modified: Fri May 31 10:03:07 2024, max compression
```

## Comparing `capeditor-0.5.7.tar` & `capeditor-0.5.8.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 10:49:11.000000 capeditor-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-16 10:49:15.676053 capeditor-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-16 10:49:11.000000 capeditor-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/cap_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/caputils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/forms/capimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.652053 capeditor-0.5.7/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.660053 capeditor-0.5.7/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.656053 capeditor-0.5.7/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/0002_alter_capsetting_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/0003_capsetting_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/0004_predefinedalertarea.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/0005_alter_capsetting_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/pubsub/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/pubsub/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.656053 capeditor-0.5.7/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.656053 capeditor-0.5.7/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/cap_detail_page.css
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/import_cap_preview.css
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/mapbox-gl-draw.css
--rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.664053 capeditor-0.5.7/capeditor/static/capeditor/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.672053 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.672053 capeditor-0.5.7/capeditor/static/capeditor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/alert.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/area.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/certainty.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/extreme.png
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/minor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/moderate.png
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/severe.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/images/urgency.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.672053 capeditor-0.5.7/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/mapbox-gl-draw.js
--rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/turf.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.656053 capeditor-0.5.7/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/icons/cap-alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/load_cap_alert.html
--rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/preview_cap_alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-16 10:49:11.000000 capeditor-0.5.7/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:49:15.676053 capeditor-0.5.7/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-16 10:49:15.000000 capeditor-0.5.7/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-16 10:49:15.000000 capeditor-0.5.7/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:49:15.000000 capeditor-0.5.7/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 10:49:15.000000 capeditor-0.5.7/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 10:49:15.000000 capeditor-0.5.7/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 10:49:11.000000 capeditor-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-16 10:49:15.676053 capeditor-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.100842 capeditor-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 10:03:00.000000 capeditor-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-31 10:03:07.100842 capeditor-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-31 10:03:00.000000 capeditor-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26778 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/cap_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/caputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/forms/capimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.072842 capeditor-0.5.8/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.072842 capeditor-0.5.8/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.072842 capeditor-0.5.8/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.072842 capeditor-0.5.8/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.080842 capeditor-0.5.8/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0002_alter_capsetting_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0003_capsetting_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0004_predefinedalertarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0005_alter_capsetting_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/0006_capsetting_wmo_oid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/pubsub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/pubsub/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/cap_detail_page.css
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/import_cap_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/mapbox-gl-draw.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.084842 capeditor-0.5.8/capeditor/static/capeditor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.092842 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.092842 capeditor-0.5.8/capeditor/static/capeditor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/area.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/certainty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/extreme.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/minor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/moderate.png
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/severe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/images/urgency.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.092842 capeditor-0.5.8/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/mapbox-gl-draw.js
+-rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/turf.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.096842 capeditor-0.5.8/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.076842 capeditor-0.5.8/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.096842 capeditor-0.5.8/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.096842 capeditor-0.5.8/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/icons/cap-alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/load_cap_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/preview_cap_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.096842 capeditor-0.5.8/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-31 10:03:00.000000 capeditor-0.5.8/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:03:07.096842 capeditor-0.5.8/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-31 10:03:07.000000 capeditor-0.5.8/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-31 10:03:07.000000 capeditor-0.5.8/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:03:07.000000 capeditor-0.5.8/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-31 10:03:07.000000 capeditor-0.5.8/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 10:03:07.000000 capeditor-0.5.8/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 10:03:00.000000 capeditor-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-31 10:03:07.100842 capeditor-0.5.8/setup.cfg
```

### Comparing `capeditor-0.5.7/PKG-INFO` & `capeditor-0.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.7
+Version: 0.5.8
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -64,18 +64,17 @@
 
 - Modern user-friendly composer that follows [CAP 1.2](http://docs.oasis-open.org/emergency/cap/v1.2/CAP-v1.2-os.html)
   standard. Built on top of the awesome [Wagtail CMS](https://wagtail.org)
 - Preview a CAP alert as you edit. Save drafts for sharing with colleagues and collaborating
 - Inbuilt CAP validation. The page will not save if you have not input the required data according to CAP standard
 - User-friendly alert area map tool that allows multiple ways of constructing alert geographic areas, while keeping the
   interface simple
-    - Select country official administrative boundaries for different levels (Admin 1, Admin 2, Admin 3), with in-built
-      simplification of complex boundaries
     - Draw a polygon
     - Draw a circle
+    - Selecting predefined areas that you create beforehand for common alert areas
     - Use Geocode key values
 - Inbuilt publishing workflow using Wagtail's powerful page model, with automated emails to composers and approvers
 - Collaborate with team members using inbuilt comments (similar to how you could do in Word) with automated
   notifications. Request for changes and approvals
 - Publish realtime notifications/messages to third party integrations using MQTT messaging protocol
 - Predefine a list of hazards types monitored by your institution, with intuitive icons
   from [OCHA humanitarian icons](https://brand.unocha.org/d/xEPytAUjC3sH/icons#/humanitarian-icons)
@@ -215,29 +214,26 @@
 - Area Description (areaDesc),
 - Area Polygon/Polygons (polygon),
 - Area Circle/Circles (circle),
 - Area Geocode/Geocodes (geocode),
 - Altitude (altitude),
 - Ceiling (ceiling)
 
-The Alert area input has 4 selector options:
-
-- Admin Boundary (area is picked from predefined boundaries). To use this option, ensure that admin boundaries are
-  initially loaded. Refer to [Setting up boundaries](#setting-up-boundaries) section.
-
-![Alert Area boundary](images/alert_sections/alert_area_boundary.png "Alert Area Boundary")
+The Alert area input has multiple selector options:
 
 - Polygon (drawing a polygon)
 
 ![Alert Area polygon](images/alert_sections/alert_area_polygon.png "Alert Area Polygon")
 
 - Circle (drawing a circle which specifies the latitude, longitude and radius)
 
 ![Alert Area circle](images/alert_sections/alert_area_circle.png "Alert Area Circle")
 
+- Predefined Area (selecting a predefined area that you create beforehand for common alert areas)
+
 - Geocode (specifying area geocode name and value). Using this option presumes knowledge of the coding system
 
 ![Alert Area geocode](images/alert_sections/alert_area_geocode.png "Alert Area Geocode")
 
 #### Alert Resource
 
 Entity that defines supplemental information related to an <info> object Multiple instances of this section are allowed.
```

### Comparing `capeditor-0.5.7/README.md` & `capeditor-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,17 @@
 
 - Modern user-friendly composer that follows [CAP 1.2](http://docs.oasis-open.org/emergency/cap/v1.2/CAP-v1.2-os.html)
   standard. Built on top of the awesome [Wagtail CMS](https://wagtail.org)
 - Preview a CAP alert as you edit. Save drafts for sharing with colleagues and collaborating
 - Inbuilt CAP validation. The page will not save if you have not input the required data according to CAP standard
 - User-friendly alert area map tool that allows multiple ways of constructing alert geographic areas, while keeping the
   interface simple
-    - Select country official administrative boundaries for different levels (Admin 1, Admin 2, Admin 3), with in-built
-      simplification of complex boundaries
     - Draw a polygon
     - Draw a circle
+    - Selecting predefined areas that you create beforehand for common alert areas
     - Use Geocode key values
 - Inbuilt publishing workflow using Wagtail's powerful page model, with automated emails to composers and approvers
 - Collaborate with team members using inbuilt comments (similar to how you could do in Word) with automated
   notifications. Request for changes and approvals
 - Publish realtime notifications/messages to third party integrations using MQTT messaging protocol
 - Predefine a list of hazards types monitored by your institution, with intuitive icons
   from [OCHA humanitarian icons](https://brand.unocha.org/d/xEPytAUjC3sH/icons#/humanitarian-icons)
@@ -184,29 +183,26 @@
 - Area Description (areaDesc),
 - Area Polygon/Polygons (polygon),
 - Area Circle/Circles (circle),
 - Area Geocode/Geocodes (geocode),
 - Altitude (altitude),
 - Ceiling (ceiling)
 
-The Alert area input has 4 selector options:
-
-- Admin Boundary (area is picked from predefined boundaries). To use this option, ensure that admin boundaries are
-  initially loaded. Refer to [Setting up boundaries](#setting-up-boundaries) section.
-
-![Alert Area boundary](images/alert_sections/alert_area_boundary.png "Alert Area Boundary")
+The Alert area input has multiple selector options:
 
 - Polygon (drawing a polygon)
 
 ![Alert Area polygon](images/alert_sections/alert_area_polygon.png "Alert Area Polygon")
 
 - Circle (drawing a circle which specifies the latitude, longitude and radius)
 
 ![Alert Area circle](images/alert_sections/alert_area_circle.png "Alert Area Circle")
 
+- Predefined Area (selecting a predefined area that you create beforehand for common alert areas)
+
 - Geocode (specifying area geocode name and value). Using this option presumes knowledge of the coding system
 
 ![Alert Area geocode](images/alert_sections/alert_area_geocode.png "Alert Area Geocode")
 
 #### Alert Resource
 
 Entity that defines supplemental information related to an <info> object Multiple instances of this section are allowed.
```

### Comparing `capeditor-0.5.7/capeditor/blocks.py` & `capeditor-0.5.8/capeditor/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,77 +156,14 @@
     )
 
     response_type = blocks.ChoiceBlock(choices=RESPONSE_TYPE_CHOICES, label=_("Response type"),
                                        help_text=_("The code denoting the type of action recommended for the "
                                                    "target audience"))
 
 
-class AlertAreaBoundaryStructValue(StructValue):
-    @cached_property
-    def area(self):
-        geom_geojson_str = self.get("boundary")
-        geom_geojson_dict = json.loads(geom_geojson_str)
-        geom_shape = shape(geom_geojson_dict)
-
-        polygons = []
-
-        if isinstance(geom_shape, Polygon):
-            polygons.append(geom_shape)
-        else:
-            polygons = list(geom_shape.geoms)
-
-        polygons_data = []
-        for polygon in polygons:
-            coords = " ".join(["{},{}".format(y, x) for x, y in list(polygon.exterior.reverse().coords)])
-            polygons_data.append(coords)
-
-        area_data = {
-            "areaDesc": self.get("areaDesc"),
-            "polygons": polygons_data
-        }
-
-        if self.get("altitude"):
-            area_data.update({"altitude": self.get("altitude")})
-            if self.get("ceiling"):
-                area_data.update({"ceiling": self.get("ceiling")})
-
-        return area_data
-
-    @cached_property
-    def geojson(self):
-        polygon = self.get("boundary")
-        return json.loads(polygon)
-
-
-class AlertAreaBoundaryBlock(blocks.StructBlock):
-    class Meta:
-        value_class = AlertAreaBoundaryStructValue
-
-    ADMIN_LEVEL_CHOICES = (
-        (0, _("Level 0")),
-        (1, _("Level 1")),
-        (2, _("Level 2")),
-        (3, _("Level 3"))
-    )
-
-    areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
-                                help_text=_("The text describing the affected area of the alert message"))
-    admin_level = blocks.ChoiceBlock(choices=ADMIN_LEVEL_CHOICES, default=1, label=_("Administrative Level"))
-    boundary = BoundaryFieldBlock(label=_("Boundary"),
-                                  help_text=_("The paired values of points defining a polygon that delineates "
-                                              "the affected area of the alert message"))
-
-    altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
-                                help_text=_("The specific or minimum altitude of the affected "
-                                            "area of the alert message"))
-    ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
-                               help_text=_("The maximum altitude of the affected area of the alert message."
-                                           "MUST NOT be used except in combination with the altitude element. "))
-
-
 class AlertAreaPolygonStructValue(StructValue):
     @cached_property
     def area(self):
         geom_geojson_str = self.get("polygon")
         geom_geojson_dict = json.loads(geom_geojson_str)
         geom_shape = shape(geom_geojson_dict)
 
@@ -675,20 +612,19 @@
 
     senderName = blocks.CharBlock(max_length=255, label=_("Sender name"), required=False,
                                   help_text=SENDER_NAME_HELP_TEXT)
     contact = blocks.CharBlock(max_length=255, required=False, label=_("Contact"), help_text=CONTACT_HELP_TEXT)
     audience = blocks.CharBlock(max_length=255, required=False, label=_("Audience"),
                                 help_text=AUDIENCE_HELP_TEXT)
     area = blocks.StreamBlock([
-        ("boundary_block", AlertAreaBoundaryBlock(label=_("Admin Boundary"))),
         ("polygon_block", AlertAreaPolygonBlock(label=_("Draw Polygon"))),
         ("circle_block", AlertAreaCircleBlock(label=_("Circle"))),
         ("geocode_block", AlertAreaGeocodeBlock(label=_("Geocode"))),
         ("predefined_block", AlertAreaPredefined(label=_("Predefined Area"))),
-    ], label=_("Alert Area"), help_text=_("Admin Boundary, Polygon, Circle or Geocode"))
+    ], label=_("Alert Area"), help_text=_("Polygon, Circle, Predefined area or Geocode"))
 
     resource = blocks.StreamBlock([
         ("file_resource", FileResource()),
         ("external_resource", ExternalResource()),
     ], required=False, label=_("Resources"), help_text=_("Additional file with supplemental information "
                                                          "related to this alert information"))
```

### Comparing `capeditor-0.5.7/capeditor/cap_settings.py` & `capeditor-0.5.8/capeditor/cap_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
 @register_setting
 class CapSetting(BaseSiteSetting, ClusterableModel):
     sender = models.CharField(max_length=255, blank=True, null=True, verbose_name=_("CAP Sender Email"),
                               help_text=_("Email of the sending institution"))
     sender_name = models.CharField(max_length=255, blank=True, null=True, verbose_name=_("CAP Sender Name"),
                                    help_text=_("Name of the sending institution"))
+    wmo_oid = models.CharField(max_length=255, blank=True, null=True,
+                               verbose_name=_("WMO Register of Alerting Authorities OID"),
+                               help_text=_("WMO Register of Alerting Authorities "
+                                           "Object Identifier (OID) of the sending institution. "
+                                           "This will be used to generate CAP messages identifiers"))
+
     logo = models.ForeignKey("wagtailimages.Image", null=True, blank=True, on_delete=models.SET_NULL, related_name="+",
                              verbose_name=_("Logo of the sending institution"))
 
     contacts = StreamField([
         ("contact", ContactBlock(label=_("Contact")))
     ], use_json_field=True, blank=True, null=True, verbose_name=_("Contact Details"),
         help_text=_("Contact for follow-up and confirmation of the alert message"))
@@ -41,14 +47,15 @@
     class Meta:
         verbose_name = _("CAP Settings")
 
     edit_handler = TabbedInterface([
         ObjectList([
             FieldPanel("sender_name"),
             FieldPanel("sender"),
+            FieldPanel("wmo_oid"),
             FieldPanel("logo"),
             FieldPanel("contacts"),
         ], heading=_("Sender Details")),
         ObjectList([
             InlinePanel("hazard_event_types", heading=_("Hazard Types"), label=_("Hazard Type"),
                         help_text=_("Hazards monitored by the institution")),
         ], heading=_("Hazard Types")),
```

### Comparing `capeditor-0.5.7/capeditor/caputils.py` & `capeditor-0.5.8/capeditor/caputils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/constants.py` & `capeditor-0.5.8/capeditor/constants.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/forms/capimporter.py` & `capeditor-0.5.8/capeditor/forms/capimporter.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/forms/fields.py` & `capeditor-0.5.8/capeditor/forms/fields.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/forms/widgets.py` & `capeditor-0.5.8/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.5.8/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.5.8/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/migrations/0001_initial.py` & `capeditor-0.5.8/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/migrations/0002_alter_capsetting_options_and_more.py` & `capeditor-0.5.8/capeditor/migrations/0002_alter_capsetting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/migrations/0003_capsetting_logo.py` & `capeditor-0.5.8/capeditor/migrations/0003_capsetting_logo.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/migrations/0004_predefinedalertarea.py` & `capeditor-0.5.8/capeditor/migrations/0004_predefinedalertarea.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/models.py` & `capeditor-0.5.8/capeditor/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,27 +102,30 @@
                 self.add_error('references', _("You must select at least one reference alert for this message type. "
                                                "Only 'Alert' Message Type can be saved without references."))
             else:
                 alerts_ids = []
                 for reference in references:
                     ref_alert_page = reference.value.get("ref_alert").specific
                     if ref_alert_page:
-                        alerts_ids.append(ref_alert_page.identifier)
+                        if hasattr(ref_alert_page, 'identifier'):
+                            alerts_ids.append(ref_alert_page.identifier)
+                        else:
+                            alerts_ids.append(ref_alert_page.id)
 
                 # check if the same alert is selected more than once
                 if len(alerts_ids) != len(set(alerts_ids)):
                     self.add_error('references', _("You cannot select the same alert more than once."))
 
         return cleaned_data
 
 
 class AbstractCapAlertPage(Page):
     base_form_class = CapAlertPageForm
 
-    exclude_fields_in_copy = ["identifier"]
+    exclude_fields_in_copy = ["guid"]
 
     STATUS_CHOICES = (
         ("Draft", _("Draft - A preliminary template or draft, not actionable in its current form")),
         ("Actual", _("Actual - Actionable by all targeted recipients")),
         ("Test", _("Test - Technical testing only, all recipients disregard")),
         ("Exercise", _("Exercise - Actionable only by designated exercise participants; "
                        "exercise identifier SHOULD appear in note")),
@@ -142,17 +145,16 @@
     SCOPE_CHOICES = (
         ('Public', _("Public - For general dissemination to unrestricted audiences")),
         ('Restricted', _("Restricted - For dissemination only to users with a known operational "
                          "requirement as in the restriction field")),
         ('Private', _("Private - For dissemination only to specified addresses"
                       " as in the addresses field in the alert")),
     )
-
-    identifier = models.UUIDField(default=uuid.uuid4, editable=False, verbose_name=_("Identifier"),
-                                  help_text=_("Unique ID. Auto generated on creation."), unique=True)
+    guid = models.UUIDField(default=uuid.uuid4, editable=False, verbose_name=_("Id"),
+                            help_text=_("Unique ID. Auto generated on creation."), unique=True)
     sender = models.CharField(max_length=255, verbose_name=_("Sender"), default=get_default_sender,
                               help_text=_("Identifies the originator of an alert. "
                                           "For example the website address of the institution"))
     sent = models.DateTimeField(default=timezone.now, verbose_name=_("Sent"),
                                 help_text=_("Time and date of origination of the alert"))
     status = models.CharField(max_length=50, choices=STATUS_CHOICES, default="Actual", verbose_name=_("Status"),
                               help_text=_("The code denoting the appropriate handling of the alert"))
@@ -288,15 +290,16 @@
                 "urgency": urgency,
                 "certainty": certainty,
                 "sent": self.sent,
                 "effective": effective,
                 "expires": expires,
                 "expired": expired,
                 "properties": {
-                    "id": self.identifier,
+                    "id": self.guid,
+                    "identifier": self.identifier if hasattr(self, "identifier") else self.guid,
                     "event": event,
                     "event_type": info.value.get('event'),
                     "headline": info.value.get("headline"),
                     "severity": info.value.get("severity"),
                     "urgency": info.value.get("urgency"),
                     "certainty": info.value.get("certainty"),
                     "severity_color": severity.get("color"),
```

### Comparing `capeditor-0.5.7/capeditor/pubsub/base.py` & `capeditor-0.5.8/capeditor/pubsub/base.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/pubsub/mqtt.py` & `capeditor-0.5.8/capeditor/pubsub/mqtt.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/pubsub/publish.py` & `capeditor-0.5.8/capeditor/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/renderers.py` & `capeditor-0.5.8/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/serializers.py` & `capeditor-0.5.8/capeditor/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class AlertSerializer(serializers.ModelSerializer):
     addresses = serializers.SerializerMethodField()
     references = serializers.SerializerMethodField()
     info = serializers.SerializerMethodField()
     incidents = serializers.SerializerMethodField()
+    identifier = serializers.SerializerMethodField()
 
     class Meta:
         fields = [
             "identifier",
             "sender",
             "sent",
             "status",
@@ -42,14 +43,19 @@
             "code",
             "note",
             "references",
             "incidents",
             "info",
         ]
 
+    def get_identifier(self, obj):
+        if hasattr(obj, 'identifier'):
+            return obj.identifier
+        return obj.guid
+
     def get_info(self, obj):
         request = self.context.get("request")
         info_values = []
 
         for info in obj.info:
             info_obj = info.block.get_api_representation(info.value)
             if info.value.resource:
```

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/import_cap_preview.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/import_cap_preview.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/mapbox-gl-draw.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/maplibre-gl.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.5.8/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/fonts/mapbox-gl-draw.css` & `capeditor-0.5.8/capeditor/static/capeditor/fonts/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/alert.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/alert.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/alert.svg` & `capeditor-0.5.8/capeditor/static/capeditor/images/alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/area.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/area.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/certainty.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/certainty.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/extreme.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/extreme.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/minor.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/minor.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/moderate.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/moderate.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/images/severe.png` & `capeditor-0.5.8/capeditor/static/capeditor/images/severe.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/mapbox-gl-draw.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/mapbox-gl-draw.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/maplibre-gl.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/turf.min.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/turf.min.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-draw-widget.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-draw-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.5.8/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.5.8/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.5.8/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.5.8/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/load_cap_alert.html` & `capeditor-0.5.8/capeditor/templates/capeditor/load_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/preview_cap_alert.html` & `capeditor-0.5.8/capeditor/templates/capeditor/preview_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.5.8/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html` & `capeditor-0.5.8/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/templates/capeditor/widgets/polygon_draw_widget.html` & `capeditor-0.5.8/capeditor/templates/capeditor/widgets/polygon_draw_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/utils.py` & `capeditor-0.5.8/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/views.py` & `capeditor-0.5.8/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor/wagtail_hooks.py` & `capeditor-0.5.8/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.7/capeditor.egg-info/PKG-INFO` & `capeditor-0.5.8/capeditor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.7
+Version: 0.5.8
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -64,18 +64,17 @@
 
 - Modern user-friendly composer that follows [CAP 1.2](http://docs.oasis-open.org/emergency/cap/v1.2/CAP-v1.2-os.html)
   standard. Built on top of the awesome [Wagtail CMS](https://wagtail.org)
 - Preview a CAP alert as you edit. Save drafts for sharing with colleagues and collaborating
 - Inbuilt CAP validation. The page will not save if you have not input the required data according to CAP standard
 - User-friendly alert area map tool that allows multiple ways of constructing alert geographic areas, while keeping the
   interface simple
-    - Select country official administrative boundaries for different levels (Admin 1, Admin 2, Admin 3), with in-built
-      simplification of complex boundaries
     - Draw a polygon
     - Draw a circle
+    - Selecting predefined areas that you create beforehand for common alert areas
     - Use Geocode key values
 - Inbuilt publishing workflow using Wagtail's powerful page model, with automated emails to composers and approvers
 - Collaborate with team members using inbuilt comments (similar to how you could do in Word) with automated
   notifications. Request for changes and approvals
 - Publish realtime notifications/messages to third party integrations using MQTT messaging protocol
 - Predefine a list of hazards types monitored by your institution, with intuitive icons
   from [OCHA humanitarian icons](https://brand.unocha.org/d/xEPytAUjC3sH/icons#/humanitarian-icons)
@@ -215,29 +214,26 @@
 - Area Description (areaDesc),
 - Area Polygon/Polygons (polygon),
 - Area Circle/Circles (circle),
 - Area Geocode/Geocodes (geocode),
 - Altitude (altitude),
 - Ceiling (ceiling)
 
-The Alert area input has 4 selector options:
-
-- Admin Boundary (area is picked from predefined boundaries). To use this option, ensure that admin boundaries are
-  initially loaded. Refer to [Setting up boundaries](#setting-up-boundaries) section.
-
-![Alert Area boundary](images/alert_sections/alert_area_boundary.png "Alert Area Boundary")
+The Alert area input has multiple selector options:
 
 - Polygon (drawing a polygon)
 
 ![Alert Area polygon](images/alert_sections/alert_area_polygon.png "Alert Area Polygon")
 
 - Circle (drawing a circle which specifies the latitude, longitude and radius)
 
 ![Alert Area circle](images/alert_sections/alert_area_circle.png "Alert Area Circle")
 
+- Predefined Area (selecting a predefined area that you create beforehand for common alert areas)
+
 - Geocode (specifying area geocode name and value). Using this option presumes knowledge of the coding system
 
 ![Alert Area geocode](images/alert_sections/alert_area_geocode.png "Alert Area Geocode")
 
 #### Alert Resource
 
 Entity that defines supplemental information related to an <info> object Multiple instances of this section are allowed.
```

### Comparing `capeditor-0.5.7/capeditor.egg-info/SOURCES.txt` & `capeditor-0.5.8/capeditor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 capeditor/locale/sw/LC_MESSAGES/django.mo
 capeditor/locale/sw/LC_MESSAGES/django.po
 capeditor/migrations/0001_initial.py
 capeditor/migrations/0002_alter_capsetting_options_and_more.py
 capeditor/migrations/0003_capsetting_logo.py
 capeditor/migrations/0004_predefinedalertarea.py
 capeditor/migrations/0005_alter_capsetting_sender.py
+capeditor/migrations/0006_capsetting_wmo_oid.py
 capeditor/migrations/__init__.py
 capeditor/pubsub/__init__.py
 capeditor/pubsub/base.py
 capeditor/pubsub/mqtt.py
 capeditor/pubsub/publish.py
 capeditor/static/capeditor/css/cap_detail_page.css
 capeditor/static/capeditor/css/import_cap_preview.css
```

### Comparing `capeditor-0.5.7/setup.cfg` & `capeditor-0.5.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.5.7
+version = 0.5.8
 description = Wagtail based CAP composer
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-composer
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

