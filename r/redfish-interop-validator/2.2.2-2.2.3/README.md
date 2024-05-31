# Comparing `tmp/redfish_interop_validator-2.2.2.tar.gz` & `tmp/redfish_interop_validator-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_interop_validator-2.2.2.tar", last modified: Fri May  3 20:43:26 2024, max compression
+gzip compressed data, was "redfish_interop_validator-2.2.3.tar", last modified: Fri May 31 20:41:30 2024, max compression
```

## Comparing `redfish_interop_validator-2.2.2.tar` & `redfish_interop_validator-2.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.175496 redfish_interop_validator-2.2.2/redfish_interop_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishInteropValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishLogo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    39575 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/interop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/redfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/traverseInterop.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:41:30.469972 redfish_interop_validator-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-31 20:41:30.469972 redfish_interop_validator-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:41:30.469972 redfish_interop_validator-2.2.3/redfish_interop_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/RedfishInteropValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/RedfishLogo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40392 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/redfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/traverseInterop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/redfish_interop_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:41:30.469972 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 20:41:30.000000 redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:41:30.469972 redfish_interop_validator-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-31 20:41:21.000000 redfish_interop_validator-2.2.3/setup.py
```

### Comparing `redfish_interop_validator-2.2.2/LICENSE.md` & `redfish_interop_validator-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/PKG-INFO` & `redfish_interop_validator-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.2
+Version: 2.2.3
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.2/README.md` & `redfish_interop_validator-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishInteropValidator.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/RedfishInteropValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from urllib.parse import urlparse
 from collections import Counter
 
 import redfish_interop_validator.traverseInterop as traverseInterop
 from redfish_interop_validator.profile import getProfiles, checkProfileAgainstSchema, hashProfile
 from redfish_interop_validator.validateResource import validateSingleURI, validateURITree
 
-tool_version = '2.2.2'
+tool_version = '2.2.3'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO - 1
 VERBOSE2 = logging.INFO - 2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishLogo.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/config.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/interop.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,14 +275,15 @@
             if paramPass:
                 alltarget.add(item)
                 if len(alltarget) == len(target):
                     break
             else:
                 continue
         paramPass = len(alltarget) == len(target)
+
     if compareType == "LinkToResource":
         if val == REDFISH_ABSENT:
             paramPass = False
         else:
             vallink = val.get('@odata.id')
             success, rf_payload, code, elapsed, _ = callResourceURI(vallink)
             if success:
@@ -296,15 +297,15 @@
                 paramPass = False
 
     if compareType == "Absent":
         paramPass = val == REDFISH_ABSENT
     if compareType == "Present":
         paramPass = val != REDFISH_ABSENT
 
-    if isinstance(target, list):
+    if isinstance(target, list) and val != REDFISH_ABSENT:
         if compareType == "Equal":
             paramPass = val in target
         elif compareType == "NotEqual":
             paramPass = val not in target
         else:
             for value in target:
                 if compareType == "GreaterThan":
@@ -313,14 +314,18 @@
                     paramPass = val >= value
                 if compareType == "LessThan":
                     paramPass = val < value
                 if compareType == "LessThanOrEqual":
                     paramPass = val <= value
                 if paramPass is False:
                     break
+    elif compareType in ["Equal", "NotEqual", "GreaterThan", "GreaterThanOrEqual", "LessThan", "LessThanOrEqual"]:
+        if not isinstance(target, list):
+            my_logger.warn('CompareType {} requires a list of values'.format(compareType))
+
     my_logger.debug('\tpass ' + str(paramPass))
     return msgInterop('Comparison', target, compareType, val, paramPass),\
         paramPass
 
 
 def validateMembers(members, profile_entry, annotation):
     """
@@ -772,33 +777,43 @@
     my_logger.debug(str(interop_profile))
     counts = Counter()
     # rf_payload_tuple provides the chain of dicts containing dicts, needed for CompareProperty
     rf_payload_tuple = (rf_payload, None)
 
     if "UseCases" in interop_profile:
         for use_case in interop_profile['UseCases']:
-            entry_title = use_case.get("UseCaseTitle", "NoName").replace(' ','_')
-            my_logger.debug('UseCase {}'.format(entry_title))
+            entry_title = use_case.get("UseCaseTitle", "NoName").replace(' ', '_')
+            entry_type = use_case.get("UseCaseType", "Normal")
+            my_logger.debug('UseCase {} {}'.format(entry_title, entry_type))
 
             # Check if we have a valid UseCase
-            if 'URIs' not in use_case and 'UseCaseKeyProperty' not in use_case:
+            if 'URIs' not in use_case and 'UseCaseKeyProperty' not in use_case and entry_type != 'AbsentResource':
                 my_logger.error('UseCase does not have URIs or UseCaseKeyProperty...')
 
-            if 'UseCaseKeyProperty' in use_case:
+            if entry_type == 'AbsentResource':
+                my_status = rf_payload.get('Status')
+                if my_status:
+                    use_case_applies = my_status.get('State') == 'Absent'
+                else:
+                    use_case_applies = False
+                if 'URIs' in use_case:
+                    use_case_applies = use_case_applies and checkInteropURI(propResourceObj, use_case['URIs'])
+
+            elif 'UseCaseKeyProperty' in use_case:
                 entry_key, entry_comparison, entry_values = use_case['UseCaseKeyProperty'], use_case['UseCaseComparison'], use_case['UseCaseKeyValues']
 
-                _, use_case_applies = checkComparison(rf_payload.get(entry_key), entry_comparison, entry_values)
+                _, use_case_applies = checkComparison(rf_payload.get(entry_key, REDFISH_ABSENT), entry_comparison, entry_values)
 
                 # Check if URI applies to this usecase as well
                 if 'URIs' in use_case:
                     use_case_applies = checkInteropURI(propResourceObj, use_case['URIs']) and use_case_applies
 
             elif 'URIs' in use_case:
                 use_case_applies = checkInteropURI(propResourceObj, use_case['URIs'])
-            
+
             else:
                 use_case_applies = False
 
             if use_case_applies:
                 my_msg = msgInterop("UseCase.{}".format(entry_title), '-', '-', '-', testResultEnum.OK)
 
                 msgs.append(my_msg)
```

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/profile.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/profile.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/redfish.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/redfish.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/session.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/session.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/tohtml.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/traverseInterop.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/traverseInterop.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator/validateResource.py` & `redfish_interop_validator-2.2.3/redfish_interop_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/PKG-INFO` & `redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.2
+Version: 2.2.3
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/SOURCES.txt` & `redfish_interop_validator-2.2.3/redfish_interop_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.2/setup.py` & `redfish_interop_validator-2.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_interop_validator",
-    version="2.2.2",
+    version="2.2.3",
     description="Redfish Interop Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

