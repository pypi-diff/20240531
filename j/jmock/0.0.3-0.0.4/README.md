# Comparing `tmp/jmock-0.0.3.tar.gz` & `tmp/jmock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmock-0.0.3.tar", last modified: Thu May 30 09:03:29 2024, max compression
+gzip compressed data, was "jmock-0.0.4.tar", last modified: Thu May 30 09:05:24 2024, max compression
```

## Comparing `jmock-0.0.3.tar` & `jmock-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:29.834535 jmock-0.0.3/
--rw-rw-rw-   0        0        0      342 2024-05-30 09:03:29.832289 jmock-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:29.806393 jmock-0.0.3/jmock/
--rw-rw-rw-   0        0        0       49 2024-05-30 09:03:16.000000 jmock-0.0.3/jmock/__init__.py
--rw-rw-rw-   0        0        0     3339 2024-05-30 08:31:09.000000 jmock-0.0.3/jmock/aiFunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:29.830707 jmock-0.0.3/jmock.egg-info/
--rw-rw-rw-   0        0        0      342 2024-05-30 09:03:29.000000 jmock-0.0.3/jmock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-05-30 09:03:29.000000 jmock-0.0.3/jmock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:03:29.000000 jmock-0.0.3/jmock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 09:03:29.000000 jmock-0.0.3/jmock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 09:03:29.000000 jmock-0.0.3/jmock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:03:29.834535 jmock-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-30 09:03:27.000000 jmock-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:05:24.037562 jmock-0.0.4/
+-rw-rw-rw-   0        0        0      342 2024-05-30 09:05:24.036130 jmock-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 09:05:24.011874 jmock-0.0.4/jmock/
+-rw-rw-rw-   0        0        0       49 2024-05-30 09:03:16.000000 jmock-0.0.4/jmock/__init__.py
+-rw-rw-rw-   0        0        0     3374 2024-05-30 09:05:12.000000 jmock-0.0.4/jmock/aiFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:05:24.034020 jmock-0.0.4/jmock.egg-info/
+-rw-rw-rw-   0        0        0      342 2024-05-30 09:05:23.000000 jmock-0.0.4/jmock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-30 09:05:23.000000 jmock-0.0.4/jmock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:05:23.000000 jmock-0.0.4/jmock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 09:05:23.000000 jmock-0.0.4/jmock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 09:05:23.000000 jmock-0.0.4/jmock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:05:24.037562 jmock-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-30 09:05:18.000000 jmock-0.0.4/setup.py
```

### Comparing `jmock-0.0.3/jmock/aiFunctions.py` & `jmock-0.0.4/jmock/aiFunctions.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 import os
 
 from dotenv import load_dotenv
 from langchain_google_genai import ChatGoogleGenerativeAI
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 
-def getResponseFromAI(prompt):
+def getResponseFromAI(prompt, GOOGLE_API_KEY, VARIATION):
     load_dotenv()
-    GOOGLE_API_KEY = os.environ.get('GOOGLE_API_KEY')
-    VARIATION = os.environ.get('VARIATION')
     llm = ChatGoogleGenerativeAI(model="gemini-pro", google_api_key=GOOGLE_API_KEY,temperature = VARIATION)
     tweet_prompt = PromptTemplate.from_template("{prompt}")
     tweet_chain = LLMChain(llm=llm, prompt=tweet_prompt, verbose=False)
     resp = tweet_chain.run(prompt=prompt)
     return resp
 
-def dataAsString(sample, count):
+def dataAsString(sample, count, GOOGLE_API_KEY, VARIATION):
     prompt_for_gpt = "By keeping fields like email, company, website, etc that define a person, as unique always and each generated object should be inspired from a different country also no two consecutive object should be inspired from same country, generate ",count," more objects similar to the sample object like ",sample," by understanding what each key in the object means and what value is expected for each key, act like the faker library. RETURN DATA AS ARRAY OF OBJECTS JSON FORMAT, ALSO CHECK HISTORY AND DONT GENERATE SIMILAR VALUES IN ATLEAST 10 CONSECUTIVE ITERATIONS"
     print('Gemini In Action!')
-    resp = getResponseFromAI(prompt_for_gpt)
+    resp = getResponseFromAI(prompt_for_gpt, GOOGLE_API_KEY, VARIATION)
     print('Gemini Responded!')
     return resp
 
-def dataAsJSON(sample, count):
+def dataAsJSON(sample, count, GOOGLE_API_KEY, VARIATION):
     prompt_for_gpt = "By keeping fields like email, company, website, etc that define a person, as unique always and each generated object should be inspired from a different country also no two consecutive object should be inspired from same country, generate ",count," more objects similar to the sample object like ",sample," by understanding what each key in the object means and what value is expected for each key, act like the faker library. RETURN DATA AS ARRAY OF OBJECTS JSON FORMAT, ALSO CHECK HISTORY AND DONT GENERATE SIMILAR VALUES IN ATLEAST 10 CONSECUTIVE ITERATIONS"
     print('Gemini In Action!')
-    resp = getResponseFromAI(prompt_for_gpt)
+    resp = getResponseFromAI(prompt_for_gpt, GOOGLE_API_KEY, VARIATION)
     json_response = json.dumps(resp)
     print('Gemini Responded!')
     return json_response
 
 # sample = {'name': 'Lucas', 'Id': '6FGU890128', 'email': 'lucas@microsoft.com', 'company': 'microsoft', 'website': 'microsoft.com', 'Status': True, 'address': {'city': 'bangalore', 'pincode/zipcode': 560010}}
 # sample =  "{\n    \"name\": \"Samuel\",\n    \"Id\": \"6FGU890300\",\n    \"email\": \"samuel@google.com\",\n    \"company\": \"google\",\n    \"website\": \"google.com\",\n    \"Status\": False,\n    \"address\": {\n      \"city\": \"mumbai\",\n      \"pincode/zipcode\": 560011\n    }\n  }"
 # count = 5
```

### Comparing `jmock-0.0.3/setup.py` & `jmock-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = "Joe's Synthetic Data Generator"
 LONG_DESCRIPTION = "AI Package to generate synthetic data using Google's gemini AI"
 REQUIRED_PACKAGES = [
   "langchain",
 "python-dotenv",
 "langchain_google_genai"
 ]
```

