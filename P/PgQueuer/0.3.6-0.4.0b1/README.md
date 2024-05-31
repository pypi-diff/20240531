# Comparing `tmp/pgqueuer-0.3.6.tar.gz` & `tmp/pgqueuer-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.6.tar", last modified: Mon May 20 20:52:45 2024, max compression
+gzip compressed data, was "pgqueuer-0.4.0b1.tar", last modified: Fri May 31 20:18:33 2024, max compression
```

## Comparing `pgqueuer-0.3.6.tar` & `pgqueuer-0.4.0b1.tar`

### file list

```diff
@@ -1,44 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.151635 pgqueuer-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.114762 pgqueuer-0.4.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/benchmark.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/database_initialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/docs/queuemanager.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:18:33.126762 pgqueuer-0.4.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.118762 pgqueuer-0.4.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 20:18:33.000000 pgqueuer-0.4.0b1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:18:33.122762 pgqueuer-0.4.0b1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 20:18:24.000000 pgqueuer-0.4.0b1/tools/ex.py
```

### Comparing `pgqueuer-0.3.6/.github/workflows/ci.yml` & `pgqueuer-0.4.0b1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/.github/workflows/linting.yml` & `pgqueuer-0.4.0b1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/.github/workflows/release.yml` & `pgqueuer-0.4.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/.gitignore` & `pgqueuer-0.4.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/CONTRIBUTING.md` & `pgqueuer-0.4.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/LICENSE` & `pgqueuer-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/pyproject.toml` & `pgqueuer-0.4.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,19 @@
     "mypy-extensions",
     "mypy",
     "pytest-asyncio",
     "pytest",
     "ruff",
     "types-tabulate",
 ]
+docs = [
+    "myst-parser",
+    "sphinx",
+    "sphinx-rtd-theme",
+]
 
 [tool.setuptools_scm]
 write_to = "src/_version.py"
 
 [tool.ruff]
 line-length = 88
 [tool.ruff.lint]
```

### Comparing `pgqueuer-0.3.6/src/PgQueuer/cli.py` & `pgqueuer-0.4.0b1/src/PgQueuer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,14 +175,27 @@
         action="store_true",
         help=(
             "Prints the SQL statements that would be executed without "
             "actually applying any changes to the database."
         ),
     )
 
