# Comparing `tmp/kivar-0.2.0.tar.gz` & `tmp/kivar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivar-0.2.0.tar", last modified: Wed May 29 21:06:01 2024, max compression
+gzip compressed data, was "kivar-0.2.1.tar", last modified: Fri May 31 21:47:23 2024, max compression
```

## Comparing `kivar-0.2.0.tar` & `kivar-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 21:06:01.112474 kivar-0.2.0/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4285 2024-05-29 21:06:01.112474 kivar-0.2.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     4024 2024-05-29 21:06:00.000000 kivar-0.2.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 21:06:01.112474 kivar-0.2.0/kivar/
--rwxrwxr-x   0 mark      (1000) mark      (1000)       28 2024-05-29 21:06:00.000000 kivar-0.2.0/kivar/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    33767 2024-05-29 21:06:00.000000 kivar-0.2.0/kivar/kivar_backend.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)    13093 2024-05-29 21:06:00.000000 kivar-0.2.0/kivar/kivar_cli.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 21:06:01.112474 kivar-0.2.0/kivar.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4285 2024-05-29 21:06:01.000000 kivar-0.2.0/kivar.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      226 2024-05-29 21:06:01.000000 kivar-0.2.0/kivar.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-29 21:06:01.000000 kivar-0.2.0/kivar.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-29 21:06:01.000000 kivar-0.2.0/kivar.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-05-29 21:06:01.000000 kivar-0.2.0/kivar.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-29 21:06:01.112474 kivar-0.2.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      617 2024-05-29 21:06:00.000000 kivar-0.2.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-31 21:47:23.724042 kivar-0.2.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4285 2024-05-31 21:47:23.720042 kivar-0.2.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4024 2024-05-31 21:47:23.000000 kivar-0.2.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-31 21:47:23.720042 kivar-0.2.1/kivar/
+-rwxrwxr-x   0 mark      (1000) mark      (1000)       28 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    34398 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar/kivar_backend.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)    13102 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar/kivar_cli.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-31 21:47:23.720042 kivar-0.2.1/kivar.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4285 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      226 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-05-31 21:47:23.000000 kivar-0.2.1/kivar.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-31 21:47:23.724042 kivar-0.2.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      617 2024-05-31 21:47:23.000000 kivar-0.2.1/setup.py
```

### Comparing `kivar-0.2.0/PKG-INFO` & `kivar-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivar
-Version: 0.2.0
+Version: 0.2.1
 Summary: PCB Assembly Variants for KiCad
 Home-page: https://github.com/markh-de/KiVar
 Author: Mark Hämmerling
 Author-email: dev@markh.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kivar-0.2.0/README.md` & `kivar-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kivar-0.2.0/kivar/kivar_backend.py` & `kivar-0.2.1/kivar/kivar_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 #   will even save that field to your file.
 
 # TODO pre-sort errors and changes before returning them, ready to be used by caller. then remove sorting and
 #      requirements (e.g. Key class import) in callers.
 
 # TODO clarify rules for Aspect name (forbidden characters: "*" ".")
 
-# TODO filter forbidden field names (reference, value, footprint (???)) for set AND get!!
-
 # TODO in aux field parser, accept only target fields which are no KiVar fields themselves (avoid recursion!)
 
 # TODO wrap the backend with a class.
 
 # TODO more testing!
 
 # TODO KiCad 8 has different change reporting style, it seems. use this?
@@ -26,53 +24,59 @@
     # Remove R29 'exclude from BOM' fabrication attribute.
     # Add R22 'exclude from BOM' fabrication attribute.
     # Add R22 'Do not place' fabrication attribute.
     # Update R2 fields.
 #     ^^^ this "update fields" message is too generic.
 
 def version():
-    return '0.2.0'
+    return '0.2.1'
 
 def pcbnew_compatibility_error():
     ver = pcbnew.GetMajorMinorPatchVersion()
     schema = ver.split('.')
     num = int(schema[0]) * 100 + int(schema[1])
     return None if num >= 799 else f'This version of KiVar requires KiCad pcbnew version 7.99 or later.\nYou are using pcbnew version {ver}.'
 
 def fp_to_uuid(fp):
     return fp.m_Uuid.AsString()
 
 def uuid_to_fp(board, uuid):
     return board.GetItem(pcbnew.KIID(uuid)).Cast()
 
