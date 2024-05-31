# Comparing `tmp/django_content_editor-7.0a1.tar.gz` & `tmp/django_content_editor-7.0a2.tar.gz`

## Comparing `django_content_editor-7.0a1.tar` & `django_content_editor-7.0a2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/__init__.py
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/admin.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/contents.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/models.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.css
--rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.js
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.css
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.woff2
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/save_shortcut.js
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/content_editor/static/content_editor/tabbed_fieldsets.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/.gitignore
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/AUTHORS
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/LICENSE
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/README.rst
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-7.0a1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/__init__.py
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/admin.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/contents.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/models.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/content_editor.css
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/content_editor.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/material-icons.woff2
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/save_shortcut.js
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/content_editor/static/content_editor/tabbed_fieldsets.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/.gitignore
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/AUTHORS
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/LICENSE
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/README.rst
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-7.0a2/PKG-INFO
```

### Comparing `django_content_editor-7.0a1/content_editor/admin.py` & `django_content_editor-7.0a2/content_editor/admin.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/contents.py` & `django_content_editor-7.0a2/content_editor/contents.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/models.py` & `django_content_editor-7.0a2/content_editor/models.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/ca/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/cs/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.mo` & `django_content_editor-7.0a2/content_editor/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/de/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/es/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/fr/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.mo` & `django_content_editor-7.0a2/content_editor/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/hr/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/it/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/nb/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/nl/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.mo` & `django_content_editor-7.0a2/content_editor/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/pl/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/pt/LC_MESSAGES/djangojs.po` & `django_content_editor-7.0a2/content_editor/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/pt_BR/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.mo` & `django_content_editor-7.0a2/content_editor/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/ro/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.mo` & `django_content_editor-7.0a2/content_editor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/ru/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/tr/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/locale/zh_CN/LC_MESSAGES/django.po` & `django_content_editor-7.0a2/content_editor/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.css` & `django_content_editor-7.0a2/content_editor/static/content_editor/content_editor.css`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/static/content_editor/content_editor.js` & `django_content_editor-7.0a2/content_editor/static/content_editor/content_editor.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -45,15 +45,15 @@
             const button = document.createElement("a")
             button.dataset.pluginPrefix = plugin.prefix
             button.className = "plugin-button"
             button.title = plugin.title
             button.addEventListener("click", (e) => {
                 e.preventDefault()
                 ContentEditor.addContent(plugin.prefix)
-                orderMachineWrapper.removeClass("plugin-buttons-visible")
+                hidePluginButtons()
             })
 
             const icon = document.createElement("span")
             icon.className = "plugin-button-icon"
             icon.innerHTML =
                 iconHTML || '<span class="material-icons">extension</span>'
             button.appendChild(icon)
```

### Comparing `django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.css` & `django_content_editor-7.0a2/content_editor/static/content_editor/material-icons.css`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/static/content_editor/material-icons.woff2` & `django_content_editor-7.0a2/content_editor/static/content_editor/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/content_editor/static/content_editor/tabbed_fieldsets.js` & `django_content_editor-7.0a2/content_editor/static/content_editor/tabbed_fieldsets.js`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/AUTHORS` & `django_content_editor-7.0a2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/LICENSE` & `django_content_editor-7.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/README.rst` & `django_content_editor-7.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/pyproject.toml` & `django_content_editor-7.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_content_editor-7.0a1/PKG-INFO` & `django_content_editor-7.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-content-editor
-Version: 7.0a1
+Version: 7.0a2
 Summary: Editing structured content
 Project-URL: Homepage, https://github.com/matthiask/django-content-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

