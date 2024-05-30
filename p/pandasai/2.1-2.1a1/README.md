# Comparing `tmp/pandasai-2.1.tar.gz` & `tmp/pandasai-2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-2.1.tar", max compression
+gzip compressed data, was "pandasai-2.1a1.tar", max compression
```

## Comparing `pandasai-2.1.tar` & `pandasai-2.1a1.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0     1581 2024-05-30 22:59:21.773162 pandasai-2.1/LICENSE
--rw-r--r--   0        0        0     5825 2024-05-30 22:59:21.773162 pandasai-2.1/README.md
--rw-r--r--   0        0        0      694 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/__init__.py
--rw-r--r--   0        0        0       87 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/agent/__init__.py
--rw-r--r--   0        0        0     1845 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/agent/agent.py
--rw-r--r--   0        0        0    15764 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/agent/base.py
--rw-r--r--   0        0        0      998 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/agent/callbacks.py
--rw-r--r--   0        0        0     1350 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/config.py
--rw-r--r--   0        0        0      749 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/__init__.py
--rw-r--r--   0        0        0     8777 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/airtable.py
--rw-r--r--   0        0        0     8477 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/base.py
--rw-r--r--   0        0        0     5238 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/pandas.py
--rw-r--r--   0        0        0     4653 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/polars.py
--rw-r--r--   0        0        0    21412 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/sql.py
--rw-r--r--   0        0        0     5871 2024-05-30 22:59:21.777162 pandasai-2.1/pandasai/connectors/yahoo_finance.py
--rw-r--r--   0        0        0     2138 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/constants.py
--rw-r--r--   0        0        0     2183 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/LICENSE
--rw-r--r--   0        0        0     5387 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/__init__.py
--rw-r--r--   0        0        0     1448 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/Semantic_prompt_generation.py
--rw-r--r--   0        0        0     6296 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/code_generator.py
--rw-r--r--   0        0        0     1790 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_correction_pipeline.py
--rw-r--r--   0        0        0     3213 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py
--rw-r--r--   0        0        0     1941 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/llm_call.py
--rw-r--r--   0        0        0     2764 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/semantic_chat_pipeline.py
--rw-r--r--   0        0        0     2411 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/validate_pipeline_input.py
--rw-r--r--   0        0        0     1732 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/generate_df_schema.py
--rw-r--r--   0        0        0     1193 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/semantic_agent_prompt.py
--rw-r--r--   0        0        0     3289 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/templates/generate_df_schema.tmpl
--rw-r--r--   0        0        0       83 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/templates/semantic_agent_prompt.tmpl
--rw-r--r--   0        0        0       91 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/templates/shared/dataframe.tmpl
--rw-r--r--   0        0        0      418 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/connectors/__init__.py
--rw-r--r--   0        0        0     2835 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/connectors/databricks.py
--rw-r--r--   0        0        0     3449 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/connectors/google_big_query.py
--rw-r--r--   0        0        0      660 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/connectors/relations.py
--rw-r--r--   0        0        0     3862 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/connectors/snowflake.py
--rw-r--r--   0        0        0    15531 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/helpers/query_builder.py
--rw-r--r--   0        0        0      148 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/vectorstores/__init__.py
--rw-r--r--   0        0        0    10445 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/vectorstores/chroma.py
--rw-r--r--   0        0        0    10514 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/vectorstores/pinecone.py
--rw-r--r--   0        0        0    14109 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/ee/vectorstores/qdrant.py
--rw-r--r--   0        0        0      507 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/engine.py
--rw-r--r--   0        0        0     5665 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/exceptions.py
--rw-r--r--   0        0        0      446 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4613 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     3020 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0     2397 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/data_sampler.py
--rw-r--r--   0        0        0     5557 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/dataframe_serializer.py
--rw-r--r--   0        0        0     5062 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/df_config_manager.py
--rw-r--r--   0        0        0     1378 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/df_info.py
--rw-r--r--   0        0        0     3244 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/df_validator.py
--rw-r--r--   0        0        0      291 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/encoder.py
--rw-r--r--   0        0        0      526 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/env.py
--rw-r--r--   0        0        0      937 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/file_importer.py
--rw-r--r--   0        0        0      725 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/folder.py
--rw-r--r--   0        0        0     3717 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     4282 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/logger.py
--rw-r--r--   0        0        0     3415 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/memory.py
--rw-r--r--   0        0        0      447 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/node_visitors.py
--rw-r--r--   0        0        0      213 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/openai.py
--rw-r--r--   0        0        0     6147 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     4813 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/optional.py
--rw-r--r--   0        0        0     1976 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/output_types/__init__.py
--rw-r--r--   0        0        0     4658 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/output_types/_output_types.py
--rw-r--r--   0        0        0     3708 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/output_validator.py
--rw-r--r--   0        0        0     2074 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/path.py
--rw-r--r--   0        0        0     8773 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/query_exec_tracker.py
--rw-r--r--   0        0        0     2426 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/request.py
--rw-r--r--   0        0        0     1061 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     8579 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     2388 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/skills_manager.py
--rw-r--r--   0        0        0      306 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/helpers/sql.py
--rw-r--r--   0        0        0      629 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     7002 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0      624 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/bamboo_llm.py
--rw-r--r--   0        0        0    13479 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/base.py
--rw-r--r--   0        0        0     5543 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/bedrock_claude.py
--rw-r--r--   0        0        0      640 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     2974 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/google_gemini.py
--rw-r--r--   0        0        0     2757 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     5697 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/google_vertexai.py
--rw-r--r--   0        0        0     4003 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/huggingface_text_gen.py
--rw-r--r--   0        0        0     5408 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/ibm_watsonx.py
--rw-r--r--   0        0        0     1611 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1419 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/local_llm.py
--rw-r--r--   0        0        0     3403 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0      352 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pandas/__init__.py
--rw-r--r--   0        0        0      206 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/__init__.py
--rw-r--r--   0        0        0      353 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/abstract_pipeline.py
--rw-r--r--   0        0        0     1062 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/base_logic_unit.py
--rw-r--r--   0        0        0     1438 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/chat/cache_lookup.py
--rw-r--r--   0        0        0     1253 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/chat/cache_population.py
--rw-r--r--   0        0        0      572 2024-05-30 22:59:21.781162 pandasai-2.1/pandasai/pipelines/chat/chat_pipeline_input.py
--rw-r--r--   0        0        0    18734 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/code_cleaning.py
--rw-r--r--   0        0        0    15802 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/code_execution.py
--rw-r--r--   0        0        0      626 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/code_execution_pipeline_input.py
--rw-r--r--   0        0        0     1473 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/code_generator.py
--rw-r--r--   0        0        0     1638 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
--rw-r--r--   0        0        0      240 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
--rw-r--r--   0        0        0     3213 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
--rw-r--r--   0        0        0    10679 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/generate_chat_pipeline.py
--rw-r--r--   0        0        0     2258 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/prompt_generation.py
--rw-r--r--   0        0        0     2157 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/result_parsing.py
--rw-r--r--   0        0        0     1828 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/result_validation.py
--rw-r--r--   0        0        0     2025 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/chat/validate_pipeline_input.py
--rw-r--r--   0        0        0      612 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/logic_unit_output.py
--rw-r--r--   0        0        0      422 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/logic_units/code_executor.py
--rw-r--r--   0        0        0      900 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/logic_units/output_logic_unit.py
--rw-r--r--   0        0        0      511 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/logic_units/prompt_execution.py
--rw-r--r--   0        0        0     5833 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/pipeline.py
--rw-r--r--   0        0        0     1707 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pipelines/pipeline_context.py
--rw-r--r--   0        0        0      232 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     2098 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0      207 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/check_if_relevant_to_conversation.py
--rw-r--r--   0        0        0      518 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/clarification_questions_prompt.py
--rw-r--r--   0        0        0      902 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0      975 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
--rw-r--r--   0        0        0     1058 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/correct_output_type_error_prompt.py
--rw-r--r--   0        0        0     1904 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/direct_sql_prompt.py
--rw-r--r--   0        0        0      159 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/explain_prompt.py
--rw-r--r--   0        0        0     1274 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/file_based_prompt.py
--rw-r--r--   0        0        0      919 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      268 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/generate_python_code_with_sql.py
--rw-r--r--   0        0        0      189 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/generate_system_message.py
--rw-r--r--   0        0        0      172 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/rephase_query_prompt.py
--rw-r--r--   0        0        0      199 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
--rw-r--r--   0        0        0      571 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/clarification_questions_prompt.tmpl
--rw-r--r--   0        0        0      342 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/correct_error_prompt.tmpl
--rw-r--r--   0        0        0      356 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
--rw-r--r--   0        0        0      343 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
--rw-r--r--   0        0        0      325 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/explain.tmpl
--rw-r--r--   0        0        0      923 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/generate_python_code.tmpl
--rw-r--r--   0        0        0     1311 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
--rw-r--r--   0        0        0      176 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/generate_system_message.tmpl
--rw-r--r--   0        0        0      387 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/rephrase_query.tmpl
--rw-r--r--   0        0        0      123 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/shared/dataframe.tmpl
--rw-r--r--   0        0        0      916 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/shared/output_type_template.tmpl
--rw-r--r--   0        0        0      624 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/prompts/templates/shared/vectordb_docs.tmpl
--rw-r--r--   0        0        0      102 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/pydantic/__init__.py
--rw-r--r--   0        0        0      311 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/__init__.py
--rw-r--r--   0        0        0      637 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/context.py
--rw-r--r--   0        0        0     2159 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/response_parser.py
--rw-r--r--   0        0        0     1593 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/response_serializer.py
--rw-r--r--   0        0        0       96 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/response_type.py
--rw-r--r--   0        0        0     1036 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/responses/streamlit_response.py
--rw-r--r--   0        0        0       16 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/schemas/__init__.py
--rw-r--r--   0        0        0     1305 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/schemas/df_config.py
--rw-r--r--   0        0        0     3920 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/skills/__init__.py
--rw-r--r--   0        0        0     8894 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/smart_dataframe/__init__.py
--rw-r--r--   0        0        0     6256 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/smart_datalake/__init__.py
--rw-r--r--   0        0        0      193 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/vectorstores/__init__.py
--rw-r--r--   0        0        0     2705 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/vectorstores/bamboo_vectorstore.py
--rw-r--r--   0        0        0     5764 2024-05-30 22:59:21.785162 pandasai-2.1/pandasai/vectorstores/vectorstore.py
--rw-r--r--   0        0        0     3937 2024-05-30 22:59:21.789162 pandasai-2.1/pyproject.toml
--rw-r--r--   0        0        0     9734 1970-01-01 00:00:00.000000 pandasai-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1581 2024-02-29 15:48:26.870599 pandasai-2.1a1/LICENSE
+-rw-r--r--   0        0        0     5825 2024-05-19 03:18:51.906754 pandasai-2.1a1/README.md
+-rw-r--r--   0        0        0      694 2024-04-06 09:34:15.901079 pandasai-2.1a1/pandasai/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-23 12:39:50.244054 pandasai-2.1a1/pandasai/agent/__init__.py
+-rw-r--r--   0        0        0     1845 2024-05-23 12:39:50.244348 pandasai-2.1a1/pandasai/agent/agent.py
+-rw-r--r--   0        0        0    15764 2024-05-23 12:39:50.244732 pandasai-2.1a1/pandasai/agent/base.py
+-rw-r--r--   0        0        0      998 2024-03-26 00:39:20.878687 pandasai-2.1a1/pandasai/agent/callbacks.py
+-rw-r--r--   0        0        0     1350 2024-03-26 00:39:17.325195 pandasai-2.1a1/pandasai/config.py
+-rw-r--r--   0        0        0      749 2024-05-18 23:37:12.274645 pandasai-2.1a1/pandasai/connectors/__init__.py
+-rw-r--r--   0        0        0     8777 2024-03-15 21:22:46.070796 pandasai-2.1a1/pandasai/connectors/airtable.py
+-rw-r--r--   0        0        0     8477 2024-05-23 12:39:50.245442 pandasai-2.1a1/pandasai/connectors/base.py
+-rw-r--r--   0        0        0     5235 2024-05-23 12:39:50.245662 pandasai-2.1a1/pandasai/connectors/pandas.py
+-rw-r--r--   0        0        0     4653 2024-03-09 00:53:54.916215 pandasai-2.1a1/pandasai/connectors/polars.py
+-rw-r--r--   0        0        0    21412 2024-05-23 12:39:50.246483 pandasai-2.1a1/pandasai/connectors/sql.py
+-rw-r--r--   0        0        0     5871 2024-02-29 15:48:26.887142 pandasai-2.1a1/pandasai/connectors/yahoo_finance.py
+-rw-r--r--   0        0        0     2138 2024-05-23 12:39:50.247070 pandasai-2.1a1/pandasai/constants.py
+-rw-r--r--   0        0        0     2183 2024-02-29 15:48:26.887398 pandasai-2.1a1/pandasai/ee/LICENSE
+-rw-r--r--   0        0        0     4797 2024-05-23 12:40:10.986075 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/__init__.py
+-rw-r--r--   0        0        0     1448 2024-05-23 12:39:50.247652 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/Semantic_prompt_generation.py
+-rw-r--r--   0        0        0     6296 2024-05-23 12:39:50.247789 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/code_generator.py
+-rw-r--r--   0        0        0     1790 2024-05-23 12:39:50.248036 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_correction_pipeline.py
+-rw-r--r--   0        0        0     3213 2024-05-23 12:39:50.248177 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py
+-rw-r--r--   0        0        0     1941 2024-05-23 12:39:50.248484 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/llm_call.py
+-rw-r--r--   0        0        0     2764 2024-05-23 12:39:50.248622 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/semantic_chat_pipeline.py
+-rw-r--r--   0        0        0     2380 2024-05-23 12:40:16.694534 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/validate_pipeline_input.py
+-rw-r--r--   0        0        0     1732 2024-05-23 12:39:50.248987 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/generate_df_schema.py
+-rw-r--r--   0        0        0     1193 2024-05-23 12:39:50.249098 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/semantic_agent_prompt.py
+-rw-r--r--   0        0        0     3289 2024-05-23 12:39:50.249263 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/generate_df_schema.tmpl
+-rw-r--r--   0        0        0       83 2024-05-23 12:40:20.998357 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/semantic_agent_prompt.tmpl
+-rw-r--r--   0        0        0       91 2024-05-23 12:39:50.249517 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/shared/dataframe.tmpl
+-rw-r--r--   0        0        0      418 2024-04-09 07:23:17.860885 pandasai-2.1a1/pandasai/ee/connectors/__init__.py
+-rw-r--r--   0        0        0     2835 2024-02-29 15:48:26.887730 pandasai-2.1a1/pandasai/ee/connectors/databricks.py
+-rw-r--r--   0        0        0     3449 2024-03-15 18:04:31.286624 pandasai-2.1a1/pandasai/ee/connectors/google_big_query.py
+-rw-r--r--   0        0        0      660 2024-04-11 10:03:28.499882 pandasai-2.1a1/pandasai/ee/connectors/relations.py
+-rw-r--r--   0        0        0     3862 2024-02-29 15:48:26.888047 pandasai-2.1a1/pandasai/ee/connectors/snowflake.py
+-rw-r--r--   0        0        0    15531 2024-05-23 12:39:50.249757 pandasai-2.1a1/pandasai/ee/helpers/query_builder.py
+-rw-r--r--   0        0        0      148 2024-03-26 00:39:20.879018 pandasai-2.1a1/pandasai/ee/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10445 2024-02-29 15:48:26.888632 pandasai-2.1a1/pandasai/ee/vectorstores/chroma.py
+-rw-r--r--   0        0        0    14109 2024-03-26 00:39:20.879303 pandasai-2.1a1/pandasai/ee/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      507 2024-02-21 10:04:57.970176 pandasai-2.1a1/pandasai/engine.py
+-rw-r--r--   0        0        0     5665 2024-05-23 12:39:50.250070 pandasai-2.1a1/pandasai/exceptions.py
+-rw-r--r--   0        0        0      446 2024-02-21 10:04:57.970515 pandasai-2.1a1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4613 2024-02-21 10:04:57.971425 pandasai-2.1a1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     3020 2024-05-18 23:34:01.413582 pandasai-2.1a1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0     2397 2024-02-29 15:48:26.889696 pandasai-2.1a1/pandasai/helpers/data_sampler.py
+-rw-r--r--   0        0        0     5557 2024-04-11 10:03:28.500374 pandasai-2.1a1/pandasai/helpers/dataframe_serializer.py
+-rw-r--r--   0        0        0     5062 2024-02-21 10:04:57.972426 pandasai-2.1a1/pandasai/helpers/df_config_manager.py
+-rw-r--r--   0        0        0     1378 2024-04-02 18:08:09.250985 pandasai-2.1a1/pandasai/helpers/df_info.py
+-rw-r--r--   0        0        0     3244 2024-02-27 01:50:10.394311 pandasai-2.1a1/pandasai/helpers/df_validator.py
+-rw-r--r--   0        0        0      291 2024-04-06 07:25:25.510013 pandasai-2.1a1/pandasai/helpers/encoder.py
+-rw-r--r--   0        0        0      526 2024-02-21 10:04:57.973121 pandasai-2.1a1/pandasai/helpers/env.py
+-rw-r--r--   0        0        0      937 2024-03-09 00:53:54.917395 pandasai-2.1a1/pandasai/helpers/file_importer.py
+-rw-r--r--   0        0        0      725 2024-02-29 15:48:26.889894 pandasai-2.1a1/pandasai/helpers/folder.py
+-rw-r--r--   0        0        0     3717 2024-02-21 10:04:57.973750 pandasai-2.1a1/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     4282 2024-05-20 21:21:04.650404 pandasai-2.1a1/pandasai/helpers/logger.py
+-rw-r--r--   0        0        0     3415 2024-03-12 06:39:18.608291 pandasai-2.1a1/pandasai/helpers/memory.py
+-rw-r--r--   0        0        0      447 2023-09-13 09:35:53.943189 pandasai-2.1a1/pandasai/helpers/node_visitors.py
+-rw-r--r--   0        0        0      213 2023-11-20 22:14:04.734116 pandasai-2.1a1/pandasai/helpers/openai.py
+-rw-r--r--   0        0        0     6147 2024-05-18 23:34:01.416531 pandasai-2.1a1/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     4813 2024-05-05 22:29:39.907096 pandasai-2.1a1/pandasai/helpers/optional.py
+-rw-r--r--   0        0        0     1976 2024-02-21 10:04:57.974259 pandasai-2.1a1/pandasai/helpers/output_types/__init__.py
+-rw-r--r--   0        0        0     4658 2024-02-21 10:04:57.974363 pandasai-2.1a1/pandasai/helpers/output_types/_output_types.py
+-rw-r--r--   0        0        0     3708 2024-04-17 17:22:13.619024 pandasai-2.1a1/pandasai/helpers/output_validator.py
+-rw-r--r--   0        0        0     2074 2023-11-20 22:14:04.734712 pandasai-2.1a1/pandasai/helpers/path.py
+-rw-r--r--   0        0        0     8701 2024-05-23 12:39:50.250880 pandasai-2.1a1/pandasai/helpers/query_exec_tracker.py
+-rw-r--r--   0        0        0     2426 2024-04-17 17:22:13.619965 pandasai-2.1a1/pandasai/helpers/request.py
+-rw-r--r--   0        0        0     1061 2024-02-21 10:04:57.975042 pandasai-2.1a1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     8579 2024-02-21 10:04:57.975494 pandasai-2.1a1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     2388 2024-04-06 08:15:23.614472 pandasai-2.1a1/pandasai/helpers/skills_manager.py
+-rw-r--r--   0        0        0      306 2024-03-18 23:35:50.459950 pandasai-2.1a1/pandasai/helpers/sql.py
+-rw-r--r--   0        0        0      629 2024-04-26 07:56:14.443046 pandasai-2.1a1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     7002 2024-03-02 20:32:32.838102 pandasai-2.1a1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0      624 2024-04-19 09:31:18.969118 pandasai-2.1a1/pandasai/llm/bamboo_llm.py
+-rw-r--r--   0        0        0    13479 2024-05-18 23:34:01.417400 pandasai-2.1a1/pandasai/llm/base.py
+-rw-r--r--   0        0        0     5543 2024-05-18 23:34:01.417873 pandasai-2.1a1/pandasai/llm/bedrock_claude.py
+-rw-r--r--   0        0        0      640 2024-02-29 15:48:26.892045 pandasai-2.1a1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     2974 2024-03-15 16:20:10.659958 pandasai-2.1a1/pandasai/llm/google_gemini.py
+-rw-r--r--   0        0        0     2757 2024-03-08 19:32:57.678201 pandasai-2.1a1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     5697 2024-03-08 19:30:08.686882 pandasai-2.1a1/pandasai/llm/google_vertexai.py
+-rw-r--r--   0        0        0     4003 2024-02-29 15:48:26.892474 pandasai-2.1a1/pandasai/llm/huggingface_text_gen.py
+-rw-r--r--   0        0        0     5408 2024-04-26 07:56:14.443204 pandasai-2.1a1/pandasai/llm/ibm_watsonx.py
+-rw-r--r--   0        0        0     1611 2024-03-08 19:30:31.656234 pandasai-2.1a1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1419 2024-03-12 19:49:27.179633 pandasai-2.1a1/pandasai/llm/local_llm.py
+-rw-r--r--   0        0        0     3403 2024-05-18 23:34:01.418842 pandasai-2.1a1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      352 2024-02-28 20:30:56.697841 pandasai-2.1a1/pandasai/pandas/__init__.py
+-rw-r--r--   0        0        0      206 2024-02-29 15:48:26.893218 pandasai-2.1a1/pandasai/pipelines/__init__.py
+-rw-r--r--   0        0        0      353 2023-11-20 22:14:04.741653 pandasai-2.1a1/pandasai/pipelines/abstract_pipeline.py
+-rw-r--r--   0        0        0     1062 2024-02-29 15:48:26.893519 pandasai-2.1a1/pandasai/pipelines/base_logic_unit.py
+-rw-r--r--   0        0        0     1438 2024-02-29 15:48:26.893959 pandasai-2.1a1/pandasai/pipelines/chat/cache_lookup.py
+-rw-r--r--   0        0        0     1253 2024-02-29 15:48:26.894044 pandasai-2.1a1/pandasai/pipelines/chat/cache_population.py
+-rw-r--r--   0        0        0      572 2024-02-29 15:48:26.894142 pandasai-2.1a1/pandasai/pipelines/chat/chat_pipeline_input.py
+-rw-r--r--   0        0        0    18703 2024-05-23 12:39:50.251896 pandasai-2.1a1/pandasai/pipelines/chat/code_cleaning.py
+-rw-r--r--   0        0        0    15802 2024-04-19 09:12:27.360978 pandasai-2.1a1/pandasai/pipelines/chat/code_execution.py
+-rw-r--r--   0        0        0      626 2024-03-09 00:53:51.900905 pandasai-2.1a1/pandasai/pipelines/chat/code_execution_pipeline_input.py
+-rw-r--r--   0        0        0     1473 2024-02-29 15:48:26.894619 pandasai-2.1a1/pandasai/pipelines/chat/code_generator.py
+-rw-r--r--   0        0        0     1638 2024-04-17 17:22:13.622513 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
+-rw-r--r--   0        0        0      240 2024-02-29 15:48:26.894831 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
+-rw-r--r--   0        0        0     3213 2024-03-15 21:22:46.071716 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
+-rw-r--r--   0        0        0    10679 2024-05-23 12:39:50.252333 pandasai-2.1a1/pandasai/pipelines/chat/generate_chat_pipeline.py
+-rw-r--r--   0        0        0     2258 2024-02-29 15:48:26.895146 pandasai-2.1a1/pandasai/pipelines/chat/prompt_generation.py
+-rw-r--r--   0        0        0     2157 2024-03-08 19:22:54.336427 pandasai-2.1a1/pandasai/pipelines/chat/result_parsing.py
+-rw-r--r--   0        0        0     1828 2024-02-29 15:48:26.895371 pandasai-2.1a1/pandasai/pipelines/chat/result_validation.py
+-rw-r--r--   0        0        0     1994 2024-05-23 12:39:50.252632 pandasai-2.1a1/pandasai/pipelines/chat/validate_pipeline_input.py
+-rw-r--r--   0        0        0      612 2024-02-29 15:48:26.895631 pandasai-2.1a1/pandasai/pipelines/logic_unit_output.py
+-rw-r--r--   0        0        0      422 2024-02-21 10:04:57.983209 pandasai-2.1a1/pandasai/pipelines/logic_units/code_executor.py
+-rw-r--r--   0        0        0      900 2024-02-21 10:04:57.983722 pandasai-2.1a1/pandasai/pipelines/logic_units/output_logic_unit.py
+-rw-r--r--   0        0        0      511 2024-02-21 10:04:57.984328 pandasai-2.1a1/pandasai/pipelines/logic_units/prompt_execution.py
+-rw-r--r--   0        0        0     5833 2024-05-23 12:39:50.253446 pandasai-2.1a1/pandasai/pipelines/pipeline.py
+-rw-r--r--   0        0        0     1783 2024-05-23 12:39:50.253690 pandasai-2.1a1/pandasai/pipelines/pipeline_context.py
+-rw-r--r--   0        0        0      232 2024-02-29 15:48:26.896427 pandasai-2.1a1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     2098 2024-05-23 12:39:50.254517 pandasai-2.1a1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0      207 2024-02-29 15:48:26.896838 pandasai-2.1a1/pandasai/prompts/check_if_relevant_to_conversation.py
+-rw-r--r--   0        0        0      518 2024-02-29 15:48:26.896953 pandasai-2.1a1/pandasai/prompts/clarification_questions_prompt.py
+-rw-r--r--   0        0        0      902 2024-02-29 15:48:26.897330 pandasai-2.1a1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0      975 2024-02-29 15:48:26.898228 pandasai-2.1a1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
+-rw-r--r--   0        0        0     1058 2024-02-29 15:48:26.898521 pandasai-2.1a1/pandasai/prompts/correct_output_type_error_prompt.py
+-rw-r--r--   0        0        0     1904 2024-03-09 00:53:54.918124 pandasai-2.1a1/pandasai/prompts/direct_sql_prompt.py
+-rw-r--r--   0        0        0      159 2024-02-29 15:48:26.898919 pandasai-2.1a1/pandasai/prompts/explain_prompt.py
+-rw-r--r--   0        0        0     1274 2024-02-21 10:04:57.989230 pandasai-2.1a1/pandasai/prompts/file_based_prompt.py
+-rw-r--r--   0        0        0      879 2024-02-29 15:48:26.899086 pandasai-2.1a1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      268 2024-02-29 15:48:26.899212 pandasai-2.1a1/pandasai/prompts/generate_python_code_with_sql.py
+-rw-r--r--   0        0        0      189 2024-02-29 15:48:26.899664 pandasai-2.1a1/pandasai/prompts/generate_system_message.py
+-rw-r--r--   0        0        0      172 2024-02-29 15:48:26.899949 pandasai-2.1a1/pandasai/prompts/rephase_query_prompt.py
+-rw-r--r--   0        0        0      199 2024-02-29 15:48:26.900245 pandasai-2.1a1/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
+-rw-r--r--   0        0        0      571 2024-02-29 15:48:26.900559 pandasai-2.1a1/pandasai/prompts/templates/clarification_questions_prompt.tmpl
+-rw-r--r--   0        0        0      342 2024-02-29 15:48:26.900738 pandasai-2.1a1/pandasai/prompts/templates/correct_error_prompt.tmpl
+-rw-r--r--   0        0        0      356 2024-02-29 15:48:26.900820 pandasai-2.1a1/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
+-rw-r--r--   0        0        0      343 2024-02-29 15:48:26.900888 pandasai-2.1a1/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
+-rw-r--r--   0        0        0      325 2024-02-29 15:48:26.901074 pandasai-2.1a1/pandasai/prompts/templates/explain.tmpl
+-rw-r--r--   0        0        0      923 2024-03-28 17:45:03.638878 pandasai-2.1a1/pandasai/prompts/templates/generate_python_code.tmpl
+-rw-r--r--   0        0        0     1311 2024-04-06 08:15:29.233436 pandasai-2.1a1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
+-rw-r--r--   0        0        0      176 2024-02-29 15:48:26.901720 pandasai-2.1a1/pandasai/prompts/templates/generate_system_message.tmpl
+-rw-r--r--   0        0        0      387 2024-02-29 15:48:26.901838 pandasai-2.1a1/pandasai/prompts/templates/rephrase_query.tmpl
+-rw-r--r--   0        0        0      123 2024-04-02 18:08:09.251668 pandasai-2.1a1/pandasai/prompts/templates/shared/dataframe.tmpl
+-rw-r--r--   0        0        0      916 2024-02-29 15:48:26.902116 pandasai-2.1a1/pandasai/prompts/templates/shared/output_type_template.tmpl
+-rw-r--r--   0        0        0      624 2024-02-29 15:48:26.902323 pandasai-2.1a1/pandasai/prompts/templates/shared/vectordb_docs.tmpl
+-rw-r--r--   0        0        0      102 2024-02-27 01:50:10.394612 pandasai-2.1a1/pandasai/pydantic/__init__.py
+-rw-r--r--   0        0        0      311 2024-02-21 10:04:57.990280 pandasai-2.1a1/pandasai/responses/__init__.py
+-rw-r--r--   0        0        0      637 2024-02-29 15:48:26.902758 pandasai-2.1a1/pandasai/responses/context.py
+-rw-r--r--   0        0        0     2159 2024-04-06 07:25:25.512293 pandasai-2.1a1/pandasai/responses/response_parser.py
+-rw-r--r--   0        0        0     1593 2024-04-11 10:03:31.648509 pandasai-2.1a1/pandasai/responses/response_serializer.py
+-rw-r--r--   0        0        0       96 2024-02-29 15:48:26.903015 pandasai-2.1a1/pandasai/responses/response_type.py
+-rw-r--r--   0        0        0     1036 2024-02-21 10:04:57.991273 pandasai-2.1a1/pandasai/responses/streamlit_response.py
+-rw-r--r--   0        0        0       16 2023-09-04 21:53:07.396618 pandasai-2.1a1/pandasai/schemas/__init__.py
+-rw-r--r--   0        0        0     1305 2024-04-13 15:58:12.089425 pandasai-2.1a1/pandasai/schemas/df_config.py
+-rw-r--r--   0        0        0     3920 2024-02-29 15:48:26.903634 pandasai-2.1a1/pandasai/skills/__init__.py
+-rw-r--r--   0        0        0     8894 2024-05-23 12:39:50.255046 pandasai-2.1a1/pandasai/smart_dataframe/__init__.py
+-rw-r--r--   0        0        0     6256 2024-05-23 12:39:50.255362 pandasai-2.1a1/pandasai/smart_datalake/__init__.py
+-rw-r--r--   0        0        0      193 2024-02-29 15:48:26.904302 pandasai-2.1a1/pandasai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-02 18:08:09.251824 pandasai-2.1a1/pandasai/vectorstores/bamboo_vectorstore.py
+-rw-r--r--   0        0        0     5764 2024-02-29 15:48:26.904463 pandasai-2.1a1/pandasai/vectorstores/vectorstore.py
+-rw-r--r--   0        0        0     3813 2024-05-23 12:43:33.427720 pandasai-2.1a1/pyproject.toml
+-rw-r--r--   0        0        0     9608 1970-01-01 00:00:00.000000 pandasai-2.1a1/PKG-INFO
```

### Comparing `pandasai-2.1/LICENSE` & `pandasai-2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/README.md` & `pandasai-2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/__init__.py` & `pandasai-2.1a1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/agent/agent.py` & `pandasai-2.1a1/pandasai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/agent/base.py` & `pandasai-2.1a1/pandasai/agent/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/agent/callbacks.py` & `pandasai-2.1a1/pandasai/agent/callbacks.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/config.py` & `pandasai-2.1a1/pandasai/config.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/__init__.py` & `pandasai-2.1a1/pandasai/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/airtable.py` & `pandasai-2.1a1/pandasai/connectors/airtable.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/base.py` & `pandasai-2.1a1/pandasai/connectors/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/pandas.py` & `pandasai-2.1a1/pandasai/connectors/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         Args:
             config (PandasConnectorConfig): The configuration for the Pandas connector.
         """
         super().__init__(config, **kwargs)
 
         self._load_df(self.config.original_df)
-        self.sql_enabled = False
+        self.sql_enabed = False
 
     def _load_df(self, df: Union[pd.DataFrame, pd.Series, str, list, dict]):
         """
         Load the dataframe from a file or pandas dataframe.
 
         Args:
             df (Union[pd.DataFrame, pd.Series, str, list, dict]): The dataframe to load.
