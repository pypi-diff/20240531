# Comparing `tmp/ppatch-0.0.4b1.tar.gz` & `tmp/ppatch-0.0.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppatch-0.0.4b1.tar", last modified: Wed May  8 11:57:42 2024, max compression
+gzip compressed data, was "ppatch-0.0.4b2.tar", last modified: Fri May 31 13:09:50 2024, max compression
```

## Comparing `ppatch-0.0.4b1.tar` & `ppatch-0.0.4b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.4b1/LICENSE
--rw-r--r--   0        0        0      649 2024-04-11 09:30:45.056874 ppatch-0.0.4b1/README.md
--rw-r--r--   0        0        0      565 2024-05-08 11:57:42.585274 ppatch-0.0.4b1/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-13 07:54:26.926711 ppatch-0.0.4b1/src/ppatch/__init__.py
--rw-r--r--   0        0        0       28 2024-05-08 10:07:04.820507 ppatch-0.0.4b1/src/ppatch/__main__.py
--rw-r--r--   0        0        0      281 2024-04-11 08:42:18.488669 ppatch-0.0.4b1/src/ppatch/app.py
--rw-r--r--   0        0        0     1693 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/commands/apply.py
--rw-r--r--   0        0        0     4625 2024-05-08 11:54:14.559072 ppatch-0.0.4b1/src/ppatch/commands/auto.py
--rw-r--r--   0        0        0     1644 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/commands/get.py
--rw-r--r--   0        0        0      172 2024-04-11 08:42:18.909675 ppatch-0.0.4b1/src/ppatch/commands/help.py
--rw-r--r--   0        0        0      870 2024-04-11 09:03:57.269830 ppatch-0.0.4b1/src/ppatch/commands/show.py
--rw-r--r--   0        0        0     4782 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/commands/trace.py
--rw-r--r--   0        0        0      759 2024-04-11 09:04:40.900874 ppatch-0.0.4b1/src/ppatch/config.py
--rw-r--r--   0        0        0     1499 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/model.py
--rw-r--r--   0        0        0     2300 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/utils/common.py
--rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.4b1/src/ppatch/utils/parse.py
--rw-r--r--   0        0        0     9810 2024-05-08 10:07:04.829507 ppatch-0.0.4b1/src/ppatch/utils/resolve.py
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 ppatch-0.0.4b1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.4b2/LICENSE
+-rw-r--r--   0        0        0      649 2024-04-11 09:30:45.056874 ppatch-0.0.4b2/README.md
+-rw-r--r--   0        0        0      565 2024-05-31 13:09:50.446207 ppatch-0.0.4b2/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-03-13 07:54:26.926711 ppatch-0.0.4b2/src/ppatch/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-08 10:07:04.820507 ppatch-0.0.4b2/src/ppatch/__main__.py
+-rw-r--r--   0        0        0      357 2024-05-31 13:03:42.078119 ppatch-0.0.4b2/src/ppatch/app.py
+-rw-r--r--   0        0        0     1693 2024-05-08 10:07:04.829507 ppatch-0.0.4b2/src/ppatch/commands/apply.py
+-rw-r--r--   0        0        0     4918 2024-05-31 13:06:29.455938 ppatch-0.0.4b2/src/ppatch/commands/auto.py
+-rw-r--r--   0        0        0     1644 2024-05-08 10:07:04.829507 ppatch-0.0.4b2/src/ppatch/commands/get.py
+-rw-r--r--   0        0        0      172 2024-04-11 08:42:18.909675 ppatch-0.0.4b2/src/ppatch/commands/help.py
+-rw-r--r--   0        0        0      870 2024-04-11 09:03:57.269830 ppatch-0.0.4b2/src/ppatch/commands/show.py
+-rw-r--r--   0        0        0     4782 2024-05-08 10:07:04.829507 ppatch-0.0.4b2/src/ppatch/commands/trace.py
+-rw-r--r--   0        0        0      759 2024-04-11 09:04:40.900874 ppatch-0.0.4b2/src/ppatch/config.py
+-rw-r--r--   0        0        0     1783 2024-05-31 13:06:29.385937 ppatch-0.0.4b2/src/ppatch/model.py
+-rw-r--r--   0        0        0     2678 2024-05-31 13:06:29.415938 ppatch-0.0.4b2/src/ppatch/utils/common.py
+-rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.4b2/src/ppatch/utils/parse.py
+-rw-r--r--   0        0        0     9810 2024-05-08 10:07:04.829507 ppatch-0.0.4b2/src/ppatch/utils/resolve.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 ppatch-0.0.4b2/PKG-INFO
```

### Comparing `ppatch-0.0.4b1/LICENSE` & `ppatch-0.0.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/README.md` & `ppatch-0.0.4b2/README.md`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/pyproject.toml` & `ppatch-0.0.4b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ppatch"
-version = "0.0.4b1"
+version = "0.0.4b2"
 description = "Universal tool to analysis patches, bulit for Linux Kernel."
 authors = [
     { name = "jingfelix", email = "jingfelix@outlook.com" },
 ]
 dependencies = [
     "typer[all]>=0.9.0",
     "pydantic>=2.5.3",
```

