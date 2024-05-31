# Comparing `tmp/roastery-0.20240530.dev0.tar.gz` & `tmp/roastery-0.20240531.dev0.tar.gz`

## Comparing `roastery-0.20240530.dev0.tar` & `roastery-0.20240531.dev0.tar`

### file list

```diff
@@ -1,12 +1,48 @@
--rw-r--r--   0        0        0      375 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/__init__.py
--rw-r--r--   0        0        0      807 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/cli.py
--rw-r--r--   0        0        0     2246 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/config.py
--rw-r--r--   0        0        0     4143 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/edit.py
--rw-r--r--   0        0        0     2742 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/formats.py
--rw-r--r--   0        0        0     9090 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/importer.py
--rw-r--r--   0        0        0     4220 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/roastery/term.py
--rw-r--r--   0        0        0      100 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/.gitignore
--rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/LICENSE
--rw-r--r--   0        0        0     1694 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/README.md
--rw-r--r--   0        0        0      761 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/pyproject.toml
--rw-r--r--   0        0        0     2074 1980-01-01 00:00:00.000000 roastery-0.20240530.dev0/PKG-INFO
+-rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.envrc
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.python-version
+-rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/CNAME
+-rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/flake.lock
+-rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/flake.nix
+-rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/requirements-dev.lock
+-rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/requirements.lock
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/.gitignore
+-rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/misc.xml
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/modules.xml
+-rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/roastery.iml
+-rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2153 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/workspace.xml
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/bin/docs.sh
+-rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/bin/pypi.sh
+-rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/bin/refs.sh
+-rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/bin/test-pypi.sh
+-rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/bin/upload-docs.sh
+-rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/.gitignore
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/.python-version
+-rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/architecture.rst
+-rw-r--r--   0        0        0     1013 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/conf.py
+-rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/index.rst
+-rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/todo.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/cli.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/config.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/edit.rst
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/formats.rst
+-rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/importer.rst
+-rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/index.rst
+-rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/api/term.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/documentation/getting-started/index.rst
+-rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/nix/roastery.nix
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/nix/shell.nix
+-rw-r--r--   0        0        0      375 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/__init__.py
+-rw-r--r--   0        0        0      807 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/cli.py
+-rw-r--r--   0        0        0     2246 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/config.py
+-rw-r--r--   0        0        0     4143 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/edit.py
+-rw-r--r--   0        0        0     2742 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/formats.py
+-rw-r--r--   0        0        0     9494 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/importer.py
+-rw-r--r--   0        0        0     4220 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/src/roastery/term.py
+-rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/.gitignore
+-rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/LICENSE
+-rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/README.md
+-rw-r--r--   0        0        0      699 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240531.dev0/PKG-INFO
```

### Comparing `roastery-0.20240530.dev0/roastery/cli.py` & `roastery-0.20240531.dev0/src/roastery/cli.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/roastery/config.py` & `roastery-0.20240531.dev0/src/roastery/config.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/roastery/edit.py` & `roastery-0.20240531.dev0/src/roastery/edit.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/roastery/formats.py` & `roastery-0.20240531.dev0/src/roastery/formats.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/roastery/importer.py` & `roastery-0.20240531.dev0/src/roastery/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,23 @@
             narration=self.narration.value,
             meta={k: str(v) for k, v in self.meta.items()},
             tags=self.tags,
             links=self.links,
             flag=self.flag,
         )
 
-    def apply_manual_edits(self, edits: dict[Digest, ManualEdits]):
-        """Apply a user's manual edits to this entry."""
+    def apply_manual_edits(self, edits: dict[Digest, ManualEdits]) -> None:
+        """Apply manual edits to this entry.
+
+        :param edits: Dictionary of manual edits, as deserialized from
+          :py:obj:`roastery.config.Config.manual_edits_path`. The keys
+          are the digests of the entires. The values are
+          :py:class:`roastery.edit.ManualEdits` containing the updated
+          field values.
+        """
         if o := edits.get(self.digest):
             self.payee.edited = o.get("payee")
             self.account.edited = o.get("account")
             self.narration.edited = o.get("narration")
             self.tags = set(o.get("tags", []))
             self.links = set(o.get("links", []))
 
@@ -252,15 +259,16 @@
 
     The resulting Beancount file is created in the same directory as the CSV file, but with
     the extension changed to ``.beancount``. So: ``statements/foo.csv`` -> ``statements/foo.beancount``
     You can specify a different path with the ``beancount_file`` parameter.
 
     :param csv_file: Path of the CSV file to import.
     :param config: Configuration to use.
-    :param csv_args: Arguments to forward to :py:class:`csv.DictReader`.
+    :param csv_args: Arguments to forward to :py:class:`csv.DictReader`. This is used to
+      parse weird CSV dialects. For example: ``dict(delimiter=";", quotechar="|")``.
     :param extract: How to extract an :class:`Entry` from a row of CSV data. See :py:class:`~ExtractFn`.
     :param clean: User-implemented cleaning function. See :py:class:`~CleanFn`.
     :param beancount_file: Path of the beancount file to write to.
     """
     beancount_file = csv_file.with_suffix(".beancount") if beancount_file is None else beancount_file
     try:
         manual_edits = json.loads(config.manual_edits_path.read_text())
```

### Comparing `roastery-0.20240530.dev0/roastery/term.py` & `roastery-0.20240531.dev0/src/roastery/term.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/LICENSE` & `roastery-0.20240531.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `roastery-0.20240530.dev0/README.md` & `roastery-0.20240531.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 - **Plays nice with version control** &mdash; Edit one of your automatic rules?
   Re-run your imports, and see the effect with a `git diff`. Manual edits are
   stored separately from original data, and the generated beancount files, so
   you can always re-run your imports.
 
 ## Project status
 
-Roastery is a personal project without stability promise or guarantees and
+Roastery is a personal project without stability promises or guarantees or
 warranty of any kind. I reserve the right to make breaking changes and
 drastically overhaul the project without notice.
 
-Over time, I things to stabilize and will update this notice accordingly.
+Over time, I expect things to stabilize and will update this notice accordingly.
 
 <!-- end-include-doc-landing -->
 
 ## Installation
 
 ```
 $ pip install roastery
```

### Comparing `roastery-0.20240530.dev0/PKG-INFO` & `roastery-0.20240531.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roastery
-Version: 0.20240530.dev0
+Version: 0.20240531.dev0
 Summary: Framework for Beancount plain text accounting
 Author-email: Laurens Duijvesteijn <git@duijf.io>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: beancount>=2.0.0
 Requires-Dist: fava>=1.27.0
 Requires-Dist: prompt-toolkit>=3.0.0
@@ -29,19 +29,19 @@
 - **Plays nice with version control** &mdash; Edit one of your automatic rules?
   Re-run your imports, and see the effect with a `git diff`. Manual edits are
   stored separately from original data, and the generated beancount files, so
   you can always re-run your imports.
 
 ## Project status
 
-Roastery is a personal project without stability promise or guarantees and
+Roastery is a personal project without stability promises or guarantees or
 warranty of any kind. I reserve the right to make breaking changes and
 drastically overhaul the project without notice.
 
-Over time, I things to stabilize and will update this notice accordingly.
+Over time, I expect things to stabilize and will update this notice accordingly.
 
 <!-- end-include-doc-landing -->
 
 ## Installation
 
 ```
 $ pip install roastery
```

