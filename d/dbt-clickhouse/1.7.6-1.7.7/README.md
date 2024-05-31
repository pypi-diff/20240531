# Comparing `tmp/dbt-clickhouse-1.7.6.tar.gz` & `tmp/dbt_clickhouse-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.7.6.tar", last modified: Sat Apr 13 01:05:16 2024, max compression
+gzip compressed data, was "dbt_clickhouse-1.7.7.tar", last modified: Fri May 31 13:59:45 2024, max compression
```

## Comparing `dbt-clickhouse-1.7.6.tar` & `dbt_clickhouse-1.7.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.228861 dbt-clickhouse-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/column_spec_ddl.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/dictionary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/distributed_table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:05:16.228861 dbt-clickhouse-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.982807 dbt_clickhouse-1.7.7/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.982807 dbt_clickhouse-1.7.7/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.986807 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.982807 dbt_clickhouse-1.7.7/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.986807 dbt_clickhouse-1.7.7/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.986807 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.986807 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/column_spec_ddl.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/dictionary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/distributed_table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-05-31 13:59:45.000000 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-31 13:59:45.000000 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:45.000000 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 13:59:45.000000 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 13:59:45.000000 dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:59:45.990808 dbt_clickhouse-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-31 13:59:41.000000 dbt_clickhouse-1.7.7/setup.py
```

### Comparing `dbt-clickhouse-1.7.6/LICENSE` & `dbt_clickhouse-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/PKG-INFO` & `dbt_clickhouse-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.6
+Version: 1.7.7
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-clickhouse-1.7.6/README.md` & `dbt_clickhouse-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__init__.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/cache.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/column.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/column.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,30 +13,26 @@
     TYPE_LABELS = {
         'STRING': 'String',
         'TIMESTAMP': 'DateTime',
         'FLOAT': 'Float32',
         'INTEGER': 'Int32',
     }
     is_nullable: bool = False
-    _brackets_regex = re.compile(r'^(Nullable|LowCardinality)\((.*)\)$')
+    is_low_cardinality: bool = False
+    _low_card_regex = re.compile(r'^LowCardinality\((.*)\)$')
+    _nullable_regex = re.compile(r'^Nullable\((.*)\)$')
     _fix_size_regex = re.compile(r'FixedString\((.*?)\)')
     _decimal_regex = re.compile(r'Decimal\((\d+), (\d+)\)')
 
     def __init__(self, column: str, dtype: str) -> None:
         char_size = None
         numeric_precision = None
         numeric_scale = None
 
-        inner_dtype = self.match_brackets(dtype)
-        if inner_dtype:
-            dtype = inner_dtype
-            if not self.is_nullable:
-                # Support LowCardinality(Nullable(dtype))
-                inner_dtype = self.match_brackets(dtype)
-                dtype = inner_dtype if inner_dtype else dtype
+        dtype = self._inner_dtype(dtype)
 
         if dtype.lower().startswith('fixedstring'):
             match_sized = self._fix_size_regex.search(dtype)
             if match_sized:
                 char_size = int(match_sized.group(1))
 
         if dtype.lower().startswith('decimal'):
@@ -52,26 +48,23 @@
     def __repr__(self) -> str:
         return f'<ClickhouseColumn {self.name} ({self.data_type}, is nullable: {self.is_nullable})>'
 
     @property
     def data_type(self) -> str:
         if self.is_string():
             data_t = self.string_type(self.string_size())
-            if self.is_nullable:
-                return "Nullable({})".format(data_t)
-            return data_t
         elif self.is_numeric():
             data_t = self.numeric_type(self.dtype, self.numeric_precision, self.numeric_scale)
-            if self.is_nullable:
-                return "Nullable({})".format(data_t)
-            return data_t
         else:
