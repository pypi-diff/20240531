# Comparing `tmp/resticpy-1.0.4.tar.gz` & `tmp/resticpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resticpy-1.0.4.tar", last modified: Sat Dec  2 20:20:30 2023, max compression
+gzip compressed data, was "resticpy-1.0.5.tar", last modified: Thu May 30 22:18:08 2024, max compression
```

## Comparing `resticpy-1.0.4.tar` & `resticpy-1.0.5.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-12-02 20:20:30.000000 resticpy-1.0.4/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3523 2023-12-02 20:20:30.000000 resticpy-1.0.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2381 2023-12-02 20:20:22.000000 resticpy-1.0.4/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-12-02 20:20:30.000000 resticpy-1.0.4/restic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3041 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      170 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/errors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-12-02 20:20:30.000000 resticpy-1.0.4/restic/internal/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/backup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8233 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/backup_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      465 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/cat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1718 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/cat_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      439 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/check.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1143 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/check_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/command_executor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      361 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/copy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      793 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/copy_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/find.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7020 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/find_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1791 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/forget.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11363 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/forget_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/generate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1789 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/generate_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      987 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/init.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/init_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1083 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/key.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1865 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/key_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      366 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/list_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/restore.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1422 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/restore_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      613 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/rewrite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2333 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/rewrite_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      166 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/self_update.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      357 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/self_update_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/snapshots.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2742 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/snapshots_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1155 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/stats_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/unlock.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      341 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/unlock_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      489 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      662 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/internal/version_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2207 2023-12-02 20:20:22.000000 resticpy-1.0.4/restic/restic_test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-12-02 20:20:30.000000 resticpy-1.0.4/resticpy.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3523 2023-12-02 20:20:30.000000 resticpy-1.0.4/resticpy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1231 2023-12-02 20:20:30.000000 resticpy-1.0.4/resticpy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-12-02 20:20:30.000000 resticpy-1.0.4/resticpy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-12-02 20:20:30.000000 resticpy-1.0.4/resticpy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-12-02 20:20:30.000000 resticpy-1.0.4/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2023-12-02 20:20:22.000000 resticpy-1.0.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 22:18:08.714954 resticpy-1.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-05-30 22:17:57.000000 resticpy-1.0.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2754 2024-05-30 22:18:08.714954 resticpy-1.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2024-05-30 22:17:57.000000 resticpy-1.0.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 22:18:08.686953 resticpy-1.0.5/restic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3041 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/errors.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 22:18:08.710954 resticpy-1.0.5/restic/internal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/backup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8233 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/backup_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/cat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1718 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/cat_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      439 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1143 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/check_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      855 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/command_executor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/copy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      793 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/copy_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/find.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7020 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/find_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/forget.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12365 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/forget_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      550 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/generate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/generate_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1907 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/init_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1083 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1865 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/key_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      798 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/list_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      460 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/restore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1795 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/restore_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/rewrite.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2333 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/rewrite_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/self_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/self_update_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/snapshots.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6737 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/snapshots_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/stats_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/unlock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/unlock_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      662 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/internal/version_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2207 2024-05-30 22:17:57.000000 resticpy-1.0.5/restic/restic_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 22:18:08.714954 resticpy-1.0.5/resticpy.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2754 2024-05-30 22:18:08.000000 resticpy-1.0.5/resticpy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-05-30 22:18:08.000000 resticpy-1.0.5/resticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-30 22:18:08.000000 resticpy-1.0.5/resticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-30 22:18:08.000000 resticpy-1.0.5/resticpy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-30 22:18:08.714954 resticpy-1.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2024-05-30 22:17:57.000000 resticpy-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `resticpy-1.0.4/README.md` & `resticpy-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## Example
 
 I personally use this library for my backups. I've published my backup script at [mtlynch/mtlynch-backup](https://github.com/mtlynch/mtlynch-backup).
 
 ## Compatibility
 
-resticpy is tested against [restic 0.16.0](https://github.com/restic/restic/releases/tag/v0.16.0).
+resticpy is tested against [restic 0.16.2](https://github.com/restic/restic/releases/tag/v0.16.2).
 
 ## resticpy's scope and future
 
 resticpy is maintained by [Michael Lynch](https://mtlynch.io) as a hobby project.
 
 resticpy is **not** meant to achieve feature parity with restic. It is meant to cover a small subset of the most useful features of restic.
```

