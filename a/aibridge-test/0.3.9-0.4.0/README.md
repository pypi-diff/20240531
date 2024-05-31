# Comparing `tmp/aibridge_test-0.3.9.tar.gz` & `tmp/aibridge_test-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.3.9.tar", last modified: Fri May 31 06:00:26 2024, max compression
+gzip compressed data, was "aibridge_test-0.4.0.tar", last modified: Fri May 31 07:32:18 2024, max compression
```

## Comparing `aibridge_test-0.3.9.tar` & `aibridge_test-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:26.077281 aibridge_test-0.3.9/
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.715284 aibridge_test-0.3.9/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.9/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.833281 aibridge_test-0.3.9/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9357 2024-05-31 04:24:01.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    14000 2024-05-31 04:24:49.000000 aibridge_test-0.3.9/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12308 2024-05-31 04:25:25.000000 aibridge_test-0.3.9/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14683 2024-05-31 04:26:27.000000 aibridge_test-0.3.9/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7569 2024-05-31 04:28:50.000000 aibridge_test-0.3.9/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11901 2024-05-31 04:29:31.000000 aibridge_test-0.3.9/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2951 2024-05-31 04:30:00.000000 aibridge_test-0.3.9/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9267 2024-05-31 04:31:25.000000 aibridge_test-0.3.9/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.9/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10264 2024-05-31 04:32:52.000000 aibridge_test-0.3.9/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.843284 aibridge_test-0.3.9/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.9/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.9/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.891283 aibridge_test-0.3.9/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.911282 aibridge_test-0.3.9/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     4039 2024-05-31 05:38:04.000000 aibridge_test-0.3.9/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.936280 aibridge_test-0.3.9/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.9/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.9/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.956283 aibridge_test-0.3.9/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-05-31 05:04:54.000000 aibridge_test-0.3.9/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-05-31 05:04:55.000000 aibridge_test-0.3.9/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-05-31 05:04:54.000000 aibridge_test-0.3.9/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:25.982281 aibridge_test-0.3.9/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.9/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.9/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-05-31 06:00:26.072285 aibridge_test-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 06:00:26.067280 aibridge_test-0.3.9/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 06:00:25.000000 aibridge_test-0.3.9/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 06:00:26.080294 aibridge_test-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-05-31 05:59:13.000000 aibridge_test-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.371181 aibridge_test-0.4.0/
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:17.855180 aibridge_test-0.4.0/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.4.0/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.100181 aibridge_test-0.4.0/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9341 2024-05-31 07:27:59.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13984 2024-05-31 07:28:12.000000 aibridge_test-0.4.0/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12292 2024-05-31 07:29:52.000000 aibridge_test-0.4.0/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14667 2024-05-31 07:28:36.000000 aibridge_test-0.4.0/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3572 2024-05-31 07:28:41.000000 aibridge_test-0.4.0/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7553 2024-05-31 07:29:49.000000 aibridge_test-0.4.0/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11885 2024-05-31 07:27:40.000000 aibridge_test-0.4.0/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2935 2024-05-31 07:29:46.000000 aibridge_test-0.4.0/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9251 2024-05-31 07:29:20.000000 aibridge_test-0.4.0/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.4.0/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10256 2024-05-31 07:29:39.000000 aibridge_test-0.4.0/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.125180 aibridge_test-0.4.0/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.4.0/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.4.0/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.158197 aibridge_test-0.4.0/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.171182 aibridge_test-0.4.0/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     4124 2024-05-31 07:26:45.000000 aibridge_test-0.4.0/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.191216 aibridge_test-0.4.0/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.4.0/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.4.0/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.218179 aibridge_test-0.4.0/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-05-31 05:04:54.000000 aibridge_test-0.4.0/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-05-31 05:04:55.000000 aibridge_test-0.4.0/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-05-31 05:04:54.000000 aibridge_test-0.4.0/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.261181 aibridge_test-0.4.0/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.4.0/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.4.0/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-05-31 07:32:18.354184 aibridge_test-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.351181 aibridge_test-0.4.0/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:32:18.372221 aibridge_test-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-05-31 07:31:25.000000 aibridge_test-0.4.0/setup.py
```

### Comparing `aibridge_test-0.3.9/AIBridge/__init__.py` & `aibridge_test-0.4.0/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.4.0/AIBridge/ai_services/ai21labs_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise Ai21Exception(e)
 
     @classmethod
     def get_prompt_context(self, context):
         context_string = ""
         if context:
             for _context in context:
@@ -217,9 +217,9 @@
                     "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "ai21_api",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise Ai21Exception(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.4.0/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.4.0/AIBridge/ai_services/anthropic_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
                 stream=stream,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise AnthropicsException(e)
 
     @classmethod
     def execute_text_prompt(
         self, api_key, model, messages, n, max_tokens=3500, temperature=0.5
     ):
         client = Anthropic(api_key=api_key)
