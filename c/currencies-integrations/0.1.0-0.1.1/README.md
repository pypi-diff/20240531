# Comparing `tmp/currencies_integrations-0.1.0.tar.gz` & `tmp/currencies_integrations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currencies_integrations-0.1.0.tar", max compression
+gzip compressed data, was "currencies_integrations-0.1.1.tar", max compression
```

## Comparing `currencies_integrations-0.1.0.tar` & `currencies_integrations-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1083 2024-05-06 00:32:03.725352 currencies_integrations-0.1.0/LICENSE
--rw-r--r--   0        0        0      830 2024-05-06 00:25:09.411008 currencies_integrations-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-05 02:14:49.311312 currencies_integrations-0.1.0/currencies_integrations/__init__.py
--rw-r--r--   0        0        0      611 2024-05-05 20:46:36.431646 currencies_integrations-0.1.0/currencies_integrations/cli.py
--rw-r--r--   0        0        0      766 2024-05-05 17:52:18.465126 currencies_integrations-0.1.0/currencies_integrations/connection.py
--rw-r--r--   0        0        0     1491 2024-05-05 20:47:21.952566 currencies_integrations-0.1.0/currencies_integrations/dolar.py
--rw-r--r--   0        0        0     1580 2024-05-06 00:48:58.361017 currencies_integrations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 currencies_integrations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-06 00:32:03.725352 currencies_integrations-0.1.1/LICENSE
+-rw-r--r--   0        0        0      830 2024-05-06 00:25:09.411008 currencies_integrations-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 02:14:49.311312 currencies_integrations-0.1.1/currencies_integrations/__init__.py
+-rw-r--r--   0        0        0      715 2024-05-30 22:25:09.015927 currencies_integrations-0.1.1/currencies_integrations/bitcoin.py
+-rw-r--r--   0        0        0      887 2024-05-30 22:37:19.519200 currencies_integrations-0.1.1/currencies_integrations/cli.py
+-rw-r--r--   0        0        0      766 2024-05-05 17:52:18.465126 currencies_integrations-0.1.1/currencies_integrations/connection.py
+-rw-r--r--   0        0        0     1417 2024-05-30 22:23:17.341370 currencies_integrations-0.1.1/currencies_integrations/dolar.py
+-rw-r--r--   0        0        0      709 2024-05-30 22:37:58.512865 currencies_integrations-0.1.1/currencies_integrations/libra.py
+-rw-r--r--   0        0        0      136 2024-05-30 22:35:35.429832 currencies_integrations-0.1.1/currencies_integrations/utils.py
+-rw-r--r--   0        0        0     1851 2024-05-30 22:52:28.994604 currencies_integrations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 currencies_integrations-0.1.1/PKG-INFO
```

### Comparing `currencies_integrations-0.1.0/LICENSE` & `currencies_integrations-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `currencies_integrations-0.1.0/README.md` & `currencies_integrations-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `currencies_integrations-0.1.0/currencies_integrations/connection.py` & `currencies_integrations-0.1.1/currencies_integrations/connection.py`

 * *Files identical despite different names*

### Comparing `currencies_integrations-0.1.0/currencies_integrations/dolar.py` & `currencies_integrations-0.1.1/currencies_integrations/dolar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from .connection import APIConnection
-
-
-def generate_average_value(high, low):
-    return round(((float(high) + float(low)) / 2), 5)
+from .utils import *
 
 
 def dolar_comercial() -> dict[str, str]:
     """
     Retorna a cotação do dólar comercial em BRL.
 
     Returns:
```

### Comparing `currencies_integrations-0.1.0/PKG-INFO` & `currencies_integrations-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currencies-integrations
-Version: 0.1.0
+Version: 0.1.1
 Summary: Projeto para facilitar na busca por cotações de recursos financeiros.
 License: MIT
 Author: Daniel Guzman
 Author-email: dguzzz101@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

