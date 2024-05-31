# Comparing `tmp/killercoda_cli-1.1.1.tar.gz` & `tmp/killercoda_cli-1.1.2.tar.gz`

## Comparing `killercoda_cli-1.1.1.tar` & `killercoda_cli-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16418 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/killercoda_cli/cli.py
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/killercoda_cli/scenario_init.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/tests/__init__.py
--rwxr-xr-x   0        0        0    12187 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/tests/test_integration_cli.py
--rwxr-xr-x   0        0        0     4191 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/tests/test_scenario_init.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/README.md
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 killercoda_cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    17240 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/killercoda_cli/cli.py
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/killercoda_cli/scenario_init.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/tests/__init__.py
+-rwxr-xr-x   0        0        0    12187 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/tests/test_cli.py
+-rwxr-xr-x   0        0        0     5041 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/tests/test_integration_cli.py
+-rwxr-xr-x   0        0        0     4191 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/tests/test_scenario_init.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/README.md
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 killercoda_cli-1.1.2/PKG-INFO
```

### Comparing `killercoda_cli-1.1.1/.github/workflows/ci.yml` & `killercoda_cli-1.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/killercoda_cli/cli.py` & `killercoda_cli-1.1.2/killercoda_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 import difflib
 import json
 import os
 import subprocess
 import sys
 from typing import List, Optional
+from cookiecutter.main import cookiecutter
 from killercoda_cli.__about__ import __version__
 from killercoda_cli.scenario_init import init_project
 
 class FileOperation:
     """
     Define a type hint for the different types of file operations that can be performed.
     This Union type allows for specifying the operation (as a string literal indicating the type of action),
@@ -219,15 +220,14 @@
             file_operations.append(
                 FileOperation("rename", old_name, content=new_step_md)
             )
 
     return file_operations
 
 
-from typing import List
 
 def calculate_new_step_file_operations(
     insert_step_num: int, step_title: str, step_type: str
 ) -> List[FileOperation]:
     """
     Calculate the file operations needed to add a new step to the scenario.
 
@@ -342,14 +342,15 @@
         Options:
           -h, --help    Show this message and exit.
           -v, --version Display the version of the tool.
 
         Basic Commands:
           Running 'killercoda-cli' starts the interactive process.
           init: Initialize a new project by creating an 'index.json' file.
+          assets: Generate the predefined assets folder structure.
 
         Requirements:
           - The tool must be run in a directory containing step files or directories (e.g., step1.md, step2/).
           - An 'index.json' file must be present in the directory, which contains metadata about the steps.
 
         Functionality:
           - Renames and renumbers step files and directories based on user input.
@@ -366,14 +367,30 @@
             with open(operation.path, "w") as file:
                 file.write(operation.content)
         elif operation.operation == "chmod":
             os.chmod(operation.path, operation.mode)
         elif operation.operation == "rename":
             os.rename(operation.path, operation.content)
 
