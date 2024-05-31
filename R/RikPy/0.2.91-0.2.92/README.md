# Comparing `tmp/RikPy-0.2.91.tar.gz` & `tmp/RikPy-0.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.91.tar", last modified: Thu May 16 22:12:25 2024, max compression
+gzip compressed data, was "RikPy-0.2.92.tar", last modified: Fri May 31 15:29:27 2024, max compression
```

## Comparing `RikPy-0.2.91.tar` & `RikPy-0.2.92.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:12:25.209319 RikPy-0.2.91/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.91/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 22:12:25.207321 RikPy-0.2.91/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 22:12:25.190508 RikPy-0.2.91/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.91/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5429 2024-05-16 21:13:28.000000 RikPy-0.2.91/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.91/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.91/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.91/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.91/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.91/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     8993 2024-05-16 22:11:25.000000 RikPy-0.2.91/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.91/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.91/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:12:25.199767 RikPy-0.2.91/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 22:12:25.000000 RikPy-0.2.91/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 22:12:25.000000 RikPy-0.2.91/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:12:25.000000 RikPy-0.2.91/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 22:12:25.000000 RikPy-0.2.91/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.91/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.91/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 22:12:25.212224 RikPy-0.2.91/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:27.033016 RikPy-0.2.92/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.92/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-31 15:29:27.028028 RikPy-0.2.92/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:27.005096 RikPy-0.2.92/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.92/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5429 2024-05-16 21:13:28.000000 RikPy-0.2.92/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.92/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.92/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.92/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.92/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4200 2024-05-31 15:28:17.000000 RikPy-0.2.92/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     8993 2024-05-16 22:11:25.000000 RikPy-0.2.92/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.92/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.92/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:27.025036 RikPy-0.2.92/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-31 15:29:26.000000 RikPy-0.2.92/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-31 15:29:26.000000 RikPy-0.2.92/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:29:26.000000 RikPy-0.2.92/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-31 15:29:26.000000 RikPy-0.2.92/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.92/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.92/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-31 15:29:27.039998 RikPy-0.2.92/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.92/setup.py
```

### Comparing `RikPy-0.2.91/RikPy/commonfunctions.py` & `RikPy-0.2.92/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/RikPy/commongoogle.py` & `RikPy-0.2.92/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/RikPy/commonheroku.py` & `RikPy-0.2.92/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/RikPy/commonleonardo.py` & `RikPy-0.2.92/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/RikPy/commonopenai.py` & `RikPy-0.2.92/RikPy/commonopenai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import openai
 from .customresponse import CustomResponse
 import requests
 import json
 
-def OpenAI_generate_response(prompt, openai_key=""):
+def OpenAI_generate_response(prompt, openai_key="", model="gpt-3.5-turbo"):
     
     try:
         # Executes the prompt and returns the response without parsing
         print ("Warming Up the Wisdom Workshop!")
         openai.api_key = openai_key
 
         print ("Assembling Words of Wisdom!")
         details_response = openai.chat.completions.create(
-            model="gpt-3.5-turbo",
+            model=model,
             messages=[
                 {
                     "role": "user",
                     "content": prompt,  # Your prompt goes here
                 }
             ]
         )
@@ -31,27 +31,27 @@
     except openai.BadRequestError as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
     except openai.APIError as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
     except Exception as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
         
-def OpenAI_generate_image(image_prompt, number_images=1, quality="standard", size="1024x1024", openai_key=""):
+def OpenAI_generate_image(image_prompt, number_images=1, quality="standard", size="1024x1024", openai_key="", model="dall-e-3"):
     
     try:
         # Executes the prompt and returns the response without parsing
         
         print ("Sparking the Synapses of Silicon!")
         openai.api_key = openai_key
 
         print("Summoning Pixels from the Digital Depths!")
         print(image_prompt)
         
         image_response = openai.images.generate(
-            model="dall-e-3",
+            model=model,
             prompt=image_prompt,
             n=number_images,
             quality=quality,
             size=size
         )
         
         #return image_response
@@ -65,26 +65,26 @@
     except openai.BadRequestError as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
     except openai.APIError as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
     except Exception as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
     
-def OpenAI_generate_image_request(image_prompt, number_images=1, quality="standard", size="1024x1024", openai_key=""):
+def OpenAI_generate_image_request(image_prompt, number_images=1, quality="standard", size="1024x1024", openai_key="", model="dall-e-3"):
     try:
         print("Sparking the Synapses of Silicon!")
         url = "https://api.openai.com/v1/images/generations"
 
         headers = {
             "Authorization": f"Bearer {openai_key}",
             "Content-Type": "application/json"
         }
 
         payload = {
-            "model": "dall-e-3",
+            "model": model,
             "prompt": image_prompt,
             "n": number_images,
             "quality": quality,
             "size": size
         }
 
         print("Summoning Pixels from the Digital Depths!")
```

### Comparing `RikPy-0.2.91/RikPy/commons3.py` & `RikPy-0.2.92/RikPy/commons3.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/RikPy/commonshopify.py` & `RikPy-0.2.92/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.91/logfile.txt` & `RikPy-0.2.92/logfile.txt`

 * *Files identical despite different names*

