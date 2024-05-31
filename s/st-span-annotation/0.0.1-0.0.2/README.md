# Comparing `tmp/st_span_annotation-0.0.1.tar.gz` & `tmp/st_span_annotation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_span_annotation-0.0.1.tar", last modified: Thu May 30 11:26:40 2024, max compression
+gzip compressed data, was "st_span_annotation-0.0.2.tar", last modified: Thu May 30 11:43:08 2024, max compression
```

## Comparing `st_span_annotation-0.0.1.tar` & `st_span_annotation-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.926433 st_span_annotation-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 11:25:36.000000 st_span_annotation-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 11:25:36.000000 st_span_annotation-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 11:26:40.926433 st_span_annotation-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 11:25:36.000000 st_span_annotation-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:26:40.926433 st_span_annotation-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 11:25:36.000000 st_span_annotation-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.922433 st_span_annotation-0.0.1/st_span_annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-30 11:25:36.000000 st_span_annotation-0.0.1/st_span_annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.918434 st_span_annotation-0.0.1/st_span_annotation/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.922433 st_span_annotation-0.0.1/st_span_annotation/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 11:26:29.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   197459 2024-05-30 11:26:21.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-30 11:26:29.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.918434 st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.922433 st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   320316 2024-05-30 11:26:29.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 11:26:29.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1257271 2024-05-30 11:26:29.000000 st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:26:40.926433 st_span_annotation-0.0.1/st_span_annotation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 11:26:40.000000 st_span_annotation-0.0.1/st_span_annotation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 11:26:40.000000 st_span_annotation-0.0.1/st_span_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:26:40.000000 st_span_annotation-0.0.1/st_span_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 11:26:40.000000 st_span_annotation-0.0.1/st_span_annotation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 11:26:40.000000 st_span_annotation-0.0.1/st_span_annotation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.772370 st_span_annotation-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 11:42:14.000000 st_span_annotation-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 11:42:14.000000 st_span_annotation-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 11:43:08.772370 st_span_annotation-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 11:42:14.000000 st_span_annotation-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:43:08.772370 st_span_annotation-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-30 11:42:14.000000 st_span_annotation-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.768370 st_span_annotation-0.0.2/st_span_annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 11:42:14.000000 st_span_annotation-0.0.2/st_span_annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.768370 st_span_annotation-0.0.2/st_span_annotation/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.768370 st_span_annotation-0.0.2/st_span_annotation/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 11:42:59.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197459 2024-05-30 11:42:51.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-30 11:42:59.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.768370 st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.772370 st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   320316 2024-05-30 11:42:59.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 11:42:59.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1257271 2024-05-30 11:42:59.000000 st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:43:08.772370 st_span_annotation-0.0.2/st_span_annotation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 11:43:08.000000 st_span_annotation-0.0.2/st_span_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 11:43:08.000000 st_span_annotation-0.0.2/st_span_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:43:08.000000 st_span_annotation-0.0.2/st_span_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 11:43:08.000000 st_span_annotation-0.0.2/st_span_annotation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 11:43:08.000000 st_span_annotation-0.0.2/st_span_annotation.egg-info/top_level.txt
```

### Comparing `st_span_annotation-0.0.1/LICENSE` & `st_span_annotation-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/PKG-INFO` & `st_span_annotation-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-span-annotation
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component to annotate text span
 Home-page: 
 Author: r-terada
 Author-email: r.terada1993@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `st_span_annotation-0.0.1/README.md` & `st_span_annotation-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/setup.py` & `st_span_annotation-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-span-annotation",
-    version="0.0.1",
+    version="0.0.2",
     author="r-terada",
     author_email="r.terada1993@gmail.com",
     description="Streamlit component to annotate text span",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
@@ -29,9 +29,9 @@
             "wheel",
             "pytest==7.4.0",
             "playwright==1.39.0",
             "requests==2.31.0",
             "pytest-playwright-snapshot==1.0",
             "pytest-rerunfailures==12.0",
         ]
-    }
+    },
 )
```

### Comparing `st_span_annotation-0.0.1/st_span_annotation/__init__.py` & `st_span_annotation-0.0.2/st_span_annotation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import TypedDict
 import streamlit.components.v1 as components
 
-_RELEASE = os.getenv("RELEASE", "false").lower() == "true"
+_RELEASE = True
 
 if not _RELEASE:
     _component_func = components.declare_component(
         "st_span_annotation",
         url="http://localhost:3001",
     )
 else:
```

### Comparing `st_span_annotation-0.0.1/st_span_annotation/frontend/build/bootstrap.min.css` & `st_span_annotation-0.0.2/st_span_annotation/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js` & `st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js.LICENSE.txt` & `st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/st_span_annotation/frontend/build/static/js/main.f85624d4.js.map` & `st_span_annotation-0.0.2/st_span_annotation/frontend/build/static/js/main.f85624d4.js.map`

 * *Files identical despite different names*

### Comparing `st_span_annotation-0.0.1/st_span_annotation.egg-info/PKG-INFO` & `st_span_annotation-0.0.2/st_span_annotation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-span-annotation
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component to annotate text span
 Home-page: 
 Author: r-terada
 Author-email: r.terada1993@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `st_span_annotation-0.0.1/st_span_annotation.egg-info/SOURCES.txt` & `st_span_annotation-0.0.2/st_span_annotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