@@ -163,19 +163,19 @@
     def enable_sql_query(self, table_name=None):
         if not table_name and not self.name:
             raise PandasConnectorTableNotFound("Table name not found!")
 
         table = table_name or self.name
         duckdb_relation = duckdb.from_df(self.pandas_df)
         duckdb_relation.create(table)
-        self.sql_enabled = True
+        self.sql_enabed = True
         self.name = table
 
     def execute_direct_sql_query(self, sql_query):
-        if not self.sql_enabled:
+        if not self.sql_enabed:
             self.enable_sql_query()
         sql_query = sql_query.replace("`", '"')
         return duckdb.query(sql_query).df()
 
     @property
     def cs_table_name(self):
         return self.name
```

### Comparing `pandasai-2.1/pandasai/connectors/polars.py` & `pandasai-2.1a1/pandasai/connectors/polars.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/sql.py` & `pandasai-2.1a1/pandasai/connectors/sql.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/connectors/yahoo_finance.py` & `pandasai-2.1a1/pandasai/connectors/yahoo_finance.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/constants.py` & `pandasai-2.1a1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/LICENSE` & `pandasai-2.1a1/pandasai/ee/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/__init__.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     GenerateDFSchemaPrompt,
 )
 from pandasai.exceptions import InvalidConfigError
 from pandasai.helpers.cache import Cache
 from pandasai.helpers.memory import Memory
 from pandasai.llm.bamboo_llm import BambooLLM
 from pandasai.pipelines.chat.generate_chat_pipeline import GenerateChatPipeline
