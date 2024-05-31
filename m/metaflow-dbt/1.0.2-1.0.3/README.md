# Comparing `tmp/metaflow_dbt-1.0.2.tar.gz` & `tmp/metaflow_dbt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow_dbt-1.0.2.tar", last modified: Fri May 24 11:24:33 2024, max compression
+gzip compressed data, was "metaflow_dbt-1.0.3.tar", last modified: Fri May 31 10:33:51 2024, max compression
```

## Comparing `metaflow_dbt-1.0.2.tar` & `metaflow_dbt-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.743960 metaflow_dbt-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-24 11:24:33.743960 metaflow_dbt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.743960 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-24 11:24:33.000000 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 11:24:33.000000 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:24:33.000000 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 11:24:33.000000 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 11:24:33.000000 metaflow_dbt-1.0.2/metaflow_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.735960 metaflow_dbt-1.0.2/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/flow_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/config/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/config/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.739960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:24:33.743960 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/toplevel/mfextinit_dbt_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/toplevel/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:24:33.743960 metaflow_dbt-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 11:24:25.000000 metaflow_dbt-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.226795 metaflow_dbt-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-31 10:33:51.000000 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 10:33:51.000000 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:33:51.000000 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 10:33:51.000000 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 10:33:51.000000 metaflow_dbt-1.0.3/metaflow_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.218795 metaflow_dbt-1.0.3/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.218795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/flow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/config/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.218795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:33:51.222795 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/toplevel/mfextinit_dbt_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/toplevel/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:33:51.226795 metaflow_dbt-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-31 10:33:42.000000 metaflow_dbt-1.0.3/setup.py
```

### Comparing `metaflow_dbt-1.0.2/LICENSE` & `metaflow_dbt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/PKG-INFO` & `metaflow_dbt-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-dbt
-Version: 1.0.2
+Version: 1.0.3
 Summary: DBT extension for Metaflow
 Author: Outerbounds
 Author-email: help@outerbounds.co
 License: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `metaflow_dbt-1.0.2/README.md` & `metaflow_dbt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/metaflow_dbt.egg-info/PKG-INFO` & `metaflow_dbt-1.0.3/metaflow_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-dbt
-Version: 1.0.2
+Version: 1.0.3
 Summary: DBT extension for Metaflow
 Author: Outerbounds
 Author-email: help@outerbounds.co
 License: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `metaflow_dbt-1.0.2/metaflow_dbt.egg-info/SOURCES.txt` & `metaflow_dbt-1.0.3/metaflow_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py` & `metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/cmd/flow_generator.py` & `metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/cmd/flow_generator.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py` & `metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py` & `metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,32 @@
     headline = "Missing DBT Profiles configuration"
 
 
 class MissingStateStorage(MetaflowException):
     headline = "Missing DBT State Storage configuration"
 
 
+class MissingMacroName(MetaflowException):
+    headline = "Missing macro name for run-operation"
+
+
 class DbtStepDecorator(StepDecorator):
     """
     Decorator to execute DBT models before a step execution begins.
 
 
     Parameters
     ----------
     command: str, optional. Default 'run'
         DBT command to execute. Default is 'run'.
-        Supported commands are: run, seed, test and build
+        Supported commands are: run, seed, test, build and run-operation
+    macro : str, optional
+        name for macro to run. Required with the 'run-operation' command
+    args : str, optional
+        args to pass for macro. Only used with the 'run-operation' commmand.
     project_dir: str, optional
         Path to the DBT project that contains a 'dbt_project.yml'.
         If not specified, the current folder and parent folders will be tried.
     models: List[str], optional
         List of model name(s) to run. All models will be run by default if no model name is provided.
     select: List[str], optional
         List of object name(s) to run.
@@ -49,14 +57,16 @@
         a configuration dictionary that will be translated into a valid profiles.yml for the dbt CLI.
     """
 
     name = "_dbt"
 
     defaults = {
         "command": "run",
+        "macro": None,
+        "args": None,
         "project_dir": None,
         "models": None,
         "select": None,
         "exclude": None,
         "target": None,
         "profiles": None,
         "generate_docs": False,  # TODO: This could also be true by default
@@ -74,17 +84,23 @@
                 "You must provide profiles configuration for the DBT decorator.\n"
                 "Either provide a dictionary for the 'profiles=' attribute "
                 "or create a 'profiles.yml' file in the flow folder."
             )
 
         cmd = self.attributes["command"]
 
