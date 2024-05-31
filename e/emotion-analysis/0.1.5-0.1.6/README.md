# Comparing `tmp/emotion_analysis-0.1.5.tar.gz` & `tmp/emotion_analysis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_analysis-0.1.5.tar", last modified: Wed May 29 01:41:48 2024, max compression
+gzip compressed data, was "emotion_analysis-0.1.6.tar", last modified: Fri May 31 14:43:22 2024, max compression
```

## Comparing `emotion_analysis-0.1.5.tar` & `emotion_analysis-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-29 01:41:48.431806 emotion_analysis-0.1.5/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17782 2024-05-29 01:41:48.427806 emotion_analysis-0.1.5/PKG-INFO
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    16961 2024-05-28 07:25:14.000000 emotion_analysis-0.1.5/README.md
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-29 01:41:48.427806 emotion_analysis-0.1.5/emotion_analysis/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.5/emotion_analysis/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2184 2024-05-28 03:08:43.000000 emotion_analysis-0.1.5/emotion_analysis/bert_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    13042 2024-05-28 08:06:55.000000 emotion_analysis-0.1.5/emotion_analysis/data_preprocessing.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.5/emotion_analysis/frnn.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2145 2024-05-28 03:09:56.000000 emotion_analysis-0.1.5/emotion_analysis/roberta_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2293 2024-05-28 06:30:12.000000 emotion_analysis-0.1.5/emotion_analysis/tweets_embedding.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-29 01:41:48.427806 emotion_analysis-0.1.5/emotion_analysis.egg-info/
--rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17782 2024-05-29 01:41:48.000000 emotion_analysis-0.1.5/emotion_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      470 2024-05-29 01:41:48.000000 emotion_analysis-0.1.5/emotion_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-29 01:41:48.000000 emotion_analysis-0.1.5/emotion_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-29 01:41:48.000000 emotion_analysis-0.1.5/emotion_analysis.egg-info/requires.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-29 01:41:48.000000 emotion_analysis-0.1.5/emotion_analysis.egg-info/top_level.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-29 01:41:48.431806 emotion_analysis-0.1.5/setup.cfg
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1310 2024-05-29 01:41:42.000000 emotion_analysis-0.1.5/setup.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-29 01:41:48.427806 emotion_analysis-0.1.5/tests/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.5/tests/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14877 2024-05-28 08:45:15.000000 emotion_analysis-0.1.5/tests/test.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17794 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    16973 2024-05-31 14:42:06.000000 emotion_analysis-0.1.6/README.md
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/emotion_analysis/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.6/emotion_analysis/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2184 2024-05-28 03:08:43.000000 emotion_analysis-0.1.6/emotion_analysis/bert_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    13042 2024-05-28 08:06:55.000000 emotion_analysis-0.1.6/emotion_analysis/data_preprocessing.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.6/emotion_analysis/frnn.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2145 2024-05-28 03:09:56.000000 emotion_analysis-0.1.6/emotion_analysis/roberta_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2293 2024-05-28 06:30:12.000000 emotion_analysis-0.1.6/emotion_analysis/tweets_embedding.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/emotion_analysis.egg-info/
+-rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17794 2024-05-31 14:43:21.000000 emotion_analysis-0.1.6/emotion_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      504 2024-05-31 14:43:21.000000 emotion_analysis-0.1.6/emotion_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-31 14:43:21.000000 emotion_analysis-0.1.6/emotion_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-31 14:43:21.000000 emotion_analysis-0.1.6/emotion_analysis.egg-info/requires.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-31 14:43:21.000000 emotion_analysis-0.1.6/emotion_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/setup.cfg
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1310 2024-05-31 14:43:18.000000 emotion_analysis-0.1.6/setup.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-31 14:43:22.041624 emotion_analysis-0.1.6/tests/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.6/tests/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1606 2024-05-30 10:55:11.000000 emotion_analysis-0.1.6/tests/new_test.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    11813 2024-05-31 14:18:14.000000 emotion_analysis-0.1.6/tests/test.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1984 2024-05-31 14:09:34.000000 emotion_analysis-0.1.6/tests/test_3.py
```

### Comparing `emotion_analysis-0.1.5/PKG-INFO` & `emotion_analysis-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_analysis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for emotion detection using transformers-based models.
 Home-page: https://github.com/ahsantariq7/emotion_analysis
 Author: Ahsan Tariq
 Author-email: ahsantariq0724@email.com
 License: MIT
 Keywords: emotion analysis transformers machine learning,engr_ahsan_tariq_0724,bert_vector,roberta_vector,nlp,text emotion analysis,emotion analysis
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 
 This package provides tools for emotion detection using transformer-based models. It includes functionalities for preprocessing data, generating word clouds, visualizing statistics, and evaluating model performance.
 
 ## Installation
 
 To install the package, you can use pip:
 
