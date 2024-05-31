# Comparing `tmp/retrocookie-0.4.2.tar.gz` & `tmp/retrocookie-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrocookie-0.4.2.tar", max compression
+gzip compressed data, was "retrocookie-0.4.3.tar", max compression
```

## Comparing `retrocookie-0.4.2.tar` & `retrocookie-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1088 2021-11-22 11:43:53.632290 retrocookie-0.4.2/LICENSE.rst
--rw-r--r--   0        0        0     9873 2021-11-22 11:43:53.632290 retrocookie-0.4.2/README.rst
--rw-r--r--   0        0        0     2784 2021-11-22 11:44:02.304350 retrocookie-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      135 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/__init__.py
--rw-r--r--   0        0        0     4402 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/__main__.py
--rw-r--r--   0        0        0       27 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/compat/__init__.py
--rw-r--r--   0        0        0      518 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/compat/contextlib.py
--rw-r--r--   0        0        0     5692 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/core.py
--rw-r--r--   0        0        0     4560 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/filter.py
--rw-r--r--   0        0        0     8855 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/git.py
--rw-r--r--   0        0        0       70 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/__init__.py
--rw-r--r--   0        0        0     6356 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/__main__.py
--rw-r--r--   0        0        0       16 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/adapters/__init__.py
--rw-r--r--   0        0        0     7080 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/adapters/github.py
--rw-r--r--   0        0        0      346 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/adapters/retrocookie.py
--rw-r--r--   0        0        0       52 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/base/__init__.py
--rw-r--r--   0        0        0     5493 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/base/bus.py
--rw-r--r--   0        0        0    11080 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/base/exceptionhandlers.py
--rw-r--r--   0        0        0     2182 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/cache.py
--rw-r--r--   0        0        0       27 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/compat/__init__.py
--rw-r--r--   0        0        0      373 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/compat/shlex.py
--rw-r--r--   0        0        0      186 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/compat/typing.py
--rw-r--r--   0        0        0     7975 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/console.py
--rw-r--r--   0        0        0     3597 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/core.py
--rw-r--r--   0        0        0     2469 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/events.py
--rw-r--r--   0        0        0     2856 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/importer.py
--rw-r--r--   0        0        0     1474 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/list.py
--rw-r--r--   0        0        0       36 2021-11-22 11:43:53.632290 retrocookie-0.4.2/src/retrocookie/pr/protocols/__init__.py
--rw-r--r--   0        0        0     2478 2021-11-22 11:43:53.636290 retrocookie-0.4.2/src/retrocookie/pr/protocols/github.py
--rw-r--r--   0        0        0      375 2021-11-22 11:43:53.636290 retrocookie-0.4.2/src/retrocookie/pr/protocols/retrocookie.py
--rw-r--r--   0        0        0      749 2021-11-22 11:43:53.636290 retrocookie-0.4.2/src/retrocookie/pr/repository.py
--rw-r--r--   0        0        0        0 2021-11-22 11:43:53.636290 retrocookie-0.4.2/src/retrocookie/py.typed
--rw-r--r--   0        0        0      708 2021-11-22 11:43:53.636290 retrocookie-0.4.2/src/retrocookie/utils.py
--rw-r--r--   0        0        0    11604 2021-11-22 11:44:04.246537 retrocookie-0.4.2/setup.py
--rw-r--r--   0        0        0    11393 2021-11-22 11:44:04.247508 retrocookie-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-05-31 13:23:57.828514 retrocookie-0.4.3/LICENSE.rst
+-rw-r--r--   0        0        0     9873 2024-05-31 13:23:57.828514 retrocookie-0.4.3/README.rst
+-rw-r--r--   0        0        0     2920 2024-05-31 13:24:09.420496 retrocookie-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/__main__.py
+-rw-r--r--   0        0        0       27 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/compat/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/compat/contextlib.py
+-rw-r--r--   0        0        0     5702 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/core.py
+-rw-r--r--   0        0        0     4561 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/filter.py
+-rw-r--r--   0        0        0     8856 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/git.py
+-rw-r--r--   0        0        0       71 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/__init__.py
+-rw-r--r--   0        0        0     6331 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/__main__.py
+-rw-r--r--   0        0        0       16 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/adapters/__init__.py
+-rw-r--r--   0        0        0     7101 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/adapters/github.py
+-rw-r--r--   0        0        0      347 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/adapters/retrocookie.py
+-rw-r--r--   0        0        0       52 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/base/__init__.py
+-rw-r--r--   0        0        0     5494 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/base/bus.py
+-rw-r--r--   0        0        0    11086 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/base/exceptionhandlers.py
+-rw-r--r--   0        0        0     2183 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/cache.py
+-rw-r--r--   0        0        0       27 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/compat/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/compat/shlex.py
+-rw-r--r--   0        0        0      188 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/compat/typing.py
+-rw-r--r--   0        0        0     7604 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/console.py
+-rw-r--r--   0        0        0     3598 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/core.py
+-rw-r--r--   0        0        0     2470 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/events.py
+-rw-r--r--   0        0        0     2857 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/importer.py
+-rw-r--r--   0        0        0     1475 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/list.py
+-rw-r--r--   0        0        0       36 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/protocols/__init__.py
+-rw-r--r--   0        0        0     2479 2024-05-31 13:23:57.828514 retrocookie-0.4.3/src/retrocookie/pr/protocols/github.py
+-rw-r--r--   0        0        0      376 2024-05-31 13:23:57.832514 retrocookie-0.4.3/src/retrocookie/pr/protocols/retrocookie.py
+-rw-r--r--   0        0        0      750 2024-05-31 13:23:57.832514 retrocookie-0.4.3/src/retrocookie/pr/repository.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:23:57.832514 retrocookie-0.4.3/src/retrocookie/py.typed
+-rw-r--r--   0        0        0      709 2024-05-31 13:23:57.832514 retrocookie-0.4.3/src/retrocookie/utils.py
+-rw-r--r--   0        0        0    11403 1970-01-01 00:00:00.000000 retrocookie-0.4.3/PKG-INFO
```

### Comparing `retrocookie-0.4.2/LICENSE.rst` & `retrocookie-0.4.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `retrocookie-0.4.2/README.rst` & `retrocookie-0.4.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
    {{ cookiecutter | jsonify }}
 
 
 Requirements
 ------------
 
-* Python 3.7+
+* Python 3.8+
 * git >= 2.22.0
 
 
 Installation
 ------------
 
 You can install *Retrocookie* via pip_ from PyPI_:
```

