# Comparing `tmp/aibridge_test-0.3.8.tar.gz` & `tmp/aibridge_test-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.3.8.tar", last modified: Mon May 20 06:59:31 2024, max compression
+gzip compressed data, was "aibridge_test-0.3.9.tar", last modified: Fri May 31 06:00:26 2024, max compression
```

## Comparing `aibridge_test-0.3.8.tar` & `aibridge_test-0.3.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:31.345330 aibridge_test-0.3.8/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.084317 aibridge_test-0.3.8/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.8/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.188747 aibridge_test-0.3.8/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9364 2024-04-19 04:13:29.000000 aibridge_test-0.3.8/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13992 2024-05-08 12:15:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12317 2024-04-19 04:14:01.000000 aibridge_test-0.3.8/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14692 2024-05-08 11:27:54.000000 aibridge_test-0.3.8/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.8/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11902 2024-04-19 04:13:01.000000 aibridge_test-0.3.8/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.8/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9249 2024-04-19 04:14:42.000000 aibridge_test-0.3.8/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.8/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.222627 aibridge_test-0.3.8/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.8/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.8/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.342381 aibridge_test-0.3.8/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.424531 aibridge_test-0.3.8/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.8/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.702124 aibridge_test-0.3.8/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.8/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.8/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.808081 aibridge_test-0.3.8/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:30.998543 aibridge_test-0.3.8/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.8/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.8/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-05-20 06:59:31.320396 aibridge_test-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 06:59:31.316159 aibridge_test-0.3.8/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-05-20 06:59:29.000000 aibridge_test-0.3.8/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-05-20 06:59:29.000000 aibridge_test-0.3.8/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:59:29.000000 aibridge_test-0.3.8/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-05-20 06:59:29.000000 aibridge_test-0.3.8/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 06:59:29.000000 aibridge_test-0.3.8/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 06:59:31.345854 aibridge_test-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-05-20 06:58:01.000000 aibridge_test-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:26.077281 aibridge_test-0.3.9/
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.715284 aibridge_test-0.3.9/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.9/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.833281 aibridge_test-0.3.9/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9357 2024-05-31 04:24:01.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    14000 2024-05-31 04:24:49.000000 aibridge_test-0.3.9/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12308 2024-05-31 04:25:25.000000 aibridge_test-0.3.9/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14683 2024-05-31 04:26:27.000000 aibridge_test-0.3.9/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7569 2024-05-31 04:28:50.000000 aibridge_test-0.3.9/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11901 2024-05-31 04:29:31.000000 aibridge_test-0.3.9/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2951 2024-05-31 04:30:00.000000 aibridge_test-0.3.9/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9267 2024-05-31 04:31:25.000000 aibridge_test-0.3.9/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.9/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10264 2024-05-31 04:32:52.000000 aibridge_test-0.3.9/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.843284 aibridge_test-0.3.9/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.9/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.9/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.891283 aibridge_test-0.3.9/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.911282 aibridge_test-0.3.9/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     4039 2024-05-31 05:38:04.000000 aibridge_test-0.3.9/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.936280 aibridge_test-0.3.9/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.9/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.9/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.956283 aibridge_test-0.3.9/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-05-31 05:04:54.000000 aibridge_test-0.3.9/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-05-31 05:04:55.000000 aibridge_test-0.3.9/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-05-31 05:04:54.000000 aibridge_test-0.3.9/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.982281 aibridge_test-0.3.9/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.9/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.9/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-05-31 06:00:26.072285 aibridge_test-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 06:00:26.067280 aibridge_test-0.3.9/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 06:00:26.080294 aibridge_test-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-05-31 05:59:13.000000 aibridge_test-0.3.9/setup.py
```

### Comparing `aibridge_test-0.3.8/AIBridge/__init__.py` & `aibridge_test-0.3.9/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.3.9/AIBridge/ai_services/ai21labs_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import uuid
-from AIBridge.exceptions import Ai21Exception, AIBridgeException
+from AIBridge.exceptions import Ai21Exception, AIBridgeException, ValidationException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
 import ai21
 from AIBridge.output_validation.convertors import FromJson, IntoJson