+def field_accepted(field_name):
+    return not field_name.lower() in ['value', 'reference', 'footprint']
+
 def set_fp_field(fp, field, value):
-    if not field.lower() in ['value', 'reference', 'footprint']: fp.SetField(field, value)
+    if field_accepted(field): fp.SetField(field, value)
 
 def legacy_expressions_found(fpdict):
     found = 0
     for uuid in fpdict:
         for field in fpdict[uuid][Key.FIELDS]:
-            if field == 'KiVar.Rule': found += 1
+            if field == 'KiVar.Rule' and fpdict[uuid][Key.FIELDS][field]: found += 1
     return found
 
 def build_fpdict(board):
     fpdict = {}
     for fp in board.GetFootprints():
         uuid = fp_to_uuid(fp)
-        # TODO check if UUID exists in dict!
-        fpdict[uuid] = {}
-        fpdict[uuid][Key.REF] = fp.GetReferenceAsString()
-        fpdict[uuid][Key.FIELDS] = fp.GetFieldsText()
-        # TODO clean up, we currently store the value twice!
-        # the format is the same as for choice branches
-        fpdict[uuid][Key.VALUE] = fp.GetValue()
-        fpdict[uuid][Key.PROPS] = {}
-        fpdict[uuid][Key.PROPS][PropCode.BOM] = not fp.IsExcludedFromBOM()
-        fpdict[uuid][Key.PROPS][PropCode.POS] = not fp.IsExcludedFromPosFiles()
-        fpdict[uuid][Key.PROPS][PropCode.FIT] = not fp.IsDNP()
+        # if UUID is already known, skip any footprint with same UUID.
+        # TODO return error if same UUIDs are found. silently ignoring entries is bad.
+        if not uuid in fpdict:
+            fpdict[uuid] = {}
+            fpdict[uuid][Key.REF] = fp.GetReferenceAsString()
+            fields_text = fp.GetFieldsText()
+            fpdict[uuid][Key.FIELDS] = {}
+            for field in fields_text:
+                if field_accepted(field): fpdict[uuid][Key.FIELDS][field] = fields_text[field]
+            fpdict[uuid][Key.VALUE] = fp.GetValue()
+            fpdict[uuid][Key.PROPS] = {}
+            fpdict[uuid][Key.PROPS][PropCode.BOM] = not fp.IsExcludedFromBOM()
+            fpdict[uuid][Key.PROPS][PropCode.POS] = not fp.IsExcludedFromPosFiles()
+            fpdict[uuid][Key.PROPS][PropCode.FIT] = not fp.IsDNP()
     return fpdict
 
 def store_fpdict(board, fpdict):
     for uuid in fpdict:
         fp = uuid_to_fp(board, uuid)
         old_fp_value = fp.GetValue()
         new_fp_value = fpdict[uuid][Key.VALUE]
@@ -151,14 +155,15 @@
     FIT = 'F'
     BOM = 'B'
     POS = 'P'
 
 class FieldID: # case-sensitive
     BASE   = 'Var'
     ASPECT = 'Aspect'
+
 class PropGroup:
     ALL = '!'
 
 def base_prop_codes(): return PropCode.FIT + PropCode.BOM + PropCode.POS
 
 def supported_prop_codes(): return base_prop_codes() + PropGroup.ALL
 
@@ -422,14 +427,22 @@
                 # this is a choice definition. leave name and content raw and store.
                 if name_list is None or name_list == '':
                     errors.append('Choice identifier list must not be empty')
                     continue
                 choice_sets.append([name_list, content])
     return errors, aspects, choice_sets
 
+def field_name_check(field_name, available_fields):
+    error = None
+    if not field_accepted(field_name):
+        error = f"Target field '{field_name}' is forbidden" # TODO escape field name
+    elif not field_name in available_fields:
+        error = f"Target field '{field_name}' does not exist" # TODO escape field name
+    return error
+
 def parse_rule_fields(fpdict_uuid_branch):
     errors = []
     aspect = None
     base_rule_string = None
     base_choice_sets = []
     aux_rule_strings = []
     aux_choice_sets = []
