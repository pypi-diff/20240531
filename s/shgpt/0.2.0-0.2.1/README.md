# Comparing `tmp/shgpt-0.2.0.tar.gz` & `tmp/shgpt-0.2.1.tar.gz`

## Comparing `shgpt-0.2.0.tar` & `shgpt-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 shgpt-0.2.0/Makefile
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/version.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/api/ollama.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/tui/app.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/tui/app.tcss
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/utils/common.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/utils/conf.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.2.0/shgpt/utils/http.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.2.0/.gitignore
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 shgpt-0.2.0/README.md
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 shgpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 shgpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 shgpt-0.2.1/Makefile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/__main__.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/app.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/version.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/api/ollama.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/tui/app.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/tui/app.tcss
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/common.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/conf.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/http.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 shgpt-0.2.1/README.md
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 shgpt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 shgpt-0.2.1/PKG-INFO
```

### Comparing `shgpt-0.2.0/shgpt/__main__.py` & `shgpt-0.2.1/shgpt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import argparse, sys
 from os import environ, makedirs
-from smartinput import sinput
+from smartinput import sinput, Shell, Fore
 from .api.ollama import Ollama
 from .version import __version__
 from .utils.conf import *
 from .utils.common import *
 from .tui.app import ShellGPTApp
+from functools import partial
+
+
+def repl_handler(llm, prompt, shell):
+    if prompt != "":
+        try:
+            for r in llm.generate(prompt):
+                print(r, end='')
+            print()
+        except Exception as e:
+            shell.out(f"Error when infer: ${e}")
 
 
 class ShellGPT(object):
     def __init__(self, url, model, role, timeout):
         makedirs(CONF_PATH, exist_ok=True)
         self.llm = Ollama(url, model, role, timeout)
 
@@ -20,30 +31,23 @@
     def repl(self):
         print(r'''
 __      __   _                    _         ___ _        _ _  ___ ___ _____
 \ \    / /__| |__ ___ _ __  ___  | |_ ___  / __| |_  ___| | |/ __| _ \_   _|
  \ \/\/ / -_) / _/ _ \ '  \/ -_) |  _/ _ \ \__ \ ' \/ -_) | | (_ |  _/ | |
   \_/\_/\___|_\__\___/_|_|_\___|  \__\___/ |___/_||_\___|_|_|\___|_|   |_|
 ''')
-        while True:
-            prompt = sinput("> ")
-            if prompt != "":
-                try:
-                    self.infer(prompt, False, True)
-                except Exception as e:
-                    print(f"Error when infer: ${e}")
+        shell = Shell(callback=partial(repl_handler, self.llm), intitle="shellgpt> ", outtitle="", alertcolor=Fore.RED, exiton="exit")
+        shell.start()
+        return
 
     def infer(self, prompt):
         for r in self.llm.generate(prompt):
             print(r, end='')
         print()
 
-        # r = sinput("Execute, Yank, Continue", hints=['e', 'y', 'c'])
-        # print(r)
-
 
 def main():
     prog = sys.argv[0]
     parser = argparse.ArgumentParser(
         prog=prog,
         description='Make Shell easy to use with power of LLM!')
     parser.add_argument('-V', '--version', action='version', version='%(prog)s ' + __version__)
@@ -62,14 +66,16 @@
     prompt = ' '.join(args.prompt)
     if sin is not None:
         prompt = f'{sin}\n\n{prompt}'
 
     role = args.role
     if args.shell:
         role = 'shell'
+    elif args.repl:
+        pass
     elif len(prompt) == 0:
         # tui default to shell role
         role = 'shell'
 
     sg = ShellGPT(args.ollama_url, args.ollama_model, role, args.timeout)
     if args.repl:
         sg.repl()
```

### Comparing `shgpt-0.2.0/shgpt/api/ollama.py` & `shgpt-0.2.1/shgpt/api/ollama.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import json, os
 from ..utils.http import TimeoutSession
 from ..utils.common import *
 from ..utils.conf import *
 
 HIST_SEP = '=========='
 CONTENT = {
-    'default': f'''You are programming and system administration assistant.
-    You are managing {OS_NAME} operating system with {SHELL} shell.
+    'default': None,
+    'code': '''
+Provide only code as output without any description.
+Provide only code in plain text format without Markdown formatting.
+Do not include symbols such as ``` or ```python.
+If there is a lack of details, provide most logical solution.
+You are not allowed to ask for more details.
+For example if the prompt is "Hello world Python", you should return "print('Hello world')".
     ''',
     'shell': f'''
     You are a shell script assistant on {OS_NAME} running {SHELL},
     Output the best matching shell commands without any other information, or any quotes.
     Make sure it's valid shell command.
     ''',
     # commit message
```

### Comparing `shgpt-0.2.0/shgpt/tui/app.py` & `shgpt-0.2.1/shgpt/tui/app.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.2.0/shgpt/utils/common.py` & `shgpt-0.2.1/shgpt/utils/common.py`

 * *Files identical despite different names*

### Comparing `shgpt-0.2.0/pyproject.toml` & `shgpt-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shgpt-0.2.0/PKG-INFO` & `shgpt-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: shgpt
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate shell command you want with power of LLM, without leaving your terminal.
 Project-URL: Repository, https://github.com/jiacai2050/shellgpt
 Project-URL: Issues, https://github.com/jiacai2050/shellgpt/issues
 Author-email: Jiacai Liu <dev@liujiacai.net>
 License-Expression: GPL-3.0
 Keywords: gpt,llm,shell
 Requires-Dist: pyperclip
@@ -25,22 +25,37 @@
 ```
 
 This will install two commands: `sg` and `shgpt`.
 
 # Usage
 
 ShellGPT has three modes to use:
-- `sg {your question}`, direct mode
+- Direct mode, `sg [question]` or `echo question | sg`.
 - `sg`, Enter TUI mode, tailored for infer shell command
-- `sg -r`, Enter an interactive REPL
+- `sg -l`, Enter an interactive REPL.
 
 See [conf.py](shgpt/utils/conf.py) for configs.
 
-## TUI
-There are some key bindings to use in TUI:
+## Role
+
+There are some built-in roles in shellgpt:
+- `default`, used for ask general questions
+- `code`, used for ask programming questions
+- `shell`, used for infer shell command
+- `cm`, used for generate git commit message
+
+```bash
+git diff | sg -r cm
+```
+
+Users can provide their own role with `-r` option.
+
+## TUI generate git commit message
+
+Users can provide their own role with `-r`There are some key bindings to use in TUI: option
 - `ctrl+j`, Infer answer
 - `ctrl+r`, Run command
 - `ctrl+y`, Yank command
 
 ![TUI screenshot](./assets/shellgpt-tui.jpg)
 
 # Requirements
```

