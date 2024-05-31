# Comparing `tmp/hashcommit-0.1.2.tar.gz` & `tmp/hashcommit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.2.tar", last modified: Fri May 31 08:38:26 2024, max compression
+gzip compressed data, was "hashcommit-0.1.3.tar", last modified: Fri May 31 14:25:29 2024, max compression
```

## Comparing `hashcommit-0.1.2.tar` & `hashcommit-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.140516 hashcommit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 08:38:14.000000 hashcommit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 08:38:26.140516 hashcommit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-31 08:38:14.000000 hashcommit-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.136516 hashcommit-0.1.2/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.140516 hashcommit-0.1.2/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:38:26.140516 hashcommit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 08:38:14.000000 hashcommit-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.136516 hashcommit-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 14:25:20.000000 hashcommit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:25:29.592740 hashcommit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 14:25:20.000000 hashcommit-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:25:29.592740 hashcommit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 14:25:20.000000 hashcommit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.2/LICENSE` & `hashcommit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.2/PKG-INFO` & `hashcommit-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,19 @@
 
 ```sh
 hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
 ```
 
 ### Overwriting Commits in the Past
 
-Overwriting a particular commit in the past will be implemented in the future.
+You can overwrite the existing commit that has other commits on top of it. To do this, use the `--commit` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --commit <commit_hash>
+```
 
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
@@ -106,19 +110,25 @@
 # Using act
 act
 ```
 
 You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
 
 ```sh
-tox -e format && tox -e checks && tox -e py311 --
+tox -e format && tox -e checks && tox -e py312 --
+```
+
+To run tox tests under docker (not using your git):
+
+```sh
+docker compose up
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm test bash
+docker compose run --rm --workdir /repo test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.2/README.md` & `hashcommit-0.1.3/hashcommit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: hashcommit
+Version: 0.1.3
+Summary: A tool to generate a Git commit with a specific hash part.
+Home-page: https://github.com/wozniakpl/hashcommit
+Author: Bartosz Woźniak
+Author-email: bwozniakdev@protonmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hashcommit
 
 A tool to generate a Git commit with a specific hash part.
 
 ## Prerequisites
 
 Ensure you have Git installed on your system.
@@ -65,15 +79,19 @@
 
 ```sh
 hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
 ```
 
 ### Overwriting Commits in the Past
 
-Overwriting a particular commit in the past will be implemented in the future.
+You can overwrite the existing commit that has other commits on top of it. To do this, use the `--commit` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --commit <commit_hash>
+```
 
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
@@ -92,19 +110,25 @@
 # Using act
 act
 ```
 
 You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
 
 ```sh
-tox -e format && tox -e checks && tox -e py311 --
+tox -e format && tox -e checks && tox -e py312 --
+```
+
+To run tox tests under docker (not using your git):
+
+```sh
+docker compose up
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm test bash
+docker compose run --rm --workdir /repo test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hashcommit-0.1.2/hashcommit/args.py` & `hashcommit-0.1.3/hashcommit/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     hash: Optional[str]
     message: Optional[str]
     match_type: MatchType
     version: bool
     verbose: int
     overwrite: bool
     no_preserve_author: bool
+    commit: Optional[str]
 
 
 def parse_args() -> HashCommitArgs:
     parser = argparse.ArgumentParser(
         description="Generate a Git commit with a specific hash prefix."
     )
     if len(sys.argv) == 1:
@@ -50,8 +51,13 @@
         help="Overwrite the existing commit instead of creating a new one.",
     )
     parser.add_argument(
         "--no-preserve-author",
         action="store_true",
         help="Do not preserve the original commit author when overwriting.",
     )
+    parser.add_argument(
+        "--commit",
+        help="Commit hash to overwrite. If not provided, the last commit will be used.",
+        type=str,
+    )
     return parser.parse_args(namespace=HashCommitArgs())
```

### Comparing `hashcommit-0.1.2/hashcommit/main.py` & `hashcommit-0.1.3/hashcommit/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import logging
 import sys
 
 from .args import HashCommitArgs, parse_args
-from .commit import create_a_commit_with_hash, overwrite_a_commit_with_hash
+from .commit import (
+    create_a_commit_with_hash,
+    overwrite_a_commit_with_hash,
+    overwrite_and_rebase,
+)
 from .git import does_repo_have_any_commits, is_in_git_repo
 from .logging import configure_logging
 from .version import VERSION
 
 
 def main() -> int:
     args: HashCommitArgs = parse_args()
