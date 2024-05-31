# Comparing `tmp/static-sitemap-0.0.1.tar.gz` & `tmp/static_sitemap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-sitemap-0.0.1.tar", last modified: Sat Dec 16 10:14:34 2023, max compression
+gzip compressed data, was "static_sitemap-1.0.2.tar", last modified: Fri May 31 18:01:17 2024, max compression
```

## Comparing `static-sitemap-0.0.1.tar` & `static_sitemap-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2023-12-16 10:14:34.319896 static-sitemap-0.0.1/
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     1068 2023-12-16 10:14:34.319896 static-sitemap-0.0.1/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      479 2023-12-16 10:11:54.000000 static-sitemap-0.0.1/README.md
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      796 2023-12-16 10:14:02.000000 static-sitemap-0.0.1/pyproject.toml
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2023-12-16 10:14:34.319896 static-sitemap-0.0.1/setup.cfg
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2023-12-16 10:14:34.319896 static-sitemap-0.0.1/static_sitemap/
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     5375 2023-12-16 10:09:54.000000 static-sitemap-0.0.1/static_sitemap/__init__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      101 2023-12-16 09:34:39.000000 static-sitemap-0.0.1/static_sitemap/__main__.py
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2023-12-16 10:14:34.319896 static-sitemap-0.0.1/static_sitemap.egg-info/
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     1068 2023-12-16 10:14:34.000000 static-sitemap-0.0.1/static_sitemap.egg-info/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      230 2023-12-16 10:14:34.000000 static-sitemap-0.0.1/static_sitemap.egg-info/SOURCES.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2023-12-16 10:14:34.000000 static-sitemap-0.0.1/static_sitemap.egg-info/dependency_links.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       15 2023-12-16 10:14:34.000000 static-sitemap-0.0.1/static_sitemap.egg-info/top_level.txt
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-31 18:01:17.880610 static_sitemap-1.0.2/
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     1254 2024-05-31 18:01:17.880610 static_sitemap-1.0.2/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      665 2023-12-16 10:19:28.000000 static_sitemap-1.0.2/README.md
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      796 2024-05-31 18:00:35.000000 static_sitemap-1.0.2/pyproject.toml
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-05-31 18:01:17.880610 static_sitemap-1.0.2/setup.cfg
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-31 18:01:17.880610 static_sitemap-1.0.2/static_sitemap/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     5686 2024-05-31 17:59:42.000000 static_sitemap-1.0.2/static_sitemap/__init__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      101 2023-12-16 09:34:39.000000 static_sitemap-1.0.2/static_sitemap/__main__.py
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-31 18:01:17.880610 static_sitemap-1.0.2/static_sitemap.egg-info/
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     1254 2024-05-31 18:01:17.000000 static_sitemap-1.0.2/static_sitemap.egg-info/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      230 2024-05-31 18:01:17.000000 static_sitemap-1.0.2/static_sitemap.egg-info/SOURCES.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-05-31 18:01:17.000000 static_sitemap-1.0.2/static_sitemap.egg-info/dependency_links.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       15 2024-05-31 18:01:17.000000 static_sitemap-1.0.2/static_sitemap.egg-info/top_level.txt
```

### Comparing `static-sitemap-0.0.1/PKG-INFO` & `static_sitemap-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: static-sitemap
-Version: 0.0.1
+Version: 1.0.2
 Summary: Create a sitemap from an url
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 Project-URL: Homepage, https://github.com/its-just-nans/static-sitemap
 Project-URL: Bug Tracker, https://github.com/its-just-nans/static-sitemap/issues
 Keywords: sitemap,static,python,static-sitemap,static_sitemap,generator,sitemap-generator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Static-sitemap
+# static-sitemap
+
+- [PyPi page](https://pypi.org/project/static-sitemap/)
+- [PyPiStats](https://pypistats.org/packages/static-sitemap)
+- [GitHub repo](https://github.com/Its-Just-Nans/static-sitemap)
 
 ## How to use
 
 ```sh
 # install
 python -m pip install static_sitemap
 
-python -m static_sitemap https://my-static-website.com
+python -m static_sitemap https://its-just-nans.github.io/
 ```
 
 ## Options
 
 - `--verbose` : Display URLs
 - `--quiet` : Display Nothing
 - `--sitemap` : Create a `sitemap.xml` file
```

### Comparing `static-sitemap-0.0.1/pyproject.toml` & `static_sitemap-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "static-sitemap"
-version = "0.0.1"
+version = "1.0.2"
 description = "Create a sitemap from an url"
 readme = "README.md"
 authors = [{ name = "n4n5", email = "its.just.n4n5@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `static-sitemap-0.0.1/static_sitemap/__init__.py` & `static_sitemap-1.0.2/static_sitemap/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-""" static sitemap generator"""
+"""static sitemap generator"""
+
 from sys import argv
 from re import findall
 from urllib.parse import urlparse
 from datetime import datetime
 from requests import get
 
+NEWS = 'xmlns:news="http://www.google.com/schemas/sitemap-news/0.9"'
+XHTML = ' xmlns:xhtml="http://www.w3.org/1999/xhtml"'
+IMAGE = 'xmlns:image="http://www.google.com/schemas/sitemap-image/1.1"'
+VIDEO = 'xmlns:video="http://www.google.com/schemas/sitemap-video/1.1"'
 
 in_domain = []
 ext = []
 mail = []
 globalVar = {}
 
 
@@ -128,15 +133,16 @@
 
     if globalVar["sitemap"]:
         date = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
         f = open("sitemap.xml", "w", encoding="utf-8")
         string_to_add = ""
         string_to_add += '<?xml version="1.0" encoding="UTF-8"?>' + "\n"
         string_to_add += (
-            '<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">' + "\n"
+            f'<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" {NEWS} {XHTML} {IMAGE} {VIDEO}>'
+            + "\n"
         )
         for one_link in in_domain:
             string_to_add += "    <url>\n"
             string_to_add += "        <loc>\n"
             string_to_add += f"{' '*12}{one_link}\n"
             string_to_add += "        </loc>\n"
             string_to_add += f"{' '*8}<lastmod>{date}</lastmod>\n"
```

### Comparing `static-sitemap-0.0.1/static_sitemap.egg-info/PKG-INFO` & `static_sitemap-1.0.2/static_sitemap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: static-sitemap
-Version: 0.0.1
+Version: 1.0.2
 Summary: Create a sitemap from an url
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 Project-URL: Homepage, https://github.com/its-just-nans/static-sitemap
 Project-URL: Bug Tracker, https://github.com/its-just-nans/static-sitemap/issues
 Keywords: sitemap,static,python,static-sitemap,static_sitemap,generator,sitemap-generator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Static-sitemap
+# static-sitemap
+
+- [PyPi page](https://pypi.org/project/static-sitemap/)
+- [PyPiStats](https://pypistats.org/packages/static-sitemap)
+- [GitHub repo](https://github.com/Its-Just-Nans/static-sitemap)
 
 ## How to use
 
 ```sh
 # install
 python -m pip install static_sitemap
 
-python -m static_sitemap https://my-static-website.com
+python -m static_sitemap https://its-just-nans.github.io/
 ```
 
 ## Options
 
 - `--verbose` : Display URLs
 - `--quiet` : Display Nothing
 - `--sitemap` : Create a `sitemap.xml` file
```

