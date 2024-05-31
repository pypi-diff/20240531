# Comparing `tmp/pytest_cmake-0.6.0.tar.gz` & `tmp/pytest_cmake-0.7.0.tar.gz`

## Comparing `pytest_cmake-0.6.0.tar` & `pytest_cmake-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/build_backend.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/build_config.py
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/cmake/FindPytest.cmake
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/cmake/PytestAddTests.cmake
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/setup.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/LICENSE
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/README.md
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/build_backend.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/build_config.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/cmake/FindPytest.cmake
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/cmake/PytestAddTests.cmake
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/setup.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/README.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pytest_cmake-0.7.0/PKG-INFO
```

### Comparing `pytest_cmake-0.6.0/build_config.py` & `pytest_cmake-0.7.0/build_config.py`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.6.0/cmake/FindPytest.cmake` & `pytest_cmake-0.7.0/cmake/FindPytest.cmake`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.6.0/cmake/PytestAddTests.cmake` & `pytest_cmake-0.7.0/cmake/PytestAddTests.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -82,25 +82,26 @@
             if (NOT matching)
                 continue()
             endif()
 
             set(_class ${CMAKE_MATCH_3})
             set(_func ${CMAKE_MATCH_4})
 
+            if (TRIM_FROM_NAME)
+                set(pattern "${TRIM_FROM_NAME}")
+                string(REGEX REPLACE "${pattern}" "" _class "${_class}")
+                string(REGEX REPLACE "${pattern}" "" _func "${_func}")
+            endif()
+
             if (_class)
                 set(test_name "${_class}.${_func}")
             else()
                 set(test_name "${_func}")
             endif()
 
