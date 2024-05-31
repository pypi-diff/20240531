# Comparing `tmp/reaction-local-0.0.8.tar.gz` & `tmp/reaction-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaction-local-0.0.8.tar", last modified: Wed Sep 20 12:11:56 2023, max compression
+gzip compressed data, was "reaction-local-0.0.9.tar", last modified: Wed Dec  6 20:17:49 2023, max compression
```

## Comparing `reaction-local-0.0.8.tar` & `reaction-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 12:11:56.634345 reaction-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-20 12:11:56.634345 reaction-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-09-20 12:10:48.000000 reaction-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-09-20 12:10:48.000000 reaction-local-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 12:11:56.634345 reaction-local-0.0.8/reaction_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 12:10:48.000000 reaction-local-0.0.8/reaction_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 12:11:56.634345 reaction-local-0.0.8/reaction_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 12:10:48.000000 reaction-local-0.0.8/reaction_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2023-09-20 12:10:48.000000 reaction-local-0.0.8/reaction_local/src/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 12:11:56.634345 reaction-local-0.0.8/reaction_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-20 12:11:56.000000 reaction-local-0.0.8/reaction_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-20 12:11:56.000000 reaction-local-0.0.8/reaction_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 12:11:56.000000 reaction-local-0.0.8/reaction_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-20 12:11:56.000000 reaction-local-0.0.8/reaction_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 12:11:56.634345 reaction-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-09-20 12:10:48.000000 reaction-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:49.880744 reaction-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-06 20:17:49.880744 reaction-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-12-06 20:17:15.000000 reaction-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-06 20:17:15.000000 reaction-local-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:49.880744 reaction-local-0.0.9/reaction_local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:15.000000 reaction-local-0.0.9/reaction_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:49.880744 reaction-local-0.0.9/reaction_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:15.000000 reaction-local-0.0.9/reaction_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2023-12-06 20:17:15.000000 reaction-local-0.0.9/reaction_local/src/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:17:49.880744 reaction-local-0.0.9/reaction_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-06 20:17:49.000000 reaction-local-0.0.9/reaction_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-06 20:17:49.000000 reaction-local-0.0.9/reaction_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 20:17:49.000000 reaction-local-0.0.9/reaction_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-06 20:17:49.000000 reaction-local-0.0.9/reaction_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 20:17:49.880744 reaction-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-12-06 20:17:15.000000 reaction-local-0.0.9/setup.py
```

### Comparing `reaction-local-0.0.8/PKG-INFO` & `reaction-local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaction-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles reaction-local-python-package Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `reaction-local-0.0.8/README.md` & `reaction-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `reaction-local-0.0.8/pyproject.toml` & `reaction-local-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "reaction-local"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.8" # https://pypi.org/project/reaction-locali.e. https://pypi.org/project/storage-local/
+version = "0.0.9" # https://pypi.org/project/reaction-locali.e. https://pypi.org/project/storage-local/
 description = "reaction-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `reaction-local-0.0.8/reaction_local/src/reaction.py` & `reaction-local-0.0.9/reaction_local/src/reaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         INIT_METHOD_NAME = "__init__"
         logger.start(INIT_METHOD_NAME)
         self.connector = Connector.connect("reaction")
         self.cursor = self.connector.cursor()
         logger.end(INIT_METHOD_NAME)
 
     def insert(self, reaction_data: Dict[str, any], profile_id: int, lang_code: str) -> int:
+        if not isinstance(lang_code, str):
+            lang_code = lang_code.value
         INSERT_REACTION_METHOD_NAME = "insert_reaction"
         logger.start(INSERT_REACTION_METHOD_NAME, object={'reaction_data': reaction_data, 'profile_id': profile_id, 'lang_code': lang_code})
 
         title : str = str(reaction_data["title"])
         query_get = "SELECT reaction_type_id FROM reaction.reaction_type_ml_table WHERE title = %s"
         self.cursor.execute(query_get, (title,))
         rows = self.cursor.fetchall()
```

### Comparing `reaction-local-0.0.8/reaction_local.egg-info/PKG-INFO` & `reaction-local-0.0.9/reaction_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaction-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles reaction-local-python-package Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `reaction-local-0.0.8/setup.py` & `reaction-local-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 # Each Python project should have pyproject.toml or setup.py
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 # The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
      name='reaction-local',  
-     version='0.0.8', # https://pypi.org/project/reaction-local/
+     version='0.0.9', # https://pypi.org/project/reaction-local/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles reaction-local-python-package Local Python", 
      long_description="This is a package for sharing common functions of operational hours CRUD to reaction database used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

