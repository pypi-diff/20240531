# Comparing `tmp/langtrace_python_sdk-2.1.4.tar.gz` & `tmp/langtrace_python_sdk-2.1.5.tar.gz`

## Comparing `langtrace_python_sdk-2.1.4.tar` & `langtrace_python_sdk-2.1.5.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/weaviate_example/query_text.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/misc.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/prompt_registry.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/silently_fail.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/types.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/chroma/conftest.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/conftest.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/cassettes/test_langchain.yaml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/conftest.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_query.yaml
--rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_upsert.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/qdrant/conftest.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/qdrant/test_qdrant.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/LICENSE
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/README.md
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/pyproject.toml
--rw-r--r--   0        0        0    11769 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0    64491 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/examples/weaviate_example/query_text.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/misc.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/prompt_registry.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/silently_fail.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/types.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/chroma/conftest.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/langchain/conftest.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/langchain/cassettes/test_langchain.yaml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/pinecone/conftest.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/pinecone/cassettes/test_query.yaml
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/pinecone/cassettes/test_upsert.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/qdrant/conftest.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/src/tests/qdrant/test_qdrant.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/LICENSE
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/README.md
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0    11833 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.5/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.1.4/src/run_example.py` & `langtrace_python_sdk-2.1.5/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.1.5/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.1.5/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.1.5/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.1.5/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.1.5/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.1.5/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.1.5/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.1.5/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.1.5/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.1.5/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.1.5/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.1.5/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.1.5/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/examples/weaviate_example/query_text.py` & `langtrace_python_sdk-2.1.5/src/examples/weaviate_example/query_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from weaviate.classes.query import Filter, HybridFusion, MetadataQuery
 from weaviate.collections.classes.grpc import Move
 
 import langtrace_python_sdk.langtrace as langtrace
 from langtrace_python_sdk import with_langtrace_root_span
 
 # Set these environment variables
-WCS_DEMO_URL = "WEVIATE CLUSTER URL"
-WCS_DEMO_RO_KEY = "<WEAVIATE API KEY>"
+WCS_DEMO_URL = os.environ["WCS_DEMO_URL"]
+WCS_DEMO_RO_KEY = os.environ["WCS_DEMO_RO_KEY"]
 
 # Connect to a WCS instance
 client = weaviate.connect_to_wcs(
     cluster_url=WCS_DEMO_URL,
     auth_credentials=weaviate.auth.AuthApiKey(WCS_DEMO_RO_KEY),
     skip_init_checks=True,
     headers={"X-OpenAI-Api-Key": os.environ["OPENAI_APIKEY"]},
 )
 
