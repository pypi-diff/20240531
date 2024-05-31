# Comparing `tmp/hashcommit-0.1.1.tar.gz` & `tmp/hashcommit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.1.tar", last modified: Thu May 30 16:28:37 2024, max compression
+gzip compressed data, was "hashcommit-0.1.2.tar", last modified: Fri May 31 08:38:26 2024, max compression
```

## Comparing `hashcommit-0.1.1.tar` & `hashcommit-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 16:28:29.000000 hashcommit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-30 16:28:37.305824 hashcommit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-30 16:28:29.000000 hashcommit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.301824 hashcommit-0.1.1/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:28:29.000000 hashcommit-0.1.1/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 16:28:37.000000 hashcommit-0.1.1/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:28:37.305824 hashcommit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 16:28:29.000000 hashcommit-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:37.305824 hashcommit-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-30 16:28:29.000000 hashcommit-0.1.1/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.140516 hashcommit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 08:38:14.000000 hashcommit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 08:38:26.140516 hashcommit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-31 08:38:14.000000 hashcommit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.136516 hashcommit-0.1.2/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 08:38:14.000000 hashcommit-0.1.2/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.140516 hashcommit-0.1.2/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 08:38:26.000000 hashcommit-0.1.2/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:38:26.140516 hashcommit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 08:38:14.000000 hashcommit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:26.136516 hashcommit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-31 08:38:14.000000 hashcommit-0.1.2/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.1/LICENSE` & `hashcommit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.1/PKG-INFO` & `hashcommit-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hashcommit
 
 A tool to generate a Git commit with a specific hash part.
 
+## Prerequisites
+
+Ensure you have Git installed on your system.
+
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
@@ -67,15 +71,19 @@
 Date:   Thu May 23 17:06:24 2024 +0000
 
     foobar
 ```
 
 ### Author Preservation
 
-By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+By default, the author is preserved when overwriting. To overwrite the author, use the `--no-preserve-author` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
+```
 
 ### Overwriting Commits in the Past
 
 Overwriting a particular commit in the past will be implemented in the future.
 
 ## Development
 
@@ -104,13 +112,13 @@
 ```sh
 tox -e format && tox -e checks && tox -e py311 --
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm tests bash
+docker compose run --rm test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.1/README.md` & `hashcommit-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # hashcommit
 
 A tool to generate a Git commit with a specific hash part.
 
+## Prerequisites
+
+Ensure you have Git installed on your system.
+
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
@@ -53,15 +57,19 @@
 Date:   Thu May 23 17:06:24 2024 +0000
 
     foobar
 ```
 
 ### Author Preservation
 
-By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+By default, the author is preserved when overwriting. To overwrite the author, use the `--no-preserve-author` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
+```
 
 ### Overwriting Commits in the Past
 
 Overwriting a particular commit in the past will be implemented in the future.
 
 ## Development
 
@@ -90,13 +98,13 @@
 ```sh
 tox -e format && tox -e checks && tox -e py311 --
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm tests bash
+docker compose run --rm test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.1/hashcommit/args.py` & `hashcommit-0.1.2/hashcommit/args.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class HashCommitArgs(Namespace):
     hash: Optional[str]
     message: Optional[str]
     match_type: MatchType
     version: bool
     verbose: int
     overwrite: bool
+    no_preserve_author: bool
 
 
 def parse_args() -> HashCommitArgs:
     parser = argparse.ArgumentParser(
         description="Generate a Git commit with a specific hash prefix."
     )
     if len(sys.argv) == 1:
@@ -44,8 +45,13 @@
         "-v", "--verbose", action="count", default=0, help="Increase verbosity level."
     )
     parser.add_argument(
         "--overwrite",
         action="store_true",
         help="Overwrite the existing commit instead of creating a new one.",
     )
+    parser.add_argument(
+        "--no-preserve-author",
+        action="store_true",
+        help="Do not preserve the original commit author when overwriting.",
+    )
     return parser.parse_args(namespace=HashCommitArgs())
