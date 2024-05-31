# Comparing `tmp/mkdocs_print_site_plugin-2.4.1.tar.gz` & `tmp/mkdocs_print_site_plugin-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_print_site_plugin-2.4.1.tar", last modified: Wed May  8 13:58:24 2024, max compression
+gzip compressed data, was "mkdocs_print_site_plugin-2.5.0.tar", last modified: Fri May 31 19:19:27 2024, max compression
```

## Comparing `mkdocs_print_site_plugin-2.4.1.tar` & `mkdocs_print_site_plugin-2.5.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.011146 mkdocs_print_site_plugin-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.003146 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-material.css
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-readthedocs.css
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site.css
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/js/print-site.js
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/templates/cover_page.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/templates/print_site_banner.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 13:58:23.000000 mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:58:24.011146 mkdocs_print_site_plugin-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:58:24.007146 mkdocs_print_site_plugin-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/tests/test_building.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/tests/test_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-05-08 13:57:51.000000 mkdocs_print_site_plugin-2.4.1/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.970360 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-material.css
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-readthedocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-31 19:18:59.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/js/print-site.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/templates/cover_page.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/templates/print_site_banner.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 19:19:27.000000 mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:27.974360 mkdocs_print_site_plugin-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/tests/test_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/tests/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-05-31 19:19:00.000000 mkdocs_print_site_plugin-2.5.0/tests/test_urls.py
```

### Comparing `mkdocs_print_site_plugin-2.4.1/LICENSE` & `mkdocs_print_site_plugin-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/PKG-INFO` & `mkdocs_print_site_plugin-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.4.1
+Version: 2.5.0
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs-material>=7.3.0
```

### Comparing `mkdocs_print_site_plugin-2.4.1/README.md` & `mkdocs_print_site_plugin-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings1.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings1.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings2.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings2.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings3.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings3.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings4.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings4.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings5.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings5.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-enum-headings6.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-enum-headings6.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-material.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-material.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-mkdocs.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-mkdocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site-readthedocs.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site-readthedocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/css/print-site.css` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/css/print-site.css`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/exclude.py` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/js/print-site.js` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/js/print-site.js`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/plugin.py` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,27 +212,14 @@
         if not self.config.get("enabled"):
             return html
 
         # Save each page HTML *before* a template is applied inside the page class
         if page != self.print_page:
             page.html = html
 
