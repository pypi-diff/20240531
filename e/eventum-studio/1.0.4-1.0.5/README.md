# Comparing `tmp/eventum_studio-1.0.4.tar.gz` & `tmp/eventum_studio-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_studio-1.0.4.tar", max compression
+gzip compressed data, was "eventum_studio-1.0.5.tar", max compression
```

## Comparing `eventum_studio-1.0.4.tar` & `eventum_studio-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-05-29 18:59:07.580389 eventum_studio-1.0.4/LICENSE
--rw-r--r--   0        0        0       46 2024-05-29 19:01:21.540375 eventum_studio-1.0.4/README.md
--rw-r--r--   0        0        0     1350 2024-05-29 21:38:29.198163 eventum_studio-1.0.4/eventum_studio/01_Time_distribution.py
--rw-r--r--   0        0        0        0 2024-05-29 19:00:23.640392 eventum_studio-1.0.4/eventum_studio/__init__.py
--rw-r--r--   0        0        0      590 2024-05-30 10:37:07.626052 eventum_studio-1.0.4/eventum_studio/__main__.py
--rw-r--r--   0        0        0     3174 2024-05-29 19:13:53.120193 eventum_studio-1.0.4/eventum_studio/components/component.py
--rw-r--r--   0        0        0     1530 2024-05-29 20:34:03.679067 eventum_studio-1.0.4/eventum_studio/components/sample_explorer.py
--rw-r--r--   0        0        0     1855 2024-05-29 20:16:13.529325 eventum_studio-1.0.4/eventum_studio/components/span_input.py
--rw-r--r--   0        0        0     2473 2024-05-29 20:36:59.119021 eventum_studio-1.0.4/eventum_studio/components/template_configuration_editor.py
--rw-r--r--   0        0        0     1601 2024-05-29 21:38:29.208163 eventum_studio-1.0.4/eventum_studio/components/template_editor.py
--rw-r--r--   0        0        0     5885 2024-05-29 20:37:43.669011 eventum_studio-1.0.4/eventum_studio/components/template_manager.py
--rw-r--r--   0        0        0     7205 2024-05-29 20:38:45.599000 eventum_studio-1.0.4/eventum_studio/components/template_renderer.py
--rw-r--r--   0        0        0     1547 2024-05-29 20:39:47.188987 eventum_studio-1.0.4/eventum_studio/components/template_state_viewer.py
--rw-r--r--   0        0        0    15180 2024-05-29 21:13:36.178516 eventum_studio-1.0.4/eventum_studio/components/time_pattern_configurator.py
--rw-r--r--   0        0        0     8672 2024-05-29 20:40:01.868985 eventum_studio-1.0.4/eventum_studio/components/time_pattern_configurator_list.py
--rw-r--r--   0        0        0     5231 2024-05-29 20:46:35.288886 eventum_studio-1.0.4/eventum_studio/components/time_pattern_distribution_histogram.py
--rw-r--r--   0        0        0      973 2024-05-29 19:00:23.650392 eventum_studio-1.0.4/eventum_studio/notifiers.py
--rw-r--r--   0        0        0     2455 2024-05-29 21:38:29.228163 eventum_studio-1.0.4/eventum_studio/pages/02_Event_template.py
--rw-r--r--   0        0        0        0 2024-05-29 19:05:13.340315 eventum_studio-1.0.4/eventum_studio/py.typed
--rw-r--r--   0        0        0    15406 2024-05-29 21:37:07.818185 eventum_studio-1.0.4/eventum_studio/static/favicon.ico
--rw-r--r--   0        0        0      285 2024-05-29 19:09:11.880258 eventum_studio-1.0.4/eventum_studio/theme.py
--rw-r--r--   0        0        0        0 2024-05-29 20:13:32.839354 eventum_studio-1.0.4/eventum_studio/utils/__init__.py
--rw-r--r--   0        0        0     1750 2024-05-29 20:44:15.698923 eventum_studio-1.0.4/eventum_studio/utils/relative_time.py
--rw-r--r--   0        0        0     1957 2024-05-29 20:15:17.739341 eventum_studio-1.0.4/eventum_studio/utils/tests/test_relative_time.py
--rw-r--r--   0        0        0      747 2024-05-29 19:35:37.879890 eventum_studio-1.0.4/eventum_studio/utils/validation_prettier.py
--rw-r--r--   0        0        0     2094 2024-05-29 19:00:23.660392 eventum_studio-1.0.4/eventum_studio/widget_management.py
--rw-r--r--   0        0        0     1360 2024-05-30 10:35:06.376080 eventum_studio-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 eventum_studio-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 18:59:07.580389 eventum_studio-1.0.5/LICENSE
+-rw-r--r--   0        0        0       46 2024-05-29 19:01:21.540375 eventum_studio-1.0.5/README.md
+-rw-r--r--   0        0        0     1350 2024-05-29 21:38:29.198163 eventum_studio-1.0.5/eventum_studio/01_Time_distribution.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:00:23.640392 eventum_studio-1.0.5/eventum_studio/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-31 19:22:13.317990 eventum_studio-1.0.5/eventum_studio/__main__.py
+-rw-r--r--   0        0        0     3174 2024-05-29 19:13:53.120193 eventum_studio-1.0.5/eventum_studio/components/component.py
+-rw-r--r--   0        0        0     1530 2024-05-29 20:34:03.679067 eventum_studio-1.0.5/eventum_studio/components/sample_explorer.py
+-rw-r--r--   0        0        0     1855 2024-05-29 20:16:13.529325 eventum_studio-1.0.5/eventum_studio/components/span_input.py
+-rw-r--r--   0        0        0     1990 2024-05-31 19:01:30.477052 eventum_studio-1.0.5/eventum_studio/components/template_configuration_editor.py
+-rw-r--r--   0        0        0     1601 2024-05-30 11:18:47.615457 eventum_studio-1.0.5/eventum_studio/components/template_editor.py
+-rw-r--r--   0        0        0     5885 2024-05-29 20:37:43.669011 eventum_studio-1.0.5/eventum_studio/components/template_manager.py
+-rw-r--r--   0        0        0     7205 2024-05-29 20:38:45.599000 eventum_studio-1.0.5/eventum_studio/components/template_renderer.py
+-rw-r--r--   0        0        0     1547 2024-05-29 20:39:47.188987 eventum_studio-1.0.5/eventum_studio/components/template_state_viewer.py
+-rw-r--r--   0        0        0    15180 2024-05-29 21:13:36.178516 eventum_studio-1.0.5/eventum_studio/components/time_pattern_configurator.py
+-rw-r--r--   0        0        0     8672 2024-05-29 20:40:01.868985 eventum_studio-1.0.5/eventum_studio/components/time_pattern_configurator_list.py
+-rw-r--r--   0        0        0     5231 2024-05-29 20:46:35.288886 eventum_studio-1.0.5/eventum_studio/components/time_pattern_distribution_histogram.py
+-rw-r--r--   0        0        0      973 2024-05-29 19:00:23.650392 eventum_studio-1.0.5/eventum_studio/notifiers.py
+-rw-r--r--   0        0        0     2694 2024-05-31 19:01:22.237054 eventum_studio-1.0.5/eventum_studio/pages/02_Event_template.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:05:13.340315 eventum_studio-1.0.5/eventum_studio/py.typed
+-rw-r--r--   0        0        0    15406 2024-05-29 21:37:07.818185 eventum_studio-1.0.5/eventum_studio/static/favicon.ico
+-rw-r--r--   0        0        0      285 2024-05-29 19:09:11.880258 eventum_studio-1.0.5/eventum_studio/theme.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:13:32.839354 eventum_studio-1.0.5/eventum_studio/utils/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-29 20:44:15.698923 eventum_studio-1.0.5/eventum_studio/utils/relative_time.py
+-rw-r--r--   0        0        0     1957 2024-05-29 20:15:17.739341 eventum_studio-1.0.5/eventum_studio/utils/tests/test_relative_time.py
+-rw-r--r--   0        0        0      747 2024-05-29 19:35:37.879890 eventum_studio-1.0.5/eventum_studio/utils/validation_prettier.py
+-rw-r--r--   0        0        0     2094 2024-05-29 19:00:23.660392 eventum_studio-1.0.5/eventum_studio/widget_management.py
+-rw-r--r--   0        0        0     1360 2024-05-31 19:32:30.877862 eventum_studio-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 eventum_studio-1.0.5/PKG-INFO
```

### Comparing `eventum_studio-1.0.4/LICENSE` & `eventum_studio-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/01_Time_distribution.py` & `eventum_studio-1.0.5/eventum_studio/01_Time_distribution.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/__main__.py` & `eventum_studio-1.0.5/eventum_studio/__main__.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/component.py` & `eventum_studio-1.0.5/eventum_studio/components/component.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/sample_explorer.py` & `eventum_studio-1.0.5/eventum_studio/components/sample_explorer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/span_input.py` & `eventum_studio-1.0.5/eventum_studio/components/span_input.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/template_configuration_editor.py` & `eventum_studio-1.0.5/eventum_studio/components/template_configuration_editor.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,30 +9,18 @@
 from eventum_studio.notifiers import NotificationLevel, default_notifier
 
 
 class TemplateConfigurationEditor(BaseComponent):
     """Component for editing configuration for template."""
 
     _SHOW_PROPS = {
+        'content': str,
         'on_change': Callable[[str], None]
     }
 
