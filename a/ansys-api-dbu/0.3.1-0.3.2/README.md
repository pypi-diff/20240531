# Comparing `tmp/ansys_api_dbu-0.3.1.tar.gz` & `tmp/ansys_api_dbu-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_api_dbu-0.3.1.tar", last modified: Fri May 24 13:43:05 2024, max compression
+gzip compressed data, was "ansys_api_dbu-0.3.2.tar", last modified: Fri May 31 12:27:24 2024, max compression
```

## Comparing `ansys_api_dbu-0.3.1.tar` & `ansys_api_dbu-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.814770 ansys_api_dbu-0.3.1/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.814770 ansys_api_dbu-0.3.1/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys/api/dbu/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/admin.proto
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapi.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapplication.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbumodels.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuwebmodels.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/designs.proto
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/drivingdimensions.proto
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/sessionmanager.proto
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/streaming.proto
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/windows.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.551658 ansys_api_dbu-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-31 12:27:24.551658 ansys_api_dbu-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.543658 ansys_api_dbu-0.3.2/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.543658 ansys_api_dbu-0.3.2/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.547658 ansys_api_dbu-0.3.2/ansys/api/dbu/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.547658 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/admin.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuapi.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuapplication.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbumodels.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuwebmodels.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/designs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/drivingdimensions.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/sessionmanager.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/streaming.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/ansys/api/dbu/v0/windows.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:27:24.551658 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 12:27:24.000000 ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:27:24.551658 ansys_api_dbu-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-31 12:27:17.000000 ansys_api_dbu-0.3.2/setup.py
```

### Comparing `ansys_api_dbu-0.3.1/LICENSE` & `ansys_api_dbu-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/PKG-INFO` & `ansys_api_dbu-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ansys-api-dbu
-Version: 0.3.1
-Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 13:43:05 on 24 May 2024
+Version: 0.3.2
+Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 12:27:24 on 31 May 2024
 Home-page: https://github.com/ansys/ansys-api-dbu
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-dbu/#readme
 Project-URL: Source, https://github.com/ansys/ansys-api-dbu/
 Project-URL: Tracker, https://github.com/ansys/ansys-api-dbu/issues/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: grpcio~=1.47
+Requires-Dist: grpcio~=1.44
 Requires-Dist: protobuf<6,>=3.19
 
 ### ansys-api-dbu gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files for
 the Ansys DBU Service.
```

### Comparing `ansys_api_dbu-0.3.1/README.md` & `ansys_api_dbu-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/admin.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/admin.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapi.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuapi.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapplication.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuapplication.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbumodels.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbumodels.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuwebmodels.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/dbuwebmodels.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/designs.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/designs.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/drivingdimensions.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/drivingdimensions.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/sessionmanager.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/sessionmanager.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/windows.proto` & `ansys_api_dbu-0.3.2/ansys/api/dbu/v0/windows.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/PKG-INFO` & `ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ansys-api-dbu
-Version: 0.3.1
-Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 13:43:05 on 24 May 2024
+Version: 0.3.2
+Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 12:27:24 on 31 May 2024
 Home-page: https://github.com/ansys/ansys-api-dbu
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-dbu/#readme
 Project-URL: Source, https://github.com/ansys/ansys-api-dbu/
 Project-URL: Tracker, https://github.com/ansys/ansys-api-dbu/issues/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: grpcio~=1.47
+Requires-Dist: grpcio~=1.44
 Requires-Dist: protobuf<6,>=3.19
 
 ### ansys-api-dbu gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files for
 the Ansys DBU Service.
```

### Comparing `ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/SOURCES.txt` & `ansys_api_dbu-0.3.2/ansys_api_dbu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys_api_dbu-0.3.1/setup.py` & `ansys_api_dbu-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,46 +11,48 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 product = "dbu"
 library = ""
 package_info = ["ansys", "api", product, library, "v0"]
-with open(os.path.join(HERE, "ansys", "api", product, library, "VERSION"), encoding="utf-8") as f:
+with open(
+    os.path.join(HERE, "ansys", "api", product, library, "VERSION"), encoding="utf-8"
+) as f:
     version = f.read().strip()
 
 package_name = "ansys-api-dbu"
-dot_package_name = '.'.join(filter(None, package_info))
+dot_package_name = ".".join(filter(None, package_info))
 
 description = f"Autogenerated Python gRPC interface package for {package_name}, built on {datetime.now().strftime('%H:%M:%S on %d %B %Y')}"
 
 if __name__ == "__main__":
     setuptools.setup(
         name=package_name,
         version=version,
         author="ANSYS, Inc.",
-        author_email='pyansys.core@ansys.com',
+        author_email="pyansys.core@ansys.com",
         maintainer="ANSYS, Inc.",
-        maintainer_email='pyansys.core@ansys.com',
+        maintainer_email="pyansys.core@ansys.com",
         description=description,
         long_description=long_description,
-        long_description_content_type='text/markdown',
+        long_description_content_type="text/markdown",
         url=f"https://github.com/ansys/{package_name}",
         license="MIT",
         python_requires=">=3.7",
-        install_requires=["grpcio~=1.47", "protobuf>=3.19,<6"],
+        install_requires=["grpcio~=1.44", "protobuf>=3.19,<6"],
         packages=setuptools.find_namespace_packages(".", include=("ansys.*",)),
         package_data={
             "": ["*.proto", "*.pyi", "py.typed", "VERSION"],
         },
         entry_points={
             "ansys.tools.protoc_helper.proto_provider": [
                 f"{dot_package_name}={dot_package_name}"
             ],
         },
         cmdclass=CMDCLASS_OVERRIDE,
         project_urls={
-            'Documentation': 'https://github.com/ansys/ansys-api-dbu/#readme',
-            'Source': 'https://github.com/ansys/ansys-api-dbu/',
-            'Tracker': 'https://github.com/ansys/ansys-api-dbu/issues/',
+            "Documentation": "https://github.com/ansys/ansys-api-dbu/#readme",
+            "Source": "https://github.com/ansys/ansys-api-dbu/",
+            "Tracker": "https://github.com/ansys/ansys-api-dbu/issues/",
         },
     )
```

