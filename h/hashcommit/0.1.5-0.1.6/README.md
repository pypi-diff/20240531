# Comparing `tmp/hashcommit-0.1.5.tar.gz` & `tmp/hashcommit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.5.tar", last modified: Fri May 31 15:54:17 2024, max compression
+gzip compressed data, was "hashcommit-0.1.6.tar", last modified: Fri May 31 16:29:38 2024, max compression
```

## Comparing `hashcommit-0.1.5.tar` & `hashcommit-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 15:54:02.000000 hashcommit-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 15:54:17.670912 hashcommit-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 15:54:02.000000 hashcommit-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.666912 hashcommit-0.1.5/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 15:54:02.000000 hashcommit-0.1.5/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 15:54:17.000000 hashcommit-0.1.5/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:54:17.670912 hashcommit-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 15:54:02.000000 hashcommit-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:54:17.670912 hashcommit-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 15:54:02.000000 hashcommit-0.1.5/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:29:38.387385 hashcommit-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 16:29:30.000000 hashcommit-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 16:29:38.387385 hashcommit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-31 16:29:30.000000 hashcommit-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:29:38.387385 hashcommit-0.1.6/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 16:29:30.000000 hashcommit-0.1.6/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:29:38.387385 hashcommit-0.1.6/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 16:29:38.000000 hashcommit-0.1.6/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 16:29:38.000000 hashcommit-0.1.6/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:29:38.000000 hashcommit-0.1.6/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 16:29:38.000000 hashcommit-0.1.6/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 16:29:38.000000 hashcommit-0.1.6/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:29:38.387385 hashcommit-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 16:29:30.000000 hashcommit-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:29:38.387385 hashcommit-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 16:29:30.000000 hashcommit-0.1.6/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 16:29:30.000000 hashcommit-0.1.6/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 16:29:30.000000 hashcommit-0.1.6/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 16:29:30.000000 hashcommit-0.1.6/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.5/LICENSE` & `hashcommit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/PKG-INFO` & `hashcommit-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.5/README.md` & `hashcommit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/hashcommit/args.py` & `hashcommit-0.1.6/hashcommit/args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/hashcommit/commit.py` & `hashcommit-0.1.6/hashcommit/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         timestamp=timestamp,
         head_hash=parent_hash,
         preserve_author=preserve_author,
         related_commit_hash=commit_hash,
     )
 
     logging.debug(f"Replacing {commit_hash} with {new_commit_hash}")
-    subprocess.run(["git", "replace", commit_hash, new_commit_hash], check=True)
+    subprocess.run(["git", "replace", commit_hash, new_commit_hash, "--force"], check=True)
 
     logging.debug(f"Rebasing onto {new_commit_hash}")
     subprocess.run(
         ["git", "rebase", "--onto", new_commit_hash, commit_hash, "HEAD"], check=True
     )
 
     logging.debug(f"Deleting {commit_hash} replacement")
```

### Comparing `hashcommit-0.1.5/hashcommit/git.py` & `hashcommit-0.1.6/hashcommit/git.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/hashcommit/main.py` & `hashcommit-0.1.6/hashcommit/main.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.6/hashcommit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.5/setup.py` & `hashcommit-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/tests/test_args.py` & `hashcommit-0.1.6/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/tests/test_empty_repo.py` & `hashcommit-0.1.6/tests/test_empty_repo.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/tests/test_errors.py` & `hashcommit-0.1.6/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.5/tests/test_existing_repo.py` & `hashcommit-0.1.6/tests/test_existing_repo.py`

 * *Files identical despite different names*

