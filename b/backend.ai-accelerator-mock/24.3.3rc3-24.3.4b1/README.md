# Comparing `tmp/backend.ai-accelerator-mock-24.3.3rc3.tar.gz` & `tmp/backend.ai-accelerator-mock-24.3.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-mock-24.3.3rc3.tar", last modified: Tue Apr 30 16:09:49 2024, max compression
+gzip compressed data, was "backend.ai-accelerator-mock-24.3.4b1.tar", last modified: Fri May 31 19:10:20 2024, max compression
```

## Comparing `backend.ai-accelerator-mock-24.3.3rc3.tar` & `backend.ai-accelerator-mock-24.3.4b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.197435 backend.ai-accelerator-mock-24.3.3rc3/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-30 16:09:49.197435 backend.ai-accelerator-mock-24.3.3rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.193435 backend.ai-accelerator-mock-24.3.3rc3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.193435 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.193435 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.197435 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:09:49.197435 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-30 16:09:49.000000 backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:09:49.197435 backend.ai-accelerator-mock-24.3.3rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-30 16:09:48.000000 backend.ai-accelerator-mock-24.3.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.486585 backend.ai-accelerator-mock-24.3.4b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-31 19:10:20.486585 backend.ai-accelerator-mock-24.3.4b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.482585 backend.ai-accelerator-mock-24.3.4b1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.482585 backend.ai-accelerator-mock-24.3.4b1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.482585 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.486585 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:20.486585 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-31 19:10:20.000000 backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:10:20.486585 backend.ai-accelerator-mock-24.3.4b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-31 19:10:19.000000 backend.ai-accelerator-mock-24.3.4b1/setup.py
```

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/PKG-INFO` & `backend.ai-accelerator-mock-24.3.4b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 24.3.3rc3
+Version: 24.3.4b1
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -17,20 +17,20 @@
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiodocker~=0.21.0
-Requires-Dist: backend.ai-agent==24.03.3rc3
-Requires-Dist: backend.ai-cli==24.03.3rc3
-Requires-Dist: backend.ai-common==24.03.3rc3
-Requires-Dist: backend.ai-kernel-binary==24.03.3rc3
-Requires-Dist: backend.ai-kernel-helper==24.03.3rc3
-Requires-Dist: backend.ai-plugin==24.03.3rc3
+Requires-Dist: backend.ai-agent==24.03.4b1
+Requires-Dist: backend.ai-cli==24.03.4b1
+Requires-Dist: backend.ai-common==24.03.4b1
+Requires-Dist: backend.ai-kernel-binary==24.03.4b1
+Requires-Dist: backend.ai-kernel-helper==24.03.4b1
+Requires-Dist: backend.ai-plugin==24.03.4b1
 Requires-Dist: trafaret~=2.1
 
 # backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
 
 This plugin deceives the agent and manager to think as if there are accelerator devices.
```

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/plugin.py` & `backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/ai/backend/accelerator/mock/types.py` & `backend.ai-accelerator-mock-24.3.4b1/ai/backend/accelerator/mock/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/PKG-INFO` & `backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 24.3.3rc3
+Version: 24.3.4b1
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -17,20 +17,20 @@
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiodocker~=0.21.0
-Requires-Dist: backend.ai-agent==24.03.3rc3
-Requires-Dist: backend.ai-cli==24.03.3rc3
-Requires-Dist: backend.ai-common==24.03.3rc3
-Requires-Dist: backend.ai-kernel-binary==24.03.3rc3
-Requires-Dist: backend.ai-kernel-helper==24.03.3rc3
-Requires-Dist: backend.ai-plugin==24.03.3rc3
+Requires-Dist: backend.ai-agent==24.03.4b1
+Requires-Dist: backend.ai-cli==24.03.4b1
+Requires-Dist: backend.ai-common==24.03.4b1
+Requires-Dist: backend.ai-kernel-binary==24.03.4b1
+Requires-Dist: backend.ai-kernel-helper==24.03.4b1
+Requires-Dist: backend.ai-plugin==24.03.4b1
 Requires-Dist: trafaret~=2.1
 
 # backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
 
 This plugin deceives the agent and manager to think as if there are accelerator devices.
```

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/backend.ai_accelerator_mock.egg-info/SOURCES.txt` & `backend.ai-accelerator-mock-24.3.4b1/backend.ai_accelerator_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/backend_shim.py` & `backend.ai-accelerator-mock-24.3.4b1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-24.3.3rc3/setup.py` & `backend.ai-accelerator-mock-24.3.4b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     'entry_points': {
         'backendai_accelerator_v21': [
             'mock = ai.backend.accelerator.mock.plugin:MockPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
-        """backend.ai-agent==24.03.3rc3
+        """backend.ai-agent==24.03.4b1
 """,
-        """backend.ai-cli==24.03.3rc3
+        """backend.ai-cli==24.03.4b1
 """,
-        """backend.ai-common==24.03.3rc3
+        """backend.ai-common==24.03.4b1
 """,
-        """backend.ai-kernel-binary==24.03.3rc3
+        """backend.ai-kernel-binary==24.03.4b1
 """,
-        """backend.ai-kernel-helper==24.03.3rc3
+        """backend.ai-kernel-helper==24.03.4b1
 """,
-        """backend.ai-plugin==24.03.3rc3
+        """backend.ai-plugin==24.03.4b1
 """,
         'trafaret~=2.1',
     ),
     'license': 'LGPLv3',
     'long_description': """# backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
@@ -73,11 +73,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.3rc3
+    'version': """24.03.4b1
 """,
     'zip_safe': False,
 })
```

