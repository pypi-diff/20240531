# Comparing `tmp/gocept.collmex-2.0.1.tar.gz` & `tmp/gocept.collmex-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocept.collmex-2.0.1.tar", last modified: Wed Aug 23 06:10:57 2023, max compression
+gzip compressed data, was "gocept.collmex-2.1.0.tar", last modified: Fri May 31 11:06:07 2024, max compression
```

## Comparing `gocept.collmex-2.0.1.tar` & `gocept.collmex-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.471901 gocept.collmex-2.0.1/
--rw-r--r--   0 mac        (513) staff       (20)      141 2023-08-23 06:10:56.000000 gocept.collmex-2.0.1/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)     5249 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      155 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    14331 2023-08-23 06:10:57.472094 gocept.collmex-2.0.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2149 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      192 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/collmex.ini-example
--rw-r--r--   0 mac        (513) staff       (20)      213 2023-08-23 06:10:57.472675 gocept.collmex-2.0.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1810 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.461206 gocept.collmex-2.0.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.464651 gocept.collmex-2.0.1/src/gocept/
--rw-r--r--   0 mac        (513) staff       (20)       76 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.469788 gocept.collmex-2.0.1/src/gocept/collmex/
--rw-r--r--   0 mac        (513) staff       (20)       65 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    11392 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/collmex.py
--rw-r--r--   0 mac        (513) staff       (20)     5935 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/doctest.rst
--rw-r--r--   0 mac        (513) staff       (20)     1793 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     9079 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/model.py
--rw-r--r--   0 mac        (513) staff       (20)     7337 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.471536 gocept.collmex-2.0.1/src/gocept/collmex/tests/
--rw-r--r--   0 mac        (513) staff       (20)       65 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     7694 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/tests/test_collmex.py
--rw-r--r--   0 mac        (513) staff       (20)     3453 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/tests/test_model.py
--rw-r--r--   0 mac        (513) staff       (20)      882 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/tests/test_testing.py
--rw-r--r--   0 mac        (513) staff       (20)      805 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/tests/test_thread.py
--rw-r--r--   0 mac        (513) staff       (20)     3707 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept/collmex/utils.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-08-23 06:10:57.467152 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    14331 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      826 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      155 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/src/gocept.collmex.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)      885 2023-08-23 06:10:57.000000 gocept.collmex-2.0.1/tox.ini
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.275411 gocept.collmex-2.1.0/
+-rw-r--r--   0 zagy       (501) staff       (20)      141 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/.coveragerc
+-rw-r--r--   0 zagy       (501) staff       (20)     5441 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/CHANGES.rst
+-rw-r--r--   0 zagy       (501) staff       (20)      155 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/MANIFEST.in
+-rw-r--r--   0 zagy       (501) staff       (20)    15356 2024-05-31 11:06:07.275287 gocept.collmex-2.1.0/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     2149 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/README.rst
+-rw-r--r--   0 zagy       (501) staff       (20)      192 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/collmex.ini-example
+-rw-r--r--   0 zagy       (501) staff       (20)      213 2024-05-31 11:06:07.275647 gocept.collmex-2.1.0/setup.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)     1810 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/setup.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.268766 gocept.collmex-2.1.0/src/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.270513 gocept.collmex-2.1.0/src/gocept/
+-rw-r--r--   0 zagy       (501) staff       (20)       76 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.273162 gocept.collmex-2.1.0/src/gocept/collmex/
+-rw-r--r--   0 zagy       (501) staff       (20)       65 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11865 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/collmex.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6452 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/doctest.rst
+-rw-r--r--   0 zagy       (501) staff       (20)     1870 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/interfaces.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9840 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/model.py
+-rw-r--r--   0 zagy       (501) staff       (20)     7337 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/testing.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.274408 gocept.collmex-2.1.0/src/gocept/collmex/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)       65 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     7694 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/tests/test_collmex.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3453 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/tests/test_model.py
+-rw-r--r--   0 zagy       (501) staff       (20)      882 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/tests/test_testing.py
+-rw-r--r--   0 zagy       (501) staff       (20)      805 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/tests/test_thread.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3707 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept/collmex/utils.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-31 11:06:07.274640 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/
+-rw-r--r--   0 zagy       (501) staff       (20)    15356 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)      826 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/SOURCES.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/dependency_links.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        7 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/namespace_packages.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/not-zip-safe
+-rw-r--r--   0 zagy       (501) staff       (20)      155 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/requires.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        7 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/src/gocept.collmex.egg-info/top_level.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      899 2024-05-31 11:06:07.000000 gocept.collmex-2.1.0/tox.ini
```

### Comparing `gocept.collmex-2.0.1/CHANGES.rst` & `gocept.collmex-2.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changes
 =======
 
