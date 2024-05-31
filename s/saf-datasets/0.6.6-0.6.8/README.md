# Comparing `tmp/saf_datasets-0.6.6.tar.gz` & `tmp/saf_datasets-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saf_datasets-0.6.6.tar", last modified: Thu May 16 16:30:03 2024, max compression
+gzip compressed data, was "saf_datasets-0.6.8.tar", last modified: Fri May 31 15:00:27 2024, max compression
```

## Comparing `saf_datasets-0.6.6.tar` & `saf_datasets-0.6.8.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.536949 saf_datasets-0.6.6/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.6/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-16 16:30:03.536748 saf_datasets-0.6.6/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.6/README.md
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-16 16:28:22.000000 saf_datasets-0.6.6/pyproject.toml
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.6/requirements.txt
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.527062 saf_datasets-0.6.6/saf_datasets/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       27 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.530720 saf_datasets-0.6.6/saf_datasets/annotators/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.6/saf_datasets/annotators/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1325 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/annotators/allennlp_srl.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.6/saf_datasets/annotators/models.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.6/saf_datasets/annotators/spacy.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     4882 2024-05-10 08:55:47.000000 saf_datasets-0.6.6/saf_datasets/annotators/transformer.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.534760 saf_datasets-0.6.6/saf_datasets/data_access/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      341 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.6/saf_datasets/data_access/allnli.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.6/saf_datasets/data_access/codwoe.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.6/saf_datasets/data_access/cpae.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.6/saf_datasets/data_access/dataset.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3962 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/data_access/entailmentbank.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.6/saf_datasets/data_access/stsb.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8835 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/data_access/wiktionary.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4089 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/wordnet_filtered.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2891 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/wordnet_spanish.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.535906 saf_datasets-0.6.6/saf_datasets/wrappers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.6/saf_datasets/wrappers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.6/saf_datasets/wrappers/hf.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.6/saf_datasets/wrappers/torch.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.536470 saf_datasets-0.6.6/saf_datasets.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/PKG-INFO
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      917 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/SOURCES.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/dependency_links.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/requires.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-16 16:30:03.537243 saf_datasets-0.6.6/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-16 16:28:27.000000 saf_datasets-0.6.6/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.529398 saf_datasets-0.6.8/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.8/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-31 15:00:27.529221 saf_datasets-0.6.8/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-29 12:40:18.000000 saf_datasets-0.6.8/README.md
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-31 14:37:33.000000 saf_datasets-0.6.8/pyproject.toml
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.8/requirements.txt
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.522322 saf_datasets-0.6.8/saf_datasets/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       27 2024-05-16 16:27:52.000000 saf_datasets-0.6.8/saf_datasets/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.525046 saf_datasets-0.6.8/saf_datasets/annotators/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.8/saf_datasets/annotators/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1325 2024-05-16 16:27:17.000000 saf_datasets-0.6.8/saf_datasets/annotators/allennlp_srl.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2121 2024-05-31 14:36:57.000000 saf_datasets-0.6.8/saf_datasets/annotators/amr.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.8/saf_datasets/annotators/models.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.8/saf_datasets/annotators/spacy.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     4882 2024-05-10 08:55:47.000000 saf_datasets-0.6.8/saf_datasets/annotators/transformer.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.527994 saf_datasets-0.6.8/saf_datasets/data_access/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      392 2024-05-31 14:36:56.000000 saf_datasets-0.6.8/saf_datasets/data_access/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.8/saf_datasets/data_access/allnli.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.8/saf_datasets/data_access/codwoe.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.8/saf_datasets/data_access/cpae.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-31 14:52:21.000000 saf_datasets-0.6.8/saf_datasets/data_access/dataset.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3961 2024-05-31 14:56:30.000000 saf_datasets-0.6.8/saf_datasets/data_access/entailmentbank.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3328 2024-05-31 14:55:17.000000 saf_datasets-0.6.8/saf_datasets/data_access/inference_types.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.8/saf_datasets/data_access/stsb.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8834 2024-05-31 14:55:46.000000 saf_datasets-0.6.8/saf_datasets/data_access/wiktionary.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4088 2024-05-31 14:56:00.000000 saf_datasets-0.6.8/saf_datasets/data_access/wordnet_filtered.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2891 2024-05-29 12:50:22.000000 saf_datasets-0.6.8/saf_datasets/data_access/wordnet_spanish.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.528710 saf_datasets-0.6.8/saf_datasets/wrappers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.8/saf_datasets/wrappers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.8/saf_datasets/wrappers/hf.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.8/saf_datasets/wrappers/torch.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-31 15:00:27.529000 saf_datasets-0.6.8/saf_datasets.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-31 15:00:27.000000 saf_datasets-0.6.8/saf_datasets.egg-info/PKG-INFO
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      992 2024-05-31 15:00:27.000000 saf_datasets-0.6.8/saf_datasets.egg-info/SOURCES.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-31 15:00:27.000000 saf_datasets-0.6.8/saf_datasets.egg-info/dependency_links.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-31 15:00:27.000000 saf_datasets-0.6.8/saf_datasets.egg-info/requires.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-31 15:00:27.000000 saf_datasets-0.6.8/saf_datasets.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-31 15:00:27.529439 saf_datasets-0.6.8/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-31 14:37:25.000000 saf_datasets-0.6.8/setup.py
```

### Comparing `saf_datasets-0.6.6/LICENSE` & `saf_datasets-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/PKG-INFO` & `saf_datasets-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.6
+Version: 0.6.8
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.6/README.md` & `saf_datasets-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/pyproject.toml` & `saf_datasets-0.6.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saf-datasets"
-version = "0.6.6"
+version = "0.6.8"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "Data set loading and annotation facilities for the Simple Annotation Framework"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `saf_datasets-0.6.6/saf_datasets/annotators/allennlp_srl.py` & `saf_datasets-0.6.8/saf_datasets/annotators/allennlp_srl.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/annotators/spacy.py` & `saf_datasets-0.6.8/saf_datasets/annotators/spacy.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/annotators/transformer.py` & `saf_datasets-0.6.8/saf_datasets/annotators/transformer.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/allnli.py` & `saf_datasets-0.6.8/saf_datasets/data_access/allnli.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/codwoe.py` & `saf_datasets-0.6.8/saf_datasets/data_access/codwoe.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/cpae.py` & `saf_datasets-0.6.8/saf_datasets/data_access/cpae.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/dataset.py` & `saf_datasets-0.6.8/saf_datasets/data_access/dataset.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/entailmentbank.py` & `saf_datasets-0.6.8/saf_datasets/data_access/entailmentbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         :return: A single term decomposition (Sentence).
         """
         return self.data[idx]
 
     @staticmethod
     def from_resource(locator: str):
         """
-        Downloaads a per-annotated resource available at the specified locator
+        Downloads a pre-annotated resource available at the specified locator
 
         Example:
             >>> dataset = EntailmentBankDataSet.from_resource("pos+lemma+ctag+dep+srl#noproof")
         """
         dataset = None
         if (locator in ANNOT_RESOURCES):
             path = ANNOT_RESOURCES[locator]["path"]
```

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/stsb.py` & `saf_datasets-0.6.8/saf_datasets/data_access/stsb.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/wiktionary.py` & `saf_datasets-0.6.8/saf_datasets/data_access/wiktionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             self._vocab["definiendum"] = definiendum_vocab
 
         return self._vocab[source]
 
     @staticmethod
     def from_resource(locator: str):
         """
-        Downloaads a per-annotated resource available at the specified locator
+        Downloads a pre-annotated resource available at the specified locator
 
         Example:
             >>> dataset = WiktionaryDefinitionCorpus.from_resource("pos+lemma+ctag+dep+dsr")
         """
         wiktdef = None
         if (locator in ANNOT_RESOURCES):
             path = ANNOT_RESOURCES[locator]["path"]
