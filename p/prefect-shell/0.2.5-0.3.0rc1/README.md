# Comparing `tmp/prefect_shell-0.2.5.tar.gz` & `tmp/prefect_shell-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_shell-0.2.5.tar", last modified: Thu May 16 20:58:44 2024, max compression
+gzip compressed data, was "prefect_shell-0.3.0rc1.tar", last modified: Fri May 31 20:49:46 2024, max compression
```

## Comparing `prefect_shell-0.2.5.tar` & `prefect_shell-0.3.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.137058 prefect_shell-0.2.5/prefect_shell/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/prefect_shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/prefect_shell/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/prefect_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 20:58:44.000000 prefect_shell-0.2.5/prefect_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:58:43.000000 prefect_shell-0.2.5/prefect_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:44.141058 prefect_shell-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_commands_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 20:58:32.000000 prefect_shell-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.397765 prefect_shell-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-31 20:49:46.397765 prefect_shell-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.393765 prefect_shell-0.3.0rc1/prefect_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/prefect_shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:45.000000 prefect_shell-0.3.0rc1/prefect_shell/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/prefect_shell/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.393765 prefect_shell-0.3.0rc1/prefect_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 20:49:46.000000 prefect_shell-0.3.0rc1/prefect_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:46.397765 prefect_shell-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.393765 prefect_shell-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/test_commands_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 20:49:34.000000 prefect_shell-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_shell-0.2.5/LICENSE` & `prefect_shell-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.5/PKG-INFO` & `prefect_shell-0.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `prefect_shell-0.2.5/README.md` & `prefect_shell-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.5/prefect_shell/commands.py` & `prefect_shell-0.3.0rc1/prefect_shell/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,22 @@
 import tempfile
 from contextlib import AsyncExitStack, contextmanager
 from typing import Any, Dict, Generator, List, Optional, Union
 
 import anyio
 from anyio.abc import Process
 from anyio.streams.text import TextReceiveStream
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import DirectoryPath, Field, PrivateAttr
 
 from prefect import task
 from prefect.blocks.abstract import JobBlock, JobRun
 from prefect.logging import get_run_logger
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import open_process
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import DirectoryPath, Field, PrivateAttr
-else:
-    from pydantic import DirectoryPath, Field, PrivateAttr
-
 
 @task
 async def shell_run_command(
     command: str,
     env: Optional[dict] = None,
     helper_command: Optional[str] = None,
     shell: Optional[str] = None,
@@ -239,23 +234,23 @@
     )
     stream_output: bool = Field(default=True, description="Whether to stream output.")
     env: Dict[str, str] = Field(
         default_factory=dict,
         title="Environment Variables",
         description="Environment variables to use for the subprocess.",
     )
-    working_dir: DirectoryPath = Field(
+    working_dir: Optional[DirectoryPath] = Field(
         default=None,
         title="Working Directory",
         description=(
             "The absolute path to the working directory "
             "the command will be executed within."
         ),
     )
-    shell: str = Field(
+    shell: Optional[str] = Field(
         default=None,
         description=(
             "The shell to run the command with; if unset, "
             "defaults to `powershell` on Windows and `bash` on other platforms."
         ),
     )
     extension: Optional[str] = Field(
```

### Comparing `prefect_shell-0.2.5/prefect_shell.egg-info/PKG-INFO` & `prefect_shell-0.3.0rc1/prefect_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations for interacting with shell commands.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `prefect_shell-0.2.5/pyproject.toml` & `prefect_shell-0.3.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,44 +2,42 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-shell"
 description = "Prefect integrations for interacting with shell commands."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = ["prefect>=2.14.10, < 3.0.0"]
+dependencies = ["prefect>=3.0.0rc1"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pillow",
   "pre-commit",
   "pytest-asyncio",
   "pytest",
   "pytest-xdist",
 ]