-from pandasai.pipelines.pipeline import Pipeline
 from pandasai.pipelines.pipeline_context import PipelineContext
-from pandasai.ee.agents.semantic_agent.pipeline.code_generator import CodeGenerator
 from pandasai.schemas.df_config import Config
 from pandasai.vectorstores.vectorstore import VectorStore
 
 
 class SemanticAgent(BaseAgent):
     """
     Answer Semantic queries
@@ -32,26 +30,25 @@
 
     def __init__(
         self,
         dfs: Union[
             pd.DataFrame, BaseConnector, List[Union[pd.DataFrame, BaseConnector]]
         ],
         config: Optional[Union[Config, dict]] = None,
-        schema: Optional[List[dict]] = None,
         memory_size: Optional[int] = 10,
         pipeline: Optional[Type[GenerateChatPipeline]] = None,
         vectorstore: Optional[VectorStore] = None,
         description: str = None,
     ):
         super().__init__(dfs, config, memory_size, vectorstore, description)
 
         self._validate_config()
 
         self._schema_cache = Cache("schema")
-        self._schema = schema or None
+        self._schema = None
 
         self._create_schema()
 
         self.init_duckdb_instance()
 
         # semantic agent works only with direct sql true
         self.config.direct_sql = True
@@ -80,39 +77,23 @@
                 on_prompt_generation=self._callbacks.on_prompt_generation,
                 on_code_generation=self._callbacks.on_code_generation,
                 before_code_execution=self._callbacks.before_code_execution,
                 on_result=self._callbacks.on_result,
             )
         )
 
-    def query(self, query):
-        query_pipeline = Pipeline(
-            context=self.context,
-            logger=self.logger,
-            steps=[
-                CodeGenerator(),
-            ],
-        )
-        code = query_pipeline.run(query)
-
-        self.execute_code(code)
-
     def init_duckdb_instance(self):
         for index, tables in enumerate(self._schema):
             if isinstance(self.dfs[index], PandasConnector):
                 self.dfs[index].enable_sql_query(tables["table"])
 
     def _create_schema(self):
         """
         Generate schema on the initialization of Agent class
         """
-        if self._schema:
-            self.logger.log(f"using user provided schema: {self._schema}")
-            return
-
         key = self._get_schema_cache_key()
         if self.config.enable_cache:
             value = self._schema_cache.get(key)
             if value is not None:
                 self._schema = json.loads(value)
                 self.logger.log(f"using schema: {self._schema}")
                 return
```

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/Semantic_prompt_generation.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/Semantic_prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/code_generator.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/code_generator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_correction_pipeline.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/llm_call.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/llm_call.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/semantic_chat_pipeline.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/semantic_chat_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/pipeline/validate_pipeline_input.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/validate_pipeline_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         Raises:
             InvalidConfigError: Raise Error in case of config is set but criteria is not met
         """
 
         if self.context.config.direct_sql:
             if all(
                 (isinstance(df, SQLConnector) and df.equals(dfs[0])) for df in dfs
-            ) or all(
-                (isinstance(df, PandasConnector) and df.sql_enabled) for df in dfs
-            ):
+            ) or all((isinstance(df, PandasConnector) and df.sql_enabed) for df in dfs):
                 return True
             else:
                 raise InvalidConfigError(
                     "Direct requires all SQLConnector and they belong to same datasource "
                     "and have same credentials"
                 )
         return False
