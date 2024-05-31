# Comparing `tmp/datamart_yhdr-0.1.2.tar.gz` & `tmp/datamart_yhdr-0.1.3.tar.gz`

## Comparing `datamart_yhdr-0.1.2.tar` & `datamart_yhdr-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/uploadpackage.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/src/datamart_yhdr/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/src/datamart_yhdr/const.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/src/datamart_yhdr/interface.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/src/datamart_yhdr/settings.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.1.tar.gz
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.2-py3-none-any.whl
--rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.2.tar.gz
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.3-py3-none-any.whl
--rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.3.tar.gz
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.4-py3-none-any.whl
--rw-r--r--   0        0        0    79181 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.4.tar.gz
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.5-py3-none-any.whl
--rw-r--r--   0        0        0   162244 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.5.tar.gz
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0   328596 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.0.tar.gz
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0   661197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.1.tar.gz
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/uploadpackage.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/src/datamart_yhdr/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/src/datamart_yhdr/const.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/src/datamart_yhdr/interface.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/src/datamart_yhdr/settings.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.1.tar.gz
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.2.tar.gz
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.3-py3-none-any.whl
+-rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.3.tar.gz
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.4-py3-none-any.whl
+-rw-r--r--   0        0        0    79181 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.4.tar.gz
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.5-py3-none-any.whl
+-rw-r--r--   0        0        0   162244 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.5.tar.gz
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0   328596 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.0.tar.gz
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0   661197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.1.tar.gz
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1327033 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.2.tar.gz
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.3/PKG-INFO
```

### Comparing `datamart_yhdr-0.1.2/src/datamart_yhdr/interface.py` & `datamart_yhdr-0.1.3/src/datamart_yhdr/interface.py`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/src/datamart_yhdr/settings.py` & `datamart_yhdr-0.1.3/src/datamart_yhdr/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datamart_yhdr import const
 
 const.WORKSPACE_DEV = "YHDR-DM-DEV"
 const.WORKSPACE = "YHDR-DM"
-const.HALO_URL = "http://192.168.10.111:82/base/token/create"
-const.QUERY_URL = "http://192.168.10.111:82/query/query"
-const.COMMAND_URL = "http://192.168.10.111:82/message/message/submit"
-const.BATCH_URL = "http://192.168.10.111:82/message/message/submit/batch"
+const.HALO_URL = "http://192.168.100.100:82/base/token/create"
+const.QUERY_URL = "http://192.168.100.100:82/query/query"
+const.COMMAND_URL = "http://192.168.100.100:82/message/message/submit"
+const.BATCH_URL = "http://192.168.100.100:82/message/message/submit/batch"
 const.HALO_URL_UAT = "http://192.168.10.175:82/base/token/create"
 const.QUERY_URL_UAT = "http://192.168.10.175:82/query/query"
 const.COMMAND_URL_UAT = "http://192.168.10.175:82/message/message/submit"
 const.BATCH_URL_UAT = "http://192.168.10.175:82/message/message/submit/batch"
 const.HALO_URL_DEV = "http://192.168.100.73:83/base/token/create"
 const.QUERY_URL_DEV = "http://192.168.100.73:83/query/query"
 const.COMMAND_URL_DEV = "http://192.168.100.73:83/message/message/submit"
```

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.1-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.1.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.2-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.2.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.3-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.3.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.4-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.4.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.5-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.0.5.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.0-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.0.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.1-py3-none-any.whl` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/tests/datamart_yhdr-0.1.1.tar.gz` & `datamart_yhdr-0.1.3/tests/datamart_yhdr-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/LICENSE` & `datamart_yhdr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.2/pyproject.toml` & `datamart_yhdr-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datamart_yhdr"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Shihua Huang", email="huangshihua@galaxyderivatives.com" },
 ]
 description = "A data interface package developed for Galaxy Derivatives Data Mart"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `datamart_yhdr-0.1.2/PKG-INFO` & `datamart_yhdr-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: datamart_yhdr
-Version: 0.1.2
+Version: 0.1.3
 Summary: A data interface package developed for Galaxy Derivatives Data Mart
 Project-URL: Homepage, https://galaxyderivatives.feishu.cn/wiki/wikcn6BhNvlpE8yOCmkjmJHTWHe
 Project-URL: Documentation, https://galaxyderivatives.feishu.cn/wiki/wikcnjOa3s7OQ06v82CzXHBDqUd
 Author-email: Shihua Huang <huangshihua@galaxyderivatives.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

