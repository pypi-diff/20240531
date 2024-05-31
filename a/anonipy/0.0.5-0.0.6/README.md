# Comparing `tmp/anonipy-0.0.5.tar.gz` & `tmp/anonipy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonipy-0.0.5.tar", last modified: Wed May 29 17:35:23 2024, max compression
+gzip compressed data, was "anonipy-0.0.6.tar", last modified: Fri May 31 08:06:15 2024, max compression
```

## Comparing `anonipy-0.0.5.tar` & `anonipy-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 17:35:19.000000 anonipy-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-29 17:35:23.054713 anonipy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-29 17:35:19.000000 anonipy-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.046712 anonipy-0.0.5/anonipy/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/entity_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/date_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/llm_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/mask_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/number_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/redaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/language_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/anonipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 17:35:19.000000 anonipy-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 17:35:19.000000 anonipy-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 17:35:23.054713 anonipy-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_language_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.531341 anonipy-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-31 08:06:11.000000 anonipy-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-31 08:06:15.531341 anonipy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-31 08:06:11.000000 anonipy-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.523341 anonipy-0.0.6/anonipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.523341 anonipy-0.0.6/anonipy/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.523341 anonipy-0.0.6/anonipy/anonymize/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/extractors/entity_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/extractors/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.527341 anonipy-0.0.6/anonipy/anonymize/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/date_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/llm_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/mask_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/generators/number_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.527341 anonipy-0.0.6/anonipy/anonymize/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/strategies/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/strategies/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/strategies/pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/anonymize/strategies/redaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.527341 anonipy-0.0.6/anonipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/utils/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 08:06:11.000000 anonipy-0.0.6/anonipy/utils/language_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.527341 anonipy-0.0.6/anonipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-31 08:06:15.000000 anonipy-0.0.6/anonipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-31 08:06:15.000000 anonipy-0.0.6/anonipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:06:15.000000 anonipy-0.0.6/anonipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-31 08:06:15.000000 anonipy-0.0.6/anonipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 08:06:15.000000 anonipy-0.0.6/anonipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-31 08:06:11.000000 anonipy-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 08:06:11.000000 anonipy-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 08:06:15.531341 anonipy-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:06:15.527341 anonipy-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_language_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-31 08:06:11.000000 anonipy-0.0.6/test/test_strategies.py
```

### Comparing `anonipy-0.0.5/LICENSE` & `anonipy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/PKG-INFO` & `anonipy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.5
+Version: 0.0.6
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -39,23 +39,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy
-Requires-Dist: gliner
-Requires-Dist: gliner-spacy
+Requires-Dist: gliner==0.2.2
+Requires-Dist: gliner-spacy>=0.0.7
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: lingua-language-detector
 Requires-Dist: guidance==0.1.14
 Requires-Dist: sentencepiece
-Requires-Dist: pypdf
-Requires-Dist: python-docx
+Requires-Dist: pypdf>=4.2.0
+Requires-Dist: python-docx>=1.1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: python-githooks; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
@@ -104,14 +104,20 @@
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
 
