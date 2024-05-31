# Comparing `tmp/django_content_editor-7.0a3.tar.gz` & `tmp/django_content_editor-7.0a4.tar.gz`

## Comparing `django_content_editor-7.0a3.tar` & `django_content_editor-7.0a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/__init__.py
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/admin.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/contents.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/models.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/content_editor.css
--rw-r--r--   0        0        0    23376 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/content_editor.js
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/material-icons.css
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/material-icons.woff2
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/save_shortcut.js
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/content_editor/static/content_editor/tabbed_fieldsets.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/.gitignore
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/AUTHORS
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/LICENSE
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/README.rst
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-7.0a3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/__init__.py
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/admin.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/contents.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/models.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10542 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/content_editor.css
+-rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/content_editor.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/material-icons.woff2
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/save_shortcut.js
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/content_editor/static/content_editor/tabbed_fieldsets.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/.gitignore
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/AUTHORS
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/LICENSE
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/README.rst
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-7.0a4/PKG-INFO
```

### Comparing `django_content_editor-7.0a3/content_editor/admin.py` & `django_content_editor-7.0a4/content_editor/admin.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/contents.py` & `django_content_editor-7.0a4/content_editor/contents.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/models.py` & `django_content_editor-7.0a4/content_editor/models.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/ca/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/cs/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/de/LC_MESSAGES/django.mo` & `django_content_editor-7.0a4/content_editor/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/de/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/es/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/fr/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/hr/LC_MESSAGES/django.mo` & `django_content_editor-7.0a4/content_editor/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/hr/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/it/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/nb/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/nl/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/pl/LC_MESSAGES/django.mo` & `django_content_editor-7.0a4/content_editor/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/pl/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/pt/LC_MESSAGES/djangojs.po` & `django_content_editor-7.0a4/content_editor/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/pt_BR/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/ro/LC_MESSAGES/django.mo` & `django_content_editor-7.0a4/content_editor/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/ro/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/ru/LC_MESSAGES/django.mo` & `django_content_editor-7.0a4/content_editor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/ru/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/tr/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/locale/zh_CN/LC_MESSAGES/django.po` & `django_content_editor-7.0a4/content_editor/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/static/content_editor/content_editor.css` & `django_content_editor-7.0a4/content_editor/static/content_editor/content_editor.css`

 * *Files 2% similar despite different names*

```diff
@@ -180,31 +180,38 @@
 .machine-control {
 }
 
 .plugin-buttons {
   border: 1px solid var(--hairline-color, #e8e8e8);
   background: var(--darkened-bg, #f8f8f8);
   position: absolute;
-  z-index: 2;
+  z-index: 1982;
   top: 0;
   left: 0;
-  right: 10vw;
   box-shadow: 0 0 3px 0 rgba(0, 0, 50, 0.3);
 
   padding: 10px 20px 10px 10px;
 
-  column-width: 180px;
+  --_v: 8;
+  display: grid;
   column-gap: 10px;
-  column-fill: balance;
+  grid-auto-flow: column;
+  grid-template-rows: repeat(var(--_v), minmax(0, 1fr));
 
   opacity: 0;
   visibility: none;
   pointer-events: none;
 }
 
+@media screen and (max-width: 767px) {
+  .plugin-buttons {
+    display: block;
+  }
+}
+
 .plugin-buttons-visible .plugin-buttons {
   opacity: 1;
   visibility: visible;
   pointer-events: all;
 }
 
 .plugin-button {
@@ -267,25 +274,29 @@
   margin-bottom: 0;
 }
 
 #tabbed .form-row:last-child {
   border: none;
 }
 
-.content-editor-hidden {
+.content-editor-invisible {
   /* We can't simply use display: none. Some admin widgets need to know
      * their dimensions, so we can't have that -- use an alternative way
      * to hide the modules. */
   visibility: hidden !important;
   height: 0 !important;
   border: none !important;
   padding: 0 !important;
   margin: 0 !important;
 }
 
+.content-editor-hide {
+  display: none !important;
+}
+
 /* Used when dragging */
 .placeholder {
   height: 34px;
   margin: 10px 0 0 0;
   border: none;
   opacity: 0.3;
   background: #79aec8;
```

### Comparing `django_content_editor-7.0a3/content_editor/static/content_editor/content_editor.js` & `django_content_editor-7.0a4/content_editor/static/content_editor/content_editor.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -120,22 +120,25 @@
 
     const addPluginIconsToInlines = () => {
         for (const plugin of ContentEditor.plugins) {
             const fragment = document.createElement("template")
             fragment.innerHTML =
                 plugin.button || '<span class="material-icons">extension</span>'
             const button = fragment.content.firstElementChild
-            for (const title of qsa(`.dynamic-${plugin.prefix} > h3`)) {
+            for (const title of qsa(
+                    `.dynamic-${plugin.prefix} > h3, #${plugin.prefix}-empty > h3`,
+                )) {
                 title.insertAdjacentElement("afterbegin", button.cloneNode(true))
             }
         }
     }
     addPluginIconsToInlines()
 
     const orderMachineWrapper = $(".order-machine-wrapper")
+    const pluginButtons = qs(".plugin-buttons")
     const orderMachine = $(".order-machine")
     const machineEmptyMessage = $('<p class="hidden machine-message"/>')
         .text(ContentEditor.messages.empty)
         .appendTo(orderMachine)
     const noRegionsMessage = $('<p class="hidden machine-message"/>')
         .text(ContentEditor.messages.noRegions)
         .appendTo(orderMachine)
@@ -283,20 +286,25 @@
         let visible = 0
 
         buttons.forEach((button) => {
             const plugin = button.dataset.pluginPrefix
             const isVisible =
                 pluginInCurrentRegion(plugin) &&
                 !/^_unknown_/.test(ContentEditor.currentRegion)
-            button.classList.toggle("content-editor-hidden", !isVisible)
+            button.classList.toggle("content-editor-hide", !isVisible)
             visible += isVisible ? 1 : 0
         })
 
         if (visible) {
             noPluginsMessage.hide()
+
+            pluginButtons.style.setProperty(
+                "--_v",
+                Math.max(7, Math.ceil(visible / 3)),
+            )
         } else {
             if (ContentEditor.currentRegion) {
                 noPluginsMessage.show()
                 machineEmptyMessage.hide()
             }
         }
 
@@ -416,21 +424,21 @@
             const thisRow = rows[i]
             thisRow[1].value = thisRow[0].style.order = 10 * (1 + i)
         }
     }
 
     function hideInlinesFromOtherRegions() {
         const inlines = orderMachine.find(".inline-related:not(.empty-form)")
-        inlines.addClass("content-editor-hidden")
+        inlines.addClass("content-editor-invisible")
         const shown = inlines.filter(
             `[data-region="${ContentEditor.currentRegion}"]`,
         )
         machineEmptyMessage.addClass("hidden")
         if (shown.length) {
-            shown.removeClass("content-editor-hidden")
+            shown.removeClass("content-editor-invisible")
         } else {
             machineEmptyMessage.removeClass("hidden")
         }
         machineEmptyMessage.text(
             ContentEditor.messages[
                 ContentEditor.regionsByKey[ContentEditor.currentRegion].inherited ?
                 "emptyInherited" :
@@ -451,18 +459,18 @@
     pluginInlineGroups.hide()
     assignRegionDataAttribute()
 
     $(document).on(
         "click",
         ".order-machine-insert-target",
         function handleClick(e) {
-            if (e.target.classList.contains("selected")) {
-                hidePluginButtons()
+            const isSelected = e.target.classList.contains("selected")
+            hidePluginButtons()
+            if (isSelected) {
                 ContentEditor._insertBefore = null
-                e.target.classList.remove("selected")
             } else {
                 e.target.classList.add("selected")
 
                 const pos = e.target.getBoundingClientRect()
                 const buttons = qs(".plugin-buttons")
                 buttons.style.left = `${pos.left + window.scrollX + 30}px`
 
@@ -601,18 +609,18 @@
             span.className = "order-machine-insert-target"
             inline.appendChild(span)
         })
     })()
 
     $(document)
         .on("content-editor:deactivate", (event, row) => {
-            row.find("fieldset").addClass("content-editor-hidden")
+            row.find("fieldset").addClass("content-editor-invisible")
         })
         .on("content-editor:activate", (event, row) => {
-            row.find("fieldset").removeClass("content-editor-hidden")
+            row.find("fieldset").removeClass("content-editor-invisible")
         })
 
     // Hide fieldsets of to-be-deleted inlines.
     orderMachine.on(
         "click",
         ".delete>input[type=checkbox]",
         function toggleForDeletionClass() {
```

### Comparing `django_content_editor-7.0a3/content_editor/static/content_editor/material-icons.css` & `django_content_editor-7.0a4/content_editor/static/content_editor/material-icons.css`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/static/content_editor/material-icons.woff2` & `django_content_editor-7.0a4/content_editor/static/content_editor/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/content_editor/static/content_editor/tabbed_fieldsets.js` & `django_content_editor-7.0a4/content_editor/static/content_editor/tabbed_fieldsets.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,64 +1,64 @@
 /* global django */
-django.jQuery(function($) {
-    var tabbed = $(".tabbed")
+django.jQuery(($) => {
+    const tabbed = $(".tabbed")
     if (tabbed.length >= 1) {
-        var anchor = tabbed.eq(0)
+        let anchor = tabbed.eq(0)
         /* Break out of the .inline-related containment, avoids ugly h3's */
         if (anchor.parents(".inline-related").length) {
             anchor = anchor.parents(".inline-related")
         }
         anchor.before(
             '<div id="tabbed" class="clearfix">' +
             '<div class="tabs clearfix"></div>' +
             '<div class="modules tabbed-modules"></div>' +
             "</div>",
         )
 
-        var $tabs = $("#tabbed > .tabs"),
-            $modules = $("#tabbed > .modules"),
-            errorIndex = -1,
-            uncollapseIndex = -1
+        const $tabs = $("#tabbed > .tabs")
+        const $modules = $("#tabbed > .modules")
+        let errorIndex = -1
+        let uncollapseIndex = -1
 
         tabbed.each(function createTabs(index) {
-            var $old = $(this),
-                $title = $old.children("h2")
+            const $old = $(this)
+            const $title = $old.children("h2")
 
             if ($old.find(".errorlist").length) {
                 $title.addClass("has-error")
                 errorIndex = errorIndex < 0 ? index : errorIndex
             }
             if ($old.is(".uncollapse")) {
                 uncollapseIndex = uncollapseIndex < 0 ? index : uncollapseIndex
             }
 
             $title.attr("data-index", index)
             $title.addClass("tab")
             $tabs.append($title)
 
-            $old.addClass("content-editor-hidden")
+            $old.addClass("content-editor-invisible")
 
             $modules.append($old)
         })
 
         $tabs.on("click", "[data-index]", function() {
-            var $tab = $(this)
+            const $tab = $(this)
             if ($tab.hasClass("active")) {
                 $tab.removeClass("active")
-                $modules.children().addClass("content-editor-hidden")
+                $modules.children().addClass("content-editor-invisible")
             } else {
                 $tabs.find(".active").removeClass("active")
                 $tab.addClass("active")
                 $modules
                     .children()
-                    .addClass("content-editor-hidden")
+                    .addClass("content-editor-invisible")
                     .eq($tab.data("index"))
-                    .removeClass("content-editor-hidden")
+                    .removeClass("content-editor-invisible")
             }
         })
 
         if (errorIndex >= 0 || uncollapseIndex >= 0) {
-            var index = errorIndex >= 0 ? errorIndex : uncollapseIndex
-            $tabs.find("[data-index=" + index + "]").click()
+            const index = errorIndex >= 0 ? errorIndex : uncollapseIndex
+            $tabs.find(`[data-index=${index}]`).click()
         }
     }
 })
```

### Comparing `django_content_editor-7.0a3/AUTHORS` & `django_content_editor-7.0a4/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/LICENSE` & `django_content_editor-7.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/README.rst` & `django_content_editor-7.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/pyproject.toml` & `django_content_editor-7.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a3/PKG-INFO` & `django_content_editor-7.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-content-editor
-Version: 7.0a3
+Version: 7.0a4
 Summary: Editing structured content
 Project-URL: Homepage, https://github.com/matthiask/django-content-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

