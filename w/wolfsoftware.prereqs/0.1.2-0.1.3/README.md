# Comparing `tmp/wolfsoftware_prereqs-0.1.2.tar.gz` & `tmp/wolfsoftware_prereqs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfsoftware_prereqs-0.1.2.tar", last modified: Thu May 23 11:57:13 2024, max compression
+gzip compressed data, was "wolfsoftware_prereqs-0.1.3.tar", last modified: Fri May 31 09:29:53 2024, max compression
```

## Comparing `wolfsoftware_prereqs-0.1.2.tar` & `wolfsoftware_prereqs-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:57:13.327583 wolfsoftware_prereqs-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 11:57:13.327583 wolfsoftware_prereqs-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-23 11:57:13.327583 wolfsoftware_prereqs-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:57:13.323583 wolfsoftware_prereqs-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/tests/test_prereqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:57:13.323583 wolfsoftware_prereqs-0.1.2/wolfsoftware/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:57:13.327583 wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-23 11:57:04.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/prerequisite_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:57:13.327583 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 11:57:13.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 11:57:13.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:57:13.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 11:57:13.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 11:57:13.000000 wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:29:53.696897 wolfsoftware_prereqs-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-31 09:29:53.696897 wolfsoftware_prereqs-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 09:29:53.696897 wolfsoftware_prereqs-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:29:53.692897 wolfsoftware_prereqs-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/tests/test_prereqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:29:53.692897 wolfsoftware_prereqs-0.1.3/wolfsoftware/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:29:53.696897 wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-31 09:29:20.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/prerequisite_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:29:53.696897 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-31 09:29:53.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-31 09:29:53.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:29:53.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 09:29:53.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 09:29:53.000000 wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/top_level.txt
```

### Comparing `wolfsoftware_prereqs-0.1.2/LICENSE.md` & `wolfsoftware_prereqs-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.2/PKG-INFO` & `wolfsoftware_prereqs-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.prereqs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Check for the presence of prerequisite commands and returns their paths.
 Home-page: https://github.com/DevelopersToolbox/check-prerequisite-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 License: MIT
 Project-URL:  Source, https://github.com/DevelopersToolbox/check-prerequisite-package
 Project-URL:  Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/issues/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.2 Summary: Check
+Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.3 Summary: Check
 for the presence of prerequisite commands and returns their paths. Home-page:
 https://github.com/DevelopersToolbox/check-prerequisite-package Author: Wolf
 Software Author-email: pypi@wolfsoftware.com License: MIT Project-URL: Source,
 https://github.com/DevelopersToolbox/check-prerequisite-package Project-URL:
 Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/
 issues/ Project-URL: Documentation, https://github.com/DevelopersToolbox/check-
 prerequisite-package Project-URL: Sponsor, https://github.com/sponsors/
```

### Comparing `wolfsoftware_prereqs-0.1.2/README.md` & `wolfsoftware_prereqs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.2/setup.cfg` & `wolfsoftware_prereqs-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.2/setup.py` & `wolfsoftware_prereqs-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required: list[str] = f.read().splitlines()
 
 with open("README.md", 'r', encoding='UTF-8') as f:
     long_description: str = f.read()
 
 setup(
     name='wolfsoftware.prereqs',
-    version='0.1.2',
+    version='0.1.3',
     author='Wolf Software',
     author_email='pypi@wolfsoftware.com',
     description='Check for the presence of prerequisite commands and returns their paths.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=['wolfsoftware.prereqs'],
```

### Comparing `wolfsoftware_prereqs-0.1.2/tests/test_prereqs.py` & `wolfsoftware_prereqs-0.1.3/tests/test_prereqs.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 from typing import Optional
 
 import importlib.metadata
 
 import pytest
 
-from wolfsoftware.prereqs import check_prerequisite, PrerequisiteCheckError  # pylint: disable=import-error
+from wolfsoftware.prereqs import check_prerequisite, PrerequisiteCheckError  # pylint: disable=import-error, no-name-in-module
 
 
 def test_version() -> None:
     """
     Test that a version is defined.
 
     Should return the version of the package.
@@ -79,16 +79,18 @@
 
     Returns:
         None
 
     Raises:
         AssertionError: If the function does not return the expected result.
     """
-    # Mock shutil.which to return valid paths
-    mocker.patch('shutil.which', side_effect=lambda cmd: f"/usr/bin/{cmd}" if cmd in ["python", "git"] else None)
+    # Mock shutil.which to handle the additional path parameter
+    def mock_which(cmd, path=None) -> str:  # pylint: disable=unused-argument
+        return f"/usr/bin/{cmd}"
+    mocker.patch('shutil.which', side_effect=mock_which)
 
     prerequisites: list[str] = ["python", "git"]
     expected_result: dict[str, str] = {
         "python": "/usr/bin/python",
         "git": "/usr/bin/git"
     }
     assert check_prerequisite(prerequisites) == expected_result  # nosec: B101
@@ -110,16 +112,20 @@
     Returns:
         None
 
     Raises:
         AssertionError: If the function does not raise the expected exception or
                         if the exception does not contain the correct error message.
     """
-    # Mock shutil.which to return None for missing commands
-    mocker.patch('shutil.which', side_effect=lambda cmd: f"/usr/bin/{cmd}" if cmd == "python" else None)
+    # Mock shutil.which to handle the additional path parameter
+    def mock_which(cmd, path=None) -> Optional[str]:  # pylint: disable=unused-argument
+        if cmd == "python":
+            return f"/usr/bin/{cmd}"
+        return None
+    mocker.patch('shutil.which', side_effect=mock_which)
 
     prerequisites: list[str] = ["python", "git"]
     with pytest.raises(PrerequisiteCheckError) as exc_info:
         check_prerequisite(prerequisites)
 
     assert len(exc_info.value.errors) == 1  # nosec: B101
     assert exc_info.value.errors[0] == "git is not installed - Aborting"  # nosec: B101
```

### Comparing `wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/__init__.py` & `wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/__init__.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.2/wolfsoftware/prereqs/exceptions.py` & `wolfsoftware_prereqs-0.1.3/wolfsoftware/prereqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.2/wolfsoftware.prereqs.egg-info/PKG-INFO` & `wolfsoftware_prereqs-0.1.3/wolfsoftware.prereqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.prereqs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Check for the presence of prerequisite commands and returns their paths.
 Home-page: https://github.com/DevelopersToolbox/check-prerequisite-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 License: MIT
 Project-URL:  Source, https://github.com/DevelopersToolbox/check-prerequisite-package
 Project-URL:  Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/issues/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.2 Summary: Check
+Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.3 Summary: Check
 for the presence of prerequisite commands and returns their paths. Home-page:
 https://github.com/DevelopersToolbox/check-prerequisite-package Author: Wolf
 Software Author-email: pypi@wolfsoftware.com License: MIT Project-URL: Source,
 https://github.com/DevelopersToolbox/check-prerequisite-package Project-URL:
 Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/
 issues/ Project-URL: Documentation, https://github.com/DevelopersToolbox/check-
 prerequisite-package Project-URL: Sponsor, https://github.com/sponsors/
```

