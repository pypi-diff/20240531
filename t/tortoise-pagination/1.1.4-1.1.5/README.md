# Comparing `tmp/tortoise_pagination-1.1.4.tar.gz` & `tmp/tortoise_pagination-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_pagination-1.1.4.tar", max compression
+gzip compressed data, was "tortoise_pagination-1.1.5.tar", max compression
```

## Comparing `tortoise_pagination-1.1.4.tar` & `tortoise_pagination-1.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      750 2023-06-01 17:28:02.913992 tortoise_pagination-1.1.4/README.md
--rw-r--r--   0        0        0      610 2024-01-29 11:15:27.874863 tortoise_pagination-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       55 2023-06-01 17:17:33.284615 tortoise_pagination-1.1.4/tortoise_pagination/__init__.py
--rw-r--r--   0        0        0     1791 2023-12-09 16:25:43.785013 tortoise_pagination-1.1.4/tortoise_pagination/pagination.py
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 tortoise_pagination-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-06-01 17:28:02.913992 tortoise_pagination-1.1.5/README.md
+-rw-r--r--   0        0        0      610 2024-05-31 16:19:54.563368 tortoise_pagination-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-06-01 17:17:33.284615 tortoise_pagination-1.1.5/tortoise_pagination/__init__.py
+-rw-r--r--   0        0        0     1791 2023-12-09 16:25:43.785013 tortoise_pagination-1.1.5/tortoise_pagination/pagination.py
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 tortoise_pagination-1.1.5/PKG-INFO
```

### Comparing `tortoise_pagination-1.1.4/README.md` & `tortoise_pagination-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tortoise_pagination-1.1.4/pyproject.toml` & `tortoise_pagination-1.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "tortoise-pagination"
-version = "1.1.4"
+version = "1.1.5"
 description = "Pagination for Tortoise-ORM on FastAPI"
 authors = ["Sebastien Nicolet <snicolet95@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tortoise_pagination"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-tortoise-orm = "^0.20.0"
+tortoise-orm = "^0.21.0"
 fastapi = ">=0.104.1"
 pydantic = ">2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.270"
 flake8 = "^6.0.0"
```

### Comparing `tortoise_pagination-1.1.4/tortoise_pagination/pagination.py` & `tortoise_pagination-1.1.5/tortoise_pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `tortoise_pagination-1.1.4/PKG-INFO` & `tortoise_pagination-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tortoise-pagination
-Version: 1.1.4
+Version: 1.1.5
 Summary: Pagination for Tortoise-ORM on FastAPI
 License: MIT
 Author: Sebastien Nicolet
 Author-email: snicolet95@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.104.1)
 Requires-Dist: pydantic (>2.0.0)
-Requires-Dist: tortoise-orm (>=0.20.0,<0.21.0)
+Requires-Dist: tortoise-orm (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Usage
 Supposing in `myapp.schema` you have a pydantic `BaseModel` to represent your model
 
 ```python
 from fastapi import Depends
```