### Comparing `retrocookie-0.4.2/pyproject.toml` & `retrocookie-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrocookie"
-version = "0.4.2"
+version = "0.4.3"
 description = "Update Cookiecutter templates with changes from their instances"
 authors = ["Claudio Jolowicz <mail@claudiojolowicz.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/cjolowicz/retrocookie"
 repository = "https://github.com/cjolowicz/retrocookie"
 documentation = "https://retrocookie.readthedocs.io"
@@ -17,70 +17,77 @@
     "Operating System :: POSIX :: Linux",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/cjolowicz/retrocookie/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 click = "^8.0.3"
 git-filter-repo = "^2.26.0"
-pygit2 = "^1.2.1"
+pygit2 = ">=1.2.1,<1.15"
 typing-extensions = {version = ">=3.7.4,<5.0.0", optional = true}
 "github3.py" = {version = "^3.0.0", optional = true}
 tenacity = {version = ">=6.3.1,<9.0.0", optional = true}
 appdirs = {version = "^1.4.4", optional = true}
 rich = {version = ">=9.5.1,<11.0.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.1"}
 safety = ">=1.10.3"
 mypy = ">=0.800"
-typeguard = ">=2.9.1"
+typeguard = ">=2.9.1,<3"
 xdoctest = {extras = ["colors"], version = ">=0.15.2"}
 sphinx = ">=4.3.0"
 sphinx-autobuild = ">=2020.9.1"
 pre-commit = ">=2.15.0"
 cookiecutter = ">=1.7.3"
 pygments = ">=2.10.0"
 flake8 = ">=4.0.1"
 black = ">=21.10b0"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.3"
 pep8-naming = ">=0.11.1"
 darglint = ">=1.8.1"
-reorder-python-imports = ">=2.6.0"
 pre-commit-hooks = ">=4.0.1"
 sphinx-click = ">=3.0.2"
 Pygments = ">=2.10.0"
 furo = ">=2021.11.12"
 types-requests = ">=2.26.0"
 pyupgrade = ">=2.29.0"
+isort = "^5.10.1"
 
 [tool.poetry.extras]
 pr = ["appdirs", "github3.py", "rich", "tenacity", "typing-extensions"]
 
 [tool.poetry.scripts]
 retrocookie = "retrocookie.__main__:main"
 retrocookie-pr = "retrocookie.pr.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
+tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
-source = ["retrocookie"]
+source = ["retrocookie", "tests"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 90
 
+[tool.isort]
+profile = "black"
+force_single_line = true
+order_by_type = false
+lines_after_imports = 2
+
 [tool.mypy]
 strict = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
```

### Comparing `retrocookie-0.4.2/src/retrocookie/__main__.py` & `retrocookie-0.4.3/src/retrocookie/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Command-line interface."""
+
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Any
 from typing import Container
 from typing import Iterable
 from typing import Optional
 
 import click
```

### Comparing `retrocookie-0.4.2/src/retrocookie/compat/contextlib.py` & `retrocookie-0.4.3/src/retrocookie/compat/contextlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Compatibility shim for contextlib."""
+
 import contextlib
 from typing import Callable
 from typing import ContextManager
 from typing import Iterator
 from typing import TypeVar
```

### Comparing `retrocookie-0.4.2/src/retrocookie/core.py` & `retrocookie-0.4.3/src/retrocookie/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Core module."""
+
 import json
 import tempfile
 from pathlib import Path
 from typing import Any
 from typing import cast
 from typing import Container
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 
+from retrocookie.compat import contextlib
+
 from . import git
 from .filter import RepositoryFilter
-from retrocookie.compat import contextlib
 
 
 @contextlib.contextmanager
 def temporary_repository() -> Iterator[git.Repository]:
     """Create repository in temporary directory."""
     with tempfile.TemporaryDirectory() as tmpdir:
         path = Path(tmpdir)
@@ -26,15 +28,15 @@
 
 def find_template_directory(repository: git.Repository) -> Path:
     """Locate the subdirectory with the project template."""
     tokens = "{{", "cookiecutter", "}}"
     for path in repository.path.iterdir():
         if path.is_dir() and all(x in path.name for x in tokens):
             return path.relative_to(repository.path)
-    raise Exception("cannot find template directory")
+    raise FileNotFoundError("cannot find template directory")
 
 
 def load_context(repository: git.Repository, ref: str) -> Dict[str, Any]:
     """Load the context from the .cookiecutter.json file."""
     path = Path(".cookiecutter.json")
     text = repository.read_text(path, ref=ref)
     data = json.loads(text)
```

### Comparing `retrocookie-0.4.2/src/retrocookie/filter.py` & `retrocookie-0.4.3/src/retrocookie/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface for git-filter-repo."""
+
 import contextlib
 import io
 import re
 from pathlib import Path
 from typing import Any
 from typing import Container
 from typing import Dict
```

### Comparing `retrocookie-0.4.2/src/retrocookie/git.py` & `retrocookie-0.4.3/src/retrocookie/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Git interface."""
+
 from __future__ import annotations
 
 import contextlib
 import functools
 import operator
 import re
 import subprocess  # noqa: S404
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/__main__.py` & `retrocookie-0.4.3/src/retrocookie/pr/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command-line interface."""
+
 import contextlib
 import subprocess  # noqa: S404
 import webbrowser
 from pathlib import Path
 from typing import Collection
 from typing import Iterator
 from typing import List
@@ -76,15 +77,15 @@
 def register_pull_request_viewer(*, bus: Bus) -> None:
     """Register an event handler for viewing pull requests in a browser."""
 
     @bus.events.subscribe
     def _(event: events.PullRequestCreated) -> None:
         webbrowser.open(event.template_pull.html_url)
 
-    @bus.contexts.subscribe  # type: ignore[no-redef]
+    @bus.contexts.subscribe
     @contextmanager
     def _(event: events.UpdatePullRequest) -> Iterator[None]:
         yield
         webbrowser.open(event.template_pull.html_url)
 
 
 @click.command()
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/adapters/github.py` & `retrocookie-0.4.3/src/retrocookie/pr/adapters/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """GitHub interface."""
+
 from __future__ import annotations
 
 from typing import AbstractSet
 from typing import cast
 from typing import Iterable
 from typing import Optional
 from typing import Set
@@ -146,16 +147,16 @@
             base=self._repository.default_branch,
         )
 
         # The GitHub API sometimes responds with 404 when the issue for
         # a newly created pull request is requested.
         for attempt in tenacity.Retrying(
             reraise=True,
-            stop=tenacity.stop_after_attempt(3),  # type: ignore[attr-defined]
-            wait=tenacity.wait_fixed(3),  # type: ignore[attr-defined]
+            stop=tenacity.stop_after_attempt(3),
+            wait=tenacity.wait_fixed(3),
         ):
             with attempt:
                 pull_request.issue().add_labels(*labels)
 
         return PullRequest(pull_request)
 
 
@@ -207,18 +208,18 @@
                 )
             )
         return None
 
     @exceptionhandler
     def _handler2(error: github3.exceptions.ConnectionError) -> None:
         for arg in error.args:
