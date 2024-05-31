# Comparing `tmp/eventum_plugins-1.0.1.tar.gz` & `tmp/eventum_plugins-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_plugins-1.0.1.tar", max compression
+gzip compressed data, was "eventum_plugins-1.0.2.tar", max compression
```

## Comparing `eventum_plugins-1.0.1.tar` & `eventum_plugins-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2024-05-21 17:41:05.247172 eventum_plugins-1.0.1/LICENSE
--rw-r--r--   0        0        0       37 2024-05-21 17:41:05.247172 eventum_plugins-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-21 17:54:41.546979 eventum_plugins-1.0.1/eventum_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 11:40:55.321933 eventum_plugins-1.0.1/eventum_plugins/event/__init__.py
--rw-r--r--   0        0        0      722 2024-05-25 13:00:17.860819 eventum_plugins-1.0.1/eventum_plugins/event/base.py
--rw-r--r--   0        0        0    11216 2024-05-26 11:50:22.309370 eventum_plugins-1.0.1/eventum_plugins/event/jinja.py
--rw-r--r--   0        0        0        0 2024-05-25 13:52:48.830090 eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/__init__.py
--rw-r--r--   0        0        0     5656 2024-05-25 11:40:55.301933 eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/rand.py
--rw-r--r--   0        0        0       29 2024-05-26 11:41:50.809487 eventum_plugins-1.0.1/eventum_plugins/event/tests/static/sample.csv
--rw-r--r--   0        0        0     3316 2024-05-26 11:50:22.309370 eventum_plugins-1.0.1/eventum_plugins/event/tests/test_jinja.py
--rw-r--r--   0        0        0        0 2024-05-25 11:40:23.651940 eventum_plugins-1.0.1/eventum_plugins/input/__init__.py
--rw-r--r--   0        0        0     2173 2024-05-27 17:37:19.844745 eventum_plugins-1.0.1/eventum_plugins/input/base.py
--rw-r--r--   0        0        0     1554 2024-05-27 17:28:58.074867 eventum_plugins-1.0.1/eventum_plugins/input/cron.py
--rw-r--r--   0        0        0     1682 2024-05-27 17:29:08.314866 eventum_plugins-1.0.1/eventum_plugins/input/linspace.py
--rw-r--r--   0        0        0     1129 2024-05-27 17:29:14.294865 eventum_plugins-1.0.1/eventum_plugins/input/sample.py
--rw-r--r--   0        0        0      116 2024-05-26 07:54:34.102677 eventum_plugins-1.0.1/eventum_plugins/input/tests/static/time_pattern_invalid.yml
--rw-r--r--   0        0        0      227 2024-05-26 11:27:33.109687 eventum_plugins-1.0.1/eventum_plugins/input/tests/static/time_pattern_valid.yml
--rw-r--r--   0        0        0     1383 2024-05-26 09:03:08.741710 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_cron.py
--rw-r--r--   0        0        0     2062 2024-05-25 16:56:57.927494 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_linspace.py
--rw-r--r--   0        0        0      814 2024-05-25 17:03:09.517408 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_sample.py
--rw-r--r--   0        0        0     1902 2024-05-26 11:29:21.659661 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_time_patterns.py
--rw-r--r--   0        0        0      843 2024-05-26 07:18:51.813193 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timer.py
--rw-r--r--   0        0        0     2039 2024-05-26 09:37:42.431227 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timestamps.py
--rw-r--r--   0        0        0    18439 2024-05-27 17:30:13.454853 eventum_plugins-1.0.1/eventum_plugins/input/time_patterns.py
--rw-r--r--   0        0        0     1402 2024-05-27 17:29:40.814860 eventum_plugins-1.0.1/eventum_plugins/input/timer.py
--rw-r--r--   0        0        0     1862 2024-05-27 17:29:46.244859 eventum_plugins-1.0.1/eventum_plugins/input/timestamps.py
--rw-r--r--   0        0        0        0 2024-05-22 17:54:51.017205 eventum_plugins-1.0.1/eventum_plugins/output/__init__.py
--rw-r--r--   0        0        0     3915 2024-05-27 18:07:02.584332 eventum_plugins-1.0.1/eventum_plugins/output/base.py
--rw-r--r--   0        0        0     2662 2024-05-27 18:10:13.024289 eventum_plugins-1.0.1/eventum_plugins/output/file.py
--rw-r--r--   0        0        0     4966 2024-05-27 18:09:35.024298 eventum_plugins-1.0.1/eventum_plugins/output/opensearch.py
--rw-r--r--   0        0        0     1525 2024-05-27 18:10:04.304291 eventum_plugins-1.0.1/eventum_plugins/output/stdout.py
--rw-r--r--   0        0        0     1036 2024-05-26 15:11:30.906539 eventum_plugins-1.0.1/eventum_plugins/output/tests/test_file.py
--rw-r--r--   0        0        0     3971 2024-05-26 14:49:45.596850 eventum_plugins-1.0.1/eventum_plugins/output/tests/test_opensearch.py
--rw-r--r--   0        0        0        0 2024-05-24 16:48:46.953250 eventum_plugins-1.0.1/eventum_plugins/py.typed
--rw-r--r--   0        0        0        0 2024-05-25 11:40:43.771936 eventum_plugins-1.0.1/eventum_plugins/utils/__init__.py
--rw-r--r--   0        0        0      298 2024-05-25 14:02:03.079955 eventum_plugins-1.0.1/eventum_plugins/utils/modules.py
--rw-r--r--   0        0        0      469 2024-05-27 17:29:51.864858 eventum_plugins-1.0.1/eventum_plugins/utils/numpy_time.py
--rw-r--r--   0        0        0     1411 2024-05-24 18:11:28.351759 eventum_plugins-1.0.1/eventum_plugins/utils/relative_time.py
--rw-r--r--   0        0        0     1311 2024-05-22 17:28:13.897819 eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_relative_time.py
--rw-r--r--   0        0        0      715 2024-05-26 09:36:13.411247 eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_timeseries.py
--rw-r--r--   0        0        0      634 2024-05-26 09:35:32.351257 eventum_plugins-1.0.1/eventum_plugins/utils/timeseries.py
--rw-r--r--   0        0        0     1386 2024-05-27 18:10:53.894280 eventum_plugins-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 eventum_plugins-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 17:41:05.247172 eventum_plugins-1.0.2/LICENSE
+-rw-r--r--   0        0        0       37 2024-05-21 17:41:05.247172 eventum_plugins-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 17:54:41.546979 eventum_plugins-1.0.2/eventum_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:55.321933 eventum_plugins-1.0.2/eventum_plugins/event/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-25 13:00:17.860819 eventum_plugins-1.0.2/eventum_plugins/event/base.py
+-rw-r--r--   0        0        0    11294 2024-05-31 19:28:17.297905 eventum_plugins-1.0.2/eventum_plugins/event/jinja.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:52:48.830090 eventum_plugins-1.0.2/eventum_plugins/event/jinja_modules/__init__.py
+-rw-r--r--   0        0        0     5656 2024-05-25 11:40:55.301933 eventum_plugins-1.0.2/eventum_plugins/event/jinja_modules/rand.py
+-rw-r--r--   0        0        0       29 2024-05-26 11:41:50.809487 eventum_plugins-1.0.2/eventum_plugins/event/tests/static/sample.csv
+-rw-r--r--   0        0        0     3316 2024-05-26 11:50:22.309370 eventum_plugins-1.0.2/eventum_plugins/event/tests/test_jinja.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:23.651940 eventum_plugins-1.0.2/eventum_plugins/input/__init__.py
+-rw-r--r--   0        0        0     2173 2024-05-27 17:37:19.844745 eventum_plugins-1.0.2/eventum_plugins/input/base.py
+-rw-r--r--   0        0        0     1554 2024-05-27 17:28:58.074867 eventum_plugins-1.0.2/eventum_plugins/input/cron.py
+-rw-r--r--   0        0        0     1682 2024-05-27 17:29:08.314866 eventum_plugins-1.0.2/eventum_plugins/input/linspace.py
+-rw-r--r--   0        0        0     1129 2024-05-27 17:29:14.294865 eventum_plugins-1.0.2/eventum_plugins/input/sample.py
+-rw-r--r--   0        0        0      116 2024-05-26 07:54:34.102677 eventum_plugins-1.0.2/eventum_plugins/input/tests/static/time_pattern_invalid.yml
+-rw-r--r--   0        0        0      227 2024-05-26 11:27:33.109687 eventum_plugins-1.0.2/eventum_plugins/input/tests/static/time_pattern_valid.yml
+-rw-r--r--   0        0        0     1383 2024-05-26 09:03:08.741710 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_cron.py
+-rw-r--r--   0        0        0     2062 2024-05-25 16:56:57.927494 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_linspace.py
+-rw-r--r--   0        0        0      814 2024-05-25 17:03:09.517408 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_sample.py
+-rw-r--r--   0        0        0     1902 2024-05-26 11:29:21.659661 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_time_patterns.py
+-rw-r--r--   0        0        0      843 2024-05-26 07:18:51.813193 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_timer.py
+-rw-r--r--   0        0        0     2039 2024-05-26 09:37:42.431227 eventum_plugins-1.0.2/eventum_plugins/input/tests/test_timestamps.py
+-rw-r--r--   0        0        0    18439 2024-05-27 17:30:13.454853 eventum_plugins-1.0.2/eventum_plugins/input/time_patterns.py
+-rw-r--r--   0        0        0     1402 2024-05-27 17:29:40.814860 eventum_plugins-1.0.2/eventum_plugins/input/timer.py
+-rw-r--r--   0        0        0     1862 2024-05-27 17:29:46.244859 eventum_plugins-1.0.2/eventum_plugins/input/timestamps.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:54:51.017205 eventum_plugins-1.0.2/eventum_plugins/output/__init__.py
+-rw-r--r--   0        0        0     3915 2024-05-27 18:07:02.584332 eventum_plugins-1.0.2/eventum_plugins/output/base.py
+-rw-r--r--   0        0        0     2662 2024-05-27 18:10:13.024289 eventum_plugins-1.0.2/eventum_plugins/output/file.py
+-rw-r--r--   0        0        0     4966 2024-05-27 18:09:35.024298 eventum_plugins-1.0.2/eventum_plugins/output/opensearch.py
+-rw-r--r--   0        0        0     1525 2024-05-27 18:10:04.304291 eventum_plugins-1.0.2/eventum_plugins/output/stdout.py
+-rw-r--r--   0        0        0     1036 2024-05-26 15:11:30.906539 eventum_plugins-1.0.2/eventum_plugins/output/tests/test_file.py
+-rw-r--r--   0        0        0     3971 2024-05-26 14:49:45.596850 eventum_plugins-1.0.2/eventum_plugins/output/tests/test_opensearch.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:48:46.953250 eventum_plugins-1.0.2/eventum_plugins/py.typed
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:43.771936 eventum_plugins-1.0.2/eventum_plugins/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-25 14:02:03.079955 eventum_plugins-1.0.2/eventum_plugins/utils/modules.py
+-rw-r--r--   0        0        0      469 2024-05-27 17:29:51.864858 eventum_plugins-1.0.2/eventum_plugins/utils/numpy_time.py
+-rw-r--r--   0        0        0     1411 2024-05-24 18:11:28.351759 eventum_plugins-1.0.2/eventum_plugins/utils/relative_time.py
+-rw-r--r--   0        0        0     1311 2024-05-22 17:28:13.897819 eventum_plugins-1.0.2/eventum_plugins/utils/tests/test_relative_time.py
+-rw-r--r--   0        0        0      715 2024-05-26 09:36:13.411247 eventum_plugins-1.0.2/eventum_plugins/utils/tests/test_timeseries.py
+-rw-r--r--   0        0        0      634 2024-05-26 09:35:32.351257 eventum_plugins-1.0.2/eventum_plugins/utils/timeseries.py
+-rw-r--r--   0        0        0     1386 2024-05-31 19:29:25.707897 eventum_plugins-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 eventum_plugins-1.0.2/PKG-INFO
```

### Comparing `eventum_plugins-1.0.1/LICENSE` & `eventum_plugins-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/event/base.py` & `eventum_plugins-1.0.2/eventum_plugins/event/base.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/event/jinja.py` & `eventum_plugins-1.0.2/eventum_plugins/event/jinja.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Iterator, assert_never
 
 from eventum_content_manager.manage import (EVENT_TEMPLATES_DIR,
                                             ContentManagementError,
                                             load_csv_sample)
 from jinja2 import (BaseLoader, Environment, FileSystemLoader, Template,
                     TemplateError, TemplateNotFound, TemplateRuntimeError,
-                    TemplateSyntaxError)
+                    TemplateSyntaxError, Undefined)
 from pydantic import Field, field_validator
 
 from eventum_plugins.event.base import (BaseEventPlugin, EventPluginBaseConfig,
                                         EventPluginConfigurationError,
                                         EventPluginRuntimeError)
 from eventum_plugins.utils.modules import get_module_names
 