@@ -24,34 +28,42 @@
     if not is_in_git_repo():
         print("fatal: not a git repository", file=sys.stderr)
         return 1
 
     try:
 
         if args.overwrite:
-            overwrite_a_commit_with_hash(
-                desired_hash=args.hash,
-                message=args.message,
-                match_type=args.match_type,
-                preserve_author=not args.no_preserve_author,
-            )
+            if args.commit:
+                overwrite_and_rebase(
+                    desired_hash=args.hash,
+                    message=args.message,
+                    commit_hash=args.commit,
+                    preserve_author=not args.no_preserve_author,
+                    match_type=args.match_type,
+                )
+            else:
+                overwrite_a_commit_with_hash(
+                    desired_hash=args.hash,
+                    message=args.message,
+                    match_type=args.match_type,
+                    preserve_author=not args.no_preserve_author,
+                )
         else:
             if not args.message:
                 print(
                     "Error: --message argument is required if not using --overwrite.",
                     file=sys.stderr,
                 )
                 return 1
-            if not does_repo_have_any_commits():
-                if not args.message:
-                    print(
-                        "Error: --message argument is required if the repository is empty.",
-                        file=sys.stderr,
-                    )
-                    return 1
+            if not does_repo_have_any_commits() and not args.message:
+                print(
+                    "Error: --message argument is required if the repository is empty.",
+                    file=sys.stderr,
+                )
+                return 1
             create_a_commit_with_hash(
                 desired_hash=args.hash,
                 message=args.message,
                 match_type=args.match_type,
             )
     except KeyboardInterrupt:
         print("\nProcess interrupted by user")
```

### Comparing `hashcommit-0.1.2/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: hashcommit
-Version: 0.1.2
-Summary: A tool to generate a Git commit with a specific hash part.
-Home-page: https://github.com/wozniakpl/hashcommit
-Author: Bartosz Woźniak
-Author-email: bwozniakdev@protonmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hashcommit
 
 A tool to generate a Git commit with a specific hash part.
 
 ## Prerequisites
 
 Ensure you have Git installed on your system.
@@ -79,15 +65,19 @@
 
 ```sh
 hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
 ```
 
 ### Overwriting Commits in the Past
 
-Overwriting a particular commit in the past will be implemented in the future.
+You can overwrite the existing commit that has other commits on top of it. To do this, use the `--commit` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --commit <commit_hash>
+```
 
 ## Development
 
 To develop or contribute to this project, clone the repository and install the dependencies:
 
 ```sh
 git clone https://github.com/wozniakpl/hashcommit.git
@@ -106,19 +96,25 @@
 # Using act
 act
 ```
 
 You can use the following command for simplicity of development. It formats the code, runs the checks, and the tests on one Python version:
 
 ```sh
-tox -e format && tox -e checks && tox -e py311 --
+tox -e format && tox -e checks && tox -e py312 --
+```
+
+To run tox tests under docker (not using your git):
+
+```sh
+docker compose up
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm test bash
+docker compose run --rm --workdir /repo test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hashcommit-0.1.2/setup.py` & `hashcommit-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.2/tests/test_empty_repo.py` & `hashcommit-0.1.3/tests/test_empty_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pathlib import Path
 
-from utils import get_git_log, run_git_command, run_hashcommit
+from utils import configure_git, get_git_log, run_hashcommit_command
 
 
 def test_running_inside_an_empty_git_repository(empty_git_repo: Path) -> None:
-    run_git_command(["config", "user.name", "Test User"], cwd=empty_git_repo)
-    run_git_command(["config", "user.email", "test@user.com"], cwd=empty_git_repo)
-    result = run_hashcommit(
+    configure_git(empty_git_repo, "Test User", "test@user.com")
+    result = run_hashcommit_command(
         ["--message", "test", "--hash", "a", "--match-type", "begin"],
         cwd=empty_git_repo,
     )
-    assert result.returncode == 0
+    assert not result.stderr, result.stderr
 
     git_log = get_git_log(empty_git_repo)
     assert len(git_log) == 1
 
     assert git_log[0].hash.startswith("a")
     assert git_log[0].message == "test\n"
```