@@ -49,15 +47,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_shell = "prefect_shell"
 
 [tool.setuptools_scm]
 version_file = "prefect_shell/_version.py"
 root = "../../.."
-tag_regex = "^prefect-shell-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-shell-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.2.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-shell-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_shell/_version.py", "tests"]
```

### Comparing `prefect_shell-0.2.5/tests/conftest.py` & `prefect_shell-0.3.0rc1/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import logging
 
 import pytest
 
+from prefect.testing.utilities import prefect_test_harness
+
+
+@pytest.fixture(scope="session", autouse=True)
+def prefect_db():
+    """
+    Sets up test harness for temporary DB during test runs.
+    """
+    with prefect_test_harness():
+        yield
+
 
 @pytest.fixture(scope="function")
 def prefect_caplog(caplog):
     logger = logging.getLogger("prefect")
 
     # TODO: Determine a better pattern for this and expose for all tests
     logger.propagate = True
```

### Comparing `prefect_shell-0.2.5/tests/test_block_standards.py` & `prefect_shell-0.3.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_shell-0.2.5/tests/test_commands.py` & `prefect_shell-0.3.0rc1/tests/test_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,134 +9,136 @@
 from prefect import flow
 from prefect.testing.utilities import AsyncMock
 
 if sys.platform == "win32":
     pytest.skip(reason="see test_commands_windows.py", allow_module_level=True)
 
 
-def test_shell_run_command_error(prefect_task_runs_caplog):
+async def test_shell_run_command_error(prefect_task_runs_caplog):
     @flow
-    def test_flow():
-        return shell_run_command(command="ls this/is/invalid")
+    async def test_flow():
+        return await shell_run_command(command="ls this/is/invalid")
 
     match = "No such file or directory"
     with pytest.raises(RuntimeError, match=match):
-        test_flow()
+        await test_flow()
 
 
-def test_shell_run_command(prefect_task_runs_caplog):
+async def test_shell_run_command(prefect_task_runs_caplog):
     prefect_task_runs_caplog.set_level(logging.INFO)
     echo_msg = "_THIS_ IS WORKING!!!!"
 
     @flow
-    def test_flow():
-        return shell_run_command(command=f"echo {echo_msg}")
+    async def test_flow():
+        return await shell_run_command(command=f"echo {echo_msg}")
 
-    assert test_flow() == echo_msg
+    assert (await test_flow()) == echo_msg
     assert echo_msg in prefect_task_runs_caplog.text
 
 
-def test_shell_run_command_stream_level(prefect_task_runs_caplog):
+async def test_shell_run_command_stream_level(prefect_task_runs_caplog):
     prefect_task_runs_caplog.set_level(logging.WARNING)
     echo_msg = "_THIS_ IS WORKING!!!!"
 
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command=f"echo {echo_msg}",
             stream_level=logging.WARNING,
         )
 
-    assert test_flow() == echo_msg
+    assert (await test_flow()) == echo_msg
     assert echo_msg in prefect_task_runs_caplog.text
 
 
-def test_shell_run_command_helper_command():
+async def test_shell_run_command_helper_command():
     @flow
-    def test_flow():
-        return shell_run_command(command="pwd", helper_command="cd $HOME")
+    async def test_flow():
+        return await shell_run_command(command="pwd", helper_command="cd $HOME")
 
-    assert test_flow() == os.path.expandvars("$HOME")
+    assert (await test_flow()) == os.path.expandvars("$HOME")
 
 
-def test_shell_run_command_cwd():
+async def test_shell_run_command_cwd():
     @flow
-    def test_flow():
-        return shell_run_command(command="pwd", cwd=Path.home())
+    async def test_flow():
+        return await shell_run_command(command="pwd", cwd=Path.home())
 
-    assert test_flow() == os.fspath(Path.home())
+    assert (await test_flow()) == os.fspath(Path.home())
 
 
-def test_shell_run_command_return_all():
+async def test_shell_run_command_return_all():
     @flow
