# Comparing `tmp/hashcommit-0.1.4.tar.gz` & `tmp/hashcommit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.4.tar", last modified: Fri May 31 14:32:25 2024, max compression
+gzip compressed data, was "hashcommit-0.1.5.tar", last modified: Fri May 31 15:54:17 2024, max compression
```

## Comparing `hashcommit-0.1.4.tar` & `hashcommit-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 14:32:15.000000 hashcommit-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:32:25.262205 hashcommit-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 14:32:15.000000 hashcommit-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 14:32:15.000000 hashcommit-0.1.4/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:32:25.000000 hashcommit-0.1.4/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:32:25.262205 hashcommit-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 14:32:15.000000 hashcommit-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:32:25.262205 hashcommit-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 14:32:15.000000 hashcommit-0.1.4/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 15:54:02.000000 hashcommit-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 15:54:17.670912 hashcommit-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 15:54:02.000000 hashcommit-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.666912 hashcommit-0.1.5/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:54:17.670912 hashcommit-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 15:54:02.000000 hashcommit-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.4/LICENSE` & `hashcommit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/PKG-INFO` & `hashcommit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.4/README.md` & `hashcommit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/hashcommit/args.py` & `hashcommit-0.1.5/hashcommit/args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/hashcommit/commit.py` & `hashcommit-0.1.5/hashcommit/commit.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/hashcommit/git.py` & `hashcommit-0.1.5/hashcommit/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 
 
 def create_git_env(
     timestamp: str, preserve_author: bool, related_commit_hash: Optional[str]
 ) -> Dict[str, str]:
     env = os.environ.copy()
 
+    if does_repo_have_any_commits():
+        args = ["git", "show", "-s", "--format=%ad"]
+        if related_commit_hash:
+            args.append(related_commit_hash)
+        result = run_subprocess(args)
+        author_date = result.stdout.decode("utf-8").strip()
+    else:
+        author_date = timestamp
+
     if preserve_author:
         env.pop("GIT_AUTHOR_NAME", None)
         env.pop("GIT_AUTHOR_EMAIL", None)
         env.pop("GIT_COMMITTER_NAME", None)
         env.pop("GIT_COMMITTER_EMAIL", None)
 
         args = ["git", "show", "-s", "--format=%an|%ae|%cn|%ce"]
@@ -41,15 +50,15 @@
         env["GIT_AUTHOR_NAME"] = author_name
         env["GIT_AUTHOR_EMAIL"] = author_email
         env["GIT_COMMITTER_NAME"] = committer_name
         env["GIT_COMMITTER_EMAIL"] = committer_email
 
     return {
         **env,
-        "GIT_AUTHOR_DATE": timestamp,
+        "GIT_AUTHOR_DATE": author_date,
         "GIT_COMMITTER_DATE": timestamp,
     }
 
 
 def get_tree_hash(commit: Optional[str] = None) -> str:
     args = ["git", "show", "-s", "--format=%T"]
     if commit:
```

### Comparing `hashcommit-0.1.4/hashcommit/main.py` & `hashcommit-0.1.5/hashcommit/main.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.5/hashcommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.4/setup.py` & `hashcommit-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/tests/test_args.py` & `hashcommit-0.1.5/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/tests/test_empty_repo.py` & `hashcommit-0.1.5/tests/test_empty_repo.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/tests/test_errors.py` & `hashcommit-0.1.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.4/tests/test_existing_repo.py` & `hashcommit-0.1.5/tests/test_existing_repo.py`

 * *Files identical despite different names*