+    subparsers.add_parser(
+        "upgrade",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        parents=[common_arguments],
+    ).add_argument(
+        "--dry-run",
+        action="store_true",
+        help=(
+            "Prints the SQL statements that would be executed without "
+            "actually applying any changes to the database."
+        ),
+    )
+
     dashboardparser = subparsers.add_parser(
         "dashboard",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[common_arguments],
     )
     dashboardparser.add_argument(
         "-i",
@@ -248,14 +261,18 @@
                 print(QueryBuilder().create_install_query())
                 if not parsed.dry_run:
                     await queries.install()
             case "uninstall":
                 print(QueryBuilder().create_uninstall_query())
                 if not parsed.dry_run:
                     await queries.uninstall()
+            case "upgrade":
+                print("\n".join(QueryBuilder().create_upgrade_queries()))
+                if not parsed.dry_run:
+                    await queries.upgrade()
             case "dashboard":
                 await fetch_and_display(
                     queries,
                     parsed.interval,
                     parsed.tail,
                     parsed.table_format,
                 )
```

### Comparing `pgqueuer-0.3.6/src/PgQueuer/listeners.py` & `pgqueuer-0.4.0b1/src/PgQueuer/listeners.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/src/PgQueuer/models.py` & `pgqueuer-0.4.0b1/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/src/PgQueuer/qm.py` & `pgqueuer-0.4.0b1/src/PgQueuer/qm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import dataclasses
 import functools
 from datetime import timedelta
 from typing import (
     TYPE_CHECKING,
     Awaitable,
     Callable,
@@ -106,45 +107,64 @@
 
         return register
 
     async def run(
         self,
         dequeue_timeout: timedelta = timedelta(seconds=30),
         batch_size: int = 10,
+        retry_timer: timedelta | None = None,
     ) -> None:
         """
         Continuously listens for events and dispatches jobs. Manages connections and
         tasks, logs timeouts, and resets connections upon termination.
+
+        Parameters:
+            - dequeue_timeout: The timeout duration for waiting to dequeue jobs.
+            Defaults to 30 seconds.
+            - batch_size : The number of jobs to retrieve in each batch. Defaults to 10.
+            - retry_timer: If specified, selects jobs that have been in 'picked' status
+            for longer than the specified retry timer duration. If `None`, the timeout
+            job checking is skipped.
         """
+
+        if not (await self.queries.has_updated_column()):
+            raise RuntimeError(
+                f"The {self.queries.qb.settings.queue_table} table is missing the "
+                "updated column, please run 'python3 -m PgQueuer upgrade'"
+            )
+
         async with (
             self.pool.acquire() as connection,
             TaskManager() as tm,
         ):
             listener = await initialize_event_listener(connection, self.channel)  # type: ignore[arg-type]
 
             while self.alive:
                 while self.alive and (
                     jobs := await self.queries.dequeue(
                         batch_size=batch_size,
                         entrypoints=set(self.registry.keys()),
+                        retry_timer=retry_timer,
                     )
                 ):
                     for job in jobs:
                         tm.add(asyncio.create_task(self._dispatch(job)))
+                        with contextlib.suppress(asyncio.QueueEmpty):
+                            listener.get_nowait()
 
-                    try:
-                        await asyncio.wait_for(
-                            listener.get(),
-                            timeout=dequeue_timeout.total_seconds(),
-                        )
-                    except asyncio.TimeoutError:
-                        logger.debug(
-                            "Timeout after %r without receiving an event.",
-                            dequeue_timeout,
-                        )
+                try:
+                    await asyncio.wait_for(
+                        listener.get(),
+                        timeout=dequeue_timeout.total_seconds(),
+                    )
+                except asyncio.TimeoutError:
+                    logger.debug(
+                        "Timeout after %r without receiving an event.",
+                        dequeue_timeout,
+                    )
 
             connection.remove_termination_listener(_critical_termination_listener)
             await connection.reset()
 
     async def _dispatch(self, job: Job) -> None:
         """
         Handles asynchronous job dispatch. Logs exceptions, updates job status,
```

### Comparing `pgqueuer-0.3.6/src/PgQueuer/queries.py` & `pgqueuer-0.4.0b1/src/PgQueuer/queries.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import os
-from typing import Final
+from datetime import timedelta
+from typing import Final, Generator
 
 import asyncpg
 
 from . import models
 
 
 def add_prefix(string: str) -> str:
@@ -99,26 +100,29 @@
         """
 
         return f"""
     CREATE TYPE {self.settings.queue_status_type} AS ENUM ('queued', 'picked');
     CREATE TABLE {self.settings.queue_table} (
         id SERIAL PRIMARY KEY,
         priority INT NOT NULL,
-        created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
+        created TIMESTAMP WITH TIME ZONE DEFAULT NOW() NOT NULL,
+        updated TIMESTAMP WITH TIME ZONE DEFAULT NOW() NOT NULL,
         status {self.settings.queue_status_type} NOT NULL,
         entrypoint TEXT NOT NULL,
         payload BYTEA
     );
-    CREATE INDEX ON {self.settings.queue_table} (priority ASC, id DESC)
+    CREATE INDEX {self.settings.queue_table}_priority_id_id1_idx ON {self.settings.queue_table} (priority ASC, id DESC)
         INCLUDE (id) WHERE status = 'queued';
+    CREATE INDEX {self.settings.queue_table}_updated_id_id1_idx ON {self.settings.queue_table} (updated ASC, id DESC)
+        INCLUDE (id) WHERE status = 'picked';
 
     CREATE TYPE {self.settings.statistics_table_status_type} AS ENUM ('exception', 'successful');
     CREATE TABLE {self.settings.statistics_table} (
         id SERIAL PRIMARY KEY,
-        created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT DATE_TRUNC('sec', CURRENT_TIMESTAMP at time zone 'UTC'),
+        created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT DATE_TRUNC('sec', NOW() at time zone 'UTC'),
         count BIGINT NOT NULL,
         priority INT NOT NULL,
         time_in_queue INTERVAL NOT NULL,
         status {self.settings.statistics_table_status_type} NOT NULL,
         entrypoint TEXT NOT NULL
     );
     CREATE UNIQUE INDEX {self.settings.statistics_table}_unique_count ON {self.settings.statistics_table} (
@@ -192,26 +196,47 @@
     def create_dequeue_query(self) -> str:
         """
         Generates the SQL query string to insert a new job into the queue.
         This query sets the job status to 'queued' and includes parameters for priority,
         entrypoint, and payload.
         """
         return f"""
-    WITH next_job AS (
+    WITH next_job_queued AS (
         SELECT id
         FROM {self.settings.queue_table}
-        WHERE status = 'queued' AND entrypoint = ANY($2)
+        WHERE
+                entrypoint = ANY($2)
+            AND status = 'queued'
         ORDER BY priority DESC, id ASC
         FOR UPDATE SKIP LOCKED
         LIMIT $1
     ),
+    next_job_retry AS (
+        SELECT id
+        FROM {self.settings.queue_table}
+        WHERE
+                entrypoint = ANY($2)
+            AND status = 'picked'
+            AND ($3::interval IS NOT NULL AND updated < NOW() - $3::interval)
+        ORDER BY updated DESC, id ASC
+        FOR UPDATE SKIP LOCKED
+        LIMIT $1
+    ),
+    combined_jobs AS (
+        SELECT DISTINCT id
+        FROM (
+            SELECT id FROM next_job_queued
+            UNION ALL
+            SELECT id FROM next_job_retry WHERE $3::interval IS NOT NULL
+        ) AS combined
+    ),
     updated AS (
         UPDATE {self.settings.queue_table}
-        SET status = 'picked'
-        WHERE id = ANY(SELECT id FROM next_job)
+        SET status = 'picked', updated = NOW()
+        WHERE id = ANY(SELECT id FROM combined_jobs)
         RETURNING *
     )
     SELECT * FROM updated ORDER BY priority DESC, id ASC
     """
 
     def create_enqueue_query(self) -> str:
         """
@@ -337,14 +362,27 @@
         priority,
         status
     FROM {self.settings.statistics_table}
     ORDER BY id DESC
     LIMIT $1
     """
 
+    def create_upgrade_queries(self) -> Generator[str, None, None]:
+        yield f"ALTER TABLE {self.settings.queue_table} ADD COLUMN IF NOT EXISTS updated TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT NOW();"  # noqa: E501
+        yield f"CREATE INDEX {self.settings.queue_table}_updated_id_id1_idx ON {self.settings.queue_table} (updated ASC, id DESC) INCLUDE (id) WHERE status = 'picked';"  # noqa: E501
+
+    def create_has_column_query(self) -> str:
+        return """
+        SELECT EXISTS (
+            SELECT FROM information_schema.columns
+            WHERE table_schema = current_schema()
+                AND table_name = $1
+                AND column_name = $2
+            );"""
+
 
 @dataclasses.dataclass
 class Queries:
     """
     Handles operations related to job queuing such as
     enqueueing, dequeueing, and querying the size of the queue.
     """
@@ -367,27 +405,39 @@
         """
         await self.pool.execute(self.qb.create_uninstall_query())
 
     async def dequeue(
         self,
         batch_size: int,
         entrypoints: set[str],
+        retry_timer: timedelta | None = None,
     ) -> list[models.Job]:
         """
-        Retrieves and updates the next 'queued' job to 'picked'
-        status, ensuring no two jobs with the same entrypoint
-        are picked simultaneously.
+        Retrieves and updates the next 'queued' job to 'picked' status,
+        ensuring no two jobs with the same entrypoint are picked simultaneously.
+
+        Parameters:
+        - batch_size: The number of jobs to retrieve. Must be greater than one (1).
+        - entrypoints: A set of entrypoints to filter the jobs.
+        - retry_timer: If specified, selects jobs that have been in 'picked' status for
+            longer than the specified retry-timer duration. If `None`, the retry-timer
+            checking is skipped.
         """
+
         if batch_size < 1:
-            raise ValueError("Batch size must be greter then one (1)")
+            raise ValueError("Batch size must be greater or equal to one (1)")
+
+        if retry_timer and retry_timer < timedelta(seconds=0):
+            raise ValueError("Retry timer must be a non-negative timedelta")
 
         rows = await self.pool.fetch(
             self.qb.create_dequeue_query(),
             batch_size,
             entrypoints,
+            retry_timer,
         )
         return [models.Job.model_validate(dict(row)) for row in rows]
 
     async def enqueue(
         self,
         entrypoint: str | list[str],
         payload: bytes | None | list[bytes] | list[None] | list[bytes | None],
@@ -469,7 +519,19 @@
         )
 
     async def log_statistics(self, tail: int) -> list[models.LogStatistics]:
         return [
             models.LogStatistics.model_validate(dict(x))
             for x in await self.pool.fetch(self.qb.create_log_statistics_query(), tail)
         ]
+
+    async def upgrade(self) -> None:
+        async with self.pool.acquire() as conn, conn.transaction():
+            for query in self.qb.create_upgrade_queries():
+                await conn.execute(query)
+
+    async def has_updated_column(self) -> bool:
+        return await self.pool.fetchval(
+            self.qb.create_has_column_query(),
+            self.qb.settings.queue_table,
+            "updated",
+        )
```

### Comparing `pgqueuer-0.3.6/src/PgQueuer/tm.py` & `pgqueuer-0.4.0b1/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/test/conftest.py` & `pgqueuer-0.4.0b1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/test/db/Dockerfile` & `pgqueuer-0.4.0b1/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/test/test_qm.py` & `pgqueuer-0.4.0b1/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/test/test_queries.py` & `pgqueuer-0.4.0b1/test/test_queries.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from datetime import timedelta
 
 import asyncpg
 import pytest
 from PgQueuer import models, queries
 
 
 @pytest.mark.parametrize("N", (1, 2, 64))
@@ -176,7 +177,57 @@
         batch_size=10,
     ):
         for job in next_jobs:
             jobs.append(job)
             await q.log_job(job, status="successful")
 
     assert jobs == sorted(jobs, key=lambda x: x.priority, reverse=True)
+
+
+@pytest.mark.parametrize("N", (1, 2, 64))
+async def test_queue_retry_timer(
+    pgpool: asyncpg.Pool,
+    N: int,
+    retry_timer: timedelta = timedelta(seconds=0.1),
+) -> None:
+    q = queries.Queries(pgpool)
+    jobs = list[models.Job]()
+
+    await q.enqueue(
+        ["placeholder"] * N,
+        [f"{n}".encode() for n in range(N)],
+        list(range(N)),
+    )
+
+    # Pick all jobs, and mark then as "in progress"
+    while _ := await q.dequeue(batch_size=10, entrypoints={"placeholder"}):
+        ...
+    assert len(await q.dequeue(batch_size=10, entrypoints={"placeholder"})) == 0
+
+    # Sim. slow entrypoint function.
+    await asyncio.sleep(retry_timer.total_seconds())
+
+    # Re-fetch, should get the same number of jobs as queued (N).
+    while next_jobs := await q.dequeue(
+        entrypoints={"placeholder"},
+        batch_size=10,
+        retry_timer=retry_timer,
+    ):
+        jobs.extend(next_jobs)
+
+    assert len(jobs) == N
+
+
+async def test_queue_retry_timer_negative_raises(pgpool: asyncpg.Pool) -> None:
+    with pytest.raises(ValueError):
+        await queries.Queries(pgpool).dequeue(
+            entrypoints={"placeholder"},
+            batch_size=10,
+            retry_timer=-timedelta(seconds=0.001),
+        )
+
+    with pytest.raises(ValueError):
+        await queries.Queries(pgpool).dequeue(
+            entrypoints={"placeholder"},
+            batch_size=10,
+            retry_timer=timedelta(seconds=-0.001),
+        )
```

### Comparing `pgqueuer-0.3.6/test/test_tm.py` & `pgqueuer-0.4.0b1/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.6/tools/benchmark.py` & `pgqueuer-0.4.0b1/tools/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,34 +26,32 @@
     try:
         yield lambda: timedelta(seconds=((done or time.perf_counter()) - enter))
     finally:
         done = time.perf_counter()
 
 
 async def consumer(qm: QueueManager, batch_size: int) -> float:
-    cnt = 0
+    cnt = count()
 
     @qm.entrypoint("asyncfetch")
     async def asyncfetch(job: Job) -> None:
-        nonlocal cnt
-        cnt += 1
+        next(cnt)
         if job.payload is None:
             qm.alive = False
 
     @qm.entrypoint("syncfetch")
     def syncfetch(job: Job) -> None:
-        nonlocal cnt
-        cnt += 1
+        next(cnt)
         if job.payload is None:
             qm.alive = False
 
     with execution_timer() as elapsed:
         await qm.run(batch_size=batch_size)
 
-    return cnt / elapsed().total_seconds()
+    return (next(cnt) - 1) / elapsed().total_seconds()
 
 
 async def producer(
     alive: asyncio.Event,
     queries: Queries,
     batch_size: int,
     cnt: count,
@@ -68,15 +66,15 @@
 async def main() -> None:
     parser = argparse.ArgumentParser(description="PGQueuer benchmark tool.")
 
     parser.add_argument(
         "-t",
         "--timer",
         type=lambda x: timedelta(seconds=float(x)),
-        default=timedelta(seconds=30),
+        default=timedelta(seconds=15),
         help="Run the benchmark for a specified number of seconds. Default is 30.",
     )
 
     parser.add_argument(
         "-dc",
         "--dequeue",
         type=int,
@@ -98,16 +96,16 @@
         default=1,
         help="Number of concurrent enqueue workers. Default is 1.",
     )
     parser.add_argument(
         "-ecbs",
         "--enqueue-batch-size",
         type=int,
-        default=15,
-        help="Batch size for enqueue workers. Default is 15.",
+        default=20,
+        help="Batch size for enqueue workers. Default is 30.",
     )
     args = parser.parse_args()
 
     print(f"""Settings:
 Timer:                  {args.timer.total_seconds()} seconds
 Dequeue:                {args.dequeue}
 Dequeue Batch Size:     {args.dequeue_batch_size}
```

