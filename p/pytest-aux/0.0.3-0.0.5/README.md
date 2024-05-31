# Comparing `tmp/pytest_aux-0.0.3.tar.gz` & `tmp/pytest_aux-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aux-0.0.3.tar", last modified: Fri May 31 06:56:26 2024, max compression
+gzip compressed data, was "pytest_aux-0.0.5.tar", last modified: Fri May 31 07:38:46 2024, max compression
```

## Comparing `pytest_aux-0.0.3.tar` & `pytest_aux-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 06:56:26.929057 pytest_aux-0.0.3/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 pytest_aux-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1684 2024-05-31 06:56:26.928368 pytest_aux-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-05-31 06:55:46.000000 pytest_aux-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 06:56:26.916154 pytest_aux-0.0.3/pytest_aux/
--rw-rw-rw-   0        0        0      881 2024-05-31 06:55:42.000000 pytest_aux-0.0.3/pytest_aux/__init__.py
--rw-rw-rw-   0        0        0     3873 2024-05-31 06:55:42.000000 pytest_aux-0.0.3/pytest_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:56:26.927148 pytest_aux-0.0.3/pytest_aux.egg-info/
--rw-rw-rw-   0        0        0     1684 2024-05-31 06:56:26.000000 pytest_aux-0.0.3/pytest_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-31 06:56:26.000000 pytest_aux-0.0.3/pytest_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 06:56:26.000000 pytest_aux-0.0.3/pytest_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 06:56:26.000000 pytest_aux-0.0.3/pytest_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 06:56:26.929924 pytest_aux-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pytest_aux-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:46.120311 pytest_aux-0.0.5/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 pytest_aux-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1684 2024-05-31 07:38:46.119845 pytest_aux-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-05-31 07:37:54.000000 pytest_aux-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:46.108091 pytest_aux-0.0.5/pytest_aux/
+-rw-rw-rw-   0        0        0      951 2024-05-31 07:38:22.000000 pytest_aux-0.0.5/pytest_aux/__init__.py
+-rw-rw-rw-   0        0        0     5908 2024-05-31 07:37:29.000000 pytest_aux-0.0.5/pytest_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:46.118061 pytest_aux-0.0.5/pytest_aux.egg-info/
+-rw-rw-rw-   0        0        0     1684 2024-05-31 07:38:46.000000 pytest_aux-0.0.5/pytest_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-31 07:38:46.000000 pytest_aux-0.0.5/pytest_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:38:46.000000 pytest_aux-0.0.5/pytest_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 07:38:46.000000 pytest_aux-0.0.5/pytest_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:38:46.121861 pytest_aux-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pytest_aux-0.0.5/setup.py
```

### Comparing `pytest_aux-0.0.3/LICENSE` & `pytest_aux-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aux-0.0.3/PKG-INFO` & `pytest_aux-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_aux
-Version: 0.0.3
+Version: 0.0.5
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
 
-# pytest_aux (v0.0.3)
+# pytest_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.3/README.md` & `pytest_aux-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pytest_aux (v0.0.3)
+# pytest_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.3/pytest_aux/main.py` & `pytest_aux-0.0.5/pytest_aux/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 # =====================================================================================================================
 pass
 
 
 # =====================================================================================================================
 def pytest_func_tester(
         func_link: Callable[..., Union[Any, NoReturn]], # if func would get Exx - instance of exx would be returned for value!
-        args,
-        kwargs,
-        _EXPECTED: Union[Any, Exception, Type[Exception]],  # EXACT VALUE OR ExxClass
+        args: Union[tuple[Any], Any, None] = None,
+        kwargs: Optional[dict[str, Any]] = None,
+        _EXPECTED: Union[Any, Exception, Type[Exception]] = True,  # EXACT VALUE OR ExxClass
 
         _MARK: pytest.MarkDecorator | None = None,
         _COMMENT: str | None = None
 ) -> NoReturn | None:
     """
     function which test target func with exact parameters
     :return: Exception only on AssertionError, no exception withing target func!
     """
     args = args or ()
-    kwargs = kwargs or {}
+    if not isinstance(args, tuple):
+        args = (args, )
+    kwargs = kwargs or dict()
     comment = _COMMENT or ""
 
     try:
         actual_value = func_link(*args, **kwargs)
     except Exception as exx:
         actual_value = exx
 
