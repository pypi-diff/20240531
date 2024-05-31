# Comparing `tmp/django-bulk-tracker-0.0.7.tar.gz` & `tmp/django_bulk_tracker-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulk-tracker-0.0.7.tar", last modified: Thu Jul  6 16:33:01 2023, max compression
+gzip compressed data, was "django_bulk_tracker-0.0.8.tar", last modified: Fri May 31 17:30:42 2024, max compression
```

## Comparing `django-bulk-tracker-0.0.7.tar` & `django_bulk_tracker-0.0.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/bulk_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/helper_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_update_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.593367 django_bulk_tracker-0.0.8/bulk_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/helper_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/bulk_tracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-31 17:30:42.000000 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 17:30:42.000000 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:30:42.000000 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 17:30:42.000000 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 17:30:42.000000 django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-31 17:30:42.601367 django_bulk_tracker-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:42.597367 django_bulk_tracker-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/test_create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/test_delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-31 17:30:33.000000 django_bulk_tracker-0.0.8/tests/test_update_signal.py
```

### Comparing `django-bulk-tracker-0.0.7/PKG-INFO` & `django_bulk_tracker-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
@@ -16,33 +16,39 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: Django>=3.2
+Requires-Dist: django-model-utils>=4.0.0
 Provides-Extra: testing