@@ -122,14 +122,17 @@
 
 class State:
     def __init__(self) -> None:
         self._state: dict[str, Any] = dict()
 
     def set(self, key: str, value: Any) -> None:
         """Set variable value to state."""
+        if isinstance(value, Undefined):
+            value = None
+
         self._state[key] = value
 
     def get(self, key: str, default: Any | None = None) -> Any:
         """Get variable value from state. If state does not contain
         value with specified `key` then `default` value is returned.
         """
         try:
```

### Comparing `eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/rand.py` & `eventum_plugins-1.0.2/eventum_plugins/event/jinja_modules/rand.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/event/tests/test_jinja.py` & `eventum_plugins-1.0.2/eventum_plugins/event/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/base.py` & `eventum_plugins-1.0.2/eventum_plugins/input/base.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/cron.py` & `eventum_plugins-1.0.2/eventum_plugins/input/cron.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/linspace.py` & `eventum_plugins-1.0.2/eventum_plugins/input/linspace.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/sample.py` & `eventum_plugins-1.0.2/eventum_plugins/input/sample.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_cron.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_linspace.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_linspace.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_sample.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_time_patterns.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_time_patterns.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timer.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timestamps.py` & `eventum_plugins-1.0.2/eventum_plugins/input/tests/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/time_patterns.py` & `eventum_plugins-1.0.2/eventum_plugins/input/time_patterns.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/timer.py` & `eventum_plugins-1.0.2/eventum_plugins/input/timer.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/input/timestamps.py` & `eventum_plugins-1.0.2/eventum_plugins/input/timestamps.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/base.py` & `eventum_plugins-1.0.2/eventum_plugins/output/base.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/file.py` & `eventum_plugins-1.0.2/eventum_plugins/output/file.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/opensearch.py` & `eventum_plugins-1.0.2/eventum_plugins/output/opensearch.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/stdout.py` & `eventum_plugins-1.0.2/eventum_plugins/output/stdout.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/tests/test_file.py` & `eventum_plugins-1.0.2/eventum_plugins/output/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/output/tests/test_opensearch.py` & `eventum_plugins-1.0.2/eventum_plugins/output/tests/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/utils/relative_time.py` & `eventum_plugins-1.0.2/eventum_plugins/utils/relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_relative_time.py` & `eventum_plugins-1.0.2/eventum_plugins/utils/tests/test_relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_timeseries.py` & `eventum_plugins-1.0.2/eventum_plugins/utils/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/eventum_plugins/utils/timeseries.py` & `eventum_plugins-1.0.2/eventum_plugins/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.1/pyproject.toml` & `eventum_plugins-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-plugins"
-version = "1.0.1"
+version = "1.0.2"
 description = "Plugins for Eventum"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumPlugins"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["plugin", "generator", "template", "scheduling", "time"]
```

### Comparing `eventum_plugins-1.0.1/PKG-INFO` & `eventum_plugins-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-plugins
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plugins for Eventum
 Home-page: https://github.com/Eventum-Generatives/EventumPlugins
 License: Apache-2.0
 Keywords: plugin,generator,template,scheduling,time
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