-    _DEFAULT_CONTENT = (
-        'params: { }\n'
-        'samples: { }\n'
-    )
-
-    def _init_state(self) -> None:
-        self._session_state['content'] = self._DEFAULT_CONTENT
-
-    def _handle_on_change(self, value: str) -> None:
-        """Handle changes committing."""
-        self._session_state['content'] = value
-        self._props['on_change'](value)
-
     def _show(self) -> None:
         col1, col2 = st.columns([1, 1])
 
         with col1:
             st.caption(
                 'Configuration',
                 help=(
@@ -55,25 +43,20 @@
                     overrideDefault=True
                 )
 
                 editor.Monaco(
                     theme='vs-dark',
                     language='yaml',
                     height=670,
-                    value=self._DEFAULT_CONTENT,
-                    onChange=lazy(self._handle_on_change),
+                    value=self._props['content'],
+                    onChange=lazy(self._props['on_change']),
                     options={
                         'cursorSmoothCaretAnimation': True,
                         'tabSize': 2
                     }
                 )
 
         with col2:
             SampleExplorer(
                 widget_keys_context=self._wk,
                 props={'display_size': 15}
             ).show()
-
-    @property
-    def content(self) -> str:
-        """Get currently committed content in editor."""
-        return self._session_state['content']
```

### Comparing `eventum_studio-1.0.4/eventum_studio/components/template_editor.py` & `eventum_studio-1.0.5/eventum_studio/components/template_editor.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/template_manager.py` & `eventum_studio-1.0.5/eventum_studio/components/template_manager.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/template_renderer.py` & `eventum_studio-1.0.5/eventum_studio/components/template_renderer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/template_state_viewer.py` & `eventum_studio-1.0.5/eventum_studio/components/template_state_viewer.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/time_pattern_configurator.py` & `eventum_studio-1.0.5/eventum_studio/components/time_pattern_configurator.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/time_pattern_configurator_list.py` & `eventum_studio-1.0.5/eventum_studio/components/time_pattern_configurator_list.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/components/time_pattern_distribution_histogram.py` & `eventum_studio-1.0.5/eventum_studio/components/time_pattern_distribution_histogram.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/notifiers.py` & `eventum_studio-1.0.5/eventum_studio/notifiers.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/pages/02_Event_template.py` & `eventum_studio-1.0.5/eventum_studio/pages/02_Event_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,21 @@
     layout='wide',
     initial_sidebar_state='expanded'
 )
 apply_theme()
 
 for key in ['template_content', 'config_content']:
     if key not in st.session_state:
