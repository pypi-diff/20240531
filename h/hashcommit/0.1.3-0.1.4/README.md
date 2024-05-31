# Comparing `tmp/hashcommit-0.1.3.tar.gz` & `tmp/hashcommit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.3.tar", last modified: Fri May 31 14:25:29 2024, max compression
+gzip compressed data, was "hashcommit-0.1.4.tar", last modified: Fri May 31 14:32:25 2024, max compression
```

## Comparing `hashcommit-0.1.3.tar` & `hashcommit-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 14:25:20.000000 hashcommit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:25:29.592740 hashcommit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 14:25:20.000000 hashcommit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 14:25:20.000000 hashcommit-0.1.3/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:25:29.000000 hashcommit-0.1.3/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:25:29.592740 hashcommit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 14:25:20.000000 hashcommit-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:25:29.592740 hashcommit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-31 14:25:20.000000 hashcommit-0.1.3/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 14:32:15.000000 hashcommit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:32:25.262205 hashcommit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 14:32:15.000000 hashcommit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:32:25.262205 hashcommit-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 14:32:15.000000 hashcommit-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.3/LICENSE` & `hashcommit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/PKG-INFO` & `hashcommit-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.3/README.md` & `hashcommit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/hashcommit/args.py` & `hashcommit-0.1.4/hashcommit/args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/hashcommit/commit.py` & `hashcommit-0.1.4/hashcommit/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,24 +156,24 @@
         parent_hash=head_hash,
         content=content,
         preserve_author=preserve_author,
         related_commit_hash=current_hash,
     )
 
 
-def get_parent_hash(commit: Optional[str] = None) -> str:
+def get_parent_hash(commit: Optional[str] = None) -> Optional[str]:
     args = ["git", "show", "--no-patch", "--format=%P"]
     if commit:
         args.append(commit)
 
     result = run_subprocess(args)
     parents = result.stdout.decode("utf-8").strip().split()
     if len(parents) > 1:
         raise NotImplementedError("Commit has more than one parent")
-    return parents[0]
+    return parents[0] if parents else None
 
 
 def overwrite_and_rebase(
     desired_hash: str,
     message: Optional[str],
     commit_hash: str,
     preserve_author: bool,
```

### Comparing `hashcommit-0.1.3/hashcommit/git.py` & `hashcommit-0.1.4/hashcommit/git.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/hashcommit/main.py` & `hashcommit-0.1.4/hashcommit/main.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.4/hashcommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.3/setup.py` & `hashcommit-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/tests/test_args.py` & `hashcommit-0.1.4/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/tests/test_empty_repo.py` & `hashcommit-0.1.4/tests/test_empty_repo.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/tests/test_errors.py` & `hashcommit-0.1.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.3/tests/test_existing_repo.py` & `hashcommit-0.1.4/tests/test_existing_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,7 +134,36 @@
         assert git_log[1].author == "User1"
     else:
         assert git_log[1].author == "UserX"
 
     assert git_log[2].message.startswith("test0")
     assert git_log[2].hash.startswith("0")
     assert git_log[2].author == "User0"
+
+
+def test_overwriting_a_first_commit(initialized_git_repo: Path) -> None:
+    run_hashcommit_command(
+        ["--hash", "0", "--message", "test0"],
+        cwd=initialized_git_repo,
+    )
+
+    git_log = get_git_log(initialized_git_repo)
+    assert len(git_log) == 2
+
+    assert git_log[0].hash.startswith("0")
+    assert git_log[0].message.startswith("test0")
+
+    assert git_log[1].message.startswith("Initial commit")
+
+    run_hashcommit_command(
+        ["--hash", "1", "--overwrite", "--commit", git_log[1].hash],
+        cwd=initialized_git_repo,
+    )
+
+    git_log = get_git_log(initialized_git_repo)
+    assert len(git_log) == 2
+
+    # hash may change
+    assert git_log[0].message.startswith("test0")
+
+    assert git_log[1].message.startswith("Initial commit")
+    assert git_log[1].hash.startswith("1")
```

