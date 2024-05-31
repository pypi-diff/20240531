# Comparing `tmp/portkey_ai-1.2.4.tar.gz` & `tmp/portkey_ai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portkey_ai-1.2.4.tar", last modified: Sat Apr 13 13:33:12 2024, max compression
+gzip compressed data, was "portkey_ai-1.3.0.tar", last modified: Fri May 31 15:23:52 2024, max compression
```

## Comparing `portkey_ai-1.2.4.tar` & `portkey_ai-1.3.0.tar`

### file list

```diff
@@ -1,78 +1,97 @@
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.291782 portkey_ai-1.2.4/
--rw-r--r--   0 visargdesai   (501) staff       (20)     1067 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/LICENSE
--rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-04-13 13:33:12.291682 portkey_ai-1.2.4/PKG-INFO
--rw-r--r--   0 visargdesai   (501) staff       (20)     4240 2024-04-05 10:21:35.000000 portkey_ai-1.2.4/README.md
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.276054 portkey_ai-1.2.4/portkey_ai/
--rw-r--r--   0 visargdesai   (501) staff       (20)     2056 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      380 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/_portkey_scripts.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.278718 portkey_ai-1.2.4/portkey_ai/api_resources/
--rw-r--r--   0 visargdesai   (501) staff       (20)     1760 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/__init__.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.282122 portkey_ai-1.2.4/portkey_ai/api_resources/apis/
--rw-r--r--   0 visargdesai   (501) staff       (20)     1444 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      992 2024-02-13 17:21:25.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/api_resource.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7176 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/assistants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6683 2024-04-13 09:06:43.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6002 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      825 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/create_headers.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2177 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/embeddings.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2533 2024-02-13 17:21:25.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/feedback.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    10091 2024-04-05 10:21:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/generation.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     5679 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3602 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/main_files.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2639 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/models.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2493 2024-02-13 17:21:25.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/post.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    15774 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/apis/threads.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    20922 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/base_client.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     5833 2024-03-23 09:57:17.000000 portkey_ai-1.2.4/portkey_ai/api_resources/client.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      903 2024-04-05 10:21:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/common_types.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4020 2024-01-12 13:07:25.000000 portkey_ai-1.2.4/portkey_ai/api_resources/exceptions.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1164 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/global_constants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7058 2024-02-13 17:21:25.000000 portkey_ai-1.2.4/portkey_ai/api_resources/streaming.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.284451 portkey_ai-1.2.4/portkey_ai/api_resources/types/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3613 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/assistant_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3568 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/chat_complete_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2413 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/complete_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1163 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/embeddings_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3368 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/generation_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      858 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/image_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1978 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/main_file_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1675 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/models_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3053 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_message_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6102 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_run_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      965 2024-04-13 13:30:23.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      426 2024-03-21 12:59:35.000000 portkey_ai-1.2.4/portkey_ai/api_resources/types/utils.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    12195 2024-04-13 08:51:10.000000 portkey_ai-1.2.4/portkey_ai/api_resources/utils.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.284584 portkey_ai-1.2.4/portkey_ai/llms/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/llms/__init__.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.285248 portkey_ai-1.2.4/portkey_ai/llms/langchain/
--rw-r--r--   0 visargdesai   (501) staff       (20)      106 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/llms/langchain/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7232 2024-04-13 09:42:19.000000 portkey_ai-1.2.4/portkey_ai/llms/langchain/chat.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4771 2024-04-13 09:41:59.000000 portkey_ai-1.2.4/portkey_ai/llms/langchain/completion.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.285741 portkey_ai-1.2.4/portkey_ai/llms/llama_index/
--rw-r--r--   0 visargdesai   (501) staff       (20)       62 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/llms/llama_index/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7253 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/llms/llama_index/completions.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3277 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/llms/llama_index/utils.py
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/portkey_ai/py.typed
--rw-r--r--   0 visargdesai   (501) staff       (20)       18 2024-04-13 13:32:52.000000 portkey_ai-1.2.4/portkey_ai/version.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.290576 portkey_ai-1.2.4/portkey_ai.egg-info/
--rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/PKG-INFO
--rw-r--r--   0 visargdesai   (501) staff       (20)     2409 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/SOURCES.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/dependency_links.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)       64 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/entry_points.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)      263 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/requires.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)       17 2024-04-13 13:33:12.000000 portkey_ai-1.2.4/portkey_ai.egg-info/top_level.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-01-08 09:37:18.000000 portkey_ai-1.2.4/portkey_ai.egg-info/zip-safe
--rw-r--r--   0 visargdesai   (501) staff       (20)       80 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/pyproject.toml
--rw-r--r--   0 visargdesai   (501) staff       (20)     1155 2024-04-13 13:33:12.292213 portkey_ai-1.2.4/setup.cfg
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-04-13 13:33:12.290384 portkey_ai-1.2.4/tests/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.2.4/tests/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4724 2024-03-27 10:29:03.000000 portkey_ai-1.2.4/tests/test_assistants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    15529 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_async_chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    14317 2024-04-13 09:41:46.000000 portkey_ai-1.2.4/tests/test_async_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7609 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_async_images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    14966 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    13730 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7246 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2536 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/test_threads.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      497 2024-03-21 14:00:19.000000 portkey_ai-1.2.4/tests/utils.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.579394 portkey_ai-1.3.0/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1067 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/LICENSE
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 15:23:52.579286 portkey_ai-1.3.0/PKG-INFO
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4240 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/README.md
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.476666 portkey_ai-1.3.0/portkey_ai/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2816 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      380 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/_portkey_scripts.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.480650 portkey_ai-1.3.0/portkey_ai/api_resources/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2520 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/__init__.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.488632 portkey_ai-1.3.0/portkey_ai/api_resources/apis/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2324 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1180 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/api_resource.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3662 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/assistants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6417 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/audio.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3971 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/batches.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6707 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6026 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1139 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/create_headers.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2177 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/embeddings.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3795 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/feedback.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     8416 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/fine_tuning.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    10091 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/generation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5679 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4432 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/main_files.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2639 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/models.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1574 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2493 2024-02-13 17:21:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/post.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    40728 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/threads.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    24230 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/vector_stores.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    29119 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/base_client.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14130 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/client.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      903 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/common_types.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4020 2024-01-12 13:07:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/exceptions.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1164 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/global_constants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7058 2024-02-13 17:21:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/streaming.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.494855 portkey_ai-1.3.0/portkey_ai/api_resources/types/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3612 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/assistant_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1173 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/audio_types.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2159 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/batches_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3568 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/chat_complete_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2413 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/complete_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1163 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/embeddings_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      212 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/feedback_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4872 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/fine_tuning_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3420 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/generation_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      858 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/image_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1978 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/main_file_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1675 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/models_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      793 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/moderations_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3415 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_message_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6102 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_run_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      965 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      426 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/utils.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3417 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/vector_stores_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    12969 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/utils.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.495043 portkey_ai-1.3.0/portkey_ai/llms/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/__init__.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.495689 portkey_ai-1.3.0/portkey_ai/llms/langchain/
+-rw-r--r--   0 visargdesai   (501) staff       (20)      106 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7232 2024-05-31 15:19:33.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/chat.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4771 2024-05-31 15:19:33.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/completion.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.534356 portkey_ai-1.3.0/portkey_ai/llms/llama_index/
+-rw-r--r--   0 visargdesai   (501) staff       (20)       62 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7253 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/completions.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3277 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/utils.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/py.typed
+-rw-r--r--   0 visargdesai   (501) staff       (20)       18 2024-05-31 15:22:36.000000 portkey_ai-1.3.0/portkey_ai/version.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.577669 portkey_ai-1.3.0/portkey_ai.egg-info/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/PKG-INFO
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3178 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)       64 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/entry_points.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)      263 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/requires.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)       17 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/top_level.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-01-08 09:37:18.000000 portkey_ai-1.3.0/portkey_ai.egg-info/zip-safe
+-rw-r--r--   0 visargdesai   (501) staff       (20)       80 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/pyproject.toml
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1155 2024-05-31 15:23:52.586785 portkey_ai-1.3.0/setup.cfg
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.577261 portkey_ai-1.3.0/tests/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/tests/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4668 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_assistants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4609 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_speech.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4618 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_transcript.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4627 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_translation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    15529 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_async_chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14317 2024-05-31 14:40:38.000000 portkey_ai-1.3.0/tests/test_async_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7609 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_async_images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4400 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4468 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_speech.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4476 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_transcript.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4486 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_translation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14966 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    13730 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7246 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4259 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2536 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_threads.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      497 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/utils.py
```

### Comparing `portkey_ai-1.2.4/LICENSE` & `portkey_ai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/PKG-INFO` & `portkey_ai-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portkey-ai
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python client library for the Portkey API
 Home-page: https://github.com/Portkey-AI/portkey-python-sdk
 Author: Portkey.ai
 Author-email: support@portkey.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `portkey_ai-1.2.4/README.md` & `portkey_ai-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/__init__.py` & `portkey_ai-1.3.0/portkey_ai/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,22 +30,42 @@
     AsyncThreads,
     Messages,
     AsyncMessages,
     MainFiles,
     AsyncMainFiles,
     Models,
     AsyncModels,
-    ThreadFiles,
-    AsyncThreadFiles,
-    AssistantFiles,
-    AsyncAssistantFiles,
     Runs,
     AsyncRuns,
     Steps,
     AsyncSteps,
+    Moderations,
+    AsyncModerations,
+    Audio,
+    Transcriptions,
+    Translations,
+    Speech,
+    AsyncAudio,
+    AsyncTranscriptions,
+    AsyncTranslations,
+    AsyncSpeech,
+    Batches,
+    AsyncBatches,
+    FineTuning,
+    Jobs,
+    Checkpoints,
+    AsyncFineTuning,
+    AsyncJobs,
+    AsyncCheckpoints,
+    VectorStores,
+    VectorFiles,
+    VectorFileBatches,
+    AsyncVectorStores,
+    AsyncVectorFiles,
+    AsyncVectorFileBatches,
 )
 
 from portkey_ai.version import VERSION
 from portkey_ai.api_resources.global_constants import (
     PORTKEY_BASE_URL,
     PORTKEY_API_KEY_ENV,
     PORTKEY_PROXY_ENV,
@@ -91,16 +111,36 @@
     "AsyncThreads",
     "Messages",
     "AsyncMessages",
     "MainFiles",
     "AsyncMainFiles",
     "Models",
     "AsyncModels",
-    "ThreadFiles",
-    "AsyncThreadFiles",
-    "AssistantFiles",
-    "AsyncAssistantFiles",
     "Runs",
     "AsyncRuns",
     "Steps",
     "AsyncSteps",
+    "Moderations",
+    "AsyncModerations",
+    "Audio",
+    "Transcriptions",
+    "Translations",
+    "Speech",
+    "AsyncAudio",
+    "AsyncTranscriptions",
+    "AsyncTranslations",
+    "AsyncSpeech",
+    "Batches",
+    "AsyncBatches",
+    "FineTuning",
+    "Jobs",
+    "Checkpoints",
+    "AsyncFineTuning",
+    "AsyncJobs",
+    "AsyncCheckpoints",
+    "VectorStores",
+    "VectorFiles",
+    "VectorFileBatches",
+    "AsyncVectorStores",
+    "AsyncVectorFiles",
+    "AsyncVectorFileBatches",
 ]
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/__init__.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,22 +19,42 @@
     AsyncThreads,
     Messages,
     AsyncMessages,
     MainFiles,
     AsyncMainFiles,
     Models,
     AsyncModels,
-    ThreadFiles,
-    AsyncThreadFiles,
-    AssistantFiles,
-    AsyncAssistantFiles,
     Runs,
     AsyncRuns,
     Steps,
     AsyncSteps,
+    Moderations,
+    AsyncModerations,
+    Audio,
+    Transcriptions,
+    Translations,
+    Speech,
+    AsyncAudio,
+    AsyncTranscriptions,
+    AsyncTranslations,
+    AsyncSpeech,
+    Batches,
+    AsyncBatches,
+    FineTuning,
+    Jobs,
+    Checkpoints,
+    AsyncFineTuning,
+    AsyncJobs,
+    AsyncCheckpoints,
+    VectorStores,
+    VectorFiles,
+    VectorFileBatches,
+    AsyncVectorStores,
+    AsyncVectorFiles,
+    AsyncVectorFileBatches,
 )
 from .utils import (
     Modes,
     ModesLiteral,
     LLMOptions,
     ProviderTypes,
     ProviderTypesLiteral,
@@ -85,16 +105,36 @@
     "AsyncThreads",
     "Messages",
     "AsyncMessages",
     "MainFiles",
     "AsyncMainFiles",
     "Models",
     "AsyncModels",
-    "ThreadFiles",
-    "AsyncThreadFiles",
-    "AssistantFiles",
-    "AsyncAssistantFiles",
     "Runs",
     "AsyncRuns",
     "Steps",
     "AsyncSteps",
+    "Moderations",
+    "AsyncModerations",
+    "Audio",
+    "Transcriptions",
+    "Translations",
+    "Speech",
+    "AsyncAudio",
+    "AsyncTranscriptions",
+    "AsyncTranslations",
+    "AsyncSpeech",
+    "Batches",
+    "AsyncBatches",
+    "FineTuning",
+    "Jobs",
+    "Checkpoints",
+    "AsyncFineTuning",
+    "AsyncJobs",
+    "AsyncCheckpoints",
+    "VectorStores",
+    "VectorFiles",
+    "VectorFileBatches",
+    "AsyncVectorStores",
+    "AsyncVectorFiles",
+    "AsyncVectorFileBatches",
 ]
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/api_resource.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/api_resource.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,23 +15,29 @@
         # self._patch = client.patch
         # self._put = client.put
         # self._delete = client.delete
 
     def _post(self, *args, **kwargs):
         return self._client._post(*args, **kwargs)
 
+    def _put(self, *args, **kwargs):
+        return self._client._put(*args, **kwargs)
+
 
 class AsyncAPIResource:
     _client: AsyncAPIClient
 
     def __init__(self, client: AsyncAPIClient) -> None:
         self._client = client
         # self._get = client.get
         # self._patch = client.patch
         # self._put = client.put
         # self._delete = client.delete
 
     async def _post(self, *args, **kwargs):
         return await self._client._post(*args, **kwargs)
 
+    async def _put(self, *args, **kwargs):
+        return await self._client._put(*args, **kwargs)
+
     async def _sleep(self, seconds: float) -> None:
         await asyncio.sleep(seconds)
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/chat_complete.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/chat_complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class Completions(APIResource):
     def __init__(self, client: Portkey) -> None:
         super().__init__(client)
         self.openai_client = client.openai_client
 
-    def stream_create(
+    def stream_create(  # type: ignore[return]
         self, model, messages, stream, temperature, max_tokens, top_p, **kwargs
     ) -> Union[ChatCompletions, Iterator[ChatCompletionChunk]]:
         with self.openai_client.with_streaming_response.chat.completions.create(
             model=model,
             messages=messages,
             stream=stream,
             temperature=temperature,
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/complete.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class Completion(APIResource):
     def __init__(self, client: Portkey) -> None:
         super().__init__(client)
         self.openai_client = client.openai_client
         self.client = client
 
-    def stream_create(
+    def stream_create(  # type: ignore[return]
         self, model, prompt, stream, temperature, max_tokens, top_p, **kwargs
     ) -> Union[TextCompletion, Iterator[TextCompletionChunk]]:
         with self.openai_client.with_streaming_response.completions.create(
             model=model,
             prompt=prompt,
             stream=stream,
             temperature=temperature,
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/embeddings.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/embeddings.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/feedback.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/feedback.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 from typing import Optional, Dict, Any, List
 from portkey_ai.api_resources.apis.api_resource import APIResource, AsyncAPIResource
 from portkey_ai.api_resources.base_client import APIClient, AsyncAPIClient
 from portkey_ai.api_resources.streaming import AsyncStream, Stream
-from portkey_ai.api_resources.utils import GenericResponse, PortkeyApiPaths
+from portkey_ai.api_resources.types.feedback_type import FeedbackResponse
+from portkey_ai.api_resources.utils import PortkeyApiPaths
 
 
 class Feedback(APIResource):
     def __init__(self, client: APIClient) -> None:
         super().__init__(client)
 
     def create(
         self,
         *,
         trace_id: Optional[str] = None,
         value: Optional[int] = None,
         weight: Optional[float] = None,
-        metadata: Optional[Dict[str, Any]] = None
-    ) -> GenericResponse:
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> FeedbackResponse:
         body = dict(trace_id=trace_id, value=value, weight=weight, metadata=metadata)
         return self._post(
             PortkeyApiPaths.FEEDBACK_API,
             body=body,
             params=None,
-            cast_to=GenericResponse,
-            stream_cls=Stream[GenericResponse],
+            cast_to=FeedbackResponse,
+            stream_cls=Stream[FeedbackResponse],
             stream=False,
             headers={},
         )
 
-    def bulk_create(self, *, feedbacks: List[Dict[str, Any]]) -> GenericResponse:
+    def bulk_create(self, *, feedbacks: List[Dict[str, Any]]) -> FeedbackResponse:
         body = feedbacks
         return self._post(
             PortkeyApiPaths.FEEDBACK_API,
             body=body,
             params=None,
-            cast_to=GenericResponse,
-            stream_cls=Stream[GenericResponse],
+            cast_to=FeedbackResponse,
+            stream_cls=Stream[FeedbackResponse],
+            stream=False,
+            headers={},
+        )
+
+    def update(
+        self,
+        *,
+        feedback_id: Optional[str] = None,
+        value: Optional[int] = None,
+        weight: Optional[float] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> FeedbackResponse:
+        body = dict(value=value, weight=weight, metadata=metadata)
+
+        return self._put(
+            f"{PortkeyApiPaths.FEEDBACK_API}/{feedback_id}",
+            body=body,
+            params=None,
+            cast_to=FeedbackResponse,
+            stream_cls=Stream[FeedbackResponse],
             stream=False,
             headers={},
         )
 
 
 class AsyncFeedback(AsyncAPIResource):
     def __init__(self, client: AsyncAPIClient) -> None:
@@ -47,31 +68,50 @@
 
     async def create(
         self,
         *,
         trace_id: Optional[str] = None,
         value: Optional[int] = None,
         weight: Optional[float] = None,
-        metadata: Optional[Dict[str, Any]] = None
-    ) -> GenericResponse:
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> FeedbackResponse:
         body = dict(trace_id=trace_id, value=value, weight=weight, metadata=metadata)
         return await self._post(
             PortkeyApiPaths.FEEDBACK_API,
             body=body,
             params=None,
-            cast_to=GenericResponse,
-            stream_cls=AsyncStream[GenericResponse],
+            cast_to=FeedbackResponse,
+            stream_cls=AsyncStream[FeedbackResponse],
             stream=False,
             headers={},
         )
 
-    async def bulk_create(self, *, feedbacks: List[Dict[str, Any]]) -> GenericResponse:
+    async def bulk_create(self, *, feedbacks: List[Dict[str, Any]]) -> FeedbackResponse:
         body = feedbacks
         return await self._post(
             PortkeyApiPaths.FEEDBACK_API,
             body=body,
             params=None,
-            cast_to=GenericResponse,
-            stream_cls=AsyncStream[GenericResponse],
+            cast_to=FeedbackResponse,
+            stream_cls=AsyncStream[FeedbackResponse],
+            stream=False,
+            headers={},
+        )
+
+    async def update(
+        self,
+        *,
+        feedback_id: Optional[str] = None,
+        value: Optional[int] = None,
+        weight: Optional[float] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> FeedbackResponse:
+        body = dict(value=value, weight=weight, metadata=metadata)
+        return await self._put(
+            f"{PortkeyApiPaths.FEEDBACK_API}/{feedback_id}",
+            body=body,
+            params=None,
+            cast_to=FeedbackResponse,
+            stream_cls=Stream[FeedbackResponse],
             stream=False,
             headers={},
         )
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/generation.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/generation.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/images.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/main_files.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/main_files.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,14 +52,30 @@
         response = self.openai_client.files.content(file_id=file_id, **kwargs)
         return response
 
     def retrieve_content(self, file_id, **kwargs) -> Any:
         response = self.openai_client.files.content(file_id=file_id, **kwargs)
         return response
 
+    def wait_for_processing(
+        self,
+        id: str,
+        *,
+        poll_interval: float = 5.0,
+        max_wait_seconds: float = 30 * 60,
+        **kwargs
+    ) -> Any:
+        response = self.openai_client.files.wait_for_processing(
+            id=id,
+            poll_interval=poll_interval,
+            max_wait_seconds=max_wait_seconds,
+            **kwargs
+        )
+        return response
+
 
 class AsyncMainFiles(AsyncAPIResource):
     def __init__(self, client: AsyncPortkey) -> None:
         super().__init__(client)
         self.openai_client = client.openai_client
 
     async def create(self, file, purpose, **kwargs) -> FileObject:
@@ -99,7 +115,23 @@
     async def content(self, file_id, **kwargs) -> Any:
         response = await self.openai_client.files.content(file_id=file_id, **kwargs)
         return response
 
     async def retrieve_content(self, file_id, **kwargs) -> Any:
         response = await self.openai_client.files.content(file_id=file_id, **kwargs)
         return response
+
+    async def wait_for_processing(
+        self,
+        id: str,
+        *,
+        poll_interval: float = 5.0,
+        max_wait_seconds: float = 30 * 60,
+        **kwargs
+    ) -> Any:
+        response = await self.openai_client.files.wait_for_processing(
+            id=id,
+            poll_interval=poll_interval,
+            max_wait_seconds=max_wait_seconds,
+            **kwargs
+        )
+        return response
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/models.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/models.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/apis/post.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/apis/post.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/base_client.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/base_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 
 import json
 from types import TracebackType
 from typing import (
     Dict,
     Any,
+    List,
     Union,
     Mapping,
     cast,
     Optional,
     Type,
     overload,
     Literal,
@@ -49,33 +50,84 @@
         *,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         virtual_key: Optional[str] = None,
         config: Optional[Union[Mapping, str]] = None,
         provider: Optional[str] = None,
         trace_id: Optional[str] = None,
-        metadata: Optional[str] = None,
+        metadata: Union[Optional[dict[str, str]], str] = None,
+        cache_namespace: Optional[str] = None,
+        debug: Optional[bool] = None,
+        cache_force_refresh: Optional[bool] = None,
+        custom_host: Optional[str] = None,
+        forward_headers: Optional[List[str]] = None,
+        openai_project: Optional[str] = None,
+        openai_organization: Optional[str] = None,
+        aws_secret_access_key: Optional[str] = None,
+        aws_access_key_id: Optional[str] = None,
+        aws_session_token: Optional[str] = None,
+        aws_region: Optional[str] = None,
+        vertex_project_id: Optional[str] = None,
+        vertex_region: Optional[str] = None,
+        workers_ai_account_id: Optional[str] = None,
+        azure_resource_name: Optional[str] = None,
+        azure_deployment_id: Optional[str] = None,
+        azure_api_version: Optional[str] = None,
         **kwargs,
     ) -> None:
         self.api_key = api_key or default_api_key()
         self.base_url = base_url or default_base_url()
         self.virtual_key = virtual_key
         self.config = config
         self.provider = provider
         self.trace_id = trace_id
         self.metadata = metadata
+        self.debug = debug
+        self.cache_force_refresh = cache_force_refresh
+        self.custom_host = custom_host
+        self.forward_headers = forward_headers
+        self.openai_project = openai_project
+        self.openai_organization = openai_organization
+        self.aws_secret_access_key = aws_secret_access_key
+        self.aws_access_key_id = aws_access_key_id
+        self.aws_session_token = aws_session_token
+        self.aws_region = aws_region
+        self.vertex_project_id = vertex_project_id
+        self.vertex_region = vertex_region
+        self.workers_ai_account_id = workers_ai_account_id
+        self.azure_resource_name = azure_resource_name
+        self.azure_deployment_id = azure_deployment_id
+        self.azure_api_version = azure_api_version
+        self.cache_namespace = cache_namespace
         self.kwargs = kwargs
 
         self.custom_headers = createHeaders(
             api_key=api_key,
             virtual_key=virtual_key,
             config=config,
             provider=provider,
             trace_id=trace_id,
             metadata=metadata,
+            debug=debug,
+            cache_force_refresh=cache_force_refresh,
+            custom_host=custom_host,
+            forward_headers=forward_headers,
+            openai_project=openai_project,
+            openai_organization=openai_organization,
+            aws_secret_access_key=aws_secret_access_key,
+            aws_access_key_id=aws_access_key_id,
+            aws_session_token=aws_session_token,
+            aws_region=aws_region,
+            vertex_project_id=vertex_project_id,
+            vertex_region=vertex_region,
+            workers_ai_account_id=workers_ai_account_id,
+            azure_resource_name=azure_resource_name,
+            azure_deployment_id=azure_deployment_id,
+            azure_api_version=azure_api_version,
+            cache_namespace=cache_namespace,
             **kwargs,
         )
 
         self.allHeaders = self._build_headers(Options.construct())
         self._client = httpx.Client(
             base_url=self.base_url,
             headers={
@@ -177,14 +229,83 @@
             options=opts,
             stream=stream,
             cast_to=cast_to,
             stream_cls=stream_cls,
         )
         return res
 
+    @overload
+    def _put(
+        self,
+        path: str,
+        *,
+        body: Mapping[str, Any],
+        cast_to: Type[ResponseT],
+        stream: Literal[True],
+        stream_cls: type[StreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> StreamT:
+        ...
+
+    @overload
+    def _put(
+        self,
+        path: str,
+        *,
+        body: Mapping[str, Any],
+        cast_to: Type[ResponseT],
+        stream: Literal[False],
+        stream_cls: type[StreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> ResponseT:
+        ...
+
+    @overload
+    def _put(
+        self,
+        path: str,
+        *,
+        body: Mapping[str, Any],
+        cast_to: Type[ResponseT],
+        stream: bool,
+        stream_cls: type[StreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> Union[ResponseT, StreamT]:
+        ...
+
+    def _put(
+        self,
+        path: str,
+        *,
+        body: Mapping[str, Any],
+        cast_to: Type[ResponseT],
+        stream: bool,
+        stream_cls: type[StreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> Union[ResponseT, StreamT]:
+        opts = self._construct(
+            method="put",
+            url=path,
+            body=body,
+            stream=stream,
+            params=params,
+            headers=headers,
+        )
+        res = self._request(
+            options=opts,
+            stream=stream,
+            cast_to=cast_to,
+            stream_cls=stream_cls,
+        )
+        return res
+
     def _construct_generate_options(
         self,
         *,
         method: str,
         url: str,
         body: Any,
         stream: bool,
@@ -398,33 +519,84 @@
         *,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         virtual_key: Optional[str] = None,
         config: Optional[Union[Mapping, str]] = None,
         provider: Optional[str] = None,
         trace_id: Optional[str] = None,
-        metadata: Optional[str] = None,
+        metadata: Union[Optional[dict[str, str]], str] = None,
+        cache_namespace: Optional[str] = None,
+        debug: Optional[bool] = None,
+        cache_force_refresh: Optional[bool] = None,
+        custom_host: Optional[str] = None,
+        forward_headers: Optional[List[str]] = None,
+        openai_project: Optional[str] = None,
+        openai_organization: Optional[str] = None,
+        aws_secret_access_key: Optional[str] = None,
+        aws_access_key_id: Optional[str] = None,
+        aws_session_token: Optional[str] = None,
+        aws_region: Optional[str] = None,
+        vertex_project_id: Optional[str] = None,
+        vertex_region: Optional[str] = None,
+        workers_ai_account_id: Optional[str] = None,
+        azure_resource_name: Optional[str] = None,
+        azure_deployment_id: Optional[str] = None,
+        azure_api_version: Optional[str] = None,
         **kwargs,
     ) -> None:
         self.api_key = api_key or default_api_key()
         self.base_url = base_url or default_base_url()
         self.virtual_key = virtual_key
         self.config = config
         self.provider = provider
         self.trace_id = trace_id
         self.metadata = metadata
+        self.debug = debug
+        self.cache_force_refresh = cache_force_refresh
+        self.custom_host = custom_host
+        self.forward_headers = forward_headers
+        self.openai_project = openai_project
+        self.openai_organization = openai_organization
+        self.aws_secret_access_key = aws_secret_access_key
+        self.aws_access_key_id = aws_access_key_id
+        self.aws_session_token = aws_session_token
+        self.aws_region = aws_region
+        self.vertex_project_id = vertex_project_id
+        self.vertex_region = vertex_region
+        self.workers_ai_account_id = workers_ai_account_id
+        self.azure_resource_name = azure_resource_name
+        self.azure_deployment_id = azure_deployment_id
+        self.azure_api_version = azure_api_version
+        self.cache_namespace = cache_namespace
         self.kwargs = kwargs
 
         self.custom_headers = createHeaders(
             api_key=api_key,
             virtual_key=virtual_key,
             config=config,
             provider=provider,
             trace_id=trace_id,
             metadata=metadata,
+            debug=debug,
+            cache_force_refresh=cache_force_refresh,
+            custom_host=custom_host,
+            forward_headers=forward_headers,
+            openai_project=openai_project,
+            openai_organization=openai_organization,
+            aws_secret_access_key=aws_secret_access_key,
+            aws_access_key_id=aws_access_key_id,
+            aws_session_token=aws_session_token,
+            aws_region=aws_region,
+            vertex_project_id=vertex_project_id,
+            vertex_region=vertex_region,
+            workers_ai_account_id=workers_ai_account_id,
+            azure_resource_name=azure_resource_name,
+            azure_deployment_id=azure_deployment_id,
+            azure_api_version=azure_api_version,
+            cache_namespace=cache_namespace,
             **kwargs,
         )
 
         self.allHeaders = self._build_headers(Options.construct())
         self._client = AsyncHttpxClientWrapper(
             base_url=self.base_url,
             headers={
@@ -525,14 +697,83 @@
         res = await self._request(
             options=opts,
             stream=stream,
             cast_to=cast_to,
             stream_cls=stream_cls,
         )
         return res
+
+    @overload
+    async def _put(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        body: Mapping[str, Any],
+        stream: Literal[False],
+        stream_cls: type[AsyncStreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> ResponseT:
+        ...
+
+    @overload
+    async def _put(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        body: Mapping[str, Any],
+        stream: Literal[True],
+        stream_cls: type[AsyncStreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> AsyncStreamT:
+        ...
+
+    @overload
+    async def _put(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        body: Mapping[str, Any],
+        stream: bool,
+        stream_cls: type[AsyncStreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> Union[ResponseT, AsyncStreamT]:
+        ...
+
+    async def _put(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        body: Mapping[str, Any],
+        stream: bool,
+        stream_cls: type[AsyncStreamT],
+        params: Mapping[str, str],
+        headers: Mapping[str, str],
+    ) -> Union[ResponseT, AsyncStreamT]:
+        opts = await self._construct(
+            method="put",
+            url=path,
+            body=body,
+            stream=stream,
+            params=params,
+            headers=headers,
+        )
+        res = await self._request(
+            options=opts,
+            stream=stream,
+            cast_to=cast_to,
+            stream_cls=stream_cls,
+        )
+        return res
 
     async def _construct_generate_options(
         self,
         *,
         method: str,
         url: str,
         body: Any,
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/common_types.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/common_types.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/exceptions.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/global_constants.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/global_constants.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/streaming.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/streaming.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/assistant_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/assistant_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from typing import List, Any
 from pydantic import BaseModel, PrivateAttr
 
 __all__ = [
     "Assistant",
     "AssistantList",
     "AssistantDeleted",
-    "AssistantFile",
-    "AssistantFileList",
-    "AssistantFileDeleted",
     "ToolCodeInterpreter",
     "ToolRetrieval",
     "ToolFunction",
     "Tool",
 ]
 
 
@@ -34,15 +31,15 @@
 Tool = Union[ToolCodeInterpreter, ToolRetrieval, ToolFunction]
 
 
 class Assistant(BaseModel):
     id: Optional[str]
     created_at: Optional[int]
     description: Optional[str] = None
-    file_ids: Optional[List[str]]
+    file_ids: Optional[List[str]] = None
     instructions: Optional[str] = None
     metadata: Optional[object] = None
     model: Optional[str]
     name: Optional[str] = None
     object: Optional[str]
     tools: Optional[List[Tool]]
     _headers: Optional[httpx.Headers] = PrivateAttr()
@@ -90,50 +87,50 @@
         del self._headers
         return json.dumps(self.dict(), indent=4)
 
     def get_headers(self) -> Optional[Dict[str, str]]:
         return parse_headers(self._headers)
 
 
-class AssistantFile(BaseModel, extra="allow"):
-    id: Optional[str]
-    assistant_id: Optional[str]
-    created_at: Optional[int]
-    object: Optional[str]
-    _headers: Optional[httpx.Headers] = PrivateAttr()
-
-    def __str__(self):
-        del self._headers
-        return json.dumps(self.dict(), indent=4)
-
-    def get_headers(self) -> Optional[Dict[str, str]]:
-        return parse_headers(self._headers)
-
-
-class AssistantFileList(BaseModel, extra="allow"):
-    object: Optional[str]
-    data: Optional[List[AssistantFile]]
-    first_id: Optional[str]
-    last_id: Optional[str]
-    has_more: Optional[bool]
-    _headers: Optional[httpx.Headers] = PrivateAttr()
-
-    def __str__(self):
-        del self._headers
-        return json.dumps(self.dict(), indent=4)
-
-    def get_headers(self) -> Optional[Dict[str, str]]:
-        return parse_headers(self._headers)
+# class AssistantFile(BaseModel, extra="allow"):
+#     id: Optional[str]
+#     assistant_id: Optional[str]
+#     created_at: Optional[int]
+#     object: Optional[str]
+#     _headers: Optional[httpx.Headers] = PrivateAttr()
+
+#     def __str__(self):
+#         del self._headers
+#         return json.dumps(self.dict(), indent=4)
+
+#     def get_headers(self) -> Optional[Dict[str, str]]:
+#         return parse_headers(self._headers)
+
+
+# class AssistantFileList(BaseModel, extra="allow"):
+#     object: Optional[str]
+#     data: Optional[List[AssistantFile]]
+#     first_id: Optional[str]
+#     last_id: Optional[str]
+#     has_more: Optional[bool]
+#     _headers: Optional[httpx.Headers] = PrivateAttr()
+
+#     def __str__(self):
+#         del self._headers
+#         return json.dumps(self.dict(), indent=4)
+
+#     def get_headers(self) -> Optional[Dict[str, str]]:
+#         return parse_headers(self._headers)
+
+
+# class AssistantFileDeleted(BaseModel, extra="allow"):
+#     id: Optional[str]
+#     deleted: Optional[bool]
+#     object: Optional[str]
+#     _headers: Optional[httpx.Headers] = PrivateAttr()
+
+#     def __str__(self):
+#         del self._headers
+#         return json.dumps(self.dict(), indent=4)
 
-
-class AssistantFileDeleted(BaseModel, extra="allow"):
-    id: Optional[str]
-    deleted: Optional[bool]
-    object: Optional[str]
-    _headers: Optional[httpx.Headers] = PrivateAttr()
-
-    def __str__(self):
-        del self._headers
-        return json.dumps(self.dict(), indent=4)
-
-    def get_headers(self) -> Optional[Dict[str, str]]:
-        return parse_headers(self._headers)
+#     def get_headers(self) -> Optional[Dict[str, str]]:
+#         return parse_headers(self._headers)
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/chat_complete_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/chat_complete_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/complete_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/complete_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/embeddings_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/embeddings_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/generation_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/generation_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 from .utils import parse_headers
 from typing import List, Any
 from pydantic import BaseModel, PrivateAttr
 
 
 class PromptCompletion(BaseModel):
-    id: Optional[str]
-    choices: List[Choice]
-    created: Optional[int]
-    model: Optional[str]
-    object: Optional[str]
+    id: Optional[str] = None
+    choices: Optional[List[Choice]] = None
+    created: Optional[int] = None
+    model: Optional[str] = None
+    object: Optional[str] = None
     system_fingerprint: Optional[str] = None
     usage: Optional[Usage] = None
     index: Optional[int] = None
     text: Optional[str] = None
     logprobs: Optional[Logprobs] = None
     finish_reason: Optional[str] = None
     _headers: Optional[httpx.Headers] = PrivateAttr()
@@ -44,15 +44,15 @@
 
 class PromptCompletionChunk(BaseModel):
     id: Optional[str] = None
     object: Optional[str] = None
     created: Optional[int] = None
     model: Optional[str] = None
     provider: Optional[str] = None
-    choices: Optional[Union[List[TextChoice], List[StreamChoice]]]
+    choices: Optional[Union[List[TextChoice], List[StreamChoice]]] = None
 
     def __str__(self):
         return json.dumps(self.dict(), indent=4)
 
     def __getitem__(self, key):
         return getattr(self, key, None)
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/image_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/image_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/main_file_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/main_file_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/models_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/models_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_message_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_message_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,19 +103,33 @@
         del self._headers
         return json.dumps(self.dict(), indent=4)
 
     def get_headers(self) -> Optional[Dict[str, str]]:
         return parse_headers(self._headers)
 
 
-class MessageFile(BaseModel, extra="allow"):
-    id: Optional[str]
-    object: Optional[str]
-    created_at: Optional[int]
-    message_id: Optional[str]
+# class MessageFile(BaseModel, extra="allow"):
+#     id: Optional[str]
+#     object: Optional[str]
+#     created_at: Optional[int]
+#     message_id: Optional[str]
+#     _headers: Optional[httpx.Headers] = PrivateAttr()
+
+#     def __str__(self):
+#         del self._headers
+#         return json.dumps(self.dict(), indent=4)
+
+#     def get_headers(self) -> Optional[Dict[str, str]]:
+#         return parse_headers(self._headers)
+
+
+class ThreadMessageDeleted(BaseModel):
+    id: str
+    deleted: bool
+    object: str
     _headers: Optional[httpx.Headers] = PrivateAttr()
 
     def __str__(self):
         del self._headers
         return json.dumps(self.dict(), indent=4)
 
     def get_headers(self) -> Optional[Dict[str, str]]:
```

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_run_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_run_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/types/thread_type.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/api_resources/utils.py` & `portkey_ai-1.3.0/portkey_ai/api_resources/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ChatCompletionChunk,
     ChatCompletions,
 )
 from portkey_ai.api_resources.types.complete_type import (
     TextCompletionChunk,
     TextCompletion,
 )
