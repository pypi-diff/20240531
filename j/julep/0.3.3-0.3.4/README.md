# Comparing `tmp/julep-0.3.3.tar.gz` & `tmp/julep-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julep-0.3.3.tar", max compression
+gzip compressed data, was "julep-0.3.4.tar", max compression
```

## Comparing `julep-0.3.3.tar` & `julep-0.3.4.tar`

### file list

```diff
@@ -1,111 +1,119 @@
--rw-r--r--   0        0        0      121 2024-04-10 05:56:23.478641 julep-0.3.3/README.md
--rw-r--r--   0        0        0      326 2024-04-10 05:56:23.478641 julep-0.3.3/julep/__init__.py
--rw-r--r--   0        0        0     4431 2024-05-17 12:14:43.020245 julep-0.3.3/julep/api/__init__.py
--rw-r--r--   0        0        0   134843 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/client.py
--rw-r--r--   0        0        0      519 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/__init__.py
--rw-r--r--   0        0        0      440 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/api_error.py
--rw-r--r--   0        0        0      972 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      164 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/environment.py
--rw-r--r--   0        0        0     6816 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/agent.py
--rw-r--r--   0        0        0     3189 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/agent_default_settings.py
--rw-r--r--   0        0        0     1883 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/agent_default_settings_preset.py
--rw-r--r--   0        0        0      136 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/agent_instructions.py
--rw-r--r--   0        0        0      988 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/agent_metadata.py
--rw-r--r--   0        0        0     1675 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_input_data.py
--rw-r--r--   0        0        0      251 2024-04-11 12:32:21.010397 julep-0.3.3/julep/api/types/chat_input_data_tool_choice.py
--rw-r--r--   0        0        0     1530 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/chat_ml_message.py
--rw-r--r--   0        0        0     1062 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/chat_ml_message_role.py
--rw-r--r--   0        0        0     2166 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/chat_response.py
--rw-r--r--   0        0        0     1479 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_response_finish_reason.py
--rw-r--r--   0        0        0     6427 2024-04-17 06:14:33.760319 julep-0.3.3/julep/api/types/chat_settings.py
--rw-r--r--   0        0        0     1787 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_settings_preset.py
--rw-r--r--   0        0        0     2352 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_settings_response_format.py
--rw-r--r--   0        0        0     1037 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_settings_response_format_schema.py
--rw-r--r--   0        0        0      786 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_settings_response_format_type.py
--rw-r--r--   0        0        0      152 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/chat_settings_stop.py
--rw-r--r--   0        0        0     1358 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/completion_usage.py
--rw-r--r--   0        0        0      149 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/create_agent_request_instructions.py
--rw-r--r--   0        0        0     1003 2024-04-15 05:10:46.042449 julep-0.3.3/julep/api/types/create_agent_request_metadata.py
--rw-r--r--   0        0        0     1357 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/create_doc.py
--rw-r--r--   0        0        0      135 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/create_doc_content.py
--rw-r--r--   0        0        0      992 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/create_doc_metadata.py
--rw-r--r--   0        0        0     1003 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/create_session_request_metadata.py
--rw-r--r--   0        0        0     1329 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/create_tool_request.py
--rw-r--r--   0        0        0      646 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/create_tool_request_type.py
--rw-r--r--   0        0        0     1002 2024-04-15 05:10:46.042449 julep-0.3.3/julep/api/types/create_user_request_metadata.py
--rw-r--r--   0        0        0     1442 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/doc.py
--rw-r--r--   0        0        0      129 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/doc_content.py
--rw-r--r--   0        0        0     1014 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/doc_ids.py
--rw-r--r--   0        0        0      986 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/doc_metadata.py
--rw-r--r--   0        0        0     1159 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/function_call_option.py
--rw-r--r--   0        0        0     1493 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/function_def.py
--rw-r--r--   0        0        0      130 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/function_parameters.py
--rw-r--r--   0        0        0      485 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_agent_docs_request_order.py
--rw-r--r--   0        0        0      570 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_agent_docs_request_sort_by.py
--rw-r--r--   0        0        0     1023 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_agent_docs_response.py
--rw-r--r--   0        0        0     1036 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_agent_memories_response.py
--rw-r--r--   0        0        0     1027 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_agent_tools_response.py
--rw-r--r--   0        0        0     1053 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_history_response.py
--rw-r--r--   0        0        0     1046 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_suggestions_response.py
--rw-r--r--   0        0        0      482 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_user_docs_request_order.py
--rw-r--r--   0        0        0      567 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_user_docs_request_sort_by.py
--rw-r--r--   0        0        0     1022 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/get_user_docs_response.py
--rw-r--r--   0        0        0     1615 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/input_chat_ml_message.py
--rw-r--r--   0        0        0     1234 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/input_chat_ml_message_role.py
--rw-r--r--   0        0        0     1819 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/job_status.py
--rw-r--r--   0        0        0     1361 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/job_status_state.py
--rw-r--r--   0        0        0      479 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_agents_request_order.py
--rw-r--r--   0        0        0      564 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_agents_request_sort_by.py
--rw-r--r--   0        0        0     1010 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_agents_response.py
--rw-r--r--   0        0        0      485 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_sessions_request_order.py
--rw-r--r--   0        0        0      570 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_sessions_request_sort_by.py
--rw-r--r--   0        0        0     1018 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_sessions_response.py
--rw-r--r--   0        0        0      476 2024-04-10 05:56:23.478641 julep-0.3.3/julep/api/types/list_users_request_order.py
--rw-r--r--   0        0        0      561 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/list_users_request_sort_by.py
--rw-r--r--   0        0        0     1006 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/list_users_response.py
--rw-r--r--   0        0        0     1907 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/memory.py
--rw-r--r--   0        0        0     1365 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/memory_access_options.py
--rw-r--r--   0        0        0      954 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/memory_entities_item.py
--rw-r--r--   0        0        0     1240 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/named_tool_choice.py
--rw-r--r--   0        0        0     1040 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/named_tool_choice_function.py
--rw-r--r--   0        0        0     1534 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/partial_function_def.py
--rw-r--r--   0        0        0      148 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/patch_agent_request_instructions.py
--rw-r--r--   0        0        0     1000 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/patch_agent_request_metadata.py
--rw-r--r--   0        0        0     1002 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/patch_session_request_metadata.py
--rw-r--r--   0        0        0      999 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/patch_user_request_metadata.py
--rw-r--r--   0        0        0     1143 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/resource_created_response.py
--rw-r--r--   0        0        0     1143 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/resource_deleted_response.py
--rw-r--r--   0        0        0     1143 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/resource_updated_response.py
--rw-r--r--   0        0        0     2107 2024-05-17 12:14:43.030245 julep-0.3.3/julep/api/types/session.py
--rw-r--r--   0        0        0      990 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/session_metadata.py
--rw-r--r--   0        0        0     1502 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/suggestion.py
--rw-r--r--   0        0        0      546 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/suggestion_target.py
--rw-r--r--   0        0        0     1327 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/tool.py
--rw-r--r--   0        0        0       88 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/tool_choice_option.py
--rw-r--r--   0        0        0      607 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/tool_type.py
--rw-r--r--   0        0        0      149 2024-04-26 07:32:15.049340 julep-0.3.3/julep/api/types/update_agent_request_instructions.py
--rw-r--r--   0        0        0     1001 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/update_agent_request_metadata.py
--rw-r--r--   0        0        0     1003 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/update_session_request_metadata.py
--rw-r--r--   0        0        0     1000 2024-04-10 05:56:23.488641 julep-0.3.3/julep/api/types/update_user_request_metadata.py
--rw-r--r--   0        0        0     1559 2024-04-19 07:14:38.007426 julep-0.3.3/julep/api/types/user.py
--rw-r--r--   0        0        0      989 2024-04-19 07:14:38.007426 julep-0.3.3/julep/api/types/user_metadata.py
--rw-r--r--   0        0        0    11638 2024-04-16 04:52:28.980124 julep-0.3.3/julep/client.py
--rw-r--r--   0        0        0      527 2024-04-18 05:50:14.799107 julep-0.3.3/julep/env.py
--rw-r--r--   0        0        0        0 2024-04-10 05:56:23.488641 julep-0.3.3/julep/managers/__init__.py
--rw-r--r--   0        0        0    32129 2024-04-19 07:15:57.797414 julep-0.3.3/julep/managers/agent.py
--rw-r--r--   0        0        0     1249 2024-04-18 05:50:14.799107 julep-0.3.3/julep/managers/base.py
--rw-r--r--   0        0        0    21222 2024-04-26 07:32:15.049340 julep-0.3.3/julep/managers/doc.py
--rw-r--r--   0        0        0     7707 2024-04-18 05:50:14.799107 julep-0.3.3/julep/managers/memory.py
--rw-r--r--   0        0        0    47327 2024-05-17 12:14:43.030245 julep-0.3.3/julep/managers/session.py
--rw-r--r--   0        0        0    18899 2024-04-26 07:32:15.049340 julep-0.3.3/julep/managers/tool.py
--rw-r--r--   0        0        0     1758 2024-04-18 05:50:14.799107 julep-0.3.3/julep/managers/types.py
--rw-r--r--   0        0        0    19731 2024-04-16 09:40:59.218049 julep-0.3.3/julep/managers/user.py
--rw-r--r--   0        0        0     1628 2024-04-18 05:50:14.799107 julep-0.3.3/julep/managers/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 05:56:23.488641 julep-0.3.3/julep/utils/__init__.py
--rw-r--r--   0        0        0    14233 2024-04-18 05:50:14.799107 julep-0.3.3/julep/utils/openai_patch.py
--rw-r--r--   0        0        0     1668 2024-05-17 12:14:43.030245 julep-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-05-07 10:21:57.470948 julep-0.3.4/README.md
+-rw-r--r--   0        0        0      326 2024-05-07 10:21:57.470948 julep-0.3.4/julep/__init__.py
+-rw-r--r--   0        0        0     5281 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/__init__.py
+-rw-r--r--   0        0        0   134755 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/client.py
+-rw-r--r--   0        0        0      519 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      164 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/environment.py
+-rw-r--r--   0        0        0     8009 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/types/__init__.py
+-rw-r--r--   0        0        0     2024 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/agent.py
+-rw-r--r--   0        0        0     3189 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/agent_default_settings.py
+-rw-r--r--   0        0        0     1883 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/agent_default_settings_preset.py
+-rw-r--r--   0        0        0      136 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/agent_instructions.py
+-rw-r--r--   0        0        0      988 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/agent_metadata.py
+-rw-r--r--   0        0        0     1675 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_input_data.py
+-rw-r--r--   0        0        0      251 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/types/chat_input_data_tool_choice.py
+-rw-r--r--   0        0        0     1191 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_image_content_part.py
+-rw-r--r--   0        0        0     1498 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_image_content_part_image_url.py
+-rw-r--r--   0        0        0      771 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_image_content_part_image_url_detail.py
+-rw-r--r--   0        0        0     1605 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_message.py
+-rw-r--r--   0        0        0      228 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/types/chat_ml_message_content.py
+-rw-r--r--   0        0        0      830 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_message_content_item.py
+-rw-r--r--   0        0        0     1062 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/chat_ml_message_role.py
+-rw-r--r--   0        0        0     1022 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/chat_ml_text_content_part.py
+-rw-r--r--   0        0        0     2166 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/chat_response.py
+-rw-r--r--   0        0        0     1479 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_response_finish_reason.py
+-rw-r--r--   0        0        0     6427 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings.py
+-rw-r--r--   0        0        0     1787 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings_preset.py
+-rw-r--r--   0        0        0     2352 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings_response_format.py
+-rw-r--r--   0        0        0     1037 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings_response_format_schema.py
+-rw-r--r--   0        0        0      786 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings_response_format_type.py
+-rw-r--r--   0        0        0      152 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/chat_settings_stop.py
+-rw-r--r--   0        0        0     1358 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/completion_usage.py
+-rw-r--r--   0        0        0      149 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/create_agent_request_instructions.py
+-rw-r--r--   0        0        0     1003 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_agent_request_metadata.py
+-rw-r--r--   0        0        0     1357 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/create_doc.py
+-rw-r--r--   0        0        0      135 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/create_doc_content.py
+-rw-r--r--   0        0        0      992 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_doc_metadata.py
+-rw-r--r--   0        0        0     1003 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_session_request_metadata.py
+-rw-r--r--   0        0        0     1329 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_tool_request.py
+-rw-r--r--   0        0        0      646 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_tool_request_type.py
+-rw-r--r--   0        0        0     1002 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/create_user_request_metadata.py
+-rw-r--r--   0        0        0     1442 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/doc.py
+-rw-r--r--   0        0        0      129 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/doc_content.py
+-rw-r--r--   0        0        0     1014 2024-05-27 00:01:12.039552 julep-0.3.4/julep/api/types/doc_ids.py
+-rw-r--r--   0        0        0      986 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/doc_metadata.py
+-rw-r--r--   0        0        0     1159 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/function_call_option.py
+-rw-r--r--   0        0        0     1493 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/function_def.py
+-rw-r--r--   0        0        0      130 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/function_parameters.py
+-rw-r--r--   0        0        0      485 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_agent_docs_request_order.py
+-rw-r--r--   0        0        0      570 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_agent_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1023 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_agent_docs_response.py
+-rw-r--r--   0        0        0     1036 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_agent_memories_response.py
+-rw-r--r--   0        0        0     1027 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_agent_tools_response.py
+-rw-r--r--   0        0        0     1053 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_history_response.py
+-rw-r--r--   0        0        0     1046 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_suggestions_response.py
+-rw-r--r--   0        0        0      482 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_user_docs_request_order.py
+-rw-r--r--   0        0        0      567 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_user_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1022 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/get_user_docs_response.py
+-rw-r--r--   0        0        0     1706 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/input_chat_ml_message.py
+-rw-r--r--   0        0        0      255 2024-05-30 17:17:10.346542 julep-0.3.4/julep/api/types/input_chat_ml_message_content.py
+-rw-r--r--   0        0        0      855 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/input_chat_ml_message_content_item.py
+-rw-r--r--   0        0        0     1234 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/input_chat_ml_message_role.py
+-rw-r--r--   0        0        0     1819 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/job_status.py
+-rw-r--r--   0        0        0     1361 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/job_status_state.py
+-rw-r--r--   0        0        0      479 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_agents_request_order.py
+-rw-r--r--   0        0        0      564 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_agents_request_sort_by.py
+-rw-r--r--   0        0        0     1010 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_agents_response.py
+-rw-r--r--   0        0        0      485 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_sessions_request_order.py
+-rw-r--r--   0        0        0      570 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_sessions_request_sort_by.py
+-rw-r--r--   0        0        0     1018 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_sessions_response.py
+-rw-r--r--   0        0        0      476 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_users_request_order.py
+-rw-r--r--   0        0        0      561 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_users_request_sort_by.py
+-rw-r--r--   0        0        0     1006 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/list_users_response.py
+-rw-r--r--   0        0        0     1907 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/memory.py
+-rw-r--r--   0        0        0     1365 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/memory_access_options.py
+-rw-r--r--   0        0        0      954 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/memory_entities_item.py
+-rw-r--r--   0        0        0     1349 2024-05-30 01:43:53.723363 julep-0.3.4/julep/api/types/named_tool_choice.py
+-rw-r--r--   0        0        0     1040 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/named_tool_choice_function.py
+-rw-r--r--   0        0        0     1534 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/partial_function_def.py
+-rw-r--r--   0        0        0      148 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/patch_agent_request_instructions.py
+-rw-r--r--   0        0        0     1000 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/patch_agent_request_metadata.py
+-rw-r--r--   0        0        0     1002 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/patch_session_request_metadata.py
+-rw-r--r--   0        0        0      999 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/patch_user_request_metadata.py
+-rw-r--r--   0        0        0     1143 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/resource_created_response.py
+-rw-r--r--   0        0        0     1143 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/resource_deleted_response.py
+-rw-r--r--   0        0        0     1143 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/resource_updated_response.py
+-rw-r--r--   0        0        0     2107 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/session.py
+-rw-r--r--   0        0        0      990 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/session_metadata.py
+-rw-r--r--   0        0        0     1502 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/suggestion.py
+-rw-r--r--   0        0        0      546 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/suggestion_target.py
+-rw-r--r--   0        0        0     1327 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/tool.py
+-rw-r--r--   0        0        0       88 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/tool_choice_option.py
+-rw-r--r--   0        0        0      607 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/tool_type.py
+-rw-r--r--   0        0        0      149 2024-05-27 00:01:08.940572 julep-0.3.4/julep/api/types/update_agent_request_instructions.py
+-rw-r--r--   0        0        0     1001 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/update_agent_request_metadata.py
+-rw-r--r--   0        0        0     1003 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/update_session_request_metadata.py
+-rw-r--r--   0        0        0     1000 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/update_user_request_metadata.py
+-rw-r--r--   0        0        0     1559 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/user.py
+-rw-r--r--   0        0        0      989 2024-05-07 10:21:57.470948 julep-0.3.4/julep/api/types/user_metadata.py
+-rw-r--r--   0        0        0    11638 2024-05-30 17:17:10.346542 julep-0.3.4/julep/client.py
+-rw-r--r--   0        0        0      527 2024-05-07 10:21:57.470948 julep-0.3.4/julep/env.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/__init__.py
+-rw-r--r--   0        0        0    32129 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/agent.py
+-rw-r--r--   0        0        0     1249 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/base.py
+-rw-r--r--   0        0        0    21222 2024-05-27 00:01:08.940572 julep-0.3.4/julep/managers/doc.py
+-rw-r--r--   0        0        0     7707 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/memory.py
+-rw-r--r--   0        0        0    47439 2024-05-30 01:43:53.723363 julep-0.3.4/julep/managers/session.py
+-rw-r--r--   0        0        0    18899 2024-05-27 00:01:08.940572 julep-0.3.4/julep/managers/tool.py
+-rw-r--r--   0        0        0     1758 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/types.py
+-rw-r--r--   0        0        0    19731 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/user.py
+-rw-r--r--   0        0        0     1628 2024-05-07 10:21:57.470948 julep-0.3.4/julep/managers/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:21:57.470948 julep-0.3.4/julep/utils/__init__.py
+-rw-r--r--   0        0        0    14233 2024-05-07 10:21:57.470948 julep-0.3.4/julep/utils/openai_patch.py
+-rw-r--r--   0        0        0     1743 2024-05-31 05:04:22.531868 julep-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.3.4/PKG-INFO
```

### Comparing `julep-0.3.3/julep/api/__init__.py` & `julep-0.3.4/julep/api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,24 @@
     Agent,
     AgentDefaultSettings,
     AgentDefaultSettingsPreset,
     AgentInstructions,
     AgentMetadata,
     ChatInputData,
     ChatInputDataToolChoice,
