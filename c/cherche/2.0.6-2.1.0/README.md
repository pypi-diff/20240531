# Comparing `tmp/cherche-2.0.6.tar.gz` & `tmp/cherche-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherche-2.0.6.tar", last modified: Sat Sep  9 13:05:33 2023, max compression
+gzip compressed data, was "cherche-2.1.0.tar", last modified: Thu May 30 22:39:58 2024, max compression
```

## Comparing `cherche-2.0.6.tar` & `cherche-2.1.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.061211 cherche-2.0.6/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-08-30 11:51:52.000000 cherche-2.0.6/LICENSE
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     8369 2023-09-09 13:05:33.061316 cherche-2.0.6/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7732 2023-08-30 11:51:52.000000 cherche-2.0.6/README.md
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.025876 cherche-2.0.6/cherche/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      134 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-09-09 13:03:11.000000 cherche-2.0.6/cherche/__version__.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.028833 cherche-2.0.6/cherche/compose/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      151 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6368 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/base.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     8823 2023-09-05 22:16:12.000000 cherche-2.0.6/cherche/compose/intersection_union_vote.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    18160 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/pipeline.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4608 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/test_compose.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6904 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/test_union_inter.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1980 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/compose/test_vote.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.029942 cherche-2.0.6/cherche/data/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      104 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/__init__.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.042786 cherche-2.0.6/cherche/data/semanlink/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)   899186 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/semanlink/arxiv.json
--rw-r--r--   0 raphael.sourty   (502) staff       (20)  8324401 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/semanlink/docs.json
--rw-r--r--   0 raphael.sourty   (502) staff       (20)  4587473 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/semanlink/tags.json
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3013 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/semanlink.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    29097 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/towns.json
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1577 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/data/towns.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.052024 cherche-2.0.6/cherche/evaluate/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/evaluate/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4142 2023-09-01 09:03:15.000000 cherche-2.0.6/cherche/evaluate/evaluate.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.052969 cherche-2.0.6/cherche/index/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       52 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/index/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5056 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/index/faiss_index.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.053366 cherche-2.0.6/cherche/qa/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       37 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/qa/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6442 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/qa/qa.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.054143 cherche-2.0.6/cherche/query/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      110 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/query/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1153 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/query/base.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4455 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/query/norvig.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5074 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/query/prf.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.055539 cherche-2.0.6/cherche/rank/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      217 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    10310 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/base.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6692 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/cross_encoder.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4155 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/dpr.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4767 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/embedding.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3805 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/encoder.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3867 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/rank/test_rank.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.059756 cherche-2.0.6/cherche/retrieve/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      332 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/retrieve/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2438 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/retrieve/base.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4637 2023-09-01 09:03:12.000000 cherche-2.0.6/cherche/retrieve/dpr.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4659 2023-09-01 11:47:30.000000 cherche-2.0.6/cherche/retrieve/embedding.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4495 2023-09-01 09:02:27.000000 cherche-2.0.6/cherche/retrieve/encoder.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4822 2023-09-01 09:03:15.000000 cherche-2.0.6/cherche/retrieve/flash.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5047 2023-09-09 12:59:12.000000 cherche-2.0.6/cherche/retrieve/fuzz.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3455 2023-09-01 09:08:00.000000 cherche-2.0.6/cherche/retrieve/lunr.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4139 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/retrieve/test_retrieve.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7672 2023-09-05 22:17:35.000000 cherche-2.0.6/cherche/retrieve/tfidf.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.060948 cherche-2.0.6/cherche/utils/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      174 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/utils/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1468 2023-09-01 09:03:15.000000 cherche-2.0.6/cherche/utils/batch.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1754 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/utils/quantize.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1983 2023-08-30 11:51:52.000000 cherche-2.0.6/cherche/utils/topk.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-09-09 13:05:33.027249 cherche-2.0.6/cherche.egg-info/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     8369 2023-09-09 13:05:32.000000 cherche-2.0.6/cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1437 2023-09-09 13:05:32.000000 cherche-2.0.6/cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-09-09 13:05:32.000000 cherche-2.0.6/cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      736 2023-09-09 13:05:32.000000 cherche-2.0.6/cherche.egg-info/requires.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)        8 2023-09-09 13:05:32.000000 cherche-2.0.6/cherche.egg-info/top_level.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-09-09 13:05:33.062294 cherche-2.0.6/setup.cfg
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1745 2023-08-30 11:51:52.000000 cherche-2.0.6/setup.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.497278 cherche-2.1.0/
+-rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-05-21 12:16:04.000000 cherche-2.1.0/LICENSE
+-rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-05-30 22:39:58.497186 cherche-2.1.0/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     7658 2024-05-30 22:33:58.000000 cherche-2.1.0/README.md
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.470598 cherche-2.1.0/cherche/
+-rw-r--r--   0 raphael    (502) staff       (20)      134 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)       63 2024-05-30 22:27:59.000000 cherche-2.1.0/cherche/__version__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.473441 cherche-2.1.0/cherche/compose/
+-rw-r--r--   0 raphael    (502) staff       (20)      151 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6368 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     8823 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/intersection_union_vote.py
+-rw-r--r--   0 raphael    (502) staff       (20)    18160 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/pipeline.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4608 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/test_compose.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6904 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/test_union_inter.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1980 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/compose/test_vote.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.475109 cherche-2.1.0/cherche/data/
+-rw-r--r--   0 raphael    (502) staff       (20)      104 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/__init__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.482032 cherche-2.1.0/cherche/data/semanlink/
+-rw-r--r--   0 raphael    (502) staff       (20)   899186 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/semanlink/arxiv.json
+-rw-r--r--   0 raphael    (502) staff       (20)  8324401 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/semanlink/docs.json
+-rw-r--r--   0 raphael    (502) staff       (20)  4587473 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/semanlink/tags.json
+-rw-r--r--   0 raphael    (502) staff       (20)     3013 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/semanlink.py
+-rw-r--r--   0 raphael    (502) staff       (20)    29097 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/towns.json
+-rw-r--r--   0 raphael    (502) staff       (20)     1577 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/data/towns.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.486685 cherche-2.1.0/cherche/evaluate/
+-rw-r--r--   0 raphael    (502) staff       (20)       59 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/evaluate/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4094 2024-05-30 22:17:20.000000 cherche-2.1.0/cherche/evaluate/evaluate.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.487478 cherche-2.1.0/cherche/index/
+-rw-r--r--   0 raphael    (502) staff       (20)       52 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/index/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5056 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/index/faiss_index.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.488219 cherche-2.1.0/cherche/qa/
+-rw-r--r--   0 raphael    (502) staff       (20)       37 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/qa/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6442 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/qa/qa.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.489851 cherche-2.1.0/cherche/query/
+-rw-r--r--   0 raphael    (502) staff       (20)      110 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/query/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1153 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/query/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4455 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/query/norvig.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5053 2024-05-30 21:34:21.000000 cherche-2.1.0/cherche/query/prf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.491904 cherche-2.1.0/cherche/rank/
+-rw-r--r--   0 raphael    (502) staff       (20)      217 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10310 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6692 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/cross_encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4155 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/dpr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4767 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/embedding.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3805 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3867 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/rank/test_rank.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.494062 cherche-2.1.0/cherche/retrieve/
+-rw-r--r--   0 raphael    (502) staff       (20)      367 2024-05-30 22:07:08.000000 cherche-2.1.0/cherche/retrieve/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2438 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3609 2024-05-30 22:08:38.000000 cherche-2.1.0/cherche/retrieve/bm25.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4637 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/dpr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4659 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/embedding.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4495 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4822 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/flash.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5047 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/fuzz.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3455 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/lunr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4139 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/retrieve/test_retrieve.py
+-rw-r--r--   0 raphael    (502) staff       (20)     7687 2024-05-30 22:22:51.000000 cherche-2.1.0/cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.494682 cherche-2.1.0/cherche/utils/
+-rw-r--r--   0 raphael    (502) staff       (20)      174 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/utils/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1468 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/utils/batch.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1754 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/utils/quantize.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1983 2024-05-21 12:16:04.000000 cherche-2.1.0/cherche/utils/topk.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 22:39:58.494883 cherche-2.1.0/cherche.egg-info/
+-rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-05-30 22:39:58.000000 cherche-2.1.0/cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     1462 2024-05-30 22:39:58.000000 cherche-2.1.0/cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        1 2024-05-30 22:39:58.000000 cherche-2.1.0/cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael    (502) staff       (20)      788 2024-05-30 22:39:58.000000 cherche-2.1.0/cherche.egg-info/requires.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        8 2024-05-30 22:39:58.000000 cherche-2.1.0/cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       79 2024-05-30 22:39:58.497500 cherche-2.1.0/setup.cfg
+-rw-r--r--   0 raphael    (502) staff       (20)     1767 2024-05-30 21:34:25.000000 cherche-2.1.0/setup.py
```

### Comparing `cherche-2.0.6/LICENSE` & `cherche-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/PKG-INFO` & `cherche-2.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: cherche
-Version: 2.0.6
-Summary: Neural Search
-Home-page: https://github.com/raphaelsty/cherche
-Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
-Author: Raphael Sourty
-Author-email: raphael.sourty@gmail.com
-License: MIT
-Keywords: neural search,information retrieval,question answering,semantic search
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: cpu
-Provides-Extra: gpu
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
   <h1>Cherche</h1>
   <p>Neural search</p>
 </div>
 
 <p align="center"><img width=300 src="docs/img/logo.png"/></p>
 
