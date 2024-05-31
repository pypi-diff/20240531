# Comparing `tmp/ansys_api_geometry-0.4.2.tar.gz` & `tmp/ansys_api_geometry-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_api_geometry-0.4.2.tar", last modified: Fri May 24 13:50:05 2024, max compression
+gzip compressed data, was "ansys_api_geometry-0.4.3.tar", last modified: Fri May 31 13:05:40 2024, max compression
```

## Comparing `ansys_api_geometry-0.4.2.tar` & `ansys_api_geometry-0.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.479882 ansys_api_geometry-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-24 13:50:05.479882 ansys_api_geometry-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.471882 ansys_api_geometry-0.4.2/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.471882 ansys_api_geometry-0.4.2/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.475882 ansys_api_geometry-0.4.2/ansys/api/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.475882 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/bodies.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/commands.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/coordinatesystems.proto
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/curves.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/edges.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/faces.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/facettools.proto
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/materials.proto
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/measuretools.proto
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/meshes.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/models.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/namedselections.proto
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/parts.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/preparetools.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/ansys/api/geometry/v0/repairtools.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:50:05.479882 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 13:50:05.000000 ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:50:05.479882 ansys_api_geometry-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-24 13:49:57.000000 ansys_api_geometry-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.224663 ansys_api_geometry-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-31 13:05:40.224663 ansys_api_geometry-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.216663 ansys_api_geometry-0.4.3/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.216663 ansys_api_geometry-0.4.3/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.220663 ansys_api_geometry-0.4.3/ansys/api/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.220663 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/bodies.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/commands.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/coordinatesystems.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/curves.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/edges.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/faces.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/facettools.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/materials.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/measuretools.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/meshes.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/models.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/namedselections.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/parts.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/preparetools.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/ansys/api/geometry/v0/repairtools.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:05:40.224663 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 13:05:40.000000 ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:05:40.224663 ansys_api_geometry-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-31 13:05:31.000000 ansys_api_geometry-0.4.3/setup.py
```

### Comparing `ansys_api_geometry-0.4.2/LICENSE` & `ansys_api_geometry-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/PKG-INFO` & `ansys_api_geometry-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.4.2
-Summary: Autogenerated Python gRPC interface package for ansys-api-geometry, built on 13:50:05 on 24 May 2024
+Version: 0.4.3
+Summary: Autogenerated Python gRPC interface package for ansys-api-geometry, built on 13:05:40 on 31 May 2024
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-geometry/#readme
 Project-URL: Source, https://github.com/ansys/ansys-api-geometry/
 Project-URL: Tracker, https://github.com/ansys/ansys-api-geometry/issues/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: grpcio~=1.47
+Requires-Dist: grpcio~=1.44
 Requires-Dist: protobuf<6,>=3.19
-Requires-Dist: ansys-api-dbu==0.3.1
+Requires-Dist: ansys-api-dbu==0.3.2
 
 ### ansys-api-geometry gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files for
 the Ansys Geometry Service.
```

### Comparing `ansys_api_geometry-0.4.2/README.md` & `ansys_api_geometry-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/bodies.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/bodies.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/commands.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/commands.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/components.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/components.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/coordinatesystems.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/coordinatesystems.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/curves.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/curves.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/edges.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/edges.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/faces.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/faces.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/facettools.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/facettools.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/materials.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/materials.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/measuretools.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/measuretools.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/meshes.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/meshes.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/models.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/models.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/namedselections.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/namedselections.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/parts.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/parts.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/preparetools.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/preparetools.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys/api/geometry/v0/repairtools.proto` & `ansys_api_geometry-0.4.3/ansys/api/geometry/v0/repairtools.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/PKG-INFO` & `ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.4.2
-Summary: Autogenerated Python gRPC interface package for ansys-api-geometry, built on 13:50:05 on 24 May 2024
+Version: 0.4.3
+Summary: Autogenerated Python gRPC interface package for ansys-api-geometry, built on 13:05:40 on 31 May 2024
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-geometry/#readme
 Project-URL: Source, https://github.com/ansys/ansys-api-geometry/
 Project-URL: Tracker, https://github.com/ansys/ansys-api-geometry/issues/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: grpcio~=1.47
+Requires-Dist: grpcio~=1.44
 Requires-Dist: protobuf<6,>=3.19
-Requires-Dist: ansys-api-dbu==0.3.1
+Requires-Dist: ansys-api-dbu==0.3.2
 
 ### ansys-api-geometry gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files for
 the Ansys Geometry Service.
```

### Comparing `ansys_api_geometry-0.4.2/ansys_api_geometry.egg-info/SOURCES.txt` & `ansys_api_geometry-0.4.3/ansys_api_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys_api_geometry-0.4.2/setup.py` & `ansys_api_geometry-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         maintainer_email="pyansys.core@ansys.com",
         description=description,
         long_description=long_description,
         long_description_content_type="text/markdown",
         url=f"https://github.com/ansys/{package_name}",
         license="MIT",
         python_requires=">=3.7",
-        install_requires=["grpcio~=1.47", "protobuf>=3.19,<6", "ansys-api-dbu==0.3.1"],
+        install_requires=["grpcio~=1.44", "protobuf>=3.19,<6", "ansys-api-dbu==0.3.2"],
         packages=setuptools.find_namespace_packages(".", include=("ansys.*",)),
         package_data={
             "": ["*.proto", "*.pyi", "py.typed", "VERSION"],
         },
         entry_points={
             "ansys.tools.protoc_helper.proto_provider": [
                 f"{dot_package_name}={dot_package_name}"
```

