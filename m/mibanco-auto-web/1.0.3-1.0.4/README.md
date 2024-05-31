# Comparing `tmp/mibanco_auto_web-1.0.3.tar.gz` & `tmp/mibanco_auto_web-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mibanco_auto_web-1.0.3.tar", last modified: Tue May 28 22:24:32 2024, max compression
+gzip compressed data, was "mibanco_auto_web-1.0.4.tar", last modified: Fri May 31 03:52:17 2024, max compression
```

## Comparing `mibanco_auto_web-1.0.3.tar` & `mibanco_auto_web-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.550756 mibanco_auto_web-1.0.3/
--rw-rw-rw-   0        0        0       46 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3439 2024-05-28 22:24:32.548099 mibanco_auto_web-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2364 2024-05-23 16:28:02.000000 mibanco_auto_web-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.533920 mibanco_auto_web-1.0.3/mibanco_auto_web/
--rw-rw-rw-   0        0        0       63 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-05-23 16:33:38.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/functions.py
--rw-rw-rw-   0        0        0     1798 2024-05-23 16:22:52.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/main.py
--rw-rw-rw-   0        0        0      102 2024-05-28 22:22:12.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.542564 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/
--rw-rw-rw-   0        0        0     3439 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 22:24:32.550756 mibanco_auto_web-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1609 2024-05-28 22:20:59.000000 mibanco_auto_web-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:52:17.494825 mibanco_auto_web-1.0.4/
+-rw-rw-rw-   0        0        0       46 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3424 2024-05-31 03:52:17.494825 mibanco_auto_web-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2364 2024-05-23 16:28:02.000000 mibanco_auto_web-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:52:17.485620 mibanco_auto_web-1.0.4/mibanco_auto_web/
+-rw-rw-rw-   0        0        0       63 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.4/mibanco_auto_web/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-23 16:33:38.000000 mibanco_auto_web-1.0.4/mibanco_auto_web/functions.py
+-rw-rw-rw-   0        0        0     1798 2024-05-23 16:22:52.000000 mibanco_auto_web-1.0.4/mibanco_auto_web/main.py
+-rw-rw-rw-   0        0        0      102 2024-05-31 03:47:59.000000 mibanco_auto_web-1.0.4/mibanco_auto_web/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:52:17.494825 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/
+-rw-rw-rw-   0        0        0     3424 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      319 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-31 03:52:17.000000 mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:52:17.500503 mibanco_auto_web-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1607 2024-05-31 03:48:41.000000 mibanco_auto_web-1.0.4/setup.py
```

### Comparing `mibanco_auto_web-1.0.3/PKG-INFO` & `mibanco_auto_web-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple functional test library using Python and Selenium
 Author: Automation & Performance Team
-Keywords: selenium,testing,web,chrome
+Keywords: selenium,testing,web,chrome,firefox,edge,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
-Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
```

### Comparing `mibanco_auto_web-1.0.3/README.md` & `mibanco_auto_web-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.3/mibanco_auto_web/functions.py` & `mibanco_auto_web-1.0.4/mibanco_auto_web/functions.py`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.3/mibanco_auto_web/main.py` & `mibanco_auto_web-1.0.4/mibanco_auto_web/main.py`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/PKG-INFO` & `mibanco_auto_web-1.0.4/mibanco_auto_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple functional test library using Python and Selenium
 Author: Automation & Performance Team
-Keywords: selenium,testing,web,chrome
+Keywords: selenium,testing,web,chrome,firefox,edge,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
-Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
```

### Comparing `mibanco_auto_web-1.0.3/setup.py` & `mibanco_auto_web-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         "allure-behave==2.13.5",
         "allure-python-commons==2.13.5",
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
-        "playwright==1.42.0",
         "psutil==5.9.8",
         "pillow==10.3.0",
         "openpyxl==3.1.2",
         "customtkinter==5.2.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
@@ -39,11 +38,11 @@
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.12',
     ],
-    keywords=['selenium', 'testing', 'web', 'chrome'],
+    keywords=['selenium', 'testing', 'web', 'chrome', 'firefox', 'edge', 'python'],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