-            if isinstance(arg, requests.RequestException):
+            if isinstance(arg, requests.RequestException) and arg.request is not None:
                 bus.events.raise_(
                     events.ConnectionError(
-                        arg.request.url,
-                        arg.request.method,
+                        arg.request.url,  # type: ignore[arg-type]
+                        arg.request.method,  # type: ignore[arg-type]
                         str(error),
                     )
                 )
         return None
 
     return _handler1 >> _handler2
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/base/bus.py` & `retrocookie-0.4.3/src/retrocookie/pr/base/bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 ...     print("copy: file a")
 ...     print("copy: file b")
 starting copy...
 copy: file a
 copy: file b
 copy complete.
 """
+
 from collections import defaultdict
 from contextlib import ExitStack
 from typing import Any
 from typing import ContextManager
 from typing import Dict
 from typing import get_type_hints
 from typing import Iterator
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/base/exceptionhandlers.py` & `retrocookie-0.4.3/src/retrocookie/pr/base/exceptionhandlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 In algebraic terms, ``nullhandler`` is the identity element of composition
 (``<<`` and ``>>``): Combining any handler with ``nullhandler`` gives you a
 handler that behaves exactly like the original handler. As composition is also
 associative, this makes exception handlers with composition a simple monoid_.
 
 .. _monoid: https://en.wikipedia.org/wiki/Monoid
 """
+
 from __future__ import annotations
 
 import contextlib
 from types import TracebackType
 from typing import Callable
 from typing import Generic
 from typing import get_type_hints
