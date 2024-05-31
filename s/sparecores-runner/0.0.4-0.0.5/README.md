# Comparing `tmp/sparecores_runner-0.0.4.tar.gz` & `tmp/sparecores_runner-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_runner-0.0.4.tar", last modified: Wed May 15 21:38:05 2024, max compression
+gzip compressed data, was "sparecores_runner-0.0.5.tar", last modified: Fri May 31 14:34:21 2024, max compression
```

## Comparing `sparecores_runner-0.0.4.tar` & `sparecores_runner-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/src/sc_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/src/sc_runner/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/resources/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-15 21:38:01.000000 sparecores_runner-0.0.4/src/sc_runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:38:05.343559 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 21:38:05.000000 sparecores_runner-0.0.4/src/sparecores_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:34:21.733614 sparecores_runner-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-31 14:34:21.733614 sparecores_runner-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:34:21.733614 sparecores_runner-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:34:21.729614 sparecores_runner-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:34:21.729614 sparecores_runner-0.0.5/src/sc_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:34:21.729614 sparecores_runner-0.0.5/src/sc_runner/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/resources/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-31 14:34:17.000000 sparecores_runner-0.0.5/src/sc_runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:34:21.733614 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 14:34:21.000000 sparecores_runner-0.0.5/src/sparecores_runner.egg-info/top_level.txt
```

### Comparing `sparecores_runner-0.0.4/LICENSE` & `sparecores_runner-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.4/PKG-INFO` & `sparecores_runner-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-runner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Start cloud instances.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-runner
 Project-URL: issues, https://github.com/SpareCores/sc-runner/issues
 Project-URL: documentation, https://sparecores.github.io/sc-runner/
 Project-URL: homepage, https://sparecores.com
```

### Comparing `sparecores_runner-0.0.4/pyproject.toml` & `sparecores_runner-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-runner"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">= 3.9"
 dependencies = [
     "click",
     "pulumi",
     "pulumi-aws",
     "sparecores-crawler",
     "sparecores-data",
```

### Comparing `sparecores_runner-0.0.4/src/sc_runner/cli.py` & `sparecores_runner-0.0.5/src/sc_runner/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
 @add_click_opts(runner.pulumi_stack)
 @cli.group()
 def destroy(**kwargs):
     pass
 
 
+@add_click_opts(runner.pulumi_stack)
+@cli.group()
+def cancel(**kwargs):
+    pass
+
+
 for vendor in data.vendors():
     if vendor not in resources.supported_vendors:
         # exclude not yet supported vendors
         continue
 
     @create.command(name=vendor)
     @click.pass_context
@@ -60,15 +66,22 @@
     @destroy.command(name=vendor)
     @click.pass_context
     def destroy_resources(ctx, **kwargs):
         pulumi_opts = ctx.parent.params
         vendor = ctx.command.name
         runner.destroy(vendor, pulumi_opts, kwargs)
 
+    @cancel.command(name=vendor)
+    @click.pass_context
+    def cancel_resources(ctx, **kwargs):
+        pulumi_opts = ctx.parent.params
+        vendor = ctx.command.name
+        runner.cancel(vendor, pulumi_opts, kwargs)
 
     # add click options from the resource method's annotated argument list
     add_click_opts(getattr(resources, f"{resources.PREFIX}{vendor}"))(create_resources)
     add_click_opts(getattr(resources, f"{resources.PREFIX}{vendor}"))(destroy_resources)
+    add_click_opts(getattr(resources, f"{resources.PREFIX}{vendor}"))(cancel_resources)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `sparecores_runner-0.0.4/src/sc_runner/data.py` & `sparecores_runner-0.0.5/src/sc_runner/data.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.4/src/sc_runner/resources/aws.py` & `sparecores_runner-0.0.5/src/sc_runner/resources/aws.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.4/src/sc_runner/resources/base.py` & `sparecores_runner-0.0.5/src/sc_runner/resources/base.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.4/src/sc_runner/runner.py` & `sparecores_runner-0.0.5/src/sc_runner/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def pulumi_stack(
     pulumi_program: Callable,
     project_name: Annotated[str, DefaultOpt(["--project-name"], type=str, help="Pulumi project name")] = os.environ.get("PULUMI_PROJECT_NAME", "runner"),
     work_dir: Annotated[str, DefaultOpt(["--work-dir"], type=str, help="Pulumi work dir")] = os.environ.get("PULUMI_WORK_DIR", "/data/workdir"),
     pulumi_home: Annotated[str, DefaultOpt(["--pulumi-home"], type=str, help="Pulumi home")] = os.environ.get("PULUMI_HOME", "/data/.pulumi"),
-    backend_url: Annotated[str, DefaultOpt(["--pulumi-home"], type=str, help="Pulumi backend URL")] = os.environ.get("PULUMI_BACKEND_URL", "file:///data/backend"),
+    pulumi_backend_url: Annotated[str, DefaultOpt(["--pulumi-backend-url"], type=str, help="Pulumi backend URL")] = os.environ.get("PULUMI_BACKEND_URL", "file:///data/backend"),
     stack_name: Annotated[
         str,
         click.Option(["--stack-name"], type=str, help="Pulumi stack name, defaults to {vendor}.{region}.{zone}.{instance_id} or similar")]
     = os.environ.get("PULUMI_STACK_NAME", ""),
 ):
     stack = create_or_select_stack(
         stack_name=stack_name,
@@ -36,15 +36,15 @@
         program=pulumi_program,
         opts=LocalWorkspaceOptions(
             work_dir=work_dir,
             pulumi_home=pulumi_home,
             project_settings=ProjectSettings(
                 name=project_name,
                 runtime="python",
-                backend=ProjectBackend(backend_url)
+                backend=ProjectBackend(pulumi_backend_url)
             )))
     return stack
 
 
 def create(vendor, pulumi_opts, resource_opts):
     resource_f = getattr(resources, f"{resources.PREFIX}{vendor}")
     pulumi_opts["stack_name"] = get_stack_name(vendor, resource_f, resource_opts)
@@ -56,12 +56,17 @@
     stack.up(on_output=print)
 
 
 def destroy(vendor, pulumi_opts, resource_opts):
     resource_f = getattr(resources, f"{resources.PREFIX}{vendor}")
     pulumi_opts["stack_name"] = get_stack_name(vendor, resource_f, resource_opts)
 
-    def pulumi_program():
-        return lambda: None
-
-    stack = pulumi_stack(pulumi_program, **pulumi_opts)
+    stack = pulumi_stack(lambda: None, **pulumi_opts)
     stack.up(on_output=print)
+
+
+def cancel(vendor, pulumi_opts, resource_opts):
+    resource_f = getattr(resources, f"{resources.PREFIX}{vendor}")
+    pulumi_opts["stack_name"] = get_stack_name(vendor, resource_f, resource_opts)
+
+    stack = pulumi_stack(lambda: None, **pulumi_opts)
+    stack.cancel()
```

### Comparing `sparecores_runner-0.0.4/src/sparecores_runner.egg-info/PKG-INFO` & `sparecores_runner-0.0.5/src/sparecores_runner.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-runner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Start cloud instances.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-runner
 Project-URL: issues, https://github.com/SpareCores/sc-runner/issues
 Project-URL: documentation, https://sparecores.github.io/sc-runner/
 Project-URL: homepage, https://sparecores.com
```