+## ⬆️ Upgrade
+
+```bash
+pip install anonipy --upgrade
+```
+
 ## 🔎 Example
 
 The details of the example can be found in the [Overview](https://eriknovak.github.io/anonipy/documentation/notebooks/00-overview.ipynb).
 
 ```python
 original_text = """\
 Medical Record
```

### Comparing `anonipy-0.0.5/README.md` & `anonipy-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
 
+## ⬆️ Upgrade
+
+```bash
+pip install anonipy --upgrade
+```
+
 ## 🔎 Example
 
 The details of the example can be found in the [Overview](https://eriknovak.github.io/anonipy/documentation/notebooks/00-overview.ipynb).
 
 ```python
 original_text = """\
 Medical Record
```

### Comparing `anonipy-0.0.5/anonipy/anonymize/extractors/entity_extractor.py` & `anonipy-0.0.6/anonipy/anonymize/extractors/entity_extractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
 import importlib
 from typing import List, Tuple
+import warnings
 
+import torch
 from spacy import displacy
 from spacy.tokens import Doc
 from gliner_spacy.pipeline import GlinerSpacy
 
 from ..helpers import convert_spacy_to_entity
 from ..regex import regex_map
 from ...constants import LANGUAGES
@@ -17,17 +19,19 @@
 class EntityExtractor(ExtractorInterface):
 
     def __init__(
         self,
         labels: List[dict],
         lang: LANGUAGES = LANGUAGES.ENGLISH,
         score_th=0.5,
+        use_gpu=False,
     ):
         self.lang = lang
         self.score_th = score_th
+        self.use_gpu = use_gpu
         self.labels = self._prepare_labels(labels)
         self.pipeline = self._prepare_pipeline()
 
     def __call__(self, text: str) -> Tuple[Doc, List[Entity]]:
         doc = self.pipeline(text)
         entities, doc.ents = self._prepare_entities(doc)
         return doc, entities
@@ -46,21 +50,30 @@
                 continue
             regex = regex_map(l["type"])
             if regex is not None:
                 l["regex"] = regex
         return labels
 
     def _create_gliner_config(self):
+        map_location = "cpu"
+        if self.use_gpu and not torch.cuda.is_available():
+            return warnings.warn(
+                "The user requested GPU use, but not available GPU was found. Reverting back to CPU use."
+            )
+        if self.use_gpu and torch.cuda.is_available():
+            map_location = "cuda"
+
         return {
             # the model is specialized for extracting PII data
             "gliner_model": "urchade/gliner_multi_pii-v1",
             "labels": [l["label"] for l in self.labels],
             "threshold": self.score_th,
             "chunk_size": 384,
             "style": "ent",
+            "map_location": map_location,
         }
 
     def _prepare_pipeline(self):
         # load the appropriate parser for the language
         module_lang, class_lang = self.lang[0].lower(), self.lang[1].lower().title()
         language_module = importlib.import_module(f"spacy.lang.{module_lang}")
         language_class = getattr(language_module, class_lang)
```

### Comparing `anonipy-0.0.5/anonipy/anonymize/generators/date_generator.py` & `anonipy-0.0.6/anonipy/anonymize/generators/date_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/generators/llm_label_generator.py` & `anonipy-0.0.6/anonipy/anonymize/generators/llm_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/generators/mask_label_generator.py` & `anonipy-0.0.6/anonipy/anonymize/generators/mask_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/generators/number_generator.py` & `anonipy-0.0.6/anonipy/anonymize/generators/number_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/regex.py` & `anonipy-0.0.6/anonipy/anonymize/regex.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/strategies/masking.py` & `anonipy-0.0.6/anonipy/anonymize/strategies/masking.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/anonymize/strategies/pseudonymization.py` & `anonipy-0.0.6/anonipy/anonymize/strategies/pseudonymization.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
     def __init__(self, mapping, *args, **kwargs):
         self.mapping = mapping
 
     def anonymize(self, text: str, entities: List[Entity], *args, **kwargs):
         replacements = []
         for ent in entities[::-1]:
-            r = self._create_replacement(text, ent, replacements)
+            r = self._create_replacement(ent, text, replacements)
             text = (
                 text[: r["start_index"]] + r["anonymized_text"] + text[r["end_index"] :]
             )
             replacements.append(r)
         return text, replacements[::-1]
 
-    def _create_replacement(self, text: str, entity: Entity, replacements: List[dict]):
+    def _create_replacement(self, entity: Entity, text: str, replacements: List[dict]):
         # check if the replacement already exists
         anonymized_text = self._check_replacement(entity, replacements)
         # create a new replacement if it doesn't exist
         anonymized_text = (
             self.mapping(text, entity) if not anonymized_text else anonymized_text
         )
         return {
```

### Comparing `anonipy-0.0.5/anonipy/anonymize/strategies/redaction.py` & `anonipy-0.0.6/anonipy/anonymize/strategies/redaction.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/constants.py` & `anonipy-0.0.6/anonipy/constants.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/utils/file_system.py` & `anonipy-0.0.6/anonipy/utils/file_system.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy/utils/language_detector.py` & `anonipy-0.0.6/anonipy/utils/language_detector.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/anonipy.egg-info/PKG-INFO` & `anonipy-0.0.6/anonipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.5
+Version: 0.0.6
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -39,23 +39,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy
-Requires-Dist: gliner
-Requires-Dist: gliner-spacy
+Requires-Dist: gliner==0.2.2
+Requires-Dist: gliner-spacy>=0.0.7
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: lingua-language-detector
 Requires-Dist: guidance==0.1.14
 Requires-Dist: sentencepiece
-Requires-Dist: pypdf
-Requires-Dist: python-docx
+Requires-Dist: pypdf>=4.2.0
+Requires-Dist: python-docx>=1.1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: python-githooks; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
@@ -104,14 +104,20 @@
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
 
+## ⬆️ Upgrade
+
+```bash
+pip install anonipy --upgrade
+```
+
 ## 🔎 Example
 
 The details of the example can be found in the [Overview](https://eriknovak.github.io/anonipy/documentation/notebooks/00-overview.ipynb).
 
 ```python
 original_text = """\
 Medical Record
```

### Comparing `anonipy-0.0.5/anonipy.egg-info/SOURCES.txt` & `anonipy-0.0.6/anonipy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 anonipy/__init__.py
 anonipy/constants.py
 anonipy/definitions.py
-anonipy/version.py
 anonipy.egg-info/PKG-INFO
 anonipy.egg-info/SOURCES.txt
 anonipy.egg-info/dependency_links.txt
 anonipy.egg-info/requires.txt
 anonipy.egg-info/top_level.txt
 anonipy/anonymize/__init__.py
 anonipy/anonymize/helpers.py
```

### Comparing `anonipy-0.0.5/pyproject.toml` & `anonipy-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
-version = "0.0.5"
 name = "anonipy"
 description = "The data anonymization package"
 authors=[{ name = "Erik Novak", email = "erik.novak@ijs.si" }]
 readme = "README.md"
 license = { file = "LICENSE" }
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "version"]
 keywords = ["python", "machine learning", "natural language processing", "anonymization"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -43,8 +42,9 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["anonipy*"]
 
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
+dependencies = { file = ["requirements.txt"] }
+version = { attr = "anonipy.__version__" }
```

### Comparing `anonipy-0.0.5/test/test_extractors.py` & `anonipy-0.0.6/test/test_extractors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 import warnings
 
+import torch
+
 from anonipy.definitions import Entity
 from anonipy.anonymize.extractors import EntityExtractor
 from anonipy.constants import LANGUAGES
 
 # =====================================
 # Helper functions
 # =====================================
@@ -110,20 +112,34 @@
         except Exception as e:
             self.assertRaises(TypeError, e)
 
     def test_init_inputs(self):
         extractor = EntityExtractor(labels=labels, lang=LANGUAGES.ENGLISH, score_th=0.5)
         self.assertEqual(extractor.__class__, EntityExtractor)
 
+    def test_init_gpu(self):
+        if torch.cuda.is_available():
+            extractor = EntityExtractor(
+                labels=labels, lang=LANGUAGES.ENGLISH, score_th=0.5, use_gpu=True
+            )
+            self.assertEqual(extractor.__class__, EntityExtractor)
+
     def test_methods(self):
         extractor = EntityExtractor(labels=labels, lang=LANGUAGES.ENGLISH, score_th=0.5)
         self.assertEqual(hasattr(extractor, "__call__"), True)
         self.assertEqual(hasattr(extractor, "display"), True)
 
     def test_extract_default(self):
         extractor = EntityExtractor(labels=labels, lang=LANGUAGES.ENGLISH, score_th=0.5)
         doc, entities = extractor(original_text)
-        self.assertEqual(entities, original_entities)
+        for pred_entity, orig_entity in zip(entities, original_entities):
+            self.assertEqual(pred_entity.text, orig_entity.text)
+            self.assertEqual(pred_entity.label, orig_entity.label)
+            self.assertEqual(pred_entity.start_index, orig_entity.start_index)
+            self.assertEqual(pred_entity.end_index, orig_entity.end_index)
+            self.assertEqual(pred_entity.type, orig_entity.type)
+            self.assertEqual(pred_entity.regex, orig_entity.regex)
+            self.assertEqual(pred_entity.score >= 0.5, True)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `anonipy-0.0.5/test/test_file_system.py` & `anonipy-0.0.6/test/test_file_system.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/test/test_generators.py` & `anonipy-0.0.6/test/test_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,59 +38,63 @@
 
 test_entities = {
     "name": Entity(
         text="John Doe",
         label="name",
         start_index=30,
         end_index=38,
+        score=1.0,
         type="string",
         regex=".*",
     ),
     "date": Entity(
         text="20-05-2024",
         label="date",
         start_index=86,
         end_index=96,
+        score=1.0,
         type="date",
         regex="(\\d{1,2}[\\/\\-\\.]\\d{1,2}[\\/\\-\\.]\\d{2,4})|(\\d{2,4}[\\/\\-\\.]\\d{1,2}[\\/\\-\\.]\\d{1,2})",
     ),
     "integer": Entity(
         text="123456789",
         label="integer",
         start_index=121,
         end_index=132,
+        score=1.0,
         type="integer",
         regex="\d+",
     ),
     "float": Entity(
         text="123,456,789.000",
         label="float",
         start_index=121,
         end_index=132,
+        score=1.0,
         type="float",
         regex="[\d\.,]+",
     ),
     "custom": Entity(
         text="123-45-6789",
         label="custom",
         start_index=121,
         end_index=132,
+        score=1.0,
         type="custom",
         regex="\\d{3}-\\d{2}-\\d{4}",
     ),
 }
 
 
 # =====================================
 # Test LLM Label Generator
 # =====================================
 
 if torch.cuda.is_available():
-    # ! THESE TESTS REQUIRE GPU/CUDA !
-    # ! THIS WILL FAIL IF YOU DON'T HAVE GPU/CUDA !
+    # ! THESE TESTS REQUIRE GPU/CUDA! THIS WILL FAIL IF YOU DON'T HAVE GPU/CUDA!
 
     class TestLLMLabelGenerator(unittest.TestCase):
 
         @classmethod
         def setUpClass(self):
             self.generator = LLMLabelGenerator()
```

### Comparing `anonipy-0.0.5/test/test_language_detector.py` & `anonipy-0.0.6/test/test_language_detector.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/test/test_regex.py` & `anonipy-0.0.6/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.5/test/test_strategies.py` & `anonipy-0.0.6/test/test_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 # =====================================
 # Helper functions
 # =====================================
 
 test_text = "Test this string, and this test too!"
 test_entities = [
-    Entity(text="Test", label="test", start_index=0, end_index=4),
-    Entity(text="string", label="type", start_index=10, end_index=16),
-    Entity(text="test", label="test", start_index=27, end_index=31),
+    Entity(text="Test", label="test", start_index=0, end_index=4, score=1.0),
+    Entity(text="string", label="type", start_index=10, end_index=16, score=1.0),
+    Entity(text="test", label="test", start_index=27, end_index=31, score=1.0),
 ]
 
 
 def anonymization_mapping(text, entity):
     if entity.label == "test":
         return "[TEST]"
     elif entity.label == "type":
```

