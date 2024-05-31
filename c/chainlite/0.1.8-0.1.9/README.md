# Comparing `tmp/chainlite-0.1.8.tar.gz` & `tmp/chainlite-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.8.tar", last modified: Sun May 26 00:33:12 2024, max compression
+gzip compressed data, was "chainlite-0.1.9.tar", last modified: Sun May 26 21:33:44 2024, max compression
```

## Comparing `chainlite-0.1.8.tar` & `chainlite-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 00:32:57.000000 chainlite-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 00:33:12.102709 chainlite-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-26 00:32:57.000000 chainlite-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.098709 chainlite-0.1.8/chainlite/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/llm_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/load_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/chainlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 00:32:57.000000 chainlite-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:33:12.102709 chainlite-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 00:32:57.000000 chainlite-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 00:32:57.000000 chainlite-0.1.8/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 00:32:57.000000 chainlite-0.1.8/tasks/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-26 00:32:57.000000 chainlite-0.1.8/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:33:44.339985 chainlite-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 21:33:40.000000 chainlite-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 21:33:44.339985 chainlite-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-26 21:33:40.000000 chainlite-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:33:44.335985 chainlite-0.1.9/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 21:33:40.000000 chainlite-0.1.9/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-26 21:33:40.000000 chainlite-0.1.9/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-26 21:33:40.000000 chainlite-0.1.9/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-26 21:33:40.000000 chainlite-0.1.9/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 21:33:40.000000 chainlite-0.1.9/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:33:44.339985 chainlite-0.1.9/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 21:33:44.000000 chainlite-0.1.9/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 21:33:44.000000 chainlite-0.1.9/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:33:44.000000 chainlite-0.1.9/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-26 21:33:44.000000 chainlite-0.1.9/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 21:33:44.000000 chainlite-0.1.9/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 21:33:40.000000 chainlite-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:33:44.339985 chainlite-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 21:33:40.000000 chainlite-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:33:44.339985 chainlite-0.1.9/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 21:33:40.000000 chainlite-0.1.9/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 21:33:40.000000 chainlite-0.1.9/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:33:44.339985 chainlite-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-26 21:33:40.000000 chainlite-0.1.9/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.8/LICENSE` & `chainlite-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.8/PKG-INFO` & `chainlite-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.8/README.md` & `chainlite-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.8/chainlite/llm_config.py` & `chainlite-0.1.9/chainlite/llm_config.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.8/chainlite/llm_generate.py` & `chainlite-0.1.9/chainlite/llm_generate.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.8/chainlite/load_prompt.py` & `chainlite-0.1.9/chainlite/load_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     """
     raw_template = jinja_environment.loader.get_source(
         jinja_environment, template_file
     )[0]
     raw_template = re.sub(jinja2_comment_pattern, "", raw_template)
     if not keep_indentation:
         raw_template = "\n".join([line.strip() for line in raw_template.split("\n")])
+    else:
+        raw_template = "\n".join([line.rstrip() for line in raw_template.split("\n")])
     raw_template = re.sub(
         r"%}\s*", "%}", raw_template
     )  # remove the white space after {% for ... %} tags etc.
 
     return raw_template
```

### Comparing `chainlite-0.1.8/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.9/chainlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.8/setup.py` & `chainlite-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.8",
+    version="0.1.9",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
```

### Comparing `chainlite-0.1.8/tasks/main.py` & `chainlite-0.1.9/tasks/main.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.8/tests/test_llm_generate.py` & `chainlite-0.1.9/tests/test_llm_generate.py`

 * *Files identical despite different names*