```

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/generate_df_schema.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/generate_df_schema.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/semantic_agent_prompt.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/semantic_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/agents/semantic_agent/prompts/templates/generate_df_schema.tmpl` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/generate_df_schema.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/connectors/databricks.py` & `pandasai-2.1a1/pandasai/ee/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/connectors/google_big_query.py` & `pandasai-2.1a1/pandasai/ee/connectors/google_big_query.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/connectors/relations.py` & `pandasai-2.1a1/pandasai/ee/connectors/relations.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/connectors/snowflake.py` & `pandasai-2.1a1/pandasai/ee/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/helpers/query_builder.py` & `pandasai-2.1a1/pandasai/ee/helpers/query_builder.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/vectorstores/chroma.py` & `pandasai-2.1a1/pandasai/ee/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/ee/vectorstores/pinecone.py` & `pandasai-2.1a1/pandasai/ee/vectorstores/qdrant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,97 @@
+import logging
 import uuid
-from typing import Callable, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional
 
-import pinecone
+import qdrant_client
+from qdrant_client import models
 
 from pandasai.helpers.logger import Logger
 from pandasai.vectorstores.vectorstore import VectorStore
 
-
-class Pinecone(VectorStore):
-    """
-    Implementation of Pinecone vector store
+DEFAULT_COLLECTION_NAME = "pandasai"
+DEFAULT_EMBEDDING_MODEL = "BAAI/bge-small-en-v1.5"
+UUID_NAMESPACE = "f55f1395-e097-4f35-8c20-90fdea7baa14"
+
+
+class Qdrant(VectorStore):
+    """Implementation of VectorStore for Qdrant - https://qdrant.tech/
+
+    Supports adding, updating, deleting and querying code Q/As and documents.\n
+    Since Qdrant only allows unsigned integers or UUID strings as point IDs,
+    we convert any arbitrary string ID into a UUID string based on a seed.
+
+    Args:
+        collection_name: Name of the collection.
+        Will be transformed into `<COLLECTION_NAME>-qa` and `<COLLECTION_NAME>-docs` for code Q/A and documents respectively.\n
+        embedding_model: Name of the embedding model to use.\n
+        location:
+            If `':memory:'` - use in-memory Qdrant instance.\n
+            If `str` - use it as a `url` parameter.\n
+            If `None` - use default values for `host` and `port`.\n
+        url: either host or str of "`Optional[scheme]`, `host`, `Optional[port]`, `Optional[prefix]`". Default: `None`.\n
+        port: Port of the REST API interface. Default: 6333.\n
+        grpc_port: Port of the gRPC interface. Default: 6334.\n
+        prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.\n
+        https: If `true` - use HTTPS(SSL) protocol. Default: `None`.\n
+        api_key: API key for authentication in Qdrant Cloud. Default: `None`.\n
+        prefix:
+            If not `None` - add `prefix` to the REST URL path.\n
+            Example: `service/v1` will result in `http://localhost:6333/service/v1/[qdrant-endpoint]` for REST API.\n
+            Default: `None`.\n
+        timeout:
+            Timeout for REST and gRPC API requests.\n
+            Default: 5 seconds for REST and unlimited for gRPC.\n
+        host: Host name of Qdrant service. If url and host are None, set to 'localhost'.\n
+            Default: `None`.\n
+        path: Persistence path for QdrantLocal. Default: `None`.\n
+        grpc_options: Options for the low-level gRPC client, if used. Default: `None`.\n
+        similary_threshold: Similarity threshold for search. Default: `None`.\n
+        logger: Optional custom Logger instance..
     """
 
-    _logger: Logger
-
     def __init__(
         self,
-        api_key: str,
-        index: Union[str, pinecone.Index] = "pandasai",
-        embedding_function: Optional[Callable[[List[str]], List[float]]] = None,
-        dimensions=1536,
-        metric="cosine",
-        pool_threads: int = 1,
-        specs: pinecone.ServerlessSpec = None,
-        max_samples: int = 1,
-        similary_threshold: int = 1.5,
+        collection_name: str = DEFAULT_COLLECTION_NAME,
+        embedding_model: str = DEFAULT_EMBEDDING_MODEL,
+        location: Optional[str] = None,
+        url: Optional[str] = None,
+        port: Optional[int] = 6333,
+        grpc_port: int = 6334,
+        prefer_grpc: bool = False,
+        https: Optional[bool] = None,
+        api_key: Optional[str] = None,
+        prefix: Optional[str] = None,
+        timeout: Optional[int] = None,
+        host: Optional[str] = None,
+        path: Optional[str] = None,
+        grpc_options: Optional[Dict[str, Any]] = None,
+        similary_threshold: Optional[float] = None,
         logger: Optional[Logger] = None,
     ) -> None:
+        self._qa_collection_name = f"{collection_name}-qa"
+        self._docs_collection_name = f"{collection_name}-docs"
         self._logger = logger or Logger()
-        self._max_samples = max_samples
         self._similarity_threshold = similary_threshold
-        self._api_key = api_key
-
-        self._metatext_key = "text"
-
-        self._embedding_function = embedding_function
 
-        self._pinecone = pinecone.Pinecone(api_key=api_key, pool_threads=pool_threads)
-
-        if isinstance(index, str):
-            if index not in self._pinecone.list_indexes().names():
-                self._index = self._pinecone.create_index(
-                    name=index,
-                    dimension=dimensions,
-                    metric=metric,
-                    spec=specs
-                    or pinecone.ServerlessSpec(cloud="aws", region="us-east-1"),
-                )
-
-            self._index = self._pinecone.Index(name=index)
-
-        else:
-            self._index = index
-
-        self._logger.log("Successfully initialized index")
+        self._client = qdrant_client.QdrantClient(
+            location=location,
+            url=url,
+            port=port,
+            grpc_port=grpc_port,
+            prefer_grpc=prefer_grpc,
+            https=https,
+            api_key=api_key,
+            prefix=prefix,
+            timeout=timeout,
+            host=host,
+            path=path,
+            grpc_options=grpc_options,
+        )
+        self._client.set_model(embedding_model)
 
     def add_question_answer(
         self,
         queries: Iterable[str],
         codes: Iterable[str],
         ids: Optional[Iterable[str]] = None,
         metadatas: Optional[List[dict]] = None,
@@ -71,35 +105,28 @@
             metadatas: Optional list of metadatas associated with the texts.
             kwargs: vectorstore specific parameters
         Returns:
             List of ids from adding the texts into the vectorstore.
         """
         if len(queries) != len(codes):
             raise ValueError(
-                f"Queries and codes dimension doesn't match {len(queries)} != {len(codes)}"
+                f"Queries and codes length doesn't match. {len(queries)} != {len(codes)}"
             )
 
