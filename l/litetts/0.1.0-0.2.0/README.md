# Comparing `tmp/litetts-0.1.0.tar.gz` & `tmp/litetts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litetts-0.1.0.tar", last modified: Fri May 31 13:03:34 2024, max compression
+gzip compressed data, was "litetts-0.2.0.tar", last modified: Fri May 31 13:12:21 2024, max compression
```

## Comparing `litetts-0.1.0.tar` & `litetts-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.729734 litetts-0.1.0/
--rw-rw-rw-   0        0        0     1109 2024-05-31 12:59:14.000000 litetts-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      508 2024-05-31 13:03:34.726735 litetts-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-05-31 12:58:49.000000 litetts-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.607923 litetts-0.1.0/litetts/
--rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/__init__.py
--rw-rw-rw-   0        0        0     6621 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/driver.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.685791 litetts-0.1.0/litetts/drivers/
--rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/__init__.py
--rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/_espeak.py
--rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/dummy.py
--rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/espeak.py
--rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/nsss.py
--rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/drivers/sapi5.py
--rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/engine.py
--rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/six.py
--rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.1.0/litetts/voice.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.725735 litetts-0.1.0/litetts.egg-info/
--rw-rw-rw-   0        0        0      508 2024-05-31 13:03:34.000000 litetts-0.1.0/litetts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-05-31 13:03:34.000000 litetts-0.1.0/litetts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:03:34.000000 litetts-0.1.0/litetts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-31 13:03:34.000000 litetts-0.1.0/litetts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-05-30 17:47:59.000000 litetts-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 13:03:34.729734 litetts-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      621 2024-05-31 12:58:37.000000 litetts-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.701773 litetts-0.1.0/tests/
--rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     6621 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/driver.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:03:34.721395 litetts-0.1.0/tests/drivers/
--rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/__init__.py
--rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/_espeak.py
--rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/dummy.py
--rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/espeak.py
--rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/nsss.py
--rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/drivers/sapi5.py
--rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/engine.py
--rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/six.py
--rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.1.0/tests/voice.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.486693 litetts-0.2.0/
+-rw-rw-rw-   0        0        0     1109 2024-05-31 12:59:14.000000 litetts-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      508 2024-05-31 13:12:21.479974 litetts-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-05-31 12:58:49.000000 litetts-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.385733 litetts-0.2.0/litetts/
+-rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/__init__.py
+-rw-rw-rw-   0        0        0     6621 2024-05-31 13:10:17.000000 litetts-0.2.0/litetts/driver.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.438397 litetts-0.2.0/litetts/drivers/
+-rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/__init__.py
+-rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/_espeak.py
+-rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/dummy.py
+-rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/espeak.py
+-rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/nsss.py
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/sapi5.py
+-rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/engine.py
+-rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/six.py
+-rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/voice.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.478976 litetts-0.2.0/litetts.egg-info/
+-rw-rw-rw-   0        0        0      508 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-05-30 17:47:59.000000 litetts-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:12:21.489691 litetts-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      621 2024-05-31 13:12:14.000000 litetts-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.451587 litetts-0.2.0/tests/
+-rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     6621 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/driver.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.474979 litetts-0.2.0/tests/drivers/
+-rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/__init__.py
+-rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/_espeak.py
+-rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/dummy.py
+-rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/espeak.py
+-rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/nsss.py
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/sapi5.py
+-rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/engine.py
+-rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/six.py
+-rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/voice.py
```

### Comparing `litetts-0.1.0/LICENSE` & `litetts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/__init__.py` & `litetts-0.2.0/litetts/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/driver.py` & `litetts-0.2.0/tests/driver.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/__init__.py` & `litetts-0.2.0/litetts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/_espeak.py` & `litetts-0.2.0/litetts/drivers/_espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/dummy.py` & `litetts-0.2.0/litetts/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/espeak.py` & `litetts-0.2.0/litetts/drivers/espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/nsss.py` & `litetts-0.2.0/litetts/drivers/nsss.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/drivers/sapi5.py` & `litetts-0.2.0/litetts/drivers/sapi5.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/engine.py` & `litetts-0.2.0/litetts/engine.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts/six.py` & `litetts-0.2.0/litetts/six.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/litetts.egg-info/SOURCES.txt` & `litetts-0.2.0/litetts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/setup.py` & `litetts-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="litetts",
-    version="0.1.0",
+    version="0.2.0",
     author="Md Rehan",
     author_email="mdrehan4all@gmail.com",
     description="A package to convert text into speech",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mdrehan4all/litetts",
     packages=find_packages(),
```

### Comparing `litetts-0.1.0/tests/__init__.py` & `litetts-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/driver.py` & `litetts-0.2.0/litetts/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             if sys.platform == 'darwin':
                 driverName = 'nsss'
             elif sys.platform == 'win32':
                 driverName = 'sapi5'
             else:
                 driverName = 'espeak'
         # import driver module
-        name = 'pyttsx3.drivers.%s' % driverName
+        name = 'litetts.drivers.%s' % driverName
         self._module = importlib.import_module(name)
         # build driver instance
         self._driver = self._module.buildDriver(weakref.proxy(self))
         # initialize refs
         self._engine = engine
         self._queue = []
         self._busy = True
```

### Comparing `litetts-0.1.0/tests/drivers/__init__.py` & `litetts-0.2.0/tests/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/drivers/_espeak.py` & `litetts-0.2.0/tests/drivers/_espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/drivers/dummy.py` & `litetts-0.2.0/tests/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/drivers/espeak.py` & `litetts-0.2.0/tests/drivers/espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/drivers/nsss.py` & `litetts-0.2.0/tests/drivers/nsss.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/drivers/sapi5.py` & `litetts-0.2.0/tests/drivers/sapi5.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/engine.py` & `litetts-0.2.0/tests/engine.py`

 * *Files identical despite different names*

### Comparing `litetts-0.1.0/tests/six.py` & `litetts-0.2.0/tests/six.py`

 * *Files identical despite different names*

