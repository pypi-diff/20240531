# Comparing `tmp/unittestreport_yami-0.1.8.tar.gz` & `tmp/unittestreport_yami-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.1.8.tar", last modified: Thu May 30 08:21:13 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.9.tar", last modified: Thu May 30 08:32:52 2024, max compression
```

## Comparing `unittestreport_yami-0.1.8.tar` & `unittestreport_yami-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:21:13.679815 unittestreport_yami-0.1.8/
--rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2111 2024-05-30 08:21:13.675822 unittestreport_yami-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 08:21:13.679815 unittestreport_yami-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-30 08:21:03.000000 unittestreport_yami-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:21:13.236332 unittestreport_yami-0.1.8/unittestreport_yami/
--rw-rw-rw-   0        0        0      190 2024-05-29 02:14:58.000000 unittestreport_yami-0.1.8/unittestreport_yami/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:21:13.460196 unittestreport_yami-0.1.8/unittestreport_yami/core/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/parameterized.py
--rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/reRun.py
--rw-rw-rw-   0        0        0     5549 2024-05-30 04:51:21.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/resultPush.py
--rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/sendEmail.py
--rw-rw-rw-   0        0        0     7357 2024-05-30 08:20:23.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/testResult.py
--rw-rw-rw-   0        0        0    13573 2024-05-30 05:00:02.000000 unittestreport_yami-0.1.8/unittestreport_yami/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:21:13.672911 unittestreport_yami-0.1.8/unittestreport_yami/templates/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/dingtalk.md
--rw-rw-rw-   0        0        0      410 2024-05-30 02:31:03.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/remote_report.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.8/unittestreport_yami/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-05-30 08:21:13.278957 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2111 2024-05-30 08:21:12.000000 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2024-05-30 08:21:13.000000 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:21:12.000000 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-30 08:21:12.000000 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-30 08:21:12.000000 unittestreport_yami-0.1.8/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 08:32:52.810522 unittestreport_yami-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-30 08:32:52.810522 unittestreport_yami-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:32:52.810522 unittestreport_yami-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-30 08:32:42.000000 unittestreport_yami-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:32:52.728665 unittestreport_yami-0.1.9/unittestreport_yami/
+-rw-rw-rw-   0        0        0      190 2024-05-29 02:14:58.000000 unittestreport_yami-0.1.9/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:32:52.788644 unittestreport_yami-0.1.9/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     5549 2024-05-30 04:51:21.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     7357 2024-05-30 08:20:23.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    13573 2024-05-30 05:00:02.000000 unittestreport_yami-0.1.9/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:32:52.805113 unittestreport_yami-0.1.9/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0      412 2024-05-30 08:31:43.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/remote_report.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.9/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-30 08:32:52.764762 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-30 08:32:52.000000 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-05-30 08:32:52.000000 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:32:52.000000 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 08:32:52.000000 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 08:32:52.000000 unittestreport_yami-0.1.9/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.1.8/LICENSE` & `unittestreport_yami-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/PKG-INFO` & `unittestreport_yami-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.8/README.md` & `unittestreport_yami-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/setup.py` & `unittestreport_yami-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="unittestreport_yami",
-    version="0.1.8",
+    version="0.1.9",
     author="Ethan",
     author_email="ethan.liu@yamibuy.com",
     url="https://github.com/EthanLiuInyami/UnitTestReport",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["Jinja2==3.1.2", "PyYAML==5.3.1", "requests==2.32.2"],
```

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/dataDriver.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/parameterized.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/reRun.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/reRun.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/resultPush.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/resultPush.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/sendEmail.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/sendEmail.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/testResult.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/testResult.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/core/testRunner.py` & `unittestreport_yami-0.1.9/unittestreport_yami/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/templates/templates.html` & `unittestreport_yami-0.1.9/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/templates/templates03.html` & `unittestreport_yami-0.1.9/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/templates/templates2.html` & `unittestreport_yami-0.1.9/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami/templates/templates3.html` & `unittestreport_yami-0.1.9/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.9/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.8/unittestreport_yami.egg-info/SOURCES.txt` & `unittestreport_yami-0.1.9/unittestreport_yami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