-        # We need to validate that the first heading on each page is a h1
-        # This is required for the print page table of contents and enumeration logic
-        if self.config.get("add_table_of_contents") or self.config.get(
-            "enumerate_headings"
-        ):
-            if page in self.all_pages_in_nav:
-                match = re.search(r"\<h[0-6]", html)
-                if match:
-                    if not match.group() == "<h1":
-                        msg = f"The page {page.title} ({page.file.src_path}) does not start with a level 1 heading."
-                        msg += "This is required for print page Table of Contents and/or enumeration of headings."
-                        raise AssertionError(msg)
-
         # Link to the PDF version of the entire site on a page.
         if self.config.get("path_to_pdf") != "":
             pdf_url = self.config.get("path_to_pdf")
             if is_external(pdf_url):
                 page.url_to_pdf = pdf_url
             else:
                 page.url_to_pdf = get_relative_url(
```

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/renderer.py` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import jinja2
 import logging
 
 from mkdocs.structure.toc import AnchorLink, TableOfContents
 
 from mkdocs_print_site_plugin.urls import (
     fix_internal_links,
@@ -17,24 +18,24 @@
     """
     Renders the print site page.
     """
 
     def __init__(
         self,
         plugin_config,
-        mkdocs_config={},
+        mkdocs_config=None,
         cover_page_template_path="",
         banner_template_path="",
         print_page=None,
     ):
         """
         Inits the class.
         """
         self.plugin_config = plugin_config
-        self.mkdocs_config = mkdocs_config
+        self.mkdocs_config = mkdocs_config or {}
         self.cover_page_template_path = cover_page_template_path
         self.banner_template_path = banner_template_path
         self.print_page = print_page
 
         self.items = []
 
     def _get_items(self):
@@ -72,59 +73,76 @@
 
         def get_html_from_items(
             items: list, dir_urls: bool, excluded_pages: list, section_depth: int = 0
         ) -> str:
             """
             Get all the HTML from the pages.
             """
-            item_html = ""
+            items_html = ""
 
             for item in items:
                 if item.is_page:
                     # Do not include page in print page if excluded
                     if exclude(item.file.src_path, excluded_pages):
-                        logging.debug("Excluding page " + item.file.src_path)
+                        logging.debug(f"Excluding page '{item.file.src_path}'")
                         continue
 
                     # If you specify the same page twice in your navigation, it is only rendered once
                     # so we need to check if the html attribute exists
                     if hasattr(item, "html"):
                         if item.html == "":
-                            logger.warning(
-                                "[mkdocs-print-site] %s is empty and will be ignored"
-                                % item.file.src_path
-                            )
+                            logger.warning(f"[mkdocs-print-site] {item.file.src_path} is empty and will be ignored")
                             continue
+
+                        item_html = item.html
+                        
+                        # Add missing h1 tag if the first heading is not a h1
+                        match = re.search(r"\<h[0-6]", item_html)
+                        if match:
+                            if not match.group() == "<h1":
+                                item_html = f"<h1 id=\"{to_snake_case(item.title)}\">{item.title}</h1>{item_html}"
+                                logger.warning(f"[mkdocs-print-site] '{item.file.src_path}' file is missing a leading h1 tag. Added to the print-page with title '{item.title}'")
+                            
+                        # Support mkdocs-material tags
+                        # See https://squidfunk.github.io/mkdocs-material/plugins/tags
+                        if "tags" in item.meta:
+                            tags = item.meta["tags"]
+                            tags_html = "<nav class='md-tags'>"
+                            for tag in tags:
+                                tags_html += f"<span class='md-tag'>{tag}</span>"
+                            tags_html += "</nav>"
+                            item_html = tags_html + item_html
+                        
                         # Update internal anchor links, image urls, etc
-                        item_html += fix_internal_links(
-                            item.html, item.url, directory_urls=dir_urls
+                        items_html += fix_internal_links(
+                            item_html, item.url, directory_urls=dir_urls
                         )
 
                 if item.is_section:
-                    item_html += """
+                    items_html += """
                         <h%s class='nav-section-title' id='section-%s'>
                             %s <a class='headerlink' href='#section-%s' title='Permanent link'>↵</a>
                         </h%s>
                         """ % (
                         min(6, section_depth + 1),
                         to_snake_case(item.title),
                         item.title,
                         to_snake_case(item.title),
                         min(6, section_depth + 1),
                     )
-                    item_html += get_html_from_items(
+                    items_html += get_html_from_items(
                         item.children, dir_urls, excluded_pages, section_depth + 1
                     )
                     # We also need to indicate the end of section page
                     # We do that using a h1 with a specific class
                     # In CSS we display:none, in JS we can use it for formatting the table of contents.
-                    item_html += (
+                    items_html += (
                         "<h1 class='nav-section-title-end'>Ended: %s</h1>" % item.title
                     )
-            return item_html
+            return items_html
 
         html += get_html_from_items(
             self._get_items(),
             dir_urls=self.mkdocs_config.get("use_directory_urls"),
             excluded_pages=self.plugin_config.get("exclude", []),
         )
```

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/templates/cover_page.tpl` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/templates/cover_page.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/templates/print_site_banner.tpl` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/templates/print_site_banner.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/urls.py` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin/utils.py` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/PKG-INFO` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.4.1
+Version: 2.5.0
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs-material>=7.3.0
```

### Comparing `mkdocs_print_site_plugin-2.4.1/mkdocs_print_site_plugin.egg-info/SOURCES.txt` & `mkdocs_print_site_plugin-2.5.0/mkdocs_print_site_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_print_site_plugin-2.4.1/setup.py` & `mkdocs_print_site_plugin-2.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = ""
     for line in f:
         long_description += line
 
 
 setup(
     name="mkdocs-print-site-plugin",
-    version="2.4.1",
+    version="2.5.0",
     description="MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin print pdf",
     url="https://github.com/timvink/mkdocs-print-site-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
@@ -25,14 +25,15 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Topic :: Documentation",
         "Topic :: Text Processing",
     ],
     install_requires=["mkdocs-material>=7.3.0"],
     packages=find_packages(),
     entry_points={
```

### Comparing `mkdocs_print_site_plugin-2.4.1/tests/test_building.py` & `mkdocs_print_site_plugin-2.5.0/tests/test_building.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,18 +265,25 @@
     # Make sure the subsection pages are also in the page.
     assert text_in_page(prj_path, "print_page/index.html", "Subsec 1")
     assert text_in_page(prj_path, "print_page/index.html", "Subsec 2")
 
 
 def test_basic_build7(tmp_path):
     """
-    Test error when page does not start with h1 heading.
+    Test when page does not start with h1 heading.
+
+    As of v2.5.0, this is allowed (the plugin will add a heading to the print page)
     """
-    check_build(tmp_path, "bad_headings/mkdocs.yml", exit_code=1)
+    check_build(tmp_path, "bad_headings/mkdocs.yml", exit_code=0)
 
+def test_build_with_material_tags(tmp_path):
+    """
+    Test support with tags.
+    """
+    check_build(tmp_path, "mkdocs_material_tags/mkdocs.yml", exit_code=0)
 
 def test_basic_disable_plugin(tmp_path):
     """
     Test disabling plugin.
     """
     prj_path = check_build(tmp_path, "basic/mkdocs_material_disabled.yml", exit_code=0)
```

### Comparing `mkdocs_print_site_plugin-2.4.1/tests/test_urls.py` & `mkdocs_print_site_plugin-2.5.0/tests/test_urls.py`

 * *Files identical despite different names*