-`pip install isgc`
+`pip install emotion-analysis`
 
 ## Usage
 
 ### Data Preprocessing
 
 First, you need to preprocess your datasets. You can use the `upload_datasets` function to load your data. Here is the full testing code. For example:
```

### Comparing `emotion_analysis-0.1.5/README.md` & `emotion_analysis-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package provides tools for emotion detection using transformer-based models. It includes functionalities for preprocessing data, generating word clouds, visualizing statistics, and evaluating model performance.
 
 ## Installation
 
 To install the package, you can use pip:
 
-`pip install isgc`
+`pip install emotion-analysis`
 
 ## Usage
 
 ### Data Preprocessing
 
 First, you need to preprocess your datasets. You can use the `upload_datasets` function to load your data. Here is the full testing code. For example:
```

### Comparing `emotion_analysis-0.1.5/emotion_analysis/bert_pcc_score_emotions.py` & `emotion_analysis-0.1.6/emotion_analysis/bert_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.5/emotion_analysis/data_preprocessing.py` & `emotion_analysis-0.1.6/emotion_analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.5/emotion_analysis/frnn.py` & `emotion_analysis-0.1.6/emotion_analysis/frnn.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.5/emotion_analysis/roberta_pcc_score_emotions.py` & `emotion_analysis-0.1.6/emotion_analysis/roberta_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.5/emotion_analysis/tweets_embedding.py` & `emotion_analysis-0.1.6/emotion_analysis/tweets_embedding.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.5/emotion_analysis.egg-info/PKG-INFO` & `emotion_analysis-0.1.6/emotion_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion-analysis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for emotion detection using transformers-based models.
 Home-page: https://github.com/ahsantariq7/emotion_analysis
 Author: Ahsan Tariq
 Author-email: ahsantariq0724@email.com
 License: MIT
 Keywords: emotion analysis transformers machine learning,engr_ahsan_tariq_0724,bert_vector,roberta_vector,nlp,text emotion analysis,emotion analysis
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 
 This package provides tools for emotion detection using transformer-based models. It includes functionalities for preprocessing data, generating word clouds, visualizing statistics, and evaluating model performance.
 
 ## Installation
 
 To install the package, you can use pip:
 
-`pip install isgc`
+`pip install emotion-analysis`
 
 ## Usage
 
 ### Data Preprocessing
 
 First, you need to preprocess your datasets. You can use the `upload_datasets` function to load your data. Here is the full testing code. For example:
```

### Comparing `emotion_analysis-0.1.5/setup.py` & `emotion_analysis-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Directory containing the README file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="emotion_analysis",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "beautifulsoup4",
         "emoji",
         "nltk",
         "wordcloud",
```

### Comparing `emotion_analysis-0.1.5/tests/test.py` & `emotion_analysis-0.1.6/tests/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,112 +10,65 @@
 # Add the parent directory to sys.path
 sys.path.append(parent_dir)
 
 from emotion_analysis.data_preprocessing import *
 
 
 anger_train, anger_dev, anger_data, anger_test = upload_datasets(
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-anger-dev.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-anger-train.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-anger-test.txt",
+    "/home/ahsan-pmylsp/Desktop/Text Emotion Analysis Thesis Paper/emotion_analysis/dataset/EI-oc-En-anger-train.txt",
+    "dataset/2018-EI-oc-En-anger-dev.txt",
+    "dataset/2018-EI-oc-En-anger-test.txt",
 )
 
 fear_train, fear_dev, fear_data, fear_test = upload_datasets(
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-fear-train.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-fear-dev.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-fear-test.txt",
+    "dataset/EI-oc-En-fear-train.txt",
+    "dataset/2018-EI-oc-En-fear-dev.txt",
+    "dataset/2018-EI-oc-En-fear-test.txt",
 )
 
 joy_train, joy_dev, joy_data, joy_test = upload_datasets(
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-joy-train.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-joy-dev.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-joy-test.txt",
+    "dataset/EI-oc-En-joy-train.txt",
+    "dataset/2018-EI-oc-En-joy-dev.txt",
+    "dataset/2018-EI-oc-En-joy-test.txt",
 )
 
 sad_train, sad_dev, sad_data, sad_test = upload_datasets(
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-sadness-train.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-sadness-dev.txt",
-    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-sadness-test.txt",
+    "dataset/EI-oc-En-sadness-train.txt",
+    "dataset/2018-EI-oc-En-sadness-dev.txt",
+    "dataset/2018-EI-oc-En-sadness-test.txt",
 )
 
