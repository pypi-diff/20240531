# Comparing `tmp/textualheatmap-1.1.1.tar.gz` & `tmp/textualheatmap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/textualheatmap-1.1.1.tar", last modified: Wed Mar 25 17:27:11 2020, max compression
+gzip compressed data, was "textualheatmap-1.2.0.tar", last modified: Thu May 30 22:37:17 2024, max compression
```

## Comparing `textualheatmap-1.1.1.tar` & `textualheatmap-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Andreas    (501) staff       (20)        0 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/
--rw-r--r--   0 Andreas    (501) staff       (20)     6858 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/PKG-INFO
--rw-r--r--   0 Andreas    (501) staff       (20)      107 2020-03-25 16:14:18.000000 textualheatmap-1.1.1/MANIFEST.in
-drwxr-xr-x   0 Andreas    (501) staff       (20)        0 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap/
--rw-r--r--   0 Andreas    (501) staff       (20)     2599 2020-03-20 13:26:51.000000 textualheatmap-1.1.1/textualheatmap/textual_heatmap_test.py
--rw-r--r--   0 Andreas    (501) staff       (20)       45 2020-03-18 13:02:40.000000 textualheatmap-1.1.1/textualheatmap/__init__.py
-drwxr-xr-x   0 Andreas    (501) staff       (20)        0 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap/web_assets/
--rw-r--r--   0 Andreas    (501) staff       (20)     6475 2020-03-25 17:26:32.000000 textualheatmap-1.1.1/textualheatmap/web_assets/textual_heatmap.js
--rw-r--r--   0 Andreas    (501) staff       (20)     2316 2020-03-25 16:55:26.000000 textualheatmap-1.1.1/textualheatmap/web_assets/textual_heatmap.css
--rw-r--r--   0 Andreas    (501) staff       (20)     6485 2020-03-25 17:05:37.000000 textualheatmap-1.1.1/textualheatmap/textual_heatmap.py
--rw-r--r--   0 Andreas    (501) staff       (20)     4726 2020-03-25 17:19:23.000000 textualheatmap-1.1.1/README.md
-drwxr-xr-x   0 Andreas    (501) staff       (20)        0 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/
--rw-r--r--   0 Andreas    (501) staff       (20)     6858 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/PKG-INFO
--rw-r--r--   0 Andreas    (501) staff       (20)        1 2020-03-20 11:24:50.000000 textualheatmap-1.1.1/textualheatmap.egg-info/not-zip-safe
--rw-r--r--   0 Andreas    (501) staff       (20)      457 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/SOURCES.txt
--rw-r--r--   0 Andreas    (501) staff       (20)        8 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/requires.txt
--rw-r--r--   0 Andreas    (501) staff       (20)       15 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/top_level.txt
--rw-r--r--   0 Andreas    (501) staff       (20)        1 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/textualheatmap.egg-info/dependency_links.txt
--rw-r--r--   0 Andreas    (501) staff       (20)     1391 2020-03-25 17:26:53.000000 textualheatmap-1.1.1/setup.py
--rw-r--r--   0 Andreas    (501) staff       (20)       79 2020-03-25 17:27:11.000000 textualheatmap-1.1.1/setup.cfg
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2024-05-30 22:37:17.528597 textualheatmap-1.2.0/
+-rw-r--r--   0 andreas    (501) staff       (20)     1054 2020-03-20 13:20:04.000000 textualheatmap-1.2.0/LICENSE.txt
+-rw-r--r--   0 andreas    (501) staff       (20)      107 2020-03-25 16:14:18.000000 textualheatmap-1.2.0/MANIFEST.in
+-rw-r--r--   0 andreas    (501) staff       (20)     6359 2024-05-30 22:37:17.528409 textualheatmap-1.2.0/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)     5366 2020-03-26 12:10:21.000000 textualheatmap-1.2.0/README.md
+-rw-r--r--   0 andreas    (501) staff       (20)     1135 2024-05-30 22:09:40.000000 textualheatmap-1.2.0/pyproject.toml
+-rw-r--r--   0 andreas    (501) staff       (20)       38 2024-05-30 22:37:17.528640 textualheatmap-1.2.0/setup.cfg
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2024-05-30 22:37:17.526983 textualheatmap-1.2.0/textualheatmap/
+-rw-r--r--   0 andreas    (501) staff       (20)       99 2024-05-30 22:32:52.000000 textualheatmap-1.2.0/textualheatmap/__init__.py
+-rw-r--r--   0 andreas    (501) staff       (20)     6997 2024-05-30 22:31:13.000000 textualheatmap-1.2.0/textualheatmap/textual_heatmap.py
+-rw-r--r--   0 andreas    (501) staff       (20)     2599 2020-03-20 13:26:51.000000 textualheatmap-1.2.0/textualheatmap/textual_heatmap_test.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2024-05-30 22:37:17.527880 textualheatmap-1.2.0/textualheatmap/web_assets/
+-rw-r--r--   0 andreas    (501) staff       (20)     2382 2024-05-30 21:55:57.000000 textualheatmap-1.2.0/textualheatmap/web_assets/textual_heatmap.css
+-rw-r--r--   0 andreas    (501) staff       (20)     6895 2024-05-30 22:20:52.000000 textualheatmap-1.2.0/textualheatmap/web_assets/textual_heatmap.js
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2024-05-30 22:37:17.528060 textualheatmap-1.2.0/textualheatmap.egg-info/
+-rw-r--r--   0 andreas    (501) staff       (20)     6359 2024-05-30 22:37:17.000000 textualheatmap-1.2.0/textualheatmap.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)      428 2024-05-30 22:37:17.000000 textualheatmap-1.2.0/textualheatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2024-05-30 22:37:17.000000 textualheatmap-1.2.0/textualheatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       46 2024-05-30 22:37:17.000000 textualheatmap-1.2.0/textualheatmap.egg-info/requires.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       15 2024-05-30 22:37:17.000000 textualheatmap-1.2.0/textualheatmap.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `textualheatmap-1.1.1/PKG-INFO` & `textualheatmap-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,195 @@
 Metadata-Version: 2.1
 Name: textualheatmap
-Version: 1.1.1
+Version: 1.2.0
 Summary: Create interactive textual heat maps for Jupiter notebooks
-Home-page: https://github.com/AndreasMadsen/python-textualheatmap
-Author: Andreas Madsen
-Author-email: amwebdk@gmail.com
+Author-email: Andreas Madsen <amwebdk@gmail.com>
 License: MIT
-Description: # textualheatmap
-        
-        **Create interactive textual heatmaps for Jupiter notebooks.**
-        
-        I originally published this visualization method in my distill paper
-        https://distill.pub/2019/memorization-in-rnns/. In this context, it is used
-        as a saliency map for showing which parts of a sentence are used to predict
-        the next word. However, the visualization method is more general-purpose than
-        that and can be used for any kind of textual heatmap purposes.
-        
-        `textualheatmap` works with python 3.6 or newer and is distributed under the
-        MIT license.
-        
-        ![Gif of textualheatmap](gifs/show_meta.gif)
-        
-        ## Install
-        
-        ```bash
-        pip install -U textualheatmap
-        ```
-        
-        ## API
-        
-        * [`textualheatmap.TextualHeatmap`](textualheatmap/textual_heatmap.py)
-        
-        ## Examples
-        
-        ### Example of sequential-charecter model with metadata visible
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
-        
-        ```python
-        from textualheatmap import TextualHeatmap
-        
-        data = [[
-            # GRU data
-            {"token":" ",
-             "meta":["the","one","of"],
-             "heat":[1,0,0,0,0,0,0,0,0]},
-            {"token":"c",
-             "meta":["can","called","century"],
-             "heat":[1,0.22,0,0,0,0,0,0,0]},
-            {"token":"o",
-             "meta":["country","could","company"],
-             "heat":[0.57,0.059,1,0,0,0,0,0,0]},
-            {"token":"n",
-             "meta":["control","considered","construction"],
-             "heat":[1,0.20,0.11,0.84,0,0,0,0,0]},
-            {"token":"t",
-             "meta":["control","continued","continental"],
-             "heat":[0.27,0.17,0.052,0.44,1,0,0,0,0]},
-            {"token":"e",
-             "meta":["context","content","contested"],
-             "heat":[0.17,0.039,0.034,0.22,1,0.53,0,0,0]},
-            {"token":"x",
-             "meta":["context","contexts","contemporary"],
-             "heat":[0.17,0.0044,0.021,0.17,1,0.90,0.48,0,0]},
-            {"token":"t",
-             "meta":["context","contexts","contentious"],
-             "heat":[0.14,0.011,0.034,0.14,0.68,1,0.80,0.86,0]},
-            {"token":" ",
-             "meta":["of","and","the"],
-             "heat":[0.014,0.0063,0.0044,0.011,0.034,0.10,0.32,0.28,1]},
-            # ...
-        ],[
-            # LSTM data
-            # ...
-        ]]
-        
-        heatmap = TextualHeatmap(
-            width = 600,
-            show_meta = True,
-            facet_titles = ['GRU', 'LSTM']
-        )
-        # Set data and render plot, this can be called again to replace
-        # the data.
-        heatmap.set_data(data)
-        # Focus on the token with the given index. Especially useful when
-        # `interactive=False` is used in `TextualHeatmap`.
-        heatmap.highlight(159)
-        ```
-        
-        ![Gif of learning-curve for keras example](gifs/show_meta.gif)
-        
-        ### Example of sequential-charecter model without metadata
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
-        
-        ```python
-        heatmap = TextualHeatmap(
-            show_meta = False,
-            facet_titles = ['LSTM', 'GRU'],
-            rotate_facet_titles = True
-        )
-        heatmap.set_data(data)
-        heatmap.highlight(159)
-        ```
-        
-        ![Gif of learning-curve for keras example](gifs/no_meta_and_rotated.gif)
-        
-        ### Example of non-sequential-word model
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/bert_hardcoded_example.ipynb)
-        
-        `format = True` can be set in the `data` object to inducate tokens that are
-        not directly used by the model. This is useful if word or sub-word tokenization
-        is used.
-        
-        
-        ```python
-        data = [[
-        {'token': '[CLR]',
-         'meta': ['', '', ''],
-         'heat': [1, 0, 0, 0, 0, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'context',
-         'meta': ['today', 'and', 'thus'],
-         'heat': [0.13, 0.40, 0.23, 1.0, 0.56, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'the',
-         'meta': ['##ual', 'the', '##ually'],
-         'heat': [0.11, 1.0, 0.34, 0.58, 0.59, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'formal',
-         'meta': ['formal', 'academic', 'systematic'],
-         'heat': [0.13, 0.74, 0.26, 0.35, 1.0, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'study',
-         'meta': ['##ization', 'study', '##ity'],
-         'heat': [0.09, 0.27, 0.19, 1.0, 0.26, ...]}
-        ]]
-        
-        heatmap = TextualHeatmap(facet_titles = ['BERT'], show_meta=True)
-        heatmap.set_data(data)
-        ```
-        
-        ## Citation
-        
-        If you use this in a publication, please cite my [Distill publication](https://distill.pub/2019/memorization-in-rnns/) where I first demonstrated this visualization method.
-        
-        ```bib
-        @article{madsen2019visualizing,
-          author = {Madsen, Andreas},
-          title = {Visualizing memorization in RNNs},
-          journal = {Distill},
-          year = {2019},
-          note = {https://distill.pub/2019/memorization-in-rnns},
-          doi = {10.23915/distill.00016}
-        }
-        ```
-        
-        ## Sponsor
-        
-        Sponsored by <a href="https://www.nearform.com/research/">NearForm Research</a>.
-        
-Keywords: saliency heatmap text textual jupyter colab interactive
-Platform: UNKNOWN
+Keywords: saliency,heatmap,text,textual,jupyter,colab,interactive
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: ipython
+Provides-Extra: testing
+Requires-Dist: nose; extra == "testing"
+Requires-Dist: jupyterlab; extra == "testing"
+Requires-Dist: tensorflow; extra == "testing"
+
+# textualheatmap
+
+**Create interactive textual heatmaps for Jupiter notebooks.**
+
+I originally published this visualization method in my distill paper
+https://distill.pub/2019/memorization-in-rnns/. In this context, it is used
+as a saliency map for showing which parts of a sentence are used to predict
+the next word. However, the visualization method is more general-purpose than
+that and can be used for any kind of textual heatmap purposes.
+
+`textualheatmap` works with python 3.6 or newer and is distributed under the
+MIT license.
+
+![Gif of saliency in RNN models](gifs/show_meta.gif)
+
+An end-to-end example of how to use the
+[HuggingFace 🤗 Transformers](https://github.com/huggingface/transformers) python
+module to create a textual saliency map for how each masked token is predicted.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/huggingface_bert_example.ipynb)
+
+
+![Gif of saliency in BERT models](gifs/huggingface_bert.gif)
+
+## Install
+
+```bash
+pip install -U textualheatmap
+```
+
+## API
+
+* [`textualheatmap.TextualHeatmap`](textualheatmap/textual_heatmap.py)
+
+## Examples
+
+### Example of sequential-charecter model with metadata visible
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
+
+```python
+from textualheatmap import TextualHeatmap
+
+data = [[
+    # GRU data
+    {"token":" ",
+     "meta":["the","one","of"],
+     "heat":[1,0,0,0,0,0,0,0,0]},
+    {"token":"c",
+     "meta":["can","called","century"],
+     "heat":[1,0.22,0,0,0,0,0,0,0]},
+    {"token":"o",
+     "meta":["country","could","company"],
+     "heat":[0.57,0.059,1,0,0,0,0,0,0]},
+    {"token":"n",
+     "meta":["control","considered","construction"],
+     "heat":[1,0.20,0.11,0.84,0,0,0,0,0]},
+    {"token":"t",
+     "meta":["control","continued","continental"],
+     "heat":[0.27,0.17,0.052,0.44,1,0,0,0,0]},
+    {"token":"e",
+     "meta":["context","content","contested"],
+     "heat":[0.17,0.039,0.034,0.22,1,0.53,0,0,0]},
+    {"token":"x",
+     "meta":["context","contexts","contemporary"],
+     "heat":[0.17,0.0044,0.021,0.17,1,0.90,0.48,0,0]},
+    {"token":"t",
+     "meta":["context","contexts","contentious"],
+     "heat":[0.14,0.011,0.034,0.14,0.68,1,0.80,0.86,0]},
+    {"token":" ",
+     "meta":["of","and","the"],
+     "heat":[0.014,0.0063,0.0044,0.011,0.034,0.10,0.32,0.28,1]},
+    # ...
+],[
+    # LSTM data
+    # ...
+]]
+
+heatmap = TextualHeatmap(
+    width = 600,
+    show_meta = True,
+    facet_titles = ['GRU', 'LSTM']
+)
+# Set data and render plot, this can be called again to replace
+# the data.
+heatmap.set_data(data)
+# Focus on the token with the given index. Especially useful when
+# `interactive=False` is used in `TextualHeatmap`.
+heatmap.highlight(159)
+```
+
+![Shows saliency with predicted words at metadata](gifs/show_meta.gif)
+
+### Example of sequential-charecter model without metadata
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
+
+When `show_meta` is not `True`, the `meta` part of the `data` object has no effect.
+
+```python
+heatmap = TextualHeatmap(
+    facet_titles = ['LSTM', 'GRU'],
+    rotate_facet_titles = True
+)
+heatmap.set_data(data)
+heatmap.highlight(159)
+```
+
+![Shows saliency without metadata](gifs/no_meta_and_rotated.gif)
+
+### Example of non-sequential-word model
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/bert_hardcoded_example.ipynb)
+
+`format = True` can be set in the `data` object to inducate tokens that are
+not directly used by the model. This is useful if word or sub-word tokenization
+is used.
+
+
+```python
+data = [[
+{'token': '[CLR]',
+ 'meta': ['', '', ''],
+ 'heat': [1, 0, 0, 0, 0, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'context',
+ 'meta': ['today', 'and', 'thus'],
+ 'heat': [0.13, 0.40, 0.23, 1.0, 0.56, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'the',
+ 'meta': ['##ual', 'the', '##ually'],
+ 'heat': [0.11, 1.0, 0.34, 0.58, 0.59, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'formal',
+ 'meta': ['formal', 'academic', 'systematic'],
+ 'heat': [0.13, 0.74, 0.26, 0.35, 1.0, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'study',
+ 'meta': ['##ization', 'study', '##ity'],
+ 'heat': [0.09, 0.27, 0.19, 1.0, 0.26, ...]}
+]]
+
+heatmap = TextualHeatmap(facet_titles = ['BERT'], show_meta=True)
+heatmap.set_data(data)
+```
+
+![Shows saliency in a BERT model, using sub-word tokenization](gifs/sub_word_tokenized.gif)
+
+## Citation
+
+If you use this in a publication, please cite my [Distill publication](https://distill.pub/2019/memorization-in-rnns/) where I first demonstrated this visualization method.
+
+```bib
+@article{madsen2019visualizing,
+  author = {Madsen, Andreas},
+  title = {Visualizing memorization in RNNs},
+  journal = {Distill},
+  year = {2019},
+  note = {https://distill.pub/2019/memorization-in-rnns},
+  doi = {10.23915/distill.00016}
+}
+```
+
+## Sponsor
+
+Sponsored by <a href="https://www.nearform.com/research/">NearForm Research</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `textualheatmap-1.1.1/textualheatmap/textual_heatmap_test.py` & `textualheatmap-1.2.0/textualheatmap/textual_heatmap_test.py`

 * *Files identical despite different names*

### Comparing `textualheatmap-1.1.1/textualheatmap/web_assets/textual_heatmap.js` & `textualheatmap-1.2.0/textualheatmap/web_assets/textual_heatmap.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -96,19 +96,26 @@
             while (this.content.childNodes.length > 0) {
                 this.content.removeChild(this.content.firstChild);
             }
 
             for (let i = 0; i < data.length; i++) {
                 const tokenNode = document.createElement('span');
                 const heatIndex = this.heatIndexToNodeElement.length;
-                tokenNode.appendChild(document.createTextNode(data[i].token));
-                if (this.settings.interactive && !data[i].format) {
-                    tokenNode.addEventListener('mouseover', () => this.onmouseover(heatIndex), false);
-                    this.heatIndexToNodeElement.push(tokenNode)
-                    this.nonFormatData.push(data[i])
+                // allow a wrap-break after every token
+                const wrapUnicode = this.settings.wrapAfterTokens ? '\u200B' : '';
+                tokenNode.appendChild(document.createTextNode(data[i].token + wrapUnicode));
+                // only enable event listener for format items
+                if (!data[i].format) {
+                    if (this.settings.interactive) {
+                        tokenNode.addEventListener('mouseover', () => this.onmouseover(heatIndex), false);
+                    }
+                    // in the non-interactive case, the .highlight can still be called. So always populate
+                    // these datastructures.
+                    this.heatIndexToNodeElement.push(tokenNode);
+                    this.nonFormatData.push(data[i]);
                 }
                 this.content.appendChild(tokenNode);
             }
 
             if (this.highlightIndex !== null) {
                 this.highlight(this.highlightIndex);
             }
```

### Comparing `textualheatmap-1.1.1/textualheatmap/web_assets/textual_heatmap.css` & `textualheatmap-1.2.0/textualheatmap/web_assets/textual_heatmap.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 .textual-heatmap .facet {
   display: grid;
-  grid-template-columns: 1fr 60px;
+  grid-template-columns: 1fr auto;
   grid-template-rows: 40px auto;
-  grid-template-areas:
-    "meta-content ."
-    "token-content facet-title";
+  grid-template-areas: "meta-content ."
+                       "token-content facet-title";
   margin-bottom: 0.5em;
 }
 
+.textual-heatmap .facet.rotate-facet-title {
+  grid-template-columns: 1fr 40px;
+}
+
 .textual-heatmap .facet.hide-meta-content {
   grid-template-rows: auto;
   grid-template-areas:
-    "token-content facet-title";
+      "token-content facet-title";
 }
 
 .textual-heatmap .facet .token-content {
   grid-area: token-content;
 
   font-family: monospace;
   padding: 0.5em;
   box-sizing: border-box;
   background: #365d8d;
   color: white;
   line-height: 1.4em;
   border-radius: 0 0 0 5px;
+
 }
 
 .textual-heatmap .facet.hide-meta-content .token-content {
-    border-radius: 5px 0 0 5px;
+  border-radius: 5px 0 0 5px;
 }
 
 .textual-heatmap .facet .token-content span {
   border-bottom: 0.2em solid transparent;
-  white-space: pre-wrap;
 }
 
 .textual-heatmap .facet .token-content span.selected {
   border-bottom-color: white;
 }
 
 .textual-heatmap .facet .meta-content {
@@ -44,15 +47,15 @@
   display: grid;
   grid-template-columns: repeat(auto-fit, minmax(0px, 1fr));
   grid-column-gap: 2px;
   align-items: center;
 }
 
 .textual-heatmap .facet.hide-meta-content .meta-content {
-    display: none;
+  display: none;
 }
 
 .textual-heatmap .facet .meta-content .meta-content-item {
   display: flex;
   justify-content: center;
   align-items: center;
   padding: 0 5px;
@@ -62,42 +65,42 @@
   color: black;
   border-bottom: none;
   text-overflow: ellipsis;
   overflow: hidden;
 }
 
 .textual-heatmap .facet .meta-content .meta-content-item:first-of-type {
-    border-radius: 5px 0 0 0;
+  border-radius: 5px 0 0 0;
 }
 
 .textual-heatmap .facet .meta-content .meta-content-item:last-of-type {
-    border-radius: 0 5px 0 0;
+  border-radius: 0 5px 0 0;
 }
 
 .textual-heatmap .facet .meta-content .meta-content-item:first-of-type:last-of-type {
-    border-radius: 5px 5px 0 0;
+  border-radius: 5px 5px 0 0;
 }
 
 .textual-heatmap .facet .facet-title {
   grid-area: facet-title;
 
   display: flex;
-  max-width: 60px;
   background: #EEEEEE;
   justify-content: center;
   color: #555555;
   border-radius: 0 5px 5px 0;
   border: 1px solid #E0E0E0;
   border-left: none;
+  padding: 0 5px;
 }
 
 .textual-heatmap .facet .facet-title span {
   align-self: center;
   display: inline-block;
   transform-origin: center center;
   line-height: 1em;
   text-align: center;
 }
 
 .textual-heatmap .facet.rotate-facet-title .facet-title span {
   transform: translate(0, 0) rotate(90deg);
-}
+}
```

### Comparing `textualheatmap-1.1.1/textualheatmap/textual_heatmap.py` & `textualheatmap-1.2.0/textualheatmap/textual_heatmap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 
 import uuid
 import json
 import os.path as path
 import IPython
+from typing import TypedDict, Callable
 
 web_assets_dir = path.join(path.dirname(path.realpath(__file__)), 'web_assets')
 
+class TokenData(TypedDict):
+    token: str
+    meta: list[str]|None
+    heat: list[float]
+
 class TextualHeatmap:
-    """Create interactive textual heatmaps for Jupiter notebooks.
+    def __init__(self,
+                 show_meta: bool = False,
+                 facet_titles: list[str] = ['Heatmap'],
+                 rotate_facet_titles: bool = False,
+                 wrap_after_token: bool = True,
+                 width: int = 600,
+                 interactive: bool = True,
+                 display_fn: Callable=IPython.display.display
+    ):
+        """Create interactive textual heatmaps for Jupiter notebooks.
 
-    This is useful for PyTorch or pure TensorFlow. You should properly use
-    `KerasLearningCurve` if you use keras.
+        This is useful for PyTorch or pure TensorFlow. You should properly use
+        `KerasLearningCurve` if you use keras.
 
-    Line description: dict with the properties `name` and `color`.
-    Axis description:
+        Line description: dict with the properties `name` and `color`.
+        Axis description:
 
-    Example:
-        heatmap = TextualHeatmap(
-            show_meta = True,
-            facet_titles = ['LSTM', 'GRU']
-        )
-        heatmap.set_data([
-            [{
-                "token": 'a',
-                "meta": ['and', 'africa', 'america'],
-                "heat": [1, 0, 0]
-            }, {
-                "token": 'n',
-                "meta": ['and', 'anecdote', 'antelope'],
-                "heat": [0.3, 0.7, 0]
-            }, {
-                "token": 'd',
-                "meta": ['and', 'andante', 'andosol'],
-                "heat": [0.2, 0.3, 0.5]
-            }],
-            [{
-                "token": 'a',
-                "meta": ['and', 'africa', 'america'],
-                "heat": [1, 0, 0]
-            }, {
-                "token": 'n',
-                "meta": ['and', 'anecdote', 'antelope'],
-                "heat": [0.1, 0.9, 0]
-            }, {
-                "token": 'd',
-                "meta": ['and', 'andante', 'andosol'],
-                "heat": [0.1, 0.1, 0.8]
-            }]
-        ])
-        heatmap.highlight(1)
-
-    Arguments:
-        show_meta: The meta texts on top of each facet (Default: False).
-        facet_titles: The title on each facet (Default: ['Heatmap']).
-        rotate_facet_titles: If true, the facet titles will be rotated 90deg (Default: False).
-        width: The width of the heatmap (Default: 600).
-        interactive: Should the heatmap be interactive on mouseover. (Default: True)
-        debug: Depending on the notebook, a JavaScript evaluation does not provide
-            a stack trace in the developer console. Setting this to `true` works
-            around that by injecting `<script>` tags instead.
-    """
-    def __init__(self,
-                 show_meta = False,
-                 facet_titles = ['Heatmap'],
-                 rotate_facet_titles = False,
-                 width = 600,
-                 interactive = True,
-                 display_fn=IPython.display.display,
-                 debug=False
-    ):
+        Example:
+            heatmap = TextualHeatmap(
+                show_meta = True,
+                facet_titles = ['LSTM', 'GRU']
+            )
+            heatmap.set_data([
+                [{
+                    "token": 'a',
+                    "meta": ['and', 'africa', 'america'],
+                    "heat": [1, 0, 0]
+                }, {
+                    "token": 'n',
+                    "meta": ['and', 'anecdote', 'antelope'],
+                    "heat": [0.3, 0.7, 0]
+                }, {
+                    "token": 'd',
+                    "meta": ['and', 'andante', 'andosol'],
+                    "heat": [0.2, 0.3, 0.5]
+                }],
+                [{
+                    "token": 'a',
+                    "meta": ['and', 'africa', 'america'],
+                    "heat": [1, 0, 0]
+                }, {
+                    "token": 'n',
+                    "meta": ['and', 'anecdote', 'antelope'],
+                    "heat": [0.1, 0.9, 0]
+                }, {
+                    "token": 'd',
+                    "meta": ['and', 'andante', 'andosol'],
+                    "heat": [0.1, 0.1, 0.8]
+                }]
+            ])
+            heatmap.highlight(1)
+
+        Args:
+            show_meta (bool, optional): The meta texts on top of each facet. Defaults to False.
+            facet_titles (list[str], optional): The title on each facet. Defaults to ['Heatmap'].
+            rotate_facet_titles (bool, optional): If true, the facet titles will be rotated 90deg. Defaults to False.
+            wrap_after_token (bool, optional): If wrap is allowed after token, otherwise it's only after space and hypens. Defaults to True.
+            width (int, optional): The width of the heatmap. Defaults to 600.
+            interactive (bool, optional): Should the heatmap be interactive on mouseover.. Defaults to True.
+            display_fn (Callable, optional): _description_. Defaults to IPython.display.display.
+        """
         if not isinstance(width, int) or width <= 0:
             raise ValueError(f'width must be a positive number, was {width}')
 
         if not isinstance(show_meta, bool):
             raise ValueError('show_meta must be a boolean')
 
         if not isinstance(interactive, bool):
@@ -84,22 +89,22 @@
             if not isinstance(facet_title, str):
                 raise ValueError(f'facet_title["{facet_title_i}"] must a string')
 
         if not isinstance(rotate_facet_titles, bool):
             raise ValueError('rotate_facet_titles must be a boolean')
 
         # Store settings
-        self._debug = debug
         self._display = display_fn
         self._settings = {
             'id': str(uuid.uuid4()),
             'width': width,
             'showMeta': show_meta,
             'facetTitles': facet_titles,
             'rotateFacetTitles': rotate_facet_titles,
+            'wrapAfterTokens': wrap_after_token,
             'interactive': interactive
         }
 
         # Prepear data containers
         self._data = []
         self._display(self._create_inital_html())
         self._data_element = self._display(
@@ -119,15 +124,15 @@
                 f'<script>{js_fp.read()}</script>'
                 f'<div id="{self._settings["id"]}" class="textual-heatmap"></div>'
                 f'<script>'
                 f'  window.setupTextualHeatmap({json.dumps(self._settings)});'
                 f'</script>'
             )
 
-    def set_data(self, data):
+    def set_data(self, data: list[list[TokenData]]):
         """Sets the data and render the heatmap.
 
         `data` is a list of `FacetData`. Each `FacetData` is a
         list of `TokenData`.
 
             TokenData = {"token": str, "meta": List[str], "heat": List[float], "format": bool}
 
@@ -143,31 +148,31 @@
         Examples:
             data = [[
                 { "token": "context", "meta": ["content", "concise", "context"], "heat": [0, 0.2] },
                 { "token": " ", "format": True },
                 { "token": "is", "meta": ["are", "that", "is"], "heat": [0.7, 0] }
             ]]
 
-        Arguments:
-            data: List[List[TokenData]] - Heatmap data.
+        Args:
+            data (list[TokenData]): Heatmap data.
         """
         disp = IPython.display.HTML(
             f'<script>'
             f'  window.setDataTextualHeatmap({json.dumps(self._settings)}, {json.dumps(data)});'
             f'</script>'
         )
         self._data_element.update(disp)
 
-    def highlight(self, index):
+    def highlight(self, index: int):
         """Select a token index to be highlighted on the heatmap.
 
         This will affect all facets in the heatmap.
 
-        Arguments:
-            index: integer - The token index to highlight.
+        Args:
+            index (int): The token index to highlight.
         """
         disp = IPython.display.HTML(
             f'<script>'
             f'  window.highlightTextualHeatmap({json.dumps(self._settings)}, {index});'
             f'</script>'
         )
         self._highlight_element.update(disp)
```

### Comparing `textualheatmap-1.1.1/README.md` & `textualheatmap-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,24 @@
 as a saliency map for showing which parts of a sentence are used to predict
 the next word. However, the visualization method is more general-purpose than
 that and can be used for any kind of textual heatmap purposes.
 
 `textualheatmap` works with python 3.6 or newer and is distributed under the
 MIT license.
 
-![Gif of textualheatmap](gifs/show_meta.gif)
+![Gif of saliency in RNN models](gifs/show_meta.gif)
+
+An end-to-end example of how to use the
+[HuggingFace 🤗 Transformers](https://github.com/huggingface/transformers) python
+module to create a textual saliency map for how each masked token is predicted.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/huggingface_bert_example.ipynb)
+
+
+![Gif of saliency in BERT models](gifs/huggingface_bert.gif)
 
 ## Install
 
 ```bash
 pip install -U textualheatmap
 ```
 
@@ -76,31 +85,32 @@
 # the data.
 heatmap.set_data(data)
 # Focus on the token with the given index. Especially useful when
 # `interactive=False` is used in `TextualHeatmap`.
 heatmap.highlight(159)
 ```
 
-![Gif of learning-curve for keras example](gifs/show_meta.gif)
+![Shows saliency with predicted words at metadata](gifs/show_meta.gif)
 
 ### Example of sequential-charecter model without metadata
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
 
+When `show_meta` is not `True`, the `meta` part of the `data` object has no effect.
+
 ```python
 heatmap = TextualHeatmap(
-    show_meta = False,
     facet_titles = ['LSTM', 'GRU'],
     rotate_facet_titles = True
 )
 heatmap.set_data(data)
 heatmap.highlight(159)
 ```
 
-![Gif of learning-curve for keras example](gifs/no_meta_and_rotated.gif)
+![Shows saliency without metadata](gifs/no_meta_and_rotated.gif)
 
 ### Example of non-sequential-word model
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/bert_hardcoded_example.ipynb)
 
 `format = True` can be set in the `data` object to inducate tokens that are
 not directly used by the model. This is useful if word or sub-word tokenization
@@ -134,14 +144,16 @@
  'heat': [0.09, 0.27, 0.19, 1.0, 0.26, ...]}
 ]]
 
 heatmap = TextualHeatmap(facet_titles = ['BERT'], show_meta=True)
 heatmap.set_data(data)
 ```
 
+![Shows saliency in a BERT model, using sub-word tokenization](gifs/sub_word_tokenized.gif)
+
 ## Citation
 
 If you use this in a publication, please cite my [Distill publication](https://distill.pub/2019/memorization-in-rnns/) where I first demonstrated this visualization method.
 
 ```bib
 @article{madsen2019visualizing,
   author = {Madsen, Andreas},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `textualheatmap-1.1.1/textualheatmap.egg-info/PKG-INFO` & `textualheatmap-1.2.0/textualheatmap.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,195 @@
 Metadata-Version: 2.1
 Name: textualheatmap
-Version: 1.1.1
+Version: 1.2.0
 Summary: Create interactive textual heat maps for Jupiter notebooks
-Home-page: https://github.com/AndreasMadsen/python-textualheatmap
-Author: Andreas Madsen
-Author-email: amwebdk@gmail.com
+Author-email: Andreas Madsen <amwebdk@gmail.com>
 License: MIT
-Description: # textualheatmap
-        
-        **Create interactive textual heatmaps for Jupiter notebooks.**
-        
-        I originally published this visualization method in my distill paper
-        https://distill.pub/2019/memorization-in-rnns/. In this context, it is used
-        as a saliency map for showing which parts of a sentence are used to predict
-        the next word. However, the visualization method is more general-purpose than
-        that and can be used for any kind of textual heatmap purposes.
-        
-        `textualheatmap` works with python 3.6 or newer and is distributed under the
-        MIT license.
-        
-        ![Gif of textualheatmap](gifs/show_meta.gif)
-        
-        ## Install
-        
-        ```bash
-        pip install -U textualheatmap
-        ```
-        
-        ## API
-        
-        * [`textualheatmap.TextualHeatmap`](textualheatmap/textual_heatmap.py)
-        
-        ## Examples
-        
-        ### Example of sequential-charecter model with metadata visible
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
-        
-        ```python
-        from textualheatmap import TextualHeatmap
-        
-        data = [[
-            # GRU data
-            {"token":" ",
-             "meta":["the","one","of"],
-             "heat":[1,0,0,0,0,0,0,0,0]},
-            {"token":"c",
-             "meta":["can","called","century"],
-             "heat":[1,0.22,0,0,0,0,0,0,0]},
-            {"token":"o",
-             "meta":["country","could","company"],
-             "heat":[0.57,0.059,1,0,0,0,0,0,0]},
-            {"token":"n",
-             "meta":["control","considered","construction"],
-             "heat":[1,0.20,0.11,0.84,0,0,0,0,0]},
-            {"token":"t",
-             "meta":["control","continued","continental"],
-             "heat":[0.27,0.17,0.052,0.44,1,0,0,0,0]},
-            {"token":"e",
-             "meta":["context","content","contested"],
-             "heat":[0.17,0.039,0.034,0.22,1,0.53,0,0,0]},
-            {"token":"x",
-             "meta":["context","contexts","contemporary"],
-             "heat":[0.17,0.0044,0.021,0.17,1,0.90,0.48,0,0]},
-            {"token":"t",
-             "meta":["context","contexts","contentious"],
-             "heat":[0.14,0.011,0.034,0.14,0.68,1,0.80,0.86,0]},
-            {"token":" ",
-             "meta":["of","and","the"],
-             "heat":[0.014,0.0063,0.0044,0.011,0.034,0.10,0.32,0.28,1]},
-            # ...
-        ],[
-            # LSTM data
-            # ...
-        ]]
-        
-        heatmap = TextualHeatmap(
-            width = 600,
-            show_meta = True,
-            facet_titles = ['GRU', 'LSTM']
-        )
-        # Set data and render plot, this can be called again to replace
-        # the data.
-        heatmap.set_data(data)
-        # Focus on the token with the given index. Especially useful when
-        # `interactive=False` is used in `TextualHeatmap`.
-        heatmap.highlight(159)
-        ```
-        
-        ![Gif of learning-curve for keras example](gifs/show_meta.gif)
-        
-        ### Example of sequential-charecter model without metadata
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
-        
-        ```python
-        heatmap = TextualHeatmap(
-            show_meta = False,
-            facet_titles = ['LSTM', 'GRU'],
-            rotate_facet_titles = True
-        )
-        heatmap.set_data(data)
-        heatmap.highlight(159)
-        ```
-        
-        ![Gif of learning-curve for keras example](gifs/no_meta_and_rotated.gif)
-        
-        ### Example of non-sequential-word model
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/bert_hardcoded_example.ipynb)
-        
-        `format = True` can be set in the `data` object to inducate tokens that are
-        not directly used by the model. This is useful if word or sub-word tokenization
-        is used.
-        
-        
-        ```python
-        data = [[
-        {'token': '[CLR]',
-         'meta': ['', '', ''],
-         'heat': [1, 0, 0, 0, 0, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'context',
-         'meta': ['today', 'and', 'thus'],
-         'heat': [0.13, 0.40, 0.23, 1.0, 0.56, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'the',
-         'meta': ['##ual', 'the', '##ually'],
-         'heat': [0.11, 1.0, 0.34, 0.58, 0.59, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'formal',
-         'meta': ['formal', 'academic', 'systematic'],
-         'heat': [0.13, 0.74, 0.26, 0.35, 1.0, ...]},
-        {'token': ' ',
-         'format': True},
-        {'token': 'study',
-         'meta': ['##ization', 'study', '##ity'],
-         'heat': [0.09, 0.27, 0.19, 1.0, 0.26, ...]}
-        ]]
-        
-        heatmap = TextualHeatmap(facet_titles = ['BERT'], show_meta=True)
-        heatmap.set_data(data)
-        ```
-        
-        ## Citation
-        
-        If you use this in a publication, please cite my [Distill publication](https://distill.pub/2019/memorization-in-rnns/) where I first demonstrated this visualization method.
-        
-        ```bib
-        @article{madsen2019visualizing,
-          author = {Madsen, Andreas},
-          title = {Visualizing memorization in RNNs},
-          journal = {Distill},
-          year = {2019},
-          note = {https://distill.pub/2019/memorization-in-rnns},
-          doi = {10.23915/distill.00016}
-        }
-        ```
-        
-        ## Sponsor
-        
-        Sponsored by <a href="https://www.nearform.com/research/">NearForm Research</a>.
-        
-Keywords: saliency heatmap text textual jupyter colab interactive
-Platform: UNKNOWN
+Keywords: saliency,heatmap,text,textual,jupyter,colab,interactive
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: ipython
+Provides-Extra: testing
+Requires-Dist: nose; extra == "testing"
+Requires-Dist: jupyterlab; extra == "testing"
+Requires-Dist: tensorflow; extra == "testing"
+
+# textualheatmap
+
+**Create interactive textual heatmaps for Jupiter notebooks.**
+
+I originally published this visualization method in my distill paper
+https://distill.pub/2019/memorization-in-rnns/. In this context, it is used
+as a saliency map for showing which parts of a sentence are used to predict
+the next word. However, the visualization method is more general-purpose than
+that and can be used for any kind of textual heatmap purposes.
+
+`textualheatmap` works with python 3.6 or newer and is distributed under the
+MIT license.
+
+![Gif of saliency in RNN models](gifs/show_meta.gif)
+
+An end-to-end example of how to use the
+[HuggingFace 🤗 Transformers](https://github.com/huggingface/transformers) python
+module to create a textual saliency map for how each masked token is predicted.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/huggingface_bert_example.ipynb)
+
+
+![Gif of saliency in BERT models](gifs/huggingface_bert.gif)
+
+## Install
+
+```bash
+pip install -U textualheatmap
+```
+
+## API
+
+* [`textualheatmap.TextualHeatmap`](textualheatmap/textual_heatmap.py)
+
+## Examples
+
+### Example of sequential-charecter model with metadata visible
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
+
+```python
+from textualheatmap import TextualHeatmap
+
+data = [[
+    # GRU data
+    {"token":" ",
+     "meta":["the","one","of"],
+     "heat":[1,0,0,0,0,0,0,0,0]},
+    {"token":"c",
+     "meta":["can","called","century"],
+     "heat":[1,0.22,0,0,0,0,0,0,0]},
+    {"token":"o",
+     "meta":["country","could","company"],
+     "heat":[0.57,0.059,1,0,0,0,0,0,0]},
+    {"token":"n",
+     "meta":["control","considered","construction"],
+     "heat":[1,0.20,0.11,0.84,0,0,0,0,0]},
+    {"token":"t",
+     "meta":["control","continued","continental"],
+     "heat":[0.27,0.17,0.052,0.44,1,0,0,0,0]},
+    {"token":"e",
+     "meta":["context","content","contested"],
+     "heat":[0.17,0.039,0.034,0.22,1,0.53,0,0,0]},
+    {"token":"x",
+     "meta":["context","contexts","contemporary"],
+     "heat":[0.17,0.0044,0.021,0.17,1,0.90,0.48,0,0]},
+    {"token":"t",
+     "meta":["context","contexts","contentious"],
+     "heat":[0.14,0.011,0.034,0.14,0.68,1,0.80,0.86,0]},
+    {"token":" ",
+     "meta":["of","and","the"],
+     "heat":[0.014,0.0063,0.0044,0.011,0.034,0.10,0.32,0.28,1]},
+    # ...
+],[
+    # LSTM data
+    # ...
+]]
+
+heatmap = TextualHeatmap(
+    width = 600,
+    show_meta = True,
+    facet_titles = ['GRU', 'LSTM']
+)
+# Set data and render plot, this can be called again to replace
+# the data.
+heatmap.set_data(data)
+# Focus on the token with the given index. Especially useful when
+# `interactive=False` is used in `TextualHeatmap`.
+heatmap.highlight(159)
+```
+
+![Shows saliency with predicted words at metadata](gifs/show_meta.gif)
+
+### Example of sequential-charecter model without metadata
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/general_example.ipynb)
+
+When `show_meta` is not `True`, the `meta` part of the `data` object has no effect.
+
+```python
+heatmap = TextualHeatmap(
+    facet_titles = ['LSTM', 'GRU'],
+    rotate_facet_titles = True
+)
+heatmap.set_data(data)
+heatmap.highlight(159)
+```
+
+![Shows saliency without metadata](gifs/no_meta_and_rotated.gif)
+
+### Example of non-sequential-word model
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AndreasMadsen/python-textualheatmap/blob/master/notebooks/bert_hardcoded_example.ipynb)
+
+`format = True` can be set in the `data` object to inducate tokens that are
+not directly used by the model. This is useful if word or sub-word tokenization
+is used.
+
+
+```python
+data = [[
+{'token': '[CLR]',
+ 'meta': ['', '', ''],
+ 'heat': [1, 0, 0, 0, 0, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'context',
+ 'meta': ['today', 'and', 'thus'],
+ 'heat': [0.13, 0.40, 0.23, 1.0, 0.56, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'the',
+ 'meta': ['##ual', 'the', '##ually'],
+ 'heat': [0.11, 1.0, 0.34, 0.58, 0.59, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'formal',
+ 'meta': ['formal', 'academic', 'systematic'],
+ 'heat': [0.13, 0.74, 0.26, 0.35, 1.0, ...]},
+{'token': ' ',
+ 'format': True},
+{'token': 'study',
+ 'meta': ['##ization', 'study', '##ity'],
+ 'heat': [0.09, 0.27, 0.19, 1.0, 0.26, ...]}
+]]
+
+heatmap = TextualHeatmap(facet_titles = ['BERT'], show_meta=True)
+heatmap.set_data(data)
+```
+
+![Shows saliency in a BERT model, using sub-word tokenization](gifs/sub_word_tokenized.gif)
+
+## Citation
+
+If you use this in a publication, please cite my [Distill publication](https://distill.pub/2019/memorization-in-rnns/) where I first demonstrated this visualization method.
+
+```bib
+@article{madsen2019visualizing,
+  author = {Madsen, Andreas},
+  title = {Visualizing memorization in RNNs},
+  journal = {Distill},
+  year = {2019},
+  note = {https://distill.pub/2019/memorization-in-rnns},
+  doi = {10.23915/distill.00016}
+}
+```
+
+## Sponsor
+
+Sponsored by <a href="https://www.nearform.com/research/">NearForm Research</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `textualheatmap-1.1.1/setup.py` & `textualheatmap-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-import os.path as path
-from setuptools import setup, find_packages
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-with open(path.join(path.abspath(path.dirname(__file__)), 'README.md')) as f:
-    long_description = f.read()
+[tool.setuptools]
+packages = ["textualheatmap"]
+include-package-data = true
 
-setup(name='textualheatmap',
-      version='1.1.1',
-      description='Create interactive textual heat maps for Jupiter notebooks',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      keywords='saliency heatmap text textual jupyter colab interactive',
-      url='https://github.com/AndreasMadsen/python-textualheatmap',
-      author='Andreas Madsen',
-      author_email='amwebdk@gmail.com',
-      license='MIT',
-      packages=find_packages(),
-      install_requires=[
-        'ipython'
-      ],
-      test_suite='nose.collector',
-      tests_require=[
-        'nose',
-        'jupyterlab',
-        'tensorflow'
-      ],
-      classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-      ],
-      include_package_data=True,
-      zip_safe=False)
+[project]
+name = "textualheatmap"
+description = "Create interactive textual heat maps for Jupiter notebooks"
+version = "1.2.0"
+authors = [
+    {name = "Andreas Madsen", email = "amwebdk@gmail.com"},
+]
+readme = {file = 'README.md', content-type='text/markdown'}
+license = {text = "MIT"}
+requires-python = ">=3.8"
+keywords = ["saliency", "heatmap", "text", "textual", "jupyter", "colab", "interactive"]
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'Intended Audience :: Education',
+    'Intended Audience :: Science/Research',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Topic :: Software Development :: Libraries',
+    'Topic :: Software Development :: Libraries :: Python Modules'
+]
+dependencies = [
+    "ipython"
+]
+
+[project.optional-dependencies]
+testing = [
+    "nose",
+    "jupyterlab",
+    "tensorflow"
+]
```