@@ -339,13 +340,13 @@
 
         @exceptionhandler
         def exit_handler(exception: SomeException) -> NoReturn:
             raise SystemExit(str(exception))
 
     """
     if all(isinstance(arg, type) and issubclass(arg, BaseException) for arg in args):
-        exception_types: Tuple[Type[BaseException]] = args  # type: ignore[assignment]
+        exception_types: Tuple[Type[BaseException], ...] = args  # type: ignore[assignment]
         return _exceptionhandler(*exception_types)
 
     callback: _Callback[E]
     [callback] = args  # type: ignore[assignment]
     return _exceptionhandler()(callback)
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/cache.py` & `retrocookie-0.4.3/src/retrocookie/pr/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Application cache."""
+
 import hashlib
 import json
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterator
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/console.py` & `retrocookie-0.4.3/src/retrocookie/pr/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Application console."""
+
 from typing import ContextManager
 from typing import Iterator
 
 import rich.console
 import rich.theme
 import rich.traceback
 from rich.markup import escape
@@ -72,29 +73,27 @@
 
     console = Console()
 
     _subscribe(console, bus)
 
 
 def _subscribe(console: Console, bus: Bus) -> None:  # noqa: C901
-    _ = None  # Ignoring redefinitions of this name below.
-
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.GitNotFound) -> None:
         console.failure("git not found")
         console.hint("Do you have git installed?")
         console.hint("Is git on your PATH?")
         console.hint("Can you run [command]git version[/]?")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.BadGitVersion) -> None:
         console.failure(f"This program requires git [version]{event.expected}[/].")
         console.hint(f"You have git [version]{event.version}[/], which is too old.")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.GitFailed) -> None:
         def _lines() -> Iterator[str]:
             yield (
                 f"The command [command]git {event.command}[/] failed"
                 f" with status [status]{event.status}[/]."
             )
 
@@ -117,87 +116,87 @@
 
         if event.command == "cherry-pick":
             console.hint("Looks like the changes did not apply cleanly.")
             console.hint(
                 "Try running [command]retrocookie[/] on a local clone instead."
             )
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.GitHubError) -> None:
         def _lines() -> Iterator[str]:
             yield "The GitHub API returned an error response."
             yield f"[http.method]{event.method}[/] [repr.url]{event.url}[/]"
             yield f"[http.status]{event.code}[/] {event.message}"
             yield from event.errors
 
         console.failure("\n".join(_lines()))
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.ConnectionError) -> None:
         def _lines() -> Iterator[str]:
             yield "Connection to GitHub API could not be established."
             yield f"[http.method]{event.method}[/] [repr.url]{event.url}[/]"
 
         console.failure("\n".join(_lines()))
         console.highlight(event.error)
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.ProjectNotFound) -> None:
         console.failure("Project not found")
         console.hint("Does the current directory contain a repository?")
         console.hint("Is the repository on GitHub?")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.TemplateNotFound) -> None:
         console.failure(
             f"Project template for [repository]{event.project.full_name}[/] not found"
         )
         console.hint("Does the project contain a .cookiecutter.json file?")
         console.hint(
             'Does the .cookiecutter.json contain the repository URL under "_template"?'
         )
         console.hint("Is the template repository on GitHub?")
 
-    @bus.contexts.subscribe  # type: ignore[no-redef]
+    @bus.contexts.subscribe  # type: ignore[arg-type]
     def _(event: events.LoadProject) -> ContextManager[None]:
         return console.progress(f"Loading project [repository]{event.repository}[/]")
 
-    @bus.contexts.subscribe  # type: ignore[no-redef]
+    @bus.contexts.subscribe  # type: ignore[arg-type]
     def _(event: events.LoadTemplate) -> ContextManager[None]:
         return console.progress(f"Loading template [repository]{event.repository}[/]")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.RepositoryNotFound) -> None:
         console.failure(f"Repository [repository]{event.repository}[/] not found")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.PullRequestNotFound) -> None:
         spec = event.pull_request
         if spec.isnumeric():
             spec = f"#{spec}"
         console.failure(f"Pull request [pull]{spec}[/] not found")
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.PullRequestAlreadyExists) -> None:
         console.failure(
             "Already imported"
             f" [pull]#{event.project_pull.number}[/]"
             f" [title]{escape(event.project_pull.title)}[/]"
         )
         console.hint(f"See [pull]#{event.template_pull.number}[/]")
         console.hint("Use --force to update an existing pull request.")
 
-    @bus.contexts.subscribe  # type: ignore[no-redef]
+    @bus.contexts.subscribe  # type: ignore[arg-type]
     def _(event: events.CreatePullRequest) -> ContextManager[None]:
         return console.progress(
             f"[pull]#{event.project_pull.number}[/]"
             f" [title]{escape(event.project_pull.title)}[/]"
         )
 
-    @bus.contexts.subscribe  # type: ignore[no-redef]
+    @bus.contexts.subscribe
     @contextlib.contextmanager
     def _(event: events.UpdatePullRequest) -> Iterator[None]:
         with console.progress(
             f"[pull]#{event.project_pull.number}[/]"
             f" [title]{escape(event.project_pull.title)}[/]"
             f" [oldpull]#{event.template_pull.number}[/]"
         ):
@@ -205,14 +204,14 @@
 
         console.success(
             f"[pull]#{event.project_pull.number}[/]"
             f" [title]{escape(event.project_pull.title)}[/]"
             f" [pull]#{event.template_pull.number}[/]"
         )
 
-    @bus.events.subscribe  # type: ignore[no-redef]
+    @bus.events.subscribe
     def _(event: events.PullRequestCreated) -> None:
         console.success(
             f"[pull]#{event.project_pull.number}[/]"
             f" [title]{escape(event.project_pull.title)}[/]"
             f" [pull]#{event.template_pull.number}[/]"
         )
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/core.py` & `retrocookie-0.4.3/src/retrocookie/pr/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Import pull requests."""
+
 from typing import Collection
 from typing import Optional
 from urllib.parse import urlparse
 
 from retrocookie import git
 from retrocookie.core import load_context
 from retrocookie.pr import events
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/events.py` & `retrocookie-0.4.3/src/retrocookie/pr/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Events and contexts for the message bus."""
+
 from dataclasses import dataclass
 from typing import List
 
 from retrocookie import git
 from retrocookie.pr.base import bus
 from retrocookie.pr.protocols import github
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/importer.py` & `retrocookie-0.4.3/src/retrocookie/pr/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Import pull requests."""
+
 from dataclasses import dataclass
 
 from retrocookie.pr import appname
 from retrocookie.pr import events
 from retrocookie.pr.base.bus import Bus
 from retrocookie.pr.base.bus import Context
 from retrocookie.pr.cache import Cache
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/list.py` & `retrocookie-0.4.3/src/retrocookie/pr/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Listing pull requests."""
+
 import contextlib
 from typing import Collection
 from typing import Iterator
 from typing import Optional
 
 from retrocookie.pr import events
 from retrocookie.pr.base.bus import Bus
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/protocols/github.py` & `retrocookie-0.4.3/src/retrocookie/pr/protocols/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Protocols for retrocookie.pr.github."""
+
 from __future__ import annotations
 
 from typing import AbstractSet
 from typing import Iterable
 from typing import Optional
 from typing import Set
