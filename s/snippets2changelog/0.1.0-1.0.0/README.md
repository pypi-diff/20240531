# Comparing `tmp/snippets2changelog-0.1.0.tar.gz` & `tmp/snippets2changelog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snippets2changelog-0.1.0.tar", max compression
+gzip compressed data, was "snippets2changelog-1.0.0.tar", max compression
```

## Comparing `snippets2changelog-0.1.0.tar` & `snippets2changelog-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1198 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2939 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/README.md
--rw-r--r--   0        0        0     3386 2024-05-30 14:33:36.594610 snippets2changelog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/__init__.py
--rwxr-xr-x   0        0        0     3672 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/cli.py
--rw-r--r--   0        0        0     1991 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/common.py
--rw-r--r--   0        0        0     1654 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/creator.py
--rw-r--r--   0        0        0     2543 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/parser.py
--rw-r--r--   0        0        0      112 2024-05-30 14:33:19.454379 snippets2changelog-0.1.0/snippets2changelog/templates/snippet.md.template
--rw-r--r--   0        0        0      124 2024-05-30 14:33:36.038602 snippets2changelog-0.1.0/snippets2changelog/version.py
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 snippets2changelog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1198 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3205 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/README.md
+-rw-r--r--   0        0        0     3386 2024-05-30 22:18:38.539173 snippets2changelog-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/__init__.py
+-rwxr-xr-x   0        0        0     4333 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/cli.py
+-rw-r--r--   0        0        0     4262 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/collector.py
+-rw-r--r--   0        0        0     1991 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/common.py
+-rw-r--r--   0        0        0     5172 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/creator.py
+-rw-r--r--   0        0        0     2817 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/parser.py
+-rw-r--r--   0        0        0      112 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/templates/snippet.md.template
+-rw-r--r--   0        0        0      124 2024-05-30 22:18:38.015166 snippets2changelog-1.0.0/snippets2changelog/version.py
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 snippets2changelog-1.0.0/PKG-INFO
```

### Comparing `snippets2changelog-0.1.0/LICENSE.txt` & `snippets2changelog-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snippets2changelog-0.1.0/README.md` & `snippets2changelog-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
 - [Usage](#usage)
   - [Info](#info)
   - [Create](#create)
+    - [Snippet](#snippet)
+    - [Changelog](#changelog)
   - [Parse](#parse)
 - [Contributing](#contributing)
   - [Setup](#setup)
   - [Testing](#testing)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
@@ -42,14 +44,15 @@
 Print informations about snippets2changelog
 
 ```bash
 changelog-generator info
 ```
 
 ### Create
+#### Snippet
 
 Create a new snippet with the given name at the specified snippets folder
 
 ```bash
 changelog-generator create example_snippets/123.md
 ```
 
@@ -70,14 +73,23 @@
 affected: testers, users
 -->
 
 TBD
 
 ```
 
+#### Changelog
+
+Create or update a changelog with all snippets.
+New changelog will be named `<OLD_CHANGELOG_NAME.new>`
+
+```bash
+changelog-generator changelog changelog.md --snippets=.snippets
+```
+
 ### Parse
 
 Parse an existing snippet file and return the data as JSON without indentation
 
 ```bash
 changelog-generator parse example_snippets/123.md \
   --indent=4
```

### Comparing `snippets2changelog-0.1.0/pyproject.toml` & `snippets2changelog-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snippets2changelog"
-version = "0.1.0" # will-be-updated-automatically
+version = "1.0.0" # will-be-updated-automatically
 description =  "Generate a changelog from individual snippets"
 authors = ["brainelectronics <info@brainelectronics.de>"]
 repository = "https://github.com/brainelectronics/snippets2changelog"
 readme = "README.md"
 license = "MIT"
 packages = [
   { include = "snippets2changelog/**/*.py" }
@@ -36,22 +36,22 @@
 format-jinja = """{{ check_output(["python3", "-c", "from pathlib import Path; exec(Path('snippets2changelog/version.py').read_text()); print(__version__)"]).decode().strip() }}"""
 # format-jinja = "{{ env.get('PROJECT_VERSION') }}"
 
 [tool.poetry.scripts]
 changelog-generator = 'snippets2changelog.cli:main'
 
 [tool.poetry.dependencies]
-python = "^3.11"
-pyyaml = "~6.0"
+changelog2version = "^0.10"
 GitPython = "~3.1.43"
 jinja2 = "^3.1.4"
+python = "^3.11"
+pyyaml = "~6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
-changelog2version = "^0.10"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 poetry-dynamic-versioning = "^1.3.0"
 pre-commit = "*"
 pylint = "*"
 pytest = "*"
```

### Comparing `snippets2changelog-0.1.0/snippets2changelog/cli.py` & `snippets2changelog-1.0.0/snippets2changelog/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from argparse import ArgumentParser
 from argparse import Namespace as Args
 from pathlib import Path
 from sys import stdout
 from typing import Sequence
 
 from .common import LOG_LEVELS, collect_user_choice
-from .creator import SnippetCreator
+from .creator import ChangelogCreator, SnippetCreator
 from .parser import SnippetParser
 
 LOGGER_FORMAT = '[%(asctime)s] [%(levelname)-8s] [%(filename)-15s @'\
                 ' %(funcName)-15s:%(lineno)4s] %(message)s'
 
 # configure logging
 logging.basicConfig(level=logging.INFO, format=LOGGER_FORMAT, stream=stdout)
@@ -46,14 +46,30 @@
 
     parser_info = subparsers.add_parser(
         "info",
         help="Prints information about snippets2changelog",
     )
     parser_info.set_defaults(func=fn_info)
 
+    parser_changelog = subparsers.add_parser(
+        "changelog",
+        help="Create a changelog",
+    )
+    parser_changelog.set_defaults(func=fn_changelog)
+    parser_changelog.add_argument(
+        "changelog",
+        type=Path,
+        help="Path to existing changelog",
+    )
+    parser_changelog.add_argument(
+        "--snippets",
+        type=lambda x: does_exist(parser, x),
+        help="Directory to crawl for snippets",
+    )
+
     parser_create = subparsers.add_parser(
         "create",
         help="Create a snippet",
     )
     parser_create.set_defaults(func=fn_create)
     parser_create.add_argument(
         "name",
@@ -93,33 +109,39 @@
         return importlib.metadata.version("snippets2changelog")
 
 
 def fn_info(_args: Args) -> None:
     print(f"Version: {extract_version()}")
 
 
+def fn_changelog(args: Args) -> None:
+    cc = ChangelogCreator(changelog=args.changelog, snippets_folder=args.snippets, verbosity=args.verbose)
+    cc.update_changelog()
+
+
 def fn_create(args: Args) -> None:
     content = {
         "short_description": input("Short description: "),
         "type": collect_user_choice(
             question="Type of change", options=["bugfix", "feature", "breaking"]
         ),
         "scope": collect_user_choice(question="Scope of change", options=["internal", "external", "all"]),
         "affected": input("Affected users (default all): ") or "all",
         "content": "TBD",
     }
-    sc = SnippetCreator(file_name=args.name, content=content)
-    logger.debug(f"rendered content: >>>>>>\n{sc.render()}\n<<<<<<")
-    sc.create()
+    sc = SnippetCreator()
+    sc.render(content=content)
+    logger.debug(f"rendered content: >>>>>>\n{sc.rendered_content}\n<<<<<<")
+    sc.create(file_name=args.name)
 
 
 def fn_parse(args: Args) -> None:
-    sp = SnippetParser(file_name=args.name, verbosity=args.verbose)
-    sp.parse()
-    print(json.dumps(sp.content, indent=args.indent))
+    sp = SnippetParser(verbosity=args.verbose)
+    sp.parse(file_name=args.name)
+    print(json.dumps(sp.parsed_content, indent=args.indent))
 
 
 def main() -> int:
     """Entry point for everything else"""
     args = parse_args()
 
     log_level = LOG_LEVELS[min(args.verbose, max(LOG_LEVELS.keys()))]
```

### Comparing `snippets2changelog-0.1.0/snippets2changelog/common.py` & `snippets2changelog-1.0.0/snippets2changelog/common.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-0.1.0/snippets2changelog/parser.py` & `snippets2changelog-1.0.0/snippets2changelog/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,56 +16,57 @@
 
     pass
 
 
 class SnippetParser(object):
     """docstring for SnippetCreator"""
 
-    def __init__(self, file_name: Path, additional_keys: tuple[str] | tuple[()] = (), verbosity: int = 0) -> None:
-        if file_name.exists():
-            self._file_name = file_name
-        else:
-            raise SnippetParserError(f"Given snippets '{file_name}' does not exist")
-
-        self._required_keys = ("type", "scope", "affected") + additional_keys
-        self._content = dict(zip(self._required_keys, [""] * len(self._required_keys)))
-
+    def __init__(self, additional_keys: tuple[str] | tuple[()] = (), verbosity: int = 0) -> None:
+        self._file_name = Path()
+        self._required_parser_keys = ("type", "scope", "affected") + additional_keys
+        self._parsed_content = dict(zip(self._required_parser_keys, [""] * len(self._required_parser_keys)))
         self._logger = logging.getLogger(__name__)
         self._logger.setLevel(level=LOG_LEVELS[min(verbosity, max(LOG_LEVELS.keys()))])
 
     @property
-    def content(self) -> dict[str, str]:
-        return self._content
+    def parsed_content(self) -> dict[str, str]:
+        return self._parsed_content
+
+    def parse(self, file_name: Path) -> None:
+        # don't forget to clear the content before the next run
+        self._parsed_content = dict(zip(self._required_parser_keys, [""] * len(self._required_parser_keys)))
+
+        if not file_name.exists():
+            raise SnippetParserError(f"Given snippets '{file_name}' does not exist")
 
-    def parse(self) -> None:
-        file_content = read_file(self._file_name, parse="read")
+        file_content = read_file(file_name, parse="read")
 
         header_match = re.search(r"(^##\s)(.*)", file_content, re.MULTILINE)
         if header_match:
-            self._content["title"] = header_match.groups()[-1]
+            self._parsed_content["title"] = header_match.groups()[-1]
 
         matches = re.finditer(COMMENT_PATTERN, file_content, re.MULTILINE)
         match_found = False
 
         for match in matches:
             end = match.end()
             self._logger.debug(f"match: \n{match.group()}")
             found_keys = list()
-            for key in self._required_keys:
+            for key in self._required_parser_keys:
                 info_matches = re.finditer(rf"({key}:\s)(.*)", match.group(), re.MULTILINE)
                 for key_match in info_matches:
                     data = key_match.groups()[-1]
                     if key in ("affected", "scope"):
                         data = [x.strip() for x in data.split(",")]
 
                     # do not overwrite already existing data
-                    if not self._content[key]:
-                        self._content[key] = data
+                    if not self._parsed_content[key]:
+                        self._parsed_content[key] = data
                         found_keys.append(key)
-                    self._logger.debug(f"processed: '{key}' as '{data}', found_keys: {found_keys}")
+                    self._logger.debug(f"processed: '{key}' as '{data}', found_keys: {found_keys}, required: {self._required_parser_keys}")
 
-                if sorted(self._required_keys) == sorted(found_keys):
+                if sorted(self._required_parser_keys) == sorted(found_keys):
                     self._logger.debug("All required keys found, taking everything else as details content")
                     match_found = True
             if match_found:
-                self._content["details"] = file_content[end:]
+                self._parsed_content["details"] = file_content[end:]
                 break
```

### Comparing `snippets2changelog-0.1.0/PKG-INFO` & `snippets2changelog-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snippets2changelog
-Version: 0.1.0
+Version: 1.0.0
 Summary: Generate a changelog from individual snippets
 Home-page: https://github.com/brainelectronics/snippets2changelog
 License: MIT
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Version Control
 Requires-Dist: GitPython (>=3.1.43,<3.2.0)
+Requires-Dist: changelog2version (>=0.10,<0.11)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<6.1)
 Project-URL: Repository, https://github.com/brainelectronics/snippets2changelog
 Description-Content-Type: text/markdown
 
 # snippets2changelog
 
@@ -44,14 +45,16 @@
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
 - [Usage](#usage)
   - [Info](#info)
   - [Create](#create)
+    - [Snippet](#snippet)
+    - [Changelog](#changelog)
   - [Parse](#parse)
 - [Contributing](#contributing)
   - [Setup](#setup)
   - [Testing](#testing)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
@@ -69,14 +72,15 @@
 Print informations about snippets2changelog
 
 ```bash
 changelog-generator info
 ```
 
 ### Create
+#### Snippet
 
 Create a new snippet with the given name at the specified snippets folder
 
 ```bash
 changelog-generator create example_snippets/123.md
 ```
 
@@ -97,14 +101,23 @@
 affected: testers, users
 -->
 
 TBD
 
 ```
 
+#### Changelog
+
+Create or update a changelog with all snippets.
+New changelog will be named `<OLD_CHANGELOG_NAME.new>`
+
+```bash
+changelog-generator changelog changelog.md --snippets=.snippets
+```
+
 ### Parse
 
 Parse an existing snippet file and return the data as JSON without indentation
 
 ```bash
 changelog-generator parse example_snippets/123.md \
   --indent=4
```

