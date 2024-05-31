# Comparing `tmp/simpleset-0.4.0.tar.gz` & `tmp/simpleset-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleset-0.4.0.tar", max compression
+gzip compressed data, was "simpleset-0.4.1.tar", max compression
```

## Comparing `simpleset-0.4.0.tar` & `simpleset-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     2318 2023-10-13 13:52:02.676583 simpleset-0.4.0/README.md
--rw-r--r--   0        0        0      970 2023-10-13 14:15:53.933844 simpleset-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-10-09 22:23:18.368862 simpleset-0.4.0/simpleset/__init__.py
--rw-r--r--   0        0        0     6960 2023-10-13 12:00:55.595383 simpleset-0.4.0/simpleset/constant.py
--rw-r--r--   0        0        0     1497 2023-10-13 13:57:52.529965 simpleset-0.4.0/simpleset/django.py
--rw-r--r--   0        0        0      984 2023-10-13 11:55:45.340173 simpleset-0.4.0/simpleset/error.py
--rw-r--r--   0        0        0     1377 2023-10-13 00:39:03.219565 simpleset-0.4.0/simpleset/graphene.py
--rw-r--r--   0        0        0     1643 2023-10-13 13:19:17.547651 simpleset-0.4.0/simpleset/strict.py
--rw-r--r--   0        0        0      312 2023-10-12 14:52:42.700448 simpleset-0.4.0/simpleset/utils.py
--rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 simpleset-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2324 2023-10-13 14:19:23.892047 simpleset-0.4.1/README.md
+-rw-r--r--   0        0        0      970 2024-05-31 21:30:37.763742 simpleset-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-10-09 22:23:18.368862 simpleset-0.4.1/simpleset/__init__.py
+-rw-r--r--   0        0        0     7032 2024-05-31 21:28:54.164122 simpleset-0.4.1/simpleset/constant.py
+-rw-r--r--   0        0        0      984 2023-10-13 11:55:45.340173 simpleset-0.4.1/simpleset/error.py
+-rw-r--r--   0        0        0     1377 2023-10-13 00:39:03.219565 simpleset-0.4.1/simpleset/graphene.py
+-rw-r--r--   0        0        0     1643 2023-10-13 13:19:17.547651 simpleset-0.4.1/simpleset/strict.py
+-rw-r--r--   0        0        0      312 2023-10-12 14:52:42.700448 simpleset-0.4.1/simpleset/utils.py
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 simpleset-0.4.1/PKG-INFO
```

### Comparing `simpleset-0.4.0/README.md` & `simpleset-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 \[ [Documentation](https://simpleset.readthedocs.io/en/latest/) | [Cheatsheet](https://simpleset.readthedocs.io/en/latest/cheatsheet/) | [Changelog](https://github.com/odigity/simpleset/blob/master/CHANGELOG.md) \]
 
 ### Disclaimer!
 
-tl;dr — Expect breaking changes in the future, and pin the version you use to protect yourself.
+tl;dr — Expect breaking changes in the future, and pin the version to protect yourself.
 
 This package is very new and has only been used by me as far as I know.
 
 When others start using it in different contexts, providing useful feedback on the quality of the API, and guiding its evolution to a mature 1.0 release, I will then offer API stability guarantees and adhere to SemVer.
 
 In the meantime, I see no harm in using it in production given how simple it is.  However, _**please make sure to pin your package dependency to an exact version**_ so your code doesn't break if and when I decide to change something.
 
 ### Synopsis
 
-I dislike Python [Enums](https://docs.python.org/3/library/enum.html).  They behave strangely and are difficult to build on top of or extend.  This package provides a Python class named `Constant` which facilitates the creation and usage of enumerated values.  This plain old Python class is both simpler to understand and more powerful/flexible then native enums.
+I dislike Python [Enums](https://docs.python.org/3/library/enum.html).  They behave strangely and are difficult to build on top of or extend.  This package provides a Python class named `Constant` which facilitates the creation and usage of immutable enumerated value sets.  This plain old Python class is both simpler to understand and more powerful/flexible then native enums.
 
 Even a Python beginner should be able to understand *most* of the source code.  The exceptions are discussed in the [docs](https://simpleset.readthedocs.io/en/latest/internals/).
 
 ### Preview
 
 ```python
 from simpleset import Constant
```

### Comparing `simpleset-0.4.0/pyproject.toml` & `simpleset-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [ tool.poetry ]
 
 name            = "simpleset"
-version         = "0.4.0"
+version         = "0.4.1"
 description     = "Better Than Enums"
 authors         = [ "Ofer Nave <odigity@gmail.com>" ]
 readme          = "README.md"
 repository      = "https://github.com/odigity/simpleset/"
 documentation   = "https://simpleset.readthedocs.io/en/latest/"
 packages        = [ { include = "simpleset" } ]
```

### Comparing `simpleset-0.4.0/simpleset/constant.py` & `simpleset-0.4.1/simpleset/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,17 @@
     # Form 2:  populate( cname1=value1, ... )
     # Form 3:  populate( cname1=dict( attr1=val1, ... ), ... )
     #
     # Warning:  Doesn't prevent you from mixing multiple forms in a single call.
     @classmethod
     def populate( cls, *args, **kwargs ):
 
+        if not hasattr( cls, "_objdir" ):
+            cls._objdir = {}
+
         # Form 1
         for cname in args:
             cname = str( cname )
             assert cname.isidentifier()
             cls._create( cname )
 
         for cname, payload in kwargs.items():
```

### Comparing `simpleset-0.4.0/simpleset/error.py` & `simpleset-0.4.1/simpleset/error.py`

 * *Files identical despite different names*

### Comparing `simpleset-0.4.0/simpleset/graphene.py` & `simpleset-0.4.1/simpleset/graphene.py`

 * *Files identical despite different names*

### Comparing `simpleset-0.4.0/simpleset/strict.py` & `simpleset-0.4.1/simpleset/strict.py`

 * *Files identical despite different names*

### Comparing `simpleset-0.4.0/PKG-INFO` & `simpleset-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleset
-Version: 0.4.0
+Version: 0.4.1
 Summary: Better Than Enums
 Home-page: https://github.com/odigity/simpleset/
 Author: Ofer Nave
 Author-email: odigity@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,25 +17,25 @@
 Project-URL: Repository, https://github.com/odigity/simpleset/
 Description-Content-Type: text/markdown
 
 \[ [Documentation](https://simpleset.readthedocs.io/en/latest/) | [Cheatsheet](https://simpleset.readthedocs.io/en/latest/cheatsheet/) | [Changelog](https://github.com/odigity/simpleset/blob/master/CHANGELOG.md) \]
 
 ### Disclaimer!
 
-tl;dr — Expect breaking changes in the future, and pin the version you use to protect yourself.
+tl;dr — Expect breaking changes in the future, and pin the version to protect yourself.
 
 This package is very new and has only been used by me as far as I know.
 
 When others start using it in different contexts, providing useful feedback on the quality of the API, and guiding its evolution to a mature 1.0 release, I will then offer API stability guarantees and adhere to SemVer.
 
 In the meantime, I see no harm in using it in production given how simple it is.  However, _**please make sure to pin your package dependency to an exact version**_ so your code doesn't break if and when I decide to change something.
 
 ### Synopsis
 
-I dislike Python [Enums](https://docs.python.org/3/library/enum.html).  They behave strangely and are difficult to build on top of or extend.  This package provides a Python class named `Constant` which facilitates the creation and usage of enumerated values.  This plain old Python class is both simpler to understand and more powerful/flexible then native enums.
+I dislike Python [Enums](https://docs.python.org/3/library/enum.html).  They behave strangely and are difficult to build on top of or extend.  This package provides a Python class named `Constant` which facilitates the creation and usage of immutable enumerated value sets.  This plain old Python class is both simpler to understand and more powerful/flexible then native enums.
 
 Even a Python beginner should be able to understand *most* of the source code.  The exceptions are discussed in the [docs](https://simpleset.readthedocs.io/en/latest/internals/).
 
 ### Preview
 
 ```python
 from simpleset import Constant
```