@@ -55,20 +55,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -110,15 +110,15 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise Ai21Exception(f"Error in generating AI data {e}")
+            raise Ai21Exception(e)
 
     @classmethod
     def get_prompt_context(self, context):
         context_string = ""
         if context:
             for _context in context:
                 if _context["role"] not in ["user", "system", "assistant"]:
@@ -180,15 +180,15 @@
                         _formatter = output_format[index]
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise Ai21Exception(
+                            raise ValidationException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -218,8 +218,8 @@
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "ai21_api",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise Ai21Exception(f"{e}")
+            raise Ai21Exception(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.3.9/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.3.9/AIBridge/ai_services/anthropic_ai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 import time
 import uuid
-from AIBridge.exceptions import AnthropicsException, AIBridgeException
+from AIBridge.exceptions import (
+    AnthropicsException,
+    AIBridgeException,
+    ValidationException,
+)
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import (
     get_function_from_json,
     parse_fromat,
@@ -61,20 +65,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -118,15 +122,15 @@
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
                 stream=stream,
             )
         except AIBridgeException as e:
-            raise AnthropicsException(f"Error in generating AI data {e}")
+            raise AnthropicsException(e)
 
     @classmethod
     def execute_text_prompt(
         self, api_key, model, messages, n, max_tokens=3500, temperature=0.5
     ):
         client = Anthropic(api_key=api_key)
         return client.messages.create(
@@ -294,15 +298,15 @@
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise AnthropicsException(
+                            raise ValidationException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -332,8 +336,8 @@
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "anthropic",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise AnthropicsException(f"{e}")
+            raise AnthropicsException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.3.9/AIBridge/ai_services/cohere_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cohere
 import time
 import uuid
-from AIBridge.exceptions import CohereException, AIBridgeException
+from AIBridge.exceptions import CohereException, AIBridgeException, ValidationException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 from AIBridge.constant.common import get_function_from_json
@@ -56,20 +56,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -111,15 +111,15 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise CohereException(f"Error in generating AI data {e}")
+            raise CohereException(e)
 
     @classmethod
     def get_prompt_context(self, context):
         context_list = []
         prev_role = ""
         if context:
             for _context in context:
@@ -260,15 +260,15 @@
                         content = json.dumps(content)
                     try:
                         if _formatter == "csv":
                             content = FromJson.json_to_csv(json.loads(content))
                         elif _formatter == "xml":
                             content = FromJson.json_to_xml(json.loads(content))
                     except AIBridgeException as e:
-                        raise CohereException(
+                        raise ValidationException(
                             f"Ai response is not in valid {_formatter}"
                         )
                     if _formatter == "json":
                         _validate_obj = ActiveValidator.get_active_validator(_formatter)
                         try:
                             content = _validate_obj.validate(
                                 content,
@@ -296,8 +296,8 @@
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "cohere",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise CohereException(f"{e}")
+            raise CohereException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.3.9/AIBridge/ai_services/geminin_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import google.generativeai as genai
 
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 from openai import OpenAI
 import time
 import uuid
-from AIBridge.exceptions import GeminiException, AIBridgeException
+from AIBridge.exceptions import GeminiException, AIBridgeException, ValidationException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import get_function_from_json, parse_fromat, parse_api_key
 
 
@@ -62,20 +62,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -121,15 +121,15 @@
                 format_strcture,
                 api_key=api_key,
                 stop_subsequence=stop_subsequence,
                 stream=stream,
                 context=context,
             )
         except AIBridgeException as e:
-            raise GeminiException(f"Error in generating AI data {e}")
+            raise GeminiException(e)
 
     @classmethod
     def execute_text_prompt(
         self,
         api_key,
         model,
         messages,
@@ -313,15 +313,15 @@
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(content)
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(content)
                         except AIBridgeException as e:
-                            raise GeminiException(
+                            raise ValidationException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -351,8 +351,8 @@
                     "token_used": token_used,
                     "created_at": int(time.time()),
                     "ai_service": "gemini_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise GeminiException(f"{e}")
+            raise GeminiException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.3.9/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.3.9/AIBridge/ai_services/openai_images.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
-from AIBridge.exceptions import OpenAIException, AIBridgeException
+from AIBridge.exceptions import OpenAIException, AIBridgeException, ValidationException
 import json
 import uuid
 from AIBridge.constant.constant import OPENAI_IMAGE_TYPE, OPENAI_IMAGE_SIZES
 from openai import OpenAI
 from AIBridge.constant.common import parse_api_key
 from AIBridge.ai_services.image_optimisaton import ImageOptimise
 import time
@@ -26,39 +26,41 @@
         message_queue=False,
         api_key=None,
         model="dall-e-2",
         quality="standard",
     ):
         try:
             if prompts and prompt_ids:
-                raise OpenAIException(
+                raise ValidationException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
-                raise OpenAIException(
-                    "Either provide prompts or prompts ids to genrate the data"
+                raise ValidationException(
+                    "Either provide prompts or prompts ids to generate the data"
                 )
             if process_type not in OPENAI_IMAGE_TYPE:
-                raise OpenAIException(
+                raise ValidationException(
                     "process_type can be either create, variation, edit"
                 )
             if size not in OPENAI_IMAGE_SIZES:
-                raise OpenAIException(
+                raise ValidationException(
                     "size can be either 1024x1024 or 512x512 or 256x256"
                 )
             if process_type == "edit" or process_type == "variation":
                 if model != "dall-e-2":
-                    raise OpenAIException(
+                    raise ValidationException(
                         "model can be only dall-e-2 for edit and variation"
                     )
                 if not image_data:
-                    raise OpenAIException("Please enter image for edit or variation")
+                    raise ValidationException(
+                        "Please enter image for edit or variation"
+                    )
             if mask_image:
                 if len(mask_image) != len(image_data):
-                    raise OpenAIException(
+                    raise ValidationException(
                         "mask_image length should be equal to image_data length",
                     )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
@@ -71,15 +73,15 @@
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if image_data:
                 if prompts_list:
                     if len(image_data) != len(prompts_list):
-                        raise OpenAIException(
+                        raise ValidationException(
                             "image_data length should be equal to prompts length",
                         )
             if message_queue:
                 id = uuid.uuid4()
                 message_data = {
                     "id": str(id),
                     "prompts": json.dumps(prompts_list),
@@ -106,15 +108,15 @@
                 size=size,
                 process_type=process_type,
                 api_key=api_key,
                 model=model,
                 quality=quality,
             )
         except AIBridgeException as e:
-            raise OpenAIException(f"{e}")
+            raise OpenAIException(e)
 
     @classmethod
     def get_response(
         self,
         prompts,
         image_data=[],
         mask_image=[],
@@ -175,8 +177,8 @@
                     "token_used": 0,
                     "created_at": time.time(),
                     "ai_service": "open_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise OpenAIException(f"Error in creating image using open ai{e}")
+            raise OpenAIException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.3.9/AIBridge/ai_services/openai_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 from openai import OpenAI
 import time
 import uuid
-from AIBridge.exceptions import OpenAIException, AIBridgeException
+from AIBridge.exceptions import OpenAIException, AIBridgeException, ValidationException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import get_function_from_json, parse_fromat, parse_api_key
 
 
@@ -31,19 +31,19 @@
         message_queue=False,
         api_key=None,
         output_format_parse=True,
         context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise OpenAIException(
+                raise ValidationException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
-                raise OpenAIException(
+                raise ValidationException(
                     "Either provide prompts or prompts ids to genrate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
@@ -55,20 +55,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -110,15 +110,15 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise OpenAIException(f"Error in generating AI data {e}")
+            raise OpenAIException(e)
 
     @classmethod
     def execute_text_prompt(
         self, api_key, model, messages, n, max_tokens=3500, temperature=0.5
     ):
         client = OpenAI(api_key=api_key)
         return client.chat.completions.create(
@@ -248,15 +248,15 @@
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise OpenAIException(
+                            raise ValidationException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -286,8 +286,8 @@
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "open_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise OpenAIException(f"{e}")
+            raise OpenAIException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.3.9/AIBridge/ai_services/palm_chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import time
 import uuid
-from AIBridge.exceptions import PalmTextException, AIBridgeException
+from AIBridge.exceptions import (
+    PalmTextException,
+    AIBridgeException,
+    ValidationException,
+)
 from AIBridge.ai_services.ai_abstraction import AIInterface
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
 import google.generativeai as palm
 
 
 class PalmChat(AIInterface):
@@ -49,15 +53,15 @@
                 examples,
                 model,
                 variation_count,
                 temperature,
                 api_key=api_key,
             )
         except AIBridgeException as e:
-            raise PalmTextException(f"Error in generating AI data {e}")
+            raise PalmTextException(e)
 
     @classmethod
     def get_response(
         self,
         messages,
         context,
         examples,
@@ -85,8 +89,8 @@
                     "created_at": time.time(),
                     "token_used": None,
                     "ai_service": "palm_chat",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise PalmTextException(f"{e}")
+            raise PalmTextException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.3.9/AIBridge/ai_services/palm_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import time
 import uuid
-from AIBridge.exceptions import PalmTextException, AIBridgeException
+from AIBridge.exceptions import (
+    PalmTextException,
+    AIBridgeException,
+    ValidationException,
+)
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
 import google.generativeai as palm
 from AIBridge.output_validation.convertors import FromJson, IntoJson
@@ -31,19 +35,19 @@
         message_queue=False,
         api_key=None,
         output_format_parse=True,
         context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise PalmTextException(
+                raise ValidationException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
-                raise PalmTextException(
+                raise ValidationException(
                     "Either provide prompts or prompts ids to genrate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
@@ -55,20 +59,20 @@
                         prompt_data_list=prompt_data,
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if output_format:
                 if len(output_format) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of output_format must be equal to length of the prompts"
                     )
             if format_strcture:
                 if len(format_strcture) != len(prompts_list):
-                    raise AIBridgeException(
+                    raise ValidationException(
                         "length of format_strcture must be equal to length of the prompts"
                     )
             updated_prompts = []
             for _prompt in prompts_list:
                 format = None
                 format_str = None
                 if output_format:
@@ -110,28 +114,28 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise PalmTextException(f"Error in generating AI data {e}")
+            raise PalmTextException(e)
 
     @classmethod
     def get_tokens(Self, model, text):
         tokens = palm.count_text_tokens(model=model, prompt=text)
         return tokens["token_count"]
 
     @classmethod
     def get_prompt_context(self, context):
         context_string = ""
         if context:
             for _context in context:
                 if _context["role"] not in ["user", "system", "assistant"]:
-                    raise PalmTextException(
+                    raise ValidationException(
                         "Invalid role provided. Please provide either user or system, assistant"
                     )
                 context_string = (
                     context_string + f"{_context['role']}:{_context['context']}" + "\n"
                 )
         return context_string
 
@@ -152,15 +156,15 @@
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
-                raise PalmTextException("No prompts provided")
+                raise ValidationException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("palm_api")
             palm.configure(api_key=api_key)
             model_output = []
             token_used = 0
             context_string = self.get_prompt_context(context)
             for index, prompt in enumerate(prompts):
                 prompt = context_string + "\n" + prompt
@@ -179,15 +183,15 @@
                         _formatter = output_format[index]
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise PalmTextException(
+                            raise ValidationException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -215,8 +219,8 @@
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "palm_api",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise PalmTextException(f"{e}")
+            raise PalmTextException(e)
```

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.3.9/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.3.9/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
-from AIBridge.exceptions import StableDiffusionException, AIBridgeException
+from AIBridge.exceptions import (
+    StableDiffusionException,
+    AIBridgeException,
+    ValidationException,
+)
 import json
 import uuid
 from AIBridge.constant.constant import STABLE_DIFFUSION_TYPES
 from AIBridge.constant.common import parse_api_key, check_url
 import requests
 import time
 
@@ -38,37 +42,33 @@
         seed=None,
         action="text2img",
         message_queue=False,
         api_key=None,
     ):
         try:
             if prompts and prompt_ids:
-                raise StableDiffusionException(
+                raise ValidationException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
-                raise StableDiffusionException(
+                raise ValidationException(
                     "Either provide prompts or prompts ids to genrate the data"
                 )
             if action not in STABLE_DIFFUSION_TYPES:
-                raise StableDiffusionException(
+                raise ValidationException(
                     f"action should be one of the{STABLE_DIFFUSION_TYPES}"
                 )
             if action == "image2image" or action == "inpaint":
                 if not image_data:
-                    raise StableDiffusionException(
-                        "Please enter image link in image data"
-                    )
+                    raise ValidationException("Please enter image link in image data")
             if action == "inpaint" and not mask_image:
-                raise StableDiffusionException(
-                    "Please enter mask image link in mask image"
-                )
+                raise ValidationException("Please enter mask image link in mask image")
             if mask_image:
                 if len(mask_image) != len(image_data):
-                    raise StableDiffusionException(
+                    raise ValidationException(
                         "mask_image length should be equal to image_data length",
                     )
                 check_url(image_data)
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
@@ -82,15 +82,15 @@
                         variables_list=variables,
                     )
                 else:
                     prompts_list = prompts
             if image_data:
                 if prompts_list:
                     if len(image_data) != len(prompts_list):
-                        raise StableDiffusionException(
+                        raise ValidationException(
                             "image_data length should be equal to prompts length",
                         )
                 check_url(image_data)
             if message_queue:
                 id = uuid.uuid4()
                 message_data = {
                     "id": str(id),
@@ -146,15 +146,15 @@
                 upscale=upscale,
                 embeddings_model=embeddings_model,
                 action=action,
                 message_queue=message_queue,
                 api_key=api_key,
             )
         except AIBridgeException as e:
-            raise StableDiffusionException(f"{e}")
+            raise StableDiffusionException(e)
 
     @classmethod
     def get_response(
         self,
         prompts,
         image_data=[],
         mask_image=[],
```

### Comparing `aibridge_test-0.3.8/AIBridge/constant/common.py` & `aibridge_test-0.3.9/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/constant/constant.py` & `aibridge_test-0.3.9/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/database/db_layer.py` & `aibridge_test-0.3.9/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/database/no_sql_service.py` & `aibridge_test-0.3.9/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/database/session.py` & `aibridge_test-0.3.9/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/database/sql_service.py` & `aibridge_test-0.3.9/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/output_validation/convertors.py` & `aibridge_test-0.3.9/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/output_validation/validations.py` & `aibridge_test-0.3.9/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.3.9/AIBridge/prompts/prompt_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Here we are fetching the prompt with reffrence to the id and make the complete prompt out of it,
 We have vraibale and prompt data we dynamically bind the variable to the prompt and then we are returning the complete prompt
 prompt become dynamic and independant of the input varibales whne the vraible changes no need to change the prompt
 
 """
+
 from AIBridge.exceptions import (
     AIBridgeException,
     PromptSaveException,
-    VaribalesException,
+    VariablesException,
     PromptCompletionException,
 )
 from jinja2 import Environment
 from AIBridge.database.models.prompts import Prompts
 from AIBridge.database.models.variables import Variables
 import json
 from AIBridge.database.db_layer import DBLayer
@@ -22,15 +23,15 @@
     def parser(self, prompt, json_data):
         try:
             template_env = Environment(cache_size=1000)
             template = template_env.from_string(prompt)
             parsed_string = template.render(json_data)
             return parsed_string
         except AIBridgeException as e:
-            raise PromptCompletionException("Error in prasing the prompt")
+            raise PromptCompletionException("Error in parsing the prompt")
 
     @classmethod
     def create_prompt_from_id(self, prompt_ids, prompt_data_list=[], variables_list=[]):
         prompts = []
         for index in range(len(prompt_ids)):
             prompt = DBLayer.get_by_id(Prompts, id=prompt_ids[index])
             prompt_data = (
@@ -42,15 +43,15 @@
                 json.loads(prompt["variables"])
                 if not variables_list
                 else variables_list[index]
             )
             for key, value in variables.items():
                 variable = DBLayer.filter_table(Variables, **{"key": value})
                 if variable is None:
-                    raise VaribalesException(f"Invalid variable key->{key}")
+                    raise VariablesException(f"Invalid variable key->{key}")
                 var_value = json.loads(variable["value"])
                 prompt_data[key] = ",".join(map(str, var_value))
             prompt_string = self.parser(prompt["prompt"], prompt_data)
             prompts.append(prompt_string)
         return prompts
 
     @classmethod
@@ -61,13 +62,13 @@
             prompt_string = prompt_list[index]
             if prompt_data_list:
                 variables.update(prompt_data_list[index])
             if variables_list:
                 for key, value in variables_list[index].items():
                     variable = DBLayer.filter_table(Variables, **{"key": value})
                     if variable is None:
-                        raise VaribalesException(f"Invalid variable key->{key}")
+                        raise VariablesException(f"Invalid variable key->{key}")
                     var_value = json.loads(variable["value"])
                     variables[key] = ",".join(map(str, var_value))
             prompt_string = self.parser(prompt_string, variables)
             prompts.append(prompt_string)
         return prompts
```

### Comparing `aibridge_test-0.3.8/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.3.9/AIBridge/prompts/prompts_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sqlite3
 
-from AIBridge.exceptions import VaribalesException
+from AIBridge.exceptions import VariablesException
 from AIBridge.database.models.prompts import Prompts, Base
 from AIBridge.exceptions import AIBridgeException, PromptSaveException
 from AIBridge.database.models.variables import Variables, Base as v_base
 from AIBridge.database.db_layer import DBLayer
 import uuid
 import json
 import calendar
@@ -17,15 +17,15 @@
         return calendar.timegm(time.gmtime())
 
     @classmethod
     def validate_variables(self, variables):
         for key, value in variables.items():
             variable = DBLayer.filter_table(Variables, **{"key": value})
             if not variable:
-                raise VaribalesException(f"Invalid variable key->{key}")
+                raise VariablesException(f"Invalid variable key->{key}")
 
     @classmethod
     def validate_prompt(
         self, prompt=None, name=None, prompt_data={}, variables={}, id=None
     ):
         if id:
             try:
```

### Comparing `aibridge_test-0.3.8/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.3.9/AIBridge/prompts/prompts_varibales.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sqlite3
-from AIBridge.exceptions import AIBridgeException, VaribalesException
+from AIBridge.exceptions import AIBridgeException, VariablesException
 from AIBridge.database.models.variables import Variables, Base
 import uuid
 import json
 import calendar
 import time
 from AIBridge.database.db_layer import DBLayer
 
@@ -15,29 +15,29 @@
 
     @classmethod
     def validates_variables(self, var_key=None, var_value=None, id=None):
         if id:
             try:
                 uuid.UUID(id)
             except AIBridgeException as e:
-                raise VaribalesException("Invalid variable id")
+                raise VariablesException("Invalid variable id")
         if var_key:
             if not isinstance(var_key, str):
-                raise VaribalesException("Invalid variable key, it must be string")
+                raise VariablesException("Invalid variable key, it must be string")
         if var_value:
             if not isinstance(var_value, list):
-                raise VaribalesException("Invalid variable value it must be list")
+                raise VariablesException("Invalid variable value it must be list")
 
     @classmethod
     def save_variables(self, var_key: str, var_value: list):
         self.validates_variables(var_key=var_key, var_value=var_value)
         table_exist = DBLayer.check_table(Variables, Base, method="save")
         variable_n = DBLayer.filter_table(Variables, **{"key": var_key})
         if variable_n:
-            raise VaribalesException(
+            raise VariablesException(
                 f"variable already exists with the key ->{var_key}"
             )
         str_id = str(uuid.uuid4())
         variable = {
             "id": str_id,
             "key": var_key,
             "value": json.dumps(var_value),
@@ -50,15 +50,15 @@
     def update_variables(self, id: str, var_key=None, var_value=None):
         self.validates_variables(id=id, var_key=var_key, var_value=var_value)
         variable = DBLayer.get_by_id(Variables, id)
         if var_key:
             variable_key = DBLayer.filter_table(Variables, **{"key": var_key})
             if variable_key:
                 if variable_key["key"] != var_key:
-                    raise VaribalesException(
+                    raise VariablesException(
                         f"variable already exists with the key ->{var_key}"
                     )
         updates = {
             "key": var_key,
             "value": json.dumps(var_value),
             "updated_at": self.get_time(),
         }
```

### Comparing `aibridge_test-0.3.8/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.3.9/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.3.9/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.3.9/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/AIBridge/setconfig.py` & `aibridge_test-0.3.9/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/LICENSE` & `aibridge_test-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/PKG-INFO` & `aibridge_test-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.8
+Version: 0.3.9
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.8/README.md` & `aibridge_test-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.3.9/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.8
+Version: 0.3.9
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.8/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.3.9/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.8/setup.py` & `aibridge_test-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.3.8"
+VERSION = "0.3.9"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

