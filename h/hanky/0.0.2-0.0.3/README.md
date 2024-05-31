# Comparing `tmp/hanky-0.0.2.tar.gz` & `tmp/hanky-0.0.3.tar.gz`

## Comparing `hanky-0.0.2.tar` & `hanky-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/__about__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/__main__.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/cli.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/config.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/fs.py
--rw-r--r--   0        0        0    10960 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/hanky.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 hanky-0.0.2/src/hanky/media.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hanky-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hanky-0.0.2/LICENSE
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 hanky-0.0.2/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 hanky-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 hanky-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/__about__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/__main__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/cli.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/fs.py
+-rw-r--r--   0        0        0    22084 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/hanky.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 hanky-0.0.3/src/hanky/media.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hanky-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hanky-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 hanky-0.0.3/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 hanky-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 hanky-0.0.3/PKG-INFO
```

### Comparing `hanky-0.0.2/src/hanky/config.py` & `hanky-0.0.3/src/hanky/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import platform
 from pathlib import Path
-from typing import Callable, Union
+from typing import Callable, IO, Any
+
 
 def _get_default_anki_db_path() -> str:
     """Choose a default path for the anki sqlite collection database based on
     the OS.
 
     Defaults:
         Linux: "~/.local/share/Anki2/User 1/collection.anki2"
@@ -21,36 +22,53 @@
 ANKI_DB_PATH = "anki_database"
 DO_SAFET_CHECK = "database_safety_check"
 ALLOW_DUPLICATES = "allow_duplicates"
 
 DEFAULT_CONFIG = {
     ANKI_DB_PATH: _get_default_anki_db_path(),
     DO_SAFET_CHECK: True,
-    ALLOW_DUPLICATES: False
+    ALLOW_DUPLICATES: False,
 }
 
+DEFAULT_CONFIG_PATH = Path("~/.config/hanky/hanky.toml").expanduser()
+
+
 class Config(dict):
     """Configuration object"""
 
-
     def __init__(self, **kwargs):
         self._config = None
-        self.default_path = Path("~/.config/hanky/hanky.toml").expanduser()
+
         super().__init__(kwargs)
 
     def from_file(
         self,
-        file: Union[Path, str],
-        loader: Callable[[Union[str, Path], dict], dict],
-        text=False,
+        fpath: str,
+        loader: Callable[[IO[Any]], dict],
+        is_text=False,
         **kwargs,
-    ):
-        with open(file, "r" if text else "rb") as f:
+    ) -> bool:
+        """Load configuration data from a file
+
+        Args:
+            fpath: path to a file
+            loader: function to use to read the file
+            is_text: if the file should be read as text or binary. True for text
+            **kwargs: key word arguments for the loader function
+
+        Returns:
+            True on successfull
+
+        Raises:
+            TypeError if the output of the loader function is not a dictionary.
+        """
+        with open(fpath, "r" if is_text else "rb") as f:
             cfg = loader(f, **kwargs)
             if not isinstance(cfg, dict):
                 raise TypeError(
                     f"Received type '{type(cfg)}' but expected '{type(dict)}' from loader function."
                 )
 
             for k, v in cfg.items():
                 self[k] = v
 
+        return True
```

### Comparing `hanky-0.0.2/.gitignore` & `hanky-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hanky-0.0.2/LICENSE` & `hanky-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hanky-0.0.2/README.md` & `hanky-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hanky-0.0.2/pyproject.toml` & `hanky-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,21 @@
 
 dependencies = [
   "anki",
   "psutil"
 ]
 
 [project.optional-dependencies]
-# tos = [
-#   "boto3"
-# ]
-
-dev = [
-  "pytest",
-  "mypy"
+tos = [
+  "boto3"
 ]
 
+[project.scripts]
+hanky = "hanky.__main__:main"
+
 [project.urls]
 Homepage = "https://github.com/Haeata-Ash/hanky"
 Issues = "https://github.com/Haeata-Ash/hanky/issues"
 
 [tool]
 
 [tool.hatch.version]
@@ -50,8 +48,16 @@
   "/.venv",
   "/.mypy_cache",
   "/demo.py",
   "/.*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/hanky"]
+packages = ["src/hanky"]
+
+[tool.hatch.envs.dev]
+dependencies = [
+  "pytest",
+  "mypy",
+  "types-psutil",
+  "pre-commit"
+]
```

### Comparing `hanky-0.0.2/PKG-INFO` & `hanky-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.3
 Name: hanky
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple library and command line tool for loading flash cards into anki.
 Project-URL: Homepage, https://github.com/Haeata-Ash/hanky
 Project-URL: Issues, https://github.com/Haeata-Ash/hanky/issues
 Author-email: HBA <hanky-pypi.8ebs0@simplelogin.com>
 License-File: LICENSE
 Keywords: anki
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: anki
 Requires-Dist: psutil
-Provides-Extra: dev
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
+Provides-Extra: tos
+Requires-Dist: boto3; extra == 'tos'
 Description-Content-Type: text/markdown
 
 # hanky
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 
 Hanky is a simple application framework and command line application for loading flash cards into anki.
```