### Comparing `resticpy-1.0.4/restic/__init__.py` & `resticpy-1.0.5/restic/__init__.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/backup.py` & `resticpy-1.0.5/restic/internal/backup.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/backup_test.py` & `resticpy-1.0.5/restic/internal/backup_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/cat_test.py` & `resticpy-1.0.5/restic/internal/cat_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/check_test.py` & `resticpy-1.0.5/restic/internal/check_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/command_executor.py` & `resticpy-1.0.5/restic/internal/command_executor.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/copy_test.py` & `resticpy-1.0.5/restic/internal/copy_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/find_test.py` & `resticpy-1.0.5/restic/internal/find_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/forget.py` & `resticpy-1.0.5/restic/internal/forget.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/forget_test.py` & `resticpy-1.0.5/restic/internal/forget_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,23 +41,44 @@
     @mock.patch.object(forget.command_executor, 'execute')
     def test_forget_with_single_tag(self, mock_execute):
         mock_execute.return_value = '{}'
         restic.forget(prune=True, tags=['musician1'])
         mock_execute.assert_called_with(
             ['restic', '--json', 'forget', '--tag', 'musician1', '--prune'])
 
+    # See restic documentation:
+    # https://restic.readthedocs.io/en/latest/060_forget.html#removing-snapshots-according-to-a-policy
+    #
+    # Remove all but the last snapshot of all snapshots that have either
+    # the foo or bar tag set:
+    # 'restic forget --tag foo --tag bar --keep-last 1'
     @mock.patch.object(forget.command_executor, 'execute')
-    def test_forget_with_multiple_tags(self, mock_execute):
+    def test_forget_with_multiple_tags_with_or_relation(self, mock_execute):
         mock_execute.return_value = '{}'
         restic.forget(prune=True, tags=['musician1', 'musician2'])
         mock_execute.assert_called_with([
             'restic', '--json', 'forget', '--tag', 'musician1', '--tag',
             'musician2', '--prune'
         ])
 
+    # See restic documentation:
+    # https://restic.readthedocs.io/en/latest/060_forget.html#removing-snapshots-according-to-a-policy
+    #
+    # Remove all but the last snapshot of all snapshots that have both
+    # the tag foo and bar set:
+    # 'restic forget --tag foo,bar --keep-last 1'
+    @mock.patch.object(forget.command_executor, 'execute')
+    def test_forget_with_multiple_tags_with_and_relation(self, mock_execute):
+        mock_execute.return_value = '{}'
+        restic.forget(prune=True, tags=['musician1,musician2'])
+        mock_execute.assert_called_with([
+            'restic', '--json', 'forget', '--tag', 'musician1,musician2',
+            '--prune'
+        ])
+
     @mock.patch.object(forget.command_executor, 'execute')
     def test_forget_with_host(self, mock_execute):
         mock_execute.return_value = '{}'
         restic.forget(prune=True, host='myhost')
         mock_execute.assert_called_with(
             ['restic', '--json', 'forget', '--host', 'myhost', '--prune'])
```

### Comparing `resticpy-1.0.4/restic/internal/generate.py` & `resticpy-1.0.5/restic/internal/generate.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/generate_test.py` & `resticpy-1.0.5/restic/internal/generate_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/init.py` & `resticpy-1.0.5/restic/internal/init.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/init_test.py` & `resticpy-1.0.5/restic/internal/init_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/key.py` & `resticpy-1.0.5/restic/internal/key.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/key_test.py` & `resticpy-1.0.5/restic/internal/key_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/list_test.py` & `resticpy-1.0.5/restic/internal/list_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/restore_test.py` & `resticpy-1.0.5/restic/internal/restore_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,7 +31,15 @@
     @mock.patch.object(restore.command_executor, 'execute')
     def test_restore_specific_snapshot_id_and_include(self, mock_execute):
         restic.restore(snapshot_id='dummy-snapshot-id', include='include-path')
         mock_execute.assert_called_with([
             'restic', '--json', 'restore', 'dummy-snapshot-id', '--include',
             'include-path'
         ])