+2.1.0 (2024-05-31)
+------------------
+
+- Update invoice items to current collmex field names.
+  (`#27 <https://github.com/gocept/gocept.collmex/pull/27>`_)
+
+- Add CustomerAgreement (CMXCAG)
+
+
 2.0.1 (2023-08-23)
 ------------------
 
 - Mark wheel as not universal.
 
 
 2.0 (2023-08-23)
```

### Comparing `gocept.collmex-2.0.1/PKG-INFO` & `gocept.collmex-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gocept.collmex
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python-bindings for the Collmex import/export API
 Home-page: https://github.com/gocept/gocept.collmex
 Author: gocept
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -17,15 +17,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: gocept.cache>=0.6.1
+Requires-Dist: setuptools>=1.0
+Requires-Dist: transaction>=1.4
+Requires-Dist: zope.deprecation>=4.0
+Requires-Dist: zope.interface>=4.0
+Requires-Dist: webtest>=2.0
+Requires-Dist: wsgiproxy2
 Provides-Extra: test
+Requires-Dist: zope.testing>=4.0; extra == "test"
+Requires-Dist: mock>=1.0; extra == "test"
 
 .. contents::
 
 .. image:: https://github.com/gocept/gocept.collmex/workflows/tests/badge.svg
            :target: https://github.com/gocept/gocept.collmex/actions?query=workflow%3Atests
 .. image:: https://coveralls.io/repos/github/gocept/gocept.collmex/badge.svg?branch=master
            :target: https://coveralls.io/github/gocept/gocept.collmex?branch=master
@@ -161,14 +170,32 @@
 >>> product['Basismengeneinheit'] = 'HR'
 >>> product['Verkaufs-Preis'] = 5
 >>> collmex.create(product)
 >>> transaction.commit()
 >>> collmex.get_products()[0]['Bezeichnung']
 'Testprodukt'
 
+Customer Agreements
+-------------------
+
+>>> cag = gocept.collmex.model.CustomerAgreement()
+>>> cag['Kunde Nr'] = '10000'
+>>> cag['Firma Nr'] = 1
+>>> cag['Produktnummer'] = 'TEST'
+>>> cag['Gültig ab'] = '01.01.2000'
+>>> cag['Gültig bis'] = '31.12.9999'
+>>> cag['Preis'] = 7
+>>> cag['Währung'] = "EUR"
+>>> collmex.create(cag)
+>>> transaction.commit()
+>>> cag_from_collmex = collmex.get_customer_agreements()
+>>> list(cag)
+['CMXCAG', '1', '10000', 'TEST', '(NULL)', '01.01.2000', '31.12.9999', 7, 'EUR', '(NULL)']
+
+
 Invoices: ``create_invoice`` and ``get_invoices``
 -------------------------------------------------
 
 Invoices are created using the ``create_invoice`` method:
 
 >>> import datetime
 >>> start_date = datetime.datetime.now()
@@ -244,15 +271,15 @@
 >>> proj = collmex.get_projects()
 >>> len(proj)
 2
 >>> proj[0]['Projektnummer'] == proj[1]['Projektnummer']
 True
 
 >>> proj[0]['Satz']
-'5,00'
+'7,00'
 >>> proj[1]['Satz']
 '9,65'
 >>> proj[0]['Inaktiv']
 '0'
 
 Caching
 -------
@@ -294,14 +321,23 @@
 
 >>> collmex._post = original_post
 
 
 Changes
 =======
 
+2.1.0 (2024-05-31)
+------------------
+
+- Update invoice items to current collmex field names.
+  (`#27 <https://github.com/gocept/gocept.collmex/pull/27>`_)
+
+- Add CustomerAgreement (CMXCAG)
+
+
 2.0.1 (2023-08-23)
 ------------------
 
 - Mark wheel as not universal.
 
 
 2.0 (2023-08-23)
