# Comparing `tmp/aibridge_test-0.4.0.tar.gz` & `tmp/aibridge_test-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.4.0.tar", last modified: Fri May 31 07:32:18 2024, max compression
+gzip compressed data, was "aibridge_test-0.4.1.tar", last modified: Fri May 31 09:27:48 2024, max compression
```

## Comparing `aibridge_test-0.4.0.tar` & `aibridge_test-0.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.371181 aibridge_test-0.4.0/
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:17.855180 aibridge_test-0.4.0/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.4.0/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.100181 aibridge_test-0.4.0/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9341 2024-05-31 07:27:59.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13984 2024-05-31 07:28:12.000000 aibridge_test-0.4.0/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12292 2024-05-31 07:29:52.000000 aibridge_test-0.4.0/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14667 2024-05-31 07:28:36.000000 aibridge_test-0.4.0/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3572 2024-05-31 07:28:41.000000 aibridge_test-0.4.0/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7553 2024-05-31 07:29:49.000000 aibridge_test-0.4.0/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11885 2024-05-31 07:27:40.000000 aibridge_test-0.4.0/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2935 2024-05-31 07:29:46.000000 aibridge_test-0.4.0/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9251 2024-05-31 07:29:20.000000 aibridge_test-0.4.0/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.4.0/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10256 2024-05-31 07:29:39.000000 aibridge_test-0.4.0/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.125180 aibridge_test-0.4.0/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.4.0/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.4.0/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.158197 aibridge_test-0.4.0/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.171182 aibridge_test-0.4.0/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     4124 2024-05-31 07:26:45.000000 aibridge_test-0.4.0/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.191216 aibridge_test-0.4.0/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.4.0/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.4.0/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.218179 aibridge_test-0.4.0/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-05-31 05:04:54.000000 aibridge_test-0.4.0/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-05-31 05:04:55.000000 aibridge_test-0.4.0/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-05-31 05:04:54.000000 aibridge_test-0.4.0/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.261181 aibridge_test-0.4.0/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.4.0/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.4.0/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-05-31 07:32:18.354184 aibridge_test-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:32:18.351181 aibridge_test-0.4.0/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 07:32:17.000000 aibridge_test-0.4.0/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 07:32:18.372221 aibridge_test-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-05-31 07:31:25.000000 aibridge_test-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.951759 aibridge_test-0.4.1/
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.643741 aibridge_test-0.4.1/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.4.1/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.709740 aibridge_test-0.4.1/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9341 2024-05-31 07:27:59.000000 aibridge_test-0.4.1/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13984 2024-05-31 07:28:12.000000 aibridge_test-0.4.1/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12292 2024-05-31 07:29:52.000000 aibridge_test-0.4.1/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14667 2024-05-31 07:28:36.000000 aibridge_test-0.4.1/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3572 2024-05-31 07:28:41.000000 aibridge_test-0.4.1/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7553 2024-05-31 07:29:49.000000 aibridge_test-0.4.1/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11885 2024-05-31 07:27:40.000000 aibridge_test-0.4.1/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2935 2024-05-31 07:29:46.000000 aibridge_test-0.4.1/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9251 2024-05-31 07:29:20.000000 aibridge_test-0.4.1/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.4.1/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10256 2024-05-31 07:29:39.000000 aibridge_test-0.4.1/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.717744 aibridge_test-0.4.1/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.4.1/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.4.1/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.749740 aibridge_test-0.4.1/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.771742 aibridge_test-0.4.1/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     4497 2024-05-31 09:25:37.000000 aibridge_test-0.4.1/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.798740 aibridge_test-0.4.1/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.4.1/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.4.1/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.816742 aibridge_test-0.4.1/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-05-31 05:04:54.000000 aibridge_test-0.4.1/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-05-31 05:04:55.000000 aibridge_test-0.4.1/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-05-31 05:04:54.000000 aibridge_test-0.4.1/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.837742 aibridge_test-0.4.1/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.4.1/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.4.1/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-05-31 09:27:48.948738 aibridge_test-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 09:27:48.946741 aibridge_test-0.4.1/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-05-31 09:27:48.000000 aibridge_test-0.4.1/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-31 09:27:48.000000 aibridge_test-0.4.1/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:27:48.000000 aibridge_test-0.4.1/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-05-31 09:27:48.000000 aibridge_test-0.4.1/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 09:27:48.000000 aibridge_test-0.4.1/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:27:48.951759 aibridge_test-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-05-31 09:26:45.000000 aibridge_test-0.4.1/setup.py
```

### Comparing `aibridge_test-0.4.0/AIBridge/__init__.py` & `aibridge_test-0.4.1/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.4.1/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.4.1/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.4.1/AIBridge/ai_services/anthropic_ai.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.4.1/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.4.1/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.4.1/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.4.1/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.4.1/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.4.1/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.4.1/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.4.1/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.4.1/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/constant/common.py` & `aibridge_test-0.4.1/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/constant/constant.py` & `aibridge_test-0.4.1/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/database/db_layer.py` & `aibridge_test-0.4.1/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/database/no_sql_service.py` & `aibridge_test-0.4.1/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/database/session.py` & `aibridge_test-0.4.1/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/database/sql_service.py` & `aibridge_test-0.4.1/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/exceptions.py` & `aibridge_test-0.4.1/AIBridge/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
                 code = message.get("error_code", 400)
             if isinstance(message, dict):
                 if "error" in message:
                     if "message" in message["error"]:
                         message = message["error"]["message"]
                     else:
                         message = str(message)
-
+                elif "Details" in message:
+                    message = message["Details"]
+                    if "detail" in message:
+                        message = message["detail"]
         else:
             if hasattr(message, "code"):
                 code = message.code
             elif hasattr(message, "status_code"):
                 code = message.status_code
             elif hasattr(message, "error_code"):
                 code = message.error_code
@@ -31,14 +34,18 @@
                 code = 400
             if hasattr(message, "message"):
                 message = message.message
             elif hasattr(message, "body"):
                 message = message.body
             elif hasattr(message, "error"):
                 message = message.error
+            elif hasattr(message, "Details"):
+                message = message["Details"]
+                if "detail" in message:
+                    message = message["detail"]
             if isinstance(message, dict):
                 if "error" in message:
                     if "message" in message["error"]:
                         message = message["error"]["message"]
                     else:
                         message = str(message)
             else:
```

### Comparing `aibridge_test-0.4.0/AIBridge/output_validation/convertors.py` & `aibridge_test-0.4.1/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/output_validation/validations.py` & `aibridge_test-0.4.1/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.4.1/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.4.1/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.4.1/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.4.1/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.4.1/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.4.1/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/AIBridge/setconfig.py` & `aibridge_test-0.4.1/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/LICENSE` & `aibridge_test-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/PKG-INFO` & `aibridge_test-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.4.0
+Version: 0.4.1
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.4.0/README.md` & `aibridge_test-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.4.1/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.4.0
+Version: 0.4.1
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.4.0/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.4.1/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.4.0/setup.py` & `aibridge_test-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