-            if self.is_nullable:
-                return "Nullable({})".format(self.dtype)
-            return self.dtype
+            data_t = self.dtype
+
+        if self.is_nullable or self.is_low_cardinality:
+            data_t = self.nested_type(data_t, self.is_low_cardinality, self.is_nullable)
+
+        return data_t
 
     def is_string(self) -> bool:
         return self.dtype.lower() in [
             'string',
             'fixedstring',
             'longblob',
             'longtext',
@@ -107,21 +100,37 @@
     def string_type(cls, size: int) -> str:
         return 'String'
 
     @classmethod
     def numeric_type(cls, dtype: str, precision: Any, scale: Any) -> str:
         return f'Decimal({precision}, {scale})'
 
+    @classmethod
+    def nested_type(cls, dtype: str, is_low_cardinality: bool, is_nullable: bool) -> str:
+        template = "{}"
+        if is_low_cardinality:
+            template = template.format("LowCardinality({})")
+        if is_nullable:
+            template = template.format("Nullable({})")
+        return template.format(dtype)
+
     def literal(self, value):
         return f'to{self.dtype}({value})'
 
     def can_expand_to(self, other_column: 'Column') -> bool:
         if not self.is_string() or not other_column.is_string():
             return False
 
         return other_column.string_size() > self.string_size()
 
-    def match_brackets(self, dtype):
-        match = self._brackets_regex.search(dtype.strip())
-        if match:
-            self.is_nullable = match.group(1) == 'Nullable'
-            return match.group(2)
+    def _inner_dtype(self, dtype) -> str:
+        inner_dtype = dtype.strip()
+
+        if low_card_match := self._low_card_regex.search(inner_dtype):
+            self.is_low_cardinality = True
+            inner_dtype = low_card_match.group(1)
+
+        if null_match := self._nullable_regex.search(inner_dtype):
+            self.is_nullable = True
+            inner_dtype = null_match.group(1)
+
+        return inner_dtype
```

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/connections.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/credentials.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/dbclient.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/dbclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/errors.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/errors.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/httpclient.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/httpclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/impl.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,15 +451,15 @@
     def get_column_schema_from_query(self, sql: str, *_) -> List[ClickHouseColumn]:
         """Get a list of the Columns with names and data types from the given sql."""
         conn = self.connections.get_if_exists()
         return conn.handle.columns_in_query(sql)
 
     @available.parse_none
     def format_columns(self, columns) -> List[Dict]:
-        return [{'name': column.name, 'data_type': column.dtype} for column in columns]
+        return [{'name': column.name, 'data_type': column.data_type} for column in columns]
 
     @available
     def get_credentials(self, connection_overrides) -> Dict:
         conn = self.connections.get_if_exists()
         if conn is None or conn.credentials is None:
             return dict()
         credentials = {
@@ -477,15 +477,18 @@
 
         return credentials
 
     @classmethod
     def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
         rendered_columns = []
         for v in raw_columns.values():
-            rendered_columns.append(f"{quote_identifier(v['name'])} {v['data_type']}")
+            codec = f"CODEC({_codec})" if (_codec := v.get('codec')) else ""
+            rendered_columns.append(
+                f"{quote_identifier(v['name'])} {v['data_type']} {codec}".rstrip()
+            )
             if v.get("constraints"):
                 warn_or_error(ConstraintNotSupported(constraint='column', adapter='clickhouse'))
         return rendered_columns
 
     @classmethod
     def render_model_constraint(cls, constraint: ModelLevelConstraint) -> Optional[str]:
         if constraint.type == ConstraintType.check and constraint.expression:
```

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/nativeclient.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/nativeclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/relation.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/util.py` & `dbt_clickhouse-1.7.7/dbt/adapters/clickhouse/util.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/catalog.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/column_spec_ddl.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/column_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/dictionary.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/dictionary.sql`

 * *Files 5% similar despite different names*

```diff
@@ -78,24 +78,26 @@
 {% endmacro %}
 
 
 {% macro clickhouse_source(sql) %}
   {%- set credentials = adapter.get_credentials(config.get("connection_overrides", {})) -%}
   {%- set table = config.get('table') -%}
   CLICKHOUSE(
+      {% if credentials.get("user") -%}
       user '{{ credentials.get("user") }}'
-      {% if credentials.get("password") != '' -%}
+      {%- endif %}
+      {% if credentials.get("password") -%}
       password '{{ credentials.get("password") }}'
       {%- endif %}
-      {% if credentials.get("database") != '' -%}
+      {% if credentials.get("database") -%}
       db '{{ credentials.get("database") }}'
       {%- endif %}
-      {% if credentials.get("host") != '' and credentials.get("host") != 'localhost' -%}
+      {% if credentials.get("host") and credentials.get("host") != 'localhost' -%}
       host '{{ credentials.get("host") }}'
-      {% if credentials.get("port") != '' -%}
+      {% if credentials.get("port") -%}
       port '{{ credentials.get("port") }}'
       {%- endif %}
       {%- endif %}
       {%- if table is not none %}
         table '{{ table }}'
       {% else %}
         query "{{ sql }}"
```

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/distributed_table.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/distributed_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/materialized_view.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -198,10 +198,10 @@
   insert into {{ target_relation }}
         ({{ dest_cols_csv }})
   {%- if has_contract -%}
     -- Use a subquery to get columns in the right order
           SELECT {{ dest_cols_csv }} FROM ( {{ sql }} )
   {%- else -%}
       {{ sql }}
-  {{ adapter.get_model_query_settings(model) }}
   {%- endif -%}
+  {{ adapter.get_model_query_settings(model) }}
 {%- endmacro %}
```

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt_clickhouse-1.7.7/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 {% macro clickhouse__any_value(expression) -%}
     any({{ expression }})
 {%- endmacro %}
 
 
 {% macro clickhouse__bool_or(expression) -%}
-    any({{ expression }}) > 0
+    max({{ expression }}) > 0
 {%- endmacro %}
 
 
 {% macro clickhouse__cast_bool_to_text(field) %}
     multiIf({{ field }} > 0, 'true', {{ field }} = 0, 'false', NULL)
 {% endmacro %}
```

### Comparing `dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/PKG-INFO` & `dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.6
+Version: 1.7.7
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt_clickhouse-1.7.7/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.6/setup.py` & `dbt_clickhouse-1.7.7/setup.py`

 * *Files identical despite different names*

