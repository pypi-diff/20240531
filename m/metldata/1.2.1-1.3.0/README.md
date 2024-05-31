# Comparing `tmp/metldata-1.2.1.tar.gz` & `tmp/metldata-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metldata-1.2.1.tar", last modified: Tue Mar 26 15:19:13 2024, max compression
+gzip compressed data, was "metldata-1.3.0.tar", last modified: Fri May 31 12:07:38 2024, max compression
```

## Comparing `metldata-1.2.1.tar` & `metldata-1.3.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.740681 metldata-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-03-26 15:19:08.000000 metldata-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-03-26 15:19:13.740681 metldata-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19568 2024-03-26 15:19:08.000000 metldata-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-26 15:19:08.000000 metldata-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 15:19:13.740681 metldata-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.712681 metldata-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.716681 metldata-1.2.1/src/metldata/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.720681 metldata-1.2.1/src/metldata/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/accession_registry/accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/accession_registry/accession_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/accession_registry/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.720681 metldata-1.2.1/src/metldata/artifacts_rest/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/api_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/artifact_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/load_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/artifacts_rest/query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.720681 metldata-1.2.1/src/metldata/builtin_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.720681 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.724681 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/cached_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/data_subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/expanding_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/model_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/aggregate/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.724681 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.724681 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.728681 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.728681 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/infer_references/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.728681 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/model_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.732681 metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.732681 metldata-1.2.1/src/metldata/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/builtin_workflows/ghga_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.732681 metldata-1.2.1/src/metldata/event_handling/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/event_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/event_handling/artifact_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/event_handling/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/event_handling/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/event_handling/submission_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.732681 metldata-1.2.1/src/metldata/load/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/load/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.736681 metldata-1.2.1/src/metldata/model_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/anchors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/essentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/model_utils/metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.736681 metldata-1.2.1/src/metldata/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/submission_registry/submission_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.736681 metldata-1.2.1/src/metldata/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/artifact_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-26 15:19:08.000000 metldata-1.2.1/src/metldata/transform/source_event_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.740681 metldata-1.2.1/src/metldata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 15:19:13.000000 metldata-1.2.1/src/metldata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:19:13.740681 metldata-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-03-26 15:19:08.000000 metldata-1.2.1/tests/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-26 15:19:08.000000 metldata-1.2.1/tests/test_metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.582975 metldata-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-31 12:07:27.000000 metldata-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-05-31 12:07:38.582975 metldata-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-05-31 12:07:27.000000 metldata-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-31 12:07:27.000000 metldata-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:07:38.582975 metldata-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.558975 metldata-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.562975 metldata-1.3.0/src/metldata/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.562975 metldata-1.3.0/src/metldata/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/accession_registry/accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/accession_registry/accession_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/accession_registry/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.566975 metldata-1.3.0/src/metldata/artifacts_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/artifact_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/load_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/artifacts_rest/query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.566975 metldata-1.3.0/src/metldata/builtin_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.566975 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.566975 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/cached_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/data_subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/expanding_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/aggregate/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.570975 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.570975 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.570975 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.570975 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/infer_references/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.574975 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.574975 metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.574975 metldata-1.3.0/src/metldata/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/builtin_workflows/ghga_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.574975 metldata-1.3.0/src/metldata/event_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/event_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/event_handling/artifact_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/event_handling/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/event_handling/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/event_handling/submission_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.578975 metldata-1.3.0/src/metldata/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/load/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.578975 metldata-1.3.0/src/metldata/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/essentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/model_utils/metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.578975 metldata-1.3.0/src/metldata/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/submission_registry/submission_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.578975 metldata-1.3.0/src/metldata/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/artifact_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-31 12:07:27.000000 metldata-1.3.0/src/metldata/transform/source_event_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.582975 metldata-1.3.0/src/metldata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 12:07:38.000000 metldata-1.3.0/src/metldata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:07:38.582975 metldata-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-31 12:07:27.000000 metldata-1.3.0/tests/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-31 12:07:27.000000 metldata-1.3.0/tests/test_metadata_utils.py
```

### Comparing `metldata-1.2.1/LICENSE` & `metldata-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/PKG-INFO` & `metldata-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 1.2.1
+Version: 1.3.0
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/metldata
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hexkit[akafka,mongodb]<3,>=2.1.1
+Requires-Dist: hexkit[akafka,mongodb]<4,>=3
 Requires-Dist: ghga-service-commons[api,auth]<4,>=3.1.1
 Requires-Dist: ghga-event-schemas<4,>=3.0.0
-Requires-Dist: typer~=0.9.0
+Requires-Dist: typer>=0.12
 Requires-Dist: linkml==1.6.1
 Requires-Dist: linkml-runtime==1.6.0
 Requires-Dist: linkml-validator==0.4.5
