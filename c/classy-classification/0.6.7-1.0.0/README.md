# Comparing `tmp/classy-classification-0.6.7.tar.gz` & `tmp/classy-classification-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy-classification-0.6.7.tar", max compression
+gzip compressed data, was "classy-classification-1.0.0.tar", max compression
```

## Comparing `classy-classification-0.6.7.tar` & `classy-classification-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-0.6.7/LICENSE
--rw-r--r--   0        0        0    10776 2023-08-31 19:05:34.385813 classy-classification-0.6.7/README.md
--rw-r--r--   0        0        0     2596 2023-08-31 19:05:34.700736 classy-classification-0.6.7/classy_classification/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-0.6.7/classy_classification/classifiers/__init__.py
--rw-r--r--   0        0        0    10545 2023-06-18 12:48:16.591005 classy-classification-0.6.7/classy_classification/classifiers/classy_skeleton.py
--rw-r--r--   0        0        0     9213 2023-06-20 12:46:07.445669 classy-classification-0.6.7/classy_classification/classifiers/classy_spacy.py
--rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-0.6.7/classy_classification/classifiers/classy_standalone.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-0.6.7/classy_classification/examples/__init__.py
--rw-r--r--   0        0        0     2324 2023-01-14 09:24:42.022043 classy-classification-0.6.7/classy_classification/examples/data.py
--rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-0.6.7/classy_classification/examples/individual_transformer.py
--rw-r--r--   0        0        0      344 2023-08-31 19:05:34.751850 classy-classification-0.6.7/classy_classification/examples/spacy_few_shot_external.py
--rw-r--r--   0        0        0      373 2023-08-31 19:05:34.707917 classy-classification-0.6.7/classy_classification/examples/spacy_internal_embeddings.py
--rw-r--r--   0        0        0      383 2023-08-31 19:06:41.271774 classy-classification-0.6.7/classy_classification/examples/spacy_zero_shot_external.py
--rw-r--r--   0        0        0     2353 2023-08-31 19:12:16.348588 classy-classification-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    12476 1970-01-01 00:00:00.000000 classy-classification-0.6.7/setup.py
--rw-r--r--   0        0        0    12630 1970-01-01 00:00:00.000000 classy-classification-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-1.0.0/LICENSE
+-rw-r--r--   0        0        0    10405 2024-05-31 14:48:56.068443 classy-classification-1.0.0/README.md
+-rw-r--r--   0        0        0     2596 2024-05-31 11:15:00.780044 classy-classification-1.0.0/classy_classification/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-1.0.0/classy_classification/classifiers/__init__.py
+-rw-r--r--   0        0        0     9949 2024-05-31 14:48:56.068984 classy-classification-1.0.0/classy_classification/classifiers/classy_skeleton.py
+-rw-r--r--   0        0        0     9551 2024-05-31 14:48:56.069254 classy-classification-1.0.0/classy_classification/classifiers/classy_spacy.py
+-rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-1.0.0/classy_classification/classifiers/classy_standalone.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-1.0.0/classy_classification/examples/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-31 11:15:00.781510 classy-classification-1.0.0/classy_classification/examples/data.py
+-rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-1.0.0/classy_classification/examples/individual_transformer.py
+-rw-r--r--   0        0        0      344 2023-08-31 19:05:34.751850 classy-classification-1.0.0/classy_classification/examples/spacy_few_shot_external.py
+-rw-r--r--   0        0        0      373 2023-08-31 19:05:34.707917 classy-classification-1.0.0/classy_classification/examples/spacy_internal_embeddings.py
+-rw-r--r--   0        0        0      383 2023-08-31 19:06:41.271774 classy-classification-1.0.0/classy_classification/examples/spacy_zero_shot_external.py
+-rw-r--r--   0        0        0     2158 2024-05-31 14:48:59.329409 classy-classification-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11948 1970-01-01 00:00:00.000000 classy-classification-1.0.0/setup.py
+-rw-r--r--   0        0        0    12124 1970-01-01 00:00:00.000000 classy-classification-1.0.0/PKG-INFO
```

### Comparing `classy-classification-0.6.7/LICENSE` & `classy-classification-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.7/README.md` & `classy-classification-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,17 @@
 [![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # Install
 ``` pip install classy-classification```
 
-Or, install with faster inference using ONNX.
-
-``` pip install classy-classification[onnx]```
 ## SetFit support
 
 I got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️
-## ONNX issues
-
-
-### pickling
-
-ONNX does show some issues when pickling the data.
-### M1
-
-Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
-
-```
-brew install cmake
-brew install protobuf
-pip3 install onnx --no-use-pep517
-```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
 # or import standalone
 # from classy_classification import ClassyClassifier
@@ -86,27 +68,31 @@
 
 print(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)
 
 # Output:
 #
 # [[{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
+
 ### Define random seed and verbosity
+
 ```python
 
 nlp.add_pipe(
     "classy_classification",
     config={
         "data": data,
         "verbose": True,
         "config": {"seed": 42}
     }
 )
 ```
+
 ### Multi-label classification
+
 Sometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.
 
 ```python
 import spacy
 
 data = {
     "furniture": ["This text is about chairs.",
@@ -139,19 +125,22 @@
 
 print(nlp("I am looking for furniture and kitchen equipment.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.92}, {"kitchen": 0.91}]
 ```
+
 ### Outlier detection
+
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
+
 ```python
 import spacy
 
 data_binary = {
     "inlier": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
@@ -170,15 +159,17 @@
 
 print(nlp("This text is a random text")._.cats)
 
 # Output:
 #
 # [{'inlier': 0.2926672385488411, 'outlier': 0.707332761451159}]
 ```
+
 Approach 2:
+
 ```python
 import spacy
 
 data_singular = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
@@ -194,15 +185,17 @@
 
 print(nlp("This text is a random text")._.cats)
 
 # Output:
 #
 # [{'furniture': 0, 'not_furniture': 1}]
 ```
+
 ## Sentence-transfomer embeddings
+
 ```python
 import spacy
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
@@ -223,15 +216,17 @@
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
+
 ## Hugginface zero-shot classifiers
+
 ```python
 import spacy
 
 data = ["furniture", "kitchen"]
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
@@ -246,26 +241,29 @@
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
+
 # Credits
+
 ## Inspiration Drawn From
+
 [Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.
 
 - [Scikit-learn](https://github.com/scikit-learn/scikit-learn)
 - [Rasa NLU](https://github.com/RasaHQ/rasa)
 - [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)
 - [Spacy](https://github.com/explosion/spaCy)
 
 ## Or buy me a coffee
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)
 
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)
 
 # Standalone usage without spaCy
 
 ```python
 
 from classy_classification import ClassyClassifier
 
@@ -298,14 +296,15 @@
         "max_cross_validation_folds": 5
     }
 )
 classifier("I am looking for kitchen appliances.")
 ```
 
 ## Save and load models
+
 ```python
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
```

### Comparing `classy-classification-0.6.7/classy_classification/__init__.py` & `classy-classification-1.0.0/classy_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.7/classy_classification/classifiers/classy_skeleton.py` & `classy-classification-1.0.0/classy_classification/classifiers/classy_skeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import collections
-import importlib.util
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
+from sentence_transformers import SentenceTransformer
 from sklearn import preprocessing
 from sklearn.model_selection import GridSearchCV
 from sklearn.multiclass import OneVsRestClassifier
 from sklearn.svm import SVC, OneClassSVM
 from spacy.language import Language
 from spacy.tokens import Doc, Span
 
-onnx = importlib.util.find_spec("fast_sentence_transformers") or importlib.util.find_spec("fast-sentence-transformers")
-if onnx is None:
-    from sentence_transformers import SentenceTransformer
-else:
-    from fast_sentence_transformers import (
-        FastSentenceTransformer as SentenceTransformer,
-    )
-
 
 class ClassySkeleton:
     def __init__(
         self,
         nlp: Language,
         name: str,
         data: dict,
@@ -277,22 +269,16 @@
             model (str, optional): the model name. Defaults to self.model, if no model is provided.
         """
         if model:  # update if overwritten
             self.model = model
         if device:
             self.device = device
 
-        if onnx is None:
-            if self.device in ["gpu", "cuda", 0]:
-                self.device = None  # If None, checks if a GPU can be used.
-            else:
-                self.device = "cpu"
-            self.encoder = SentenceTransformer(self.model, device=self.device)
+        if self.device in ["gpu", "cuda", 0]:
+            self.device = None  # If None, checks if a GPU can be used.
         else:
-            if device in ["gpu", "cuda", 0]:
-                self.encoder = SentenceTransformer(self.model, device=self.device, quantize=False)
-            else:
-                self.encoder = SentenceTransformer(self.model, device=self.device, quantize=True)
+            self.device = "cpu"
+        self.encoder = SentenceTransformer(self.model, device=self.device)
 
         if model:  # update if overwritten
             self.set_training_data()
             self.set_classification_model()
```

### Comparing `classy-classification-0.6.7/classy_classification/classifiers/classy_spacy.py` & `classy-classification-1.0.0/classy_classification/classifiers/classy_spacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib.util
 import warnings
 from typing import List, Union
 
 import numpy as np
-from spacy import util
+from spacy import __version__, util
 from spacy.tokens import Doc
 
 from .classy_skeleton import ClassyExternal, ClassySkeleton, ClassySkeletonFewShot
 
 
 class ClassySpacy:
     def sentence_pipe(self, doc: Doc):
@@ -93,16 +93,21 @@
             raise ValueError("This should be a List")
 
         embeddings = []
         for doc in docs:
             if doc.has_vector:
                 embeddings.append(doc.vector)
             elif doc.has_extension("trf_data"):
-                print(doc)
-                embeddings.append(doc._.trf_data.model_output.pooler_output[0])
+                # check if version is larger than 3.7.0
+                major, minor, patch = map(int, __version__.split("."))
+                is_greater_than_3_7 = (major > 3) or (major == 3 and minor >= 7)
+                if is_greater_than_3_7:
+                    embeddings.append(doc._.trf_data.all_outputs[0].data[-1])
+                else:
+                    embeddings.append(doc._.trf_data.model_output.pooler_output[0])
             else:
                 warnings.warn(
                     f"None of the words in the text `{str(doc)}` have vectors. Returning zeros.", stacklevel=1
                 )
                 embeddings.append(np.zeros(self.nlp.vocab.vectors_length))
         return np.array(embeddings)
```

### Comparing `classy-classification-0.6.7/classy_classification/classifiers/classy_standalone.py` & `classy-classification-1.0.0/classy_classification/classifiers/classy_standalone.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.7/classy_classification/examples/data.py` & `classy-classification-1.0.0/classy_classification/examples/data.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.7/pyproject.toml` & `classy-classification-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-classification"
-version = "0.6.7"
+version = "1.0.0"
 description = "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/classy-classification"
 repository = "https://github.com/davidberenstein1957/classy-classification"
 documentation = "https://github.com/davidberenstein1957/classy-classification"
@@ -27,23 +27,17 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 spacy = {extras = ["transformers"], version = "^3.0"}
 sentence-transformers = "^2.0"
 scikit-learn = "^1.0"
-pandas = "^1.4"
-fast-sentence-transformers = { version = "^0.4.1", optional = true }
-optimum = {extras = ["onnxruntime"], version = "^1.8.6"}
-transformers = {extras = ["torch"], version = ">4.20"}
-
-[tool.poetry.extras]
-onnx = ["fast-sentence-transformers", "optimum"]
-
-[tool.poetry.plugins]
+pandas = ">=1,<2"
+transformers = {extras = ["torch"], version = ">4.20,<5"}
+terminado = "<0.18"
 
 [tool.poetry.plugins."spacy_factories"]
 "spacy" = "classy_classification.__init__:make_text_categorizer"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
```

### Comparing `classy-classification-0.6.7/setup.py` & `classy-classification-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,41 +6,37 @@
  'classy_classification.classifiers',
  'classy_classification.examples']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.4,<2.0',
+['pandas>=1,<2',
  'scikit-learn>=1.0,<2.0',
  'sentence-transformers>=2.0,<3.0',
  'spacy[transformers]>=3.0,<4.0',
- 'transformers[torch]>4.20']
-
-extras_require = \
-{':extra == "onnx"': ['optimum[onnxruntime]>=1.8.6,<2.0.0'],
- 'onnx': ['fast-sentence-transformers>=0.4.1,<0.5.0']}
+ 'terminado<0.18',
+ 'transformers[torch]>4.20,<5']
 
 entry_points = \
 {'spacy_factories': ['spacy = '
                      'classy_classification.__init__:make_text_categorizer']}
 
 setup_kwargs = {
     'name': 'classy-classification',
-    'version': '0.6.7',
+    'version': '1.0.0',
     'description': "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!",
-    'long_description': '# Classy Classification\nHave you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn\'t have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).\n\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)\n[![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n# Install\n``` pip install classy-classification```\n\nOr, install with faster inference using ONNX.\n\n``` pip install classy-classification[onnx]```\n## SetFit support\n\nI got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️\n## ONNX issues\n\n\n### pickling\n\nONNX does show some issues when pickling the data.\n### M1\n\nSome [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.\n\n```\nbrew install cmake\nbrew install protobuf\npip3 install onnx --no-use-pep517\n```\n\n# Quickstart\n## SpaCy embeddings\n```python\nimport spacy\n# or import standalone\n# from classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.load("en_core_web_trf")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Sentence level classification\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy",\n        "include_sent": True\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)\n\n# Output:\n#\n# [[{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Define random seed and verbosity\n```python\n\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "verbose": True,\n        "config": {"seed": 42}\n    }\n)\n```\n### Multi-label classification\nSometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.\n\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table.",\n               "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table.",\n                "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy",\n        "multi_label": True,\n    }\n)\n\nprint(nlp("I am looking for furniture and kitchen equipment.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.92}, {"kitchen": 0.91}]\n```\n### Outlier detection\nSometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using\na binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.\n\nApproach 1:\n```python\nimport spacy\n\ndata_binary = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data_binary,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'inlier\': 0.2926672385488411, \'outlier\': 0.707332761451159}]\n```\nApproach 2:\n```python\nimport spacy\n\ndata_singular = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table."]\n}\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data_singular,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'furniture\': 0, \'not_furniture\': 1}]\n```\n## Sentence-transfomer embeddings\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n## Hugginface zero-shot classifiers\n```python\nimport spacy\n\ndata = ["furniture", "kitchen"]\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "typeform/distilbert-base-uncased-mnli",\n        "cat_type": "zero",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n# Credits\n## Inspiration Drawn From\n[Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.\n\n- [Scikit-learn](https://github.com/scikit-learn/scikit-learn)\n- [Rasa NLU](https://github.com/RasaHQ/rasa)\n- [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)\n- [Spacy](https://github.com/explosion/spaCy)\n\n## Or buy me a coffee\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)\n\n\n# Standalone usage without spaCy\n\n```python\n\nfrom classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nclassifier = ClassyClassifier(data=data)\nclassifier("I am looking for kitchen appliances.")\nclassifier.pipe(["I am looking for kitchen appliances."])\n\n# overwrite training data\nclassifier.set_training_data(data=data)\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite [embedding model](https://www.sbert.net/docs/pretrained_models.html)\nclassifier.set_embedding_model(model="paraphrase-MiniLM-L3-v2")\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite SVC config\nclassifier.set_classification_model(\n    config={\n        "C": [1, 2, 5, 10, 20, 100],\n        "kernel": ["linear"],\n        "max_cross_validation_folds": 5\n    }\n)\nclassifier("I am looking for kitchen appliances.")\n```\n\n## Save and load models\n```python\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\nclassifier = classyClassifier(data=data)\n\nwith open("./classifier.pkl", "wb") as f:\n    pickle.dump(classifier, f)\n\nf = open("./classifier.pkl", "rb")\nclassifier = pickle.load(f)\nclassifier("I am looking for kitchen appliances.")\n```\n',
+    'long_description': '# Classy Classification\nHave you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn\'t have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).\n\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)\n[![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n# Install\n``` pip install classy-classification```\n\n## SetFit support\n\nI got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️\n\n# Quickstart\n## SpaCy embeddings\n```python\nimport spacy\n# or import standalone\n# from classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.load("en_core_web_trf")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Sentence level classification\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy",\n        "include_sent": True\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)\n\n# Output:\n#\n# [[{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n\n### Define random seed and verbosity\n\n```python\n\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "verbose": True,\n        "config": {"seed": 42}\n    }\n)\n```\n\n### Multi-label classification\n\nSometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.\n\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table.",\n               "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table.",\n                "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "spacy",\n        "multi_label": True,\n    }\n)\n\nprint(nlp("I am looking for furniture and kitchen equipment.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.92}, {"kitchen": 0.91}]\n```\n\n### Outlier detection\n\nSometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using\na binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.\n\nApproach 1:\n\n```python\nimport spacy\n\ndata_binary = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data_binary,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'inlier\': 0.2926672385488411, \'outlier\': 0.707332761451159}]\n```\n\nApproach 2:\n\n```python\nimport spacy\n\ndata_singular = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table."]\n}\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data_singular,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'furniture\': 0, \'not_furniture\': 1}]\n```\n\n## Sentence-transfomer embeddings\n\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n\n## Hugginface zero-shot classifiers\n\n```python\nimport spacy\n\ndata = ["furniture", "kitchen"]\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "classy_classification",\n    config={\n        "data": data,\n        "model": "typeform/distilbert-base-uncased-mnli",\n        "cat_type": "zero",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n\n# Credits\n\n## Inspiration Drawn From\n\n[Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.\n\n- [Scikit-learn](https://github.com/scikit-learn/scikit-learn)\n- [Rasa NLU](https://github.com/RasaHQ/rasa)\n- [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)\n- [Spacy](https://github.com/explosion/spaCy)\n\n## Or buy me a coffee\n\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)\n\n# Standalone usage without spaCy\n\n```python\n\nfrom classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nclassifier = ClassyClassifier(data=data)\nclassifier("I am looking for kitchen appliances.")\nclassifier.pipe(["I am looking for kitchen appliances."])\n\n# overwrite training data\nclassifier.set_training_data(data=data)\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite [embedding model](https://www.sbert.net/docs/pretrained_models.html)\nclassifier.set_embedding_model(model="paraphrase-MiniLM-L3-v2")\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite SVC config\nclassifier.set_classification_model(\n    config={\n        "C": [1, 2, 5, 10, 20, 100],\n        "kernel": ["linear"],\n        "max_cross_validation_folds": 5\n    }\n)\nclassifier("I am looking for kitchen appliances.")\n```\n\n## Save and load models\n\n```python\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\nclassifier = classyClassifier(data=data)\n\nwith open("./classifier.pkl", "wb") as f:\n    pickle.dump(classifier, f)\n\nf = open("./classifier.pkl", "rb")\nclassifier = pickle.load(f)\nclassifier("I am looking for kitchen appliances.")\n```\n',
     'author': 'David Berenstein',
     'author_email': 'david.m.berenstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/davidberenstein1957/classy-classification',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `classy-classification-0.6.7/PKG-INFO` & `classy-classification-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-classification
-Version: 0.6.7
+Version: 1.0.0
 Summary: Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!
 Home-page: https://github.com/davidberenstein1957/classy-classification
 License: MIT
 Keywords: spacy,rasa,few-shot classification,nlu,sentence-transformers
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -20,22 +20,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Provides-Extra: onnx
-Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0); extra == "onnx"
-Requires-Dist: optimum[onnxruntime] (>=1.8.6,<2.0.0); extra == "onnx"
-Requires-Dist: pandas (>=1.4,<2.0)
+Requires-Dist: pandas (>=1,<2)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sentence-transformers (>=2.0,<3.0)
 Requires-Dist: spacy[transformers] (>=3.0,<4.0)
-Requires-Dist: transformers[torch] (>4.20)
+Requires-Dist: terminado (<0.18)
+Requires-Dist: transformers[torch] (>4.20,<5)
 Project-URL: Documentation, https://github.com/davidberenstein1957/classy-classification
 Project-URL: Repository, https://github.com/davidberenstein1957/classy-classification
 Description-Content-Type: text/markdown
 
 # Classy Classification
 Have you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
 
@@ -43,35 +41,17 @@
 [![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # Install
 ``` pip install classy-classification```
 
-Or, install with faster inference using ONNX.
-
-``` pip install classy-classification[onnx]```
 ## SetFit support
 
 I got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️
-## ONNX issues
-
-
-### pickling
-
-ONNX does show some issues when pickling the data.
-### M1
-
-Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
-
-```
-brew install cmake
-brew install protobuf
-pip3 install onnx --no-use-pep517
-```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
 # or import standalone
 # from classy_classification import ClassyClassifier
@@ -124,27 +104,31 @@
 
 print(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)
 
 # Output:
 #
 # [[{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
+
 ### Define random seed and verbosity
+
 ```python
 
 nlp.add_pipe(
     "classy_classification",
     config={
         "data": data,
         "verbose": True,
         "config": {"seed": 42}
     }
 )
 ```
+
 ### Multi-label classification
+
 Sometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.
 
 ```python
 import spacy
 
 data = {
     "furniture": ["This text is about chairs.",
@@ -177,19 +161,22 @@
 
 print(nlp("I am looking for furniture and kitchen equipment.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.92}, {"kitchen": 0.91}]
 ```
+
 ### Outlier detection
+
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
+
 ```python
 import spacy
 
 data_binary = {
     "inlier": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
@@ -208,15 +195,17 @@
 
 print(nlp("This text is a random text")._.cats)
 
 # Output:
 #
 # [{'inlier': 0.2926672385488411, 'outlier': 0.707332761451159}]
 ```
+
 Approach 2:
+
 ```python
 import spacy
 
 data_singular = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
@@ -232,15 +221,17 @@
 
 print(nlp("This text is a random text")._.cats)
 
 # Output:
 #
 # [{'furniture': 0, 'not_furniture': 1}]
 ```
+
 ## Sentence-transfomer embeddings
+
 ```python
 import spacy
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
@@ -261,15 +252,17 @@
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
+
 ## Hugginface zero-shot classifiers
+
 ```python
 import spacy
 
 data = ["furniture", "kitchen"]
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
@@ -284,26 +277,29 @@
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
+
 # Credits
+
 ## Inspiration Drawn From
+
 [Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.
 
 - [Scikit-learn](https://github.com/scikit-learn/scikit-learn)
 - [Rasa NLU](https://github.com/RasaHQ/rasa)
 - [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)
 - [Spacy](https://github.com/explosion/spaCy)
 
 ## Or buy me a coffee
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)
 
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)
 
 # Standalone usage without spaCy
 
 ```python
 
 from classy_classification import ClassyClassifier
 
@@ -336,14 +332,15 @@
         "max_cross_validation_folds": 5
     }
 )
 classifier("I am looking for kitchen appliances.")
 ```
 
 ## Save and load models
+
 ```python
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
```

