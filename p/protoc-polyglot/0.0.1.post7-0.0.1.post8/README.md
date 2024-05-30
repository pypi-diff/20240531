# Comparing `tmp/protoc_polyglot-0.0.1.post7.tar.gz` & `tmp/protoc_polyglot-0.0.1.post8.tar.gz`

## Comparing `protoc_polyglot-0.0.1.post7.tar` & `protoc_polyglot-0.0.1.post8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/__init__.py
--rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/cli.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/wrapper.py
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/cpp/cli.py
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/csharp/cli.py
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/go/cli.py
--rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/java/cli.py
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/js/cli.py
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/obj-c/cli.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/php/cli.py
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/python/cli.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/ruby/cli.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/core/rust/cli.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/.gitignore
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/pyproject.toml
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/__init__.py
+-rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/cli.py
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/wrapper.py
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/cpp/cli.py
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/csharp/cli.py
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/go/cli.py
+-rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/java/cli.py
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/js/cli.py
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/obj-c/cli.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/php/cli.py
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/python/cli.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/ruby/cli.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/rust/cli.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/.gitignore
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/pyproject.toml
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/PKG-INFO
```

### Comparing `protoc_polyglot-0.0.1.post7/core/cli.py` & `protoc_polyglot-0.0.1.post8/core/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/wrapper.py` & `protoc_polyglot-0.0.1.post8/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/cpp/cli.py` & `protoc_polyglot-0.0.1.post8/core/cpp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/csharp/cli.py` & `protoc_polyglot-0.0.1.post8/core/csharp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/go/cli.py` & `protoc_polyglot-0.0.1.post8/core/go/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/java/cli.py` & `protoc_polyglot-0.0.1.post8/core/java/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/js/cli.py` & `protoc_polyglot-0.0.1.post8/core/js/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/obj-c/cli.py` & `protoc_polyglot-0.0.1.post8/core/obj-c/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/php/cli.py` & `protoc_polyglot-0.0.1.post8/core/php/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/python/cli.py` & `protoc_polyglot-0.0.1.post8/core/python/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/ruby/cli.py` & `protoc_polyglot-0.0.1.post8/core/ruby/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/core/rust/cli.py` & `protoc_polyglot-0.0.1.post8/core/rust/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/README.md` & `protoc_polyglot-0.0.1.post8/README.md`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post7/pyproject.toml` & `protoc_polyglot-0.0.1.post8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.hatch.build.targets.wheel]
 include = [
   "core/*",
 ]
 
 [project]
 name = "protoc_polyglot"
-version = "0.0.1-7"
+version = "0.0.1-8"
 license = {text = "MIT License"}
 authors = [
   { name="Milan Pultar", email="milan.pultar@gmail.com" },
   { name="Hugo Kunák", email="author@example.com" },
 ]
 description = "Protoc wrapper for compilation into any language"
 readme = "README.md"
@@ -33,8 +33,11 @@
 Homepage = "https://github.com/pypa/sampleproject"
 Issues = "https://github.com/pypa/sampleproject/issues"
 
 [bdist_wheel]
 universal=1
 
 [tool.hatch.scripts]
+protoc-polyglot = "core.wrapper:execute"
+
+[project.scripts]
 protoc-polyglot = "core.wrapper:execute"
```

### Comparing `protoc_polyglot-0.0.1.post7/PKG-INFO` & `protoc_polyglot-0.0.1.post8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: protoc_polyglot
-Version: 0.0.1.post7
+Version: 0.0.1.post8
 Summary: Protoc wrapper for compilation into any language
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Milan Pultar <milan.pultar@gmail.com>, Hugo Kunák <author@example.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