+def generate_assets():
+    try:
+        template_repo = 'https://github.com/Piotr1215/cookiecutter-killercoda-assets'
+        output_dir = os.getcwd()
+        
+        print(f"Generating assets from template: {template_repo}")
+        print(f"Output directory: {output_dir}")
+        
+        cookiecutter(template_repo, no_input=True, extra_context={"project_name": "killercoda-assets"}, output_dir=output_dir)
+        
+        print("Assets generated successfully.")
+    except Exception as e:
+        print(f"An error occurred in generate_assets: {e}")
+        raise
+
+
 def main():
     """
     This function orchestrates the entire process of adding a new step to the scenario,
     from taking user input to updating the file system and the index.json file.
     It ensures that the 'index.json' file is present, gathers the current directory structure,
     prompts the user for the new step's title and number, calculates the necessary file operations,
     and applies those changes to the file system and the index.json file.
@@ -385,14 +402,17 @@
             return
         if len(sys.argv) > 1 and sys.argv[1] in ["-v", "--version"]:
             print(f"killercoda-cli v{__version__}")
             return
         if len(sys.argv) > 1 and sys.argv[1] in ["init"]:
             init_project()
             return
+        if len(sys.argv) > 1 and sys.argv[1] in ["assets"]:
+            generate_assets()
+            return
         
         old_tree_structure = get_tree_structure()
         directory_items = os.listdir(".")
         steps_dict = get_current_steps_dict(directory_items)
         if "index.json" not in directory_items:
             print(
                 "The 'index.json' file is missing. Please ensure it is present in the current directory."
@@ -422,12 +442,14 @@
         with open(index_file_path, "w") as index_file:
             json.dump(updated_index_data, index_file, ensure_ascii=False, indent=4)
         new_tree_structure = get_tree_structure()
         tree_diff = generate_diff(old_tree_structure, new_tree_structure)
         print("\nFile structure changes:")
         print(tree_diff, end="")
     except Exception as e:
+        import traceback
         print(f"An error occurred: {e}")
+        traceback.print_exc()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `killercoda_cli-1.1.1/killercoda_cli/scenario_init.py` & `killercoda_cli-1.1.2/killercoda_cli/scenario_init.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/tests/test_cli.py` & `killercoda_cli-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/tests/test_integration_cli.py` & `killercoda_cli-1.1.2/tests/test_integration_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 import json
 from unittest.mock import patch
 from io import StringIO
 import os
+import shutil
 
 # Assuming cli.py is structured as a module you can import from
 from killercoda_cli import cli
 
 class TestCLIIntegration(unittest.TestCase):
     def setUp(self):
         # Setup test environment, e.g., creating a temporary directory structure
@@ -15,14 +16,32 @@
         # Create necessary files and directories for testing
         os.makedirs(os.path.join(self.test_dir, 'step1'), exist_ok=True)
         with open(os.path.join(self.test_dir, 'step1/step1.md'), 'w') as f:
             f.write("# Step 1\n")
         with open(os.path.join(self.test_dir, 'index.json'), 'w') as f:
             json.dump({"details": {"steps": [{"title": "Step 1", "text": "step1/step1.md", "background": "step1/background.sh"}]}}, f)
 
+    def test_generate_assets(self):
+        # Setup test environment
+        test_generate_dir = '/tmp/test_generate_assets'
+        os.makedirs(test_generate_dir, exist_ok=True)
+        os.chdir(test_generate_dir)
+        
+        # Run the generate_assets function
+        cli.generate_assets()
+
+        # Verify the generated files and directories
+        self.assertTrue(os.path.exists(os.path.join(test_generate_dir, 'assets')))
+        self.assertTrue(os.path.exists(os.path.join(test_generate_dir, 'assets', 'deploy.sh')))
+        self.assertTrue(os.path.exists(os.path.join(test_generate_dir, 'background.sh')))
+        self.assertTrue(os.path.exists(os.path.join(test_generate_dir, 'foreground.sh')))
+        
+        # Clean up the test directory
+        shutil.rmtree(test_generate_dir)
+
     @patch('sys.argv', ['killercoda-cli', '--help'])
     @patch('sys.stdout', new_callable=StringIO)
     def test_cli_main_help_message(self, mock_stdout):
         cli.main()
         output = mock_stdout.getvalue()
         self.assertIn("Usage: killercoda-cli [OPTIONS]", output)
         self.assertIn("A CLI helper for writing KillerCoda scenarios", output)
```

### Comparing `killercoda_cli-1.1.1/tests/test_scenario_init.py` & `killercoda_cli-1.1.2/tests/test_scenario_init.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/.gitignore` & `killercoda_cli-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/LICENSE.txt` & `killercoda_cli-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.1.1/README.md` & `killercoda_cli-1.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 
 **Table of Contents**
 
 * [Installation](#installation)
 * [Introduction](#introduction)
 * [Documentation](#documentation)
   * [Requirements](#requirements)
-  * [Example usage](#example-usage)
+* [Usage](#usage)
+  * [Initialize a new scenario](#initialize-a-new-scenario)
+  * [Add a new step](#add-a-new-step)
+  * [Adding assets](#adding-assets)
 * [Development](#development)
 * [Testing](#testing)
 * [Disclaimer](#disclaimer)
 * [License](#license)
- 
+
 ## Installation
 
 ```console
 pip install killercoda-cli
 ```
 
 > [!NOTE]
@@ -50,17 +53,32 @@
 at: https://piotr1215.github.io/killercoda-cli/killercoda_cli/cli.html.
 
 ### Requirements
 
 - The tool must be run in a directory containing step files or directories (e.g. step1.md, step2/).
 - An `index.json` file must be present in the directory, which contains metadata about the steps.
 
-### Example usage
+## Usage
+
+### Initialize a new scenario
+
+In a new directory run `killercoda-cli init`. This command will trigger a wizard
+to create a new scenario. After answering all the questions, the directory will
+contain the following structure:
+
+    .
+    ├── index.json
+    ├── intro.md
+    ├── finish.md
+
+### Add a new step
 
-Suppose you have a scenario directory with the following structure:
+From here run `killercoda-cli` without arguments. This command will trigger a
+wizard to add a new step. After answering all the questions, the directory will
+contain steps in the similar structure:
 
     .
     ├── index.json
     ├── step1.md
     └── step2
         └── step2.md
 
@@ -117,14 +135,28 @@
       "title": "Step 2",
       "text": "step3/step3.md"
     }
   ]
 }
 ```
 
+### Adding assets
+
+The `killercoda-cli assets` command has been added to facilitate the generation of necessary assets and folder structures in the current working directory using a predefined [cookiecutter template](https://github.com/Piotr1215/cookiecutter-killercoda-assets).
+
+> [!NOTE]
+> The assets are opinionated and may not fit all use cases, but it's a good
+> starting point to add some interactivity to the scenario.
+
+This command will generate the required folder structure and files directly in
+the current working directory and **remove** the temporary directory.
+
+Assets are NOT automatically added to the `index.json` to leave the decision to
+the user how to bring the assets into the scenario.
+
 ## Development
 
 Installing locally with `pip install -e . --user` will allow you to run the tool
 locally.
 
 ## Testing
```

### Comparing `killercoda_cli-1.1.1/pyproject.toml` & `killercoda_cli-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dynamic = ["version"]
 description = 'A CLI helper for writing killercoda scenarios and managing steps'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 dependencies = [
     "inquirer",
+    "cookiecutter",
 ]
 keywords = []
 authors = [
   { name = "Piotr Zaniewski", email = "piotrzan@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `killercoda_cli-1.1.1/PKG-INFO` & `killercoda_cli-1.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: cookiecutter
 Requires-Dist: inquirer
 Description-Content-Type: text/markdown
 
 # killercoda-cli
 
 [![PyPI - Version](https://img.shields.io/pypi/v/killercoda-cli.svg)](https://pypi.org/project/killercoda-cli)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/killercoda-cli.svg)](https://pypi.org/project/killercoda-cli)
@@ -30,20 +31,23 @@
 
 **Table of Contents**
 
 * [Installation](#installation)
 * [Introduction](#introduction)
 * [Documentation](#documentation)
   * [Requirements](#requirements)
-  * [Example usage](#example-usage)
+* [Usage](#usage)
+  * [Initialize a new scenario](#initialize-a-new-scenario)
+  * [Add a new step](#add-a-new-step)
+  * [Adding assets](#adding-assets)
 * [Development](#development)
 * [Testing](#testing)
 * [Disclaimer](#disclaimer)
 * [License](#license)
- 
+
 ## Installation
 
 ```console
 pip install killercoda-cli
 ```
 
 > [!NOTE]
@@ -73,17 +77,32 @@
 at: https://piotr1215.github.io/killercoda-cli/killercoda_cli/cli.html.
 
 ### Requirements
 
 - The tool must be run in a directory containing step files or directories (e.g. step1.md, step2/).
 - An `index.json` file must be present in the directory, which contains metadata about the steps.
 
-### Example usage
+## Usage
+
+### Initialize a new scenario
+
+In a new directory run `killercoda-cli init`. This command will trigger a wizard
+to create a new scenario. After answering all the questions, the directory will
+contain the following structure:
+
+    .
+    ├── index.json
+    ├── intro.md
+    ├── finish.md
+
+### Add a new step
 
-Suppose you have a scenario directory with the following structure:
+From here run `killercoda-cli` without arguments. This command will trigger a
+wizard to add a new step. After answering all the questions, the directory will
+contain steps in the similar structure:
 
     .
     ├── index.json
     ├── step1.md
     └── step2
         └── step2.md
 
@@ -140,14 +159,28 @@
       "title": "Step 2",
       "text": "step3/step3.md"
     }
   ]
 }
 ```
 
+### Adding assets
+
+The `killercoda-cli assets` command has been added to facilitate the generation of necessary assets and folder structures in the current working directory using a predefined [cookiecutter template](https://github.com/Piotr1215/cookiecutter-killercoda-assets).
+
+> [!NOTE]
+> The assets are opinionated and may not fit all use cases, but it's a good
+> starting point to add some interactivity to the scenario.
+
+This command will generate the required folder structure and files directly in
+the current working directory and **remove** the temporary directory.
+
+Assets are NOT automatically added to the `index.json` to leave the decision to
+the user how to bring the assets into the scenario.
+
 ## Development
 
 Installing locally with `pip install -e . --user` will allow you to run the tool
 locally.
 
 ## Testing
```

