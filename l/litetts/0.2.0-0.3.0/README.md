# Comparing `tmp/litetts-0.2.0.tar.gz` & `tmp/litetts-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litetts-0.2.0.tar", last modified: Fri May 31 13:12:21 2024, max compression
+gzip compressed data, was "litetts-0.3.0.tar", last modified: Fri May 31 13:46:35 2024, max compression
```

## Comparing `litetts-0.2.0.tar` & `litetts-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.486693 litetts-0.2.0/
--rw-rw-rw-   0        0        0     1109 2024-05-31 12:59:14.000000 litetts-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      508 2024-05-31 13:12:21.479974 litetts-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-05-31 12:58:49.000000 litetts-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.385733 litetts-0.2.0/litetts/
--rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/__init__.py
--rw-rw-rw-   0        0        0     6621 2024-05-31 13:10:17.000000 litetts-0.2.0/litetts/driver.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.438397 litetts-0.2.0/litetts/drivers/
--rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/__init__.py
--rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/_espeak.py
--rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/dummy.py
--rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/espeak.py
--rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/nsss.py
--rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/drivers/sapi5.py
--rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/engine.py
--rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/six.py
--rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.2.0/litetts/voice.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.478976 litetts-0.2.0/litetts.egg-info/
--rw-rw-rw-   0        0        0      508 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-31 13:12:21.000000 litetts-0.2.0/litetts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-05-30 17:47:59.000000 litetts-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 13:12:21.489691 litetts-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      621 2024-05-31 13:12:14.000000 litetts-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.451587 litetts-0.2.0/tests/
--rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     6621 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/driver.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:12:21.474979 litetts-0.2.0/tests/drivers/
--rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/__init__.py
--rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/_espeak.py
--rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/dummy.py
--rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/espeak.py
--rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/nsss.py
--rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/drivers/sapi5.py
--rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/engine.py
--rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/six.py
--rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.2.0/tests/voice.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.282555 litetts-0.3.0/
+-rw-rw-rw-   0        0        0     1109 2024-05-31 12:59:14.000000 litetts-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      730 2024-05-31 13:46:35.280557 litetts-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-05-31 12:58:49.000000 litetts-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.178532 litetts-0.3.0/litetts/
+-rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/__init__.py
+-rw-rw-rw-   0        0        0     6621 2024-05-31 13:10:17.000000 litetts-0.3.0/litetts/driver.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.243648 litetts-0.3.0/litetts/drivers/
+-rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/__init__.py
+-rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/_espeak.py
+-rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/dummy.py
+-rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/espeak.py
+-rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/nsss.py
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/drivers/sapi5.py
+-rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/engine.py
+-rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/six.py
+-rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.3.0/litetts/voice.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.278559 litetts-0.3.0/litetts.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-31 13:46:34.000000 litetts-0.3.0/litetts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2024-05-31 13:46:35.000000 litetts-0.3.0/litetts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:46:34.000000 litetts-0.3.0/litetts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-05-31 13:46:34.000000 litetts-0.3.0/litetts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-31 13:46:34.000000 litetts-0.3.0/litetts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-05-30 17:47:59.000000 litetts-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:46:35.283555 litetts-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      865 2024-05-31 13:46:23.000000 litetts-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.259523 litetts-0.3.0/tests/
+-rw-rw-rw-   0        0        0      782 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     6621 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/driver.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:46:35.275560 litetts-0.3.0/tests/drivers/
+-rw-rw-rw-   0        0        0      830 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/__init__.py
+-rw-rw-rw-   0        0        0    17730 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/_espeak.py
+-rw-rw-rw-   0        0        0     6008 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/dummy.py
+-rw-rw-rw-   0        0        0     6301 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/espeak.py
+-rw-rw-rw-   0        0        0     3483 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/nsss.py
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/drivers/sapi5.py
+-rw-rw-rw-   0        0        0     6902 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/engine.py
+-rw-rw-rw-   0        0        0    28688 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/six.py
+-rw-rw-rw-   0        0        0      417 2024-05-31 12:50:54.000000 litetts-0.3.0/tests/voice.py
```

### Comparing `litetts-0.2.0/LICENSE` & `litetts-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/__init__.py` & `litetts-0.3.0/litetts/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/driver.py` & `litetts-0.3.0/litetts/driver.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/__init__.py` & `litetts-0.3.0/litetts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/_espeak.py` & `litetts-0.3.0/litetts/drivers/_espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/dummy.py` & `litetts-0.3.0/litetts/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/espeak.py` & `litetts-0.3.0/litetts/drivers/espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/nsss.py` & `litetts-0.3.0/litetts/drivers/nsss.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/drivers/sapi5.py` & `litetts-0.3.0/litetts/drivers/sapi5.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/engine.py` & `litetts-0.3.0/litetts/engine.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts/six.py` & `litetts-0.3.0/litetts/six.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/litetts.egg-info/SOURCES.txt` & `litetts-0.3.0/litetts.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 litetts/driver.py
 litetts/engine.py
 litetts/six.py
 litetts/voice.py
 litetts.egg-info/PKG-INFO
 litetts.egg-info/SOURCES.txt
 litetts.egg-info/dependency_links.txt
+litetts.egg-info/requires.txt
 litetts.egg-info/top_level.txt
 litetts/drivers/__init__.py
 litetts/drivers/_espeak.py
 litetts/drivers/dummy.py
 litetts/drivers/espeak.py
 litetts/drivers/nsss.py
 litetts/drivers/sapi5.py
```

### Comparing `litetts-0.2.0/tests/__init__.py` & `litetts-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/driver.py` & `litetts-0.3.0/tests/driver.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/__init__.py` & `litetts-0.3.0/tests/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/_espeak.py` & `litetts-0.3.0/tests/drivers/_espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/dummy.py` & `litetts-0.3.0/tests/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/espeak.py` & `litetts-0.3.0/tests/drivers/espeak.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/nsss.py` & `litetts-0.3.0/tests/drivers/nsss.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/drivers/sapi5.py` & `litetts-0.3.0/tests/drivers/sapi5.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/engine.py` & `litetts-0.3.0/tests/engine.py`

 * *Files identical despite different names*

### Comparing `litetts-0.2.0/tests/six.py` & `litetts-0.3.0/tests/six.py`

 * *Files identical despite different names*