+Requires-Dist: cryptography>=42.0.0
 
 [![tests](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/metldata/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/metldata?branch=main)
 
 # Metldata
 
 metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
@@ -81,29 +81,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:1.2.1
+docker pull ghga/metldata:1.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:1.2.1 .
+docker build -t ghga/metldata:1.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:1.2.1 --help
+docker run -p 8080:8080 ghga/metldata:1.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -166,15 +166,15 @@
 
 - **`kafka_ssl_cafile`** *(string)*: Certificate Authority file path containing certificates used to sign broker certificates. If a CA is not specified, the default system CA will be used if found by OpenSSL. Default: `""`.
 
 - **`kafka_ssl_certfile`** *(string)*: Optional filename of client certificate, as well as any CA certificates needed to establish the certificate's authenticity. Default: `""`.
 
 - **`kafka_ssl_keyfile`** *(string)*: Optional filename containing the client private key. Default: `""`.
 
-- **`kafka_ssl_password`** *(string)*: Optional password to be used for the client private key. Default: `""`.
+- **`kafka_ssl_password`** *(string, format: password)*: Optional password to be used for the client private key. Default: `""`.
 
 - **`generate_correlation_id`** *(boolean)*: A flag, which, if False, will result in an error when inbound requests don't possess a correlation ID. If True, requests without a correlation ID will be assigned a newly generated ID in the correlation ID middleware function. Default: `true`.
 
 
   Examples:
 
   ```json
@@ -357,20 +357,63 @@
   ```json
   []
   ```
 
 
 - **`artifact_infos`** *(array)*: Information for artifacts to be queryable via the Artifacts REST API.
 
-  - **Items**: Refer to *[#/$defs/ArtifactInfo](#$defs/ArtifactInfo)*.
+  - **Items**: Refer to *[#/$defs/ArtifactInfo](#%24defs/ArtifactInfo)*.
 
 - **`loader_token_hashes`** *(array)*: Hashes of tokens used to authenticate for loading artifact.
 
   - **Items** *(string)*
 
+## Definitions
+
+
+- <a id="%24defs/AnchorPoint"></a>**`AnchorPoint`** *(object)*: A model for describing an anchor point for the specified target class.
+
+  - **`target_class`** *(string, required)*: The name of the class to be targeted.
+
+  - **`identifier_slot`** *(string, required)*: The name of the slot in the target class that is used as identifier.
+
+  - **`root_slot`** *(string, required)*: The name of the slot in the root class used to link to the target class.
+
+- <a id="%24defs/ArtifactInfo"></a>**`ArtifactInfo`** *(object)*: Model to describe general information on an artifact.
+Please note, it does not contain actual artifact instances derived from specific
+metadata.
+
+  - **`name`** *(string, required)*: The name of the artifact.
+
+  - **`description`** *(string, required)*: A description of the artifact.
+
+  - **`resource_classes`** *(object, required)*: A dictionary of resource classes for this artifact. The keys are the names of the classes. The values are the corresponding class models. Can contain additional properties.
+
+    - **Additional properties**: Refer to *[#/$defs/ArtifactResourceClass](#%24defs/ArtifactResourceClass)*.
+
+- <a id="%24defs/ArtifactResourceClass"></a>**`ArtifactResourceClass`** *(object)*: Model to describe a resource class of an artifact.
+
+  - **`name`** *(string, required)*: The name of the metadata class.
+
+  - **`description`**: A description of the metadata class. Default: `null`.
+
+    - **Any of**
+
+      - *string*
+
+      - *null*
+
+  - **`anchor_point`**: The anchor point for this metadata class.
+
+    - **All of**
+
+      - : Refer to *[#/$defs/AnchorPoint](#%24defs/AnchorPoint)*.
+
+  - **`json_schema`** *(object, required)*: The JSON schema for this metadata class.
+
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.metldata.yaml`, and place it into one of the following locations:
 - in the current working directory were you are execute the service (on unix: `./.metldata.yaml`)
```

### Comparing `metldata-1.2.1/README.md` & `metldata-1.3.0/src/metldata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: metldata
+Version: 1.3.0
+Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
+Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
+License: Apache 2.0
+Project-URL: Repository, https://github.com/ghga-de/metldata
+Classifier: Development Status :: 1 - Planning
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: hexkit[akafka,mongodb]<4,>=3
+Requires-Dist: ghga-service-commons[api,auth]<4,>=3.1.1
+Requires-Dist: ghga-event-schemas<4,>=3.0.0
+Requires-Dist: typer>=0.12
+Requires-Dist: linkml==1.6.1
+Requires-Dist: linkml-runtime==1.6.0
+Requires-Dist: linkml-validator==0.4.5
+Requires-Dist: cryptography>=42.0.0
+
 [![tests](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/metldata/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/metldata?branch=main)
 
 # Metldata
 
 metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 
@@ -54,29 +81,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:1.2.1
+docker pull ghga/metldata:1.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:1.2.1 .
+docker build -t ghga/metldata:1.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:1.2.1 --help
+docker run -p 8080:8080 ghga/metldata:1.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -139,15 +166,15 @@
 
 - **`kafka_ssl_cafile`** *(string)*: Certificate Authority file path containing certificates used to sign broker certificates. If a CA is not specified, the default system CA will be used if found by OpenSSL. Default: `""`.
 
 - **`kafka_ssl_certfile`** *(string)*: Optional filename of client certificate, as well as any CA certificates needed to establish the certificate's authenticity. Default: `""`.
 
 - **`kafka_ssl_keyfile`** *(string)*: Optional filename containing the client private key. Default: `""`.
 
-- **`kafka_ssl_password`** *(string)*: Optional password to be used for the client private key. Default: `""`.
+- **`kafka_ssl_password`** *(string, format: password)*: Optional password to be used for the client private key. Default: `""`.
 
 - **`generate_correlation_id`** *(boolean)*: A flag, which, if False, will result in an error when inbound requests don't possess a correlation ID. If True, requests without a correlation ID will be assigned a newly generated ID in the correlation ID middleware function. Default: `true`.
 
 
   Examples:
 
   ```json
@@ -330,20 +357,63 @@
   ```json
   []
   ```
 
 
 - **`artifact_infos`** *(array)*: Information for artifacts to be queryable via the Artifacts REST API.
 
-  - **Items**: Refer to *[#/$defs/ArtifactInfo](#$defs/ArtifactInfo)*.
+  - **Items**: Refer to *[#/$defs/ArtifactInfo](#%24defs/ArtifactInfo)*.
 
 - **`loader_token_hashes`** *(array)*: Hashes of tokens used to authenticate for loading artifact.
 
   - **Items** *(string)*
 
+## Definitions
+
+
+- <a id="%24defs/AnchorPoint"></a>**`AnchorPoint`** *(object)*: A model for describing an anchor point for the specified target class.
+
+  - **`target_class`** *(string, required)*: The name of the class to be targeted.
+
+  - **`identifier_slot`** *(string, required)*: The name of the slot in the target class that is used as identifier.
+
+  - **`root_slot`** *(string, required)*: The name of the slot in the root class used to link to the target class.
+
+- <a id="%24defs/ArtifactInfo"></a>**`ArtifactInfo`** *(object)*: Model to describe general information on an artifact.
+Please note, it does not contain actual artifact instances derived from specific
+metadata.
+
+  - **`name`** *(string, required)*: The name of the artifact.
+
+  - **`description`** *(string, required)*: A description of the artifact.
+
+  - **`resource_classes`** *(object, required)*: A dictionary of resource classes for this artifact. The keys are the names of the classes. The values are the corresponding class models. Can contain additional properties.
+
+    - **Additional properties**: Refer to *[#/$defs/ArtifactResourceClass](#%24defs/ArtifactResourceClass)*.
+
+- <a id="%24defs/ArtifactResourceClass"></a>**`ArtifactResourceClass`** *(object)*: Model to describe a resource class of an artifact.
+
+  - **`name`** *(string, required)*: The name of the metadata class.
+
+  - **`description`**: A description of the metadata class. Default: `null`.
+
+    - **Any of**
+
+      - *string*
+
+      - *null*
+
+  - **`anchor_point`**: The anchor point for this metadata class.
+
+    - **All of**
+
+      - : Refer to *[#/$defs/AnchorPoint](#%24defs/AnchorPoint)*.
+
+  - **`json_schema`** *(object, required)*: The JSON schema for this metadata class.
+
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.metldata.yaml`, and place it into one of the following locations:
 - in the current working directory were you are execute the service (on unix: `./.metldata.yaml`)
```

### Comparing `metldata-1.2.1/pyproject.toml` & `metldata-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = [
-    "setuptools>=67.7.2",
+    "setuptools>=69",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 readme = "README.md"
 authors = [
     { name = "German Human Genome Phenome Archive (GHGA)", email = "contact@ghga.de" },
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.12"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "metldata"
-version = "1.2.1"
+version = "1.3.0"
 description = "metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing."
 dependencies = [
-    "hexkit[akafka,mongodb] >=2.1.1, <3",
+    "hexkit[akafka,mongodb] >=3, <4",
     "ghga-service-commons[api,auth] >=3.1.1, <4",
     "ghga-event-schemas >=3.0.0, <4",
-    "typer~=0.9.0",
+    "typer>=0.12",
     "linkml==1.6.1",
     "linkml-runtime==1.6.0",
     "linkml-validator==0.4.5",
+    "cryptography>=42.0.0",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.urls]
 Repository = "https://github.com/ghga-de/metldata"
@@ -59,38 +59,40 @@
 line-length = 88
 src = [
     "src",
     "tests",
     "examples",
     "scripts",
 ]
-target-version = "py39"
+target-version = "py312"
 
 [tool.ruff.lint]
 fixable = [
     "UP",
     "I",
     "D",
 ]
 ignore = [
-    "E",
-    "W",
+    "E111",
+    "E114",
+    "E116",
     "PLW",
     "RUF001",
     "RUF010",
     "RUF012",
     "N818",
     "B008",
     "PLR2004",
     "D205",
     "D400",
     "D401",
     "D107",
     "D206",
     "D300",
+    "UP040",
 ]
 select = [
     "C90",
     "F",
     "I",
     "S",
     "B",
@@ -142,15 +144,15 @@
 ]
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
-minversion = "7.1"
+minversion = "8.0"
 asyncio_mode = "strict"
 
 [tool.coverage.paths]
 source = [
     "src",
     "/workspace/src",
     "**/lib/python*/site-packages",
```

### Comparing `metldata-1.2.1/src/metldata/__init__.py` & `metldata-1.3.0/src/metldata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/__main__.py` & `metldata-1.3.0/src/metldata/event_handling/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
 
-"""Entrypoint of the package"""
-
-from metldata.cli import cli
-
-
-def run():
-    """Run the service"""
-    cli()
-
-
-if __name__ == "__main__":
-    run()
+"""Event handling logic."""
```

### Comparing `metldata-1.2.1/src/metldata/accession_registry/__init__.py` & `metldata-1.3.0/src/metldata/accession_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/accession_registry/accession_registry.py` & `metldata-1.3.0/src/metldata/accession_registry/accession_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/accession_registry/accession_store.py` & `metldata-1.3.0/src/metldata/accession_registry/accession_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/accession_registry/config.py` & `metldata-1.3.0/src/metldata/accession_registry/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/__init__.py` & `metldata-1.3.0/src/metldata/artifacts_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/api_factory.py` & `metldata-1.3.0/src/metldata/artifacts_rest/api_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/artifact_dao.py` & `metldata-1.3.0/src/metldata/artifacts_rest/artifact_dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """DAO for managing artifacts."""
 
+from typing import TypeAlias
+
 from hexkit.protocols.dao import DaoFactoryProtocol, DaoNaturalId
-from typing_extensions import TypeAlias
 
 from metldata.artifacts_rest.artifact_info import get_artifact_info_dict
 from metldata.artifacts_rest.models import ArtifactInfo, ArtifactResource
 
 ArtifactResourceDao: TypeAlias = DaoNaturalId[ArtifactResource]
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/artifact_info.py` & `metldata-1.3.0/src/metldata/artifacts_rest/artifact_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for handling information on artifacts."""
 
 import json
-from typing import Optional
 
 from linkml.generators.jsonschemagen import JsonSchemaGenerator
 from linkml_runtime.linkml_model.annotations import Annotation
 from linkml_runtime.linkml_model.meta import ClassDefinition
 
 from metldata.artifacts_rest.models import ArtifactInfo, ArtifactResourceClass
 from metldata.custom_types import Json
@@ -110,17 +109,15 @@
     return {
         "$schema": global_json_schema["$schema"],
         **target_definition,
         "$defs": filtered_definitions,
     }
 
 
-def load_description_for_class(
-    *, model: MetadataModel, class_name: str
-) -> Optional[str]:
+def load_description_for_class(*, model: MetadataModel, class_name: str) -> str | None:
     """Load the description for the specified class of the metadata model."""
     return model.schema_view.get_class(class_name, strict=True).description
 
 
 def load_resource_classes(*, model: MetadataModel) -> dict[str, ArtifactResourceClass]:
     """Load all classes from a metadata model.
     Only anchored classes are considered. Classes that are annotated as `hidden`
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/config.py` & `metldata-1.3.0/src/metldata/artifacts_rest/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/load_resources.py` & `metldata-1.3.0/src/metldata/artifacts_rest/load_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -181,15 +181,15 @@
                 artifact_info_dict=artifact_info_dict,
                 artifact_name=artifact_name,
                 event_publisher=event_publisher,
                 resource=resource,
             )
 
 
-async def process_resource_upsert(  # pylint: disable=too-many-locals
+async def process_resource_upsert(
     *,
     artifact_info_dict: dict[str, ArtifactInfo],
     artifact_name: str,
     event_publisher: EventPublisherPort,
     resource: ArtifactResource,
 ):
     """Convert available data to correct event model and delegate firing appropriate events"""
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/models.py` & `metldata-1.3.0/src/metldata/artifacts_rest/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,27 +12,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Data models."""
 
-from typing import Optional
-
 from ghga_service_commons.utils.utc_dates import UTCDatetime
 from pydantic import BaseModel, Field, field_validator
 from typing_extensions import TypedDict
 
 from metldata.custom_types import Json
 from metldata.model_utils.anchors import AnchorPoint
 
 try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
-    from typing_extensions import Literal
+    from typing import Literal
 except ImportError:
-    from typing import Literal  # type: ignore
+    from typing import Literal
 
 
 class ArtifactResource(BaseModel):
     """Information on a resource of an artifact."""
 
     id_: str = Field(..., description="The ID of the resource.")
     class_name: str = Field(
@@ -41,15 +39,15 @@
     content: Json = Field(..., description="The metadata content of that resource.")
 
 
 class ArtifactResourceClass(BaseModel):
     """Model to describe a resource class of an artifact."""
 
     name: str = Field(..., description="The name of the metadata class.")
-    description: Optional[str] = Field(
+    description: str | None = Field(
         None, description="A description of the metadata class."
     )
     anchor_point: AnchorPoint = Field(
         ..., description="The anchor point for this metadata class."
     )
     json_schema: Json = Field(
         ..., description="The JSON schema for this metadata class."
```

### Comparing `metldata-1.2.1/src/metldata/artifacts_rest/query_resources.py` & `metldata-1.3.0/src/metldata/artifacts_rest/query_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,12 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A transformation to add accessions to metadata."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.add_accessions.main import (  # noqa: F401
     ACCESSION_ADDITION_TRANSFORMATION,
     AccessionAdditionConfig,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -77,15 +77,15 @@
             references=self._references,
             anchor_points_by_target=self._anchor_points_by_target,
         )
 
 
 def check_model_assumptions(
     model: MetadataModel,
-    config: AccessionAdditionConfig,  # pylint: disable=unused-argument
+    config: AccessionAdditionConfig,
 ) -> None:
     """Check the assumptions of the model.
 
     Raises:
         MetadataModelAssumptionError:
             if the model does not fulfill the assumptions.
     """
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/metadata_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,17 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for transforming metadata."""
 
 from collections import defaultdict
+from typing import TypeAlias
 
 from pydantic import Json
-from typing_extensions import TypeAlias
 
 from metldata.metadata_utils import lookup_self_id
 from metldata.model_utils.anchors import AnchorPoint, lookup_anchor_point
 from metldata.model_utils.essentials import MetadataModel
 from metldata.submission_registry.models import AccessionMap
 from metldata.transform.base import MetadataTransformationError
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/add_accessions/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/add_accessions/model_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,27 +13,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for transforming metadata models."""
 
 from copy import deepcopy
-from typing import Optional, cast
+from typing import cast
 
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
 
 from metldata.model_utils.anchors import get_anchors_points_by_target
 from metldata.model_utils.essentials import ExportableSchemaView, MetadataModel
 from metldata.model_utils.identifiers import get_class_identifiers
 from metldata.model_utils.manipulate import upsert_class
 from metldata.transform.base import MetadataModelTransformationError
 
 
 def unset_identifier(
-    *, class_definition: ClassDefinition, class_identifiers: dict[str, Optional[str]]
+    *, class_definition: ClassDefinition, class_identifiers: dict[str, str | None]
 ) -> ClassDefinition:
     """Get a modified copy of the provided class definition with the identifier being
     unset.
     """
     identifier_slot_name = class_identifiers[class_definition.name]
     if identifier_slot_name is None:
         raise RuntimeError(  # This should never happen
@@ -70,15 +70,15 @@
     )
 
 
 def add_accessions_to_class(
     *,
     class_definition: ClassDefinition,
     accession_slot_name: str,
-    class_identifiers: dict[str, Optional[str]],
+    class_identifiers: dict[str, str | None],
 ) -> ClassDefinition:
     """Get a modified copy of the provided class definition with the accession slot
     being added as identifier.
     """
     modified_class = unset_identifier(
         class_definition=class_definition, class_identifiers=class_identifiers
     )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,14 +13,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Aggregate transformation for metadata."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.aggregate.config import (  # noqa: F401
     AggregateConfig,
 )
 from metldata.builtin_transformations.aggregate.main import (  # noqa: F401
     AGGREGATE_TRANSFORMATION,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/cached_model.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/cached_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Config for aggregate transformations"""
 
-from typing import Optional
-
 from pydantic import BaseModel, model_validator
 from pydantic_settings import BaseSettings
 
 from metldata.builtin_transformations.aggregate.func import (
     AggregationFunction,
     transformation_by_name,
 )
@@ -30,15 +28,15 @@
 class AggregationOperation(BaseModel):
     """A model for a single aggregation operation executed on one or multiple
     branches in the data described by a path in the model.
     """
 
     input_paths: list[str]
     output_path: str
-    visit_only_once: Optional[list[str]] = None
+    visit_only_once: list[str] | None = None
     function: type[AggregationFunction]
 
     @model_validator(mode="before")
     def lookup_operation(cls, values: dict) -> dict:  # noqa: N805
         """Replaces operation strings with operation types."""
         if "function" in values:
             values["function"] = transformation_by_name(values["function"])
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/data_subgraph.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/data_subgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +16,15 @@
 
 """This module provides the DataSubgraph class to traverse a subgraph of a
 LinkML-based JSON data graph.
 """
 
 from collections import defaultdict
 from collections.abc import Iterator
-from typing import Any, Optional
+from typing import Any
 
 from linkml_runtime.linkml_model import SlotDefinition
 
 from metldata.builtin_transformations.aggregate.cached_model import CachedMetadataModel
 from metldata.custom_types import Json
 from metldata.metadata_utils import get_resource_dict_of_class
 from metldata.model_utils.anchors import AnchorPoint
@@ -68,15 +68,15 @@
     can have various cardinalities (i.e. LinkML slots may be multivalued).
 
     The DataSubgraph enables to iterate through the nodes of the subgraph.
     """
 
     _model: MetadataModel
     _paths: list[list[SlotDefinition]]
-    _class_identifiers: dict[str, Optional[str]]
+    _class_identifiers: dict[str, str | None]
     _all_classes: list[str]
     _anchor_points: dict[str, AnchorPoint]
 
     def _get_class_identifier(self, class_name: str) -> str:
         """Returns the identifier slot name for the given class name.
 
         Args:
@@ -218,15 +218,15 @@
     def __init__(  # noqa: PLR0913
         self,
         *,
         model: CachedMetadataModel,
         submission_data: Json,
         origin: str,
         path_strings: list[str],
-        visit_once_classes: Optional[list[str]] = None,
+        visit_once_classes: list[str] | None = None,
     ):
         """Creates a new DataSubgraph object.
 
         Args:
             model (MetadataModel): The LinkML metadata model
             submission_data (Json): The full submission data, a representation
             of the LinkML tree root class
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/expanding_dict.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/expanding_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/func.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/func.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +16,15 @@
 
 """Transformation and aggregation functions for the aggregate module."""
 
 from abc import ABC, abstractmethod
 from collections import Counter
 from collections.abc import Iterable
 from operator import itemgetter
-from typing import Any, Optional
+from typing import Any
 
 from metldata.builtin_transformations.aggregate.models import (
     MinimalClass,
     MinimalNamedSlot,
 )
 from metldata.transform.base import MetadataTransformationError
 
@@ -33,15 +33,15 @@
 
 class AggregationFunction(ABC):
     """An abstract class for aggregation transformation functions"""
 
     result_range_name: str
     """The name of the range of the data produced by func."""
 
-    result_range_cls_def: Optional[MinimalClass]
+    result_range_cls_def: MinimalClass | None
     """The class definition of the data produced by func. None if the function
     result range is a type rather than a class."""
 
     result_multivalued: bool
     """Whether or not the transformation function produces a single value or a
     list."""
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -69,15 +69,15 @@
             metadata=metadata,
             aggregations=self._config.aggregations,
         )
 
 
 def check_model_assumptions(
     model: MetadataModel,
-    config: AggregateConfig,  # pylint: disable=unused-argument
+    config: AggregateConfig,
 ) -> None:
     """Check the assumptions of the model.
 
     Raises:
         MetadataModelAssumptionError:
             if the model does not fulfill the assumptions.
     """
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/metadata_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -21,15 +21,14 @@
 from metldata.builtin_transformations.aggregate.data_subgraph import DataSubgraph
 from metldata.builtin_transformations.aggregate.expanding_dict import ExpandingDict
 from metldata.builtin_transformations.aggregate.func import MetadataTransformationError
 from metldata.custom_types import Json
 from metldata.model_utils.anchors import AnchorPoint
 
 
-# pylint: disable=unused-argument
 def execute_aggregation(
     *,
     original_model: CachedMetadataModel,
     original_data: Json,
     aggregation: Aggregation,
 ) -> list[Json]:
     """Transforms the metadata according to the specified aggregation operation."""
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/model_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +16,14 @@
 
 """Model transformation for aggregate transformations."""
 
 import itertools
 from collections import defaultdict
 from collections.abc import Iterable
 from dataclasses import asdict
-from typing import Optional
 
 from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
 from stringcase import snakecase
 
 from metldata.builtin_transformations.aggregate.config import (
     AggregateConfig,
     Aggregation,
@@ -37,15 +36,15 @@
 )
 from metldata.model_utils.anchors import AnchorPoint
 from metldata.model_utils.essentials import ROOT_CLASS, MetadataModel
 from metldata.model_utils.identifiers import get_class_identifier
 from metldata.model_utils.manipulate import add_anchor_point, upsert_class_slot
 from metldata.transform.base import MetadataModelTransformationError
 
-Path = tuple[Optional[str], ...]
+Path = tuple[str | None, ...]
 
 
 class PathMatrix:
     """Represents a matrix of data paths."""
 
     __paths: list[Path]
     leaf_slots: list[MinimalNamedSlot]
@@ -77,15 +76,15 @@
 
     def load_leaf_slots(self, leaf_slots: list[MinimalSlot]) -> None:
         """Combines the paths and the specified leaf slots to NamedSlots and
         stores them.
         """
         self.leaf_slots = [
             MinimalNamedSlot(slot_name=slot_name, **asdict(slot))
-            for slot_name, slot in zip(self.path_leaves(), leaf_slots)
+            for slot_name, slot in zip(self.path_leaves(), leaf_slots, strict=False)
         ]
 
     @property
     def paths(self):
         """Returns a copy of the paths."""
         return self.__paths[:]
 
@@ -199,15 +198,15 @@
     leaf_ranges = [op.function.result_range_name for op in aggregation.operations]
     leaf_multivalued = [op.function.result_multivalued for op in aggregation.operations]
 
     path_matrix = PathMatrix(
         path_strings=path_strings,
         leaf_slots=[
             MinimalSlot(range=slot_range, multivalued=mv)
-            for slot_range, mv in zip(leaf_ranges, leaf_multivalued)
+            for slot_range, mv in zip(leaf_ranges, leaf_multivalued, strict=False)
         ],
     )
 
     for _ in range(path_matrix.max_depth):
         classes: dict[Path, set[MinimalNamedSlot]] = defaultdict(set[MinimalNamedSlot])
         for idx, path_prefix in enumerate(path_matrix.paths):
             if path_prefix[-1]:
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/aggregate/models.py` & `metldata-1.3.0/src/metldata/builtin_transformations/aggregate/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,12 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A transformation to generate custom embeddings for classes of a metadata model."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.custom_embeddings.main import (  # noqa: F401
     CUSTOM_EMBEDDING_TRANSFORMATION,
     CustomEmbeddingConfig,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -48,15 +48,14 @@
     embedding_profiles: list[EmbeddingProfile] = Field(
         ...,
         description=(
             "A list of custom embedding profiles for classes from a metadata model."
         ),
     )
 
-    # pylint: disable=no-self-argument
     @field_validator("embedding_profiles")
     def check_embedding_profiles_unique(
         cls,  # noqa: N805
         value: list[EmbeddingProfile],
     ) -> list[EmbeddingProfile]:
         """Check that names for embedded classes are unique among the embedding_profiles."""
         embedded_classes = [
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/embedding_profile.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/embedding_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -69,15 +69,15 @@
             model=self._original_model,
             anchor_points_by_target=self._anchor_points_by_target,
         )
 
 
 def check_model_assumptions(
     model: MetadataModel,
-    config: CustomEmbeddingConfig,  # pylint: disable=unused-argument
+    config: CustomEmbeddingConfig,
 ) -> None:
     """Check the assumptions of the model.
 
     Raises:
         MetadataModelAssumptionError:
             if the model does not fulfill the assumptions.
     """
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/metadata_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for transforming metadata."""
 
-from typing import Union, cast
+from typing import cast
 
 from metldata.builtin_transformations.custom_embeddings.embedding_profile import (
     EmbeddingProfile,
 )
 from metldata.builtin_transformations.custom_embeddings.model_transform import (
     get_embedding_profile_root_slot,
 )
@@ -49,15 +49,15 @@
         )
 
     return bool(slot_definition.multivalued)
 
 
 def resolve_target_resource(
     target_resource_id: str,
-    target: Union[str, EmbeddingProfile],
+    target: str | EmbeddingProfile,
     global_metadata: Json,
     model: MetadataModel,
     anchor_points_by_target: dict,
 ) -> Json:
     """Resolves a target resource.
 
     Raises:
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/custom_embeddings/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/custom_embeddings/model_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for transforming metadata models."""
 
 from copy import deepcopy
-from typing import Union
 
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
 from stringcase import snakecase
 
 from metldata.builtin_transformations.custom_embeddings.embedding_profile import (
     EmbeddingProfile,
 )
@@ -47,15 +46,15 @@
 
 
 def get_embedded_reference_slot(
     *,
     class_: ClassDefinition,
     schema_view: ExportableSchemaView,
     reference_slot_name: str,
-    target: Union[str, EmbeddingProfile],
+    target: str | EmbeddingProfile,
 ) -> SlotDefinition:
     """Update the slot definition of an embedded reference."""
     if not class_.slots or reference_slot_name not in class_.slots:
         raise MetadataModelTransformationError(
             f"Class '{class_.name}' does not have the slot '{reference_slot_name}'"
         )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,12 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A transformation that deletes slots from models and associated metadata."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.delete_slots.main import (  # noqa: F401
     SLOT_DELETION_TRANSFORMATION,
     SlotDeletionConfig,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/assumptions.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/assumptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/metadata_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/delete_slots/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/delete_slots/model_transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,12 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A transformation to infer references based on existing ones in the metadata model."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.infer_references.main import (  # noqa: F401
     REFERENCE_INFERENCE_TRANSFORMATION,
     ReferenceInferenceConfig,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -70,15 +70,15 @@
             references=self._config.inferred_references,
             anchor_points_by_target=self._anchor_points_by_target,
         )
 
 
 def check_model_assumptions(
     model: MetadataModel,
-    config: ReferenceInferenceConfig,  # pylint: disable=unused-argument
+    config: ReferenceInferenceConfig,
 ) -> None:
     """Check the assumptions of the model.
 
     Raises:
         MetadataModelAssumptionError:
             if the model does not fulfill the assumptions.
     """
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/metadata_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/model_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path_elements.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/path_str.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/path_str.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Data models"""
 
 import re
-from typing import Optional
 
 from metldata.builtin_transformations.infer_references.path.path_elements import (
     ReferencePathElement,
     ReferencePathElementType,
 )
 
 NAME_PATTERN = r"(?!\d)\w+"
@@ -103,15 +102,15 @@
 
     if not match:
         raise ValidationError(f"Cannot find target class of path string: {path_str}")
 
     return match.group(1)
 
 
-def split_first_element(*, path_str: str) -> tuple[str, Optional[str]]:
+def split_first_element(*, path_str: str) -> tuple[str, str | None]:
     """Return a tuple of the first element and the remaining path string.
     Thereby, the target class of the first element is set as the source class of the
     remaining path.
     The second element is None if the provided path only contained one element.
     The path_str is assumed to be cleaned.
     """
     first_element = extract_first_element(path_str=path_str)
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/path/resolve.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/path/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/infer_references/reference.py` & `metldata-1.3.0/src/metldata/builtin_transformations/infer_references/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,12 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A transformation that merges multiple slots of a class into a single one."""
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.builtin_transformations.merge_slots.main import (  # noqa: F401
     SLOT_MERGING_TRANSFORMATION,
     SlotMergingConfig,
 )
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/assumptions.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/assumptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/metadata_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/metadata_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/model_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/merge_slots/models.py` & `metldata-1.3.0/src/metldata/builtin_transformations/merge_slots/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Models to describe slot merging instructions."""
 
-from typing import Optional
-
 from pydantic import BaseModel, Field, model_validator
 
 
 class SlotMergeInstruction(BaseModel):
     """A model to describe slot merging instructions."""
 
     class_name: str = Field(..., description="The class to which the slots belong.")
@@ -29,15 +27,15 @@
         ...,
         description="The slots that should be merged into the target slot.",
         min_length=2,
     )
     target_slot: str = Field(
         ..., description="The slot into which the source slots should be merged."
     )
-    target_description: Optional[str] = Field(
+    target_description: str | None = Field(
         None,
         description="A description of the target slot.",
     )
 
     @model_validator(mode="before")
     def validate_overlapping_slots(cls, values) -> dict:  # noqa: N805
         """Validate that source and target slots do not overlap."""
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/__init__.py` & `metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/config.py` & `metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/main.py` & `metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -22,20 +22,18 @@
 )
 from metldata.custom_types import Json
 from metldata.event_handling.models import SubmissionAnnotation
 from metldata.model_utils.essentials import MetadataModel
 from metldata.transform.base import MetadataTransformer, TransformationDefinition
 
 
-# pylint: disable=unused-argument
 def check_model_assumptions(model: MetadataModel, config: NormalizationConfig):
     """Check that the classes and slots specified in the config exist in the model."""
 
 
-# pylint: disable=unused-argument
 def transform_model(model: MetadataModel, config: NormalizationConfig) -> MetadataModel:
     """Normalize the model."""
     return normalize_model(model)
 
 
 class NormalizationTransformer(MetadataTransformer[NormalizationConfig]):
     """Transformer for normalizing the metadata model."""
```

### Comparing `metldata-1.2.1/src/metldata/builtin_transformations/normalize_model/model_transform.py` & `metldata-1.3.0/src/metldata/builtin_transformations/normalize_model/model_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_workflows/__init__.py` & `metldata-1.3.0/src/metldata/builtin_workflows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/builtin_workflows/ghga_archive.py` & `metldata-1.3.0/src/metldata/builtin_workflows/ghga_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/cli.py` & `metldata-1.3.0/src/metldata/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/combined.py` & `metldata-1.3.0/src/metldata/combined.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/config.py` & `metldata-1.3.0/src/metldata/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,24 +13,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Config Parameter Modeling and Parsing"""
 
 from hexkit.config import config_from_yaml
 
-# pylint: disable=unused-import
 from metldata.accession_registry.config import Config as AccessionRegistryConfig
 from metldata.artifacts_rest.config import ArtifactsRestConfig
-
-# pylint: disable=unused-import
 from metldata.load.config import ArtifactLoaderAPIConfig
 from metldata.submission_registry.config import Config as SubmissionRegistryConfig
 
 
-# pylint: disable=too-many-ancestors
 @config_from_yaml(prefix="metl_sub")
 class SubmissionConfig(AccessionRegistryConfig, SubmissionRegistryConfig):
     """Config parameters and their defaults."""
 
 
 @config_from_yaml(prefix="metldata")
 class Config(ArtifactLoaderAPIConfig, ArtifactsRestConfig):
```

### Comparing `metldata-1.2.1/src/metldata/custom_types.py` & `metldata-1.3.0/src/metldata/custom_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,14 +12,12 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A collection of custom types."""
 
-from typing import Any
-
-from typing_extensions import TypeAlias
+from typing import Any, TypeAlias
 
 Json: TypeAlias = dict[str, Any]
 
 SubmissionContent = dict[str, list[Json]]
```

### Comparing `metldata-1.2.1/src/metldata/event_handling/__init__.py` & `metldata-1.3.0/src/metldata/model_utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Event handling logic."""
+"""Utilities for handling metadata models."""
```

### Comparing `metldata-1.2.1/src/metldata/event_handling/artifact_events.py` & `metldata-1.3.0/src/metldata/event_handling/artifact_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/event_handling/event_handling.py` & `metldata-1.3.0/src/metldata/event_handling/event_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +15,14 @@
 #
 
 """Functionality to publish and consume events stored on the file system."""
 
 import json
 from collections.abc import Iterator
 from pathlib import Path
-from typing import Optional
 
 from hexkit.base import InboundProviderBase
 from hexkit.custom_types import Ascii, JsonObject
 from hexkit.protocols.eventpub import EventPublisherProtocol
 from hexkit.protocols.eventsub import EventSubscriberProtocol
 from pydantic import BaseModel, Field
 from pydantic_settings import BaseSettings
@@ -161,30 +160,30 @@
             raise NotImplementedError
 
         for event in read_events_from_topic(
             topic=self._topic_of_interest,
             event_store_path=self._config.event_store_path,
         ):
             await self._translator.consume(
-                payload=event.payload, type_=event.type_, topic=event.topic
+                payload=event.payload, type_=event.type_, topic=event.topic, key=""
             )
 
 
 class FileSystemEventCollector:
     """An alternative to the FileSystemEventSubscriber that can be used to obtain a
     collection of events without the need to hand over individual events to a
     translator.
     """
 
     def __init__(self, *, config: FileSystemEventConfig):
         """Initialize with config."""
         self._config = config
 
     def collect_events(
-        self, *, topic: str, types: Optional[list[str]] = None
+        self, *, topic: str, types: list[str] | None = None
     ) -> Iterator[Event]:
         """Collect all events for the given types from the given topic."""
         events = read_events_from_topic(
             topic=topic,
             event_store_path=self._config.event_store_path,
         )
```

### Comparing `metldata-1.2.1/src/metldata/event_handling/models.py` & `metldata-1.3.0/src/metldata/event_handling/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/event_handling/submission_events.py` & `metldata-1.3.0/src/metldata/event_handling/submission_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/__init__.py` & `metldata-1.3.0/src/metldata/load/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/aggregator.py` & `metldata-1.3.0/src/metldata/load/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/api.py` & `metldata-1.3.0/src/metldata/load/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """API for loading artifacts into running services."""
 
-from typing import Optional
-
 from fastapi import Depends, HTTPException, Response, Security
 from fastapi.routing import APIRouter
 from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
 from ghga_service_commons.auth.context import AuthContextProtocol
 from ghga_service_commons.auth.policies import require_auth_context_using_credentials
 from hexkit.protocols.dao import DaoFactoryProtocol
 from hexkit.providers.akafka import KafkaEventPublisher
@@ -55,15 +53,15 @@
 class LoaderTokenAuthProvider(AuthContextProtocol[LoaderTokenAuthContext]):
     """A provider for the loader token auth context."""
 
     def __init__(self, *, token_hashes: list[str]):
         """Initialize the loader token auth provider."""
         self._token_hashes = token_hashes
 
-    async def get_context(self, token: str) -> Optional[LoaderTokenAuthContext]:
+    async def get_context(self, token: str) -> LoaderTokenAuthContext | None:
         """Get a loader token auth context."""
         if not token:
             return None
 
         if not check_token(token=token, token_hashes=self._token_hashes):
             raise self.AuthContextValidationError("Invalid token.")
```

### Comparing `metldata-1.2.1/src/metldata/load/auth.py` & `metldata-1.3.0/src/metldata/load/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/client.py` & `metldata-1.3.0/src/metldata/load/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/collect.py` & `metldata-1.3.0/src/metldata/load/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -62,10 +62,10 @@
             artifact_topic_prefix=config.artifact_topic_prefix,
             artifact_type=artifact_type,
         )
         for event in event_collector.collect_events(topic=topic):
             content = event.payload.get("content")
             if not content:
                 raise RuntimeError("Artifact does not contain 'content' field.")
-            artifact_resources[artifact_type].append(content)
+            artifact_resources[artifact_type].append(content)  # type: ignore
 
     return artifact_resources
```

### Comparing `metldata-1.2.1/src/metldata/load/config.py` & `metldata-1.3.0/src/metldata/load/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -23,15 +23,15 @@
 
 from metldata.artifacts_rest.config import ArtifactsRestConfig
 from metldata.event_handling.event_handling import FileSystemEventConfig
 from metldata.load.collect import ArtifactCollectorConfig
 from metldata.load.event_publisher import EventPubTranslatorConfig
 
 
-class ArtifactLoaderAPIConfig(  # pylint: disable=too-many-ancestors
+class ArtifactLoaderAPIConfig(
     ArtifactsRestConfig,
     ApiConfigBase,
     EventPubTranslatorConfig,
     KafkaConfig,
     MongoDbConfig,
 ):
     """Config settings for the loader API."""
```

### Comparing `metldata-1.2.1/src/metldata/load/event_publisher.py` & `metldata-1.3.0/src/metldata/load/event_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/load.py` & `metldata-1.3.0/src/metldata/load/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -78,15 +78,15 @@
         artifact_info_dict=artifact_info_dict,
         event_publisher=event_publisher,
         resources=changed_resources,
         dao_collection=dao_collection,
     )
 
 
-async def _get_changed_resources(  # pylint: disable=too-many-locals
+async def _get_changed_resources(
     artifact_resources: ArtifactResourceDict,
     artifact_info_dict: dict[str, ArtifactInfo],
     dao_collection: ArtifactDaoCollection,
 ) -> tuple[
     set[tuple[str, str, str]],
     dict[tuple[str, str, str], ArtifactResource],
     dict[tuple[str, str, str], ArtifactResource],
```

### Comparing `metldata-1.2.1/src/metldata/load/main.py` & `metldata-1.3.0/src/metldata/load/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/load/models.py` & `metldata-1.3.0/src/metldata/load/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,14 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Data models."""
 
-from typing_extensions import TypeAlias
+from typing import TypeAlias
 
 from metldata.custom_types import Json
 
 # A dictionary of an artifact. The keys on the first correspond to artifact names.
 # The values are lists of resources for different submissions.
 ArtifactResourceDict: TypeAlias = dict[str, list[Json]]
```

### Comparing `metldata-1.2.1/src/metldata/load/stats.py` & `metldata-1.3.0/src/metldata/load/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,30 +13,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Generate global summary statistics."""
 
 from operator import itemgetter
-from typing import Any, Optional, cast
+from typing import Any, cast
 
 from ghga_service_commons.utils.utc_dates import now_as_utc
 
 from metldata.artifacts_rest.models import (
     ArtifactInfo,
     GlobalStats,
     ResourceStats,
     ValueCount,
 )
 from metldata.load.aggregator import DbAggregator
 
 STATS_COLLECTION_NAME = "stats"
 
 
-def get_stat_slot(resource_class: str) -> Optional[str]:
+def get_stat_slot(resource_class: str) -> str | None:
     """Get the name of the slot that shall be used as grouping key."""
     if resource_class.endswith("File"):
         return "format"
     if resource_class.endswith("Protocol"):
         return "type"
     if resource_class.endswith("Individual"):
         return "sex"
```

### Comparing `metldata-1.2.1/src/metldata/metadata_utils.py` & `metldata-1.3.0/src/metldata/metadata_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Utilities for handling metadata."""
 
 from copy import deepcopy
-from typing import Union, cast
+from typing import cast
 
 from metldata.custom_types import Json
 from metldata.model_utils.anchors import AnchorPoint, lookup_anchor_point
 
 
 class SelfIdLookUpError(RuntimeError):
     """Raised when the self id cannot be looked up."""
@@ -274,17 +274,15 @@
     )
 
     global_metadata_copy = deepcopy(global_metadata)
 
     return {**global_metadata_copy, anchor_point.root_slot: resources}
 
 
-def lookup_slot_in_resource(
-    *, resource: Json, slot_name: str
-) -> Union[Json, list[Json]]:
+def lookup_slot_in_resource(*, resource: Json, slot_name: str) -> Json | list[Json]:
     """Lookup a slot in a resource. Raises an error if the slot does not exist."""
     content = resource.get(slot_name)
 
     if content is None:
         raise SlotNotFoundError(
             f"Could not find slot '{slot_name}' in resource: {resource}"
         )
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/__init__.py` & `metldata-1.3.0/src/metldata/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,27 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
 
-"""Utilities for handling metadata models."""
+"""Entrypoint of the package"""
+
+from metldata.cli import cli
+
+
+def run():
+    """Run the service"""
+    cli()
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/anchors.py` & `metldata-1.3.0/src/metldata/model_utils/anchors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/assumptions.py` & `metldata-1.3.0/src/metldata/model_utils/assumptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic to check basic assumptions about the metadata model."""
 
-from typing import Optional
-
 from metldata.model_utils.anchors import (
     AnchorPointNotFoundError,
     InvalidAnchorPointError,
     filter_anchor_points,
     get_anchors_points_by_target,
 )
 from metldata.model_utils.essentials import ROOT_CLASS, MetadataModel
@@ -88,17 +86,15 @@
         )
     if not root_class.tree_root:
         raise MetadataModelAssumptionError(
             f"The {ROOT_CLASS} class must have the tree_root property set to true."
         )
 
 
-def check_anchor_points(
-    model: MetadataModel, classes: Optional[list[str]] = None
-) -> None:
+def check_anchor_points(model: MetadataModel, classes: list[str] | None = None) -> None:
     """Checks the anchor points of the root class. If classes is specified, also checks
     that anchor points for the classes exist.
 
     Raises:
         MetadataModelAssumptionError: if validation fails.
     """
     try:
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/config.py` & `metldata-1.3.0/src/metldata/model_utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/essentials.py` & `metldata-1.3.0/src/metldata/model_utils/essentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -69,15 +69,14 @@
     def __eq__(self, other: object):
         """For comparisons."""
         if not isinstance(other, MetadataModel):
             return NotImplemented
 
         return self.as_dict() == other.as_dict()
 
-    # pylint: disable=too-many-nested-blocks,too-many-branches
     def as_dict(self, essential: bool = True):  # noqa: PLR0912, C901
         """Get a dictionary representation of the model. If essential set to True, the
         dictionary will be cleaned of all fields that are not essential.
         """
         model_dict = dataclasses.asdict(self)
 
         if essential:
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/identifiers.py` & `metldata-1.3.0/src/metldata/model_utils/identifiers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,20 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Handling identifiers of classes in a metadata model."""
 
-from typing import Optional
-
 from metldata.model_utils.essentials import ROOT_CLASS, MetadataModel
 
 
-def get_class_identifier(model: MetadataModel, class_name: str) -> Optional[str]:
+def get_class_identifier(model: MetadataModel, class_name: str) -> str | None:
     """Get the identifier of a class in a metadata model.
 
     Returns:
         The identifier of the class, or None if the class does not have an identifier.
     """
     schema_view = model.schema_view
 
@@ -33,24 +31,24 @@
         slot_def = schema_view.induced_slot(slot_name=slot_name, class_name=class_name)
         if slot_def.identifier:
             return str(slot_def.name)
 
     return None
 
 
-def get_class_identifiers(model: MetadataModel) -> dict[str, Optional[str]]:
+def get_class_identifiers(model: MetadataModel) -> dict[str, str | None]:
     """Get the identifiers of all classes in a metadata model.
 
     Returns:
         A dictionary with the class names as keys and the identifiers as values. If a
         class does not have an identifier, the value is None.
     """
     schema_view = model.schema_view
 
-    identifiers_by_class: dict[str, Optional[str]] = {}
+    identifiers_by_class: dict[str, str | None] = {}
     for class_name in schema_view.all_classes():
         if class_name == ROOT_CLASS:
             continue  # Root class does not have an identifier
         class_def = schema_view.get_class(class_name=class_name)
         if class_def.mixin or class_def.abstract:
             continue  # Mixins and abstract classes do not have an identifier
         identifier = get_class_identifier(model=model, class_name=class_name)
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/manipulate.py` & `metldata-1.3.0/src/metldata/model_utils/manipulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +15,14 @@
 #
 
 """Utilities for manipulating the schemas. This extends the functionality provided by
 the standard linkml SchemaView class.
 """
 
 from copy import deepcopy
-from typing import Optional, Union
 
 import jsonasobj2
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
 
 from metldata.model_utils.anchors import AnchorPoint
 from metldata.model_utils.assumptions import ROOT_CLASS
 from metldata.model_utils.essentials import ExportableSchemaView
@@ -46,15 +45,15 @@
     """Raised when a slot of a class was not found."""
 
     def __init__(
         self,
         class_name: str,
         slot_name: str,
         direct: bool = False,
-        context: Optional[str] = None,
+        context: str | None = None,
     ):
         message = (
             f"The slot '{slot_name}' does not exist"
             + (" as direct slot" if direct else "")
             + f" in the class '{class_name}' of the metadata model."
             + (f" {context}" if context else "")
         )
@@ -177,15 +176,15 @@
 
 def add_slot_usage_annotation(
     *,
     schema_view: ExportableSchemaView,
     slot_name: str,
     class_name: str,
     annotation_key: str,
-    annotation_value: Union[str, bool, int, float],
+    annotation_value: str | bool | int | float,
 ) -> ExportableSchemaView:
     """Add annotations to a slot in the context of a class.
     For more details see:
     https://linkml.io/linkml/schemas/metadata.html#arbitrary-annotations
     """
     class_ = schema_view.get_class(class_name=class_name)
 
@@ -246,15 +245,15 @@
     return modified_schema_view
 
 
 def add_anchor_point(
     *,
     schema_view: ExportableSchemaView,
     anchor_point: AnchorPoint,
-    description: Optional[str] = None,
+    description: str | None = None,
 ) -> ExportableSchemaView:
     """Add an anchor point for a class to the tree root of the model."""
     class_ = schema_view.get_class(class_name=anchor_point.target_class)
 
     if not class_:
         raise ClassNotFoundError(class_name=anchor_point.target_class)
```

### Comparing `metldata-1.2.1/src/metldata/model_utils/metadata_validator.py` & `metldata-1.3.0/src/metldata/model_utils/metadata_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/__init__.py` & `metldata-1.3.0/src/metldata/submission_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/config.py` & `metldata-1.3.0/src/metldata/submission_registry/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,14 +16,13 @@
 """Config Parameter Modeling and Parsing"""
 
 from metldata.submission_registry.event_publisher import SourceEventPublisherConfig
 from metldata.submission_registry.submission_registry import SubmissionRegistryConfig
 from metldata.submission_registry.submission_store import SubmissionStoreConfig
 
 
-# pylint: disable=too-many-ancestors
 class Config(
     SubmissionStoreConfig,
     SubmissionRegistryConfig,
     SourceEventPublisherConfig,
 ):
     """Config parameters and their defaults."""
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/event_publisher.py` & `metldata-1.3.0/src/metldata/submission_registry/event_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/identifiers.py` & `metldata-1.3.0/src/metldata/submission_registry/identifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,15 +14,14 @@
 # limitations under the License.
 #
 
 """Logic for handling identifiers and accessions."""
 
 from collections.abc import Iterable
 from functools import partial
-from typing import Optional
 from uuid import uuid4
 
 from pydantic import Json
 
 from metldata.accession_registry import AccessionRegistry
 from metldata.custom_types import SubmissionContent
 from metldata.metadata_utils import lookup_self_id
@@ -41,15 +40,15 @@
 
 
 def lookup_accession(
     *,
     anchor: str,
     alias: str,
     accession_map: AccessionMap,
-) -> Optional[str]:
+) -> str | None:
     """Lookup the accession for a resource with the provided user-defined alias of
     the class with the provided anchor. If no accession exists, None is returned.
     """
     return accession_map.get(anchor, {}).get(alias, None)
 
 
 def get_accession(
@@ -99,15 +98,15 @@
             resource=resource, identifier_slot=anchor_point.identifier_slot
         )
 
 
 def generate_accession_map(
     *,
     content: SubmissionContent,
-    existing_accession_map: Optional[AccessionMap] = None,
+    existing_accession_map: AccessionMap | None = None,
     accession_registry: AccessionRegistry,
     anchor_points_by_target: dict[str, AnchorPoint],
 ) -> AccessionMap:
     """Generate an accession map for the provided content.
 
     If an existing accession map is provided, an updated version is returned. Thereby,
     new accessions are added for new content resources. Existing accessions are kept if
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/models.py` & `metldata-1.3.0/src/metldata/submission_registry/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,19 +14,18 @@
 # limitations under the License.
 #
 
 """Data models"""
 
 from enum import Enum
 from operator import attrgetter
-from typing import Optional
+from typing import TypeAlias
 
 from ghga_service_commons.utils.utc_dates import UTCDatetime, now_as_utc
 from pydantic import BaseModel, Field, field_validator
-from typing_extensions import TypeAlias
 
 from metldata.custom_types import SubmissionContent
 
 AccessionMap: TypeAlias = dict[str, dict[str, str]]
 
 
 class SubmissionStatus(Enum):
@@ -51,23 +50,23 @@
     new_status: SubmissionStatus
 
 
 class SubmissionHeader(BaseModel):
     """Basic information provided for a submission."""
 
     title: str = Field(..., description="A descriptive title for this submission.")
-    description: Optional[str] = Field(None, description="An optional description.")
+    description: str | None = Field(None, description="An optional description.")
 
 
 class Submission(SubmissionHeader):
     """A model for describing a submission."""
 
     id: str
 
-    content: Optional[SubmissionContent] = Field(
+    content: SubmissionContent | None = Field(
         None,
         description=(
             "The metadata content of the submission. Keys on the top level correspond to"
             + " names of anchored metadata classes. Keys and values on the second level"
             + " correspond to the user-defined aliases and contents of class instance. Please note,"
             + " that the user-defined alias might only be unique within the scope of"
             + " the coressponding class and this submission."
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/submission_registry.py` & `metldata-1.3.0/src/metldata/submission_registry/submission_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/submission_registry/submission_store.py` & `metldata-1.3.0/src/metldata/submission_registry/submission_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/transform/__init__.py` & `metldata-1.3.0/src/metldata/transform/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/transform/artifact_publisher.py` & `metldata-1.3.0/src/metldata/transform/artifact_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/transform/base.py` & `metldata-1.3.0/src/metldata/transform/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,32 +14,32 @@
 # limitations under the License.
 #
 
 """Models to describe transformations and workflows."""
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from collections.abc import Callable
 from dataclasses import dataclass
 from graphlib import CycleError, TopologicalSorter
-from typing import Callable, Generic, Optional, TypeVar
+from typing import Generic, TypeVar
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     create_model,
     field_validator,
     model_validator,
 )
 
 from metldata.custom_types import Json
 from metldata.event_handling.models import SubmissionAnnotation
 
 # shortcuts:
-# pylint: disable=unused-import
 from metldata.model_utils.assumptions import MetadataModelAssumptionError  # noqa: F401
 from metldata.model_utils.essentials import MetadataModel
 
 
 class MetadataModelTransformationError(RuntimeError):
     """Raised when a transformation failed when applied to the metadata model."""
 
@@ -118,15 +118,15 @@
 
 
 class WorkflowStepBase(BaseModel, ABC):
     """A base class for workflow steps."""
 
     model_config = ConfigDict(frozen=True)
     description: str = Field(..., description="A description of the step.")
-    input: Optional[str] = Field(
+    input: str | None = Field(
         ...,
         description=(
             "The name of the workflow step from which the output is used as input"
             " for this step. If this is the first step, set to None."
         ),
     )
 
@@ -157,15 +157,14 @@
         description=(
             "A dictionary of artifacts that are output by this workflow."
             + " The keys are the names of the artifacts, and the values are the names"
             + " of the workflow steps that output them."
         ),
     )
 
-    # pylint: disable=no-self-argument
     @field_validator("steps", mode="after")
     def validate_step_references(
         cls,  # noqa: N805
         steps: dict[str, WorkflowStep],
     ) -> dict[str, WorkflowStep]:
         """Validate that workflow steps reference other existing steps as input.
         There should be exactly one step with input=None.
```

### Comparing `metldata-1.2.1/src/metldata/transform/config.py` & `metldata-1.3.0/src/metldata/transform/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,12 +17,11 @@
 """Config parameters and their defaults."""
 
 from metldata.event_handling.event_handling import FileSystemEventConfig
 from metldata.transform.artifact_publisher import ArtifactEventPublisherConfig
 from metldata.transform.source_event_subscriber import SourceEventSubscriberConfig
 
 
-# pylint: disable=too-many-ancestors
 class TransformationEventHandlingConfig(
     FileSystemEventConfig, ArtifactEventPublisherConfig, SourceEventSubscriberConfig
 ):
     """Config parameters for consuming source events and publishing artifacts."""
```

### Comparing `metldata-1.2.1/src/metldata/transform/handling.py` & `metldata-1.3.0/src/metldata/transform/handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `metldata-1.2.1/src/metldata/transform/main.py` & `metldata-1.3.0/src/metldata/transform/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Main logic for running a transformation workflow on submissions."""
 
-from collections.abc import Awaitable
-from typing import Callable
+from collections.abc import Awaitable, Callable
 
 from metldata.event_handling.event_handling import (
     FileSystemEventPublisher,
     FileSystemEventSubscriber,
 )
 from metldata.event_handling.models import SubmissionEventPayload
 from metldata.model_utils.essentials import MetadataModel
```

### Comparing `metldata-1.2.1/src/metldata/transform/source_event_subscriber.py` & `metldata-1.3.0/src/metldata/transform/source_event_subscriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for subscribing to source events."""
 
-from collections.abc import Awaitable
-from typing import Callable
+from collections.abc import Awaitable, Callable
 
 from hexkit.custom_types import Ascii, JsonObject
 from hexkit.protocols.eventsub import EventSubscriberProtocol
 
 from metldata.event_handling.models import SubmissionEventPayload
 from metldata.event_handling.submission_events import SourceEventConfig
 
@@ -40,21 +39,20 @@
         run_workflow_func: Callable[[SubmissionEventPayload], Awaitable[None]],
     ):
         """Initialize with config parameters."""
         self.topics_of_interest = [config.source_event_topic]
         self.types_of_interest = [config.source_event_type]
         self._run_workflow_func = run_workflow_func
 
-    # pylint: disable=unused-argument
     async def _consume_validated(
-        self, *, payload: JsonObject, type_: Ascii, topic: Ascii
+        self, *, payload: JsonObject, type_: Ascii, topic: Ascii, key: Ascii
     ) -> None:
         """
         Receive and process an event with already validated topic and type.
 
         Args:
             payload (JsonObject): The data/payload to send with the event.
             type_ (str): The type of the event.
             topic (str): Name of the topic the event was published to.
         """
-        submission_event_payload = SubmissionEventPayload(**payload)
+        submission_event_payload = SubmissionEventPayload(**payload)  # type: ignore
         await self._run_workflow_func(submission_event_payload)
```

### Comparing `metldata-1.2.1/src/metldata.egg-info/PKG-INFO` & `metldata-1.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: metldata
-Version: 1.2.1
-Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
-Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
-License: Apache 2.0
-Project-URL: Repository, https://github.com/ghga-de/metldata
-Classifier: Development Status :: 1 - Planning
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: hexkit[akafka,mongodb]<3,>=2.1.1
-Requires-Dist: ghga-service-commons[api,auth]<4,>=3.1.1
-Requires-Dist: ghga-event-schemas<4,>=3.0.0
-Requires-Dist: typer~=0.9.0
-Requires-Dist: linkml==1.6.1
-Requires-Dist: linkml-runtime==1.6.0
-Requires-Dist: linkml-validator==0.4.5
-
 [![tests](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/metldata/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/metldata/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/metldata?branch=main)
 
 # Metldata
 
 metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 
@@ -81,29 +54,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:1.2.1
+docker pull ghga/metldata:1.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:1.2.1 .
+docker build -t ghga/metldata:1.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:1.2.1 --help
+docker run -p 8080:8080 ghga/metldata:1.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -166,15 +139,15 @@
 
 - **`kafka_ssl_cafile`** *(string)*: Certificate Authority file path containing certificates used to sign broker certificates. If a CA is not specified, the default system CA will be used if found by OpenSSL. Default: `""`.
 
 - **`kafka_ssl_certfile`** *(string)*: Optional filename of client certificate, as well as any CA certificates needed to establish the certificate's authenticity. Default: `""`.
 
 - **`kafka_ssl_keyfile`** *(string)*: Optional filename containing the client private key. Default: `""`.
 
-- **`kafka_ssl_password`** *(string)*: Optional password to be used for the client private key. Default: `""`.
+- **`kafka_ssl_password`** *(string, format: password)*: Optional password to be used for the client private key. Default: `""`.
 
 - **`generate_correlation_id`** *(boolean)*: A flag, which, if False, will result in an error when inbound requests don't possess a correlation ID. If True, requests without a correlation ID will be assigned a newly generated ID in the correlation ID middleware function. Default: `true`.
 
 
   Examples:
 
   ```json
@@ -357,20 +330,63 @@
   ```json
   []
   ```
 
 
 - **`artifact_infos`** *(array)*: Information for artifacts to be queryable via the Artifacts REST API.
 
-  - **Items**: Refer to *[#/$defs/ArtifactInfo](#$defs/ArtifactInfo)*.
+  - **Items**: Refer to *[#/$defs/ArtifactInfo](#%24defs/ArtifactInfo)*.
 
 - **`loader_token_hashes`** *(array)*: Hashes of tokens used to authenticate for loading artifact.
 
   - **Items** *(string)*
 
+## Definitions
+
+
+- <a id="%24defs/AnchorPoint"></a>**`AnchorPoint`** *(object)*: A model for describing an anchor point for the specified target class.
+
+  - **`target_class`** *(string, required)*: The name of the class to be targeted.
+
+  - **`identifier_slot`** *(string, required)*: The name of the slot in the target class that is used as identifier.
+
+  - **`root_slot`** *(string, required)*: The name of the slot in the root class used to link to the target class.
+
+- <a id="%24defs/ArtifactInfo"></a>**`ArtifactInfo`** *(object)*: Model to describe general information on an artifact.
+Please note, it does not contain actual artifact instances derived from specific
+metadata.
+
+  - **`name`** *(string, required)*: The name of the artifact.
+
+  - **`description`** *(string, required)*: A description of the artifact.
+
+  - **`resource_classes`** *(object, required)*: A dictionary of resource classes for this artifact. The keys are the names of the classes. The values are the corresponding class models. Can contain additional properties.
+
+    - **Additional properties**: Refer to *[#/$defs/ArtifactResourceClass](#%24defs/ArtifactResourceClass)*.
+
+- <a id="%24defs/ArtifactResourceClass"></a>**`ArtifactResourceClass`** *(object)*: Model to describe a resource class of an artifact.
+
+  - **`name`** *(string, required)*: The name of the metadata class.
+
+  - **`description`**: A description of the metadata class. Default: `null`.
+
+    - **Any of**
+
+      - *string*
+
+      - *null*
+
+  - **`anchor_point`**: The anchor point for this metadata class.
+
+    - **All of**
+
+      - : Refer to *[#/$defs/AnchorPoint](#%24defs/AnchorPoint)*.
+
+  - **`json_schema`** *(object, required)*: The JSON schema for this metadata class.
+
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.metldata.yaml`, and place it into one of the following locations:
 - in the current working directory were you are execute the service (on unix: `./.metldata.yaml`)
```

### Comparing `metldata-1.2.1/src/metldata.egg-info/SOURCES.txt` & `metldata-1.3.0/src/metldata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metldata-1.2.1/tests/test_event_handling.py` & `metldata-1.3.0/tests/test_event_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -76,19 +76,19 @@
         events. Only consumes from topic1.
 
         Consumed events are captured in the consumed_events attribute.
         """
 
         def __init__(self):
             self.consumed_events: set[ConsumedEvent] = set()
-            self.topics_of_interest = {"topic1"}
-            self.types_of_interest = {"type1", "type2"}
+            self.topics_of_interest = {"topic1"}  # type: ignore
+            self.types_of_interest = {"type1", "type2"}  # type: ignore
 
         async def _consume_validated(
-            self, *, payload: JsonObject, type_: Ascii, topic: Ascii
+            self, *, payload: JsonObject, type_: Ascii, topic: Ascii, key: Ascii
         ) -> None:
             self.consumed_events.add(
                 ConsumedEvent(topic=topic, type_=type_, payload=json.dumps(payload))
             )
 
     translator = MockSubscriberTranslator()
     subscriber = FileSystemEventSubscriber(
```

### Comparing `metldata-1.2.1/tests/test_metadata_utils.py` & `metldata-1.3.0/tests/test_metadata_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

