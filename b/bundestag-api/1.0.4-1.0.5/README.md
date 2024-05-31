# Comparing `tmp/bundestag_api-1.0.4.tar.gz` & `tmp/bundestag_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundestag_api-1.0.4.tar", last modified: Thu May 30 08:08:38 2024, max compression
+gzip compressed data, was "bundestag_api-1.0.5.tar", last modified: Thu May 30 20:50:36 2024, max compression
```

## Comparing `bundestag_api-1.0.4.tar` & `bundestag_api-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/bundestag_api/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41897 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/bta_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20096 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/bundestag_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/tests/test_btawrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:50:36.864474 bundestag_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 20:50:36.864474 bundestag_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:50:36.860474 bundestag_api-1.0.5/bundestag_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/bundestag_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40000 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/bundestag_api/bta_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/bundestag_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/bundestag_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:50:36.864474 bundestag_api-1.0.5/bundestag_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 20:50:36.000000 bundestag_api-1.0.5/bundestag_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 20:50:36.000000 bundestag_api-1.0.5/bundestag_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:50:36.000000 bundestag_api-1.0.5/bundestag_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 20:50:36.000000 bundestag_api-1.0.5/bundestag_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 20:50:36.000000 bundestag_api-1.0.5/bundestag_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 20:50:36.864474 bundestag_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:50:36.864474 bundestag_api-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-30 20:50:32.000000 bundestag_api-1.0.5/tests/test_btawrapper.py
```

### Comparing `bundestag_api-1.0.4/LICENSE` & `bundestag_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bundestag_api-1.0.4/PKG-INFO` & `bundestag_api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bundestag_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper for the official Bundestag-API
 Home-page: https://github.com/jschibberges/Bundestag-API
 Author: Julian Schibberges
 Author-email: julian@schibberges.de
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `bundestag_api-1.0.4/README.md` & `bundestag_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bundestag_api-1.0.4/bundestag_api/bta_wrapper.py` & `bundestag_api-1.0.5/bundestag_api/bta_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         prs = True
         while prs is True:
             r = requests.get(r_url, params=payload)
             logger.debug(r.url)
             if r.status_code == requests.codes.ok:
                 content = r.json()
                 if content["numFound"] == 0:
-                    # print("No data was returned.")
+                    logging.info("No data was returned.")
                     data = "No data was returned."
                     prs = False
                 elif content["numFound"] > 0 and content["numFound"] <= 50:
                     data.extend(content["documents"])
                     prs = False
                 elif content["numFound"] > 50:
                     if payload["cursor"] == content["cursor"]:
@@ -403,15 +403,17 @@
                           fid=fid,
                           date_start=date_start,
                           date_end=date_end,
                           num=num,
                           updated_since=updated_since,
                           updated_until=updated_until,
                           descriptor=descriptor,
-                          sachgebiet=sachgebiet,)
+                          sachgebiet=sachgebiet,
+                          document_type=document_type,
+                          title=title)
         return data
 
     def get_procedure(self,
                       btid=None,
                       return_format="json",
                       documentID=None,
                       plenaryprotocolID=None):
@@ -500,15 +502,17 @@
         data = self.query(resource="vorgangsposition",
                           return_format=return_format,
                           fid=fid,
                           date_start=date_start,
                           date_end=date_end,
                           num=num,
                           updated_since=updated_since,
-                          updated_until=updated_until,)
+                          updated_until=updated_until,,
+                          document_type=document_type,
+                          title=title)
         return data
 
     def get_procedureposition(self,
                               btid,
                               return_format="json",
                               documentID=None,
                               procedureID=None,
@@ -614,15 +618,17 @@
                           return_format=return_format,
                           fid=fid,
                           date_start=date_start,
                           date_end=date_end,
                           institution=institution,
                           num=num,
                           updated_since=updated_since,
-                          updated_until=updated_until,)
+                          updated_until=updated_until,
+                          document_type=document_type,
+                          title=title)
         return data
 
     def get_document(self,
                      btid,
                      return_format="json",
                      fulltext=False):
         """
@@ -921,65 +927,8 @@
         -------
         data: list
             A list of strings
 
         """
         list_of_methods = dir(btaConnection)
         list_of_methods = [item for item in list_of_methods if "__" not in item]
-        """
-        list_of_methods = ["get_activity","search_activity","get_person",
-                           "search_person", "get_plenaryprotocol",
-                           "search_plenaryprotocol", "get_document",
-                           "search_document", "get_procedureposition",
-                           "search_procedureposition", "get_procedure",
-                           "search_procedure", "query"] 
-        """
         return list_of_methods
-
-
-def main_function():
-    arguments = parse_args_to_dict(sys.argv[1:])
-    if arguments.get("o") is not None:
-        output_format = arguments.get("o")
-        output_defined = True
-        arguments.pop("o")
-        if arguments.get("n") is not None:
-            file_name = arguments.get("n")
-            if output_format not in file_name:
-                file_name = file_name+"."+output_format
-            arguments.pop("n")
-        else:
-            raise ValueError("Output defined but no filename given.")
-    if arguments.get("apikey") is not None:
-        bta = btaConnection(apikey=arguments.get("apikey"))
-        arguments.pop("apikey")
-    else:
-        bta = btaConnection()
-    if arguments.get("method") is not None:
-        if arguments.get("method") in bta.list_methods():
-            method = arguments.get("method")
-            arguments.pop("method")
-            if method == "searchProcedure":
-                data = bta.search_procedure(arguments)
-        else:
-            raise ValueError("No valid method supplied.")
-    else:
-        raise ValueError("No method supplied")
-    if output_defined == True:
-        if output_format == "xlsx" or output_format == "xls":
-            import pandas as pd
-            data = pd.json_normalize(data)
-            data.to_excel(file_name, index=False)
-        elif output_format == "csv":
-            import pandas as pd
-            data = pd.json_normalize(data)
-            data.to_csv(file_name, index=False)
-        elif output_format == "json":
-            import json
-            with open(file_name, 'w', encoding='utf-8') as f:
-                json.dump(data, f, ensure_ascii=False, indent=4)
-    else:
-        return data
-
-
-if __name__ == "__main__":
-    main_function()
```

