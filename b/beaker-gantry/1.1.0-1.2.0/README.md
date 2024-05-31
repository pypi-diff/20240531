# Comparing `tmp/beaker_gantry-1.1.0.tar.gz` & `tmp/beaker_gantry-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaker_gantry-1.1.0.tar", last modified: Wed May 29 19:56:55 2024, max compression
+gzip compressed data, was "beaker_gantry-1.2.0.tar", last modified: Fri May 31 03:08:17 2024, max compression
```

## Comparing `beaker_gantry-1.1.0.tar` & `beaker_gantry-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/beaker_gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.958855 beaker_gantry-1.1.0/gantry/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/gantry/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/follow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/beaker_gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/gantry/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/follow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/setup.cfg
```

### Comparing `beaker_gantry-1.1.0/LICENSE` & `beaker_gantry-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/PKG-INFO` & `beaker_gantry-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.1.0
+Version: 1.2.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beaker-py<2.0,>=1.26.11
+Requires-Dist: beaker-py<2.0,>=1.26.13
 Requires-Dist: GitPython<4.0,>=3.0
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: click-help-colors
 Requires-Dist: petname<3.0,>=2.6
 Requires-Dist: requests
 Requires-Dist: packaging
```

### Comparing `beaker_gantry-1.1.0/README.md` & `beaker_gantry-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/beaker_gantry.egg-info/PKG-INFO` & `beaker_gantry-1.2.0/beaker_gantry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.1.0
+Version: 1.2.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beaker-py<2.0,>=1.26.11
+Requires-Dist: beaker-py<2.0,>=1.26.13
 Requires-Dist: GitPython<4.0,>=3.0
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: click-help-colors
 Requires-Dist: petname<3.0,>=2.6
 Requires-Dist: requests
 Requires-Dist: packaging
```

### Comparing `beaker_gantry-1.1.0/beaker_gantry.egg-info/SOURCES.txt` & `beaker_gantry-1.2.0/beaker_gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/gantry/commands/config.py` & `beaker_gantry-1.2.0/gantry/commands/config.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/gantry/commands/list.py` & `beaker_gantry-1.2.0/gantry/commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, timedelta, timezone
 from itertools import islice
-from typing import Generator, Optional, Tuple
+from typing import Generator, List, Optional, Tuple
 
 import click
 from beaker import Beaker, Experiment, Task, Tasks
 from rich import print
 from rich.progress import Progress
 from rich.table import Table
 
@@ -54,27 +54,28 @@
     help="Only show your own experiments. Mutually exclusive with '--author'.",
 )
 @click.option(
     "-s",
     "--status",
     type=click.Choice(list(JobStatus)),
     help="Filter by status.",
+    multiple=True,
 )
 @click.option(
     "--max-age",
     type=int,
     default=Defaults.max_age,
     help=f"Maximum age of experiments, in days. Default: {Defaults.max_age}",
 )
 def list_cmd(
     workspace: Optional[str] = None,
     limit: int = Defaults.limit,
     author: Optional[str] = None,
     me: bool = False,
-    status: Optional[str] = None,
+    status: Optional[List[str]] = None,
     max_age: int = Defaults.max_age,
 ):
     """
     List gantry experiments.
     """
     beaker = Beaker.from_env(session=True)
 
@@ -90,15 +91,15 @@
         else:
             author = beaker.account.whoami().name
 
     with Progress(transient=True) as progress:
         task = progress.add_task("Collecting experiments...", total=limit)
         for exp, tasks in islice(
             iter_experiments(
-                beaker, workspace=workspace, author=author, status=status, max_age=max_age
+                beaker, workspace=workspace, author=author, statuses=status, max_age=max_age
             ),
             limit,
         ):
             table.add_row(
                 f"[b cyan]{exp.display_name}[/]\n[u i blue]{beaker.experiment.url(exp)}[/]",
                 exp.author.name,
                 exp.created.astimezone(tz=None).strftime("%I:%M %p on %a, %b %-d"),
@@ -112,15 +113,15 @@
 
 
 def iter_experiments(
     beaker: Beaker,
     *,
     workspace: Optional[str],
     author: Optional[str],
-    status: Optional[str],
+    statuses: Optional[List[str]],
     max_age: int,
 ) -> Generator[Tuple[Experiment, Tasks], None, None]:
     now = datetime.now(tz=timezone.utc).astimezone()
     for exp in beaker.workspace.iter_experiments(workspace=workspace):
         # Filter by age.
         age = now - exp.created.astimezone()
         if age > timedelta(days=max_age):
@@ -138,17 +139,17 @@
                     break
             else:
                 continue
 
         tasks = beaker.experiment.tasks(exp)
 
         # Maybe filter by status.
-        if status is not None:
+        if statuses:
             for task in tasks:
-                if get_status(task) == status:
+                if get_status(task) in statuses:
                     break
             else:
                 continue
 
         yield exp, tasks
```

### Comparing `beaker_gantry-1.1.0/gantry/commands/main.py` & `beaker_gantry-1.2.0/gantry/commands/main.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/gantry/commands/run.py` & `beaker_gantry-1.2.0/gantry/commands/run.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/gantry/entrypoint.sh` & `beaker_gantry-1.2.0/gantry/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/gantry/util.py` & `beaker_gantry-1.2.0/gantry/util.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.1.0/pyproject.toml` & `beaker_gantry-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 authors = [
     { name = "Allen Institute for Artificial Intelligence", email = "contact@allenai.org" },
     { name = "Pete Walsh", email = "petew@allenai.org" },
 ]
 license = {file = "LICENSE"}
 requires-python = ">3.7"
 dependencies = [
-    "beaker-py>=1.26.11,<2.0",
+    "beaker-py>=1.26.13,<2.0",
     "GitPython>=3.0,<4.0",
     "rich",
     "click",
     "click-help-colors",
     "petname>=2.6,<3.0",
     "requests",
     "packaging",
```

