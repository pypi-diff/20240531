# Comparing `tmp/zlai-0.3.75.tar.gz` & `tmp/zlai-0.3.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlai-0.3.75.tar", last modified: Tue May 28 02:47:07 2024, max compression
+gzip compressed data, was "zlai-0.3.76.tar", last modified: Fri May 31 03:39:24 2024, max compression
```

## Comparing `zlai-0.3.75.tar` & `zlai-0.3.76.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.284833 zlai-0.3.75/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-28 02:47:07.284833 zlai-0.3.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 02:43:16.000000 zlai-0.3.75/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:47:07.284833 zlai-0.3.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 02:43:16.000000 zlai-0.3.75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.244833 zlai-0.3.75/zlai/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.252833 zlai-0.3.75/zlai/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.256833 zlai-0.3.75/zlai/agent/echarts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/echarts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/echarts/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/fund.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.260833 zlai-0.3.75/zlai/agent/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/auto_web.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/bing.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/fund.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/pyecharts.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/prompt/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/pyecharts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/task_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/try_times.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.264833 zlai-0.3.75/zlai/agent/v_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/v_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/v_1/fund.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.264833 zlai-0.3.75/zlai/agent/web/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/auto_web_selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/auto_web_unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/agent/web/web_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.264833 zlai-0.3.75/zlai/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/database/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)    20101 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/database/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.264833 zlai-0.3.75/zlai/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/dispatch/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.268833 zlai-0.3.75/zlai/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/elasticsearch/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.268833 zlai-0.3.75/zlai/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/ali.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/emb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/embedding/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.272833 zlai-0.3.75/zlai/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/ali.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.272833 zlai-0.3.75/zlai/llms/generate_config/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/ali.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/yi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/generate_config/zhipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/yi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/llms/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.276833 zlai-0.3.75/zlai/parse/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/parse/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/parse/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.276833 zlai-0.3.75/zlai/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/prompt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/prompt/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/prompt/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/prompt/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.280833 zlai-0.3.75/zlai/retrievers/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/retrievers/spliter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.280833 zlai-0.3.75/zlai/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/content.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/schema/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.280833 zlai-0.3.75/zlai/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/streamlit/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.280833 zlai-0.3.75/zlai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/utils/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.284833 zlai-0.3.75/zlai/vector_db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/vector_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/vector_db/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.284833 zlai-0.3.75/zlai/vector_db/milvus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/vector_db/milvus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/vector_db/milvus/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/vector_db/milvus/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.284833 zlai-0.3.75/zlai/warpper/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/warpper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-28 02:43:16.000000 zlai-0.3.75/zlai/warpper/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:47:07.284833 zlai-0.3.75/zlai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-28 02:47:07.000000 zlai-0.3.75/zlai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-28 02:47:07.000000 zlai-0.3.75/zlai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:47:07.000000 zlai-0.3.75/zlai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 02:47:07.000000 zlai-0.3.75/zlai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 02:47:07.000000 zlai-0.3.75/zlai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.325091 zlai-0.3.76/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-31 03:39:24.325091 zlai-0.3.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 03:35:46.000000 zlai-0.3.76/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:39:24.325091 zlai-0.3.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 03:35:46.000000 zlai-0.3.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.289091 zlai-0.3.76/zlai/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.297091 zlai-0.3.76/zlai/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.297091 zlai-0.3.76/zlai/agent/echarts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/echarts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/echarts/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/fund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.301091 zlai-0.3.76/zlai/agent/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/auto_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/fund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/pyecharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/prompt/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/pyecharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/try_times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.301091 zlai-0.3.76/zlai/agent/v_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/v_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/v_1/fund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.305091 zlai-0.3.76/zlai/agent/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/auto_web_selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/auto_web_unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/agent/web/web_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.305091 zlai-0.3.76/zlai/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/database/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20101 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/database/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.305091 zlai-0.3.76/zlai/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/dispatch/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.305091 zlai-0.3.76/zlai/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/elasticsearch/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.309091 zlai-0.3.76/zlai/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/ali.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/emb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14798 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/embedding/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.313091 zlai-0.3.76/zlai/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/ali.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.313091 zlai-0.3.76/zlai/llms/generate_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/ali.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/yi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/generate_config/zhipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/yi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/llms/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.313091 zlai-0.3.76/zlai/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/parse/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/parse/sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.317091 zlai-0.3.76/zlai/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/prompt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/prompt/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/prompt/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/prompt/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.317091 zlai-0.3.76/zlai/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/retrievers/spliter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.321091 zlai-0.3.76/zlai/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/schema/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.321091 zlai-0.3.76/zlai/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/streamlit/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.321091 zlai-0.3.76/zlai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/utils/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.321091 zlai-0.3.76/zlai/vector_db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/vector_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/vector_db/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.321091 zlai-0.3.76/zlai/vector_db/milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/vector_db/milvus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/vector_db/milvus/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/vector_db/milvus/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.325091 zlai-0.3.76/zlai/warpper/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/warpper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-31 03:35:46.000000 zlai-0.3.76/zlai/warpper/sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:39:24.325091 zlai-0.3.76/zlai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-31 03:39:24.000000 zlai-0.3.76/zlai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-31 03:39:24.000000 zlai-0.3.76/zlai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:39:24.000000 zlai-0.3.76/zlai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 03:39:24.000000 zlai-0.3.76/zlai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 03:39:24.000000 zlai-0.3.76/zlai.egg-info/top_level.txt
```

### Comparing `zlai-0.3.75/PKG-INFO` & `zlai-0.3.76/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlai
-Version: 0.3.75
+Version: 0.3.76
 Summary: llm
 Home-page: https://zlai-llm.github.io/zlai-doc/#/
 Author: chensy
 Author-email: chensy.cao@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,16 @@
 Requires-Dist: transformers>=4.35.2
 Requires-Dist: dataclasses>=0.6
 Requires-Dist: pydantic>=1.9.0
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: setuptools>=58.1.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: termcolor>=2.3.0
-Requires-Dist: elasticsearch==7.17.9
-Requires-Dist: elasticsearch_dsl==7.4.1
+Requires-Dist: elasticsearch>=8.12.0
+Requires-Dist: elasticsearch_dsl>=8.12.0
 Requires-Dist: pypdf
 Requires-Dist: unstructured[pdf]>=0.10.5
 Requires-Dist: huggingface_hub==0.20.1
 Requires-Dist: sentencepiece>=0.1.99
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: zhipuai>=2.0.1
 Requires-Dist: dashscope>=1.14.1