+    ChatMlImageContentPart,
+    ChatMlImageContentPartImageUrl,
+    ChatMlImageContentPartImageUrlDetail,
     ChatMlMessage,
+    ChatMlMessageContent,
+    ChatMlMessageContentItem,
+    ChatMlMessageContentItem_ImageUrl,
+    ChatMlMessageContentItem_Text,
     ChatMlMessageRole,
+    ChatMlTextContentPart,
     ChatResponse,
     ChatResponseFinishReason,
     ChatSettings,
     ChatSettingsPreset,
     ChatSettingsResponseFormat,
     ChatSettingsResponseFormatSchema,
     ChatSettingsResponseFormatType,
@@ -42,14 +50,18 @@
     GetAgentToolsResponse,
     GetHistoryResponse,
     GetSuggestionsResponse,
     GetUserDocsRequestOrder,
     GetUserDocsRequestSortBy,
     GetUserDocsResponse,
     InputChatMlMessage,
+    InputChatMlMessageContent,
+    InputChatMlMessageContentItem,
+    InputChatMlMessageContentItem_ImageUrl,
+    InputChatMlMessageContentItem_Text,
     InputChatMlMessageRole,
     JobStatus,
     JobStatusState,
     ListAgentsRequestOrder,
     ListAgentsRequestSortBy,
     ListAgentsResponse,
     ListSessionsRequestOrder,