```

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/wordnet_filtered.py` & `saf_datasets-0.6.8/saf_datasets/data_access/wordnet_filtered.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def vocabulary(self, source: str = "_token", lowercase: bool = True) -> Vocabulary:
         return WiktionaryDefinitionCorpus.vocabulary(self, source, lowercase)
 
 
     @staticmethod
     def from_resource(locator: str):
         """
-        Downloaads a per-annotated resource available at the specified locator
+        Downloads a pre-annotated resource available at the specified locator
 
         Example:
             >>> dataset = WordNetFilteredDataSet.from_resource("pos+lemma+ctag+dep+dsr+srl")
         """
         dataset = None
         if (locator in ANNOT_RESOURCES):
             path = ANNOT_RESOURCES[locator]["path"]
```

### Comparing `saf_datasets-0.6.6/saf_datasets/data_access/wordnet_spanish.py` & `saf_datasets-0.6.8/saf_datasets/data_access/wordnet_spanish.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/wrappers/hf.py` & `saf_datasets-0.6.8/saf_datasets/wrappers/hf.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets/wrappers/torch.py` & `saf_datasets-0.6.8/saf_datasets/wrappers/torch.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.6/saf_datasets.egg-info/PKG-INFO` & `saf_datasets-0.6.8/saf_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.6
+Version: 0.6.8
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.6/saf_datasets.egg-info/SOURCES.txt` & `saf_datasets-0.6.8/saf_datasets.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 saf_datasets.egg-info/PKG-INFO
 saf_datasets.egg-info/SOURCES.txt
 saf_datasets.egg-info/dependency_links.txt
 saf_datasets.egg-info/requires.txt
 saf_datasets.egg-info/top_level.txt
 saf_datasets/annotators/__init__.py
 saf_datasets/annotators/allennlp_srl.py
+saf_datasets/annotators/amr.py
 saf_datasets/annotators/models.py
 saf_datasets/annotators/spacy.py
 saf_datasets/annotators/transformer.py
 saf_datasets/data_access/__init__.py
 saf_datasets/data_access/allnli.py
 saf_datasets/data_access/codwoe.py
 saf_datasets/data_access/cpae.py
 saf_datasets/data_access/dataset.py
 saf_datasets/data_access/entailmentbank.py
+saf_datasets/data_access/inference_types.py
 saf_datasets/data_access/stsb.py
 saf_datasets/data_access/wiktionary.py
 saf_datasets/data_access/wordnet_filtered.py
 saf_datasets/data_access/wordnet_spanish.py
 saf_datasets/wrappers/__init__.py
 saf_datasets/wrappers/hf.py
 saf_datasets/wrappers/torch.py
```

### Comparing `saf_datasets-0.6.6/setup.py` & `saf_datasets-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='saf_datasets',
-    version='0.6.6',
+    version='0.6.8',
     packages=['saf_datasets', 'saf_datasets.annotators', 'saf_datasets.data_access', 'saf_datasets.wrappers'],
     url='',
     author='Danilo S. Carvalho',
     author_email='danilo.carvalho@manchester.ac.uk',
     description='Data set loading and annotation facilities for the Simple Annotation Framework',
     install_requires=load_requirements()
 )
```

