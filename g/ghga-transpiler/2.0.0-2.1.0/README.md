# Comparing `tmp/ghga_transpiler-2.0.0.tar.gz` & `tmp/ghga_transpiler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_transpiler-2.0.0.tar", last modified: Fri Dec  8 09:47:48 2023, max compression
+gzip compressed data, was "ghga_transpiler-2.1.0.tar", last modified: Fri May 31 12:15:21 2024, max compression
```

## Comparing `ghga_transpiler-2.0.0.tar` & `ghga_transpiler-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.006366 ghga_transpiler-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/src/ghga_transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/src/ghga_transpiler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/config/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/src/ghga_transpiler/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/src/ghga_transpiler/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2023-12-08 09:47:47.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-08 09:47:48.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 09:47:47.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-08 09:47:47.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-08 09:47:48.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 09:47:48.000000 ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 09:47:48.010366 ghga_transpiler-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/tests/test_convert_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/tests/test_create_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-12-08 09:47:40.000000 ghga_transpiler-2.0.0/tests/test_process_workbook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.153774 ghga_transpiler-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.153774 ghga_transpiler-2.1.0/src/ghga_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/src/ghga_transpiler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/config/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/src/ghga_transpiler/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/src/ghga_transpiler/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 12:15:21.000000 ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:21.157774 ghga_transpiler-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/tests/test_convert_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/tests/test_create_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-31 12:15:17.000000 ghga_transpiler-2.1.0/tests/test_process_workbook.py
```

### Comparing `ghga_transpiler-2.0.0/LICENSE` & `ghga_transpiler-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_transpiler-2.0.0/PKG-INFO` & `ghga_transpiler-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ghga_transpiler
-Version: 2.0.0
+Version: 2.1.0
 Summary: GHGA-Transpiler - excel to JSON converter
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-transpiler
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer~=0.9.0
+Requires-Dist: typer>=0.12
 Requires-Dist: openpyxl==3.*,>=3.1.2
 Requires-Dist: defusedxml==0.*,>=0.7
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: semver==3.*
```

### Comparing `ghga_transpiler-2.0.0/README.md` & `ghga_transpiler-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/__init__.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+
+"""Entrypoint of the package"""
 
-"""Short description of package"""  # Please adapt to package
+from ghga_transpiler.cli import cli
 
-from importlib.metadata import version
 
-from openpyxl.xml import DEFUSEDXML
+def run():
+    """Run the application."""
+    cli()
 
-__version__ = version(__package__)
 
-if not DEFUSEDXML:
-    raise RuntimeError(
-        "The 'defusedxml' package must be present to safely run ghga-transpiler."
-    )
+if __name__ == "__main__":
+    run()
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/__main__.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
 
-"""Entrypoint of the package"""
-
-from ghga_transpiler.cli import cli
-
+"""GHGA metadata transpiler"""
 
-def run():
-    """Run the application."""
-    cli()
+from openpyxl.xml import DEFUSEDXML
 
+__version__ = "2.1.0"
 
-if __name__ == "__main__":
-    run()
+if not DEFUSEDXML:
+    raise RuntimeError(
+        "The 'defusedxml' package must be present to safely run ghga-transpiler."
+    )
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/cli.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 """CLI-specific wrappers around core functions."""
+
 import sys
 from pathlib import Path
-from typing import Optional
 
 import typer
 
 from . import __version__, io
 from .config.exceptions import UnknownVersionError
 from .core import InvalidSematicVersion, convert_workbook
 
@@ -39,15 +40,15 @@
     spread_sheet: Path = typer.Argument(
         ...,
         exists=True,
         help="The path to input file (XLSX)",
         dir_okay=False,
         readable=True,
     ),