```

### Comparing `retrocookie-0.4.2/src/retrocookie/pr/repository.py` & `retrocookie-0.4.3/src/retrocookie/pr/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """High-level repository abstraction."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from retrocookie import git
 from retrocookie.pr.cache import Cache
 from retrocookie.pr.protocols import github as gh
```

### Comparing `retrocookie-0.4.2/src/retrocookie/utils.py` & `retrocookie-0.4.3/src/retrocookie/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities."""
+
 import os
 from pathlib import Path
 from typing import Iterator
 
 from retrocookie.compat import contextlib
```

### Comparing `retrocookie-0.4.2/setup.py` & `retrocookie-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,367 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: retrocookie
+Version: 0.4.3
+Summary: Update Cookiecutter templates with changes from their instances
+Home-page: https://github.com/cjolowicz/retrocookie
+License: MIT
+Author: Claudio Jolowicz
+Author-email: mail@claudiojolowicz.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: pr
+Requires-Dist: appdirs (>=1.4.4,<2.0.0) ; extra == "pr"
+Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: git-filter-repo (>=2.26.0,<3.0.0)
+Requires-Dist: github3.py (>=3.0.0,<4.0.0) ; extra == "pr"
+Requires-Dist: pygit2 (>=1.2.1,<1.15)
+Requires-Dist: rich (>=9.5.1,<11.0.0) ; extra == "pr"
+Requires-Dist: tenacity (>=6.3.1,<9.0.0) ; extra == "pr"
+Requires-Dist: typing-extensions (>=3.7.4,<5.0.0) ; extra == "pr"
+Project-URL: Changelog, https://github.com/cjolowicz/retrocookie/releases
+Project-URL: Documentation, https://retrocookie.readthedocs.io
+Project-URL: Repository, https://github.com/cjolowicz/retrocookie
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+Retrocookie
+===========
 