```

### Comparing `zlai-0.3.75/setup.py` & `zlai-0.3.76/setup.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/__init__.py` & `zlai-0.3.76/zlai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/address.py` & `zlai-0.3.76/zlai/agent/address.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/agent.py` & `zlai-0.3.76/zlai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/base.py` & `zlai-0.3.76/zlai/agent/base.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/chat.py` & `zlai-0.3.76/zlai/agent/chat.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/csv.py` & `zlai-0.3.76/zlai/agent/csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,57 +93,14 @@
     def _trans_invoke_data_str(self, data: Union[pd.DataFrame, pd.Series, str]) -> str:
         """"""
         if isinstance(data, (pd.DataFrame, pd.Series)):
             return data.to_markdown()
         else:
             return str(data)
 
-    def generate(
-            self,
-            query: str,
-    ):
-        """"""
-        self._logger(msg=f"[{self.agent_name}] Start ...\n", color="green")
-        self._logger(msg=f"[{self.agent_name}] Question: {query}\n", color="green")
-        messages = self._make_messages(content=query, df_head_markdown=self.df.head().to_markdown())
-        while True:
-            completion = self.llm.generate(messages=messages)
-            messages.append(completion.choices[0].message)
-            content = completion.choices[0].message.content
-            self._logger(msg=f"[{self.agent_name}] Assistant: {content}\n", color="green")
-            codes = ParseCode.sparse_script(string=content, script="python")
-
-            if len(codes) > 0:
-                code = codes[0]
-            else:
-                self._logger(msg=f"[{self.agent_name}] End ...\n", color="green")
-                return completion
-
-            self._logger(msg=f"[{self.agent_name}] Parsed code: ```\n{code}\n```", color="magenta")
-            invoke_data = self.tool.invoke(input=code)
-            invoke_data = self._trans_invoke_data_str(data=invoke_data)
-            self._logger(msg=f"[{self.agent_name}] Tools invoke: {invoke_data}\n", color="green")
-
-            # observation
-            observation_messages = [PromptDataFrame.system_message_dataframe_summary]
-            observation_messages.extend([
-                UserMessage(content=query),
-                AssistantMessage(content=content),
-                UserMessage(
-                    content=PromptDataFrame.prompt_dataframe_observation_summary.format_prompt(
-                        question=query, observation=invoke_data).to_string()),
-            ])
-            self._show_messages(messages=observation_messages, drop_system=True, content_length=-1, logger_name=self.agent_name)
-
-            completion = self.llm.generate(messages=observation_messages)
-            answer = completion.choices[0].message.content
-            self._logger(msg=f"[{self.agent_name}] Final Answer: {answer}.", color="yellow")
-            self._logger(msg=f"[{self.agent_name}] End ...\n", color="green")
-            return answer
-
 
 class CSVQA(AgentObservationMixin, CSVAgent):
     """"""
 
     def __init__(
             self,
             csv_path: Optional[str] = None,
```

### Comparing `zlai-0.3.75/zlai/agent/dataframe.py` & `zlai-0.3.76/zlai/agent/dataframe.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/echarts/charts.py` & `zlai-0.3.76/zlai/agent/echarts/charts.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/fund.py` & `zlai-0.3.76/zlai/agent/fund.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/knowledge.py` & `zlai-0.3.76/zlai/agent/knowledge.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/policy.py` & `zlai-0.3.76/zlai/agent/policy.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/address.py` & `zlai-0.3.76/zlai/agent/prompt/address.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/auto_web.py` & `zlai-0.3.76/zlai/agent/prompt/auto_web.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/bing.py` & `zlai-0.3.76/zlai/agent/prompt/bing.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/chat.py` & `zlai-0.3.76/zlai/agent/prompt/chat.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/csv.py` & `zlai-0.3.76/zlai/agent/prompt/csv.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/fund.py` & `zlai-0.3.76/zlai/agent/prompt/fund.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/knowledge.py` & `zlai-0.3.76/zlai/agent/prompt/knowledge.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/pyecharts.py` & `zlai-0.3.76/zlai/agent/prompt/pyecharts.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/sqlite.py` & `zlai-0.3.76/zlai/agent/prompt/sqlite.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/tasks.py` & `zlai-0.3.76/zlai/agent/prompt/tasks.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/prompt/weather.py` & `zlai-0.3.76/zlai/agent/prompt/weather.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/pyecharts.py` & `zlai-0.3.76/zlai/agent/pyecharts.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/shell.py` & `zlai-0.3.76/zlai/agent/shell.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/sql.py` & `zlai-0.3.76/zlai/agent/sql.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/sqlite.py` & `zlai-0.3.76/zlai/agent/sqlite.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/task_description.py` & `zlai-0.3.76/zlai/agent/task_description.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/tasks.py` & `zlai-0.3.76/zlai/agent/tasks.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/try_times.py` & `zlai-0.3.76/zlai/agent/try_times.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/v_1/fund.py` & `zlai-0.3.76/zlai/agent/v_1/fund.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/weather.py` & `zlai-0.3.76/zlai/agent/weather.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/web/auto_web_selenium.py` & `zlai-0.3.76/zlai/agent/web/auto_web_selenium.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/web/auto_web_unstructured.py` & `zlai-0.3.76/zlai/agent/web/auto_web_unstructured.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/web/bing.py` & `zlai-0.3.76/zlai/agent/web/bing.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/web/links.py` & `zlai-0.3.76/zlai/agent/web/links.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/agent/web/web_search.py` & `zlai-0.3.76/zlai/agent/web/web_search.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/database/spark.py` & `zlai-0.3.76/zlai/database/spark.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/database/sql.py` & `zlai-0.3.76/zlai/database/sql.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/dispatch/dispatch.py` & `zlai-0.3.76/zlai/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/elasticsearch/config.py` & `zlai-0.3.76/zlai/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/elasticsearch/document.py` & `zlai-0.3.76/zlai/elasticsearch/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     batch_size: Optional[int]
     thresh: Optional[float]
     logger: Optional[Callable]
     verbose: Optional[bool]
 
     def __init__(
             self,
+            host: Optional[str],
             index_name: Optional[str],
             tools: Optional[ElasticSearchTools] = None,
             embedding: Optional[Embedding] = None,
             batch_size: Optional[int] = 32,
             thresh: Optional[float] = 1.95,
             logger: Optional[Callable] = None,
             verbose: Optional[bool] = False,
@@ -58,15 +59,15 @@
         self.index_name = index_name
         self.tools = tools
         self.embedding = embedding
         self.batch_size = batch_size
         self.thresh = thresh
         self.logger = logger
         self.verbose = verbose
-        self.con = get_es_con(hosts=ESUrl.url)
+        self.con = get_es_con(hosts=host)
         self.tools = ElasticSearchTools(index_name=self.index_name, con=self.con)
 
     def __call__(self, data: List[Dict], *args, **kwargs):
         """"""
         documents_count = self.tools.count()
         self._logger(color="blue", msg=f"Start saving data to ElasticSearch, current document: {documents_count} ...")
         if documents_count > 0:
```

### Comparing `zlai-0.3.75/zlai/elasticsearch/elasticsearch.py` & `zlai-0.3.76/zlai/elasticsearch/elasticsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             self.search_query.append(_filter)
 
         combined_query = reduce(lambda q1, q2: q1 & q2, self.search_query)
         self.search_exe = self.search.query(combined_query)
 
     def match_context(
             self,
-            key_word: Union[str, None],
+            key_word: Union[str, None] = None,
             fields: Union[List[str], str, None] = None,
             match_type='match',
             **kwargs
     ) -> None:
         """
         :param key_word:
         :param fields:
@@ -313,15 +313,15 @@
         else:
             query = Q("terms", **{field: values})
         self.add_search_execute(query)
 
     def cos_smi(self, vector, doc_vec_name='vector') -> None:
         """"""
         script = {
-            "source": f"cosineSimilarity(params.query_vector, doc['{doc_vec_name}']) + 1.0",
+            "source": f"cosineSimilarity(params.query_vector, '{doc_vec_name}') + 1.0",
             "params": {"query_vector": vector}
         }
         query = ScriptScore(query=MatchAll(), script=script)
         self.add_search_execute(query=query)
 
     def agg_metric(self, field: str, op: str):
         """"""
```

### Comparing `zlai-0.3.75/zlai/embedding/ali.py` & `zlai-0.3.76/zlai/embedding/ali.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/embedding/emb_utils.py` & `zlai-0.3.76/zlai/embedding/emb_utils.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/embedding/embedding.py` & `zlai-0.3.76/zlai/embedding/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,20 @@
     "Embedding",
     "EmbeddingMixin",
     "EmbeddingCompletion",
 ]
 
 headers = {'Content-Type': 'application/json'}
 
+emb_url = EMBUrl()
+
 
 class EmbeddingCompletion(LoggerMixin):
     """"""
-    emb_url: Union[str, EMBUrl, None] = EMBUrl.bge_m3
+    emb_url: Union[str, EMBUrl, None] = emb_url.bge_m3
     model_name: Optional[EmbeddingsModel] = None
     max_len: int = 512
     instruction: bool = False
     max_len_error: Literal['split', 'drop', 'error'] = 'split'
     model_path = Optional[str]
     batch_size = Optional[int]
     api_key: Optional[str] = None
@@ -133,15 +135,15 @@
             return self.pretrained_model_embedding(text=text)
         else:
             raise ValueError(f"{self.emb_url} or {self.model_name} is not supported.")
 
 
 class EmbeddingMixin(EmbeddingCompletion):
     """"""
-    emb_url: Union[str, EMBUrl, None] = EMBUrl.bge_m3
+    emb_url: Union[str, EMBUrl, None] = emb_url.bge_m3
     model_name: Optional[EmbeddingsModel] = None
     max_len: int = 512
     instruction: bool = False
     max_len_error: Literal['split', 'drop', 'error'] = 'split'
     verbose: bool = False
 
     def trans_any_vectors(self, vectors: Union[EmbeddingsResponded, np.ndarray, List[List[float]]]) -> np.ndarray:
@@ -333,15 +335,15 @@
             return self._merge_match_output(score_match, keyword_match)
         else:
             return score_match + keyword_match
 
 
 class Embedding(EmbeddingMixin):
     """"""
-    emb_url: Union[str, EMBUrl, None] = EMBUrl.bge_m3
+    emb_url: Union[str, EMBUrl, None] = emb_url.bge_m3
     model_name: Optional[EmbeddingsModel] = None
     max_len: int = 512
     instruction: bool = False
     max_len_error: Literal['split', 'drop', 'error'] = 'split'
     verbose: bool = False
     model_path = Optional[str]
     batch_size = Optional[int]
@@ -367,15 +369,15 @@
 
         # local
         self.emb_url = emb_url
         self.model_name = model_name
         self.max_len = max_len
         self.instruction = instruction
         self.max_len_error = max_len_error
-        self.emb_metadata = get_dataclass_metadata(cls=EMBUrl)
+        # self.emb_metadata = get_dataclass_metadata(cls=EMBUrl)
 
         # from pretrained model
         self.model_path = model_path
         self.batch_size = batch_size
 
     def __call__(
             self,
```

### Comparing `zlai-0.3.75/zlai/embedding/embedding_config.py` & `zlai-0.3.76/zlai/embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/embedding/zhipu.py` & `zlai-0.3.76/zlai/embedding/zhipu.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/ali.py` & `zlai-0.3.76/zlai/llms/ali.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/atom.py` & `zlai-0.3.76/zlai/llms/atom.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/base.py` & `zlai-0.3.76/zlai/llms/base.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/deepseek.py` & `zlai-0.3.76/zlai/llms/deepseek.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate.py` & `zlai-0.3.76/zlai/llms/generate.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/ali.py` & `zlai-0.3.76/zlai/llms/generate_config/ali.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/atom.py` & `zlai-0.3.76/zlai/llms/generate_config/atom.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/baichuan.py` & `zlai-0.3.76/zlai/llms/generate_config/baichuan.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/base.py` & `zlai-0.3.76/zlai/llms/generate_config/base.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/deepseek.py` & `zlai-0.3.76/zlai/llms/generate_config/deepseek.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/local.py` & `zlai-0.3.76/zlai/llms/generate_config/local.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/moonshot.py` & `zlai-0.3.76/zlai/llms/generate_config/moonshot.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/yi.py` & `zlai-0.3.76/zlai/llms/generate_config/yi.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/generate_config/zhipu.py` & `zlai-0.3.76/zlai/llms/generate_config/zhipu.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/local.py` & `zlai-0.3.76/zlai/llms/local.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/moonshot.py` & `zlai-0.3.76/zlai/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/yi.py` & `zlai-0.3.76/zlai/llms/yi.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/llms/zhipu.py` & `zlai-0.3.76/zlai/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/parse/amount.py` & `zlai-0.3.76/zlai/parse/amount.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/parse/sparse.py` & `zlai-0.3.76/zlai/parse/sparse.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/prompt/base.py` & `zlai-0.3.76/zlai/prompt/base.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/prompt/tools.py` & `zlai-0.3.76/zlai/prompt/tools.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/retrievers/clean.py` & `zlai-0.3.76/zlai/retrievers/clean.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/retrievers/rag.py` & `zlai-0.3.76/zlai/retrievers/rag.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/retrievers/retrievers.py` & `zlai-0.3.76/zlai/retrievers/retrievers.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/retrievers/spliter.py` & `zlai-0.3.76/zlai/retrievers/spliter.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/content.py` & `zlai-0.3.76/zlai/schema/content.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/messages.py` & `zlai-0.3.76/zlai/schema/messages.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/models.py` & `zlai-0.3.76/zlai/schema/models.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/request.py` & `zlai-0.3.76/zlai/schema/request.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/response.py` & `zlai-0.3.76/zlai/schema/response.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/schema/url.py` & `zlai-0.3.76/zlai/schema/url.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/streamlit/web.py` & `zlai-0.3.76/zlai/streamlit/web.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/utils/config.py` & `zlai-0.3.76/zlai/utils/config.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/utils/mixin.py` & `zlai-0.3.76/zlai/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/utils/utils.py` & `zlai-0.3.76/zlai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/vector_db/milvus/collection.py` & `zlai-0.3.76/zlai/vector_db/milvus/collection.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai/warpper/sparse.py` & `zlai-0.3.76/zlai/warpper/sparse.py`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai.egg-info/PKG-INFO` & `zlai-0.3.76/zlai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlai
-Version: 0.3.75
+Version: 0.3.76
 Summary: llm
 Home-page: https://zlai-llm.github.io/zlai-doc/#/
 Author: chensy
 Author-email: chensy.cao@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,16 @@
 Requires-Dist: transformers>=4.35.2
 Requires-Dist: dataclasses>=0.6
 Requires-Dist: pydantic>=1.9.0
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: setuptools>=58.1.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: termcolor>=2.3.0
-Requires-Dist: elasticsearch==7.17.9
-Requires-Dist: elasticsearch_dsl==7.4.1
+Requires-Dist: elasticsearch>=8.12.0
+Requires-Dist: elasticsearch_dsl>=8.12.0
 Requires-Dist: pypdf
 Requires-Dist: unstructured[pdf]>=0.10.5
 Requires-Dist: huggingface_hub==0.20.1
 Requires-Dist: sentencepiece>=0.1.99
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: zhipuai>=2.0.1
 Requires-Dist: dashscope>=1.14.1
```

### Comparing `zlai-0.3.75/zlai.egg-info/SOURCES.txt` & `zlai-0.3.76/zlai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zlai-0.3.75/zlai.egg-info/requires.txt` & `zlai-0.3.76/zlai.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 transformers>=4.35.2
 dataclasses>=0.6
 pydantic>=1.9.0
 numpy>=1.23.5
 setuptools>=58.1.0
 tqdm>=4.65.0
 termcolor>=2.3.0
-elasticsearch==7.17.9
-elasticsearch_dsl==7.4.1
+elasticsearch>=8.12.0
+elasticsearch_dsl>=8.12.0
 pypdf
 unstructured[pdf]>=0.10.5
 huggingface_hub==0.20.1
 sentencepiece>=0.1.99
 beautifulsoup4>=4.12.2
 zhipuai>=2.0.1
 dashscope>=1.14.1
```