### Comparing `ppatch-0.0.4b1/src/ppatch/commands/apply.py` & `ppatch-0.0.4b2/src/ppatch/commands/apply.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/commands/auto.py` & `ppatch-0.0.4b2/src/ppatch/commands/auto.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,56 +2,62 @@
 
 import typer
 
 from ppatch.app import app
 from ppatch.commands.get import getpatches
 from ppatch.commands.trace import trace
 from ppatch.config import settings
-from ppatch.model import Diff, File
+from ppatch.model import CommandResult, CommandType, Diff, File
 from ppatch.utils.common import process_title, unpack
 from ppatch.utils.parse import parse_patch
 from ppatch.utils.resolve import apply_change
 
 
 @app.command()
 def auto(filename: str, output: str = typer.Option("", "--output", "-o")):
     """Automatic do ANYTHING"""
     if not os.path.exists(filename):
         typer.echo(f"Warning: {filename} not found!")
-        return
 
-    if not os.path.isdir(output):
-        typer.echo(f"Warning: dir {output} not found!")
-        return
+        return CommandResult(
+            type=CommandType.AUTO,
+        )
+
+    if os.path.isdir(output):
+        output = os.path.join(output, "auto.patch")
 
     content = ""
     with open(filename, mode="r", encoding="utf-8") as (f):
         content = f.read()
 
     parser = parse_patch(content)
     fail_file_list: dict[str, list[int]] = {}
     raw_diffes = parser.diff  # TODO: patchobj 应该换成 Pydantic Model，然后注意换掉 unpack() 的调用
     for diff in raw_diffes:
         diff = Diff(**unpack(diff))
         target_file = diff.header.new_path  # 这里注意是 new_path 还是 old_path
         origin_file = File(file_path=target_file)
 
+        # 执行 Reverse，确定失败的 Hunk
         apply_result = apply_change(
             diff.changes, origin_file.line_list, reverse=True, fuzz=3
         )
 
         if len(apply_result.failed_hunk_list) != 0:
             typer.echo(f"Failed hunk in {target_file}")
             fail_file_list[target_file] = [
                 hunk.index for hunk in apply_result.failed_hunk_list
             ]
 
     if len(fail_file_list) == 0:
         typer.echo("No failed patch")
-        return
+
+        return CommandResult(
+            type=CommandType.AUTO,
+        )
 
     subject = parser.subject
     diffes: list = []
     for file_name, hunk_list in fail_file_list.items():
         typer.echo(
             f"{len(hunk_list)} hunk(s) failed in {file_name} with subject {subject}"
         )