```

### Comparing `hashcommit-0.1.1/hashcommit/commit.py` & `hashcommit-0.1.2/hashcommit/commit.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 import subprocess
 from datetime import datetime, timedelta
 from typing import Callable, Dict, Optional, Tuple
 
 from .args import MatchType
 from .git import (
     create_git_env,
-    get_commit_hash,
     get_head_hash,
     get_parent_head_hash,
     get_tree_hash,
-    will_commits_be_signed,
+    run_commit_tree,
 )
 
 
 def create_a_commit(message: str, timestamp: str) -> subprocess.CompletedProcess:
     return subprocess.run(
         ["git", "commit", "--allow-empty", "-m", message],
-        env=create_git_env(timestamp),
+        env=create_git_env(timestamp, preserve_author=False),
         stdout=subprocess.PIPE,
         check=True,
     )
 
 
 def create_commit_content(message: Optional[str], number: int) -> str:
     return f"""\
@@ -32,15 +31,16 @@
 
 
 def find_commit_content(
     desired_hash: str,
     message: str,
     match_type: MatchType,
     tree_hash: str,
-    head_hash: str,
+    head_hash: Optional[str],
+    preserve_author: bool,
 ) -> Tuple[str, str]:
 
     def compare(value: str) -> bool:
         mapping: Dict[MatchType, Callable[[], bool]] = {
             MatchType.BEGIN: lambda: value.startswith(desired_hash),
             MatchType.END: lambda: value.endswith(desired_hash),
             MatchType.CONTAIN: lambda: desired_hash in value,
@@ -49,15 +49,17 @@
 
     timestamp = datetime.now()
     logging.debug(f"Starting from: {timestamp}")
     while True:
         timestamp -= timedelta(seconds=1)
         timestamp_str = timestamp.astimezone().strftime("%a %b %d %H:%M:%S %Y %z")
         content = message
-        commit_hash = get_commit_hash(content, timestamp_str, tree_hash, head_hash)
+        commit_hash = run_commit_tree(
+            tree_hash, content, timestamp_str, head_hash, preserve_author
+        )
 
         if compare(commit_hash):
             logging.debug(f"End timestamp: {timestamp}")
             print(f"Found matching commit hash: {commit_hash}")
             return content, timestamp_str
 
 
@@ -66,58 +68,73 @@
 ) -> None:
     logging.debug(f"Creating a commit with hash: {desired_hash} ({match_type})")
     head_hash = get_head_hash()
     logging.debug(f"HEAD: {head_hash}")
     tree_hash = get_tree_hash()
     logging.debug(f"Tree: {tree_hash}")
     content, timestamp = find_commit_content(
-        desired_hash, message, match_type, tree_hash, head_hash
+        desired_hash=desired_hash,
+        message=message,
+        match_type=match_type,
+        tree_hash=tree_hash,
+        head_hash=head_hash,
+        preserve_author=False,
     )
-    create_a_commit(content, timestamp)
+    create_a_commit(message=content, timestamp=timestamp)
 
 
 def get_commit_message() -> str:
     result = subprocess.run(
         ["git", "log", "-1", "--pretty=%B"],
         stdout=subprocess.PIPE,
         check=True,
     )
     return result.stdout.decode("utf-8").strip()
 
 
 def amend_a_commit(
-    timestamp: str, tree_hash: str, parent_hash: str, content: str
+    timestamp: str,
+    tree_hash: str,
+    parent_hash: str,
+    content: str,
+    preserve_author: bool,
 ) -> None:
-    commit_env = create_git_env(timestamp)
-    args = ["git", "commit-tree", tree_hash, "-m", content, "-p", parent_hash]
-    if will_commits_be_signed():
-        args.append("-S")
-
-    result = subprocess.run(
-        args,
-        stdout=subprocess.PIPE,
-        env=commit_env,
-        check=True,
+    new_commit_hash = run_commit_tree(
+        tree_hash=tree_hash,
+        content=content,
+        timestamp=timestamp,
+        head_hash=parent_hash,
+        preserve_author=preserve_author,
     )
-    new_commit_hash = result.stdout.decode("utf-8").strip()
-
     subprocess.run(
         ["git", "reset", "--hard", new_commit_hash],
         check=True,
     )
 
 
 def overwrite_a_commit_with_hash(
     desired_hash: str,
     message: Optional[str],
     match_type: MatchType,
+    preserve_author: bool,
 ) -> None:
     logging.debug(f"Overwriting a commit with hash: {desired_hash} ({match_type})")
     head_hash = get_parent_head_hash()
     logging.debug(f"HEAD^: {head_hash}")
     tree_hash = get_tree_hash()
     logging.debug(f"Tree: {tree_hash}")
     commit_message = message or get_commit_message()
     content, timestamp = find_commit_content(
-        desired_hash, commit_message, match_type, tree_hash, head_hash
+        desired_hash=desired_hash,
+        message=commit_message,
+        match_type=match_type,
+        tree_hash=tree_hash,
+        head_hash=head_hash,
+        preserve_author=preserve_author,
+    )
+    amend_a_commit(
+        timestamp=timestamp,
+        tree_hash=tree_hash,
+        parent_hash=head_hash,
+        content=content,
+        preserve_author=preserve_author,
     )
-    amend_a_commit(timestamp, tree_hash, head_hash, content)
```

### Comparing `hashcommit-0.1.1/hashcommit/git.py` & `hashcommit-0.1.2/hashcommit/git.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import subprocess
-from typing import Dict
+from typing import Dict, Optional
 
 
 def is_in_git_repo() -> bool:
     return (
         subprocess.run(
             ["git", "rev-parse", "--is-inside-work-tree"],
             check=False,
@@ -23,44 +23,63 @@
             stderr=subprocess.PIPE,
         )
         return True
     except subprocess.CalledProcessError:
         return False
 
 
-def create_git_env(timestamp: str) -> Dict[str, str]:
+def create_git_env(timestamp: str, preserve_author: bool) -> Dict[str, str]:
+    env = os.environ.copy()
+
+    if preserve_author:
+        env.pop("GIT_AUTHOR_NAME", None)
+        env.pop("GIT_AUTHOR_EMAIL", None)
+        env.pop("GIT_COMMITTER_NAME", None)
+        env.pop("GIT_COMMITTER_EMAIL", None)
+
+        result = subprocess.run(
+            ["git", "show", "-s", "--format=%an|%ae|%cn|%ce"],
+            stdout=subprocess.PIPE,
+            check=True,
+        )
+        author_name, author_email, committer_name, committer_email = (
+            result.stdout.decode("utf-8").strip().split("|")
+        )
+
+        env["GIT_AUTHOR_NAME"] = author_name
+        env["GIT_AUTHOR_EMAIL"] = author_email
+        env["GIT_COMMITTER_NAME"] = committer_name
+        env["GIT_COMMITTER_EMAIL"] = committer_email
+
     return {
-        **os.environ,
+        **env,
         "GIT_AUTHOR_DATE": timestamp,
         "GIT_COMMITTER_DATE": timestamp,
     }
 
 
 def get_tree_hash() -> str:
     result = subprocess.run(
         ["git", "write-tree"],
         stdout=subprocess.PIPE,
         check=True,
     )
     return result.stdout.decode("utf-8").strip()
 
 
-def get_head_hash() -> str:
+def get_head_hash() -> Optional[str]:
     try:
         result = subprocess.run(
             ["git", "rev-parse", "HEAD"],
             stdout=subprocess.PIPE,
             check=True,
         )
-        value = result.stdout.decode("utf-8").strip()
-        if not value:
-            raise ValueError("Empty HEAD hash")
-        return value
+        return result.stdout.decode("utf-8").strip()
     except subprocess.CalledProcessError:
-        raise ValueError("Failed to get HEAD hash")
+        return None
 
 
 def get_parent_head_hash() -> str:
     try:
         result = subprocess.run(
             ["git", "rev-parse", "HEAD^"],
             stdout=subprocess.PIPE,
@@ -79,22 +98,26 @@
         ["git", "config", "commit.gpgSign"],
         stdout=subprocess.PIPE,
         check=False,
     )
     return result.returncode == 0 and result.stdout.decode("utf-8").strip() == "true"
 
 
-def get_commit_hash(
-    content: str, timestamp: str, tree_hash: str, head_hash: str
+def run_commit_tree(
+    tree_hash: str,
+    content: str,
+    timestamp: str,
+    head_hash: Optional[str],
+    preserve_author: bool,
 ) -> str:
-    if not head_hash:
-        raise NotImplementedError("Handling empty repositories is not implemented yet")
-    args = ["git", "commit-tree", tree_hash, "-m", content, "-p", head_hash]
+    args = ["git", "commit-tree", tree_hash, "-m", content]
+    if head_hash:
+        args.extend(["-p", head_hash])
     if will_commits_be_signed():
         args.append("-S")
     result = subprocess.run(
         args,
         stdout=subprocess.PIPE,
-        env=create_git_env(timestamp),
+        env=create_git_env(timestamp, preserve_author),
         check=True,
     )
     return result.stdout.decode("utf-8").strip()
```

### Comparing `hashcommit-0.1.1/hashcommit/main.py` & `hashcommit-0.1.2/hashcommit/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,33 +22,41 @@
         return 1
 
     if not is_in_git_repo():
         print("fatal: not a git repository", file=sys.stderr)
         return 1
 
     try:
-        if not does_repo_have_any_commits():
-            raise NotImplementedError(
-                "Handling empty repositories is not implemented yet"
-            )
 
         if args.overwrite:
             overwrite_a_commit_with_hash(
-                args.hash,
-                args.message,
-                args.match_type,
+                desired_hash=args.hash,
+                message=args.message,
+                match_type=args.match_type,
+                preserve_author=not args.no_preserve_author,
             )
         else:
             if not args.message:
                 print(
                     "Error: --message argument is required if not using --overwrite.",
                     file=sys.stderr,
                 )
                 return 1
-            create_a_commit_with_hash(args.hash, args.message, args.match_type)
+            if not does_repo_have_any_commits():
+                if not args.message:
+                    print(
+                        "Error: --message argument is required if the repository is empty.",
+                        file=sys.stderr,
+                    )
+                    return 1
+            create_a_commit_with_hash(
+                desired_hash=args.hash,
+                message=args.message,
+                match_type=args.match_type,
+            )
     except KeyboardInterrupt:
         print("\nProcess interrupted by user")
         return 3
     except RuntimeError as e:
         print(f"Error: {e}", file=sys.stderr)
         return 2
```

### Comparing `hashcommit-0.1.1/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.2/hashcommit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hashcommit
 
 A tool to generate a Git commit with a specific hash part.
 
+## Prerequisites
+
+Ensure you have Git installed on your system.
+
 ## Installation
 
 You can install the package using pip:
 
 ```sh
 pip install hashcommit
 ```
@@ -67,15 +71,19 @@
 Date:   Thu May 23 17:06:24 2024 +0000
 
     foobar
 ```
 
 ### Author Preservation
 
-By default, the author is not preserved and gets overwritten when overwriting a commit. This feature will be implemented in the future.
+By default, the author is preserved when overwriting. To overwrite the author, use the `--no-preserve-author` option:
+
+```sh
+hashcommit --hash <desired_hash_part> --overwrite --no-preserve-author
+```
 
 ### Overwriting Commits in the Past
 
 Overwriting a particular commit in the past will be implemented in the future.
 
 ## Development
 
@@ -104,13 +112,13 @@
 ```sh
 tox -e format && tox -e checks && tox -e py311 --
 ```
 
 To set up an environment with `hashcommit` installed and a git repository initialized in the `/repo` directory, use Docker Compose:
 
 ```sh
-docker compose run --rm tests bash
+docker compose run --rm test bash
 ```
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `hashcommit-0.1.1/setup.py` & `hashcommit-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.1/tests/test_errors.py` & `hashcommit-0.1.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.1/tests/test_existing_repo.py` & `hashcommit-0.1.2/tests/test_existing_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,18 @@
     assert result.returncode == 0
 
     git_log = get_git_log(initialized_git_repo)
     assert len(git_log) == 2
     assert git_log[0].hash.startswith("1")
 
 
-@pytest.mark.xfail(reason="Not implemented yet")
-def test_preserving_original_commit_author(initialized_git_repo: Path) -> None:
+@pytest.mark.parametrize("preserve_author", [True, False])
+def test_preserving_original_commit_author(
+    initialized_git_repo: Path, preserve_author: bool
+) -> None:
     run_git_command(["config", "user.name", "User1"], cwd=initialized_git_repo)
     run_git_command(
         ["config", "user.email", "user1@user.com"], cwd=initialized_git_repo
     )
 
     result = run_hashcommit(
         ["--hash", "0", "--message", "test"],
@@ -59,18 +61,25 @@
     assert git_log[0].author == "User1"
 
     run_git_command(["config", "user.name", "User2"], cwd=initialized_git_repo)
     run_git_command(
         ["config", "user.email", "user2@user.com"], cwd=initialized_git_repo
     )
 
+    args = ["--hash", "1", "--overwrite"]
+    if not preserve_author:
+        args.append("--no-preserve-author")
+
     result = run_hashcommit(
-        ["--hash", "1", "--overwrite"],
+        args,
         cwd=initialized_git_repo,
     )
     assert result.returncode == 0
 
     git_log = get_git_log(initialized_git_repo)
     assert len(git_log) == 2
     assert git_log[0].hash.startswith("1")
 
-    assert git_log[0].author == "User1"
+    if preserve_author:
+        assert git_log[0].author == "User1"
+    else:
+        assert git_log[0].author == "User2"
```