-    output_file: Optional[Path] = typer.Argument(
+    output_file: Path | None = typer.Argument(
         None, help="The path to output file (JSON).", dir_okay=False
     ),
     force: bool = typer.Option(
         False, "--force", "-f", help="Override output file if it exists."
     ),
     version: bool = typer.Option(
         False,
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/config/__init__.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
+
+"""Module to load workbook configurations and convert it to transpiler config"""
 
-"""Module to load workbook configurations and convert it to transpiler config """
 from .config import Config, load_config  # noqa
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/config/config.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """Module to process config file"""
 
 from collections import Counter
+from collections.abc import Callable
 from importlib import resources
-from typing import Callable, Optional
 
 import yaml
 from pydantic import BaseModel, model_validator
 
 from .exceptions import DuplicatedName, UnknownVersionError
 
 
@@ -36,26 +37,26 @@
     transformations: dict[str, Callable] = {}
 
 
 class WorksheetSettings(BaseModel):
     """A data model for the per-worksheet settings of a transpiler config"""
 
     name: str
-    header_row: Optional[int] = None
-    start_row: Optional[int] = None
-    start_column: Optional[int] = None
-    end_column: Optional[int] = None
-    transformations: Optional[dict[str, Callable]] = None
+    header_row: int | None = None
+    start_row: int | None = None
+    start_column: int | None = None
+    end_column: int | None = None
+    transformations: dict[str, Callable] | None = None
 
 
 class Worksheet(BaseModel):
     """A data model for worksheets in the transpiler config"""
 
     sheet_name: str
-    settings: Optional[WorksheetSettings]
+    settings: WorksheetSettings | None
 
 
 class Config(BaseModel):
     """A data model for the transpiler config"""
 
     ghga_metadata_version: str
     default_settings: DefaultSettings
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/config/exceptions.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/config/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """Module to collect custom exceptions"""
 
 
 class DuplicatedName(ValueError):
     """Raised when worksheet names are not unique in the config file"""
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/configs/__init__.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/configs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/core.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """This module contains functionalities for processing excel sheets into json object."""
+
+from collections.abc import Callable
 from importlib import resources
-from typing import Callable, Optional, Union
 
 import semver
 from openpyxl import Workbook
 
 from . import config
 
 
@@ -55,34 +57,34 @@
     def major_minor_version(self):
         """Returns only major and minor version numbers"""
         return f"{self.wb_version.major}.{self.wb_version.minor}"
 
 
 def get_worksheet_rows(
     worksheet,
-    min_row: Union[int, None],
+    min_row: int | None,
     max_row: int,
-    min_col: Union[int, None],
-    max_col: Union[int, None],
+    min_col: int | None,
+    max_col: int | None,
 ) -> list:
     """Function to create a list of rows of a worksheet"""
     return list(
         row
         for row in worksheet.iter_rows(
             min_row, max_row, min_col, max_col, values_only=True
         )
         if not all(cell is None for cell in row)
     )
 
 
 def get_header(
     worksheet,
-    header_row: Union[int, None],
-    min_col: Union[int, None],
-    max_col: Union[int, None],
+    header_row: int | None,
+    min_col: int | None,
+    max_col: int | None,
 ) -> list[str]:
     """Function to return a list column names of a worksheet"""
     return list(
         cell.value
         for row in worksheet.iter_rows(header_row, header_row, min_col, max_col)
         for cell in row
     )
@@ -91,23 +93,23 @@
 def convert_rows(header, rows) -> list[dict]:
     """Function to return list of dictionaries, rows as worksheet row values and
     column names as keys
     """
     return [
         {
             key: value
-            for key, value in zip(header, row)
+            for key, value in zip(header, row, strict=False)
             if value is not None and value != ""
         }
         for row in rows
     ]
 
 
 def transform_rows(
-    rows: list[dict], transformations: Optional[dict[str, Callable]]
+    rows: list[dict], transformations: dict[str, Callable] | None
 ) -> list[dict]:
     """Transforms row values if it is applicable with a given function"""
     transformed = []
     for row in rows:
         transformed_row = {}
         for key, value in row.items():
             if transformations and key in transformations:
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/io.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """IO related functionality"""
 
 import json
 import sys
 from importlib import resources
 from pathlib import Path
-from typing import Optional, TextIO
+from typing import TextIO
 
 from openpyxl import load_workbook
 
 from .core import GHGAWorkbook
 
 
 def read_workbook(
@@ -35,15 +36,15 @@
 
 
 def _write_json(data: dict, file: TextIO):
     """Write the data to the specified file in JSON format"""
     json.dump(obj=data, fp=file, ensure_ascii=False, indent=4)
 
 
-def write_json(data: dict, path: Optional[Path], force: bool) -> None:
+def write_json(data: dict, path: Path | None, force: bool) -> None:
     """Write the data provided as a dictionary to the specified output path or
     to stdout if the path is None.
     """
     if path is None:
         _write_json(data, sys.stdout)
     elif path.exists() and not force:
         raise FileExistsError(f"File already exists: {path}")
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler/transformations.py` & `ghga_transpiler-2.1.0/src/ghga_transpiler/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """Module containing transformation functions"""
 
-from typing import Callable
+from collections.abc import Callable
 
 
 def split_by_semicolon(value: str) -> list[str]:
     """Splits a string by semicolon"""
     return [elem.strip() for elem in value.split(";")]
 
 
@@ -31,15 +32,15 @@
 
 def to_attributes() -> Callable:
     """Returns a function to convert string to attributes"""
 
     def split_one(value: str) -> dict:
         """Returns a dictionary with key, value as keys, splitted string as values"""
         splitted = (elem.strip() for elem in value.split("="))
-        return dict(zip(("key", "value"), splitted))
+        return dict(zip(("key", "value"), splitted, strict=False))
 
     def split_mult(value: str) -> list[dict]:
         """Converts string to attributes"""
         return [split_one(elem) for elem in split_by_semicolon(value)]
 
     return split_mult
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/PKG-INFO` & `ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
-Name: ghga-transpiler
-Version: 2.0.0
+Name: ghga_transpiler
+Version: 2.1.0
 Summary: GHGA-Transpiler - excel to JSON converter
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-transpiler
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer~=0.9.0
+Requires-Dist: typer>=0.12
 Requires-Dist: openpyxl==3.*,>=3.1.2
 Requires-Dist: defusedxml==0.*,>=0.7
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: semver==3.*
```

### Comparing `ghga_transpiler-2.0.0/src/ghga_transpiler.egg-info/SOURCES.txt` & `ghga_transpiler-2.1.0/src/ghga_transpiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-2.0.0/tests/test_convert_workbook.py` & `ghga_transpiler-2.1.0/tests/test_convert_workbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """Tests for converting the workbook"""
 
 from ghga_transpiler import io
 from ghga_transpiler.core import convert_workbook
 
 from .fixtures.test_data_objects.conversion_data import EXPECTED_CONVERSION
```

### Comparing `ghga_transpiler-2.0.0/tests/test_create_config.py` & `ghga_transpiler-2.1.0/tests/test_create_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """Tests for creating the config"""
 
 from ghga_transpiler.config.config import (
     Config,
     DefaultSettings,
     Worksheet,
```

### Comparing `ghga_transpiler-2.0.0/tests/test_io.py` & `ghga_transpiler-2.1.0/tests/test_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 
 """IO functionality tests"""
 
 import json
 
 import pytest
```

### Comparing `ghga_transpiler-2.0.0/tests/test_process_workbook.py` & `ghga_transpiler-2.1.0/tests/test_process_workbook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
-#
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-#
+
 #     http://www.apache.org/licenses/LICENSE-2.0
-#
+
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
 """Unit tests for core functions"""
 
 import pytest
 import semver
 
 from ghga_transpiler.core import GHGAWorkbook, InvalidSematicVersion
```

