# Comparing `tmp/django_pictures-1.3.0.tar.gz` & `tmp/django_pictures-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pictures-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pictures-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pictures-1.3.0.tar` & `django_pictures-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2024-05-25 10:16:19.145867 django_pictures-1.3.0/LICENSE
--rw-r--r--   0        0        0    10067 2024-05-25 10:16:19.145867 django_pictures-1.3.0/README.md
--rw-r--r--   0        0        0      171 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/__init__.py
--rw-r--r--   0        0        0      411 2024-05-25 10:16:32.377768 django_pictures-1.3.0/pictures/_version.py
--rw-r--r--   0        0        0      155 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/apps.py
--rw-r--r--   0        0        0     1012 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/checks.py
--rw-r--r--   0        0        0      683 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/conf.py
--rw-r--r--   0        0        0        0 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/contrib/__init__.py
--rw-r--r--   0        0        0     2912 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2024-05-25 10:16:30.101783 django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3167 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/migrations.py
--rw-r--r--   0        0        0    10158 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/models.py
--rw-r--r--   0        0        0     3863 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/tasks.py
--rw-r--r--   0        0        0      165 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      618 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     2281 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/urls.py
--rw-r--r--   0        0        0     4752 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/utils.py
--rw-r--r--   0        0        0     1907 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/validators.py
--rw-r--r--   0        0        0      741 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/views.py
--rw-r--r--   0        0        0     2540 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    12583 1970-01-01 00:00:00.000000 django_pictures-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1324 2024-05-31 08:11:38.141685 django_pictures-1.3.1/LICENSE
+-rw-r--r--   0        0        0    10067 2024-05-31 08:11:38.141685 django_pictures-1.3.1/README.md
+-rw-r--r--   0        0        0      171 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-31 08:12:22.861371 django_pictures-1.3.1/pictures/_version.py
+-rw-r--r--   0        0        0      155 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/checks.py
+-rw-r--r--   0        0        0      683 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/conf.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2869 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2024-05-31 08:12:19.425399 django_pictures-1.3.1/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3167 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/migrations.py
+-rw-r--r--   0        0        0    10158 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/models.py
+-rw-r--r--   0        0        0     3863 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      618 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2281 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/urls.py
+-rw-r--r--   0        0        0     4752 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/validators.py
+-rw-r--r--   0        0        0      741 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pictures/views.py
+-rw-r--r--   0        0        0     2540 2024-05-31 08:11:38.141685 django_pictures-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12583 1970-01-01 00:00:00.000000 django_pictures-1.3.1/PKG-INFO
```

### Comparing `django_pictures-1.3.0/LICENSE` & `django_pictures-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/README.md` & `django_pictures-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/checks.py` & `django_pictures-1.3.1/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/conf.py` & `django_pictures-1.3.1/pictures/conf.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/contrib/rest_framework.py` & `django_pictures-1.3.1/pictures/contrib/rest_framework.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,54 +30,52 @@
 
         base_payload = {
             "url": obj.url,
             "width": obj.width,
             "height": obj.height,
         }
 
-        payload = {
-            **base_payload,
-            "ratios": {
-                ratio: {
-                    "sources": {
-                        f"image/{file_type.lower()}": sizes
-                        for file_type, sizes in sources.items()
-                        if file_type in self.file_types or not self.file_types
-                    },
-                }
-                for ratio, sources in obj.aspect_ratios.items()
-                if ratio in self.aspect_ratios or not self.aspect_ratios
-            },
-        }
-
         # if the request has query parameters, filter the payload
         try:
             query_params: QueryDict = self.context["request"].GET
         except KeyError:
-            pass
+            ratios = self.aspect_ratios
+            container = get_settings().CONTAINER_WIDTH
+            breakpoints = {}
         else:
-            ratio = query_params.get(f"{self.field_name}_ratio")
+            ratios = (
+                query_params.getlist(f"{self.field_name}_ratio")
+            ) or self.aspect_ratios
             container = query_params.get(f"{self.field_name}_container")
             try:
                 container = int(container)
             except TypeError:
                 container = get_settings().CONTAINER_WIDTH
             except ValueError as e:
                 raise ValueError(f"Container width is not a number: {container}") from e
             breakpoints = {
                 bp: int(query_params.get(f"{self.field_name}_{bp}"))
                 for bp in get_settings().BREAKPOINTS
                 if f"{self.field_name}_{bp}" in query_params
             }
-            if ratio is not None:
-                try:
-                    payload["ratios"] = {ratio: payload["ratios"][ratio]}
-                except KeyError as e:
-                    raise ValueError(
-                        f"Invalid ratio: {ratio}. Choices are: {', '.join(filter(None, obj.aspect_ratios.keys()))}"
-                    ) from e
-                else:
-                    payload["ratios"][ratio]["media"] = utils.sizes(
-                        container_width=container, **breakpoints
-                    )
+            if set(ratios) - set(self.aspect_ratios or obj.aspect_ratios.keys()):
+                raise ValueError(
+                    f"Invalid ratios: {', '.join(ratios)}. Choices are: {', '.join(filter(None, obj.aspect_ratios.keys()))}"
+                )
+
+        payload = {
+            **base_payload,
+            "ratios": {
+                ratio: {
+                    "sources": {
+                        f"image/{file_type.lower()}": sizes
+                        for file_type, sizes in sources.items()
+                        if file_type in self.file_types or not self.file_types
+                    },
+                    "media": utils.sizes(container_width=container, **breakpoints),
+                }
+                for ratio, sources in obj.aspect_ratios.items()
+                if ratio in ratios or not ratios
+            },
+        }
 
         return json.loads(json.dumps(payload, default=default))
```

### Comparing `django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.mo` & `django_pictures-1.3.1/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.po` & `django_pictures-1.3.1/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/migrations.py` & `django_pictures-1.3.1/pictures/migrations.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/models.py` & `django_pictures-1.3.1/pictures/models.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/tasks.py` & `django_pictures-1.3.1/pictures/tasks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/templates/pictures/picture.html` & `django_pictures-1.3.1/pictures/templates/pictures/picture.html`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/templatetags/pictures.py` & `django_pictures-1.3.1/pictures/templatetags/pictures.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/utils.py` & `django_pictures-1.3.1/pictures/utils.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/validators.py` & `django_pictures-1.3.1/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pictures/views.py` & `django_pictures-1.3.1/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/pyproject.toml` & `django_pictures-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pictures-1.3.0/PKG-INFO` & `django_pictures-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.3.0
+Version: 1.3.1
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