-        if ids is None:
-            ids = [f"{str(uuid.uuid4())}-qa" for _ in queries]
-
-        metadatas = metadatas or [{} for _ in ids]
+        qdrant_ids = self._convert_ids(ids) if ids else None
 
         qa_str = [self._format_qa(query, code) for query, code in zip(queries, codes)]
 
-        for index, metadata in enumerate(metadatas):
-            metadata[self._metatext_key] = qa_str[index]
-
-        vector_data = [
-            {"id": ids[index], "values": qa, "metadata": metadatas[index]}
-            for index, qa in enumerate(self._embedding_function(qa_str))
-        ]
-
-        self._index.upsert(vectors=vector_data, namespace="qa")
-
-        return ids
+        # If IDs are not provided(None), qdrant_client generates random UUIDs
+        return self._client.add(
+            self._qa_collection_name,
+            documents=qa_str,
+            metadata=metadatas,
+            ids=qdrant_ids,
+        )
 
     def add_docs(
         self,
         docs: Iterable[str],
         ids: Optional[Iterable[str]] = None,
         metadatas: Optional[List[dict]] = None,
     ) -> List[str]:
@@ -110,35 +137,23 @@
             ids: Optional Iterable of ids associated with the texts.
             metadatas: Optional list of metadatas associated with the texts.
             kwargs: vectorstore specific parameters
 
         Returns:
             List of ids from adding the texts into the vectorstore.
         """
-        if not isinstance(docs, list):
-            raise ValueError("Docs must be list of strings!")
-
-        if ids is None:
-            ids = [f"{str(uuid.uuid4())}-docs" for _ in docs]
-
-        metadatas = metadatas or [{} for _ in ids]
-
-        doc_embeddings = self._embedding_function(docs)
+        qdrant_ids = self._convert_ids(ids) if ids else None
 
-        for index, metadata in enumerate(metadatas):
-            metadata[self._metatext_key] = docs[index]
-
-        vector_data = [
-            {"id": ids[index], "values": doc, "metadata": metadatas[index]}
-            for index, doc in enumerate(doc_embeddings)
-        ]
-
-        self._index.upsert(vectors=vector_data, namespace="docs")
-
-        return ids
+        # If IDs are not provided(None), qdrant_client generates random UUIDs
+        return self._client.add(
+            self._docs_collection_name,
+            documents=docs,
+            metadata=metadatas,
+            ids=qdrant_ids,
+        )
 
     def update_question_answer(
         self,
         ids: Iterable[str],
         queries: Iterable[str],
         codes: Iterable[str],
         metadatas: Optional[List[dict]] = None,
@@ -150,30 +165,35 @@
             queries: string of question
             codes: str
             metadatas: Optional list of metadatas associated with the texts.
             kwargs: vectorstore specific parameters
         Returns:
             List of ids from updating the texts into the vectorstore.
         """