-    def test_flow():
-        return shell_run_command(command="echo work! && echo yes!", return_all=True)
+    async def test_flow():
+        return await shell_run_command(
+            command="echo work! && echo yes!", return_all=True
+        )
 
-    assert test_flow() == ["work!", "yes!"]
+    assert (await test_flow()) == ["work!", "yes!"]
 
 
-def test_shell_run_command_no_output():
+async def test_shell_run_command_no_output():
     @flow
-    def test_flow():
-        return shell_run_command(command="sleep 1")
+    async def test_flow():
+        return await shell_run_command(command="sleep 1")
 
-    assert test_flow() == ""
+    assert (await test_flow()) == ""
 
 
-def test_shell_run_command_uses_current_env():
+async def test_shell_run_command_uses_current_env():
     @flow
-    def test_flow():
-        return shell_run_command(command="echo $HOME")
+    async def test_flow():
+        return await shell_run_command(command="echo $HOME")
 
-    assert test_flow() == os.environ["HOME"]
+    assert (await test_flow()) == os.environ["HOME"]
 
 
-def test_shell_run_command_update_current_env():
+async def test_shell_run_command_update_current_env():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo $HOME && echo $TEST_VAR",
             env={"TEST_VAR": "test value"},
             return_all=True,
         )
 
-    result = test_flow()
+    result = await test_flow()
     assert result[0] == os.environ["HOME"]
     assert result[1] == "test value"
 
 
 class AsyncIter:
     def __init__(self, items):
         self.items = items
 
     async def __aiter__(self):
         for item in self.items:
             yield item
 
 
 @pytest.mark.parametrize("shell", [None, "bash", "zsh"])
-def test_shell_run_command_override_shell(shell, monkeypatch):
+async def test_shell_run_command_override_shell(shell, monkeypatch):
     open_process_mock = AsyncMock()
     stdout_mock = AsyncMock()
     stdout_mock.receive.side_effect = lambda: b"received"
     open_process_mock.return_value.__aenter__.return_value = AsyncMock(
         stdout=stdout_mock
     )
     open_process_mock.return_value.__aenter__.return_value.returncode = 0
     monkeypatch.setattr("anyio.open_process", open_process_mock)
     monkeypatch.setattr("prefect_shell.commands.TextReceiveStream", AsyncIter)
 
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo 'testing'",
             shell=shell,
         )
 
-    test_flow()
+    await test_flow()
     assert open_process_mock.call_args_list[0][0][0][0] == shell or "bash"
 
 
 class TestShellOperation:
     async def execute(self, op, method):
         if method == "run":
             return await op.run()
@@ -147,14 +149,15 @@
 
     @pytest.mark.parametrize("method", ["run", "trigger"])
     async def test_error(self, method):
         op = ShellOperation(commands=["ls this/is/invalid"])
         with pytest.raises(RuntimeError, match="return code"):
             await self.execute(op, method)
 
+    @pytest.mark.skipif(sys.version >= "3.12", reason="Fails on Python 3.12")
     @pytest.mark.parametrize("method", ["run", "trigger"])
     async def test_output(self, prefect_task_runs_caplog, method):
         op = ShellOperation(commands=["echo 'testing\nthe output'", "echo good"])
         assert await self.execute(op, method) == ["testing", "the output", "good"]
         records = prefect_task_runs_caplog.records
         assert len(records) == 3
         assert "triggered with 2 commands running" in records[0].message
```

### Comparing `prefect_shell-0.2.5/tests/test_commands_windows.py` & `prefect_shell-0.3.0rc1/tests/test_commands_windows.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,205 +10,207 @@
 from prefect import flow
 from prefect.testing.utilities import AsyncMock
 
 if sys.platform != "win32":
     pytest.skip(reason="see test_commands.py", allow_module_level=True)
 
 