+
+    @mock.patch.object(restore.command_executor, 'execute')
+    def test_restore_specific_snapshot_id_and_exclude(self, mock_execute):
+        restic.restore(snapshot_id='dummy-snapshot-id', exclude='exclude-path')
+        mock_execute.assert_called_with([
+            'restic', '--json', 'restore', 'dummy-snapshot-id', '--exclude',
+            'exclude-path'
+        ])
```

### Comparing `resticpy-1.0.4/restic/internal/rewrite.py` & `resticpy-1.0.5/restic/internal/rewrite.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/rewrite_test.py` & `resticpy-1.0.5/restic/internal/rewrite_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/restic/internal/stats_test.py` & `resticpy-1.0.5/restic/internal/stats_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,7 +36,39 @@
                 'total_size': 20,
                 'total_file_count': 1,
                 'total_blob_count': 1
             }, restic.stats(mode='blobs-per-file'))
 
         mock_execute.assert_called_with(
             ['restic', '--json', 'stats', '--mode', 'blobs-per-file'])
+
+    @mock.patch.object(stats.command_executor, 'execute')
+    def test_stats_with_tag(self, mock_execute):
+        mock_execute.return_value = """{
+            "total_size": 10,
+            "total_file_count": 2
+            }
+            """
+
+        self.assertEqual({
+            'total_size': 10,
+            'total_file_count': 2
+        }, restic.stats(tags=['musician1']))
+
+        mock_execute.assert_called_with(
+            ['restic', '--json', 'stats', '--tag', 'musician1'])
+
+    @mock.patch.object(stats.command_executor, 'execute')
+    def test_stats_with_host(self, mock_execute):
+        mock_execute.return_value = """{
+            "total_size": 10,
+            "total_file_count": 2
+            }
+            """
+
+        self.assertEqual({
+            'total_size': 10,
+            'total_file_count': 2
+        }, restic.stats(host='myhost'))
+
+        mock_execute.assert_called_with(
+            ['restic', '--json', 'stats', '--host', 'myhost'])
```

### Comparing `resticpy-1.0.4/restic/internal/version_test.py` & `resticpy-1.0.5/restic/internal/version_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 
 class VersionTest(unittest.TestCase):
 
     @mock.patch.object(version.command_executor, 'execute')
     def test_version(self, mock_execute):
         mock_execute.return_value = (
-            'restic 0.16.0 compiled with go1.20.6 on windows/amd64')
+            'restic 0.16.2 compiled with go1.20.6 on windows/amd64')
 
         self.assertEqual(
             {
                 'architecture': 'amd64',
                 'go_version': '1.20.6',
                 'platform_version': 'windows',
-                'restic_version': '0.16.0'
+                'restic_version': '0.16.2'
             }, restic.version())
 
         mock_execute.assert_called_with(['restic', '--json', 'version'])
```

### Comparing `resticpy-1.0.4/restic/restic_test.py` & `resticpy-1.0.5/restic/restic_test.py`

 * *Files identical despite different names*

### Comparing `resticpy-1.0.4/resticpy.egg-info/SOURCES.txt` & `resticpy-1.0.5/resticpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 restic/__init__.py
 restic/errors.py
 restic/restic_test.py
 restic/internal/__init__.py
 restic/internal/backup.py
```

### Comparing `resticpy-1.0.4/setup.py` & `resticpy-1.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     name='resticpy',
     long_description=open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)),
                      'README.md')).read(),
     long_description_content_type="text/markdown",
-    version='1.0.4',
+    version='1.0.5',
     description='Restic backup Python wrapper',
     project_urls={
         "repository": "https://github.com/mtlynch/resticpy",
     },
     author='Michael Lynch',
     author_email='michael@mtlynch.io',
     license="MIT",
```