-        if len(queries) != len(codes):
+
+        if not (len(ids) == len(queries) == len(codes)):
             raise ValueError(
-                f"Queries and codes dimension doesn't match {len(queries)} != {len(codes)}"
+                f"Queries, codes and ids length doesn't match. {len(queries)} != {len(codes)} != {len(ids)}"
             )
 
-        qa_str = [self._format_qa(query, code) for query, code in zip(queries, codes)]
+        qdrant_ids = self._convert_ids(ids)
 
-        metadatas = metadatas or [{} for _ in ids]
+        # Ensure that the IDs exist in the collection
+        if not self._validate_update_ids(self._qa_collection_name, qdrant_ids):
+            return []
 
-        for index, metadata in enumerate(metadatas):
-            metadata[self._metatext_key] = qa_str[index]
+        qa_str = [self._format_qa(query, code) for query, code in zip(queries, codes)]
 
-        for index, qa in enumerate(self._embedding_function(qa_str)):
-            self._index.update(
-                id=ids[index], values=qa, set_metadata=metadatas[index], namespace="qa"
-            )
+        # Entries with same IDs will be overwritten. Essentially updating them.
+        return self._client.add(
+            self._qa_collection_name,
+            documents=qa_str,
+            metadata=metadatas,
+            ids=qdrant_ids,
+        )
 
     def update_docs(
         self,
         ids: Iterable[str],
         docs: Iterable[str],
         metadatas: Optional[List[dict]] = None,
     ) -> List[str]:
@@ -185,144 +205,198 @@
             metadatas: Optional list of metadatas associated with the texts.
             kwargs: vectorstore specific parameters
 
         Returns:
             List of ids from adding the texts into the vectorstore.
         """
 
-        doc_embeddings = self._embedding_function(docs)
-
-        metadatas = metadatas or [{} for _ in ids]
+        if len(ids) != len(docs):
+            raise ValueError(
+                f"Docs and ids length doesn't match. {len(docs)} != {len(ids)}"
+            )
 
-        for index, metadata in enumerate(metadatas):
-            metadata[self._metatext_key] = docs[index]
+        qdrant_ids = self._convert_ids(ids)
 
-        for index, doc in enumerate(doc_embeddings):
-            self._index.update(
-                id=ids[index],
-                values=doc,
-                set_metadata=metadatas[index],
-                namespace="docs",
-            )
+        # Ensure that the IDs exist in the collection
+        if not self._validate_update_ids(self._qa_collection_name, qdrant_ids):
+            return []
+
+        # Entries with same IDs will be overwritten. Essentially updating them.
+        return self._client.add(
+            self._docs_collection_name,
+            documents=docs,
+            metadata=metadatas,
+            ids=qdrant_ids,
+        )
 
     def delete_question_and_answers(
         self, ids: Optional[List[str]] = None
     ) -> Optional[bool]:
         """
         Delete by vector ID to delete question and answers
         Args:
             ids: List of ids to delete
 
         Returns:
             Optional[bool]: True if deletion is successful,
             False otherwise
         """
-
-        self._index.delete(ids=ids, namespace="qa")
-        return True
+        if ids:
+            ids = self._convert_ids(ids)
+            response = self._client.delete(
+                self._qa_collection_name, points_selector=ids
+            )
+            return response.status == models.UpdateStatus.COMPLETED
 
     def delete_docs(self, ids: Optional[List[str]] = None) -> Optional[bool]:
         """
         Delete by vector ID to delete docs
         Args:
             ids: List of ids to delete
 
         Returns:
             Optional[bool]: True if deletion is successful,
             False otherwise
         """
-        self._index.delete(ids=ids, namespace="docs")
-        return True
+        if ids:
+            ids = self._convert_ids(ids)
+            response = self._client.delete(
+                self._docs_collection_name, points_selector=ids
+            )
+            return response.status == models.UpdateStatus.COMPLETED
 
-    def get_relevant_question_answers(
-        self, question: str, k: Union[int, None] = None
-    ) -> List[dict]:
+    def delete_collection(self, collection_name: str) -> Optional[bool]:
+        self._client.delete_collection(f"{collection_name}-qa")
+        self._client.delete_collection(f"{collection_name}-docs")
+
+    def get_relevant_question_answers(self, question: str, k: int = 1) -> List[dict]:
         """
         Returns relevant question answers based on search
         """
-        k = k or self._max_samples
-
-        questions = self._embedding_function([question])
-
-        results = self._index.query(
-            vector=questions,
-            top_k=k,
-            include_metadata=True,
-            namespace="qa",
-            include_values=True,
+        response = self._client.query(
+            self._qa_collection_name,
+            query_text=question,
+            limit=k,
+            score_threshold=self._similarity_threshold,
         )
 
-        return self._filter_docs_based_on_distance(results, self._similarity_threshold)
+        return self._convert_query_response(response)
 
-    def get_relevant_docs(self, question: str, k: int = None) -> List[dict]:
+    def get_relevant_docs(self, question: str, k: int = 1) -> List[dict]:
         """
-        Returns relevant documents based search
+        Returns relevant documents based on semantic search
         """
-        k = k or self._max_samples
-
-        questions = self._embedding_function([question])
-
-        results = self._index.query(
-            vector=questions,
-            top_k=k,
-            include_metadata=True,
-            namespace="docs",
-            include_values=True,
+        response = self._client.query(
+            self._docs_collection_name,
+            query_text=question,
+            limit=k,
+            score_threshold=self._similarity_threshold,
         )
 
-        return self._filter_docs_based_on_distance(results, self._similarity_threshold)
+        return self._convert_query_response(response)
 
     def get_relevant_question_answers_by_id(self, ids: Iterable[str]) -> List[dict]:
         """
-        Returns relevant question answers based on ids
+        Returns question answers based on ids
         """
-        return self._index.fetch(id=ids, namespace="qa")
+
+        qdrant_ids = self._convert_ids(ids)
+
+        response = self._client.retrieve(self._qa_collection_name, ids=qdrant_ids)
+
+        return self._convert_retrieve_response(response)
 
     def get_relevant_docs_by_id(self, ids: Iterable[str]) -> List[dict]:
         """
