# Comparing `tmp/pytest_aux-0.0.1.tar.gz` & `tmp/pytest_aux-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aux-0.0.1.tar", last modified: Thu May 30 15:20:12 2024, max compression
+gzip compressed data, was "pytest_aux-0.0.2.tar", last modified: Thu May 30 15:44:59 2024, max compression
```

## Comparing `pytest_aux-0.0.1.tar` & `pytest_aux-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 15:20:12.178682 pytest_aux-0.0.1/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 pytest_aux-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1684 2024-05-30 15:20:12.178682 pytest_aux-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-05-30 15:16:37.000000 pytest_aux-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 15:20:12.170673 pytest_aux-0.0.1/pytest_aux/
--rw-rw-rw-   0        0        0      892 2024-05-30 14:53:14.000000 pytest_aux-0.0.1/pytest_aux/__init__.py
--rw-rw-rw-   0        0        0     1617 2024-05-30 15:08:17.000000 pytest_aux-0.0.1/pytest_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:20:12.177629 pytest_aux-0.0.1/pytest_aux.egg-info/
--rw-rw-rw-   0        0        0     1684 2024-05-30 15:20:12.000000 pytest_aux-0.0.1/pytest_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-30 15:20:12.000000 pytest_aux-0.0.1/pytest_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 15:20:12.000000 pytest_aux-0.0.1/pytest_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 15:20:12.000000 pytest_aux-0.0.1/pytest_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 15:20:12.180507 pytest_aux-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pytest_aux-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:44:59.701792 pytest_aux-0.0.2/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 pytest_aux-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1684 2024-05-30 15:44:59.701792 pytest_aux-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-05-30 15:44:18.000000 pytest_aux-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 15:44:59.695960 pytest_aux-0.0.2/pytest_aux/
+-rw-rw-rw-   0        0        0      892 2024-05-30 14:53:14.000000 pytest_aux-0.0.2/pytest_aux/__init__.py
+-rw-rw-rw-   0        0        0     1821 2024-05-30 15:44:18.000000 pytest_aux-0.0.2/pytest_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:44:59.701717 pytest_aux-0.0.2/pytest_aux.egg-info/
+-rw-rw-rw-   0        0        0     1684 2024-05-30 15:44:59.000000 pytest_aux-0.0.2/pytest_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-30 15:44:59.000000 pytest_aux-0.0.2/pytest_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:44:59.000000 pytest_aux-0.0.2/pytest_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 15:44:59.000000 pytest_aux-0.0.2/pytest_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:44:59.705241 pytest_aux-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pytest_aux-0.0.2/setup.py
```

### Comparing `pytest_aux-0.0.1/LICENSE` & `pytest_aux-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aux-0.0.1/PKG-INFO` & `pytest_aux-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_aux
-Version: 0.0.1
+Version: 0.0.2
 Summary: templates/examples and aux for pytest
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/pytest_aux
 Keywords: pytest templates,pytest examples,pytest aux,pytest parametrisation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pytest_aux (v0.0.1)
+# pytest_aux (v0.0.2)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.1/README.md` & `pytest_aux-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pytest_aux (v0.0.1)
+# pytest_aux (v0.0.2)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.1/pytest_aux/__init__.py` & `pytest_aux-0.0.2/pytest_aux/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_aux-0.0.1/pytest_aux/main.py` & `pytest_aux-0.0.2/pytest_aux/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 # =====================================================================================================================
 pass
 
 
 # =====================================================================================================================
 def pytest_parametrisation_tester(
-        func_link, args, kwargs, _EXPECTED,
+        func_link: Callable[..., Union[Any, NoReturn]], # if func would get Exx - instance of exx would be returned for value!
+        args,
+        kwargs,
+        _EXPECTED: Union[Any, Exception, Type[Exception]],  # EXACT VARIANT OR ExxClass
         _MARK: pytest.MarkDecorator | None  = None,
         _COMMENT: str | None = None
 ):
     args = args or ()
     kwargs = kwargs or {}
     comment = _COMMENT or ""
```

### Comparing `pytest_aux-0.0.1/pytest_aux.egg-info/PKG-INFO` & `pytest_aux-0.0.2/pytest_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_aux
-Version: 0.0.1
+Version: 0.0.2
 Summary: templates/examples and aux for pytest
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/pytest_aux
 Keywords: pytest templates,pytest examples,pytest aux,pytest parametrisation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pytest_aux (v0.0.1)
+# pytest_aux (v0.0.2)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.1/setup.py` & `pytest_aux-0.0.2/setup.py`

 * *Files identical despite different names*

