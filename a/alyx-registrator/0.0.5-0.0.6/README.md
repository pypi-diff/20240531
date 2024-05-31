# Comparing `tmp/alyx_registrator-0.0.5.tar.gz` & `tmp/alyx_registrator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_registrator-0.0.5.tar", last modified: Wed May 29 17:14:20 2024, max compression
+gzip compressed data, was "alyx_registrator-0.0.6.tar", last modified: Fri May 31 16:24:33 2024, max compression
```

## Comparing `alyx_registrator-0.0.5.tar` & `alyx_registrator-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6234 2024-05-29 17:14:10.969092 alyx_registrator-0.0.5/one_registrator/README.md
--rw-r--r--   0        0        0       51 2024-05-29 17:14:10.969092 alyx_registrator-0.0.5/one_registrator/__init__.py
--rw-r--r--   0        0        0    28329 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/registration.py
--rw-r--r--   0        0        0    11707 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/rules.json
--rw-r--r--   0        0        0     2904 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/utils.py
--rw-r--r--   0        0        0      660 2024-05-29 17:14:20.592923 alyx_registrator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6234 2024-05-31 16:24:23.920416 alyx_registrator-0.0.6/one_registrator/README.md
+-rw-r--r--   0        0        0       94 2024-05-31 16:24:23.920416 alyx_registrator-0.0.6/one_registrator/__init__.py
+-rw-r--r--   0        0        0    29712 2024-05-31 16:24:23.924416 alyx_registrator-0.0.6/one_registrator/registration.py
+-rw-r--r--   0        0        0    11707 2024-05-31 16:24:23.924416 alyx_registrator-0.0.6/one_registrator/rules.json
+-rw-r--r--   0        0        0     2874 2024-05-31 16:24:23.924416 alyx_registrator-0.0.6/one_registrator/utils.py
+-rw-r--r--   0        0        0      660 2024-05-31 16:24:33.168358 alyx_registrator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.6/PKG-INFO
```

### Comparing `alyx_registrator-0.0.5/one_registrator/README.md` & `alyx_registrator-0.0.6/one_registrator/README.md`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.5/one_registrator/registration.py` & `alyx_registrator-0.0.6/one_registrator/registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # source_path is the original path from disk scan. will never change
     source_path: str
 
     # dest_path is the path after renaming method calculated it. It is a frozen version of renamed_path
     # if it appears empty in a dataframe, it's because to_user_dict sets it to "" if rename is false, for clarity sake
     dest_path: str = ""
 
-    _alf_info: dict = None
+    _alf_info: dict | None = None
 
     match: bool = False
     matching_rules: list = field(default_factory=list)
     used_rule: str = ""
 
     valid_alf: bool = False
     path_conflicts: bool = False
@@ -35,22 +35,47 @@
         elif item == "source":
             return self.source_alf_info["object"] + "." + self.source_alf_info["attribute"]
         else:
             raise ValueError("Value must be 'dest' or 'source'")
 
     @property
     def alf_info(self) -> dict:
+        """Returns a dictionary containing information about the ALF file associated with the current instance.
+
+        This property first checks if the `_alf_info` attribute is already set.
+            If it is, it returns the value of `_alf_info`.
+        If `_alf_info` is not set, it calls the `full_path_parts` function from the `one.alf.files`
+            module to retrieve the ALF information.
+        The `full_path_parts` function takes the `source_path` attribute as input and returns a
+            dictionary containing the ALF information.
+
+        Returns:
+            dict: A dictionary containing the ALF information.
+        """
         if self._alf_info is None:
             self._alf_info = one.alf.files.full_path_parts(
                 self.source_path, as_dict=True, absolute=True, assert_valid=False
             )
-        return self._alf_info
+        return self._alf_info  # type: ignore
 
     @property
     def source_alf_info(self) -> dict:
+        """Returns a dictionary containing information about the ALF file associated
+        with the source path of the current instance.
+
+        This property first checks if the `_source_alf_info` attribute is already set.
+            If it is, it returns the value of `_source_alf_info`.
+        If `_source_alf_info` is not set, it calls the `full_path_parts` function from the `one.alf.files`
+            module to retrieve the ALF information.
+        The `full_path_parts` function takes the `source_path` attribute as input and
+            returns a dictionary containing the ALF information.
+
+        Returns:
+            dict: A dictionary containing the ALF information.
+        """
         return one.alf.files.full_path_parts(self.source_path, as_dict=True, absolute=True, assert_valid=False)
 
     # this is usefull to get the renamed path in a dynamically updated version in the bulding stages.
     # Do not use it in the apply stages.
     @property
     def renamed_path(self) -> str:
         return one.alf.spec.to_full_path(**self.alf_info)
@@ -630,15 +655,15 @@
         records_groups = self.apply_to_alyx(session, selected_records)
         return records_groups
 
     def evaluate_session(self, session):
         folder = getattr(session, "path", None)
         if folder is None:
             session = self.one_connector.search(id=session, no_cache=True, details=True)
-            folder = session["path"]
+            folder = session["path"]  # type: ignore
 
         files_list = find_files(folder, relative=False, levels=-1, get="files")
 
         return self.evaluate(files_list)
 
     def evaluate(self, file_list):
         file_records = [FileRecord(file_path) for file_path in file_list]
```