@@ -91,16 +103,24 @@
     "Agent",
     "AgentDefaultSettings",
     "AgentDefaultSettingsPreset",
     "AgentInstructions",
     "AgentMetadata",
     "ChatInputData",
     "ChatInputDataToolChoice",
+    "ChatMlImageContentPart",
+    "ChatMlImageContentPartImageUrl",
+    "ChatMlImageContentPartImageUrlDetail",
     "ChatMlMessage",
+    "ChatMlMessageContent",
+    "ChatMlMessageContentItem",
+    "ChatMlMessageContentItem_ImageUrl",
+    "ChatMlMessageContentItem_Text",
     "ChatMlMessageRole",
+    "ChatMlTextContentPart",
     "ChatResponse",
     "ChatResponseFinishReason",
     "ChatSettings",
     "ChatSettingsPreset",
     "ChatSettingsResponseFormat",
     "ChatSettingsResponseFormatSchema",
     "ChatSettingsResponseFormatType",
@@ -129,14 +149,18 @@
     "GetAgentToolsResponse",
     "GetHistoryResponse",
     "GetSuggestionsResponse",
     "GetUserDocsRequestOrder",
     "GetUserDocsRequestSortBy",
     "GetUserDocsResponse",
     "InputChatMlMessage",
+    "InputChatMlMessageContent",
+    "InputChatMlMessageContentItem",
+    "InputChatMlMessageContentItem_ImageUrl",
+    "InputChatMlMessageContentItem_Text",
     "InputChatMlMessageRole",
     "JobStatus",
     "JobStatusState",
     "JulepApiEnvironment",
     "ListAgentsRequestOrder",
     "ListAgentsRequestSortBy",
     "ListAgentsResponse",