@@ -33,14 +13,16 @@
   <!-- License -->
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="license"></a>
 </div>
 
 
 Cherche enables the development of a neural search pipeline that employs retrievers and pre-trained language models both as retrievers and rankers. The primary advantage of Cherche lies in its capacity to construct end-to-end pipelines. Additionally, Cherche is well-suited for offline semantic search due to its compatibility with batch computation.
 
+Here are some of the features Cherche offers:
+
 [Live demo of a NLP search engine powered by Cherche](https://raphaelsty.github.io/knowledge/?query=cherche%20neural%20search)
 
 ![Alt text](docs/img/explain.png)
 
 ## Installation 🤖
 
 To install Cherche for use with a simple retriever on CPU, such as TfIdf, Flash, Lunr, Fuzz, use the following command:
@@ -98,20 +80,26 @@
 ### Retriever ranker
 
 Here is an example of a neural search pipeline composed of a TF-IDF that quickly retrieves documents, followed by a ranking model. The ranking model sorts the documents produced by the retriever based on the semantic similarity between the query and the documents. We can call the pipeline using a list of queries and get relevant documents for each query.
 
 ```python
 from cherche import data, retrieve, rank
 from sentence_transformers import SentenceTransformer
+from lenlp import sparse
 
 # List of dicts
 documents = data.load_towns()
 
 # Retrieve on fields title and article
-retriever = retrieve.TfIdf(key="id", on=["title", "article"], documents=documents, k=30)
+retriever = retrieve.BM25(
+  key="id", 
+  on=["title", "article"], 
+  documents=documents, 
+  k=30
+)
 
 # Rank on fields title and article
 ranker = rank.Encoder(
     key = "id",
     on = ["title", "article"],
     encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode,
     k = 3,
@@ -179,14 +167,15 @@
 ```
 
 ## Retrieve
 
 Cherche provides [retrievers](https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input documents based on a query.
 
 - retrieve.TfIdf
+- retrieve.BM25
 - retrieve.Lunr
 - retrieve.Flash
 - retrieve.Encoder
 - retrieve.DPR
 - retrieve.Fuzz
 - retrieve.Embedding
 
@@ -209,15 +198,15 @@
 Cherche was created for/by Renault and is now available to all.
 We welcome all contributions.
 
 <p align="center"><img src="docs/img/renault.jpg"/></p>
 
 ## Acknowledgements 👏
 
-TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
+Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
 ```bibtex
 @inproceedings{Sourty2022sigir,
```

#### html2text {}

```diff
@@ -1,56 +1,48 @@
-Metadata-Version: 2.1 Name: cherche Version: 2.0.6 Summary: Neural Search Home-
-page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
-user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
-raphael.sourty@gmail.com License: MIT Keywords: neural search,information
-retrieval,question answering,semantic search Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown Provides-Extra: cpu Provides-Extra: gpu Provides-Extra: dev
-License-File: LICENSE
                              ************ CChheerrcchhee ************
                                  Neural search
                               [docs/img/logo.png]
                         _[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_e_m_o_]_[_l_i_c_e_n_s_e_]
 Cherche enables the development of a neural search pipeline that employs
 retrievers and pre-trained language models both as retrievers and rankers. The
 primary advantage of Cherche lies in its capacity to construct end-to-end
 pipelines. Additionally, Cherche is well-suited for offline semantic search due
-to its compatibility with batch computation. [Live demo of a NLP search engine
-powered by Cherche](https://raphaelsty.github.io/knowledge/
-?query=cherche%20neural%20search) ![Alt text](docs/img/explain.png) ##
-Installation ð¤ To install Cherche for use with a simple retriever on CPU,
-such as TfIdf, Flash, Lunr, Fuzz, use the following command: ```sh pip install
-cherche ``` To install Cherche for use with any semantic retriever or ranker on
-CPU, use the following command: ```sh pip install "cherche[cpu]" ``` Finally,
-if you plan to use any semantic retriever or ranker on GPU, use the following
-command: ```sh pip install "cherche[gpu]" ``` By following these installation
-instructions, you will be able to use Cherche with the appropriate requirements
-for your needs. ### Documentation Documentation is available [here](https://
-raphaelsty.github.io/cherche/). It provides details about retrievers, rankers,
-pipelines and examples. ## QuickStart ð ### Documents Cherche allows
-findings the right document within a list of objects. Here is an example of a
-corpus. ```python from cherche import data documents = data.load_towns()
-documents[:3] [{'id': 0, 'title': 'Paris', 'url': 'https://en.wikipedia.org/
-wiki/Paris', 'article': 'Paris is the capital and most populous city of
-France.'}, {'id': 1, 'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/
-Paris', 'article': "Since the 17th century, Paris has been one of Europe's
-major centres of science, and arts."}, {'id': 2, 'title': 'Paris', 'url':
-'https://en.wikipedia.org/wiki/Paris', 'article': 'The City of Paris is the
-centre and seat of government of the region and province of Ãle-de-France.' }]
-``` ### Retriever ranker Here is an example of a neural search pipeline
-composed of a TF-IDF that quickly retrieves documents, followed by a ranking
-model. The ranking model sorts the documents produced by the retriever based on
-the semantic similarity between the query and the documents. We can call the
-pipeline using a list of queries and get relevant documents for each query.
-```python from cherche import data, retrieve, rank from sentence_transformers
-import SentenceTransformer # List of dicts documents = data.load_towns() #
-Retrieve on fields title and article retriever = retrieve.TfIdf(key="id", on=
-["title", "article"], documents=documents, k=30) # Rank on fields title and
-article ranker = rank.Encoder( key = "id", on = ["title", "article"], encoder =
+to its compatibility with batch computation. Here are some of the features
+Cherche offers: [Live demo of a NLP search engine powered by Cherche](https://
+raphaelsty.github.io/knowledge/?query=cherche%20neural%20search) ![Alt text]
+(docs/img/explain.png) ## Installation ð¤ To install Cherche for use with a
+simple retriever on CPU, such as TfIdf, Flash, Lunr, Fuzz, use the following
+command: ```sh pip install cherche ``` To install Cherche for use with any
+semantic retriever or ranker on CPU, use the following command: ```sh pip
+install "cherche[cpu]" ``` Finally, if you plan to use any semantic retriever
+or ranker on GPU, use the following command: ```sh pip install "cherche[gpu]"
+``` By following these installation instructions, you will be able to use
+Cherche with the appropriate requirements for your needs. ### Documentation
+Documentation is available [here](https://raphaelsty.github.io/cherche/). It
+provides details about retrievers, rankers, pipelines and examples. ##
+QuickStart ð ### Documents Cherche allows findings the right document within
+a list of objects. Here is an example of a corpus. ```python from cherche
+import data documents = data.load_towns() documents[:3] [{'id': 0, 'title':
+'Paris', 'url': 'https://en.wikipedia.org/wiki/Paris', 'article': 'Paris is the
+capital and most populous city of France.'}, {'id': 1, 'title': 'Paris', 'url':
+'https://en.wikipedia.org/wiki/Paris', 'article': "Since the 17th century,
+Paris has been one of Europe's major centres of science, and arts."}, {'id': 2,
+'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/Paris', 'article': 'The
+City of Paris is the centre and seat of government of the region and province
+of Ãle-de-France.' }] ``` ### Retriever ranker Here is an example of a neural
+search pipeline composed of a TF-IDF that quickly retrieves documents, followed
+by a ranking model. The ranking model sorts the documents produced by the
+retriever based on the semantic similarity between the query and the documents.
+We can call the pipeline using a list of queries and get relevant documents for
+each query. ```python from cherche import data, retrieve, rank from
+sentence_transformers import SentenceTransformer from lenlp import sparse #
+List of dicts documents = data.load_towns() # Retrieve on fields title and
+article retriever = retrieve.BM25( key="id", on=["title", "article"],
+documents=documents, k=30 ) # Rank on fields title and article ranker =
+rank.Encoder( key = "id", on = ["title", "article"], encoder =
 SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode, k = 3, )
 # Pipeline creation search = retriever + ranker search.add(documents=documents)
 # Search documents for 3 queries. search(["Bordeaux", "Paris", "Toulouse"]) [[
 {'id': 57, 'similarity': 0.69513524}, {'id': 63, 'similarity': 0.6214994},
 {'id': 65, 'similarity': 0.61809087}], [{'id': 16, 'similarity': 0.59158516},
 {'id': 0, 'similarity': 0.58217555}, {'id': 1, 'similarity': 0.57944715}], [
 {'id': 26, 'similarity': 0.6925601}, {'id': 37, 'similarity': 0.63977146},
@@ -67,37 +59,35 @@
 en.wikipedia.org/wiki/Paris', 'similarity': 0.57944715}], [{'id': 26, 'title':
 'Toulouse', 'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity':
 0.6925601}, {'id': 37, 'title': 'Toulouse', 'url': 'https://en.wikipedia.org/
 wiki/Toulouse', 'similarity': 0.63977146}, {'id': 28, 'title': 'Toulouse',
 'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity': 0.62772334}]]
 ``` ## Retrieve Cherche provides [retrievers](https://raphaelsty.github.io/
 cherche/retrieve/retrieve/) that filter input documents based on a query. -
-retrieve.TfIdf - retrieve.Lunr - retrieve.Flash - retrieve.Encoder -
-retrieve.DPR - retrieve.Fuzz - retrieve.Embedding ## Rank Cherche provides
-[rankers](https://raphaelsty.github.io/cherche/rank/rank/) that filter
-documents in output of retrievers. Cherche rankers are compatible with
-[SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html)
+retrieve.TfIdf - retrieve.BM25 - retrieve.Lunr - retrieve.Flash -
+retrieve.Encoder - retrieve.DPR - retrieve.Fuzz - retrieve.Embedding ## Rank
+Cherche provides [rankers](https://raphaelsty.github.io/cherche/rank/rank/
+) that filter documents in output of retrievers. Cherche rankers are compatible
+with [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html)
 models which are available on [Hugging Face hub](https://huggingface.co/
 models?pipeline_tag=zero-shot-classification&sort=downloads). - rank.Encoder -
 rank.DPR - rank.CrossEncoder - rank.Embedding ## Question answering Cherche
 provides modules dedicated to question answering. These modules are compatible
 with Hugging Face's pre-trained models and fully integrated into neural search
 pipelines. ## Contributors ð¤ Cherche was created for/by Renault and is now
 available to all. We welcome all contributions.
                             [docs/img/renault.jpg]
-## Acknowledgements ð TfIdf retriever is a wrapper around [scikit-learn's
-TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/
-sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
-wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
-retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
-flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
-use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
-docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
-use cherche to produce results for your scientific publication, please refer to
-our SIGIR paper: ```bibtex @inproceedings{Sourty2022sigir, author = {Raphael
-Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
-{CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
-booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
-The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
-raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
-Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
-scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
+## Acknowledgements ð Lunr retriever is a wrapper around [Lunr.py](https://
+github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around
+[FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder
+rankers are wrappers dedicated to the use of the pre-trained models of
+[SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a
+neural search pipeline. ## Citations If you use cherche to produce results for
+your scientific publication, please refer to our SIGIR paper: ```bibtex
+@inproceedings{Sourty2022sigir, author = {Raphael Sourty and Jose G. Moreno and
+Lynda Tamine and Francois-Paul Servant}, title = {CHERCHE: A new tool to
+rapidly implement pipelines in information retrieval}, booktitle = {Proceedings
+of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾ The Cherche dev team is
+made up of [RaphaÃ«l Sourty](https://github.com/raphaelsty), [FranÃ§ois-Paul
+Servant](https://github.com/fpservant), [Nicolas Bizzozzero](https://
+github.com/NicolasBizzozzero), [Jose G Moreno](https://scholar.google.com/
+citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-2.0.6/cherche/compose/base.py` & `cherche-2.1.0/cherche/compose/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/compose/intersection_union_vote.py` & `cherche-2.1.0/cherche/compose/intersection_union_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/compose/pipeline.py` & `cherche-2.1.0/cherche/compose/pipeline.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/compose/test_compose.py` & `cherche-2.1.0/cherche/compose/test_compose.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/compose/test_union_inter.py` & `cherche-2.1.0/cherche/compose/test_union_inter.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/compose/test_vote.py` & `cherche-2.1.0/cherche/compose/test_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/semanlink/arxiv.json` & `cherche-2.1.0/cherche/data/semanlink/arxiv.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/semanlink/docs.json` & `cherche-2.1.0/cherche/data/semanlink/docs.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/semanlink/tags.json` & `cherche-2.1.0/cherche/data/semanlink/tags.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/semanlink.py` & `cherche-2.1.0/cherche/data/semanlink.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/towns.json` & `cherche-2.1.0/cherche/data/towns.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/data/towns.py` & `cherche-2.1.0/cherche/data/towns.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/evaluate/evaluate.py` & `cherche-2.1.0/cherche/evaluate/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 __all__ = ["evaluation"]
 
 import collections
 import typing
 
-import numpy as np
-
 __all__ = ["evaluation"]
 
 
 class Mean:
     """Online running mean.
 
     Reference
@@ -52,25 +50,25 @@
     batch_size
         Batch size.
 
     Examples
     --------
     >>> from pprint import pprint as print
     >>> from cherche import data, evaluate, retrieve
-    >>> from sklearn.feature_extraction.text import TfidfVectorizer
+    >>> from lenlp import sparse
 
     >>> documents, query_answers = data.arxiv_tags(
     ...    arxiv_title=True, arxiv_summary=False, comment=False
     ... )
 
     >>> search = retrieve.TfIdf(
     ...     key="uri",
     ...     on=["prefLabel_text", "altLabel_text"],
     ...     documents=documents,
-    ...     tfidf=TfidfVectorizer(lowercase=True, ngram_range=(3, 7), analyzer="char"),
+    ...     tfidf=sparse.TfidfVectorizer(normalize=True, ngram_range=(3, 7), analyzer="char"),
     ... ) + documents
 
     >>> scores = evaluate.evaluation(search=search, query_answers=query_answers, k=10)
 
     >>> print(scores)
     {'F1@1': '26.52%',
      'F1@2': '29.41%',
```

### Comparing `cherche-2.0.6/cherche/index/faiss_index.py` & `cherche-2.1.0/cherche/index/faiss_index.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/qa/qa.py` & `cherche-2.1.0/cherche/qa/qa.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/query/base.py` & `cherche-2.1.0/cherche/query/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/query/norvig.py` & `cherche-2.1.0/cherche/query/norvig.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/query/prf.py` & `cherche-2.1.0/cherche/query/prf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 
 import numpy as np
 import sklearn
-from sklearn.feature_extraction.text import TfidfVectorizer
+from lenlp import sparse
 from sklearn.metrics.pairwise import cosine_similarity
 
 from ..utils import yield_batch_single
 from .base import Query
 
 __all__ = ["PRF"]
 
@@ -17,15 +17,15 @@
     retrieve top words from relevant documents to give a proper augmentation of a given query.
 
     Parameters
     ----------
     on
         Fields to use for fitting the spelling corrector on.
     tf
-        defaults to sklearn.feature_extraction.text.TfidfVectorizer.
+        defaults to sklearn.feature_extraction.text.sparse.TfidfVectorizer.
         If you want to implement your own tf, it needs to follow the sklearn base API and provides the `transform`
         `fit_transform` and `get_feature_names_out` methods. See sklearn documentation for more information.
     nb_docs
         Number of documents from which to retrieve top-terms.
     nb_terms_per_doc
         Number of terms to extract from each top documents retrieved.
 
@@ -61,15 +61,15 @@
 
     """
 
     def __init__(
         self,
         on: typing.Union[str, list],
         documents: list,
-        tf: sklearn.feature_extraction.text.CountVectorizer = TfidfVectorizer(),
+        tf: sklearn.feature_extraction.text.CountVectorizer = sparse.TfidfVectorizer(),
         nb_docs: int = 5,
         nb_terms_per_doc: int = 3,
     ) -> None:
         super().__init__(on=on)
         self.nb_docs = nb_docs
         self.nb_terms_per_doc = nb_terms_per_doc
         self.func = tf
```

### Comparing `cherche-2.0.6/cherche/rank/base.py` & `cherche-2.1.0/cherche/rank/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/rank/cross_encoder.py` & `cherche-2.1.0/cherche/rank/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/rank/dpr.py` & `cherche-2.1.0/cherche/rank/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/rank/embedding.py` & `cherche-2.1.0/cherche/rank/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/rank/encoder.py` & `cherche-2.1.0/cherche/rank/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/rank/test_rank.py` & `cherche-2.1.0/cherche/rank/test_rank.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/base.py` & `cherche-2.1.0/cherche/retrieve/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/dpr.py` & `cherche-2.1.0/cherche/retrieve/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/embedding.py` & `cherche-2.1.0/cherche/retrieve/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/encoder.py` & `cherche-2.1.0/cherche/retrieve/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/flash.py` & `cherche-2.1.0/cherche/retrieve/flash.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/fuzz.py` & `cherche-2.1.0/cherche/retrieve/fuzz.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/lunr.py` & `cherche-2.1.0/cherche/retrieve/lunr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/test_retrieve.py` & `cherche-2.1.0/cherche/retrieve/test_retrieve.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/retrieve/tfidf.py` & `cherche-2.1.0/cherche/retrieve/tfidf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["TfIdf"]
 
 import typing
 
 import numpy as np
+from lenlp import sparse
 from scipy.sparse import csc_matrix, hstack
-from sklearn.feature_extraction.text import TfidfVectorizer
 
 from ..utils import yield_batch
 from .base import Retriever
 
 
 class TfIdf(Retriever):
     """TfIdf retriever based on cosine similarities.
@@ -88,23 +88,25 @@
     """
 
     def __init__(
         self,
         key: str,
         on: typing.Union[str, list],
         documents: typing.List[typing.Dict[str, str]] = None,
-        tfidf: TfidfVectorizer = None,
+        tfidf: sparse.TfidfVectorizer = None,
         k: typing.Optional[int] = None,
         batch_size: int = 1024,
         fit: bool = True,
     ) -> None:
         super().__init__(key=key, on=on, k=k, batch_size=batch_size)
 
         self.tfidf = (
-            TfidfVectorizer(lowercase=True, ngram_range=(3, 7), analyzer="char_wb")
+            sparse.TfidfVectorizer(
+                normalize=True, ngram_range=(3, 7), analyzer="char_wb"
+            )
             if tfidf is None
             else tfidf
         )
 
         self.documents = [{self.key: document[self.key]} for document in documents]
         self.duplicates = {document[self.key]: True for document in documents}
 
@@ -203,15 +205,15 @@
             Batch size to use to retrieve documents.
         """
         k = k if k is not None else self.k
 
         ranked = []
 
         for batch in yield_batch(
-            q,
+            array=q,
             batch_size=batch_size if batch_size is not None else self.batch_size,
             desc=f"{self.__class__.__name__} retriever",
             tqdm_bar=tqdm_bar,
         ):
             similarities = -1 * self.tfidf.transform(batch).dot(self.matrix)
 
             batch_match, batch_similarities = self.top_k(similarities=similarities, k=k)
```

### Comparing `cherche-2.0.6/cherche/utils/batch.py` & `cherche-2.1.0/cherche/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/utils/quantize.py` & `cherche-2.1.0/cherche/utils/quantize.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche/utils/topk.py` & `cherche-2.1.0/cherche/utils/topk.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.6/cherche.egg-info/SOURCES.txt` & `cherche-2.1.0/cherche.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 cherche/rank/cross_encoder.py
 cherche/rank/dpr.py
 cherche/rank/embedding.py
 cherche/rank/encoder.py
 cherche/rank/test_rank.py
 cherche/retrieve/__init__.py
 cherche/retrieve/base.py
+cherche/retrieve/bm25.py
 cherche/retrieve/dpr.py
 cherche/retrieve/embedding.py
 cherche/retrieve/encoder.py
 cherche/retrieve/flash.py
 cherche/retrieve/fuzz.py
 cherche/retrieve/lunr.py
 cherche/retrieve/test_retrieve.py
```

### Comparing `cherche-2.0.6/cherche.egg-info/requires.txt` & `cherche-2.1.0/cherche.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 numpy>=1.23.5
 scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
+lenlp>=1.0.3
 
 [cpu]
 numpy>=1.23.5
 scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
+lenlp>=1.0.3
 sentence-transformers>=2.2.2
 faiss-cpu>=1.7.4
 
 [dev]
 numpy>=1.23.5
 scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
+lenlp>=1.0.3
 sentence-transformers>=2.2.2
 faiss-cpu>=1.7.4
 numpydoc>=1.4.0
 mkdocs_material>=8.3.5
 mkdocs-awesome-pages-plugin>=2.7.0
 mkdocs-jupyter>=0.21.0
 pytest-cov>=4.0.0
@@ -40,9 +43,10 @@
 numpy>=1.23.5
 scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
+lenlp>=1.0.3
 sentence-transformers>=2.2.2
 faiss-gpu>=1.7.4
```

### Comparing `cherche-2.0.6/setup.py` & `cherche-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "numpy >= 1.23.5",
     "scikit-learn >= 1.1.2",
     "lunr >= 0.6.2",
     "rapidfuzz >= 3.0.0",
     "flashtext >= 2.7",
     "tqdm >= 4.62.3",
     "scipy >= 1.7.3",
+    "lenlp >= 1.0.3",
 ]
 
 cpu = ["sentence-transformers >= 2.2.2", "faiss-cpu >= 1.7.4"]
 gpu = ["sentence-transformers >= 2.2.2", "faiss-gpu >= 1.7.4"]
 dev = [
     "numpydoc >= 1.4.0",
     "mkdocs_material >= 8.3.5",
```

