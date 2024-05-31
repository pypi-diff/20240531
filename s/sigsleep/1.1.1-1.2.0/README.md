# Comparing `tmp/sigsleep-1.1.1.tar.gz` & `tmp/sigsleep-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigsleep-1.1.1.tar", last modified: Wed Jan 17 18:36:43 2024, max compression
+gzip compressed data, was "sigsleep-1.2.0.tar", last modified: Fri May 31 01:09:42 2024, max compression
```

## Comparing `sigsleep-1.1.1.tar` & `sigsleep-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:36:43.139387 sigsleep-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-17 18:36:32.000000 sigsleep-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-17 18:36:43.139387 sigsleep-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-17 18:36:32.000000 sigsleep-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-17 18:36:32.000000 sigsleep-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 18:36:43.139387 sigsleep-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:36:43.139387 sigsleep-1.1.1/sigsleep/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-17 18:36:32.000000 sigsleep-1.1.1/sigsleep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-17 18:36:32.000000 sigsleep-1.1.1/sigsleep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-17 18:36:32.000000 sigsleep-1.1.1/sigsleep/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-17 18:36:32.000000 sigsleep-1.1.1/sigsleep/sigsleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:36:43.139387 sigsleep-1.1.1/sigsleep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-17 18:36:43.000000 sigsleep-1.1.1/sigsleep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-17 18:36:43.000000 sigsleep-1.1.1/sigsleep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 18:36:43.000000 sigsleep-1.1.1/sigsleep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-17 18:36:43.000000 sigsleep-1.1.1/sigsleep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-17 18:36:43.000000 sigsleep-1.1.1/sigsleep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:09:42.497053 sigsleep-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 01:09:35.000000 sigsleep-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 01:09:42.497053 sigsleep-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 01:09:35.000000 sigsleep-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 01:09:35.000000 sigsleep-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:09:42.497053 sigsleep-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:09:42.493053 sigsleep-1.2.0/sigsleep/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 01:09:35.000000 sigsleep-1.2.0/sigsleep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 01:09:35.000000 sigsleep-1.2.0/sigsleep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 01:09:35.000000 sigsleep-1.2.0/sigsleep/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-31 01:09:35.000000 sigsleep-1.2.0/sigsleep/sigsleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:09:42.497053 sigsleep-1.2.0/sigsleep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 01:09:42.000000 sigsleep-1.2.0/sigsleep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 01:09:42.000000 sigsleep-1.2.0/sigsleep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:09:42.000000 sigsleep-1.2.0/sigsleep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 01:09:42.000000 sigsleep-1.2.0/sigsleep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 01:09:42.000000 sigsleep-1.2.0/sigsleep.egg-info/top_level.txt
```

### Comparing `sigsleep-1.1.1/LICENSE` & `sigsleep-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigsleep-1.1.1/pyproject.toml` & `sigsleep-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     "Programming Language :: Python :: 3.8",
 ]
 license = {text = "GPL"}
 description = "Sleep that prints info upon receiving a specified signal"
 urls = {Homepage = "https://github.com/zwimer/sigsleep"}
 requires-python = ">= 3.8"
 dynamic = ["version"]
-dependencies = [
-]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
 sigsleep = "sigsleep:cli"
@@ -36,14 +34,18 @@
 [tool.setuptools.dynamic]
 version = {attr = "sigsleep._version.__version__"}
 
 # Tools
 
 [tool.black]
 line-length = 120
-target-version = ["py310"]
+target-version = ["py38", "py39", "py310", "py311", "py312"]
 
 [tool.ruff]
 ignore=["E731"]
 line-length = 120
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
+
+[tool.vulture]
+ignore_names = ["cli"]
+paths = ["sigsleep"]
```

### Comparing `sigsleep-1.1.1/sigsleep/sigsleep.py` & `sigsleep-1.2.0/sigsleep/sigsleep.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 
 def _handler(total: float, start: int, *_) -> None:
     """
     Bind total and start to make into a signal handler that prints elapsed time
     """
     remain: int = round(total - (time.time_ns() - start) / 1e9)
-    print(f"sleep: about {remain} seconds(s) left out of the original {total}")
+    t: str = str(int(total) if int(total) == total else total)
+    print(f"sleep: about {remain} seconds(s) left out of the original {t}")
 
 
 def sigsleep(seconds: float, sig: signal.Signals) -> int:
     """
     Sleep, print elapsed time on intercepting signal
     :return Exit code
     """
```

