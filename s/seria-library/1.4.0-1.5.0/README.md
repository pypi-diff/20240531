# Comparing `tmp/seria_library-1.4.0.tar.gz` & `tmp/seria_library-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seria_library-1.4.0.tar", max compression
+gzip compressed data, was "seria_library-1.5.0.tar", max compression
```

## Comparing `seria_library-1.4.0.tar` & `seria_library-1.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35802 2024-02-12 14:14:14.476983 seria_library-1.4.0/LICENSE
--rw-r--r--   0        0        0      984 2024-05-31 04:26:14.516911 seria_library-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       44 2024-02-12 14:14:14.417944 seria_library-1.4.0/README.md
--rw-r--r--   0        0        0      196 2024-02-13 09:11:45.197055 seria_library-1.4.0/seria/constants.py
--rw-r--r--   0        0        0     1680 2024-02-13 09:27:08.672935 seria_library-1.4.0/seria/dpy/ui.py
--rw-r--r--   0        0        0     1427 2024-05-31 04:26:14.518903 seria_library-1.4.0/seria/logging.py
--rw-r--r--   0        0        0     1136 2024-05-31 04:20:18.257910 seria_library-1.4.0/seria/tortoise/model.py
--rw-r--r--   0        0        0     4349 2024-05-31 04:26:14.518903 seria_library-1.4.0/seria/utils.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 seria_library-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35803 2024-02-16 14:31:05.554944 seria_library-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1213 2024-05-31 07:42:17.185490 seria_library-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-02-16 14:31:05.554944 seria_library-1.5.0/README.md
+-rw-r--r--   0        0        0      196 2024-02-16 14:31:05.555948 seria_library-1.5.0/seria/constants.py
+-rw-r--r--   0        0        0     1680 2024-02-16 14:31:05.555948 seria_library-1.5.0/seria/dpy/ui.py
+-rw-r--r--   0        0        0     1427 2024-05-31 07:27:46.296027 seria_library-1.5.0/seria/logging.py
+-rw-r--r--   0        0        0     1136 2024-02-16 14:49:11.055742 seria_library-1.5.0/seria/tortoise/model.py
+-rw-r--r--   0        0        0     4136 2024-05-31 07:33:01.061328 seria_library-1.5.0/seria/utils.py
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 seria_library-1.5.0/PKG-INFO
```

### Comparing `seria_library-1.4.0/LICENSE` & `seria_library-1.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `seria_library-1.4.0/pyproject.toml` & `seria_library-1.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 [tool.poetry]
 authors = ["seriaati <seria.ati@gmail.com>"]
 description = "Seria's library (of code)"
 license = "GPL-3.0"
 name = "seria-library"
 packages = [{include = "seria"}]
 readme = "README.md"
-version = "1.4.0"
+version = "1.5.0"
 
 [tool.poetry.dependencies]
-aiofiles = "^23.2.1"
-discord-py = {extras = ["speed"], version = "^2.3.2"}
-jishaku = "^2.5.2"
-orjson = "^3.9.13"
+aiofiles = {version = "^23.2.1", optional = true}
+discord-py = {version = "^2.3.2", optional = true}
+orjson = {version = "^3.9.13", optional = true}
 python = "^3.11"
-python-dotenv = "^1.0.1"
-pyyaml = "^6.0.1"
+pyyaml = {version = "^6.0.1", optional = true}
 tortoise-orm = {extras = ["asyncpg"], version = "^0.21.0"}
 
+[tool.poetry.extras]
+all = ["discord-py", "aiofiles", "orjson", "pyyaml", "tortoise-orm"]
+discord = ["discord-py"]
+files = ["aiofiles", "orjson", "pyyaml"]
+tortoise = ["tortoise-orm"]
+
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.1"
 ruff = "^0.4.0"
```

### Comparing `seria_library-1.4.0/seria/dpy/ui.py` & `seria_library-1.5.0/seria/dpy/ui.py`

 * *Files identical despite different names*

### Comparing `seria_library-1.4.0/seria/logging.py` & `seria_library-1.5.0/seria/logging.py`

 * *Files identical despite different names*

### Comparing `seria_library-1.4.0/seria/tortoise/model.py` & `seria_library-1.5.0/seria/tortoise/model.py`

 * *Files identical despite different names*

### Comparing `seria_library-1.4.0/seria/utils.py` & `seria_library-1.5.0/seria/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,14 @@
 import asyncio
 import os
 import re
 from typing import Any, TypeVar
 
-import aiofiles
-import orjson
-import yaml
-
 from .constants import IMAGE_EXTENSIONS, VIDEO_EXTENSIONS
 
-__all__ = (
-    "clean_url",
-    "create_bullet_list",
-    "extract_image_urls",
-    "extract_media_urls",
-    "extract_urls",
-    "extract_video_urls",
-    "read_json",
-    "read_yaml",
-    "shorten",
-    "split_list_to_chunks",
-    "write_json",
-    "write_yaml",
-)
-
 T = TypeVar("T")
 locks: dict[str, asyncio.Lock] = {}
 
 
 def clean_url(url: str) -> str:
     """Remove query parameters from the URL."""
     return url.split("?")[0]
@@ -69,14 +50,18 @@
 
 async def _read_file(
     path: str,
     encoding: str = "utf-8",
     handle_file_not_found: bool = True,
     ignore_lock: bool = False,
 ) -> Any:
+    import aiofiles
+    import orjson
+    import yaml
+
     lock = locks.setdefault(path, asyncio.Lock()) if not ignore_lock else asyncio.Lock()
     try:
         async with lock, aiofiles.open(path, mode="r", encoding=encoding) as file:
             if path.endswith(".json"):
                 return orjson.loads(await file.read())
             elif path.endswith(".yaml"):
                 return yaml.safe_load(await file.read())
@@ -90,14 +75,18 @@
 
 async def _write_file(
     path: str, data: Any, encoding: str = "utf-8", ignore_lock: bool = False
 ) -> None:
     if not os.path.exists(os.path.dirname(path)):
         os.makedirs(os.path.dirname(path))
 
+    import aiofiles
+    import orjson
+    import yaml
+
     lock = locks.setdefault(path, asyncio.Lock()) if not ignore_lock else asyncio.Lock()
     async with lock, aiofiles.open(path, mode="w", encoding=encoding) as file:
         if path.endswith(".json"):
             await file.write(orjson.dumps(data).decode(encoding))
         elif path.endswith(".yaml"):
             await file.write(yaml.dump(data))
         else:
```

