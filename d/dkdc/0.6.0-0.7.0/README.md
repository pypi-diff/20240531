# Comparing `tmp/dkdc-0.6.0.tar.gz` & `tmp/dkdc-0.7.0.tar.gz`

## Comparing `dkdc-0.6.0.tar` & `dkdc-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dkdc-0.6.0/dev-requirements.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dkdc-0.6.0/justfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.6.0/untitled.ipynb
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/__init__.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/defaults.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/models.py
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/openai.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/systems.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/tokenize.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/__init__.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/ai.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/config.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/console.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/image.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/open.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/tokenize.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/config.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/filesystem.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/vars.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dkdc-0.6.0/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.6.0/LICENSE
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dkdc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dkdc-0.6.0/readme.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dkdc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dkdc-0.7.0/dev-requirements.txt
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 dkdc-0.7.0/justfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.7.0/untitled.ipynb
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/defaults.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/ai/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/ai/models.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/ai/openai.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/ai/systems.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/ai/tokenize.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/__init__.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/ai.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/config.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/console.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/image.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/open.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/cli/tokenize.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/utils/config.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/utils/database.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/utils/filesystem.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dkdc-0.7.0/src/dkdc/utils/vars.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dkdc-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.7.0/LICENSE
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dkdc-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dkdc-0.7.0/readme.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dkdc-0.7.0/PKG-INFO
```

### Comparing `dkdc-0.6.0/justfile` & `dkdc-0.7.0/justfile`

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,7 @@
 # smoke-test
 smoke-test:
     ruff format --check .
 
 # clean
 clean:
     @rm -r dist || True
-
```

### Comparing `dkdc-0.6.0/src/dkdc/ai/openai.py` & `dkdc-0.7.0/src/dkdc/ai/openai.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/src/dkdc/ai/systems.py` & `dkdc-0.7.0/src/dkdc/ai/systems.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/src/dkdc/cli/__init__.py` & `dkdc-0.7.0/src/dkdc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/src/dkdc/cli/console.py` & `dkdc-0.7.0/src/dkdc/cli/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     "user": "bold cyan",
     "dkdc.ai": "bold violet",
 }
 
 
 # functions
 def print(
-    text: str, as_markdown: bool = True, with_panel: bool = True, header: str = "dkdc"
+    text: str, as_markdown: bool = True, as_panel: bool = True, header: str = "dkdc"
 ) -> None:
     """
     print text
     """
     if as_markdown:
         text = Markdown(text)
 
-    if with_panel:
+    if as_panel:
         text = Panel(text, title=header, border_style=style_map[header])
 
     console.print(text)
```

### Comparing `dkdc-0.6.0/src/dkdc/cli/image.py` & `dkdc-0.7.0/src/dkdc/cli/image.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/src/dkdc/cli/open.py` & `dkdc-0.7.0/src/dkdc/cli/open.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/src/dkdc/utils/filesystem.py` & `dkdc-0.7.0/src/dkdc/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/LICENSE` & `dkdc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dkdc-0.6.0/pyproject.toml` & `dkdc-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dkdc"
-version = "0.6.0"
+version = "0.7.0"
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
 description = "dkdc"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `dkdc-0.6.0/PKG-INFO` & `dkdc-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dkdc
-Version: 0.6.0
+Version: 0.7.0
 Summary: dkdc
 Project-URL: Homepage, https://github.com/lostmygithubaccount/dkdc
 Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/dkdc/issues
 Author-email: Cody <cody@dkdc.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