-        Returns relevant question answers based on ids
+        Returns docs based on ids
         """
 
-        return self._index.fetch(id=ids, namespace="docs")
+        qdrant_ids = self._convert_ids(ids)
+
+        response = self._client.retrieve(self._docs_collection_name, ids=qdrant_ids)
+
+        return self._convert_retrieve_response(response)
 
-    def get_relevant_qa_documents(self, question: str, k: int = None) -> List[str]:
+    def get_relevant_qa_documents(self, question: str, k: int = 1) -> List[str]:
         """
-        Returns relevant question answers documents only
-        Args:
-            question (_type_): list of documents
+        Returns question answers documents only
         """
-        return self.get_relevant_question_answers(question, k)["documents"][0]
+        return self.get_relevant_question_answers(question, k)["documents"]
 
-    def get_relevant_docs_documents(self, question: str, k: int = None) -> List[str]:
+    def get_relevant_docs_documents(self, question: str, k: int = 1) -> List[str]:
         """
-        Returns relevant question answers documents only
-        Args:
-            question (_type_): list of documents
+        Returns question answers documents only
         """
-        return self.get_relevant_docs(question, k)["documents"][0]
+        return self.get_relevant_docs(question, k)["documents"]
 
-    def _filter_docs_based_on_distance(self, documents, threshold: int) -> List[str]:
+    def _validate_update_ids(self, collection_name: str, ids: List[str]) -> bool:
         """
-        Filter documents based on threshold
-        Args:
-            documents (List[str]): list of documents in string
-            distances (List[float]): list of distances in float
-            threshold (int): similarity threshold
-
-        Returns:
-            _type_: _description_
+        Validates all the IDs exist in the collection
         """
-        filtered_data = [
-            (
-                document["metadata"][self._metatext_key],
-                document["score"],
-                document["metadata"],
-                document["id"],
+        retrieved_ids = [
+            point.id
+            for point in self._client.retrieve(
+                collection_name, ids=ids, with_payload=False, with_vectors=False
             )
-            for document in documents["matches"]
-            if document["score"] < threshold
         ]
 
+        if missing_ids := set(ids) - set(retrieved_ids):
+            self._logger.log(
+                f"Missing IDs: {missing_ids}. Skipping update", level=logging.WARN
+            )
+            return False
+
+        return True
+
+    def _convert_ids(self, ids: Iterable[str]) -> List[str]:
+        """
+        Converts any string into a UUID string based on a seed.
+
+        Qdrant accepts UUID strings and unsigned integers as point ID.
+        We use a seed to convert each string into a UUID string deterministically.
+        This allows us to overwrite the same point with the original ID.
+        """
+        return [
+            id
+            if self._is_valid_uuid(id)
+            else str(uuid.uuid5(uuid.UUID(UUID_NAMESPACE), id))
+            for id in ids
+        ]
+
+    def _convert_query_response(
+        self, results: List[models.QueryResponse]
+    ) -> List[dict]:
+        documents, distances, metadatas, ids = [], [], [], []
+
+        for point in results:
+            documents.append(point.document)
+            distances.append(point.score)
+            metadatas.append(point.metadata)
+            ids.append(point.id)
+
         return {
-            key: [[data[i] for data in filtered_data]]
-            for i, key in enumerate(["documents", "distances", "metadata", "ids"])
+            "documents": documents,
+            "distances": distances,
+            "metadatas": metadatas,
+            "ids": ids,
         }
+
+    def _convert_retrieve_response(self, response: List[models.Record]) -> List[dict]:
+        documents, metadatas, ids = [], [], []
+
+        for point in response:
+            documents.append(point.payload.get("document", ""))
+            metadatas.append(point.payload)
+            ids.append(point.id)
+
+        return {
+            "documents": documents,
+            "metadatas": metadatas,
+            "ids": ids,
+        }
+
+    def _is_valid_uuid(self, id: str):
+        try:
+            uuid.UUID(id)
+            return True
+        except ValueError:
+            return False
```

### Comparing `pandasai-2.1/pandasai/exceptions.py` & `pandasai-2.1a1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/anonymizer.py` & `pandasai-2.1a1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/cache.py` & `pandasai-2.1a1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/data_sampler.py` & `pandasai-2.1a1/pandasai/helpers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/dataframe_serializer.py` & `pandasai-2.1a1/pandasai/helpers/dataframe_serializer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/df_config_manager.py` & `pandasai-2.1a1/pandasai/helpers/df_config_manager.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/df_info.py` & `pandasai-2.1a1/pandasai/helpers/df_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/df_validator.py` & `pandasai-2.1a1/pandasai/helpers/df_validator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/env.py` & `pandasai-2.1a1/pandasai/helpers/env.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/file_importer.py` & `pandasai-2.1a1/pandasai/helpers/file_importer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/folder.py` & `pandasai-2.1a1/pandasai/helpers/folder.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/from_google_sheets.py` & `pandasai-2.1a1/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/logger.py` & `pandasai-2.1a1/pandasai/helpers/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         """Initialize the logger"""
         self._logs = []
         self._verbose = verbose
         self._last_time = time.time()
 
         if save_logs:
             try:
-                filename = find_closest("pandasai.log")
+                filaname = find_closest("pandasai.log")
             except ValueError:
-                filename = "pandasai.log"
-            handlers = [logging.FileHandler(filename)]
+                filaname = "pandasai.log"
+            handlers = [logging.FileHandler(filaname)]
         else:
             handlers = []
 
         if verbose:
             handlers.append(logging.StreamHandler(sys.stdout))
 
         logging.basicConfig(
@@ -137,14 +137,14 @@
         """Return the save_logs flag"""
         return len(self._logger.handlers) > 0
 
     @save_logs.setter
     def save_logs(self, save_logs: bool):
         """Set the save_logs flag"""
         if save_logs and not self.save_logs:
-            filename = find_closest("pandasai.log")
-            self._logger.addHandler(logging.FileHandler(filename))
+            filaname = find_closest("pandasai.log")
+            self._logger.addHandler(logging.FileHandler(filaname))
         elif not save_logs and self.save_logs:
             # remove the FileHandler if it exists
             for handler in self._logger.handlers:
                 if isinstance(handler, logging.FileHandler):
                     self._logger.removeHandler(handler)
```

### Comparing `pandasai-2.1/pandasai/helpers/memory.py` & `pandasai-2.1a1/pandasai/helpers/memory.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/openai_info.py` & `pandasai-2.1a1/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/optional.py` & `pandasai-2.1a1/pandasai/helpers/optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/output_types/__init__.py` & `pandasai-2.1a1/pandasai/helpers/output_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/output_types/_output_types.py` & `pandasai-2.1a1/pandasai/helpers/output_types/_output_types.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/output_validator.py` & `pandasai-2.1a1/pandasai/helpers/output_validator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/path.py` & `pandasai-2.1a1/pandasai/helpers/path.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/query_exec_tracker.py` & `pandasai-2.1a1/pandasai/helpers/query_exec_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,14 @@
 
     def add_step(self, step: dict) -> None:
         """
         Add Custom Step that is performed for additional information
         Args:
             step (dict): dictionary containing information
         """
-        if "_steps" not in self.__dict__:
-            self._steps = []
-
         self._steps.append(step)
 
     def set_final_response(self, response: Any):
         self._response = response
 
     def execute_func(self, function, *args, **kwargs) -> Any:
         """
