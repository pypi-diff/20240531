# Comparing `tmp/pr_pilot_cli-1.3.1.tar.gz` & `tmp/pr_pilot_cli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.3.1.tar", last modified: Thu May 30 17:51:15 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.3.2.tar", last modified: Fri May 31 00:11:37 2024, max compression
```

## Comparing `pr_pilot_cli-1.3.1.tar` & `pr_pilot_cli-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.212295 pr_pilot_cli-1.3.1/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/task_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:11:37.327683 pr_pilot_cli-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 00:11:37.327683 pr_pilot_cli-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:11:37.323683 pr_pilot_cli-1.3.2/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:11:37.323683 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 00:11:37.000000 pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:11:37.327683 pr_pilot_cli-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 00:11:29.000000 pr_pilot_cli-1.3.2/setup.py
```

### Comparing `pr_pilot_cli-1.3.1/LICENSE` & `pr_pilot_cli-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.1/PKG-INFO` & `pr_pilot_cli-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.1 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.2 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
```

### Comparing `pr_pilot_cli-1.3.1/README.md` & `pr_pilot_cli-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.1/cli/cli.py` & `pr_pilot_cli-1.3.2/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 from pr_pilot.util import create_task, wait_for_result, get_task
 from rich.console import Console
 from rich.markdown import Markdown
 from yaspin import yaspin
 
 from cli.detect_repository import detect_repository
 from cli.task_handler import TaskHandler
-from cli.templating import render_prompt_template
+from cli.prompt_template import PromptTemplate
 
 CONFIG_LOCATION = os.path.expanduser('~/.pr-pilot.yaml')
 CONFIG_API_KEY = "api_key"
 CODE_MODEL = "gpt-4"
 POLL_INTERVAL = 2
 
 
 def load_config():
     """Load the configuration from the default location. If it doesn't exist,
     ask user to enter API key and save config."""
     if not os.path.exists(CONFIG_LOCATION):
         api_key_url = "https://app.pr-pilot.ai/dashboard/api-keys/"
-        console.print(f"Configuration file not found. Please create an API key at {api_key_url}.")
+        click.echo(f"Configuration file not found. Please create an API key at {api_key_url}.")
         api_key = click.prompt("PR Pilot API key")
         with open(CONFIG_LOCATION, "w") as f:
             f.write(f"{CONFIG_API_KEY}: {api_key}")
-        console.print(f"Configuration saved in {CONFIG_LOCATION}")
+        click.echo(f"Configuration saved in {CONFIG_LOCATION}")
     with open(CONFIG_LOCATION) as f:
         config = yaml.safe_load(f)
     return config
 
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
@@ -60,15 +60,16 @@
     if not repo:
         # Current directory is not a git repository, see if there is a default repo in the config
         repo = config.get("default_repo")
     if not repo:
         console.print(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
         return
     if file:
-        prompt = render_prompt_template(file, repo, model)
+        renderer = PromptTemplate(file, repo, model)
+        prompt = renderer.render(show_spinner=not raw)
     if not prompt:
         prompt = click.edit("", extension=".md")
         if not prompt:
             console.print("No prompt provided.")
             return
     if code:
         raw = True
```

### Comparing `pr_pilot_cli-1.3.1/cli/detect_repository.py` & `pr_pilot_cli-1.3.2/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.1/cli/task_handler.py` & `pr_pilot_cli-1.3.2/cli/task_handler.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.3.2/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.1 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.2 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
```

### Comparing `pr_pilot_cli-1.3.1/setup.py` & `pr_pilot_cli-1.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.3.1',
+    version='1.3.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

