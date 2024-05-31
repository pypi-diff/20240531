# Comparing `tmp/ukrr_models-2.1.1.tar.gz` & `tmp/ukrr_models-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukrr_models-2.1.1.tar", max compression
+gzip compressed data, was "ukrr_models-2.2.0.tar", max compression
```

## Comparing `ukrr_models-2.1.1.tar` & `ukrr_models-2.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1078 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/LICENSE
--rw-r--r--   0        0        0     1291 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/README.md
--rw-r--r--   0        0        0      637 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/__init__.py
--rw-r--r--   0        0        0     1680 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/nhsbt_models.py
--rw-r--r--   0        0        0     2386 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/rr_models.py
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 ukrr_models-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1291 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/README.md
+-rw-r--r--   0        0        0      637 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/ukrr_models/__init__.py
+-rw-r--r--   0        0        0     1822 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/ukrr_models/nhsbt_models.py
+-rw-r--r--   0        0        0     2386 2024-05-31 08:36:56.282947 ukrr_models-2.2.0/ukrr_models/rr_models.py
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 ukrr_models-2.2.0/PKG-INFO
```

### Comparing `ukrr_models-2.1.1/LICENSE` & `ukrr_models-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukrr_models-2.1.1/README.md` & `ukrr_models-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ukrr_models-2.1.1/pyproject.toml` & `ukrr_models-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ukrr-models"
-version = "2.1.1"
+version = "2.2.0"
 description = "Models of the UKRR database"
 authors = ["UK Renal Registry"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ukrr_models-2.1.1/ukrr_models/nhsbt_models.py` & `ukrr_models-2.2.0/ukrr_models/nhsbt_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,7 +44,14 @@
     transplant_relationship = Column(String(20))
     transplant_sex = Column(String(12))
     cause_of_failure = Column(String(10))
     cause_of_failure_text = Column(String(500))
     cit_mins = Column(String(10))
     hla_mismatch = Column(String(10))
     ukt_suspension = Column(Boolean)
+
+
+class UKTSites(Base):
+    __tablename__ = "ukt_sites"
+
+    site_name = Column(String(50), primary_key=True)
+    rr_code = Column(String(8))
```

### Comparing `ukrr_models-2.1.1/ukrr_models/rr_models.py` & `ukrr_models-2.2.0/ukrr_models/rr_models.py`

 * *Files identical despite different names*

### Comparing `ukrr_models-2.1.1/PKG-INFO` & `ukrr_models-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukrr-models
-Version: 2.1.1
+Version: 2.2.0
 Summary: Models of the UKRR database
 License: MIT
 Author: UK Renal Registry
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ukrr-models Version: 2.1.1 Summary: Models of the
+Metadata-Version: 2.1 Name: ukrr-models Version: 2.2.0 Summary: Models of the
 UKRR database License: MIT Author: UK Renal Registry Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: sqlalchemy (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
```

