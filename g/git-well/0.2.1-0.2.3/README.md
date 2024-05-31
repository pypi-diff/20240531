# Comparing `tmp/git_well-0.2.1.tar.gz` & `tmp/git_well-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_well-0.2.1.tar", last modified: Fri Feb 23 17:43:53 2024, max compression
+gzip compressed data, was "git_well-0.2.3.tar", last modified: Fri May 31 00:40:43 2024, max compression
```

## Comparing `git_well-0.2.1.tar` & `git_well-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:53.165739 git_well-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-02-23 17:43:53.165739 git_well-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-02-23 17:43:31.000000 git_well-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:53.137739 git_well-0.2.1/git_well/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:53.137739 git_well-0.2.1/git_well/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_autoconf_gpgsign.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_autoconf_gpgsign.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_branch_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_branch_cleanup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_branch_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_branch_upgrade.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_discover_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_discover_remote.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_rebase_add_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_rebase_add_continue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_remote_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_remote_protocol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    43738 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_squash_streaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_squash_streaks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_stats.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_sync.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_track_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/git_track_upstream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-23 17:43:31.000000 git_well-0.2.1/git_well/repo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:53.137739 git_well-0.2.1/git_well.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 17:43:53.000000 git_well-0.2.1/git_well.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-23 17:43:31.000000 git_well-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 17:43:53.165739 git_well-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9707 2024-02-23 17:43:31.000000 git_well-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:43:53.137739 git_well-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-23 17:43:31.000000 git_well-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 17:43:31.000000 git_well-0.2.1/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:43.122413 git_well-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-05-31 00:40:43.122413 git_well-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-31 00:40:27.000000 git_well-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:43.098413 git_well-0.2.3/git_well/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:43.098413 git_well-0.2.3/git_well/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_autoconf_gpgsign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_autoconf_gpgsign.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_branch_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_branch_cleanup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_branch_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_branch_upgrade.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_discover_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_discover_remote.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_rebase_add_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_rebase_add_continue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_remote_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_remote_protocol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    43738 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_squash_streaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_squash_streaks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_sync.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_track_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/git_track_upstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 00:40:27.000000 git_well-0.2.3/git_well/repo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:43.098413 git_well-0.2.3/git_well.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 00:40:43.000000 git_well-0.2.3/git_well.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-31 00:40:27.000000 git_well-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:40:43.122413 git_well-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9707 2024-05-31 00:40:27.000000 git_well-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:40:43.098413 git_well-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-31 00:40:27.000000 git_well-0.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:40:27.000000 git_well-0.2.3/tests/test_import.py
```

### Comparing `git_well-0.2.1/PKG-INFO` & `git_well-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_well
-Version: 0.2.1
+Version: 0.2.3
 Summary: The git_well module
 Home-page: https://github.com/Erotemic/git_well
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `git_well-0.2.1/README.rst` & `git_well-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/_utils.py` & `git_well-0.2.3/git_well/_utils.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/demo/__init__.py` & `git_well-0.2.3/git_well/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_autoconf_gpgsign.py` & `git_well-0.2.3/git_well/git_autoconf_gpgsign.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class GitAutoconfGpgsignCLI(scfg.DataConfig):
     __command__ = 'autoconf-gpg'
 
     remote = scfg.Value(None, help='param1')
     repo_dpath = scfg.Value('.', help='repo to set gpg for')
+    email = scfg.Value(None, help='The email the the signing GPG key is associated with. If unspecified attempt to infer via ssh credentials')
 
     @classmethod
     def main(cls, cmdline=1, **kwargs):
         """
         Example:
             >>> # xdoctest: +SKIP
             >>> from git_well.git_autoconf_gpgsign import *  # NOQA
@@ -50,34 +51,40 @@
             for line in info.stderr.split('\n'):
                 if 'identity file' in line:
                     cand = line.split(' ')[3]
                     cand = ub.Path(cand)
                     if cand.exists():
                         identify_file_cands.add(cand)
 
-        email_candidates = ub.oset()
-        for id_fpath in identify_file_cands:
-            pub_key_fpath = id_fpath.augment(tail='.pub')
-            if pub_key_fpath.exists():
-                pub_email = pub_key_fpath.read_text().strip().split(' ')[-1]
-                email_candidates.add(pub_email)
+        if config.email is None:
+            email_candidates = ub.oset()
+            for id_fpath in identify_file_cands:
+                pub_key_fpath = id_fpath.augment(tail='.pub')
+                if pub_key_fpath.exists():
+                    pub_email = pub_key_fpath.read_text().strip().split(' ')[-1]
+                    email_candidates.add(pub_email)
+        else:
+            email_candidates = [config.email]
 
         gpg_candidates = []
         for email in email_candidates:
             # info = ub.cmd(f'gpg --list-keys --keyid-format LONG "{email}"')
             # print(info.stdout)
             # entries = gpg_entries(email)
             candidates = lookup_gpg_keyinfos(
                 email, verbose=0, allow_mainkey=False, capabilities='sign',
                 mintrust='u')
             gpg_candidates.extend(candidates)
 
         unique_fprs = {cand['fpr'] for cand in gpg_candidates}
 
-        if len(unique_fprs) != 1:
+        if len(unique_fprs) == 0:
+            raise Exception('Unable to find any gpg candidates. '
+                            'Is the repo not using git/ssh credentials?')
+        elif len(unique_fprs) != 1:
             print(f'unique_fprs = {ub.urepr(unique_fprs, nl=1)}')
             print('gpg_candidates = {}'.format(ub.urepr(gpg_candidates, nl=1)))
             raise AssertionError('need to choose 1')
 
         # assert len(gpg_candidates) == 1
         fpr = ub.peek(unique_fprs)
 
@@ -95,19 +102,22 @@
         repo.cmd(r'git config --local --list | grep "gpg\|sign\|email"', shell=True, verbose=1)
 
 
 def lookup_gpg_keyinfos(identifier, verbose=0, capabilities=None,
                         allow_subkey=True, allow_mainkey=True, full=True,
                         filter_expired=True, mintrust=None):
     """
-    python ~/local/scripts/xgpg.py lookup_keyid "Emmy"
-    python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=sign
-    python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=encrypt
-    python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=auth
-    python ~/local/scripts/xgpg.py lookup_keyid "Jonathan Crall"
+    Creates a table of information about GPG key candidates that match a query.
+
+    Ignore:
+        python ~/local/scripts/xgpg.py lookup_keyid "Emmy"
+        python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=sign
+        python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=encrypt
+        python ~/local/scripts/xgpg.py lookup_keyid "Crall" --allow_mainkey=False --capabilities=auth
+        python ~/local/scripts/xgpg.py lookup_keyid "Jonathan Crall"
     """
     if capabilities is None:
         capabilities = {'certify'}
     if isinstance(capabilities, str):
         capabilities = set(capabilities.split(','))
 
     entries = gpg_entries(identifier)
```

