# Comparing `tmp/stldim-0.3.3.tar.gz` & `tmp/stldim-0.4.0.tar.gz`

## Comparing `stldim-0.3.3.tar` & `stldim-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.3/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.3/dev-requirements.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.3/requirements.txt
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 stldim-0.3.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.3/.github/workflows/pytest_coverage.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/version.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/templates/openscad_lib.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.3/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.3/tests/3DBenchy.stl
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.3/README.md
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.4.0/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.4.0/dev-requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 stldim-0.4.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.4.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.4.0/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/version.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/templates/openscad_lib.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 stldim-0.4.0/src/stldim/tests/test_mesh_with_bounds.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/11test.stl -> test.stl
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/3DBenchy.stl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/test -> test.stl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/test test.stl -> test.stl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/test!@#$%^&*().stl -> test.stl
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/test.stl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/test11.stl -> test.stl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.4.0/tests/subdir/test.stl -> test.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.4.0/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.4.0/PKG-INFO
```

### Comparing `stldim-0.3.3/.github/workflows/pylint.yml` & `stldim-0.4.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/.github/workflows/pytest.yml` & `stldim-0.4.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/.github/workflows/pytest_coverage.yml` & `stldim-0.4.0/.github/workflows/pytest_coverage.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/tests/3DBenchy.stl` & `stldim-0.4.0/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/LICENSE.md` & `stldim-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/README.md` & `stldim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/pyproject.toml` & `stldim-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.3/PKG-INFO` & `stldim-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.3.3
+Version: 0.4.0
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