### Comparing `alyx_registrator-0.0.5/one_registrator/rules.json` & `alyx_registrator-0.0.6/one_registrator/rules.json`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.5/one_registrator/utils.py` & `alyx_registrator-0.0.6/one_registrator/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 import os, re, pandas as pd
 
-def file_records_to_df(file_records, details = False):
-    
+
+def file_records_to_df(file_records, details=False):
+
     dicts = []
 
-    if details :
-        for file_record in file_records :
+    if details:
+        for file_record in file_records:
             dico = file_record.__dict__
             dico["info"] = file_record.info_message
-            dicts.append( dico )
-    else :
-        for file_record in file_records :
-            dicts.append( file_record.to_user_dict() )
-    
+            dicts.append(dico)
+    else:
+        for file_record in file_records:
+            dicts.append(file_record.to_user_dict())
+
     return pd.DataFrame(dicts)
 
+
 def get_existing_datasets(one_connector):
-    existing_dst = one_connector.alyx.rest("dataset-types","list", no_cache = True)
-    existing_types = [dst["object"] + "." + dst["attribute"] for dst in existing_dst if dst["attribute"] != "" and dst["attribute"] != '']
+    existing_dst = one_connector.alyx.rest("dataset-types", "list", no_cache=True)
+    existing_types = [
+        dst["object"] + "." + dst["attribute"]
+        for dst in existing_dst
+        if dst["attribute"] != "" and dst["attribute"] != ""
+    ]
     return existing_types
 
 
-def find_files(input_path, re_pattern = None, relative = False,levels = -1, get = "files", parts = "all", sort = True):
+def find_files(input_path, re_pattern=None, relative=False, levels=-1, get="files", parts="all", sort=True):
     """
     Get full path of files from all folders under the ``input_path`` (including itself).
-    Can return specific files with optionnal conditions 
+    Can return specific files with optionnal conditions
     Args:
-        input_path (str): A valid path to a folder. 
-            This folder is used as the root to return files found 
+        input_path (str): A valid path to a folder.
+            This folder is used as the root to return files found
             (possible condition selection by giving to re_callback a function taking a regexp pattern and a string as argument, an returning a boolean).
     Returns:
         list: List of the file fullpaths found under ``input_path`` folder and subfolders.
     """
-    #if levels = -1, we get  everything whatever the depth (at least up to 32767 subfolders, but this should be fine...)
+    # if levels = -1, we get  everything whatever the depth (at least up to 32767 subfolders, but this should be fine...)
 
-    if levels == -1 :
+    if levels == -1:
         levels = 32767
     current_level = 0
     output_list = []
-    
-    if re_pattern is not None : 
+
+    if re_pattern is not None:
         re_pattern = re.compile(re_pattern)
 
     def _recursive_search(_input_path):
         nonlocal current_level
         for subdir in os.listdir(_input_path):
-            fullpath = os.path.join(_input_path,subdir)
-            if os.path.isfile(fullpath): 
+            fullpath = os.path.join(_input_path, subdir)
+            if os.path.isfile(fullpath):
                 if (get == "all" or get == "files") and (re_pattern is None or re_pattern.match(fullpath)):
                     output_list.append(os.path.normpath(fullpath))
-                    
-            else :
-                if (get == "all" or get == "dirs" or get == "folders") and (re_pattern is None or re_pattern.match(fullpath)):
+
+            else:
+                if (get == "all" or get == "dirs" or get == "folders") and (
+                    re_pattern is None or re_pattern.match(fullpath)
+                ):
                     output_list.append(os.path.normpath(fullpath))
                 if current_level < levels:
-                    current_level += 1 
+                    current_level += 1
                     _recursive_search(fullpath)
         current_level -= 1
-        
+
     if os.path.isfile(input_path):
         raise ValueError(f"Can only list files in a directory. A file was given : {input_path}")
- 
+
     _recursive_search(input_path)
-    
-    if relative :
-        output_list = [os.path.relpath(file,start = input_path) for file in output_list]
-    if parts == "name" :
+
+    if relative:
+        output_list = [os.path.relpath(file, start=input_path) for file in output_list]
+    if parts == "name":
         output_list = [os.path.basename(file) for file in output_list]
 
     return output_list
-        
-
-    
-
```

### Comparing `alyx_registrator-0.0.5/pyproject.toml` & `alyx_registrator-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "numpy>=1.23",
     "alyx-connector>=1.16",
     "pandas>=1.4",
 ]
 requires-python = ">=3.11"
 dynamic = []
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