@@ -72,15 +78,18 @@
                 text = f.read()
                 if parse_patch(text).subject == subject:
                     sha_for_sure = sha
                     break
 
         if sha_for_sure is None:
             typer.echo(f"Error: No patch found for {file_name}")
-            return
+
+            return CommandResult(
+                type=CommandType.AUTO,
+            )
 
         typer.echo(f"Found correspond patch {sha_for_sure} to {file_name}")
         typer.echo(f"Hunk list: {hunk_list}")
 
         conflict_list = trace(
             file_name, from_commit=sha_for_sure, flag_hunk_list=hunk_list
         )
@@ -127,13 +136,17 @@
             tofile="b/" + file_name,
         )
 
         for line in diffes_:
             diffes.append(line + "\n" if not line.endswith("\n") else line)
 
     with open(
-        os.path.join(output, "auto.patch"),
+        os.path.join(output),
         mode="w",
         encoding="utf-8",
     ) as (f):
         f.write("".join(diffes))
-        typer.echo("Patch file generated: auto.patch")
+        typer.echo(f"Patch file generated: {output}")
+
+    return CommandResult(
+        type=CommandType.AUTO,
+    )
```

### Comparing `ppatch-0.0.4b1/src/ppatch/commands/get.py` & `ppatch-0.0.4b2/src/ppatch/commands/get.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/commands/show.py` & `ppatch-0.0.4b2/src/ppatch/commands/show.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/commands/trace.py` & `ppatch-0.0.4b2/src/ppatch/commands/trace.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/config.py` & `ppatch-0.0.4b2/src/ppatch/config.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/model.py` & `ppatch-0.0.4b2/src/ppatch/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 class Line(BaseModel):
     index: int
@@ -58,7 +59,22 @@
     text: str
 
 
 class ApplyResult(BaseModel):
     new_line_list: list[Line] = []
     conflict_hunk_num_list: list[int] = []
     failed_hunk_list: list[Hunk] = []
+
+
+class CommandType(Enum):
+    APPLY = "apply"
+    AUTO = "auto"
+    GET = "get"
+    HELP = "help"
+    SHOW = "show"
+    TRACE = "trace"
+    UNKNOWN = "unknown"
+
+
+class CommandResult(BaseModel):
+    type: CommandType
+    content: dict | list | str | None = None
```

### Comparing `ppatch-0.0.4b1/src/ppatch/utils/common.py` & `ppatch-0.0.4b2/src/ppatch/utils/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import subprocess
 
+import typer
+
+from ppatch.model import CommandResult, CommandType
+
 # import typer
 # import whatthepatch
 
 # from ppatch.model import Line
 # from .resolve import apply_change
 
 
@@ -74,7 +78,19 @@
         return [unpack(value) for value in obj]
     elif isnamedtupleinstance(obj):
         return {key: unpack(value) for key, value in obj._asdict().items()}
     elif isinstance(obj, tuple):
         return tuple(unpack(value) for value in obj)
     else:
         return obj
+
+
+def post_executed(executed_command_result: CommandResult) -> None:
+    """Executed command result callback function"""
+
+    typer.echo(f"Executed {executed_command_result.type}")
+
+    match executed_command_result.type:
+        case CommandType.AUTO:
+            clean_repo()
+        case _:
+            pass
```

### Comparing `ppatch-0.0.4b1/src/ppatch/utils/parse.py` & `ppatch-0.0.4b2/src/ppatch/utils/parse.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/src/ppatch/utils/resolve.py` & `ppatch-0.0.4b2/src/ppatch/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.4b1/PKG-INFO` & `ppatch-0.0.4b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppatch
-Version: 0.0.4b1
+Version: 0.0.4b2
 Summary: Universal tool to analysis patches, bulit for Linux Kernel.
 Author-Email: jingfelix <jingfelix@outlook.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: pydantic>=2.5.3
 Requires-Dist: whatthepatch>=1.0.5
```

