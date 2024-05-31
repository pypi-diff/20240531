# Comparing `tmp/django_content_editor-6.5.1.tar.gz` & `tmp/django_content_editor-7.0a1.tar.gz`

## Comparing `django_content_editor-6.5.1.tar` & `django_content_editor-7.0a1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/__init__.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/admin.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/contents.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/models.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/content_editor.css
--rw-r--r--   0        0        0    23519 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/content_editor.js
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/material-icons.css
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/material-icons.woff2
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/save_shortcut.js
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/content_editor/static/content_editor/tabbed_fieldsets.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/.gitignore
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/AUTHORS
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/LICENSE
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/README.rst
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-6.5.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/__init__.py
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/admin.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/contents.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/models.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.css
+-rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.woff2
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/save_shortcut.js
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/tabbed_fieldsets.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/.gitignore
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/AUTHORS
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/LICENSE
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/README.rst
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/PKG-INFO
```

### Comparing `django_content_editor-6.5.1/content_editor/admin.py` & `django_content_editor-7.0a1/content_editor/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,22 +178,18 @@
                     "emptyInherited": gettext("No items. Region may inherit content."),
                     "noRegions": gettext("No regions available."),
                     "noPlugins": gettext("No plugins allowed in this region."),
                     "newItem": gettext("New item"),
                     "unknownRegion": gettext("Unknown region"),
                     "collapseAll": gettext("Collapse all items"),
                     "uncollapseAll": gettext("Uncollapse all items"),
-                    "toggleSidebar": gettext("Toggle sidebar"),
                     "forDeletion": gettext("marked for deletion"),
                     "selectMultiple": gettext(
                         "Use Ctrl-Click to select and move multiple items."
                     ),
