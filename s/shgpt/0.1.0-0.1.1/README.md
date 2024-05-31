# Comparing `tmp/shgpt-0.1.0.tar.gz` & `tmp/shgpt-0.1.1.tar.gz`

## Comparing `shgpt-0.1.0.tar` & `shgpt-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 shgpt-0.1.0/Makefile
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 shgpt-0.1.0/README.md
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/main.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/version.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/api/ollama.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/tui/app.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/tui/app.tcss
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/utils/common.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/utils/conf.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.1.0/shgpt/utils/http.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 shgpt-0.1.0/.gitignore
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 shgpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 shgpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 shgpt-0.1.1/Makefile
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/main.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/version.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/api/ollama.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/tui/app.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/tui/app.tcss
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/utils/common.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/utils/conf.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.1.1/shgpt/utils/http.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.1.1/.gitignore
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 shgpt-0.1.1/README.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 shgpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 shgpt-0.1.1/PKG-INFO
```

### Comparing `shgpt-0.1.0/shgpt/main.py` & `shgpt-0.1.1/shgpt/main.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.1.0/shgpt/api/ollama.py` & `shgpt-0.1.1/shgpt/api/ollama.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.1.0/shgpt/tui/app.py` & `shgpt-0.1.1/shgpt/tui/app.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.1.0/shgpt/utils/common.py` & `shgpt-0.1.1/shgpt/utils/common.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.1.0/pyproject.toml` & `shgpt-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "shgpt"
 dynamic = ["version"]
 authors = [{name = "Jiacai Liu", email="dev@liujiacai.net"}]
 description = "Generate shell command you want with power of LLM, without leaving your terminal."
+readme = "README.md"
 keywords = ["llm", "shell", "gpt"]
 license = "GPL-3.0"
 dependencies = [
   "requests",
   "smartinput",
   "pyperclip",
   "textual",
@@ -18,14 +19,15 @@
 
 [project.urls]
 Repository = "https://github.com/jiacai2050/shellgpt"
 Issues = "https://github.com/jiacai2050/shellgpt/issues"
 
 [project.scripts]
 sg = "shgpt.main:main"
+shgpt = "shgpt.main:main"
 
 [tool.hatch.version]
 path = "shgpt/version.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
   "shgpt",
```