-        st.session_state[key] = ''
+        if key == 'config_content':
+            st.session_state[key] = (
+                'params: { }\n'
+                'samples: { }\n'
+            )
+        else:
+            st.session_state[key] = ''
 
 manager = TemplateManager(
     props={
         'get_content_callback': lambda: st.session_state['template_content'],
         'set_content_callback': (
             lambda content:
             st.session_state.__setitem__('template_content', content)
@@ -44,24 +50,25 @@
             lambda value:
             st.session_state.__setitem__('template_content', value)
         )
     }
 )
 config_editor = TemplateConfigurationEditor(
     props={
+        'content': st.session_state['config_content'],
         'on_change': (
             lambda value:
             st.session_state.__setitem__('config_content', value)
         )
     }
 )
 renderer = TemplateRenderer(
     props={
         'template_content': st.session_state['template_content'],
-        'configuration_content': config_editor.content
+        'configuration_content': st.session_state['config_content']
     }
 )
 state_viewer = TemplateStateViewer(
     props={
         'local_vars': renderer.local_vars_state,
         'shared_vars': renderer.shared_vars_state,
         'subprocess_commands_history': renderer.subprocess_commands_history,
```

### Comparing `eventum_studio-1.0.4/eventum_studio/static/favicon.ico` & `eventum_studio-1.0.5/eventum_studio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/utils/relative_time.py` & `eventum_studio-1.0.5/eventum_studio/utils/relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/utils/tests/test_relative_time.py` & `eventum_studio-1.0.5/eventum_studio/utils/tests/test_relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/utils/validation_prettier.py` & `eventum_studio-1.0.5/eventum_studio/utils/validation_prettier.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/eventum_studio/widget_management.py` & `eventum_studio-1.0.5/eventum_studio/widget_management.py`

 * *Files identical despite different names*

### Comparing `eventum_studio-1.0.4/pyproject.toml` & `eventum_studio-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-studio"
-version = "1.0.4"
+version = "1.0.5"
 description = "Content designer for Eventum "
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumStudio"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["content", "IDE", "template", "visualization"]
```

### Comparing `eventum_studio-1.0.4/PKG-INFO` & `eventum_studio-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-studio
-Version: 1.0.4
+Version: 1.0.5
 Summary: Content designer for Eventum 
 Home-page: https://github.com/Eventum-Generatives/EventumStudio
 License: Apache-2.0
 Keywords: content,IDE,template,visualization
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