-                    "dblclickInsertion": gettext(
-                        "Doubleclicking inserts an item at the end."
-                    ),
                 },
             }
         )
 
     def _content_editor_media(self, request, context):
         return forms.Media(
             css={
```

### Comparing `django_content_editor-6.5.1/content_editor/contents.py` & `django_content_editor-7.0a1/content_editor/contents.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/models.py` & `django_content_editor-7.0a1/content_editor/models.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/ca/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/cs/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/de/LC_MESSAGES/django.mo` & `django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/de/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/es/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/fr/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/hr/LC_MESSAGES/django.mo` & `django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/hr/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/it/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/nb/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/nl/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/pl/LC_MESSAGES/django.mo` & `django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/pl/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/pt/LC_MESSAGES/djangojs.po` & `django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/pt_BR/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/ro/LC_MESSAGES/django.mo` & `django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/ro/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/ru/LC_MESSAGES/django.mo` & `django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/ru/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/tr/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/locale/zh_CN/LC_MESSAGES/django.po` & `django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/static/content_editor/content_editor.css` & `django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.css`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,40 @@
 
 .clearfix::after {
   content: "";
   display: table;
   clear: both;
 }
 
+.tabs.regions {
+  display: flex;
+}
+
+.machine-collapse {
+  order: 1;
+  margin-left: auto;
+}
+
 .tabs > .tab {
   text-transform: none;
   letter-spacing: 0;
   float: left;
   padding: 10px 15px;
   margin: 0 4px 0 0;
   cursor: pointer;
   font-weight: bold;
   font-size: 13px;
   color: var(--body-quiet-color, #666);
   background: var(--darkened-bg, #f8f8f8);
   border: 1px solid var(--hairline-color, #e8e8e8);
   border-bottom: none;
   user-select: none;
+  transition:
+    0.15s background,
+    0.15s color;
 }
 
 .tabs > .active {
   background: var(--button-bg, #79aec8);
   color: white;
 }
 
@@ -45,33 +57,19 @@
   .tabbed-modules .form-row {
     padding-left: 10px;
     padding-right: 10px;
   }
 }
 
 .order-machine-wrapper {
-  --control-width: 220px;
   clear: both;
-  display: grid;
-  grid-template-columns: 1fr var(--control-width);
-  transition: grid-template-columns 0.2s;
-}
-
-.order-machine-wrapper.collapsed {
-  --control-width: 20px;
-}
-
-@media (min-width: 1024px) {
-  .order-machine-wrapper.collapsed {
-    --control-width: 0px;
-  }
 }
 
 .order-machine {
-  padding: 0 10px 10px 10px;
+  padding: 10px 10px 20px 30px;
   border: 1px solid var(--hairline-color, #e8e8e8);
   position: relative;
 
   display: flex;
   flex-flow: column nowrap;
 
   overflow: hidden;
@@ -89,16 +87,16 @@
   font-size: 13px;
   font-weight: normal;
   height: 16px;
   padding: 7px;
   margin: 0;
   background-color: var(--darkened-bg, #f8f8f8);
   transition:
-    0.2s background,
-    0.2s color;
+    0.15s background,
+    0.15s color;
 
   white-space: nowrap;
   overflow: hidden;
   text-overflow: ellipsis;
 
   display: flex;
   flex-flow: row nowrap;
@@ -135,18 +133,18 @@
 
 /* Replace the broken content type counter for new contents with a "new" label */
 .order-machine .last-related .inline_label {
   content: "new";
 }
 
 .order-machine .inline-related {
-  transition: border 0.2s;
+  transition: border 0.15s;
   display: grid;
   grid-template-rows: min-content 1fr;
-  transition: grid-template-rows 0.2s ease-out;
+  transition: grid-template-rows 0.15s ease-out;
 }
 
 .order-machine .inline-related fieldset {
   position: relative;
   overflow: hidden;
 }
 
@@ -179,70 +177,66 @@
 
 .machine-message {
   margin: 1.5em 1em 1em;
   text-align: center;
 }
 
 .machine-control {
+}
+
+.plugin-buttons {
   border: 1px solid var(--hairline-color, #e8e8e8);
-  border-top-right-radius: 4px;
-  border-bottom-right-radius: 4px;
   background: var(--darkened-bg, #f8f8f8);
-  position: sticky;
+  position: absolute;
+  z-index: 2;
   top: 0;
-  align-self: flex-start;
+  left: 0;
+  right: 10vw;
+  box-shadow: 0 0 3px 0 rgba(0, 0, 50, 0.3);
+
+  padding: 10px 20px 10px 10px;
 
-  width: 220px;
+  column-width: 180px;
+  column-gap: 10px;
+  column-fill: balance;
+
+  opacity: 0;
+  visibility: none;
+  pointer-events: none;
 }
 
-.plugin-buttons {
-  border-top: 1px solid var(--hairline-color, #e8e8e8);
-  margin-top: 8px;
+.plugin-buttons-visible .plugin-buttons {
+  opacity: 1;
+  visibility: visible;
+  pointer-events: all;
 }
 
 .plugin-button {
   margin: 4px 4px;
   padding: 4px 4px;
   cursor: pointer;
   display: flex;
   align-items: center;
   border-radius: 4px;
   transition: 0.1s background;
   user-select: none;
-}
-
-.plugin-button.selected {
-  background: var(--primary, #79aec8);
+  break-inside: avoid;
 }
 
 .plugin-button-icon {
   width: 24px;
   display: grid;
   place-items: center;
   margin-right: 0.75rem;
 }
 
-.toggle-sidebar,
 .collapse-items {
   cursor: pointer;
 }
 
-.toggle-sidebar .plugin-button-icon {
-  transform-origin: center;
-}
-
-.order-machine-wrapper.collapsed .toggle-sidebar .plugin-button-icon {
-  transform: scaleX(-1);
-}
-
-.order-machine-wrapper.collapsed .invisible-when-collapsed {
-  opacity: 0;
-}
-
-.toggle-sidebar input,
 .collapse-items input {
   display: none;
 }
 
 .collapse-items .uncollapse-all {
   display: none;
 }
@@ -338,55 +332,54 @@
   bottom: 0;
   left: 0;
   z-index: 1;
 }
 
 .order-machine-insert-target {
   position: absolute;
-  left: 48%;
-  top: -0.9em;
-  font-size: 1.5rem;
+  left: -28px;
+  top: -20px;
+  font-size: 1.25rem;
   width: 1.25em;
   height: 1.25em;
   line-height: 1.25em;
   border-radius: 99px;
   background: var(--button-bg, #79aec8);
   color: var(--button-fg, #fff);
   box-shadow: 0 0 3px 1px var(--button-fg);
   display: grid;
   place-items: center;
   cursor: pointer;
-  opacity: 0;
-  pointer-events: none;
+  opacity: 0.5;
+  transition:
+    color 0.15s,
+    background 0.15s,
+    opacity,
+    0.15s;
 }
 .order-machine-insert-target.last {
   top: auto;
-  bottom: 2px;
-  left: 48.2%;
+  bottom: 3px;
+  left: 2px;
   z-index: 1;
 }
-.order-machine-insertion .order-machine-insert-target {
-  opacity: 0.5;
-  pointer-events: all;
-  transition: opacity 0.1s;
-}
-.order-machine-insert-target:hover {
+.order-machine-insert-target:hover,
+.order-machine-insert-target.selected {
   opacity: 1;
   background: var(--button-hover-bg, #609ab6);
 }
 .order-machine-insert-target::before {
-  content: "→";
+  content: "+";
   font-weight: bold;
 }
 
 @media screen and (max-width: 767px) {
   /* CSS fix for Django's responsive admin interface (shows fields below the
    * 767px breakpoint despite them being .hidden */
-  html .aligned .form-row.hidden,
-  .toggle-sidebar {
+  html .aligned .form-row.hidden {
     display: none;
   }
 
   html .aligned .form-row > div {
     width: calc(100vw - 90px);
   }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_content_editor-6.5.1/content_editor/static/content_editor/content_editor.js` & `django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /* global django,ContentEditor */
 
-django.jQuery(function($) {
+django.jQuery(($) => {
     const context = document.getElementById("content-editor-context")
     if (!context) return
 
     function qs(sel, ctx = document) {
         return ctx.querySelector(sel)
     }
 
@@ -30,47 +30,30 @@
             },
         }
     }
 
     const LS = safeStorage(localStorage)
     const SS = safeStorage(sessionStorage)
 
-    function unselectSelectedPlugin() {
-        qsa(".plugin-button.selected").forEach((btn) =>
-            btn.classList.remove("selected"),
-        )
-        qs(".order-machine").classList.remove("order-machine-insertion")
-    }
-
-    document.body.addEventListener("keyup", (e) => {
-        if (e.key === "Escape") unselectSelectedPlugin()
-    })
-
     window.ContentEditor = {
         addContent: function addContent(prefix) {
-            $("#" + prefix + "-group .add-row a").click()
+            $(`#${prefix}-group .add-row a`).click()
         },
         addPluginButton: function addPluginButton(prefix, iconHTML) {
             const plugin = ContentEditor.pluginsByPrefix[prefix]
             if (!plugin) return
 
             const button = document.createElement("a")
             button.dataset.pluginPrefix = plugin.prefix
             button.className = "plugin-button"
             button.title = plugin.title
-            button.addEventListener("click", function(e) {
+            button.addEventListener("click", (e) => {
                 e.preventDefault()
-                if (button.classList.contains("selected")) {
-                    button.classList.remove("selected")
-                    ContentEditor.addContent(plugin.prefix)
-                } else {
-                    unselectSelectedPlugin()
-                    button.classList.add("selected")
-                    qs(".order-machine").classList.add("order-machine-insertion")
-                }
+                ContentEditor.addContent(plugin.prefix)
+                orderMachineWrapper.removeClass("plugin-buttons-visible")
             })
 
             const icon = document.createElement("span")
             icon.className = "plugin-button-icon"
             icon.innerHTML =
                 iconHTML || '<span class="material-icons">extension</span>'
             button.appendChild(icon)
@@ -86,44 +69,32 @@
             hideNotAllowedPluginButtons([button])
         },
     }
 
     $.extend(window.ContentEditor, JSON.parse(context.dataset.context))
 
     ContentEditor.pluginsByPrefix = {}
-    ContentEditor.plugins.forEach(function(plugin) {
+    ContentEditor.plugins.forEach((plugin) => {
         ContentEditor.pluginsByPrefix[plugin.prefix] = plugin
     })
     ContentEditor.regionsByKey = {}
-    ContentEditor.regions.forEach(function(region) {
+    ContentEditor.regions.forEach((region) => {
         ContentEditor.regionsByKey[region.key] = region
     })
 
     // Add basic structure. There is always at least one inline group if
     // we even have any plugins.
     let $anchor = $(".inline-group:first")
     if (ContentEditor.plugins.length) {
-        $anchor = $("#" + ContentEditor.plugins[0].prefix + "-group")
+        $anchor = $(`#${ContentEditor.plugins[0].prefix}-group`)
     }
     $anchor.before(
         `
-    <div class="tabs regions"></div>
-    <div class="module order-machine-wrapper">
-      <div class="order-machine">
-        <span class="order-machine-insert-target last"></span>
-      </div>
-      <div class="machine-control">
-        <label class="toggle-sidebar">
-          <div class="plugin-button">
-            <span class="plugin-button-icon">
-              <span class="material-icons">chevron_right</span>
-            </span>
-            <input type="checkbox" />${ContentEditor.messages.toggleSidebar}
-          </div>
-        </label>
+    <div class="tabs regions">
+      <div class="machine-collapse">
         <label class="collapse-items">
           <input type="checkbox" />
           <div class="plugin-button collapse-all">
             <span class="plugin-button-icon">
               <span class="material-icons">unfold_less</span>
             </span>
             ${ContentEditor.messages.collapseAll}
@@ -131,37 +102,42 @@
           <div class="plugin-button uncollapse-all">
             <span class="plugin-button-icon">
               <span class="material-icons">unfold_more</span>
             </span>
             ${ContentEditor.messages.uncollapseAll}
           </div>
         </label>
-        <div class="plugin-buttons"></div>
-        <p class="small invisible-when-collapsed">${ContentEditor.messages.dblclickInsertion}</p>
       </div>
     </div>
+    <div class="module order-machine-wrapper">
+      <div class="order-machine">
+        <span class="order-machine-insert-target last"></span>
+      </div>
+      <div class="plugin-buttons"></div>
+    </div>
     <p class="order-machine-help">${ContentEditor.messages.selectMultiple}</p>
     `,
     )
 
-    const orderMachine = $(".order-machine"),
-        machineEmptyMessage = $('<p class="hidden machine-message"/>')
+    const orderMachineWrapper = $(".order-machine-wrapper")
+    const orderMachine = $(".order-machine")
+    const machineEmptyMessage = $('<p class="hidden machine-message"/>')
         .text(ContentEditor.messages.empty)
-        .appendTo(orderMachine),
-        noRegionsMessage = $('<p class="hidden machine-message"/>')
+        .appendTo(orderMachine)
+    const noRegionsMessage = $('<p class="hidden machine-message"/>')
         .text(ContentEditor.messages.noRegions)
-        .appendTo(orderMachine),
-        noPluginsMessage = $('<p class="hidden machine-message"/>')
+        .appendTo(orderMachine)
+    const noPluginsMessage = $('<p class="hidden machine-message"/>')
         .text(ContentEditor.messages.noPlugins)
         .appendTo(orderMachine)
 
     // Pre map plugin regions
-    const pluginRegions = (function() {
+    const pluginRegions = (() => {
         const result = {}
-        ContentEditor.plugins.forEach(function(plugin) {
+        ContentEditor.plugins.forEach((plugin) => {
             result[plugin.prefix] = plugin.regions
         })
         const plugins = ContentEditor.plugins
         for (let i = 0; i < plugins.length; i++) {
             result[plugins[i].prefix] = plugins[i].regions
         }
         return result
@@ -174,15 +150,15 @@
     }
 
     function ensureDraggable(arg) {
         if (arg.hasClass("empty-form") || arg.hasClass("fs-draggable")) return
 
         const inline = arg[0]
 
-        inline.addEventListener("dragstart", function(e) {
+        inline.addEventListener("dragstart", (e) => {
             // Only handle events from [draggable] elements
             if (!e.target.closest("h3[draggable]")) return
 
             // window.__fs_dragging = inline;
             window.__fs_dragging = e.target.closest(".inline-related")
             window.__fs_dragging.classList.add("fs-dragging")
             window.__fs_dragging.classList.add("selected")
@@ -191,38 +167,38 @@
             e.dataTransfer.effectAllowed = "move"
             try {
                 e.dataTransfer.setData("text/plain", "")
             } catch (e) {
                 // IE11 needs this.
             }
         })
-        inline.addEventListener("dragend", function() {
+        inline.addEventListener("dragend", () => {
             $(".fs-dragging").removeClass("fs-dragging")
             $(".fs-dragover").removeClass("fs-dragover")
             qsa(".order-machine .inline-related.selected").forEach((el) =>
                 el.classList.remove("selected"),
             )
         })
         inline.addEventListener(
             "dragover",
-            function(e) {
+            (e) => {
                 if (window.__fs_dragging) {
                     e.preventDefault()
                     $(".fs-dragover").removeClass("fs-dragover")
                     const inline = e.target.closest(".inline-related")
                     inline.classList.add("fs-dragover")
                     inline.classList.toggle(
                         "fs-dragover--after",
                         shouldInsertAfter(inline, e.clientY),
                     )
                 }
             },
             true,
         )
-        inline.addEventListener("drop", function(e) {
+        inline.addEventListener("drop", (e) => {
             if (window.__fs_dragging) {
                 e.preventDefault()
                 const inline = e.target.closest(".inline-related")
                 const toMove = qsa(".order-machine .inline-related.selected").map(
                     (inline) => [inline, +inline.style.order],
                 )
                 const orAfter = shouldInsertAfter(inline, e.clientY)
@@ -236,16 +212,15 @@
         })
 
         arg.find(">h3, .card-title").attr("draggable", true) // Default admin, Jazzmin
         arg.addClass("fs-draggable")
     }
 
     function reorderInlines(context) {
-        context = context || orderMachine
-        const inlines = context.find(".inline-related")
+        const inlines = (context || orderMachine).find(".inline-related")
         inlines.not(".empty-form").each(function() {
             $(document).trigger("content-editor:deactivate", [$(this)])
 
             ensureDraggable($(this))
         })
 
         inlines.detach()
@@ -285,20 +260,20 @@
         const plugin = ContentEditor.pluginsByPrefix[prefix]
         const regions = plugin.regions || Object.keys(ContentEditor.regionsByKey)
         return regions.includes(ContentEditor.currentRegion)
     }
 
     // Hide not allowed plugin buttons
     // If buttons only checks this buttons, else checks all
-    function hideNotAllowedPluginButtons(buttons) {
-        buttons = buttons ? buttons : qsa(".plugin-buttons .plugin-button")
+    function hideNotAllowedPluginButtons(_buttons) {
+        const buttons = _buttons ? _buttons : qsa(".plugin-buttons .plugin-button")
 
         let visible = 0
 
-        buttons.forEach(function(button) {
+        buttons.forEach((button) => {
             const plugin = button.dataset.pluginPrefix
             const isVisible =
                 pluginInCurrentRegion(plugin) &&
                 !/^_unknown_/.test(ContentEditor.currentRegion)
             button.classList.toggle("content-editor-hidden", !isVisible)
             visible += isVisible ? 1 : 0
         })
@@ -342,22 +317,22 @@
             ) {
                 regions.push(ContentEditor.regions[i])
             }
         }
 
         if (regions.length < 2 && !/^_unknown_/.test($inline.data("region"))) return
 
-        const select = buildDropdown(regions),
-            regionInput = $inline.find(".field-region input")
+        const select = buildDropdown(regions)
+        const regionInput = $inline.find(".field-region input")
 
         select.className = "inline_move_to_region"
         select.value = regionInput.val()
         $inline.find("> h3 .inline_label").after(select)
 
-        select.addEventListener("change", function() {
+        select.addEventListener("change", () => {
             $inline.attr("data-region", select.value)
             regionInput.val(select.value)
             hideInlinesFromOtherRegions()
             setBiggestOrdering($inline)
             reorderInlines()
         })
     }
@@ -390,59 +365,55 @@
             attachMoveToRegionDropdown($this)
         })
     }
 
     function setBiggestOrdering($row) {
         const orderings = []
         orderMachine.find(".field-ordering input").each(function() {
-            if (!isNaN(+this.value)) orderings.push(+this.value)
+            if (!Number.isNaN(+this.value)) orderings.push(+this.value)
         })
         const ordering = 10 + Math.max.apply(null, orderings)
         $row.find(".field-ordering input").val(ordering)
         $row.css("order", ordering)
     }
 
     function insertAdjacent(row, inline, after = false) {
-        const inlineOrdering = +qs(".field-ordering input", inline).value,
-            beforeRows = [],
-            afterRows = []
+        const inlineOrdering = +qs(".field-ordering input", inline).value
+        const beforeRows = []
+        const afterRows = []
         orderMachine.find(".inline-related:not(.empty-form)").each(function() {
             const thisOrderingField = qs(".field-ordering input", this)
-            if (this != row && !isNaN(+thisOrderingField.value)) {
+            if (this !== row && !Number.isNaN(+thisOrderingField.value)) {
                 if (
                     after ?
                     +thisOrderingField.value > inlineOrdering :
                     +thisOrderingField.value >= inlineOrdering
                 ) {
                     afterRows.push([this, thisOrderingField])
                 } else {
                     beforeRows.push([this, thisOrderingField])
                 }
             }
         })
-        beforeRows.sort(function(a, b) {
-            return a[1].value - b[1].value
-        })
-        afterRows.sort(function(a, b) {
-            return a[1].value - b[1].value
-        })
+        beforeRows.sort((a, b) => a[1].value - b[1].value)
+        afterRows.sort((a, b) => a[1].value - b[1].value)
         let rows = [].concat(beforeRows)
         rows.push([row, qs(".field-ordering input", row)])
         rows = rows.concat(afterRows)
         for (let i = 0; i < rows.length; ++i) {
             const thisRow = rows[i]
             thisRow[1].value = thisRow[0].style.order = 10 * (1 + i)
         }
     }
 
     function hideInlinesFromOtherRegions() {
         const inlines = orderMachine.find(".inline-related:not(.empty-form)")
         inlines.addClass("content-editor-hidden")
         const shown = inlines.filter(
-            '[data-region="' + ContentEditor.currentRegion + '"]',
+            `[data-region="${ContentEditor.currentRegion}"]`,
         )
         machineEmptyMessage.addClass("hidden")
         if (shown.length) {
             shown.removeClass("content-editor-hidden")
         } else {
             machineEmptyMessage.removeClass("hidden")
         }
@@ -454,32 +425,50 @@
             ],
         )
     }
 
     const pluginInlineGroups = (function selectPluginInlineGroups() {
         const selector = []
         for (let i = 0; i < ContentEditor.plugins.length; i++) {
-            selector.push("#" + ContentEditor.plugins[i].prefix + "-group")
+            selector.push(`#${ContentEditor.plugins[i].prefix}-group`)
         }
         return $(selector.join(", "))
     })()
 
     reorderInlines(pluginInlineGroups)
     pluginInlineGroups.hide()
     assignRegionDataAttribute()
 
     $(document).on(
         "click",
         ".order-machine-insert-target",
-        function handleInsertion(e) {
-            const plugin = qs(".plugin-button.selected")
-            if (!plugin) return
+        function handleClick(e) {
+            if (e.target.classList.contains("selected")) {
+                hidePluginButtons()
+                ContentEditor._insertBefore = null
+                e.target.classList.remove("selected")
+            } else {
+                e.target.classList.add("selected")
+
+                const pos = e.target.getBoundingClientRect()
+                const buttons = qs(".plugin-buttons")
+                buttons.style.left = `${pos.left + window.scrollX + 30}px`
+
+                const y =
+                    pos.top +
+                    window.scrollY +
+                    (e.target.classList.contains("last") ?
+                        30 - buttons.getBoundingClientRect().height :
+                        0)
+                buttons.style.top = `${y}px`
+
+                orderMachineWrapper.addClass("plugin-buttons-visible")
 
-            ContentEditor._insertBefore = e.target.closest(".inline-related")
-            ContentEditor.addContent(plugin.dataset.pluginPrefix)
+                ContentEditor._insertBefore = e.target.closest(".inline-related")
+            }
         },
     )
 
     // Always move empty forms to the end, because new plugins are inserted
     // just before its empty form. Also, assign region data.
     function handleFormsetAdded($row, prefix) {
         // Not one of our managed inlines?
@@ -507,56 +496,56 @@
 
     function handleFormsetRemoved(prefix) {
         // Not one of our managed inlines?
         if (!ContentEditor.pluginsByPrefix[prefix]) return
 
         if (
             !orderMachine.find(
-                '.inline-related[data-region="' + ContentEditor.currentRegion + '"]',
+                `.inline-related[data-region="${ContentEditor.currentRegion}"]`,
             ).length
         ) {
             machineEmptyMessage.removeClass("hidden")
         }
         orderMachine
             .find(".inline-related.last-related:not(.empty-form)")
             .each(function() {
                 $(document).trigger("content-editor:deactivate", [$(this)])
             })
 
         // As soon as possible, but not sooner (let the inline.js code run to the end first)
-        setTimeout(function() {
+        setTimeout(() => {
             orderMachine
                 .find(".inline-related.last-related:not(.empty-form)")
                 .each(function() {
                     $(document).trigger("content-editor:activate", [$(this)])
                 })
         }, 0)
     }
 
-    $(document).on("formset:added", function(event, $row, formsetName) {
-        if (event.detail && event.detail.formsetName) {
+    $(document).on("formset:added", (event, $row, formsetName) => {
+        if (event.detail?.formsetName) {
             // Django >= 4.1
             handleFormsetAdded($(event.target), event.detail.formsetName)
         } else {
             handleFormsetAdded($row, formsetName)
         }
     })
 
-    $(document).on("formset:removed", function(event, $row, formsetName) {
-        if (event.detail && event.detail.formsetName) {
+    $(document).on("formset:removed", (event, $row, formsetName) => {
+        if (event.detail?.formsetName) {
             // Django >= 4.1
             handleFormsetRemoved(event.detail.formsetName)
         } else {
             handleFormsetRemoved(formsetName)
         }
     })
 
     // Initialize tabs and currentRegion.
     ;
-    (function() {
+    (() => {
         const tabContainer = $(".tabs.regions")
         for (let i = 0; i < ContentEditor.regions.length; i++) {
             const t = document.createElement("h2")
             t.className = "tab"
             t.textContent = ContentEditor.regions[i].title
             t.setAttribute("data-region", ContentEditor.regions[i].key)
             tabContainer.append(t)
@@ -564,15 +553,15 @@
 
         const tabs = tabContainer.find("h2")
         tabs.on("click", function() {
             ContentEditor.currentRegion = $(this).data("region")
             hideInlinesFromOtherRegions()
             tabs
                 .removeClass("active")
-                .filter('[data-region="' + ContentEditor.currentRegion + '"]')
+                .filter(`[data-region="${ContentEditor.currentRegion}"]`)
                 .addClass("active")
 
             // Make sure only allowed plugins are in select
             hideNotAllowedPluginButtons()
         })
 
         const collapseAllInput = $(".collapse-items input")
@@ -588,36 +577,28 @@
                     function uncollapseInvalidFieldsets() {
                         this.closest(".inline-related").classList.remove("collapsed")
                     },
                 )
             }
         })
         collapseAllInput.attr("checked", LS.get("collapseAll")).trigger("change")
-
-        const toggleSidebar = $(".toggle-sidebar input")
-        const omWrapper = document.querySelector(".order-machine-wrapper")
-        toggleSidebar.on("change", function() {
-            omWrapper.classList.toggle("collapsed", this.checked)
-            LS.set("collapseSidebar", this.checked)
-        })
-        toggleSidebar.attr("checked", LS.get("collapseSidebar")).trigger("change")
     })();
     (function initializeInsertTargets() {
         qsa(".order-machine .inline-related").forEach((inline) => {
             const span = document.createElement("span")
             span.className = "order-machine-insert-target"
             inline.appendChild(span)
         })
     })()
 
     $(document)
-        .on("content-editor:deactivate", function(event, row) {
+        .on("content-editor:deactivate", (event, row) => {
             row.find("fieldset").addClass("content-editor-hidden")
         })
-        .on("content-editor:activate", function(event, row) {
+        .on("content-editor:activate", (event, row) => {
             row.find("fieldset").removeClass("content-editor-hidden")
         })
 
     // Hide fieldsets of to-be-deleted inlines.
     orderMachine.on(
         "click",
         ".delete>input[type=checkbox]",
@@ -655,20 +636,31 @@
         } else {
             e.target.textContent = window.gettext("Show")
             fieldset.classList.add("collapsed")
         }
     })
 
     // Unselect the currently selected plugin
-    $(document.body).on("click", function removeSelected(e) {
+    const hidePluginButtons = () => {
+        orderMachineWrapper.removeClass("plugin-buttons-visible")
+        for (const el of qsa(".order-machine-insert-target.selected")) {
+            el.classList.remove("selected")
+        }
+    }
+
+    document.body.addEventListener("keyup", (e) => {
+        if (e.key === "Escape") hidePluginButtons()
+    })
+
+    document.body.addEventListener("click", (e) => {
         if (
-            !e.target.closest(".plugin-button") &&
-            !e.target.closest(".order-machine-insert-target")
+            !e.target.closest(".order-machine-insert-target") &&
+            !e.target.closest(".plugin-buttons")
         ) {
-            unselectSelectedPlugin()
+            hidePluginButtons()
         }
     })
 
     const saveEditorState = () => {
         SS.set(location.pathname, {
             region: ContentEditor.currentRegion,
             scrollY: window.scrollY,
@@ -677,30 +669,30 @@
             ).map((inline) => {
                 return qs(".field-ordering input", inline).value
             }),
         })
     }
 
     const restoreEditorState = () => {
-        let tabs = $(".tabs.regions .tab")
+        const tabs = $(".tabs.regions .tab")
 
         const state = location.hash.includes("restore") ?
             SS.get(location.pathname) :
             null
         if (state) {
-            let tab = tabs.filter(`[data-region="${state.region}"]`)
+            const tab = tabs.filter(`[data-region="${state.region}"]`)
             if (tab.length) {
                 tab.click()
             } else {
                 tabs.eq(0).click()
             }
 
             qsa(".order-machine .inline-related:not(.empty-form)").forEach(
                 (inline) => {
-                    let collapsed = state.collapsed.includes(
+                    const collapsed = state.collapsed.includes(
                         qs(".field-ordering input", inline).value,
                     )
                     inline.classList.toggle("collapsed", collapsed)
                 },
             )
 
             setTimeout(() => {
@@ -713,15 +705,15 @@
 
     $("form").submit(function() {
         this.action += "#restore"
         saveEditorState()
     })
     setTimeout(restoreEditorState, 1)
 
-    ContentEditor.plugins.forEach(function(plugin) {
+    ContentEditor.plugins.forEach((plugin) => {
         ContentEditor.addPluginButton(plugin.prefix, plugin.button)
     })
 
     const style = document.createElement("style")
     style.textContent = `
 .order-machine .inline-related .inline_label::after {
   content: "(${window.gettext("Hide")})";
```

### Comparing `django_content_editor-6.5.1/content_editor/static/content_editor/material-icons.css` & `django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.css`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/static/content_editor/material-icons.woff2` & `django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/content_editor/static/content_editor/tabbed_fieldsets.js` & `django_content_editor-7.0a1/content_editor/static/content_editor/tabbed_fieldsets.js`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/AUTHORS` & `django_content_editor-7.0a1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/LICENSE` & `django_content_editor-7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/README.rst` & `django_content_editor-7.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/pyproject.toml` & `django_content_editor-7.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.5.1/PKG-INFO` & `django_content_editor-7.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-content-editor
-Version: 6.5.1
+Version: 7.0a1
 Summary: Editing structured content
 Project-URL: Homepage, https://github.com/matthiask/django-content-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

