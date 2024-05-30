# Comparing `tmp/promptic-0.6.1.tar.gz` & `tmp/promptic-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.7.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.6.1.tar` & `promptic-0.7.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      487 2024-05-28 18:25:36.700697 promptic-0.6.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-28 18:25:36.700697 promptic-0.6.1/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-28 18:25:36.704697 promptic-0.6.1/LICENSE
--rw-r--r--   0        0        0     3507 2024-05-28 18:25:36.704697 promptic-0.6.1/README.md
--rw-r--r--   0        0        0     4325 2024-05-28 18:25:36.704697 promptic-0.6.1/promptic.py
--rw-r--r--   0        0        0      527 2024-05-28 18:25:36.704697 promptic-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 promptic-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-27 22:34:43.554619 promptic-0.7.0a1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 19:31:43.907511 promptic-0.7.0a1/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     3507 2024-05-27 23:39:52.432096 promptic-0.7.0a1/README.md
+-rw-r--r--   0        0        0     4344 2024-05-30 22:04:55.738073 promptic-0.7.0a1/promptic.py
+-rw-r--r--   0        0        0      529 2024-05-30 22:05:34.280788 promptic-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 promptic-0.7.0a1/PKG-INFO
```

### Comparing `promptic-0.6.1/.gitignore` & `promptic-0.7.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.6.1/LICENSE` & `promptic-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.6.1/README.md` & `promptic-0.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.6.1/promptic.py` & `promptic-0.7.0a1/promptic.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 logger = logging.getLogger("promptic")
 
 if os.getenv("PROMPTIC_DEBUG"):
     logger.setLevel(logging.DEBUG)
     logger.addHandler(logging.StreamHandler())
 
+regex = re.compile(r"```json(.*?)```", re.DOTALL)
+
 
 def promptic(fn=None, model="gpt-3.5-turbo", system: str = None, **litellm_kwargs):
     """
     Decorator to call the LLM with a prompt generated from the function's docstring and arguments.
 
     Args:
         fn: The function to decorate.
@@ -89,15 +91,15 @@
                 # Get the generated text from the LLM response
                 generated_text = response["choices"][0]["message"]["content"]
 
                 logger.debug(f"{generated_text = }")
 
                 if return_type and issubclass(return_type, BaseModel):
                     # Extract the JSON result using regex
-                    match = re.search(r"```json\n(.*?)\n```", generated_text, re.DOTALL)
+                    match = regex.search(generated_text)
                     if match:
                         json_result = match.group(1)
                         # Parse the JSON and return an instance of the Pydantic model
                         return return_type.model_validate_json(json_result)
                     else:
                         raise ValueError(
                             "Failed to extract JSON result from the generated text."
```

### Comparing `promptic-0.6.1/pyproject.toml` & `promptic-0.7.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.6.1"
+version = "0.7.0a1"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.6.1/PKG-INFO` & `promptic-0.7.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.6.1
+Version: 0.7.0a1
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

