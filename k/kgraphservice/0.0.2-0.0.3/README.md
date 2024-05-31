# Comparing `tmp/kgraphservice-0.0.2.tar.gz` & `tmp/kgraphservice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphservice-0.0.2.tar", last modified: Mon May 20 21:32:55 2024, max compression
+gzip compressed data, was "kgraphservice-0.0.3.tar", last modified: Fri May 31 01:49:00 2024, max compression
```

## Comparing `kgraphservice-0.0.2.tar` & `kgraphservice-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.871361 kgraphservice-0.0.2/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.2/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-20 21:32:55.871160 kgraphservice-0.0.2/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.2/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.870176 kgraphservice-0.0.2/kgraphservice/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.2/kgraphservice/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     3287 2024-05-20 21:31:52.000000 kgraphservice-0.0.2/kgraphservice/kgraph_service.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.870951 kgraphservice-0.0.2/kgraphservice.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      268 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-20 21:32:55.871400 kgraphservice-0.0.2/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      948 2024-05-20 21:32:34.000000 kgraphservice-0.0.2/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.267253 kgraphservice-0.0.3/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.3/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-31 01:49:00.267055 kgraphservice-0.0.3/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.3/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.265893 kgraphservice-0.0.3/kgraphservice/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.3/kgraphservice/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-31 01:46:46.000000 kgraphservice-0.0.3/kgraphservice/kg_comparator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     4522 2024-05-31 01:46:01.000000 kgraphservice-0.0.3/kgraphservice/kgraph_service.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-31 01:48:26.000000 kgraphservice-0.0.3/kgraphservice/kgslot_criterion.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.266812 kgraphservice-0.0.3/kgraphservice.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      333 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-31 01:49:00.267298 kgraphservice-0.0.3/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      948 2024-05-31 01:42:40.000000 kgraphservice-0.0.3/setup.py
```

### Comparing `kgraphservice-0.0.2/LICENSE` & `kgraphservice-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphservice-0.0.2/PKG-INFO` & `kgraphservice-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.2
+Version: 0.0.3
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.12
+Requires-Dist: vital-ai-vitalsigns>=0.1.14
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.6
+Requires-Dist: vital-ai-haley-kg>=0.1.8
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.2/kgraphservice/kgraph_service.py` & `kgraphservice-0.0.3/kgraphservice/kgraph_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-from typing import List, TypeVar, Type
-
+from typing import List, TypeVar, Type, Tuple
 from ai_haley_kg_domain.model.KGInteraction import KGInteraction
 from ai_haley_kg_domain.model.KGNode import KGNode
 from vital_ai_vitalsigns.query.result_list import ResultList
 from vital_ai_vitalsigns.service.vital_namespace import VitalNamespace
 from vital_ai_vitalsigns.service.vital_service import VitalService
 from vital_ai_vitalsigns.service.vital_service_status import VitalServiceStatus
 
 
 G = TypeVar('G', bound='GraphObject')
 KGN = TypeVar('KGN', bound='KGNode')
 
+# notes:
+# define primary vector for kg objects and secondary vector
+# for the type of the object
+# use naming convention _vector and _type_vector
+# see: https://weaviate.io/developers/weaviate/config-refs/schema/multi-vector
+
 
 class KGraphService:
     def __init__(self, vital_service: VitalService):
         self.vital_service = vital_service
 
-    def get_interaction_list(self, account_uri: str, limit=100, offset=0) -> ResultList:
-        pass
-
-    def get_interaction_graph(self, interaction: KGInteraction) -> ResultList:
-        pass
-
-    def get_interaction_frames(self, interaction: KGInteraction) -> ResultList:
-        pass
-
-    def get_interaction_nodes(self, interaction: KGInteraction, kgnode_type: Type[KGN]) -> ResultList:
-        pass
-
     def get_graph(self, graph_uri: str) -> VitalNamespace:
         return self.vital_service.get_graph(graph_uri)
 
     def list_graphs(self) -> List[VitalNamespace]:
         return self.vital_service.list_graphs()
 
     def check_create_graph(self, graph_uri: str) -> bool:
@@ -51,33 +44,60 @@
 
     def insert_object(self, graph_uri: str, graph_object: G) -> VitalServiceStatus:
         return self.vital_service.insert_object(graph_uri, graph_object)
 
     def insert_object_list(self, graph_uri: str, graph_object_list: List[G]) -> VitalServiceStatus:
         return self.vital_service.insert_object_list(graph_uri, graph_object_list)
 
