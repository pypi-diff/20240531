# Comparing `tmp/PropertyExtract-1.0.tar.gz` & `tmp/propertyextract-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PropertyExtract-1.0.tar", last modified: Thu May 16 20:57:50 2024, max compression
+gzip compressed data, was "propertyextract-1.1.tar", last modified: Fri May 31 13:54:20 2024, max compression
```

## Comparing `PropertyExtract-1.0.tar` & `propertyextract-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-16 20:57:50.496201 PropertyExtract-1.0/
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    35149 2024-05-16 20:46:35.000000 PropertyExtract-1.0/LICENSE
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7510 2024-05-16 20:57:50.496201 PropertyExtract-1.0/PKG-INFO
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7150 2024-05-16 20:46:11.000000 PropertyExtract-1.0/README.md
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      661 2024-05-16 20:57:50.496201 PropertyExtract-1.0/setup.cfg
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      892 2024-05-16 19:39:30.000000 PropertyExtract-1.0/setup.py
-drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-16 20:57:50.496201 PropertyExtract-1.0/src/
-drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-16 20:57:50.496201 PropertyExtract-1.0/src/PropertyExtract.egg-info/
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7510 2024-05-16 20:57:50.000000 PropertyExtract-1.0/src/PropertyExtract.egg-info/PKG-INFO
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      321 2024-05-16 20:57:50.000000 PropertyExtract-1.0/src/PropertyExtract.egg-info/SOURCES.txt
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)        1 2024-05-16 20:57:50.000000 PropertyExtract-1.0/src/PropertyExtract.egg-info/dependency_links.txt
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      118 2024-05-16 20:57:50.000000 PropertyExtract-1.0/src/PropertyExtract.egg-info/requires.txt
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)       34 2024-05-16 20:57:50.000000 PropertyExtract-1.0/src/PropertyExtract.egg-info/top_level.txt
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    37937 2024-05-16 19:44:26.000000 PropertyExtract-1.0/src/propertyextractor.py
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     4050 2024-05-16 19:39:42.000000 PropertyExtract-1.0/src/propextract
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7122 2024-05-16 19:39:42.000000 PropertyExtract-1.0/src/readin.py
--rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    11223 2024-05-16 20:50:34.000000 PropertyExtract-1.0/src/writeout.py
+drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-31 13:54:20.547603 propertyextract-1.1/
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    35149 2024-05-16 20:46:35.000000 propertyextract-1.1/LICENSE
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7842 2024-05-31 13:54:20.547603 propertyextract-1.1/PKG-INFO
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7150 2024-05-16 20:46:11.000000 propertyextract-1.1/README.md
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      669 2024-05-31 13:54:20.547603 propertyextract-1.1/setup.cfg
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      892 2024-05-16 19:39:30.000000 propertyextract-1.1/setup.py
+drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-31 13:54:20.546604 propertyextract-1.1/src/
+drwxr-xr-x   0 chineduekuma  (1000) chineduekuma  (1000)        0 2024-05-31 13:54:20.547603 propertyextract-1.1/src/PropertyExtract.egg-info/
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7842 2024-05-31 13:54:20.000000 propertyextract-1.1/src/PropertyExtract.egg-info/PKG-INFO
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      325 2024-05-31 13:54:20.000000 propertyextract-1.1/src/PropertyExtract.egg-info/SOURCES.txt
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)        1 2024-05-31 13:54:20.000000 propertyextract-1.1/src/PropertyExtract.egg-info/dependency_links.txt
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)      118 2024-05-31 13:54:20.000000 propertyextract-1.1/src/PropertyExtract.egg-info/requires.txt
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)       34 2024-05-31 13:54:20.000000 propertyextract-1.1/src/PropertyExtract.egg-info/top_level.txt
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     4036 2024-05-19 14:42:18.000000 propertyextract-1.1/src/propertyextract
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    38072 2024-05-31 13:50:19.000000 propertyextract-1.1/src/propertyextractor.py
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)     7122 2024-05-16 19:39:42.000000 propertyextract-1.1/src/readin.py
+-rw-r--r--   0 chineduekuma  (1000) chineduekuma  (1000)    11223 2024-05-16 20:50:34.000000 propertyextract-1.1/src/writeout.py
```

### Comparing `PropertyExtract-1.0/LICENSE` & `propertyextract-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PropertyExtract-1.0/PKG-INFO` & `propertyextract-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: PropertyExtract
-Version: 1.0
-Summary: "PropertyExtract -- LLM-based model to extract material property from unstructured dataset",
-Home-page: https://sourceforge.net/projects/propextract/
-Author: Chinedu Ekuma
-Author-email: cekuma1@gmail.com
-License: GNU GPL version 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PropertyExtractor: An Open-Source Conversational LLM-Based Tool
 
 ## Introduction
 
 The advent of natural language processing and large language models (LLMs) has revolutionized the extraction of data from unstructured scholarly papers. However, ensuring data trustworthiness remains a significant challenge. **PropertyExtractor** is an open-source tool that leverages advanced conversational LLMs like **Google Gemini Pro** and **OpenAI GPT-4**, blends zero-shot with few-shot in-context learning, and employs engineered prompts for the dynamic refinement of structured information hierarchies to enable autonomous, efficient, scalable, and accurate identification, extraction, and verification of material property data to generate material property database. 
 
 ## Features