@@ -335,9 +335,9 @@
                     "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "anthropic",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise AnthropicsException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.4.0/AIBridge/ai_services/cohere_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise CohereException(e)
 
     @classmethod
     def get_prompt_context(self, context):
         context_list = []
         prev_role = ""
         if context:
@@ -295,9 +295,9 @@
                     "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "cohere",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise CohereException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.4.0/AIBridge/ai_services/geminin_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 stop_subsequence=stop_subsequence,
                 stream=stream,
                 context=context,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise GeminiException(e)
 
     @classmethod
     def execute_text_prompt(
         self,
         api_key,
         model,
@@ -350,9 +350,9 @@
                     "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": int(time.time()),
                     "ai_service": "gemini_ai",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise GeminiException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.4.0/AIBridge/ai_services/image_optimisaton.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                         binary_data = image_file.read()
                     image_buffer = BytesIO(binary_data)
                     image = Image.open(image_buffer)
                 if image.mode != "RGBA":
                     image = image.convert("RGBA")
                 image_obj.append(image)
             return image_obj
-        except AIBridgeException as e:
+        except Exception as e:
             raise ImageException(f"Error in reading the the image {e}")
 
     @classmethod
     def get_bytes_io(self, image_data):
         image_obj = []
         for image in image_data:
             buf = BytesIO()
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.4.0/AIBridge/ai_services/openai_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 variation_count=variation_count,
                 size=size,
                 process_type=process_type,
                 api_key=api_key,
                 model=model,
                 quality=quality,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise OpenAIException(e)
 
     @classmethod
     def get_response(
         self,
         prompts,
         image_data=[],
@@ -176,9 +176,9 @@
                     "response": data,
                     "token_used": 0,
                     "created_at": time.time(),
                     "ai_service": "open_ai",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise OpenAIException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.4.0/AIBridge/ai_services/openai_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise OpenAIException(e)
 
     @classmethod
     def execute_text_prompt(
         self, api_key, model, messages, n, max_tokens=3500, temperature=0.5
     ):
         client = OpenAI(api_key=api_key)
@@ -285,9 +285,9 @@
                     "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "open_ai",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise OpenAIException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.4.0/AIBridge/ai_services/palm_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 context,
                 examples,
                 model,
                 variation_count,
                 temperature,
                 api_key=api_key,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise PalmTextException(e)
 
     @classmethod
     def get_response(
         self,
         messages,
         context,
@@ -88,9 +88,9 @@
                     },
                     "created_at": time.time(),
                     "token_used": None,
                     "ai_service": "palm_chat",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise PalmTextException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.4.0/AIBridge/ai_services/palm_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise PalmTextException(e)
 
     @classmethod
     def get_tokens(Self, model, text):
         tokens = palm.count_text_tokens(model=model, prompt=text)
         return tokens["token_count"]
 
@@ -218,9 +218,9 @@
                     "response": model_output,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "palm_api",
                 }
             }
             return message_value
-        except AIBridgeException as e:
+        except Exception as e:
             raise PalmTextException(e)
```

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.4.0/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.4.0/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 self_attention=self_attention,
                 upscale=upscale,
                 embeddings_model=embeddings_model,
                 action=action,
                 message_queue=message_queue,
                 api_key=api_key,
             )
-        except AIBridgeException as e:
+        except Exception as e:
             raise StableDiffusionException(e)
 
     @classmethod
     def get_response(
         self,
         prompts,
         image_data=[],
```

### Comparing `aibridge_test-0.3.9/AIBridge/constant/common.py` & `aibridge_test-0.4.0/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/constant/constant.py` & `aibridge_test-0.4.0/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/database/db_layer.py` & `aibridge_test-0.4.0/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/database/no_sql_service.py` & `aibridge_test-0.4.0/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/database/session.py` & `aibridge_test-0.4.0/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/database/sql_service.py` & `aibridge_test-0.4.0/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/output_validation/convertors.py` & `aibridge_test-0.4.0/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/output_validation/validations.py` & `aibridge_test-0.4.0/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.4.0/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.4.0/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.4.0/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.4.0/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.4.0/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.4.0/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/AIBridge/setconfig.py` & `aibridge_test-0.4.0/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/LICENSE` & `aibridge_test-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/PKG-INFO` & `aibridge_test-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.9
+Version: 0.4.0
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.9/README.md` & `aibridge_test-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.4.0/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.9
+Version: 0.4.0
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.9/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.4.0/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.9/setup.py` & `aibridge_test-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.3.9"
+VERSION = "0.4.0"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