-
-generate_wordclouds(anger_train, anger_dev, anger_data, anger_test, "Anger")
-plot_statistics(anger_train, anger_dev, anger_data, anger_test, "Anger")
-plot_additional_statistics(anger_train, anger_dev, anger_test, "Anger")
-plot_top_n_words(anger_train, n=20, title="Top 20 Frequent Words in Anger Train Data")
-plot_ngrams_frequency(
-    anger_train, n=2, top_n=10, title="Bigram Frequency in Anger Train Data"
-)
-plot_ngrams_frequency(
-    anger_train, n=3, top_n=10, title="Trigram Frequency in Anger Train Data"
-)
-
-generate_wordclouds(joy_train, joy_dev, joy_data, joy_test, "Joy")
-plot_statistics(joy_train, joy_dev, joy_data, joy_test, "Joy")
-plot_additional_statistics(joy_train, joy_dev, joy_test, "Joy")
-plot_top_n_words(joy_train, n=20, title="Top 20 Frequent Words in Joy Train Data")
-plot_ngrams_frequency(
-    joy_train, n=2, top_n=10, title="Bigram Frequency in Joy Train Data"
-)
-plot_ngrams_frequency(
-    joy_train, n=3, top_n=10, title="Trigram Frequency in Joy Train Data"
-)
-
-generate_wordclouds(sad_train, sad_dev, sad_data, sad_test, "Sadness")
-plot_statistics(sad_train, sad_dev, sad_data, sad_test, "Sadness")
-plot_additional_statistics(sad_train, sad_dev, sad_test, "Sadness")
-plot_top_n_words(sad_train, n=20, title="Top 20 Frequent Words in Sadness Train Data")
-plot_ngrams_frequency(
-    sad_train, n=2, top_n=10, title="Bigram Frequency in Sadness Train Data"
-)
-plot_ngrams_frequency(
-    sad_train, n=3, top_n=10, title="Trigram Frequency in Sadness Train Data"
-)
-
-generate_wordclouds(fear_train, fear_dev, fear_data, fear_test, "Fear")
-plot_statistics(fear_train, fear_dev, fear_data, fear_test, "Fear")
-plot_additional_statistics(fear_train, fear_dev, fear_test, "Fear")
-plot_top_n_words(fear_train, n=20, title="Top 20 Frequent Words in Fear Train Data")
-plot_ngrams_frequency(
-    fear_train, n=2, top_n=10, title="Bigram Frequency in Fear Train Data"
-)
-plot_ngrams_frequency(
-    fear_train, n=3, top_n=10, title="Trigram Frequency in Fear Train Data"
-)
-
-
-plot_dataset_statistics([anger_data, joy_data, sad_data, fear_data])
 from emotion_analysis.tweets_embedding import *
 from emotion_analysis.frnn import *
 from emotion_analysis.bert_pcc_score_emotions import *
 from emotion_analysis.roberta_pcc_score_emotions import *
 
 anger_train, anger_dev, anger_data, anger_test = (
-    anger_train[:5],
-    anger_dev[:5],
-    anger_data[:5],
-    anger_test[:5],
+    anger_train[:10],
+    anger_dev[:10],
+    anger_data[:10],
+    anger_test[:10],
 )
 fear_train, fear_dev, fear_data, fear_test = (
-    fear_train[:5],
-    fear_dev[:5],
-    fear_data[:5],
-    fear_test[:5],
+    fear_train[:10],
+    fear_dev[:10],
+    fear_data[:10],
+    fear_test[:10],
 )
 joy_train, joy_dev, joy_data, joy_test = (
-    joy_train[:5],
-    joy_dev[:5],
-    joy_data[:5],
-    joy_test[:5],
+    joy_train[:10],
+    joy_dev[:10],
+    joy_data[:10],
+    joy_test[:10],
 )
 sad_train, sad_dev, sad_data, sad_test = (
-    sad_train[:5],
-    sad_dev[:5],
-    sad_data[:5],
-    sad_test[:5],
+    sad_train[:10],
+    sad_dev[:10],
+    sad_data[:10],
+    sad_test[:10],
 )
 
 anger_data["Vector_bert"] = anger_data["Tweet"].apply(get_vector_bert)
 anger_test["Vector_bert"] = anger_test["Tweet"].apply(get_vector_bert)
 
 joy_data["Vector_bert"] = joy_data["Tweet"].apply(get_vector_bert)
 joy_test["Vector_bert"] = joy_test["Tweet"].apply(get_vector_bert)
```

