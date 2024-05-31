# Comparing `tmp/fastapi_inertia-0.1.3.tar.gz` & `tmp/fastapi_inertia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_inertia-0.1.3.tar", max compression
+gzip compressed data, was "fastapi_inertia-0.1.4.tar", max compression
```

## Comparing `fastapi_inertia-0.1.3.tar` & `fastapi_inertia-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-04-21 18:04:08.142429 fastapi_inertia-0.1.3/LICENSE
--rw-r--r--   0        0        0    16710 2024-04-23 16:11:11.035698 fastapi_inertia-0.1.3/README.md
--rw-r--r--   0        0        0      556 2024-04-21 18:04:08.143798 fastapi_inertia-0.1.3/inertia/__init__.py
--rw-r--r--   0        0        0      704 2024-04-21 18:04:08.144132 fastapi_inertia-0.1.3/inertia/config.py
--rw-r--r--   0        0        0     2215 2024-04-21 18:04:08.144480 fastapi_inertia-0.1.3/inertia/exceptions.py
--rw-r--r--   0        0        0    12335 2024-04-23 15:17:26.663599 fastapi_inertia-0.1.3/inertia/inertia.py
--rw-r--r--   0        0        0        0 2024-04-23 15:27:17.449490 fastapi_inertia-0.1.3/inertia/py.typed
--rw-r--r--   0        0        0     1481 2024-04-23 15:17:26.663934 fastapi_inertia-0.1.3/inertia/utils.py
--rw-r--r--   0        0        0     1154 2024-05-08 15:09:54.434001 fastapi_inertia-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    17644 1970-01-01 00:00:00.000000 fastapi_inertia-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/LICENSE
+-rw-r--r--   0        0        0    16710 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/README.md
+-rw-r--r--   0        0        0      556 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/config.py
+-rw-r--r--   0        0        0     2215 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/exceptions.py
+-rw-r--r--   0        0        0    12502 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/inertia.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/py.typed
+-rw-r--r--   0        0        0     1481 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/inertia/utils.py
+-rw-r--r--   0        0        0     1406 2024-05-31 12:53:42.689848 fastapi_inertia-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    17644 1970-01-01 00:00:00.000000 fastapi_inertia-0.1.4/PKG-INFO
```

### Comparing `fastapi_inertia-0.1.3/LICENSE` & `fastapi_inertia-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/README.md` & `fastapi_inertia-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/inertia/__init__.py` & `fastapi_inertia-0.1.4/inertia/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/inertia/config.py` & `fastapi_inertia-0.1.4/inertia/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/inertia/exceptions.py` & `fastapi_inertia-0.1.4/inertia/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/inertia/inertia.py` & `fastapi_inertia-0.1.4/inertia/inertia.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         :param prop: Property to transform
         :return: Transformed property
         """
         if not isinstance(prop, dict):
             if callable(prop):
                 return prop()
             if isinstance(prop, BaseModel):
-                return prop.model_dump()
+                return json.loads(prop.model_dump_json())
             return prop
 
         prop_ = prop.copy()
         for key in list(prop_.keys()):
             prop_[key] = cls._deep_transform_callables(prop_[key])
 
         return prop_
@@ -249,14 +249,27 @@
         displayable_head = "\n".join(head)
         body = response_json["body"]
 
         html_content = self._get_html_content(displayable_head, body)
 
         return HTMLResponse(content=html_content, status_code=200)
 
+    def _render_json(self) -> JSONResponse:
+        """
+        Render the page using JSON
+        :return: The JSON response
+        """
+        return JSONResponse(
+            content=self._get_page_data(),
+            headers={
+                "Vary": "Accept",
+                "X-Inertia": "true",
+            },
+        )
+
     def share(self, **props: Any) -> None:
         """
         Share props between functions. Useful to share props between dependencies/middlewares and routes
         :param props: Props to share
         """
         self._props.update(props)
 
@@ -325,21 +338,15 @@
                 {self._config.flash_error_key: self._get_flashed_errors()}
             )
 
         self._component = component
         self._props.update(props or {})
 
         if "X-Inertia" in self._request.headers:
-            return JSONResponse(
-                content=self._get_page_data(),
-                headers={
-                    "Vary": "Accept",
-                    "X-Inertia": "true",
-                },
-            )
+            return self._render_json()
 
         if self._config.ssr_enabled:
             try:
                 return await self._render_ssr()
             except Exception as exc:
                 logger.error(
                     f"An error occurred in rendering SSR (falling back to classic rendering): {exc}"
```

### Comparing `fastapi_inertia-0.1.3/inertia/utils.py` & `fastapi_inertia-0.1.4/inertia/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.3/pyproject.toml` & `fastapi_inertia-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-inertia"
-version = "0.1.3"
+version = "0.1.4"
 description = "An implementation of the Inertia protocol for FastAPI."
 authors = ["Hugo Mortreux <70602545+hxjo@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hxjo/fastapi-inertia"
 homepage = "https://github.com/hxjo/fastapi-inertia"
 keywords = ["inertia", "inertiajs", "fastapi", "python"]
@@ -31,16 +31,26 @@
 ruff = "^0.4.1"
 pytest = "^8.1.1"
 httpx = "^0.27.0"
 pytest-cov = "^5.0.0"
 types-requests = "^2.31.0.20240406"
 itsdangerous = "^2.2.0"
 requests = "^2.31.0"
+poethepoet = "^0.26.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
 strict = true
 check_untyped_defs = true
+
+
+[tool.poe.tasks]
+test = "pytest inertia/tests --cov inertia --cov-report term-missing"
+type_check = "mypy inertia"
+format = "ruff format inertia"
+lint = "ruff check inertia --fix"
+
+pc = ["test", "type_check", "format", "lint"]
```

### Comparing `fastapi_inertia-0.1.3/PKG-INFO` & `fastapi_inertia-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-inertia
-Version: 0.1.3
+Version: 0.1.4
 Summary: An implementation of the Inertia protocol for FastAPI.
 Home-page: https://github.com/hxjo/fastapi-inertia
 License: MIT
 Keywords: inertia,inertiajs,fastapi,python
 Author: Hugo Mortreux
 Author-email: 70602545+hxjo@users.noreply.github.com
 Requires-Python: >=3.9
```