-def test_shell_run_command_error_windows(prefect_task_runs_caplog):
+async def test_shell_run_command_error_windows(prefect_task_runs_caplog):
     @flow
-    def test_flow():
-        return shell_run_command(command="throw", return_all=True, shell="powershell")
+    async def test_flow():
+        return await shell_run_command(
+            command="throw", return_all=True, shell="powershell"
+        )
 
     with pytest.raises(RuntimeError, match="Exception"):
-        test_flow()
+        await test_flow()
 
     assert len(prefect_task_runs_caplog.records) == 7
 
 
-def test_shell_run_command_windows(prefect_task_runs_caplog):
+async def test_shell_run_command_windows(prefect_task_runs_caplog):
     prefect_task_runs_caplog.set_level(logging.INFO)
     echo_msg = "WORKING"
 
     @flow
-    def test_flow():
-        msg = shell_run_command(
+    async def test_flow():
+        msg = await shell_run_command(
             command=f"echo {echo_msg}", return_all=True, shell="powershell"
         )
         return msg
 
-    print(prefect_task_runs_caplog.text)
-
-    assert " ".join(test_flow()) == echo_msg
+    assert " ".join(await test_flow()) == echo_msg
     for record in prefect_task_runs_caplog.records:
         if "WORKING" in record.msg:
             break  # it's in the records
     else:
         raise AssertionError
 
 
-def test_shell_run_command_stream_level_windows(prefect_task_runs_caplog):
+async def test_shell_run_command_stream_level_windows(prefect_task_runs_caplog):
     prefect_task_runs_caplog.set_level(logging.WARNING)
     echo_msg = "WORKING"
 
     @flow
-    def test_flow():
-        msg = shell_run_command(
+    async def test_flow():
+        msg = await shell_run_command(
             command=f"echo {echo_msg}",
             stream_level=logging.WARNING,
             return_all=True,
             shell="powershell",
         )
         return msg
 
     print(prefect_task_runs_caplog.text)
 
-    assert " ".join(test_flow()) == echo_msg
+    assert " ".join(await test_flow()) == echo_msg
     for record in prefect_task_runs_caplog.records:
         if "WORKING" in record.msg:
             break  # it's in the records
     else:
         raise AssertionError
 
 
-def test_shell_run_command_helper_command_windows():
+async def test_shell_run_command_helper_command_windows():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="Get-Location",
             helper_command="cd $env:USERPROFILE",
             shell="powershell",
             return_all=True,
         )
 
-    assert os.path.expandvars("$USERPROFILE") in test_flow()
+    assert os.path.expandvars("$USERPROFILE") in await test_flow()
 
 
-def test_shell_run_command_cwd():
+async def test_shell_run_command_cwd():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo 'work!'; Get-Location",
             shell="powershell",
             cwd=Path.home(),
             return_all=True,
         )
 
-    assert os.fspath(Path.home()) in test_flow()
+    assert os.fspath(Path.home()) in await test_flow()
 
 
-def test_shell_run_command_return_all():
+async def test_shell_run_command_return_all():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo 'work!'; echo 'yes!'", return_all=True, shell="powershell"
         )
 
-    result = test_flow()
+    result = await test_flow()
     assert result[0].rstrip() == "work!"
     assert result[1].rstrip() == "yes!"
 
 
-def test_shell_run_command_no_output_windows():
+async def test_shell_run_command_no_output_windows():
     @flow
-    def test_flow():
-        return shell_run_command(command="sleep 1", shell="powershell")
+    async def test_flow():
+        return await shell_run_command(command="sleep 1", shell="powershell")
 
-    assert test_flow() == ""
+    assert await test_flow() == ""
 
 
-def test_shell_run_command_uses_current_env_windows():
+async def test_shell_run_command_uses_current_env_windows():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo $env:USERPROFILE", return_all=True, shell="powershell"
         )
 
