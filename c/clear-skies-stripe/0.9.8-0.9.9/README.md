# Comparing `tmp/clear_skies_stripe-0.9.8.tar.gz` & `tmp/clear_skies_stripe-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_stripe-0.9.8.tar", max compression
+gzip compressed data, was "clear_skies_stripe-0.9.9.tar", max compression
```

## Comparing `clear_skies_stripe-0.9.8.tar` & `clear_skies_stripe-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.8/LICENSE
--rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.8/README.md
--rw-r--r--   0        0        0      728 2024-05-13 11:24:09.220883 clear_skies_stripe-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.8/src/clearskies_stripe/__init__.py
--rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.8/src/clearskies_stripe/backends/__init__.py
--rw-r--r--   0        0        0     3082 2024-05-12 17:41:08.620060 clear_skies_stripe-0.9.8/src/clearskies_stripe/backends/stripe_sdk_backend.py
--rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.8/src/clearskies_stripe/di/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.8/src/clearskies_stripe/di/stripe.py
--rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.8/src/clearskies_stripe/handlers/__init__.py
--rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.8/src/clearskies_stripe/handlers/create_setup_intent.py
--rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.8/src/clearskies_stripe/handlers/create_setup_intent_test.py
--rw-r--r--   0        0        0      223 2024-05-12 17:44:47.700270 clear_skies_stripe-0.9.8/src/clearskies_stripe/models/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-12 16:24:18.957847 clear_skies_stripe-0.9.8/src/clearskies_stripe/models/stripe_charge.py
--rw-r--r--   0        0        0     1279 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.8/src/clearskies_stripe/models/stripe_customer.py
--rw-r--r--   0        0        0      812 2024-05-13 11:10:06.337540 clear_skies_stripe-0.9.8/src/clearskies_stripe/models/stripe_payment_method.py
--rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.9/LICENSE
+-rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.9/README.md
+-rw-r--r--   0        0        0      728 2024-05-27 17:24:26.551957 clear_skies_stripe-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.9/src/clearskies_stripe/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.9/src/clearskies_stripe/backends/__init__.py
+-rw-r--r--   0        0        0     3082 2024-05-12 17:41:08.620060 clear_skies_stripe-0.9.9/src/clearskies_stripe/backends/stripe_sdk_backend.py
+-rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.9/src/clearskies_stripe/di/__init__.py
+-rw-r--r--   0        0        0     6515 2024-05-27 17:19:09.046893 clear_skies_stripe-0.9.9/src/clearskies_stripe/di/stripe.py
+-rw-r--r--   0        0        0     1698 2024-05-27 17:22:23.395174 clear_skies_stripe-0.9.9/src/clearskies_stripe/di/stripe_test.py
+-rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.9/src/clearskies_stripe/handlers/__init__.py
+-rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.9/src/clearskies_stripe/handlers/create_setup_intent.py
+-rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.9/src/clearskies_stripe/handlers/create_setup_intent_test.py
+-rw-r--r--   0        0        0      223 2024-05-12 17:44:47.700270 clear_skies_stripe-0.9.9/src/clearskies_stripe/models/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-12 16:24:18.957847 clear_skies_stripe-0.9.9/src/clearskies_stripe/models/stripe_charge.py
+-rw-r--r--   0        0        0     1279 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.9/src/clearskies_stripe/models/stripe_customer.py
+-rw-r--r--   0        0        0     1522 2024-05-20 11:41:05.988634 clear_skies_stripe-0.9.9/src/clearskies_stripe/models/stripe_payment_method.py
+-rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.9/PKG-INFO
```

### Comparing `clear_skies_stripe-0.9.8/LICENSE` & `clear_skies_stripe-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/README.md` & `clear_skies_stripe-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/pyproject.toml` & `clear_skies_stripe-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-stripe"
-version = "0.9.8"
+version = "0.9.9"
 description = "clearskies bindings for working with Stripe"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-stripe"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_stripe-0.9.8/src/clearskies_stripe/backends/stripe_sdk_backend.py` & `clear_skies_stripe-0.9.9/src/clearskies_stripe/backends/stripe_sdk_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/src/clearskies_stripe/handlers/create_setup_intent.py` & `clear_skies_stripe-0.9.9/src/clearskies_stripe/handlers/create_setup_intent.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/src/clearskies_stripe/handlers/create_setup_intent_test.py` & `clear_skies_stripe-0.9.9/src/clearskies_stripe/handlers/create_setup_intent_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/src/clearskies_stripe/models/stripe_charge.py` & `clear_skies_stripe-0.9.9/src/clearskies_stripe/models/stripe_charge.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/src/clearskies_stripe/models/stripe_customer.py` & `clear_skies_stripe-0.9.9/src/clearskies_stripe/models/stripe_customer.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.8/PKG-INFO` & `clear_skies_stripe-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-stripe
-Version: 0.9.8
+Version: 0.9.9
 Summary: clearskies bindings for working with Stripe
 Home-page: https://github.com/cmancone/clearskies-stripe
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