### Comparing `git_well-0.2.1/git_well/git_autoconf_gpgsign.pyi` & `git_well-0.2.3/git_well/git_autoconf_gpgsign.pyi`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_branch_cleanup.py` & `git_well-0.2.3/git_well/git_branch_cleanup.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_branch_upgrade.py` & `git_well-0.2.3/git_well/git_branch_upgrade.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_discover_remote.py` & `git_well-0.2.3/git_well/git_discover_remote.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_rebase_add_continue.py` & `git_well-0.2.3/git_well/git_rebase_add_continue.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_remote_protocol.py` & `git_well-0.2.3/git_well/git_remote_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     group = scfg.Value('special:auto', position=1, help=ub.paragraph(
         '''
         The group for which all matching remotes will have their protocol
         changed. If "special:auto", then attempts to determine what the group
         should be. (i.e. if there is only one, use that, otherwise ask).
         '''))
 
-    protocol = scfg.Value('ssh', position=2, choices=VALID_PROTOCOLS, help=ub.paragraph(
+    protocol = scfg.Value('git', position=2, choices=VALID_PROTOCOLS, help=ub.paragraph(
         '''
         The protocol to change to.
         '''))
 
     repo_dpath = scfg.Value('.', position=3, help=ub.paragraph(
         '''
         A path inside the repo to modify.
```

### Comparing `git_well-0.2.1/git_well/git_remote_protocol.pyi` & `git_well-0.2.3/git_well/git_remote_protocol.pyi`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_squash_streaks.py` & `git_well-0.2.3/git_well/git_squash_streaks.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_squash_streaks.pyi` & `git_well-0.2.3/git_well/git_squash_streaks.pyi`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_stats.py` & `git_well-0.2.3/git_well/git_stats.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_sync.py` & `git_well-0.2.3/git_well/git_sync.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_sync.pyi` & `git_well-0.2.3/git_well/git_sync.pyi`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/git_track_upstream.py` & `git_well-0.2.3/git_well/git_track_upstream.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/main.py` & `git_well-0.2.3/git_well/main.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well/repo.py` & `git_well-0.2.3/git_well/repo.py`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well.egg-info/PKG-INFO` & `git_well-0.2.3/git_well.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_well
-Version: 0.2.1
+Version: 0.2.3
 Summary: The git_well module
 Home-page: https://github.com/Erotemic/git_well
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `git_well-0.2.1/git_well.egg-info/SOURCES.txt` & `git_well-0.2.3/git_well.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/git_well.egg-info/requires.txt` & `git_well-0.2.3/git_well.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/pyproject.toml` & `git_well-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `git_well-0.2.1/setup.py` & `git_well-0.2.3/setup.py`

 * *Files identical despite different names*