@@ -441,37 +454,39 @@
         except: continue
         if len(parts) == 2 and parts[0] == FieldID.BASE and parts[1] == FieldID.ASPECT:
             aspect = value
         elif len(parts) == 1 and parts[0] == FieldID.BASE:
             base_rule_string = value
         elif len(parts) > 1 and parts[-1] == FieldID.BASE:
             target_field = '.'.join(parts[0:-1])
-            if target_field in fpdict_uuid_branch[Key.FIELDS]:
-                aux_rule_strings.append([target_field, value])
-            else:
-                errors.append(f"Target field '{target_field}' does not exist for combined aux expression") # TODO escape field name?
+            field_name_error = field_name_check(target_field, fpdict_uuid_branch[Key.FIELDS])
+            if field_name_error is not None:
+                errors.append(f"Combined aux expression: {field_name_error}")
                 continue
+            else:
+                aux_rule_strings.append([target_field, value])
         else:
             try: prefix, name_list = split_parens(parts[-1])
             except: continue
             if prefix == FieldID.BASE:
                 try: parts_in_parens = split_raw_str(name_list, ' ', True)
                 except: continue
                 if len(parts_in_parens) > 1:
                     errors.append(f"Choice identifier list '{name_list}' contains illegal space character")
                     continue
                 if len(parts) == 1:
                     base_choice_sets.append([name_list, value])
                 else:
                     target_field = '.'.join(parts[0:-1])
-                    if target_field in fpdict_uuid_branch[Key.FIELDS]:
-                        aux_choice_sets.append([target_field, name_list, value])
-                    else:
-                        errors.append(f"Target field '{target_field}' does not exist for simple aux expression") # TODO escape field name?
+                    field_name_error = field_name_check(target_field, fpdict_uuid_branch[Key.FIELDS])
+                    if field_name_error is not None:
+                        errors.append(f"Simple aux expression: {field_name_error}")
                         continue
+                    else:
+                        aux_choice_sets.append([target_field, name_list, value])
     return errors, aspect, base_rule_string, base_choice_sets, aux_rule_strings, aux_choice_sets
 
 def build_vardict(fpdict):
     vardict = {}
     errors = []
     auxdict = {}
     # Handle base rule
```

### Comparing `kivar-0.2.0/kivar/kivar_cli.py` & `kivar-0.2.1/kivar/kivar_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 for uuid in sorted(ndict[aspect][choice], key=lambda x: natural_sort_key(fpdict[x][Key.REF])):
                     ref = fpdict[uuid][Key.REF]
                     print(f'        {ref}: {ndict[aspect][choice][uuid]}')
                     for field in sorted(vardict[uuid][Key.AUX], key=natural_sort_key):
                         f = quote_str(field)
                         v = quote_str(vardict[uuid][Key.AUX][field][choice][Key.VALUE])
                         print(f"            {f}: {v}")
-                        # Future note: When options for aux rules are allowed, print them here
+                        # Future note: When properties for aux expressions are allowed, print them here
         print()
     return True
 
 def state_command(board=None, all=False, query_aspect=None, verbose=False):
     b = load_board(board)
     if b is None: return False
     fpdict = build_fpdict(b)
```

### Comparing `kivar-0.2.0/kivar.egg-info/PKG-INFO` & `kivar-0.2.1/kivar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivar
-Version: 0.2.0
+Version: 0.2.1
 Summary: PCB Assembly Variants for KiCad
 Home-page: https://github.com/markh-de/KiVar
 Author: Mark Hämmerling
 Author-email: dev@markh.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kivar-0.2.0/setup.py` & `kivar-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     description='PCB Assembly Variants for KiCad',
     long_description=long_descr,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/markh-de/KiVar',
     author='Mark Hämmerling',
     author_email='dev@markh.de',
-    version="0.2.0",
+    version="0.2.1",
     packages=["kivar"],
     install_requires=[],
     entry_points={
         "console_scripts": [
             "kivar = kivar:main"
         ]
     }
```