### Comparing `bundestag_api-1.0.4/bundestag_api/models.py` & `bundestag_api-1.0.5/bundestag_api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,8 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Fri Mar  1 22:45:35 2024
-
-@author: jschi
-"""
-
-# Classes
-
 
 class Person:
     """This class represents a German parliamentarian"""
 
     def __init__(self, dictionary):
         self.btid = dictionary["id"]
         if "nachname" in dictionary:
```

### Comparing `bundestag_api-1.0.4/bundestag_api/utils.py` & `bundestag_api-1.0.5/bundestag_api/utils.py`

 * *Files identical despite different names*

### Comparing `bundestag_api-1.0.4/bundestag_api.egg-info/PKG-INFO` & `bundestag_api-1.0.5/bundestag_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bundestag_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper for the official Bundestag-API
 Home-page: https://github.com/jschibberges/Bundestag-API
 Author: Julian Schibberges
 Author-email: julian@schibberges.de
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `bundestag_api-1.0.4/setup.py` & `bundestag_api-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     description='Python wrapper for the official Bundestag-API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/jschibberges/Bundestag-API",
     readme="README.md",
     license="MIT",
     name='bundestag_api',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     install_requires=[
          'requests>=2.0.0',
     ],
     python_requires='>=3.7.0'
 )
```

### Comparing `bundestag_api-1.0.4/tests/test.py` & `bundestag_api-1.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `bundestag_api-1.0.4/tests/test_btawrapper.py` & `bundestag_api-1.0.5/tests/test_btawrapper.py`

 * *Files identical despite different names*