```

### Comparing `pandasai-2.1/pandasai/helpers/request.py` & `pandasai-2.1a1/pandasai/helpers/request.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/save_chart.py` & `pandasai-2.1a1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/shortcuts.py` & `pandasai-2.1a1/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/helpers/skills_manager.py` & `pandasai-2.1a1/pandasai/helpers/skills_manager.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/__init__.py` & `pandasai-2.1a1/pandasai/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/azure_openai.py` & `pandasai-2.1a1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/bamboo_llm.py` & `pandasai-2.1a1/pandasai/llm/bamboo_llm.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/base.py` & `pandasai-2.1a1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/bedrock_claude.py` & `pandasai-2.1a1/pandasai/llm/bedrock_claude.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/fake.py` & `pandasai-2.1a1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/google_gemini.py` & `pandasai-2.1a1/pandasai/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/google_palm.py` & `pandasai-2.1a1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/google_vertexai.py` & `pandasai-2.1a1/pandasai/llm/google_vertexai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/huggingface_text_gen.py` & `pandasai-2.1a1/pandasai/llm/huggingface_text_gen.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/ibm_watsonx.py` & `pandasai-2.1a1/pandasai/llm/ibm_watsonx.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/langchain.py` & `pandasai-2.1a1/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/local_llm.py` & `pandasai-2.1a1/pandasai/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/llm/openai.py` & `pandasai-2.1a1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/base_logic_unit.py` & `pandasai-2.1a1/pandasai/pipelines/base_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/cache_lookup.py` & `pandasai-2.1a1/pandasai/pipelines/chat/cache_lookup.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/cache_population.py` & `pandasai-2.1a1/pandasai/pipelines/chat/cache_population.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/chat_pipeline_input.py` & `pandasai-2.1a1/pandasai/pipelines/chat/chat_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/code_cleaning.py` & `pandasai-2.1a1/pandasai/pipelines/chat/code_cleaning.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,15 @@
         Raises:
             InvalidConfigError: Raise Error in case of config is set but criteria is not met
         """
 
         if self._config.direct_sql:
             if all(
                 (isinstance(df, SQLConnector) and df.equals(dfs[0])) for df in dfs
-            ) or all(
-                (isinstance(df, PandasConnector) and df.sql_enabled) for df in dfs
-            ):
+            ) or all((isinstance(df, PandasConnector) and df.sql_enabed) for df in dfs):
                 return True
             else:
                 raise InvalidConfigError(
                     "Direct requires all SQLConnector and they belong to same datasource "
                     "and have same credentials"
                 )
         return False
```

### Comparing `pandasai-2.1/pandasai/pipelines/chat/code_execution.py` & `pandasai-2.1a1/pandasai/pipelines/chat/code_execution.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/code_execution_pipeline_input.py` & `pandasai-2.1a1/pandasai/pipelines/chat/code_execution_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/code_generator.py` & `pandasai-2.1a1/pandasai/pipelines/chat/code_generator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py` & `pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/generate_chat_pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/chat/generate_chat_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/prompt_generation.py` & `pandasai-2.1a1/pandasai/pipelines/chat/prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/result_parsing.py` & `pandasai-2.1a1/pandasai/pipelines/chat/result_parsing.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/result_validation.py` & `pandasai-2.1a1/pandasai/pipelines/chat/result_validation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/chat/validate_pipeline_input.py` & `pandasai-2.1a1/pandasai/pipelines/chat/validate_pipeline_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,15 @@
         Raises:
             InvalidConfigError: Raise Error in case of config is set but criteria is not met
         """
 
         if self.context.config.direct_sql:
             if all(
                 (isinstance(df, SQLConnector) and df.equals(dfs[0])) for df in dfs
-            ) or all(
-                (isinstance(df, PandasConnector) and df.sql_enabled) for df in dfs
-            ):
+            ) or all((isinstance(df, PandasConnector) and df.sql_enabed) for df in dfs):
                 return True
             else:
                 raise InvalidConfigError(
                     "Direct requires all Connector and they belong to same datasource "
                     "and have same credentials"
                 )
         return False
```

### Comparing `pandasai-2.1/pandasai/pipelines/logic_unit_output.py` & `pandasai-2.1a1/pandasai/pipelines/logic_unit_output.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/logic_units/output_logic_unit.py` & `pandasai-2.1a1/pandasai/pipelines/logic_units/output_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/pipelines/pipeline_context.py` & `pandasai-2.1a1/pandasai/pipelines/pipeline_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         self.intermediate_values = initial_values or {}
 
         self.vectorstore = vectorstore
 
         self._initial_values = initial_values
 
     def reset_intermediate_values(self):
+        print(self._initial_values)
         self.intermediate_values = self._initial_values or {}
+        print(self.intermediate_values)
 
     def add(self, key: str, value: Any):
         self.intermediate_values[key] = value
 
     def add_many(self, values: dict):
         self.intermediate_values.update(values)
```

### Comparing `pandasai-2.1/pandasai/prompts/base.py` & `pandasai-2.1a1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/clarification_questions_prompt.py` & `pandasai-2.1a1/pandasai/prompts/clarification_questions_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/correct_output_type_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_output_type_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/direct_sql_prompt.py` & `pandasai-2.1a1/pandasai/prompts/direct_sql_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/file_based_prompt.py` & `pandasai-2.1a1/pandasai/prompts/file_based_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/generate_python_code.py` & `pandasai-2.1a1/pandasai/prompts/generate_python_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,13 @@
         # prepare datasets
         datasets = [dataset.to_json() for dataset in context.dfs]
 
         return {
             "datasets": datasets,
             "conversation": conversations,
             "system_prompt": system_prompt,
-            "prompt": self.to_string(),
             "config": {
                 "direct_sql": context.config.direct_sql,
                 "viz_lib": viz_lib,
                 "output_type": output_type,
             },
         }
```

### Comparing `pandasai-2.1/pandasai/prompts/templates/clarification_questions_prompt.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/clarification_questions_prompt.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/templates/generate_python_code.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/generate_python_code.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/templates/shared/output_type_template.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/shared/output_type_template.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/prompts/templates/shared/vectordb_docs.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/shared/vectordb_docs.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/responses/context.py` & `pandasai-2.1a1/pandasai/responses/context.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/responses/response_parser.py` & `pandasai-2.1a1/pandasai/responses/response_parser.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/responses/response_serializer.py` & `pandasai-2.1a1/pandasai/responses/response_serializer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/responses/streamlit_response.py` & `pandasai-2.1a1/pandasai/responses/streamlit_response.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/schemas/df_config.py` & `pandasai-2.1a1/pandasai/schemas/df_config.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/skills/__init__.py` & `pandasai-2.1a1/pandasai/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/smart_dataframe/__init__.py` & `pandasai-2.1a1/pandasai/smart_dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/smart_datalake/__init__.py` & `pandasai-2.1a1/pandasai/smart_datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/vectorstores/bamboo_vectorstore.py` & `pandasai-2.1a1/pandasai/vectorstores/bamboo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pandasai/vectorstores/vectorstore.py` & `pandasai-2.1a1/pandasai/vectorstores/vectorstore.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.1/pyproject.toml` & `pandasai-2.1a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "2.1"
+version = "2.1a1"
 description = "Chat with your database (SQL, CSV, pandas, polars, mongodb, noSQL, etc). PandasAI makes data analysis conversational using LLMs (GPT 3.5 / 4, Anthropic, VertexAI) and RAG."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -45,17 +45,16 @@
 snowflake-sqlalchemy = { version = "^1.5.0", optional = true }
 flask = { version = "^3.0.2", optional = true }
 sqlalchemy-cockroachdb = { version = "^2.0.2", optional = true }
 sqlalchemy-bigquery = {version = "^1.8.0", optional = true, markers = "python_version >= '3.8' and python_version < '3.13'"}
 chromadb = {version = "^0.4.22", optional = true}
 boto3 = { version = ">=1.34.59", optional = true }
 qdrant-client = {version = "^1.8.0", extras = ["fastembed"], optional = true }
-ibm-watsonx-ai = { version = "^0.2.3", optional = true,  markers = "python_version >= '3.10'"}
+ibm-watsonx-ai = { version = "^0.2.3", optional = true , markers = "python_version >= '3.10'"}
 cx-Oracle = { version = "^8.3.0", optional = true }
-pinecone-client = { version = "^4.1.0", optional = true, markers = "python_version >= '3.10'"}
 
 [tool.poetry.group.dev]
 optional = true
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
@@ -86,15 +85,14 @@
 text-generation = ["fsspec", "huggingface-hub", "text-generation"]
 yfinance = ["yfinance"]
 modin = ["modin", "ray"]
 chromadb = ["chromadb"]
 bedrock = ["boto3"]
 flask = ["flask"]
 qdrant = ["qdrant-client"]
-pinecone = ["pinecone-client"]
 ibm-watsonx-ai = ["ibm-watsonx-ai"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
```

### Comparing `pandasai-2.1/PKG-INFO` & `pandasai-2.1a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 2.1
+Version: 2.1a1
 Summary: Chat with your database (SQL, CSV, pandas, polars, mongodb, noSQL, etc). PandasAI makes data analysis conversational using LLMs (GPT 3.5 / 4, Anthropic, VertexAI) and RAG.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,14 @@
 Provides-Extra: ggplot
 Provides-Extra: google-ai
 Provides-Extra: google-sheets
 Provides-Extra: ibm-watsonx-ai
 Provides-Extra: langchain
 Provides-Extra: modin
 Provides-Extra: numpy
-Provides-Extra: pinecone
 Provides-Extra: plotly
 Provides-Extra: polars
 Provides-Extra: qdrant
 Provides-Extra: scikit-learn
 Provides-Extra: seaborn
 Provides-Extra: statsmodels
 Provides-Extra: streamlit
@@ -51,15 +50,14 @@
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: modin[ray] (==0.18.1) ; extra == "modin"
 Requires-Dist: numpy (>=1.17,<2.0) ; extra == "numpy"
 Requires-Dist: openai (<2)
 Requires-Dist: openpyxl (>=3.0.7,<4.0.0) ; extra == "excel"
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
-Requires-Dist: pinecone-client (>=4.1.0,<5.0.0) ; (python_version >= "3.10") and (extra == "pinecone")
 Requires-Dist: plotly (>=5.15.0,<6.0.0) ; extra == "plotly"
 Requires-Dist: polars (>=0.18.15,<0.19.0) ; extra == "polars"
 Requires-Dist: psycopg2-binary (>=2.9.7,<3.0.0) ; extra == "connectors"
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0) ; extra == "connectors"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: qdrant-client[fastembed] (>=1.8.0,<2.0.0) ; extra == "qdrant"
```