-langtrace.init(api_key="asdf", write_spans_to_console=True, batch=False)
+langtrace.init()
 
 
 @with_langtrace_root_span()
 def create():
     questions = client.collections.create(
         name="Question",
         # Set the vectorizer to "text2vec-openai" to use the OpenAI API for vector-related operations
```

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/langtrace.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,54 +24,30 @@
     ConsoleSpanExporter,
     SimpleSpanProcessor,
 )
 import sys
 from opentelemetry.sdk.resources import Resource
 
 from langtrace_python_sdk.extensions.langtrace_exporter import LangTraceExporter
-from langtrace_python_sdk.instrumentation.anthropic.instrumentation import (
+from langtrace_python_sdk.instrumentation import (
     AnthropicInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.chroma.instrumentation import (
     ChromaInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.cohere.instrumentation import (
     CohereInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.groq.instrumentation import (
     GroqInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.langchain.instrumentation import (
     LangchainInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.langchain_community.instrumentation import (
     LangchainCommunityInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.langchain_core.instrumentation import (
     LangchainCoreInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.langgraph.instrumentation import (
     LanggraphInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.llamaindex.instrumentation import (
     LlamaindexInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.openai.instrumentation import (
     OpenAIInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.pinecone.instrumentation import (
     PineconeInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.qdrant.instrumentation import (
     QdrantInstrumentation,
-)
-from langtrace_python_sdk.instrumentation.weaviate.instrumentation import (
     WeaviateInstrumentation,
 )
-
+from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from colorama import Fore
 
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_spans_to_console: bool = False,
@@ -93,15 +69,15 @@
     simple_processor_console = SimpleSpanProcessor(console_exporter)
 
     if write_spans_to_console:
         print(Fore.BLUE + "Writing spans to console" + Fore.RESET)
         provider.add_span_processor(simple_processor_console)
 
     elif custom_remote_exporter is not None:
-        print(Fore.BLUE + f"Exporting spans to custom remote exporter.." + Fore.RESET)
+        print(Fore.BLUE + "Exporting spans to custom remote exporter.." + Fore.RESET)
         if batch:
             provider.add_span_processor(batch_processor_remote)
         else:
             provider.add_span_processor(simple_processor_remote)
 
     elif api_host is not None:
         print(Fore.BLUE + f"Exporting spans to custom host: {api_host}.." + Fore.RESET)
@@ -126,14 +102,15 @@
         "langchain": LangchainInstrumentation(),
         "langchain_core": LangchainCoreInstrumentation(),
         "langchain_community": LangchainCommunityInstrumentation(),
         "langgraph": LanggraphInstrumentation(),
         "anthropic": AnthropicInstrumentation(),
         "cohere": CohereInstrumentation(),
         "weaviate": WeaviateInstrumentation(),
+        "sqlalchemy": SQLAlchemyInstrumentor(),
     }
 
     init_instrumentations(disable_instrumentations, all_instrumentations)
 
 
 def init_instrumentations(
     disable_instrumentations: DisableInstrumentations, all_instrumentations: dict
```

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/weaviate.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/constants/instrumentation/weaviate.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/patch.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/instrumentation/weaviate/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/misc.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/prompt_registry.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.1.5/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/utils.py` & `langtrace_python_sdk-2.1.5/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.1.5/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.1.5/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.1.5/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.1.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/langchain/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/langchain/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.1.5/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/langchain/cassettes/test_langchain.yaml` & `langtrace_python_sdk-2.1.5/src/tests/langchain/cassettes/test_langchain.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.1.5/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.1.5/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.1.5/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/pinecone/conftest.py` & `langtrace_python_sdk-2.1.5/src/tests/pinecone/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.1.5/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_query.yaml` & `langtrace_python_sdk-2.1.5/src/tests/pinecone/cassettes/test_query.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_upsert.yaml` & `langtrace_python_sdk-2.1.5/src/tests/pinecone/cassettes/test_upsert.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/src/tests/qdrant/test_qdrant.py` & `langtrace_python_sdk-2.1.5/src/tests/qdrant/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/.gitignore` & `langtrace_python_sdk-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/LICENSE` & `langtrace_python_sdk-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/README.md` & `langtrace_python_sdk-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.4/pyproject.toml` & `langtrace_python_sdk-2.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'trace-attributes>=4.0.4',
   'opentelemetry-api>=1.24.0',
   'opentelemetry-sdk>=1.24.0',
   'opentelemetry-instrumentation>=0.45b0',
-  'tiktoken>=0.1.1',
+  'opentelemetry-instrumentation-sqlalchemy>=0.45b0',
   'opentelemetry-exporter-otlp-proto-http>=1.24.0',
   'opentelemetry-exporter-otlp-proto-grpc>=1.24.0',
+  'tiktoken>=0.1.1',
   'colorama>=0.4.6'
+
 ]
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "openai",
```

### Comparing `langtrace_python_sdk-2.1.4/PKG-INFO` & `langtrace_python_sdk-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: opentelemetry-api>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.24.0
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy>=0.45b0
 Requires-Dist: opentelemetry-instrumentation>=0.45b0
 Requires-Dist: opentelemetry-sdk>=1.24.0
 Requires-Dist: tiktoken>=0.1.1
 Requires-Dist: trace-attributes>=4.0.4
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
```