```

### Comparing `PropertyExtract-1.0/README.md` & `propertyextract-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: PropertyExtract
+Version: 1.1
+Summary: "PropertyExtract -- LLM-based model to extract material property from unstructured dataset",
+Home-page: https://sourceforge.net/projects/propertyextract/
+Author: Chinedu Ekuma
+Author-email: cekuma1@gmail.com
+License: GNU GPL version 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: spglib
+Requires-Dist: mendeleev
+Requires-Dist: openai
+Requires-Dist: nltk
+Requires-Dist: spacy
+Requires-Dist: urllib3
+Requires-Dist: textblob
+Requires-Dist: google-generativeai
+Requires-Dist: backoff
+Requires-Dist: chardet
+
 # PropertyExtractor: An Open-Source Conversational LLM-Based Tool
 
 ## Introduction
 
 The advent of natural language processing and large language models (LLMs) has revolutionized the extraction of data from unstructured scholarly papers. However, ensuring data trustworthiness remains a significant challenge. **PropertyExtractor** is an open-source tool that leverages advanced conversational LLMs like **Google Gemini Pro** and **OpenAI GPT-4**, blends zero-shot with few-shot in-context learning, and employs engineered prompts for the dynamic refinement of structured information hierarchies to enable autonomous, efficient, scalable, and accurate identification, extraction, and verification of material property data to generate material property database. 
 
 ## Features
```

### Comparing `PropertyExtract-1.0/setup.cfg` & `propertyextract-1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = PropertyExtract
-version = 1.0
+version = 1.1
 description = "PropertyExtract -- LLM-based model to extract material property from unstructured dataset",
 author = Chinedu Ekuma
 author_email = cekuma1@gmail.com
-url = https://sourceforge.net/projects/propextract/
+url = https://sourceforge.net/projects/propertyextract/
 license = GNU GPL version 3
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= src
 scripts = 
-	src/propextract
+	src/propertyextract
 install_requires = 
 	numpy
 	scipy
 	matplotlib
 	pandas
 	spglib
 	mendeleev
```

### Comparing `PropertyExtract-1.0/setup.py` & `propertyextract-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `PropertyExtract-1.0/src/PropertyExtract.egg-info/PKG-INFO` & `propertyextract-1.1/src/PropertyExtract.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 Metadata-Version: 2.1
 Name: PropertyExtract
-Version: 1.0
+Version: 1.1
 Summary: "PropertyExtract -- LLM-based model to extract material property from unstructured dataset",
-Home-page: https://sourceforge.net/projects/propextract/
+Home-page: https://sourceforge.net/projects/propertyextract/
 Author: Chinedu Ekuma
 Author-email: cekuma1@gmail.com
 License: GNU GPL version 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: spglib
+Requires-Dist: mendeleev
+Requires-Dist: openai
+Requires-Dist: nltk
+Requires-Dist: spacy
+Requires-Dist: urllib3
+Requires-Dist: textblob
+Requires-Dist: google-generativeai
+Requires-Dist: backoff
+Requires-Dist: chardet
 
 # PropertyExtractor: An Open-Source Conversational LLM-Based Tool
 
 ## Introduction
 
 The advent of natural language processing and large language models (LLMs) has revolutionized the extraction of data from unstructured scholarly papers. However, ensuring data trustworthiness remains a significant challenge. **PropertyExtractor** is an open-source tool that leverages advanced conversational LLMs like **Google Gemini Pro** and **OpenAI GPT-4**, blends zero-shot with few-shot in-context learning, and employs engineered prompts for the dynamic refinement of structured information hierarchies to enable autonomous, efficient, scalable, and accurate identification, extraction, and verification of material property data to generate material property database.
```

### Comparing `PropertyExtract-1.0/src/propertyextractor.py` & `propertyextract-1.1/src/propertyextractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -766,18 +766,23 @@
 
         try:
             if file_extension == '.csv':
                 examples = self.read_file_with_detected_encoding(input_csv) #pd.read_csv(input_csv) #
             elif file_extension in ['.xls', '.xlsx']:
                 examples = pd.read_excel(input_csv)
             else:
-                logging.error("Unsupported file format")
+                message = "Unsupported file format"
+                logging.error(message)
+                print(message)
                 return
         except Exception as e:
-            logging.error(f"Error reading the file: {e}")
+            message = f"Error reading the file: {e}"
+            print(message)
+            logging.error(message)
+            
             return
 
 
         examples.dropna(subset=[text_column], how='all', inplace=True)
 
         file_exists = os.path.isfile(output_csv)
```

### Comparing `PropertyExtract-1.0/src/propextract` & `propertyextract-1.1/src/propertyextract`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     print("")
 
     end_time = time.time()  # Capture the end time
     elapsed_time = end_time - start_time  # Calculate the elapsed time
 
     print(f"Calculation Completed Successfully Using {elapsed_time:.3f}s\nGOOD LUCK!")
-    logging.info("Calculation Completed Successfully Using {elapsed_time:.3f}s\nGOOD LUCK!")
+    logging.info(f"Calculation Completed Successfully Using {elapsed_time} s")
     logging.info("Analysis results successfully saved.")
     print("")
 
     with open("calctime.log", 'w') as f:
         f.write(f"Calculation done in {elapsed_time:.2f} s\n")
```

### Comparing `PropertyExtract-1.0/src/readin.py` & `propertyextract-1.1/src/readin.py`

 * *Files identical despite different names*

### Comparing `PropertyExtract-1.0/src/writeout.py` & `propertyextract-1.1/src/writeout.py`

 * *Files identical despite different names*