+Requires-Dist: pytest>=7.2.1; extra == "testing"
+Requires-Dist: tox>=4.4.5; extra == "testing"
 
 django-bulk-tracker
 ===============
 
 [![Build Status](https://github.com/hassaanalansary/django-bulk-tracker/actions/workflows/tests.yml/badge.svg)](https://github.com/hassaanalansary/django-bulk-tracker/actions)
 
 
-
+Documentation
+=============
+https://django-bulk-tracker.readthedocs.io/en/latest/
 
 Run tests
 ==========
 ```shell
 pip install -r requirements_dev.txt
 pytest
 ```
 
 Contribute
-----------
+==========
 
 If you have great ideas for django-bulk-tracker, or if you like to improve something,
 feel free to fork this repository and/or create a pull request. 
 I'm open for suggestions. 
 If you like to discuss something with me (about django-bulk-tracker), please open an issue.
```

### Comparing `django-bulk-tracker-0.0.7/README.md` & `django_bulk_tracker-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 django-bulk-tracker
 ===============
 
 [![Build Status](https://github.com/hassaanalansary/django-bulk-tracker/actions/workflows/tests.yml/badge.svg)](https://github.com/hassaanalansary/django-bulk-tracker/actions)
 
 
-
+Documentation
+=============
+https://django-bulk-tracker.readthedocs.io/en/latest/
 
 Run tests
 ==========
 ```shell
 pip install -r requirements_dev.txt
 pytest
 ```
 
 Contribute
-----------
+==========
 
 If you have great ideas for django-bulk-tracker, or if you like to improve something,
 feel free to fork this repository and/or create a pull request. 
 I'm open for suggestions. 
 If you like to discuss something with me (about django-bulk-tracker), please open an issue.
```

### Comparing `django-bulk-tracker-0.0.7/bulk_tracker/helper_objects.py` & `django_bulk_tracker-0.0.8/bulk_tracker/helper_objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,7 +20,8 @@
 @dataclass
 class TrackingInfo:
     user: User | None = None
     comment: str | None = None
     reason: Model | None = None
     system: str | None = None
     kwargs: dict[str, Any] = field(default_factory=dict)
+    is_robust: bool = False
```

### Comparing `django-bulk-tracker-0.0.7/bulk_tracker/managers.py` & `django_bulk_tracker-0.0.8/bulk_tracker/managers.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/bulk_tracker/models.py` & `django_bulk_tracker-0.0.8/bulk_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/bulk_tracker/signals.py` & `django_bulk_tracker-0.0.8/bulk_tracker/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any
 
+from django.db import transaction
 from django.dispatch import Signal
 
 from bulk_tracker.helper_objects import ModifiedObject, TrackingInfo
 
 
 if TYPE_CHECKING:
     from bulk_tracker.models import BulkTrackerModel
@@ -57,18 +58,24 @@
 
 
 def send_post_create_signal(
     objs: Iterable[BulkTrackerModel], model: type[BulkTrackerModel], tracking_info_: TrackingInfo | None = None
 ):
     modified_objects = [ModifiedObject(ob, {}) for ob in objs]
     if modified_objects:
-        post_create_signal.send(
-            objects=modified_objects,
-            sender=model,
-            tracking_info_=tracking_info_,
+        if tracking_info_ and tracking_info_.is_robust:
+            method = post_create_signal.send_robust
+        else:
+            method = post_create_signal.send
+        transaction.on_commit(
+            lambda: method(
+                objects=modified_objects,
+                sender=model,
+                tracking_info_=tracking_info_,
+            )
         )
 
 
 def send_post_update_signal(
     queryset: Iterable[BulkTrackerModel],
     model: type[BulkTrackerModel],
     old_values: dict[int, [dict[str, Any]]],  # {pk: changed_values}
@@ -81,24 +88,38 @@
         for key, old_value in changed.items():
             if getattr(obj, key) != old_value:  # if new_values != old_value
                 diff_dict[key] = old_value
         if diff_dict:
             modified_objects.append(ModifiedObject(obj, diff_dict))
 
     if modified_objects:
-        post_update_signal.send(
-            sender=model,
-            objects=modified_objects,
-            tracking_info_=tracking_info_,
+        if tracking_info_ and tracking_info_.is_robust:
+            method = post_update_signal.send_robust
+        else:
+            method = post_update_signal.send
+        transaction.on_commit(
+            lambda: method(
+                sender=model,
+                objects=modified_objects,
+                tracking_info_=tracking_info_,
+            )
         )
 
 
 def send_post_delete_signal(
-    objs: Iterable[BulkTrackerModel], model: type[BulkTrackerModel], tracking_info_: TrackingInfo | None = None
+    objs: Iterable[BulkTrackerModel],
+    model: type[BulkTrackerModel],
+    tracking_info_: TrackingInfo | None = None,
 ):
     modified_objects = [ModifiedObject(ob, {}) for ob in objs]
     if modified_objects:
-        post_delete_signal.send(
-            objects=modified_objects,
-            sender=model,
-            tracking_info_=tracking_info_,
+        if tracking_info_ and tracking_info_.is_robust:
+            method = post_delete_signal.send_robust
+        else:
+            method = post_delete_signal.send
+        transaction.on_commit(
+            lambda: method(
+                objects=modified_objects,
+                sender=model,
+                tracking_info_=tracking_info_,
+            )
         )
```

### Comparing `django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/PKG-INFO` & `django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
@@ -16,33 +16,39 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: Django>=3.2
+Requires-Dist: django-model-utils>=4.0.0
 Provides-Extra: testing
+Requires-Dist: pytest>=7.2.1; extra == "testing"
+Requires-Dist: tox>=4.4.5; extra == "testing"
 
 django-bulk-tracker
 ===============
 
 [![Build Status](https://github.com/hassaanalansary/django-bulk-tracker/actions/workflows/tests.yml/badge.svg)](https://github.com/hassaanalansary/django-bulk-tracker/actions)
 
 
-
+Documentation
+=============
+https://django-bulk-tracker.readthedocs.io/en/latest/
 
 Run tests
 ==========
 ```shell
 pip install -r requirements_dev.txt
 pytest
 ```
 
 Contribute
-----------
+==========
 
 If you have great ideas for django-bulk-tracker, or if you like to improve something,
 feel free to fork this repository and/or create a pull request. 
 I'm open for suggestions. 
 If you like to discuss something with me (about django-bulk-tracker), please open an issue.
```

### Comparing `django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/SOURCES.txt` & `django_bulk_tracker-0.0.8/django_bulk_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/Makefile` & `django_bulk_tracker-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/make.bat` & `django_bulk_tracker-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/source/conf.py` & `django_bulk_tracker-0.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/source/index.rst` & `django_bulk_tracker-0.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/source/installation.rst` & `django_bulk_tracker-0.0.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/docs/source/usage.rst` & `django_bulk_tracker-0.0.8/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/setup.cfg` & `django_bulk_tracker-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.7/tests/test_create_signal.py` & `django_bulk_tracker-0.0.8/tests/test_create_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from unittest.mock import patch
 
-from django.test import TestCase
+from django.test import TransactionTestCase
 
 from bulk_tracker.helper_objects import ModifiedObject, TrackingInfo
 from bulk_tracker.signals import post_create_signal
 from tests.models import Author, Post
 
 
-class TestCreateSignal(TestCase):
-    @classmethod
-    def setUpTestData(cls):
-        cls.author_john = Author.objects.create(first_name="John", last_name="Doe")
+class TestCreateSignal(TransactionTestCase):
+    serialized_rollback = True
+
+    def setUp(self):
+        self.author_john = Author.objects.create(first_name="John", last_name="Doe")
 
     def test_model_create_should_emit_post_create_signal(self):
         # Arrange
         signal_called_with = {}
 
         def post_create_receiver(
             sender,
@@ -108,68 +109,68 @@
         modified_objects: list[ModifiedObject[Post]] = signal_called_with["objects"]
 
         self.assertEqual("Sound of Winter", modified_objects[0].instance.title)
         self.assertEqual("1998-01-08", modified_objects[0].instance.publish_date)
         self.assertEqual(self.author_john, modified_objects[0].instance.author)
         self.assertEqual({}, modified_objects[0].changed_values)
 
-    @patch('bulk_tracker.signals.post_create_signal.send')
+    @patch("bulk_tracker.signals.post_create_signal.send")
     def test_model_save_should_only_emit_post_create_signal_once(self, mocked_signal):
         # Arrange
         signal_called_with = {}
 
         def post_create_receiver(
-                sender,
-                objects: list[ModifiedObject[Post]],
-                tracking_info_: TrackingInfo | None = None,
-                **kwargs,
+            sender,
+            objects: list[ModifiedObject[Post]],
+            tracking_info_: TrackingInfo | None = None,
+            **kwargs,
         ):
             signal_called_with["objects"] = objects
             signal_called_with["tracking_info_"] = tracking_info_
 
         post_create_signal.connect(post_create_receiver, sender=Post)
 
         # Act
         Post(title="Sound of Winter", publish_date="1998-01-08", author=self.author_john).save()
 
         # Assert
         self.assertEqual(mocked_signal.call_count, 1, msg="The signal wasn't called once")
 
-    @patch('bulk_tracker.signals.post_create_signal.send')
+    @patch("bulk_tracker.signals.post_create_signal.send")
     def test_model_create_should_only_emit_post_create_signal_once(self, mocked_signal):
         # Arrange
         signal_called_with = {}
 
         def post_create_receiver(
-                sender,
-                objects: list[ModifiedObject[Post]],
-                tracking_info_: TrackingInfo | None = None,
-                **kwargs,
+            sender,
+            objects: list[ModifiedObject[Post]],
+            tracking_info_: TrackingInfo | None = None,
+            **kwargs,
         ):
             signal_called_with["objects"] = objects
             signal_called_with["tracking_info_"] = tracking_info_
 
         post_create_signal.connect(post_create_receiver, sender=Post)
 
         # Act
         Post.objects.create(title="Sound of Winter", publish_date="1998-03-08", author=self.author_john)
 
         # Assert
         self.assertEqual(mocked_signal.call_count, 1, msg="The signal wasn't called once")
 
-    @patch('bulk_tracker.signals.post_create_signal.send')
+    @patch("bulk_tracker.signals.post_create_signal.send")
     def test_model_bulk_create_should_only_emit_post_create_signal_once(self, mocked_signal):
         # Arrange
         signal_called_with = {}
 
         def post_create_receiver(
-                sender,
-                objects: list[ModifiedObject[Post]],
-                tracking_info_: TrackingInfo | None = None,
-                **kwargs,
+            sender,
+            objects: list[ModifiedObject[Post]],
+            tracking_info_: TrackingInfo | None = None,
+            **kwargs,
         ):
             signal_called_with["objects"] = objects
             signal_called_with["tracking_info_"] = tracking_info_
 
         post_create_signal.connect(post_create_receiver, sender=Post)
 
         posts = [
@@ -178,7 +179,64 @@
         ]
 
         # Act
         Post.objects.bulk_create(posts)
 
         # Assert
         self.assertEqual(mocked_signal.call_count, 1, msg="The signal wasn't called once")
+
+    @patch("bulk_tracker.signals.post_create_signal.send")
+    def test_create_signal_should_be_only_emitted_after_transaction_commit(self, mocked_signal):
+        # Arrange
+
+        def post_create_receiver(
+            sender,
+            objects: list[ModifiedObject[Post]],
+            tracking_info_: TrackingInfo | None = None,
+            **kwargs,
+        ):
+            pass
+
+        post_create_signal.connect(post_create_receiver, sender=Post)
+
+        posts = [
+            Post(title="Sound of Winter", publish_date="1998-01-08", author=self.author_john),
+            Post(title="Sound of Summer", publish_date="1998-06-08", author=self.author_john),
+        ]
+
+        # Act
+        from django.db import transaction
+
+        with transaction.atomic():
+            Post.objects.bulk_create(posts)
+            mocked_signal.assert_not_called()
+
+            author = Author.objects.create(first_name="Jane", last_name="Doe")
+            author.delete()
+
+        # Assert
+        self.assertEqual(
+            mocked_signal.call_count,
+            2,
+            msg=f"The signal wasn't called twice. it was called {mocked_signal.call_count}.",
+        )
+        signal_called_with_first = mocked_signal.call_args_list[0].kwargs
+        self.assertEqual(signal_called_with_first["sender"], Post)
+
+        signal_called_with_second = mocked_signal.call_args_list[1].kwargs
+        self.assertEqual(signal_called_with_second["sender"], Author)
+
+    @patch("bulk_tracker.signals.post_create_signal.send")
+    @patch("bulk_tracker.signals.post_create_signal.send_robust")
+    def test_should_use_robust_send_if_is_robust_is_true_in_tracking_info(self, mocked_signal_robust, mocked_signal):
+        # Arrange
+        posts = [
+            Post(title="Sound of Winter", publish_date="1998-01-08", author=self.author_john),
+            Post(title="Sound of Summer", publish_date="1998-06-08", author=self.author_john),
+        ]
+
+        # Act
+        Post.objects.bulk_create(posts, tracking_info_=TrackingInfo(is_robust=True))
+
+        # Assert
+        mocked_signal.assert_not_called()
+        mocked_signal_robust.assert_called_once()
```

### Comparing `django-bulk-tracker-0.0.7/tests/test_update_signal.py` & `django_bulk_tracker-0.0.8/tests/test_update_signal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 from datetime import datetime
+from unittest.mock import patch
 
-from django.test import TestCase
+from django.test import TransactionTestCase
 
 from bulk_tracker.helper_objects import ModifiedObject, TrackingInfo
 from bulk_tracker.signals import post_update_signal
 from tests.models import Author, Post
 
 
-class TestUpdateSignal(TestCase):
-    @classmethod
-    def setUpTestData(cls):
-        cls.author_john = Author.objects.create(first_name="John", last_name="Doe")
-        cls.author_soha = Author.objects.create(first_name="Soha", last_name="Reid")
-
+class TestUpdateSignal(TransactionTestCase):
     def setUp(self):
+        self.author_john = Author.objects.create(first_name="John", last_name="Doe")
+        self.author_soha = Author.objects.create(first_name="Soha", last_name="Reid")
+
         Post.objects.create(title="Defend the Lie", publish_date="1999-05-19", author=self.author_john)
         Post.objects.create(title="Cold Vice", publish_date="2001-07-22", author=self.author_john)
         Post.objects.create(title="Sound of Winter", publish_date="2000-09-12", author=self.author_john)
 
         Post.objects.create(title="Prince's Advent", publish_date="1999-05-19", author=self.author_soha)
         Post.objects.create(title="The Midnight Wolf", publish_date="2002-01-12", author=self.author_soha)
 
@@ -63,27 +62,31 @@
             self.assertEqual(datetime.strptime("1999-12-31", "%Y-%m-%d").date(), modified_object.instance.publish_date)
             self.assertEqual(
                 datetime.strptime("1999-05-19", "%Y-%m-%d").date(), modified_object.changed_values["publish_date"]
             )
 
     def test_should_raise_attribute_error_when_model_does_not_have_tracker(self):
         # Arrange
+        cache_tracker = Post.tracker
         del Post.tracker
         posts = Post.objects.filter(publish_date="1999-05-19").order_by("publish_date")
         for post in posts:
             post.publish_date = "1999-12-31"
 
         # Act & Assert
         with self.assertRaises(AttributeError) as context:
             posts[0].save()
         self.assertEqual(
             f"Model {Post} doesn't have tracker, please add `tracker = FieldTracker()` to your model",
             context.exception.args[0],
         )
 
+        # Cleanup
+        Post.tracker = cache_tracker
+
     def test_model_save_should_emit_post_update_signal(self):
         # Arrange
         signal_called_with = {}
 
         def post_update_receiver(
             sender,
             objects: list[ModifiedObject[Post]],
@@ -132,7 +135,51 @@
         self.assertTrue(signal_called_with != {})
         self.assertEqual(1, len(signal_called_with["objects"]))
         self.assertEqual(None, signal_called_with["tracking_info_"])
 
         modified_objects: list[ModifiedObject[Post]] = signal_called_with["objects"]
         self.assertEqual("The Sunset Wolf", modified_objects[0].instance.title)
         self.assertEqual("The Midnight Wolf", modified_objects[0].changed_values["title"])
+
+    @patch("bulk_tracker.signals.post_update_signal.send")
+    def test_update_signal_should_be_only_emitted_after_transaction_commit(self, mocked_signal):
+        # Arrange
+
+        def post_update_receiver(
+            sender,
+            objects: list[ModifiedObject[Post]],
+            tracking_info_: TrackingInfo | None = None,
+            **kwargs,
+        ):
+            pass
+
+        post_update_signal.connect(post_update_receiver, sender=Post)
+        post = Post.objects.create(title="Sound of Summer", publish_date="1998-06-08", author=self.author_john)
+
+        # Act
+        from django.db import transaction
+
+        with transaction.atomic():
+            post.title = "Sound of Winter"
+            Post.objects.bulk_update([post], fields=["title"])
+            mocked_signal.assert_not_called()
+
+            self.author_john.first_name = "Johny"
+            Author.objects.bulk_update([self.author_john], fields=["first_name"])
+
+        # Assert
+        mocked_signal.assert_called_once()
+        signal_called_with_first = mocked_signal.call_args_list[0].kwargs
+        self.assertEqual(signal_called_with_first["sender"], Post)
+
+    @patch("bulk_tracker.signals.post_update_signal.send")
+    @patch("bulk_tracker.signals.post_update_signal.send_robust")
+    def test_should_use_robust_send_if_is_robust_is_true_in_tracking_info(self, mocked_signal_robust, mocked_signal):
+        # Arrange
+        self.author_john.first_name = "Johny"
+
+        # Act
+        self.author_john.save(tracking_info_=TrackingInfo(is_robust=True))
+
+        # Assert
+        mocked_signal.assert_not_called()
+        mocked_signal_robust.assert_called_once()
```