```

### Comparing `gocept.collmex-2.0.1/README.rst` & `gocept.collmex-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/setup.py` & `gocept.collmex-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages
 from setuptools import setup
 import os.path
 
 
 setup(
     name='gocept.collmex',
-    version='2.0.1',
+    version='2.1.0',
     author='gocept',
     author_email='mail@gocept.com',
     description='Python-bindings for the Collmex import/export API',
     url='https://github.com/gocept/gocept.collmex',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
```

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/collmex.py` & `gocept.collmex-2.1.0/src/gocept/collmex/collmex.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,14 +211,27 @@
             'PRODUCT_GET',
             self.company_id,
             product_id,
             product_group,
             price_group,
             0, self.system_identifier)
 
+    def get_customer_agreements(self, customer_id=NULL, product_id=NULL,
+                                valid_on_date=NULL, inactive=NULL,
+                                only_changed=NULL):
+        return self._query_objects(
+            'CUSTOMER_AGREEMENT_GET',
+            self.company_id,
+            customer_id,
+            product_id,
+            date_to_collmex(valid_on_date),
+            inactive,
+            only_changed,
+            self.system_identifier)
+
     def get_projects(self, project_id=NULL, customer_id=NULL):
         return self._query_objects(
             'PROJECT_GET',
             project_id,
             self.company_id,
             customer_id)
```

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/doctest.rst` & `gocept.collmex-2.1.0/src/gocept/collmex/doctest.rst`

 * *Files 7% similar despite different names*

```diff
@@ -86,14 +86,32 @@
 >>> product['Basismengeneinheit'] = 'HR'
 >>> product['Verkaufs-Preis'] = 5
 >>> collmex.create(product)
 >>> transaction.commit()
 >>> collmex.get_products()[0]['Bezeichnung']
 'Testprodukt'
 
+Customer Agreements
+-------------------
+
+>>> cag = gocept.collmex.model.CustomerAgreement()
+>>> cag['Kunde Nr'] = '10000'
+>>> cag['Firma Nr'] = 1
+>>> cag['Produktnummer'] = 'TEST'
+>>> cag['Gültig ab'] = '01.01.2000'
+>>> cag['Gültig bis'] = '31.12.9999'
+>>> cag['Preis'] = 7
+>>> cag['Währung'] = "EUR"
+>>> collmex.create(cag)
+>>> transaction.commit()
+>>> cag_from_collmex = collmex.get_customer_agreements()
+>>> list(cag)
+['CMXCAG', '1', '10000', 'TEST', '(NULL)', '01.01.2000', '31.12.9999', 7, 'EUR', '(NULL)']
+
+
 Invoices: ``create_invoice`` and ``get_invoices``
 -------------------------------------------------
 
 Invoices are created using the ``create_invoice`` method:
 
 >>> import datetime
 >>> start_date = datetime.datetime.now()
@@ -169,15 +187,15 @@
 >>> proj = collmex.get_projects()
 >>> len(proj)
 2
 >>> proj[0]['Projektnummer'] == proj[1]['Projektnummer']
 True
 
 >>> proj[0]['Satz']
-'5,00'
+'7,00'
 >>> proj[1]['Satz']
 '9,65'
 >>> proj[0]['Inaktiv']
 '0'
 
 Caching
 -------
```

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/interfaces.py` & `gocept.collmex-2.1.0/src/gocept/collmex/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,13 +62,17 @@
     """A customer (CMXMGD)."""
 
 
 class IProduct(IModel):
     """A product (CMXPRD)."""
 
 
+class ICustomerAgreement(IModel):
+    """A customer agreement (CMXCAG)."""
+
+
 class IActivity(IModel):
     """A product (CMXACT)."""
 
 
 class IProject(IModel):
     """A project (CMXPRJ)."""
```

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/testing.py` & `gocept.collmex-2.1.0/src/gocept/collmex/testing.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/tests/test_collmex.py` & `gocept.collmex-2.1.0/src/gocept/collmex/tests/test_collmex.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/tests/test_model.py` & `gocept.collmex-2.1.0/src/gocept/collmex/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/tests/test_testing.py` & `gocept.collmex-2.1.0/src/gocept/collmex/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/tests/test_thread.py` & `gocept.collmex-2.1.0/src/gocept/collmex/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept/collmex/utils.py` & `gocept.collmex-2.1.0/src/gocept/collmex/utils.py`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/src/gocept.collmex.egg-info/PKG-INFO` & `gocept.collmex-2.1.0/src/gocept.collmex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gocept.collmex
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python-bindings for the Collmex import/export API
 Home-page: https://github.com/gocept/gocept.collmex
 Author: gocept
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -17,15 +17,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: gocept.cache>=0.6.1
+Requires-Dist: setuptools>=1.0
+Requires-Dist: transaction>=1.4
+Requires-Dist: zope.deprecation>=4.0
+Requires-Dist: zope.interface>=4.0
+Requires-Dist: webtest>=2.0
+Requires-Dist: wsgiproxy2
 Provides-Extra: test
+Requires-Dist: zope.testing>=4.0; extra == "test"
+Requires-Dist: mock>=1.0; extra == "test"
 
 .. contents::
 
 .. image:: https://github.com/gocept/gocept.collmex/workflows/tests/badge.svg
            :target: https://github.com/gocept/gocept.collmex/actions?query=workflow%3Atests
 .. image:: https://coveralls.io/repos/github/gocept/gocept.collmex/badge.svg?branch=master
            :target: https://coveralls.io/github/gocept/gocept.collmex?branch=master
@@ -161,14 +170,32 @@
 >>> product['Basismengeneinheit'] = 'HR'
 >>> product['Verkaufs-Preis'] = 5
 >>> collmex.create(product)
 >>> transaction.commit()
 >>> collmex.get_products()[0]['Bezeichnung']
 'Testprodukt'
 
+Customer Agreements
+-------------------
+
+>>> cag = gocept.collmex.model.CustomerAgreement()
+>>> cag['Kunde Nr'] = '10000'
+>>> cag['Firma Nr'] = 1
+>>> cag['Produktnummer'] = 'TEST'
+>>> cag['Gültig ab'] = '01.01.2000'
+>>> cag['Gültig bis'] = '31.12.9999'
+>>> cag['Preis'] = 7
+>>> cag['Währung'] = "EUR"
+>>> collmex.create(cag)
+>>> transaction.commit()
+>>> cag_from_collmex = collmex.get_customer_agreements()
+>>> list(cag)
+['CMXCAG', '1', '10000', 'TEST', '(NULL)', '01.01.2000', '31.12.9999', 7, 'EUR', '(NULL)']
+
+
 Invoices: ``create_invoice`` and ``get_invoices``
 -------------------------------------------------
 
 Invoices are created using the ``create_invoice`` method:
 
 >>> import datetime
 >>> start_date = datetime.datetime.now()
@@ -244,15 +271,15 @@
 >>> proj = collmex.get_projects()
 >>> len(proj)
 2
 >>> proj[0]['Projektnummer'] == proj[1]['Projektnummer']
 True
 
 >>> proj[0]['Satz']
-'5,00'
+'7,00'
 >>> proj[1]['Satz']
 '9,65'
 >>> proj[0]['Inaktiv']
 '0'
 
 Caching
 -------
@@ -294,14 +321,23 @@
 
 >>> collmex._post = original_post
 
 
 Changes
 =======
 
+2.1.0 (2024-05-31)
+------------------
+
+- Update invoice items to current collmex field names.
+  (`#27 <https://github.com/gocept/gocept.collmex/pull/27>`_)
+
+- Add CustomerAgreement (CMXCAG)
+
+
 2.0.1 (2023-08-23)
 ------------------
 
 - Mark wheel as not universal.
 
 
 2.0 (2023-08-23)
```

### Comparing `gocept.collmex-2.0.1/src/gocept.collmex.egg-info/SOURCES.txt` & `gocept.collmex-2.1.0/src/gocept.collmex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocept.collmex-2.0.1/tox.ini` & `gocept.collmex-2.1.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 
 [testenv:flake8]
 basepython=python3
 deps=flake8
 commands=flake8 src setup.py --doctest
 
 [pytest]
-addopts = src -x --timeout=60 --instafail --doctest-glob="doctest.rst" --reruns 2
+addopts = src -x --timeout=60 --instafail --reruns 2  --doctest-modules  --doctest-glob="*.rst"
```

