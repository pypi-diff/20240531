# Comparing `tmp/napari_sphinx_theme-0.3.2.tar.gz` & `tmp/napari_sphinx_theme-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_sphinx_theme-0.3.2.tar", last modified: Wed Jan 31 11:07:45 2024, max compression
+gzip compressed data, was "napari_sphinx_theme-0.4.0.tar", last modified: Thu May 30 23:38:40 2024, max compression
```

## Comparing `napari_sphinx_theme-0.3.2.tar` & `napari_sphinx_theme-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.045291 napari_sphinx_theme-0.3.2/napari_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-copyright.html
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-footer-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari_code_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/page-toc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/github-light-blue.html
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/github.html
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/image-sc-light-blue.html
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/image-sc.html
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari-hub-light-blue.html
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari-hub.html
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari.html
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/twitter-light-blue.html
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/twitter.html
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/zulip-light-blue.html
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/zulip.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/search-button-field.html
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/search-field.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.041291 napari_sphinx_theme-0.3.2/napari_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/napari_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    24777 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/static/css/napari-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 11:07:27.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-31 11:07:45.000000 napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-01-31 11:07:17.000000 napari_sphinx_theme-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 11:07:45.049291 napari_sphinx_theme-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.326270 napari_sphinx_theme-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.330270 napari_sphinx_theme-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.github/workflows/build_napari.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.github/workflows/lighthouserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.334270 napari_sphinx_theme-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/docs/test1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/docs/test2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/github_deploy_key_pandas_dev_pandas_sphinx_theme.enc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.334270 napari_sphinx_theme-0.4.0/napari_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-copyright.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-footer-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari_code_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/page-toc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/github-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/github.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/image-sc-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/image-sc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/mastodon-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/mastodon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari-hub-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari-hub.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/twitter-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/twitter.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/zulip-light-blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/zulip.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/search-button-field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/search-field.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.330270 napari_sphinx_theme-0.4.0/napari_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/napari_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/static/css/napari-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:38:30.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 23:38:40.000000 napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 23:38:27.000000 napari_sphinx_theme-0.4.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:38:40.338270 napari_sphinx_theme-0.4.0/setup.cfg
```

### Comparing `napari_sphinx_theme-0.3.2/LICENSE` & `napari_sphinx_theme-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/PKG-INFO` & `napari_sphinx_theme-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_sphinx_theme
-Version: 0.3.2
+Version: 0.4.0
 Summary: Bootstrap-based Sphinx theme from the napari community
 Author: napari team
 License: BSD 3-Clause License
         
         Copyright (c) 2018, pandas
         All rights reserved.
         
@@ -40,15 +40,15 @@
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydata-sphinx-theme==0.14.4
+Requires-Dist: pydata-sphinx-theme>=0.15.3
 Requires-Dist: packaging
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `napari_sphinx_theme-0.3.2/README.md` & `napari_sphinx_theme-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/__init__.py` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from pathlib import Path
 
 from .napari_code_theme import *
 