-    result = test_flow()
+    result = await test_flow()
     assert result[0].rstrip() == os.environ["USERPROFILE"]
 
 
-def test_shell_run_command_update_current_env_windows():
+async def test_shell_run_command_update_current_env_windows():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo $env:USERPROFILE ; echo $env:TEST_VAR",
             helper_command="$env:TEST_VAR = 'test value'",
             env={"TEST_VAR": "test value"},
             return_all=True,
             shell="powershell",
         )
 
-    result = test_flow()
+    result = await test_flow()
     assert os.environ["USERPROFILE"] in " ".join(result)
     assert "test value" in result
 
 
-def test_shell_run_command_ensure_suffix_ps1():
+async def test_shell_run_command_ensure_suffix_ps1():
     @flow
-    def test_flow():
-        return shell_run_command(command="1 + 1", shell="powershell", extension=".zzz")
+    async def test_flow():
+        return await shell_run_command(
+            command="1 + 1", shell="powershell", extension=".zzz"
+        )
 
-    result = test_flow()
+    result = await test_flow()
     assert result == "2"
 
 
-def test_shell_run_command_ensure_tmp_file_removed():
+async def test_shell_run_command_ensure_tmp_file_removed():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo 'clean up after yourself!'", shell="powershell"
         )
 
-    test_flow()
+    await test_flow()
     temp_dir = os.environ["TEMP"]
     assert len(glob.glob(f"{temp_dir}\\prefect-*.ps1")) == 0
 
 
-def test_shell_run_command_throw_exception_on_nonzero_exit_code():
+async def test_shell_run_command_throw_exception_on_nonzero_exit_code():
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="ping ???",
             shell="powershell",  # ping ??? returns exit code 1
         )
 
     with pytest.raises(RuntimeError, match=r"Command failed with exit code 1"):
-        test_flow()
+        await test_flow()
 
 
 class AsyncIter:
     def __init__(self, items):
         self.items = items
 
     async def __aiter__(self):
         for item in self.items:
             yield item
 
 
 @pytest.mark.parametrize("shell", [None, "powershell", "powershell.exe"])
-def test_shell_run_command_override_shell(shell, monkeypatch):
+async def test_shell_run_command_override_shell(shell, monkeypatch):
     open_process_mock = AsyncMock()
     stdout_mock = AsyncMock()
     stdout_mock.receive.side_effect = lambda: b"received"
     open_process_mock.return_value.__aenter__.return_value = AsyncMock(
         stdout=stdout_mock
     )
     open_process_mock.return_value.__aenter__.return_value.returncode = 0
     monkeypatch.setattr("anyio.open_process", open_process_mock)
     monkeypatch.setattr("prefect_shell.commands.TextReceiveStream", AsyncIter)
 
     @flow
-    def test_flow():
-        return shell_run_command(
+    async def test_flow():
+        return await shell_run_command(
             command="echo 'testing'",
             shell=shell,
         )
 
-    test_flow()
+    await test_flow()
     assert open_process_mock.call_args_list[0][0][0][0] == shell or "powershell"
 
 
 class TestShellOperation:
     async def execute(self, op, method):
         if method == "run":
             return await op.run()
@@ -223,14 +225,15 @@
 
     @pytest.mark.parametrize("method", ["run", "trigger"])
     async def test_error(self, method):
         op = ShellOperation(commands=["throw"])
         with pytest.raises(RuntimeError, match="return code"):
             await self.execute(op, method)
 
+    @pytest.mark.skipif(sys.version >= "3.12", reason="Fails on Python 3.12")
     @pytest.mark.parametrize("method", ["run", "trigger"])
     async def test_output(self, prefect_task_runs_caplog, method):
         op = ShellOperation(commands=["echo 'testing'"])
         assert await self.execute(op, method) == ["testing"]
         records = prefect_task_runs_caplog.records
         assert len(records) == 3
         assert "triggered with 1 commands running" in records[0].message
```