-packages = \
-['retrocookie',
- 'retrocookie.compat',
- 'retrocookie.pr',
- 'retrocookie.pr.adapters',
- 'retrocookie.pr.base',
- 'retrocookie.pr.compat',
- 'retrocookie.pr.protocols']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.3,<9.0.0',
- 'git-filter-repo>=2.26.0,<3.0.0',
- 'pygit2>=1.2.1,<2.0.0']
-
-extras_require = \
-{'pr': ['typing-extensions>=3.7.4,<5.0.0',
-        'github3.py>=3.0.0,<4.0.0',
-        'tenacity>=6.3.1,<9.0.0',
-        'appdirs>=1.4.4,<2.0.0',
-        'rich>=9.5.1,<11.0.0']}
-
-entry_points = \
-{'console_scripts': ['retrocookie = retrocookie.__main__:main',
-                     'retrocookie-pr = retrocookie.pr.__main__:main']}
-
-setup_kwargs = {
-    'name': 'retrocookie',
-    'version': '0.4.2',
-    'description': 'Update Cookiecutter templates with changes from their instances',
-    'long_description': 'Retrocookie\n===========\n\n|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/retrocookie.svg\n   :target: https://pypi.org/project/retrocookie/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/retrocookie\n   :target: https://pypi.org/project/retrocookie\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/retrocookie\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/retrocookie/latest.svg?label=Read%20the%20Docs\n   :target: https://retrocookie.readthedocs.io/\n   :alt: Read the documentation at https://retrocookie.readthedocs.io/\n.. |Tests| image:: https://github.com/cjolowicz/retrocookie/workflows/Tests/badge.svg\n   :target: https://github.com/cjolowicz/retrocookie/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/cjolowicz/retrocookie/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/cjolowicz/retrocookie\n   :alt: Codecov\n\n\nRetrocookie updates Cookiecutter_ templates with changes from generated projects.\n\nWhen developing Cookiecutter templates,\nyou often need to work in a generated project rather than the template itself.\nReasons for this include the following:\n\n- You need to run the Continuous Integration suite for the generated project\n- Your development tools choke when running on the templated project\n\nAny changes you make in the generated project\nneed to be backported into the template,\ncarefully replacing expanded variables from ``cookiecutter.json`` by templating tags,\nand escaping any use of ``{{`` and ``}}``\nor other tokens with special meaning in Jinja.\n\n✨ Retrocookie helps you in this situation. ✨\n\nIt is designed to fetch commits from the repository of a generated project,\nand import them into your Cookiecutter repository,\nrewriting them on the fly to insert templating tags,\nescape Jinja-special constructs,\nand place files in the template directory.\n\nUnder the hood,\nRetrocookie rewrites the selected commits using git-filter-repo_,\nsaving them to a temporary repository.\nIt then fetches and cherry-picks the rewritten commits\nfrom the temporary repository into the Cookiecutter template,\nusing pygit2_.\n\nMaybe you\'re thinking,\nhow can this possibly work?\nOne cannot reconstruct a Jinja template from its rendered output.\nHowever, simple replacements of template variables work well in practice\nwhen you\'re only importing a handful of commits at a time.\n\n**Important:**\n\nRetrocookie relies on a ``.cookiecutter.json`` file in the generated project\nto work out how to rewrite commits.\nThis file is similar to the ``cookiecutter.json`` file in the template,\nbut contains the specific values chosen during project generation.\nYou can generate this file by putting it into the template directory in the Cookiecutter,\nwith the following contents:\n\n.. code:: jinja\n\n   {{ cookiecutter | jsonify }}\n\n\nRequirements\n------------\n\n* Python 3.7+\n* git >= 2.22.0\n\n\nInstallation\n------------\n\nYou can install *Retrocookie* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install retrocookie\n\nOptionally, install the ``pr`` extra for the retrocookie-pr_ command:\n\n.. code:: console\n\n   $ pip install retrocookie[pr]\n\n\nExample\n-------\n\nHere\'s an example to demonstrate the general workflow.\n\nTo start with, we clone the repository of your Cookiecutter template.\nFor this example, I\'ll use my own `Hypermodern Python Cookiecutter`_.\n\n.. code:: console\n\n   $ git clone https://github.com/cjolowicz/cookiecutter-hypermodern-python\n\nNext, we\'ll create a project from the template,\nand set up a git repository for it:\n\n.. code:: console\n\n   $ cookiecutter --no-input cookiecutter-hypermodern-python\n   $ cd hypermodern-python\n   $ git init\n   $ git add .\n   $ git commit --message="Initial commit"\n\nLet\'s open a feature branch in the project repository,\nand make a fictitious change involving the default project name *hypermodern-python*:\n\n.. code:: console\n\n   $ git switch --create add-example\n   $ echo \'# hypermodern-python\' > EXAMPLE.md\n   $ git add EXAMPLE.md\n   $ git commit --message="Add example"\n\nBack in the Cookiecutter repository,\nwe can now invoke retrocookie to import the changes from the feature branch:\n\n.. code:: console\n\n   $ cd ../cookiecutter-hypermodern-python\n   $ retrocookie --branch add-example --create ../hypermodern-python\n\nA ``git show`` in the Cookiecutter shows the file under the template directory,\non a branch named as in the original repository,\nwith the project name replaced by a Jinja tag:\n\n.. code:: diff\n\n   commit abb4f823b9f1760e3a678c927ec9797c0a40a9b6 (HEAD -> add-example)\n   Author: Your Name <your.name@example.com>\n   Date:   Fri Dec 4 23:40:41 2020 +0100\n\n       Add example\n\n   diff --git a/{{cookiecutter.project_name}}/EXAMPLE.md b/{{cookiecutter.project_name}}/EXAMPLE.md\n   new file mode 100644\n   index 0000000..a158618\n   --- /dev/null\n   +++ b/{{cookiecutter.project_name}}/EXAMPLE.md\n   @@ -0,0 +1 @@\n   +# {{cookiecutter.project_name}}\n\n\nUsage\n-----\n\nThe basic form:\n\n.. code::\n\n   $ retrocookie <repository> [<commits>...]\n   $ retrocookie <repository> -b <branch> [--create]\n\nThe ``<repository>`` is a filesystem path to the source repository.\nFor ``<commits>``, see `gitrevisions(7)`__.\n\n__ https://git-scm.com/docs/gitrevisions\n\nImport ``HEAD`` from ``<repository>``:\n\n.. code::\n\n   $ retrocookie <repository>\n\nImport the last two commits:\n\n.. code::\n\n   $ retrocookie <repository> HEAD~2..\n\nImport by commit hash:\n\n.. code::\n\n   $ retrocookie <repository> 53268f7 6a3368a c0b4c6c\n\nImport commits from branch ``topic``:\n\n.. code::\n\n   $ retrocookie <repository> --branch=topic\n\nEquivalently:\n\n.. code::\n\n   $ retrocookie <repository> master..topic\n\nImport commits from ``topic`` into a branch with the same name:\n\n.. code::\n\n   $ retrocookie <repository> --branch=topic --create\n\nEquivalently, using short options:\n\n.. code::\n\n   $ retrocookie <repository> -cb topic\n\nImport commits from branch ``topic``, which was branched off ``1.0``:\n\n.. code::\n\n   $ retrocookie <repository> --branch=topic --upstream=1.0\n\nEquivalently:\n\n.. code::\n\n   $ retrocookie <repository> 1.0..topic\n\nImport ``HEAD`` into a new branch ``topic``:\n\n.. code::\n\n   $ retrocookie <repository> --create-branch=topic\n\nPlease see the `Command-line Reference <Usage_>`_ for further details.\n\n\n.. _retrocookie-pr:\n\nImporting pull requests from generated projects with retrocookie-pr\n-------------------------------------------------------------------\n\nYou can import pull requests from a generated project to the project template,\nassuming their repositories are on GitHub_.\nThis requires activating the ``pr`` extra when installing with pip_:\n\n.. code::\n\n  $ pip install retrocookie[pr]\n\nThe command ``retrocookie-pr`` has the basic form:\n\n.. code::\n\n   $ retrocookie-pr [-R <repository>] [<pr>...]\n   $ retrocookie-pr [-R <repository>] --user=<user>\n   $ retrocookie-pr [-R <repository>] --all\n\nCommand-line arguments specify pull requests to import, by number or by branch.\nPull requests from forks are currently not supported.\n\nUse the ``-R <repository>`` option to specify the GitHub repository of the generated project\nfrom which the pull requests should be imported.\nProvide the full name of the repository on GitHub in the form ``owner/name``.\nThe owner can be omitted if the repository is owned by the authenticated user.\nThis option can be omitted when the command is invoked from a local clone.\n\nYou can also select pull requests by specifying the user that opened them, via the ``--user`` option.\nThis is handy for importing automated pull requests, such as dependency updates from Dependabot_.\n\nUse the ``--all`` option to import all open pull requests in the generated project.\n\nYou can update previously imported pull requests by specifying ``--force``.\nBy default, ``retrocookie-pr`` refuses to overwrite existing pull requests.\n\nThe command needs a `personal access token`_ to access the GitHub API.\n(This token is also used to push to the GitHub repository of the project template.)\nYou will be prompted for the token when you invoke the command for the first time.\nOn subsequent invocations, the token is read from the application cache.\nAlternatively, you can specify the token using the ``--token`` option or the ``GITHUB_TOKEN`` environment variable;\nboth of these methods bypass the cache.\n\nUse the ``--open`` option to open each imported pull request in a web browser.\n\nPlease see the `Command-line Reference <Usage_>`_ for further details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the MIT_ license,\n*Retrocookie* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_\'s `Hypermodern Python Cookiecutter`_ template.\n\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _Dependabot: https://dependabot.com/\n.. _GitHub: https://github.com/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _MIT: http://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _file an issue: https://github.com/cjolowicz/retrocookie/issues\n.. _git-filter-repo: https://github.com/newren/git-filter-repo\n.. _git rebase: https://git-scm.com/docs/git-rebase\n.. _pip: https://pip.pypa.io/\n.. _personal access token: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token\n.. _pygit2: https://github.com/libgit2/pygit2\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://retrocookie.readthedocs.io/en/latest/usage.html\n',
-    'author': 'Claudio Jolowicz',
-    'author_email': 'mail@claudiojolowicz.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/cjolowicz/retrocookie',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov|
 
+.. |PyPI| image:: https://img.shields.io/pypi/v/retrocookie.svg
+   :target: https://pypi.org/project/retrocookie/
+   :alt: PyPI
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/retrocookie
+   :target: https://pypi.org/project/retrocookie
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/retrocookie
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/retrocookie/latest.svg?label=Read%20the%20Docs
+   :target: https://retrocookie.readthedocs.io/
+   :alt: Read the documentation at https://retrocookie.readthedocs.io/
+.. |Tests| image:: https://github.com/cjolowicz/retrocookie/workflows/Tests/badge.svg
+   :target: https://github.com/cjolowicz/retrocookie/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/cjolowicz/retrocookie/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/cjolowicz/retrocookie
+   :alt: Codecov
+
+
+Retrocookie updates Cookiecutter_ templates with changes from generated projects.
+
+When developing Cookiecutter templates,
+you often need to work in a generated project rather than the template itself.
+Reasons for this include the following:
+
+- You need to run the Continuous Integration suite for the generated project
+- Your development tools choke when running on the templated project
+
+Any changes you make in the generated project
+need to be backported into the template,
+carefully replacing expanded variables from ``cookiecutter.json`` by templating tags,
+and escaping any use of ``{{`` and ``}}``
+or other tokens with special meaning in Jinja.
+
+✨ Retrocookie helps you in this situation. ✨
+
+It is designed to fetch commits from the repository of a generated project,
+and import them into your Cookiecutter repository,
+rewriting them on the fly to insert templating tags,
+escape Jinja-special constructs,
+and place files in the template directory.
+
+Under the hood,
+Retrocookie rewrites the selected commits using git-filter-repo_,
+saving them to a temporary repository.
+It then fetches and cherry-picks the rewritten commits
+from the temporary repository into the Cookiecutter template,
+using pygit2_.
+
+Maybe you're thinking,
+how can this possibly work?
+One cannot reconstruct a Jinja template from its rendered output.
+However, simple replacements of template variables work well in practice
+when you're only importing a handful of commits at a time.
+
+**Important:**
+
+Retrocookie relies on a ``.cookiecutter.json`` file in the generated project
+to work out how to rewrite commits.
+This file is similar to the ``cookiecutter.json`` file in the template,
+but contains the specific values chosen during project generation.
+You can generate this file by putting it into the template directory in the Cookiecutter,
+with the following contents:
+
+.. code:: jinja
+
+   {{ cookiecutter | jsonify }}
+
+
+Requirements
+------------
+
+* Python 3.8+
+* git >= 2.22.0
+
+
+Installation
+------------
+
+You can install *Retrocookie* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install retrocookie
+
+Optionally, install the ``pr`` extra for the retrocookie-pr_ command:
+
+.. code:: console
+
+   $ pip install retrocookie[pr]
+
+
+Example
+-------
+
+Here's an example to demonstrate the general workflow.
+
+To start with, we clone the repository of your Cookiecutter template.
+For this example, I'll use my own `Hypermodern Python Cookiecutter`_.
+
+.. code:: console
+
+   $ git clone https://github.com/cjolowicz/cookiecutter-hypermodern-python
+
+Next, we'll create a project from the template,
+and set up a git repository for it:
+
+.. code:: console
+
+   $ cookiecutter --no-input cookiecutter-hypermodern-python
+   $ cd hypermodern-python
+   $ git init
+   $ git add .
+   $ git commit --message="Initial commit"
+
+Let's open a feature branch in the project repository,
+and make a fictitious change involving the default project name *hypermodern-python*:
+
+.. code:: console
+
+   $ git switch --create add-example
+   $ echo '# hypermodern-python' > EXAMPLE.md
+   $ git add EXAMPLE.md
+   $ git commit --message="Add example"
+
+Back in the Cookiecutter repository,
+we can now invoke retrocookie to import the changes from the feature branch:
+
+.. code:: console
+
+   $ cd ../cookiecutter-hypermodern-python
+   $ retrocookie --branch add-example --create ../hypermodern-python
+
+A ``git show`` in the Cookiecutter shows the file under the template directory,
+on a branch named as in the original repository,
+with the project name replaced by a Jinja tag:
+
+.. code:: diff
+
+   commit abb4f823b9f1760e3a678c927ec9797c0a40a9b6 (HEAD -> add-example)
+   Author: Your Name <your.name@example.com>
+   Date:   Fri Dec 4 23:40:41 2020 +0100
+
+       Add example
+
+   diff --git a/{{cookiecutter.project_name}}/EXAMPLE.md b/{{cookiecutter.project_name}}/EXAMPLE.md
+   new file mode 100644
+   index 0000000..a158618
+   --- /dev/null
+   +++ b/{{cookiecutter.project_name}}/EXAMPLE.md
+   @@ -0,0 +1 @@
+   +# {{cookiecutter.project_name}}
+
+
+Usage
+-----
+
+The basic form:
+
+.. code::
+
+   $ retrocookie <repository> [<commits>...]
+   $ retrocookie <repository> -b <branch> [--create]
+
+The ``<repository>`` is a filesystem path to the source repository.
+For ``<commits>``, see `gitrevisions(7)`__.
+
+__ https://git-scm.com/docs/gitrevisions
+
+Import ``HEAD`` from ``<repository>``:
+
+.. code::
+
+   $ retrocookie <repository>
+
+Import the last two commits:
+
+.. code::
+
+   $ retrocookie <repository> HEAD~2..
+
+Import by commit hash:
+
+.. code::
+
+   $ retrocookie <repository> 53268f7 6a3368a c0b4c6c
+
+Import commits from branch ``topic``:
+
+.. code::
+
+   $ retrocookie <repository> --branch=topic
+
+Equivalently:
+
+.. code::
+
+   $ retrocookie <repository> master..topic
+
+Import commits from ``topic`` into a branch with the same name:
+
+.. code::
+
+   $ retrocookie <repository> --branch=topic --create
+
+Equivalently, using short options:
+
+.. code::
+
+   $ retrocookie <repository> -cb topic
+
+Import commits from branch ``topic``, which was branched off ``1.0``:
+
+.. code::
+
+   $ retrocookie <repository> --branch=topic --upstream=1.0
+
+Equivalently:
+
+.. code::
+
+   $ retrocookie <repository> 1.0..topic
+
+Import ``HEAD`` into a new branch ``topic``:
+
+.. code::
+
+   $ retrocookie <repository> --create-branch=topic
+
+Please see the `Command-line Reference <Usage_>`_ for further details.
+
+
+.. _retrocookie-pr:
+
+Importing pull requests from generated projects with retrocookie-pr
+-------------------------------------------------------------------
+
+You can import pull requests from a generated project to the project template,
+assuming their repositories are on GitHub_.
+This requires activating the ``pr`` extra when installing with pip_:
+
+.. code::
+
+  $ pip install retrocookie[pr]
+
+The command ``retrocookie-pr`` has the basic form:
+
+.. code::
+
+   $ retrocookie-pr [-R <repository>] [<pr>...]
+   $ retrocookie-pr [-R <repository>] --user=<user>
+   $ retrocookie-pr [-R <repository>] --all
+
+Command-line arguments specify pull requests to import, by number or by branch.
+Pull requests from forks are currently not supported.
+
+Use the ``-R <repository>`` option to specify the GitHub repository of the generated project
+from which the pull requests should be imported.
+Provide the full name of the repository on GitHub in the form ``owner/name``.
+The owner can be omitted if the repository is owned by the authenticated user.
+This option can be omitted when the command is invoked from a local clone.
+
+You can also select pull requests by specifying the user that opened them, via the ``--user`` option.
+This is handy for importing automated pull requests, such as dependency updates from Dependabot_.
+
+Use the ``--all`` option to import all open pull requests in the generated project.
+
+You can update previously imported pull requests by specifying ``--force``.
+By default, ``retrocookie-pr`` refuses to overwrite existing pull requests.
+
+The command needs a `personal access token`_ to access the GitHub API.
+(This token is also used to push to the GitHub repository of the project template.)
+You will be prompted for the token when you invoke the command for the first time.
+On subsequent invocations, the token is read from the application cache.
+Alternatively, you can specify the token using the ``--token`` option or the ``GITHUB_TOKEN`` environment variable;
+both of these methods bypass the cache.
+
+Use the ``--open`` option to open each imported pull request in a web browser.
+
+Please see the `Command-line Reference <Usage_>`_ for further details.
+
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the MIT_ license,
+*Retrocookie* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _Dependabot: https://dependabot.com/
+.. _GitHub: https://github.com/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _MIT: http://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/
+.. _file an issue: https://github.com/cjolowicz/retrocookie/issues
+.. _git-filter-repo: https://github.com/newren/git-filter-repo
+.. _git rebase: https://git-scm.com/docs/git-rebase
+.. _pip: https://pip.pypa.io/
+.. _personal access token: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token
+.. _pygit2: https://github.com/libgit2/pygit2
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
+.. _Usage: https://retrocookie.readthedocs.io/en/latest/usage.html
 
-setup(**setup_kwargs)
```