-__version__ = "0.3.2"
-
+try:
+    from ._version import version as __version__
+except ImportError:
+    __version__ = 'not-installed'
 
 def update_templates(app, pagename, templatename, context, doctree):
     """Update template names for page build."""
     template_sections = [
         "theme_navbar_start",
         "theme_navbar_center",
         "theme_navbar_end",
```

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-copyright.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-copyright.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-footer-links.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-footer-links.html`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 <a class="footer-icon__hover-blue" href="https://github.com/napari/napari" target="_blank" rel="noreferrer">
   {% include "partials/github.html" %}
   {% include "partials/github-light-blue.html" %}
   <span>GitHub</span>
 </a>
 
+<a class="footer-icon__hover-blue" href="https://fosstodon.org/@napari" target="_blank" rel="noreferrer">
+  {% include "partials/mastodon.html" %}
+  {% include "partials/mastodon-light-blue.html" %}
+  <span>Mastodon</span>
+</a>
+
 <a class="footer-icon__hover-blue" href="https://twitter.com/napari_imaging" target="_blank" rel="noreferrer">
   {% include "partials/twitter.html" %}
   {% include "partials/twitter-light-blue.html" %}
   <span>Twitter</span>
 </a>
 
 <a class="footer-icon__hover-blue" href="https://forum.image.sc/tag/napari" target="_blank" rel="noreferrer">
```

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari-layout.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari-layout.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/napari_code_theme.py` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/napari_code_theme.py`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/github-light-blue.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/github-light-blue.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/github.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/github.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/image-sc-light-blue.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/image-sc-light-blue.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/image-sc.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/image-sc.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari-hub-light-blue.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari-hub-light-blue.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari-hub.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari-hub.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/napari.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/napari.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/twitter-light-blue.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/twitter-light-blue.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/twitter.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/twitter.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/zulip-light-blue.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/zulip-light-blue.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/partials/zulip.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/partials/zulip.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/search-field.html` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/search-field.html`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/static/css/napari-sphinx-theme.css` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/static/css/napari-sphinx-theme.css`

 * *Files 7% similar despite different names*

```diff
@@ -208,69 +208,60 @@
 
 /****************************
  Nav bar section
 *****************************/
 
 .navbar {
     background-color: var(--napari-primary-blue) !important;
-    height: 64px;
     box-shadow: none;
 }
 
-.navbar .nav-item.active a {
-    font-weight: 700 !important;
-}
-
-.navbar .nav-item a>i {
-    margin-left: 0.5rem;
-    font-size: 0.875rem !important;
-}
-
 .navbar-brand {
     vertical-align: middle;
     font-size: 1.25rem;
     color: black !important;
     position: relative;
     font-weight: bolder;
 }
 .navbar-brand:hover,
 .navbar-brand:focus {
     text-decoration: none !important;
     color: var(--napari-color-text-base) !important;
 }
 
-.navbar .navbar-brand p.title {
-    font-size: 1rem;
-    line-height: 125%;
+.bd-header .navbar-nav li.pst-header-nav-item {
+    font-size: 1.0625rem;
+    font-weight: 500 !important;
 }
 
-.navbar .nav-item a {
-    text-decoration-line: none;
+.navbar-icon-links li.nav-item a.nav-link {
     color: var(--napari-color-text-base) !important;
-    font-size: 1.0625rem;
-    padding: 15px 1.0625rem 15px !important;
-    border-bottom: .1875rem solid transparent;
-    font-weight: 500 !important;
 }
 
-.bd-header .navbar-nav li a.nav-link {
-    font-weight: bold;
+.bd-header .navbar-nav li.pst-header-nav-item>.nav-link {
+    color: var(--napari-color-text-base) !important;
+    border-bottom: 3px solid transparent;
 }
 
-.bd-header .navbar-nav li a.nav-link:hover {
-    text-decoration: none !important;
-    border-bottom: .1875rem solid var(--napari-color-text-base);
+.bd-header .navbar-nav li.pst-header-nav-item>.nav-link:hover {
+    color: var(--napari-color-text-base) !important;
+    border-bottom: 3px solid var(--pst-color-primary);
 }
 
-.bd-header .navbar-nav>.current>.nav-link {
-    border-bottom: .1875rem solid var(--napari-color-text-base);
+.bd-header .navbar-nav li.pst-header-nav-item.current>.nav-link::before {
+    border-bottom: 0px solid var(--pst-color-primary);
 }
 
-.col-lg-9.navbar-header-items {
-    max-width: 75%;
+.bd-header .navbar-nav li.pst-header-nav-item.current>.nav-link {
+    border-bottom: 3px solid var(--pst-color-primary);
+    font-weight: 700 !important;
+}
+
+.bd-header .navbar-nav li.pst-header-nav-item>.nav-link {
+    padding: 15px 1.0625rem 15px !important;
 }
 
 /***************************
  version switcher
 ***************************/
 
 button.btn.version-switcher__button {
@@ -304,37 +295,40 @@
     border-radius: unset;
 }
 
 /***************************
  sidebar
 ***************************/
 
-.bd-sidebar label {
-    left: 0px;
+.bd-search {
+    border: 1px solid transparent;
+}
+
+/* Remove "Section Navigation" caption */
+.bd-links__title {
+    display: none;
 }
 
-.bd-sidebar-primary label.toctree-toggle:hover {
-    background: none;
+/* Move chevron to the left */
+.bd-sidebar-primary li.has-children>details>summary .toctree-toggle {
+    right: unset;
 }
 
+/* Fonts and styles */
 .bd-sidebar a.reference,
 .bd-sidebar .caption-text {
     font-size: 0.875rem;
     line-height: 1.25rem;
 }
 
 .bd-sidebar-primary .sidebar-primary-items__end {
     margin-bottom: 0;
     margin-top: 0;
 }
 
-.bd-search {
-    border: 1px solid transparent;
-}
-
 .bd-sidebar .toctree-l1 a {
     padding-left: 32px;
 }
 
 .bd-sidebar .toctree-l2 {
     margin-left: -0.2rem;
     border-left: 1px solid var(--napari-color-text-base);
@@ -435,18 +429,14 @@
 
 .navbar-nav li a:focus,
 .navbar-nav li a:hover,
 .navbar-nav li.current>a {
     color: var(--napari-color-text-base);
 }
 
-.navbar-nav .toctree-checkbox:checked~label i {
-    transform: rotate(90deg);
-}
-
 nav.bd-links li>a {
     color: var(--napari-color-text-base);
     display: block;
     line-height: 1.25rem;
 }
 
 nav.bd-links li>a:active,
@@ -623,15 +613,14 @@
 h2 {
     font-weight: 700;
     color: var(--napari-color-text-base) !important;
 }
 
 h3 {
     font-weight: 700;
-    font-size: 1.25rem;
     color: var(--napari-color-text-base) !important;
 }
 
 h4 {
     font-weight: 700;
     color: var(--napari-color-text-base) !important;
 }
@@ -651,14 +640,18 @@
 }
 
 .sd-card-hover:hover {
     border-color: var(--napari-color-text-base) !important;
     transform: scale(1.01);
 }
 
+.prev-next-area p {
+    color: var(--napari-color-text-base);
+}
+
 /***************************
  Admonitions
 ***************************/
 
 .admonition,
 div.admonition {
     box-shadow: none !important;
@@ -678,14 +671,18 @@
 }
 
 div.admonition *:last-child,
 .admonition *:last-child {
     margin-bottom: 0;
 }
 
+div.admonition::after {
+    padding-bottom: 10px;
+}
+
 div.admonition p.admonition-title~*,
 .admonition p.admonition-title~* {
     margin-left: 1.4rem;
     margin-right: 1.4rem;
 }
 
 div.admonition>ol,
@@ -1014,15 +1011,14 @@
 ***************************/
 
 #pst-back-to-top {
     background-color: var(--napari-light-blue);
     color: var(--napari-dark-gray);
 }
 
-
 /***************************
  Calendar popup
 ***************************/
 
 /* The Modal (background) */
 .modal {
     /* Hidden by default */
```

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme/theme.conf` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/PKG-INFO` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_sphinx_theme
-Version: 0.3.2
+Version: 0.4.0
 Summary: Bootstrap-based Sphinx theme from the napari community
 Author: napari team
 License: BSD 3-Clause License
         
         Copyright (c) 2018, pandas
         All rights reserved.
         
@@ -40,15 +40,15 @@
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydata-sphinx-theme==0.14.4
+Requires-Dist: pydata-sphinx-theme>=0.15.3
 Requires-Dist: packaging
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `napari_sphinx_theme-0.3.2/napari_sphinx_theme.egg-info/SOURCES.txt` & `napari_sphinx_theme-0.4.0/napari_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,32 @@
+.flake8
+.gitignore
+.pre-commit-config.yaml
+.prettierignore
+.prettierrc.yml
+CONTRIBUTING.md
 LICENSE
+Makefile
 README.md
+codecov.yml
+github_deploy_key_pandas_dev_pandas_sphinx_theme.enc
+noxfile.py
+package.json
 pyproject.toml
+readthedocs.yml
+.github/workflows/build_napari.yml
+.github/workflows/deploy.yml
+.github/workflows/lighthouserc.json
+docs/Makefile
+docs/conf.py
+docs/index.rst
+docs/test1.rst
+docs/test2.rst
 napari_sphinx_theme/__init__.py
+napari_sphinx_theme/_version.py
 napari_sphinx_theme/footer.html
 napari_sphinx_theme/napari-copyright.html
 napari_sphinx_theme/napari-footer-links.html
 napari_sphinx_theme/napari-layout.html
 napari_sphinx_theme/napari_code_theme.py
 napari_sphinx_theme/page-toc.html
 napari_sphinx_theme/search-button-field.html
@@ -18,14 +39,16 @@
 napari_sphinx_theme.egg-info/not-zip-safe
 napari_sphinx_theme.egg-info/requires.txt
 napari_sphinx_theme.egg-info/top_level.txt
 napari_sphinx_theme/partials/github-light-blue.html
 napari_sphinx_theme/partials/github.html
 napari_sphinx_theme/partials/image-sc-light-blue.html
 napari_sphinx_theme/partials/image-sc.html
+napari_sphinx_theme/partials/mastodon-light-blue.html
+napari_sphinx_theme/partials/mastodon.html
 napari_sphinx_theme/partials/menu.html
 napari_sphinx_theme/partials/napari-hub-light-blue.html
 napari_sphinx_theme/partials/napari-hub.html
 napari_sphinx_theme/partials/napari.html
 napari_sphinx_theme/partials/twitter-light-blue.html
 napari_sphinx_theme/partials/twitter.html
 napari_sphinx_theme/partials/zulip-light-blue.html
```

### Comparing `napari_sphinx_theme-0.3.2/pyproject.toml` & `napari_sphinx_theme-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napari_sphinx_theme"
 description = "Bootstrap-based Sphinx theme from the napari community"
 dynamic = ["version"]
 readme = "README.md"
 authors = [ {name = "napari team" }]
 
 requires-python = ">=3.7"
 dependencies = [
-  "pydata-sphinx-theme==0.14.4",
+  "pydata-sphinx-theme>=0.15.3",
   "packaging",
 ]
 
 license = { file = "LICENSE" }
 
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -45,16 +45,16 @@
 homepage = "https://napari.org/napari-sphinx-theme/"
 repository = "https://github.com/napari/napari-sphinx-theme"
 
 [tool.setuptools]
 packages = ["napari_sphinx_theme"]
 zip-safe = false
 
-[tool.setuptools.dynamic]
-version = {attr = "napari_sphinx_theme.__version__"}
+[tool.setuptools_scm]
+version_file = "napari_sphinx_theme/_version.py"
 
 [tool.setuptools.package-data]
 napari_sphinx_theme = [
     "theme.conf",
     "*.html",
     "static/css/*.css",
     "components/*.html",
```

