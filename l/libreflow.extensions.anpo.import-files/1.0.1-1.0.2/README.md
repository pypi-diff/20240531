# Comparing `tmp/libreflow_extensions_anpo_import_files-1.0.1.tar.gz` & `tmp/libreflow_extensions_anpo_import_files-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_import_files-1.0.1.tar", last modified: Fri May 24 14:17:44 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_import_files-1.0.2.tar", last modified: Fri May 31 10:23:04 2024, max compression
```

## Comparing `libreflow_extensions_anpo_import_files-1.0.1.tar` & `libreflow_extensions_anpo_import_files-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.611589 libreflow_extensions_anpo_import_files-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      640 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-24 14:17:44.611589 libreflow_extensions_anpo_import_files-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-05-24 14:17:44.611589 libreflow_extensions_anpo_import_files-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1311 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.605589 libreflow_extensions_anpo_import_files-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.608589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.609589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.610589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.610589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/import_files/
--rw-rw-rw-   0 root         (0) root         (0)     7985 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/import_files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-24 14:17:44.611589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/import_files/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:17:44.610589 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-24 14:17:44.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-24 14:17:44.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:17:44.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 14:17:44.000000 libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-24 14:17:34.000000 libreflow_extensions_anpo_import_files-1.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.678625 libreflow_extensions_anpo_import_files-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1428 2024-05-31 10:23:04.678625 libreflow_extensions_anpo_import_files-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-05-31 10:23:04.678625 libreflow_extensions_anpo_import_files-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.674625 libreflow_extensions_anpo_import_files-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.676625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.677625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.677625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.677625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/import_files/
+-rw-rw-rw-   0 root         (0) root         (0)     8501 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/import_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-31 10:23:04.679625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/import_files/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:23:04.678625 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1428 2024-05-31 10:23:04.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-31 10:23:04.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 10:23:04.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 10:23:04.000000 libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-31 10:22:55.000000 libreflow_extensions_anpo_import_files-1.0.2/versioneer.py
```

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/PKG-INFO` & `libreflow_extensions_anpo_import_files-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.import-files
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -35,14 +35,21 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.2] - 2024-05-31
+
+### Changed
+
+* Use Connection Param on project settings for use the action from a task.
+* Harmonise logs
+
 ## [1.0.1] - 2024-05-24
 
 ### Fixed
 
 * package folder name
 
 ## [1.0.0] - 2024-05-24
```

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/setup.py` & `libreflow_extensions_anpo_import_files-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/src/libreflow/extensions/anpo/import_files/__init__.py` & `libreflow_extensions_anpo_import_files-1.0.2/src/libreflow/extensions/anpo/import_files/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
 from kabaret import flow
 from kabaret.flow.object import _Manager
 from libreflow.utils.flow.import_files import ImportFilesAction as BaseImportFilesAction
+from libreflow.flows.default.flow import Project
+from libreflow.baseflow.film import FilmCollection
+from libreflow.baseflow import ProjectSettings
 
 from . import _version
 __version__ = _version.get_versions()['version']
 
 
 class ANPOImportFilesAction(BaseImportFilesAction):
 
@@ -37,15 +40,15 @@
                     map_items = self.root().project().asset_types.mapped_items()
 
                 for item in reversed(map_items):
                     regexp = pattern.format(name=item.name())
 
                     match = re.search(regexp, file_name)
                     if match:
-                        print(f'ImportFiles :: Find matching {key} ({match.group(0)})')
+                        self.session.log_info(f'[Import Files] Find matching {key} ({match.group(0)})')
                         match_dict[key] = match.group(0)
                         break
 
                 # Set main film if parameter enabled
                 if (
                     key == 'film'
                     and match_dict[key] is None
@@ -69,15 +72,15 @@
                                 regexp = pattern.format(
                                     asset_type=match_dict['asset_type'],
                                     name=item.name()
                                 )
 
                                 match = re.search(regexp, file_name)
                                 if match:
-                                    print(f'ImportFiles :: Find matching {key} ({match.group(0)})')
+                                    self.session.log_info(f'[Import Files] Find matching {key} ({match.group(0)})')
                                     match_dict[key] = match.group(0)
                                     break
                             
                             if match_dict[key]:
                                 continue
                         else:
                             continue
@@ -120,37 +123,37 @@
                                 name_and_doc = [(i["name"], i) for i in cursor]
 
                             if name_and_doc:
                                 if len(name_and_doc) == 1:
                                     oid = name_and_doc[0][0]
 
                                     match_dict['asset_type'] = re.search('(?<=asset_types\/)[^\/]*', oid).group(0)
-                                    print(f'ImportFiles :: Find matching asset_type ({match_dict["asset_type"]})')
+                                    self.session.log_info(f'[Import Files] Find matching asset_type ({match_dict["asset_type"]})')
 
                                     # Check for Asset Family
                                     regexp = '(?<=asset_families\/)[^\/]*'
                                     match = re.search(regexp, oid)
 
                                     if match:
                                         match_dict['asset_family'] = match.group(0)
-                                        print(f'ImportFiles :: Find matching asset_family ({match_dict["asset_family"]})')
+                                        self.session.log_info(f'[Import Files] Find matching asset_family ({match_dict["asset_family"]})')
 
                                 if code:
                                     asset_name = asset_name.replace('-', '_')    
 
                                 match_dict['asset'] = asset_name
-                                print(f'ImportFiles :: Find matching asset ({match_dict["asset"]})')
+                                self.session.log_info(f'[Import Files] Find matching asset ({match_dict["asset"]})')
                                 
                                 continue
 
                         continue
 
                 match = re.search(regexp, file_name)
                 if match:
-                    print(f'ImportFiles :: Find matching {key} ({match.group(0)})')
+                    self.session.log_info(f'[Import Files] Find matching {key} ({match.group(0)})')
                     match_dict[key] = match.group(0)
 
         return match_dict
 
     def create_entities(self, item):
         super(ANPOImportFilesAction, self).create_entities(item)
         
@@ -166,25 +169,30 @@
                 new_entity.code.set(data['name'].replace('_', '-'))
 
                 map_object.touch()
 
 
 def import_files_action(parent):
     # Hide original action
-    if parent.oid() == '/'+parent.name() and parent.name() == "anpo":
+    if isinstance(parent, Project) and parent.name() == "anpo":
         r = flow.Child(flow.Object)
         r.ui(hidden=True)
         r.name = 'import_files'
         return r
     # Recreate action in a sub object
-    if parent.oid() == '/anpo/films':
+    if isinstance(parent, FilmCollection) and 'anpo' in parent.oid():
         r = flow.Child(ANPOImportFilesAction).ui(dialog_size=(800,600))
         r.name = 'import_files'
         r.index = 1
         return r
+    # Relocate relation in project settings
+    if isinstance(parent, ProjectSettings) and 'anpo' in parent.oid():
+        action = parent.root().get_object('/anpo/films/import_files')
+        parent.import_files_object.set(action)
+        return
 
 
 def install_extensions(session):
     return {
         "import_files": [
             import_files_action,
         ]
```

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/PKG-INFO` & `libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.import-files
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -35,14 +35,21 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.2] - 2024-05-31
+
+### Changed
+
+* Use Connection Param on project settings for use the action from a task.
+* Harmonise logs
+
 ## [1.0.1] - 2024-05-24
 
 ### Fixed
 
 * package folder name
 
 ## [1.0.0] - 2024-05-24
```

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/src/libreflow.extensions.anpo.import_files.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_import_files-1.0.2/src/libreflow.extensions.anpo.import_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_import_files-1.0.1/versioneer.py` & `libreflow_extensions_anpo_import_files-1.0.2/versioneer.py`

 * *Files identical despite different names*