+from portkey_ai.api_resources.types.feedback_type import FeedbackResponse
 from portkey_ai.api_resources.types.generation_type import (
     PromptCompletion,
     PromptCompletionChunk,
     PromptRender,
 )
 from .exceptions import (
     APIStatusError,
@@ -57,15 +58,15 @@
 
 
 CacheLiteral = Literal["semantic", "simple"]
 
 
 ResponseT = TypeVar(
     "ResponseT",
-    bound="Union[ChatCompletionChunk, ChatCompletions, TextCompletion, TextCompletionChunk, GenericResponse, PromptCompletion, PromptCompletionChunk, PromptRender,  httpx.Response]",  # noqa: E501
+    bound="Union[ChatCompletionChunk, ChatCompletions, TextCompletion, TextCompletionChunk, GenericResponse, PromptCompletion, PromptCompletionChunk, PromptRender, FeedbackResponse, httpx.Response]",  # noqa: E501
 )
 
 
 class ProviderTypes(str, Enum):
     """_summary_
 
     Args:
@@ -239,19 +240,35 @@
     virtual_key: Optional[str] = None
     cache: Optional[bool] = None
     cache_age: Optional[int] = None
     cache_status: Optional[Union[CacheType, CacheLiteral]] = None
     cache_force_refresh: Optional[bool] = None
     trace_id: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
+    debug: Optional[bool] = None
+    custom_host: Optional[str] = None
+    forward_headers: Optional[str] = None
     weight: Optional[float] = None
     retry: Optional[RetrySettings] = None
     deployment_id: Optional[str] = None
     resource_name: Optional[str] = None
     api_version: Optional[str] = None
+    openai_project: Optional[str] = None
+    openai_organization: Optional[str] = None
+    aws_secret_access_key: Optional[str] = None
+    aws_access_key_id: Optional[str] = None
+    aws_session_token: Optional[str] = None
+    aws_region: Optional[str] = None
+    vertex_project_id: Optional[str] = None
+    vertex_region: Optional[str] = None
+    workers_ai_account_id: Optional[str] = None
+    azure_resource_name: Optional[str] = None
+    azure_deployment_id: Optional[str] = None
+    azure_api_version: Optional[str] = None
+    cache_namespace: Optional[str] = None
 
 
 class LLMOptions(Constructs, ConversationInput, ModelParams):
     @validator("api_key", "virtual_key", always=False)
     @classmethod
     def parse_api_key(cls, api_key, values):
         if api_key is None and values.get("virtual_key") is None:
```

### Comparing `portkey_ai-1.2.4/portkey_ai/llms/langchain/chat.py` & `portkey_ai-1.3.0/portkey_ai/llms/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/llms/langchain/completion.py` & `portkey_ai-1.3.0/portkey_ai/llms/langchain/completion.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/llms/llama_index/completions.py` & `portkey_ai-1.3.0/portkey_ai/llms/llama_index/completions.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai/llms/llama_index/utils.py` & `portkey_ai-1.3.0/portkey_ai/llms/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/portkey_ai.egg-info/PKG-INFO` & `portkey_ai-1.3.0/portkey_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portkey-ai
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python client library for the Portkey API
 Home-page: https://github.com/Portkey-AI/portkey-python-sdk
 Author: Portkey.ai
 Author-email: support@portkey.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `portkey_ai-1.2.4/portkey_ai.egg-info/SOURCES.txt` & `portkey_ai-1.3.0/portkey_ai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,48 +20,67 @@
 portkey_ai/api_resources/exceptions.py
 portkey_ai/api_resources/global_constants.py
 portkey_ai/api_resources/streaming.py
 portkey_ai/api_resources/utils.py
 portkey_ai/api_resources/apis/__init__.py
 portkey_ai/api_resources/apis/api_resource.py
 portkey_ai/api_resources/apis/assistants.py
+portkey_ai/api_resources/apis/audio.py
+portkey_ai/api_resources/apis/batches.py
 portkey_ai/api_resources/apis/chat_complete.py
 portkey_ai/api_resources/apis/complete.py
 portkey_ai/api_resources/apis/create_headers.py
 portkey_ai/api_resources/apis/embeddings.py
 portkey_ai/api_resources/apis/feedback.py
+portkey_ai/api_resources/apis/fine_tuning.py
 portkey_ai/api_resources/apis/generation.py
 portkey_ai/api_resources/apis/images.py
 portkey_ai/api_resources/apis/main_files.py
 portkey_ai/api_resources/apis/models.py
+portkey_ai/api_resources/apis/moderations.py
 portkey_ai/api_resources/apis/post.py
 portkey_ai/api_resources/apis/threads.py
+portkey_ai/api_resources/apis/vector_stores.py
 portkey_ai/api_resources/types/__init__.py
 portkey_ai/api_resources/types/assistant_type.py
+portkey_ai/api_resources/types/audio_types.py
+portkey_ai/api_resources/types/batches_type.py
 portkey_ai/api_resources/types/chat_complete_type.py
 portkey_ai/api_resources/types/complete_type.py
 portkey_ai/api_resources/types/embeddings_type.py
+portkey_ai/api_resources/types/feedback_type.py
+portkey_ai/api_resources/types/fine_tuning_type.py
 portkey_ai/api_resources/types/generation_type.py
 portkey_ai/api_resources/types/image_type.py
 portkey_ai/api_resources/types/main_file_type.py
 portkey_ai/api_resources/types/models_type.py
+portkey_ai/api_resources/types/moderations_type.py
 portkey_ai/api_resources/types/thread_message_type.py
 portkey_ai/api_resources/types/thread_run_type.py
 portkey_ai/api_resources/types/thread_type.py
 portkey_ai/api_resources/types/utils.py
+portkey_ai/api_resources/types/vector_stores_type.py
 portkey_ai/llms/__init__.py
 portkey_ai/llms/langchain/__init__.py
 portkey_ai/llms/langchain/chat.py
 portkey_ai/llms/langchain/completion.py
 portkey_ai/llms/llama_index/__init__.py
 portkey_ai/llms/llama_index/completions.py
 portkey_ai/llms/llama_index/utils.py
 tests/__init__.py
 tests/test_assistants.py
+tests/test_async_audio_speech.py
+tests/test_async_audio_transcript.py
+tests/test_async_audio_translation.py
 tests/test_async_chat_complete.py
 tests/test_async_complete.py
 tests/test_async_images.py
+tests/test_async_moderations.py
+tests/test_audio_speech.py
+tests/test_audio_transcript.py
+tests/test_audio_translation.py
 tests/test_chat_complete.py
 tests/test_complete.py
 tests/test_images.py
+tests/test_moderations.py
 tests/test_threads.py
 tests/utils.py
```

### Comparing `portkey_ai-1.2.4/setup.cfg` & `portkey_ai-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_assistants.py` & `portkey_ai-1.3.0/tests/test_assistants.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             trace_id=str(uuid4()),
             metadata=metadata,
         )
 
         assistant = portkey.beta.assistants.create(
             model=model,
             description="string",
-            file_ids=["file-m9QiEaDT9Le28LydiUTsUwDv"],
             instructions="You are a personal math tutor."
             + "Write and run code to answer math questions.",
             metadata=metadata,
             name="Math Tutor",
             tools=[{"type": "code_interpreter"}],
         )
```

### Comparing `portkey_ai-1.2.4/tests/test_async_chat_complete.py` & `portkey_ai-1.3.0/tests/test_async_chat_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_async_complete.py` & `portkey_ai-1.3.0/tests/test_async_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_async_images.py` & `portkey_ai-1.3.0/tests/test_async_images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_chat_complete.py` & `portkey_ai-1.3.0/tests/test_chat_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_complete.py` & `portkey_ai-1.3.0/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_images.py` & `portkey_ai-1.3.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.2.4/tests/test_threads.py` & `portkey_ai-1.3.0/tests/test_threads.py`

 * *Files identical despite different names*

