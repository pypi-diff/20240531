# Comparing `tmp/touying-0.11.2.tar.gz` & `tmp/touying-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "touying-0.11.2.tar", last modified: Tue May 28 02:59:27 2024, max compression
+gzip compressed data, was "touying-0.11.3.tar", last modified: Fri May 31 12:44:38 2024, max compression
```

## Comparing `touying-0.11.2.tar` & `touying-0.11.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:59:27.271558 touying-0.11.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 02:59:19.000000 touying-0.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 02:59:27.271558 touying-0.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-28 02:59:19.000000 touying-0.11.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 02:59:19.000000 touying-0.11.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:59:27.271558 touying-0.11.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:59:27.267558 touying-0.11.2/touying/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 02:59:19.000000 touying-0.11.2/touying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-28 02:59:19.000000 touying-0.11.2/touying/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-28 02:59:19.000000 touying-0.11.2/touying/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    65079 2024-05-28 02:59:19.000000 touying-0.11.2/touying/template.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:59:27.271558 touying-0.11.2/touying.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 02:59:27.000000 touying-0.11.2/touying.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:44:38.511773 touying-0.11.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 12:44:34.000000 touying-0.11.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-31 12:44:38.511773 touying-0.11.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-31 12:44:34.000000 touying-0.11.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 12:44:34.000000 touying-0.11.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:44:38.511773 touying-0.11.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:44:38.511773 touying-0.11.3/touying/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 12:44:34.000000 touying-0.11.3/touying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-31 12:44:34.000000 touying-0.11.3/touying/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-31 12:44:34.000000 touying-0.11.3/touying/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65079 2024-05-31 12:44:34.000000 touying-0.11.3/touying/template.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:44:38.511773 touying-0.11.3/touying.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 12:44:38.000000 touying-0.11.3/touying.egg-info/top_level.txt
```

### Comparing `touying-0.11.2/LICENSE` & `touying-0.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `touying-0.11.2/PKG-INFO` & `touying-0.11.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: touying
-Version: 0.11.2
+Version: 0.11.3
 Summary: Export presentation slides in various formats for Touying
 Author-email: OrangeX4 <318483724@qq.com>
 License: MIT
 Project-URL: Home, https://github.com/touying-typ/touying-exporter
 Keywords: presentation,slides,export
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typst>=0.11.1
 Requires-Dist: python-pptx>=0.6
 Requires-Dist: pillow
 Requires-Dist: jinja2
-Requires-Dist: scour
 Requires-Dist: argparse
 
 # Touying Exporter
 
 Export presentation slides in various formats for Touying.
```

### Comparing `touying-0.11.2/README.md` & `touying-0.11.3/README.md`

 * *Files identical despite different names*

### Comparing `touying-0.11.2/pyproject.toml` & `touying-0.11.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "touying"
-version = "0.11.2"
+version = "0.11.3"
 description = "Export presentation slides in various formats for Touying"
 readme = "README.md"
 keywords = ["presentation", "slides", "export"]
 license = {text = "MIT"}
 authors = [
     {name = "OrangeX4", email = "318483724@qq.com"}
 ]
 dependencies = [
     "typst>=0.11.1",
     "python-pptx>=0.6",
     "pillow",
     "jinja2",
-    "scour",
     "argparse",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `touying-0.11.2/touying/cli.py` & `touying-0.11.3/touying/cli.py`

 * *Files identical despite different names*

### Comparing `touying-0.11.2/touying/exporter.py` & `touying-0.11.3/touying/exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pathlib import Path
 from PIL import Image
 from io import BytesIO
 import json
 import jinja2
 import os
 import re
-from scour import scour
 
 FILE_PATH = os.path.dirname(os.path.realpath(__file__))
 
 
 def to_html(
     input, root=None, font_paths=[], output=None, start_page=1, count=None, silent=False
 ):
@@ -30,18 +29,14 @@
         re.sub(
             r'width="([0-9\.]+)pt" height="([0-9\.]+)pt"',
             'width="100%" height="100%"',
             image,
         )
         for image in images
     ]
-    # minify svgs
-    scour_options = scour.sanitizeOptions(options=None)
-    scour_options.remove_metadata = True
-    images = [scour.scourString(image, scour_options) for image in images]
 
     # query <pdfpc-file> from typst file
     pdfpc = json.loads(
         typst.query(
             input, "<pdfpc-file>", root=root, font_paths=font_paths, field="value"
         )
     )
```

### Comparing `touying-0.11.2/touying/template.html.j2` & `touying-0.11.3/touying/template.html.j2`

 * *Files identical despite different names*

### Comparing `touying-0.11.2/touying.egg-info/PKG-INFO` & `touying-0.11.3/touying.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: touying
-Version: 0.11.2
+Version: 0.11.3
 Summary: Export presentation slides in various formats for Touying
 Author-email: OrangeX4 <318483724@qq.com>
 License: MIT
 Project-URL: Home, https://github.com/touying-typ/touying-exporter
 Keywords: presentation,slides,export
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typst>=0.11.1
 Requires-Dist: python-pptx>=0.6
 Requires-Dist: pillow
 Requires-Dist: jinja2
-Requires-Dist: scour
 Requires-Dist: argparse
 
 # Touying Exporter
 
 Export presentation slides in various formats for Touying.
```

