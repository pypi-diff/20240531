# Comparing `tmp/protoc_polyglot-0.0.1.post8.tar.gz` & `tmp/protoc_polyglot-0.0.1.post9.tar.gz`

## Comparing `protoc_polyglot-0.0.1.post8.tar` & `protoc_polyglot-0.0.1.post9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/__init__.py
--rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/cli.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/wrapper.py
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/cpp/cli.py
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/csharp/cli.py
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/go/cli.py
--rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/java/cli.py
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/js/cli.py
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/obj-c/cli.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/php/cli.py
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/python/cli.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/ruby/cli.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/core/rust/cli.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/.gitignore
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/pyproject.toml
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/__init__.py
+-rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/cli.py
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/wrapper.py
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/cpp/cli.py
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/csharp/cli.py
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/go/cli.py
+-rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/java/cli.py
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/js/cli.py
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/obj-c/cli.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/php/cli.py
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/python/cli.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/ruby/cli.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/core/rust/cli.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/.gitignore
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/README.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/pyproject.toml
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post9/PKG-INFO
```

### Comparing `protoc_polyglot-0.0.1.post8/core/cli.py` & `protoc_polyglot-0.0.1.post9/core/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/wrapper.py` & `protoc_polyglot-0.0.1.post9/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/cpp/cli.py` & `protoc_polyglot-0.0.1.post9/core/cpp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/csharp/cli.py` & `protoc_polyglot-0.0.1.post9/core/csharp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/go/cli.py` & `protoc_polyglot-0.0.1.post9/core/go/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/java/cli.py` & `protoc_polyglot-0.0.1.post9/core/java/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/js/cli.py` & `protoc_polyglot-0.0.1.post9/core/js/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/obj-c/cli.py` & `protoc_polyglot-0.0.1.post9/core/obj-c/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/php/cli.py` & `protoc_polyglot-0.0.1.post9/core/php/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/python/cli.py` & `protoc_polyglot-0.0.1.post9/core/python/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/ruby/cli.py` & `protoc_polyglot-0.0.1.post9/core/ruby/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/core/rust/cli.py` & `protoc_polyglot-0.0.1.post9/core/rust/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/README.md` & `protoc_polyglot-0.0.1.post9/README.md`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post8/PKG-INFO` & `protoc_polyglot-0.0.1.post9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.3
 Name: protoc_polyglot
-Version: 0.0.1.post8
+Version: 0.0.1.post9
 Summary: Protoc wrapper for compilation into any language
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Milan Pultar <milan.pultar@gmail.com>, Hugo Kunák <author@example.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: fire
+Requires-Dist: requests
+Requires-Dist: shutil
+Requires-Dist: yaml
+Requires-Dist: zipfile
 Description-Content-Type: text/markdown
 
 ## All-in-one Protocol Buffers compilation tool
 ### Supported languages:
 Python, JavaScript, C++, Rust, Java, Go, ObjectiveC, PHP, Ruby, C#
 
 ### TODO:
```