@@ -48,14 +50,52 @@
     else:
         if TypeChecker.check__exception(_EXPECTED):
             assert TypeChecker.check__nested__by_cls_or_inst(actual_value, _EXPECTED)
         else:
             assert actual_value == _EXPECTED
 
 
+# ---------------------------------------------------------------------------------------------------------------------
+def pytest_func_tester__wo_kwargs(
+        func_link,
+        args,
+        _EXPECTED,
+
+        _MARK = None,
+        _COMMENT = None
+) -> NoReturn | None:
+    """
+    short variant in case of kwargs is not needed
+
+    WHY IT NEED
+    -----------
+     ll params passed by pytest while parametrisation as TUPLE!!!! so you cant miss any param in the middle!
+    """
+    pytest_func_tester(func_link=func_link, args=args, _EXPECTED=_EXPECTED, _MARK=_MARK, _COMMENT=_COMMENT)
+
+
+# ---------------------------------------------------------------------------------------------------------------------
+def pytest_func_tester__wo_args(
+        func_link,
+        kwargs,
+        _EXPECTED,
+
+        _MARK = None,
+        _COMMENT = None
+) -> NoReturn | None:
+    """
+    short variant in case of args is not needed
+
+    WHY IT NEED
+    -----------
+     ll params passed by pytest while parametrisation as TUPLE!!!! so you cant miss any param in the middle!
+    """
+    pytest_func_tester(func_link=func_link, kwargs=kwargs, _EXPECTED=_EXPECTED, _MARK=_MARK, _COMMENT=_COMMENT)
+
+
 # =====================================================================================================================
 pass    # USAGE EXAMPLES
 pass    # USAGE EXAMPLES
 pass    # USAGE EXAMPLES
 pass    # USAGE EXAMPLES
 pass    # USAGE EXAMPLES
 pass    # USAGE EXAMPLES
@@ -84,25 +124,40 @@
         ((1, 2), {}, None, mark.skip, "skip"),
         ((1, 2), {}, None, mark.skipif(True), "skip"),
         ((1, 2), {}, "12", mark.skipif(False), "ok"),
         ((1, 2), {}, None, mark.xfail, "ok"),
         ((1, 2), {}, "12", mark.xfail, "SHOULD BE FAIL!"),
     ]
 )
-def test__full_params(func_link, args, kwargs, _EXPECTED, _MARK, _COMMENT):
+def test__full_params(func_link, args, kwargs, _EXPECTED, _MARK, _COMMENT):     # NOTE: all params passed by TUPLE!!!! so you cant miss any in the middle!
     pytest_func_tester(func_link, args, kwargs, _EXPECTED, _MARK, _COMMENT)
 
 
 # =====================================================================================================================
 @pytest.mark.parametrize(argnames="func_link", argvalues=[int, ])
 @pytest.mark.parametrize(
     argnames="args, kwargs, _EXPECTED",
     argvalues=[
         (("1", ), {}, 1),
-        (("hello", ), {}, Exception),
+        ("1", {}, 1),                   # ARGS - direct one value acceptable
+        (("hello", ), {}, Exception),   # EXPECT - direct exceptions
     ]
 )
 def test__short_variant(func_link, args, kwargs, _EXPECTED):
     pytest_func_tester(func_link, args, kwargs, _EXPECTED)
 
 
 # =====================================================================================================================
+@pytest.mark.parametrize(argnames="func_link", argvalues=[int, ])
+@pytest.mark.parametrize(
+    argnames="args, _EXPECTED",
+    argvalues=[
+        (("1", ), 1),
+        ("1", 1),
+        (("hello", ), Exception),
+    ]
+)
+def test__shortest_variant(func_link, args, _EXPECTED):
+    pytest_func_tester__wo_kwargs(func_link, args, _EXPECTED)
+
+
+# =====================================================================================================================
```

### Comparing `pytest_aux-0.0.3/pytest_aux.egg-info/PKG-INFO` & `pytest_aux-0.0.5/pytest_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_aux
-Version: 0.0.3
+Version: 0.0.5
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
 
-# pytest_aux (v0.0.3)
+# pytest_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 templates/examples and aux for pytest
 
 ## DESCRIPTION_LONG
 designed for ...
```

### Comparing `pytest_aux-0.0.3/setup.py` & `pytest_aux-0.0.5/setup.py`

 * *Files identical despite different names*