-        if cmd not in ["run", "seed", "test", "build"]:
+        if cmd not in ["run", "seed", "test", "build", "run-operation"]:
             raise CommandNotSupported(f"command '{cmd}' is not supported.")
 
+        if cmd == "run-operation" and self.attributes["macro"] is None:
+            raise MissingMacroName(
+                "Specify the macro name to run with the 'macro=' option on the DBT decorator for the *%s* step."
+                % step_name
+            )
+
         # Do we need persisted state due to the selectors or not?
         self.use_state = self.attributes["models"] and any(
             any(sel in val for val in self.attributes["models"])
             for sel in ["result:", "state:"]
         )
 
         self.ds_type = flow_datastore.TYPE
@@ -113,14 +129,16 @@
         # so that consecutive executions have a known location to look in for previous state
         # TODO: cover projects.
         # TODO: evaluate prefix for sufficient uniqueness
         state_prefix = f"{flow.name}/{step_func.__name__}"
         build_cache_prefix = f"{flow.name}/{self.run_id}"
         with DBTExecutor(
             models=self.attributes["models"],
+            macro=self.attributes["macro"],
+            args=self.attributes["args"],
             select=self.attributes["select"],
             exclude=self.attributes["exclude"],
             project_dir=self.attributes["project_dir"],
             target=self.attributes["target"],
             profiles=self.attributes["profiles"],
             state_prefix=state_prefix if self.use_state else None,
             build_cache_prefix=build_cache_prefix,
```

### Comparing `metaflow_dbt-1.0.2/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py` & `metaflow_dbt-1.0.3/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,27 +40,31 @@
 # TODO: There is a choice to utilize the Python library provided by DBT for performing the run, and accessing run results as well.
 # This would introduce a heavy dependency for the decorator use case, which can be completely avoided with the custom implementation
 # via calling the CLI via subprocess only at the point when execution needs to happen. Decide on the approach after PoC is complete.
 class DBTExecutor:
     def __init__(
         self,
         models: List[str] = None,
+        macro: str = None,
+        args: str = None,
         select: List[str] = None,
         exclude: List[str] = None,
         project_dir: str = None,
         target: str = None,
         profiles: Dict = None,
         state_prefix: str = None,
         build_cache_prefix: str = None,
         ds_type=None,
     ):
 
         self.models = " ".join(models) if models is not None else None
         self.select = " ".join(select) if select is not None else None
         self.exclude = " ".join(exclude) if exclude is not None else None
+        self.macro = macro
+        self.args = args
         self.project_dir = project_dir
         self.target = target
         self.bin = which("./dbt") or which("dbt")
         if self.bin is None:
             raise DBTExecutionFailed("Can not find DBT binary. Please install DBT")
         self.profiles = profiles
         conf = DBTProjectConfig(project_dir)
@@ -118,14 +122,15 @@
     def command(self, cmd: str):
         supported = {
             "run": self.run,
             "parse": self.parse,
             "seed": self.seed,
             "build": self.build,
             "test": self.test,
+            "run-operation": self.run_operation,
             "docs": self.generate_docs,
         }
         if cmd not in supported:
             raise UnsupportedCommand(
                 'The command "%s" is not supported by the DBT Extension' % cmd
             )
 
@@ -168,14 +173,29 @@
         if self.select is not None:
             args.extend(["--select", self.select])
         if self.target is not None:
             args.extend(["--target", self.target])
 
         return self._call("build", args)
 
+    def run_operation(self) -> str:
+        if self.macro is None:
+            raise DBTExecutionFailed(
+                "run-operation requires specifying the name of a macro to be executed."
+            )
+        args = [self.macro, "--fail-fast", "--no-use-colors"]
+        if self.args is not None:
+            args.extend(["--args", self.args])
+        if self.project_dir is not None:
+            args.extend(["--project-dir", self.project_dir])
+        if self.target is not None:
+            args.extend(["--target", self.target])
+
+        return self._call("run-operation", args)
+
     def parse(self) -> str:
         args = ["--fail-fast", "--no-use-colors"]
         if self.project_dir is not None:
             args.extend(["--project-dir", self.project_dir])
         if self.models is not None:
             args.extend(["--models", self.models])
         if self.select is not None:
```

### Comparing `metaflow_dbt-1.0.2/setup.py` & `metaflow_dbt-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "1.0.2"
+version = "1.0.3"
 
 setup(
     name="metaflow-dbt",
     version=version,
     description="DBT extension for Metaflow",
     long_description=open("README.md").read(),
     author="Outerbounds",
```