-            if (TRIM_FROM_NAME)
-                string(REGEX REPLACE
-                        "${TRIM_FROM_NAME}" "" test_name "${test_name}")
-            endif()
-
             set(test_name "${TEST_GROUP_NAME}.${test_name}")
             set(test_case "${WORKING_DIRECTORY}/${line}")
 
             string(APPEND _content
                 "add_test(\n"
                 "    \"${test_name}\"\n"
                 "    ${PYTEST_EXECUTABLE} \"${test_case}\"\n"
```

### Comparing `pytest_cmake-0.6.0/setup.py` & `pytest_cmake-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         subprocess.call(["cmake", "-P", str(script_path), "-VV"])
         return install.run(self)
 
 
 setup(
     name="pytest-cmake",
-    version="0.6.0",
+    version="0.7.0",
     data_files=[
         (
             "share/Pytest/cmake",
             [
                 "build/PytestConfig.cmake",
                 "build/PytestConfigVersion.cmake",
                 "cmake/FindPytest.cmake",
```

### Comparing `pytest_cmake-0.6.0/.gitignore` & `pytest_cmake-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.6.0/LICENSE` & `pytest_cmake-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.6.0/README.md` & `pytest_cmake-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Pytest CMake
 
 [![PyPi version](https://img.shields.io/pypi/v/pytest-cmake.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.python.org/pypi/pytest-cmake)
 [![CMake](https://img.shields.io/badge/CMake-3.20...3.29-blue.svg?logo=CMake&logoColor=blue)](https://cmake.org)
-[![Documentation](https://readthedocs.org/projects/pytest-cmake/badge/?version=stable)](https://pytest-cmake.readthedocs.io/en/stable/)
-[![Test](https://github.com/buddly27/pytest-cmake/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/buddly27/pytest-cmake/actions/workflows/test.yml)
+[![Test](https://github.com/python-cmake/pytest-cmake/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/python-cmake/pytest-cmake/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This project provides convenient ways to use [Pytest](https://docs.pytest.org/)
 within a [CMake](https://cmake.org/) project. The package can be discovered from a specific range of
 versions on Linux, macOS or Windows using the
 [find_package](https://cmake.org/cmake/help/latest/command/find_package.html)
 function:
 
 ```cmake
-find_package(Pytest 4.6.11 REQUIRED)
+find_package(Pytest 8.2.1 REQUIRED)
 ```
 
 A ``pytest_discover_tests`` function is provided to simplify automatic
 testing for C++ projects with Python bindings. It can create CTest tests
-for each Python test collected within a correct environment:
+for each Python test collected within a controlled environment:
 
 ```cmake
 pytest_discover_tests(
     PythonTest
     LIBRARY_PATH_PREPEND
         $<TARGET_FILE_DIR:MyLibrary>
     PYTHON_PATH_PREPEND
@@ -44,8 +43,8 @@
     Start 4: PythonTest.greet_michael
 4/4 Test #4: PythonTest.greet_michael .........   Passed    0.54 sec
 ```
 
 ## Documentation
 
 Full documentation, including installation and setup guides, can be found at
-https://pytest-cmake.readthedocs.io/en/stable/
+https://python-cmake.github.io/pytest-cmake/
```

### Comparing `pytest_cmake-0.6.0/pyproject.toml` & `pytest_cmake-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "cmake >= 3.20, < 3.30"
 ]
 build-backend = "build_backend"
 backend-path = ["."]
 
 [project]
 name = "pytest-cmake"
-version = "0.6.0"
+version = "0.7.0"
 description = "Provide CMake module for Pytest"
 readme = "README.md"
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4"
 license = {file = "LICENSE"}
 keywords = ["cmake", "pytest", "development"]
 authors = [
     {name = "Jeremy Retailleau", email = "jeremy.retailleau@gmail.com" }
@@ -32,14 +32,20 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
+[project.urls]
+Documentation = "https://python-cmake.github.io/pytest-cmake"
+Repository = "https://github.com/python-cmake/pytest-cmake"
+Issues = "https://github.com/python-cmake/pytest-cmake/issues"
+Changelog = "https://python-cmake.github.io/pytest-cmake/release/release_notes.html"
+
 [tool.hatch.build.hooks.custom]
 require-runtime-dependencies = true
 path = "build_config.py"
 
 [tool.hatch.build.targets.wheel.shared-data]
 "build/PytestConfig.cmake" = "share/Pytest/cmake/PytestConfig.cmake"
 "build/PytestConfigVersion.cmake" = "share/Pytest/cmake/PytestConfigVersion.cmake"
```

### Comparing `pytest_cmake-0.6.0/PKG-INFO` & `pytest_cmake-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.3
 Name: pytest-cmake
-Version: 0.6.0
+Version: 0.7.0
 Summary: Provide CMake module for Pytest
+Project-URL: Documentation, https://python-cmake.github.io/pytest-cmake
+Project-URL: Repository, https://github.com/python-cmake/pytest-cmake
+Project-URL: Issues, https://github.com/python-cmake/pytest-cmake/issues
+Project-URL: Changelog, https://python-cmake.github.io/pytest-cmake/release/release_notes.html
 Author-email: Jeremy Retailleau <jeremy.retailleau@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Retailleau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -42,31 +46,30 @@
 Requires-Dist: pytest<9,>=4
 Description-Content-Type: text/markdown
 
 # Pytest CMake
 
 [![PyPi version](https://img.shields.io/pypi/v/pytest-cmake.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.python.org/pypi/pytest-cmake)
 [![CMake](https://img.shields.io/badge/CMake-3.20...3.29-blue.svg?logo=CMake&logoColor=blue)](https://cmake.org)
-[![Documentation](https://readthedocs.org/projects/pytest-cmake/badge/?version=stable)](https://pytest-cmake.readthedocs.io/en/stable/)
-[![Test](https://github.com/buddly27/pytest-cmake/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/buddly27/pytest-cmake/actions/workflows/test.yml)
+[![Test](https://github.com/python-cmake/pytest-cmake/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/python-cmake/pytest-cmake/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This project provides convenient ways to use [Pytest](https://docs.pytest.org/)
 within a [CMake](https://cmake.org/) project. The package can be discovered from a specific range of
 versions on Linux, macOS or Windows using the
 [find_package](https://cmake.org/cmake/help/latest/command/find_package.html)
 function:
 
 ```cmake
-find_package(Pytest 4.6.11 REQUIRED)
+find_package(Pytest 8.2.1 REQUIRED)
 ```
 
 A ``pytest_discover_tests`` function is provided to simplify automatic
 testing for C++ projects with Python bindings. It can create CTest tests
-for each Python test collected within a correct environment:
+for each Python test collected within a controlled environment:
 
 ```cmake
 pytest_discover_tests(
     PythonTest
     LIBRARY_PATH_PREPEND
         $<TARGET_FILE_DIR:MyLibrary>
     PYTHON_PATH_PREPEND
@@ -88,8 +91,8 @@
     Start 4: PythonTest.greet_michael
 4/4 Test #4: PythonTest.greet_michael .........   Passed    0.54 sec
 ```
 
 ## Documentation
 
 Full documentation, including installation and setup guides, can be found at
-https://pytest-cmake.readthedocs.io/en/stable/
+https://python-cmake.github.io/pytest-cmake/
```