-    def update_object(self, graph_object: G) -> VitalServiceStatus:
-        return self.vital_service.update_object(graph_object)
+    def update_object(self, graph_object: G, graph_uri: str) -> VitalServiceStatus:
+        return self.vital_service.update_object(graph_object, graph_uri)
+
+    def update_object_list(self, graph_object_list: List[G], graph_uri: str) -> VitalServiceStatus:
+        return self.vital_service.update_object_list(graph_object_list, graph_uri)
 
-    def update_object_list(self, graph_object_list: List[G]) -> VitalServiceStatus:
-        return self.vital_service.update_object_list(graph_object_list)
+    def get_object(self, object_uri: str, graph_uri: str = None) -> G:
+        return self.vital_service.get_object(object_uri, graph_uri)
 
-    def get_object(self, object_uri: str) -> G:
-        return self.vital_service.get_object(object_uri)
+    def get_object_list(self, object_uri_list: List[str], graph_uri: str = None) -> ResultList:
+        return self.vital_service.get_object_list(object_uri_list, graph_uri)
 
-    def get_object_list(self, object_uri_list: List[str]) -> ResultList:
-        return self.vital_service.get_object_list(object_uri_list)
+    def delete_object(self, object_uri: str, graph_uri: str = None) -> VitalServiceStatus:
+        return self.vital_service.delete_object(object_uri, graph_uri)
 
-    def delete_object(self, object_uri: str) -> VitalServiceStatus:
-        return self.vital_service.delete_object(object_uri)
+    def delete_object_list(self, object_uri_list: List[str], graph_uri: str = None) -> VitalServiceStatus:
+        return self.vital_service.delete_object_list(object_uri_list, graph_uri)
 
-    def delete_object_list(self, object_uri_list: List[str]) -> VitalServiceStatus:
-        return self.vital_service.delete_object_list(object_uri_list)
+    def filter_query(self, graph_uri: str, sparql_query: str) -> ResultList:
+        return self.vital_service.filter_query(graph_uri, sparql_query)
 
-    def filter_query(self, sparql_query: str) -> ResultList:
-        return self.vital_service.filter_query(sparql_query)
+    def query(self, graph_uri: str, sparql_query: str) -> ResultList:
+        return self.vital_service.query(sparql_query, graph_uri)
 
-    def query(self, sparql_query: str) -> ResultList:
-        return self.vital_service.query(sparql_query)
+    # Tuple[binding name, property uri]
+    def query_construct(self, graph_uri: str, sparql_query: str, binding_list: List[Tuple[str, str]]) -> ResultList:
+        pass
+
+    def get_interaction_list(self, graph_uri: str, limit=100, offset=0) -> ResultList:
+        pass
 
+    def get_interaction_graph(self, graph_uri: str, interaction: KGInteraction, limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_interaction_frames(self, graph_uri: str, interaction: KGInteraction, limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_interaction_nodes(self, graph_uri: str, interaction: KGInteraction, kgnode_type: Type[KGN], limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_frame(self, graph_uri: str, frame_uri: str, limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_frames(self, graph_uri: str, frame_uri_list: List[str], limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_frames_root(self, graph_uri: str, root_uri: str, limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_graph_objects_type(self, graph_uri: str, class_uri: str, include_subclasses=True, limit=100, offset=0) -> ResultList:
+        pass
```

### Comparing `kgraphservice-0.0.2/kgraphservice.egg-info/PKG-INFO` & `kgraphservice-0.0.3/kgraphservice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.2
+Version: 0.0.3
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.12
+Requires-Dist: vital-ai-vitalsigns>=0.1.14
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.6
+Requires-Dist: vital-ai-haley-kg>=0.1.8
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.2/setup.py` & `kgraphservice-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphservice',
-    version='0.0.2',
+    version='0.0.3',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Service',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphservice',
     packages=find_packages(exclude=["test"]),
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns>=0.1.12',
+            'vital-ai-vitalsigns>=0.1.14',
             'vital-ai-domain>=0.1.4',
             'six',
             'pyyaml',
-            'vital-ai-haley-kg>=0.1.6',
+            'vital-ai-haley-kg>=0.1.8',
             'rdflib==7.0.0',
             'SPARQLWrapper==2.0.0',
             'networkx',
             'matplotlib',
     ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