```

### Comparing `julep-0.3.3/julep/api/client.py` & `julep-0.3.4/julep/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,19 +786,17 @@
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.chat(
             session_id="session_id",
-            min_p=0.01,
             messages=[
                 InputChatMlMessage(
                     role=InputChatMlMessageRole.USER,
-                    content="content",
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"messages": messages}
         if tools is not OMIT:
             _request["tools"] = tools
@@ -827,15 +825,15 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if min_p is not OMIT:
             _request["min_p"] = min_p
         if preset is not OMIT:
-            _request["preset"] = preset.value  # type: ignore
+            _request["preset"] = preset.value  # pytype: disable=attribute-error
         if recall is not OMIT:
             _request["recall"] = recall
         if record is not OMIT:
             _request["record"] = record
         if remember is not OMIT:
             _request["remember"] = remember
         _response = self._client_wrapper.httpx_client.request(
@@ -2549,19 +2547,17 @@
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.chat(
             session_id="session_id",
-            min_p=0.01,
             messages=[
                 InputChatMlMessage(
                     role=InputChatMlMessageRole.USER,
-                    content="content",
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"messages": messages}
         if tools is not OMIT:
             _request["tools"] = tools
@@ -2590,15 +2586,15 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if min_p is not OMIT:
             _request["min_p"] = min_p
         if preset is not OMIT:
-            _request["preset"] = preset.value  # type: ignore
+            _request["preset"] = preset.value  # pytype: disable=attribute-error
         if recall is not OMIT:
             _request["recall"] = recall
         if record is not OMIT:
             _request["record"] = record
         if remember is not OMIT:
             _request["remember"] = remember
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `julep-0.3.3/julep/api/core/__init__.py` & `julep-0.3.4/julep/api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/core/client_wrapper.py` & `julep-0.3.4/julep/api/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/core/datetime_utils.py` & `julep-0.3.4/julep/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/core/jsonable_encoder.py` & `julep-0.3.4/julep/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/__init__.py` & `julep-0.3.4/julep/api/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,28 @@
 from .agent import Agent
 from .agent_default_settings import AgentDefaultSettings
 from .agent_default_settings_preset import AgentDefaultSettingsPreset
 from .agent_instructions import AgentInstructions
 from .agent_metadata import AgentMetadata
 from .chat_input_data import ChatInputData
 from .chat_input_data_tool_choice import ChatInputDataToolChoice
+from .chat_ml_image_content_part import ChatMlImageContentPart
+from .chat_ml_image_content_part_image_url import ChatMlImageContentPartImageUrl
+from .chat_ml_image_content_part_image_url_detail import (
+    ChatMlImageContentPartImageUrlDetail,
+)
 from .chat_ml_message import ChatMlMessage
+from .chat_ml_message_content import ChatMlMessageContent
+from .chat_ml_message_content_item import (
+    ChatMlMessageContentItem,
+    ChatMlMessageContentItem_ImageUrl,
+    ChatMlMessageContentItem_Text,
+)
 from .chat_ml_message_role import ChatMlMessageRole
+from .chat_ml_text_content_part import ChatMlTextContentPart
 from .chat_response import ChatResponse
 from .chat_response_finish_reason import ChatResponseFinishReason
 from .chat_settings import ChatSettings
 from .chat_settings_preset import ChatSettingsPreset
 from .chat_settings_response_format import ChatSettingsResponseFormat
 from .chat_settings_response_format_schema import ChatSettingsResponseFormatSchema
 from .chat_settings_response_format_type import ChatSettingsResponseFormatType
@@ -41,14 +53,20 @@
 from .get_agent_tools_response import GetAgentToolsResponse
 from .get_history_response import GetHistoryResponse
 from .get_suggestions_response import GetSuggestionsResponse
 from .get_user_docs_request_order import GetUserDocsRequestOrder
 from .get_user_docs_request_sort_by import GetUserDocsRequestSortBy
 from .get_user_docs_response import GetUserDocsResponse
 from .input_chat_ml_message import InputChatMlMessage
+from .input_chat_ml_message_content import InputChatMlMessageContent
+from .input_chat_ml_message_content_item import (
+    InputChatMlMessageContentItem,
+    InputChatMlMessageContentItem_ImageUrl,
+    InputChatMlMessageContentItem_Text,
+)
 from .input_chat_ml_message_role import InputChatMlMessageRole
 from .job_status import JobStatus
 from .job_status_state import JobStatusState
 from .list_agents_request_order import ListAgentsRequestOrder
 from .list_agents_request_sort_by import ListAgentsRequestSortBy
 from .list_agents_response import ListAgentsResponse
 from .list_sessions_request_order import ListSessionsRequestOrder
@@ -88,16 +106,24 @@
     "Agent",
     "AgentDefaultSettings",
     "AgentDefaultSettingsPreset",
     "AgentInstructions",
     "AgentMetadata",
     "ChatInputData",
     "ChatInputDataToolChoice",
+    "ChatMlImageContentPart",
+    "ChatMlImageContentPartImageUrl",
+    "ChatMlImageContentPartImageUrlDetail",
     "ChatMlMessage",
+    "ChatMlMessageContent",
+    "ChatMlMessageContentItem",
+    "ChatMlMessageContentItem_ImageUrl",
+    "ChatMlMessageContentItem_Text",
     "ChatMlMessageRole",
+    "ChatMlTextContentPart",
     "ChatResponse",
     "ChatResponseFinishReason",
     "ChatSettings",
     "ChatSettingsPreset",
     "ChatSettingsResponseFormat",
     "ChatSettingsResponseFormatSchema",
     "ChatSettingsResponseFormatType",
@@ -126,14 +152,18 @@
     "GetAgentToolsResponse",
     "GetHistoryResponse",
     "GetSuggestionsResponse",
     "GetUserDocsRequestOrder",
     "GetUserDocsRequestSortBy",
     "GetUserDocsResponse",
     "InputChatMlMessage",
+    "InputChatMlMessageContent",
+    "InputChatMlMessageContentItem",
+    "InputChatMlMessageContentItem_ImageUrl",
+    "InputChatMlMessageContentItem_Text",
     "InputChatMlMessageRole",
     "JobStatus",
     "JobStatusState",
     "ListAgentsRequestOrder",
     "ListAgentsRequestSortBy",
     "ListAgentsResponse",
     "ListSessionsRequestOrder",
```

### Comparing `julep-0.3.3/julep/api/types/agent.py` & `julep-0.3.4/julep/api/types/agent.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/agent_default_settings.py` & `julep-0.3.4/julep/api/types/agent_default_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/agent_default_settings_preset.py` & `julep-0.3.4/julep/api/types/agent_default_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/agent_metadata.py` & `julep-0.3.4/julep/api/types/agent_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_input_data.py` & `julep-0.3.4/julep/api/types/chat_input_data.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_ml_message.py` & `julep-0.3.4/julep/api/types/chat_ml_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .chat_ml_message_content import ChatMlMessageContent
 from .chat_ml_message_role import ChatMlMessageRole
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -18,15 +19,15 @@
             "ChatML role (system\n"
             "assistant\n"
             "user\n"
             "function_call\n"
             "function)\n"
         )
     )
-    content: str = pydantic.Field(description="ChatML content")
+    content: ChatMlMessageContent = pydantic.Field(description="ChatML content")
     name: typing.Optional[str] = pydantic.Field(description="ChatML name")
     created_at: dt.datetime = pydantic.Field(
         description="Message created at (RFC-3339 format)"
     )
     id: str = pydantic.Field(description="Message ID")
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `julep-0.3.3/julep/api/types/chat_ml_message_role.py` & `julep-0.3.4/julep/api/types/chat_ml_message_role.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_response.py` & `julep-0.3.4/julep/api/types/chat_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_response_finish_reason.py` & `julep-0.3.4/julep/api/types/chat_response_finish_reason.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_settings.py` & `julep-0.3.4/julep/api/types/chat_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_settings_preset.py` & `julep-0.3.4/julep/api/types/chat_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_settings_response_format.py` & `julep-0.3.4/julep/api/types/chat_settings_response_format.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_settings_response_format_schema.py` & `julep-0.3.4/julep/api/types/chat_settings_response_format_schema.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/chat_settings_response_format_type.py` & `julep-0.3.4/julep/api/types/chat_settings_response_format_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/completion_usage.py` & `julep-0.3.4/julep/api/types/completion_usage.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_agent_request_metadata.py` & `julep-0.3.4/julep/api/types/create_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_doc.py` & `julep-0.3.4/julep/api/types/create_doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_doc_metadata.py` & `julep-0.3.4/julep/api/types/create_doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_session_request_metadata.py` & `julep-0.3.4/julep/api/types/create_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_tool_request.py` & `julep-0.3.4/julep/api/types/create_tool_request.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_tool_request_type.py` & `julep-0.3.4/julep/api/types/create_tool_request_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/create_user_request_metadata.py` & `julep-0.3.4/julep/api/types/create_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/doc.py` & `julep-0.3.4/julep/api/types/doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/doc_ids.py` & `julep-0.3.4/julep/api/types/doc_ids.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/doc_metadata.py` & `julep-0.3.4/julep/api/types/doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/function_call_option.py` & `julep-0.3.4/julep/api/types/function_call_option.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/function_def.py` & `julep-0.3.4/julep/api/types/function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_agent_docs_request_sort_by.py` & `julep-0.3.4/julep/api/types/get_agent_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_agent_docs_response.py` & `julep-0.3.4/julep/api/types/get_agent_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_agent_memories_response.py` & `julep-0.3.4/julep/api/types/get_agent_memories_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_agent_tools_response.py` & `julep-0.3.4/julep/api/types/get_agent_tools_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_history_response.py` & `julep-0.3.4/julep/api/types/get_history_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_suggestions_response.py` & `julep-0.3.4/julep/api/types/get_suggestions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_user_docs_request_sort_by.py` & `julep-0.3.4/julep/api/types/get_user_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/get_user_docs_response.py` & `julep-0.3.4/julep/api/types/get_user_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/input_chat_ml_message.py` & `julep-0.3.4/julep/api/types/input_chat_ml_message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .input_chat_ml_message_content import InputChatMlMessageContent
 from .input_chat_ml_message_role import InputChatMlMessageRole
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -19,15 +20,15 @@
             "assistant\n"
             "user\n"
             "function_call\n"
             "function\n"
             "auto)\n"
         )
     )
-    content: str = pydantic.Field(description="ChatML content")
+    content: InputChatMlMessageContent = pydantic.Field(description="ChatML content")
     name: typing.Optional[str] = pydantic.Field(description="ChatML name")
     continue_: typing.Optional[bool] = pydantic.Field(
         alias="continue",
         description="Whether to continue this message or return a new one",
     )
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `julep-0.3.3/julep/api/types/input_chat_ml_message_role.py` & `julep-0.3.4/julep/api/types/input_chat_ml_message_role.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/job_status.py` & `julep-0.3.4/julep/api/types/job_status.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/job_status_state.py` & `julep-0.3.4/julep/api/types/job_status_state.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_agents_request_sort_by.py` & `julep-0.3.4/julep/api/types/list_agents_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_agents_response.py` & `julep-0.3.4/julep/api/types/list_agents_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_sessions_request_sort_by.py` & `julep-0.3.4/julep/api/types/list_sessions_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_sessions_response.py` & `julep-0.3.4/julep/api/types/list_sessions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_users_request_sort_by.py` & `julep-0.3.4/julep/api/types/list_users_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/list_users_response.py` & `julep-0.3.4/julep/api/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/memory.py` & `julep-0.3.4/julep/api/types/memory.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/memory_access_options.py` & `julep-0.3.4/julep/api/types/memory_access_options.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/memory_entities_item.py` & `julep-0.3.4/julep/api/types/memory_entities_item.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/named_tool_choice.py` & `julep-0.3.4/julep/api/types/named_tool_choice.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 class NamedToolChoice(pydantic.BaseModel):
     """
     Specifies a tool the model should use. Use to force the model to call a specific function.
     """
 
-    type: typing_extensions.Literal["function"]
+    type: typing_extensions.Literal["function"] = pydantic.Field(
+        description="The type of the tool. Currently, only `function` is supported."
+    )
     function: NamedToolChoiceFunction
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.3.3/julep/api/types/named_tool_choice_function.py` & `julep-0.3.4/julep/api/types/named_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/partial_function_def.py` & `julep-0.3.4/julep/api/types/partial_function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/patch_agent_request_metadata.py` & `julep-0.3.4/julep/api/types/patch_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/patch_session_request_metadata.py` & `julep-0.3.4/julep/api/types/patch_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/patch_user_request_metadata.py` & `julep-0.3.4/julep/api/types/patch_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/resource_created_response.py` & `julep-0.3.4/julep/api/types/resource_created_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/resource_deleted_response.py` & `julep-0.3.4/julep/api/types/resource_deleted_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/resource_updated_response.py` & `julep-0.3.4/julep/api/types/resource_updated_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/session.py` & `julep-0.3.4/julep/api/types/session.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/session_metadata.py` & `julep-0.3.4/julep/api/types/session_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/suggestion.py` & `julep-0.3.4/julep/api/types/suggestion.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/suggestion_target.py` & `julep-0.3.4/julep/api/types/suggestion_target.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/tool.py` & `julep-0.3.4/julep/api/types/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/tool_type.py` & `julep-0.3.4/julep/api/types/tool_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/update_agent_request_metadata.py` & `julep-0.3.4/julep/api/types/update_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/update_session_request_metadata.py` & `julep-0.3.4/julep/api/types/update_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/update_user_request_metadata.py` & `julep-0.3.4/julep/api/types/update_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/user.py` & `julep-0.3.4/julep/api/types/user.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/api/types/user_metadata.py` & `julep-0.3.4/julep/api/types/user_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/client.py` & `julep-0.3.4/julep/client.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/env.py` & `julep-0.3.4/julep/env.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/agent.py` & `julep-0.3.4/julep/managers/agent.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/base.py` & `julep-0.3.4/julep/managers/base.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/doc.py` & `julep-0.3.4/julep/managers/doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/memory.py` & `julep-0.3.4/julep/managers/memory.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/session.py` & `julep-0.3.4/julep/managers/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,20 @@
 
         Note:
             The precise types of some arguments, like `Tool`, `ToolChoiceOption`, `ChatSettingsResponseFormat`, and `ChatSettingsStop`, are not defined within the given context. It's assumed that these types have been defined elsewhere in the code base.
 
         Raises:
             It is not specified what exceptions this function might raise. Typically, one would expect potential exceptions to be associated with the underlying API client's `chat` method failure modes, such as network issues, invalid parameters, etc.
         """
+        if recall is None:
+            recall = True
+
+        if remember is None:
+            remember = True
+
         return self.api_client.chat(
             session_id=session_id,
             messages=messages,
             tools=tools,
             tool_choice=tool_choice,
             frequency_penalty=frequency_penalty,
             length_penalty=length_penalty,
```

### Comparing `julep-0.3.3/julep/managers/tool.py` & `julep-0.3.4/julep/managers/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/types.py` & `julep-0.3.4/julep/managers/types.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/user.py` & `julep-0.3.4/julep/managers/user.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/managers/utils.py` & `julep-0.3.4/julep/managers/utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/julep/utils/openai_patch.py` & `julep-0.3.4/julep/utils/openai_patch.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.3/pyproject.toml` & `julep-0.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "julep"
-version = "0.3.3"
+version = "0.3.4"
 description = "Julep is a platform for creating agents with long-term memory"
 authors = ["Julep Developers <developers@julep.ai>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
@@ -22,14 +22,15 @@
 ward = "^0.68.0b0"
 ruff = "^0.1.13"
 poethepoet = "^0.25.1"
 ipython = "<8.13"
 pyright = "^1.1.348"
 handsdown = "^2.1.0"
 jupyterlab = "^4.1.0"
+pycozo = {extras = ["embedded", "pandas", "requests"], version = "^0.7.6"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 format = "black ."
```

### Comparing `julep-0.3.3/PKG-INFO` & `julep-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julep
-Version: 0.3.3
+Version: 0.3.4
 Summary: Julep is a platform for creating agents with long-term memory
 License: ISC
 Author: Julep Developers
 Author-email: developers@julep.ai
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

