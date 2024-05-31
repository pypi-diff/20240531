# Comparing `tmp/modelbest_sdk-0.1.6.tar.gz` & `tmp/modelbest_sdk-0.1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbest_sdk-0.1.6.tar", last modified: Mon May 27 13:11:04 2024, max compression
+gzip compressed data, was "modelbest_sdk-0.1.8.4.tar", last modified: Fri May 31 12:57:11 2024, max compression
```

## Comparing `modelbest_sdk-0.1.6.tar` & `modelbest_sdk-0.1.8.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       99 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/MANIFEST.in
--rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/PKG-INFO
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      209 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/README.md
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/__init__.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5434 2024-05-27 13:08:02.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/batched_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2606 2024-05-27 12:13:33.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/cache.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2667 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/range.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1065 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/cuda_prefetcher.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)    11228 2024-05-27 13:04:55.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/mbtable_iterable_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5045 2024-05-23 12:03:16.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/segment_dataset.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4938 2024-05-27 10:14:19.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/modelbest_dataloader.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       58 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/sampler.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      344 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/weighted_sampler.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2801 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     7642 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2220 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      853 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/utils.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4133 2024-05-27 13:10:02.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/weighted_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/file_format/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/__init__.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/
--rwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)  7125976 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5910 2024-05-22 10:23:07.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2953 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_builder.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4765 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_partition.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/modelbest_sdk/proto/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      405 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/breadcrumb.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3259 2024-05-21 11:42:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/chatdoc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5842 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/const.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      830 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/context.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3846 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/data_base.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      631 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_checkpoint.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      454 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_context.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1806 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/general_doc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1624 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/general_servlet_rpc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3408 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/linkinfo.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1556 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/mergeddoc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      497 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/traindoc.thrift
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/
--rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1913 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        1 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       19 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/top_level.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       38 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/setup.cfg
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      708 2024-05-27 13:10:44.000000 modelbest_sdk-0.1.6/setup.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/test/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/test/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4124 2024-05-27 07:16:24.000000 modelbest_sdk-0.1.6/test/test_base.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1258 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/test/test_batched_dataset.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4820 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/test/test_checkpoint.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      881 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_dataset_context.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2682 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_mbtable.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2248 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_mbtable_partition.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.646453 modelbest_sdk-0.1.8.4/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       99 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/MANIFEST.in
+-rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      707 2024-05-31 12:57:11.646453 modelbest_sdk-0.1.8.4/PKG-INFO
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      209 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/README.md
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.634453 modelbest_sdk-0.1.8.4/modelbest_sdk/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/__init__.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.634453 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5433 2024-05-30 07:02:22.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/batched_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.634453 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2606 2024-05-27 12:13:33.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/cache.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2667 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/range.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1065 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/cuda_prefetcher.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)    11228 2024-05-30 07:02:22.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/mbtable_iterable_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.634453 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/megatron/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/megatron/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5045 2024-05-23 12:03:16.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/megatron/segment_dataset.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     6841 2024-05-30 09:49:15.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/modelbest_dataloader.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.638453 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/sampler/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/sampler/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       58 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/sampler/sampler.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1134 2024-05-31 09:28:42.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/sampler/weighted_megatron_sampler.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      891 2024-05-30 08:42:19.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/sampler/weighted_sampler.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.638453 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2801 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     7642 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2220 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      853 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/utils.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4384 2024-05-31 11:28:23.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/weighted_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.638453 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/__init__.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.638453 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/lib/
+-rwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)  7125976 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5910 2024-05-29 03:21:01.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2953 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable_builder.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4765 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable_partition.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.646453 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      405 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/breadcrumb.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3259 2024-05-21 11:42:27.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/chatdoc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5842 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/const.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      830 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/context.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3846 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/data_base.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      631 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/dataset_checkpoint.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      454 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/dataset_context.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1806 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/general_doc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1624 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/general_servlet_rpc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3408 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/linkinfo.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1556 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/mergeddoc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      497 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.8.4/modelbest_sdk/proto/traindoc.thrift
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.634453 modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/
+-rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      707 2024-05-31 12:57:11.000000 modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1972 2024-05-31 12:57:11.000000 modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        1 2024-05-31 12:57:11.000000 modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       19 2024-05-31 12:57:11.000000 modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       38 2024-05-31 12:57:11.646453 modelbest_sdk-0.1.8.4/setup.cfg
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      710 2024-05-31 12:57:08.000000 modelbest_sdk-0.1.8.4/setup.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-31 12:57:11.646453 modelbest_sdk-0.1.8.4/test/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.8.4/test/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4124 2024-05-27 07:16:24.000000 modelbest_sdk-0.1.8.4/test/test_base.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1258 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/test/test_batched_dataset.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4820 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.8.4/test/test_checkpoint.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      881 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/test/test_dataset_context.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2682 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/test/test_mbtable.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2248 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.8.4/test/test_mbtable_partition.py
```

### Comparing `modelbest_sdk-0.1.6/PKG-INFO` & `modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: modelbest_sdk
-Version: 0.1.6
+Name: modelbest-sdk
+Version: 0.1.8.4
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## 项目名称
 > 设计文档: https://www.kdocs.cn/l/cvKBY8SqJoCC  
 > Release Note: https://www.kdocs.cn/l/cvR7iKFqYQqY  
 > 快速上手: https://www.kdocs.cn/l/caTTLzF7yoWF  
 > 使用样例: example/*.py
```

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/batched_dataset.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/batched_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         self.max_total_length = batch_size * max_len
         self.batch_size = 1
         self.drop_last = drop_last
         
         self.buffer = []
         self.current_length = 0
 
-        # 初始化tag_to_index
-        self.tag_to_hash = defaultdict()
+        # 初始化hash_to_tag
+        self.hash_to_tag = defaultdict()
       
     def put(self, data):
         self.buffer.append(data)
         self.current_length += len(data['doc'].token_ids)
     
     def pop(self):
         lengths = []
@@ -73,15 +73,15 @@
             "dataset_ids": dataset_ids,
             "indexes": indexes,
             "cu_seqlens": cu_seqlens,
             "max_seqlen": int(torch.max(cu_seqlens[1:] - cu_seqlens[:-1])),
             "lengths": torch.tensor(sum(lengths)).int(),
             "position_ids": position_ids,
             "tags": tags,
-            "tag_to_hash": self.tag_to_hash
+            "hash_to_tag": self.hash_to_tag
         }
         self.current_length = 0
         return batch
         
 
     def will_exceed(self, data):
         return self.current_length + len(data['doc'].token_ids) > self.max_total_length
@@ -96,15 +96,15 @@
 
     @staticmethod
     def collate_fn(batch):
         return batch[0]
     
     def encode_tags(self, token_ids, tag):
         tag_hash = self._get_tag_hash(tag)
-        self.tag_to_hash[tag] = tag_hash
+        self.hash_to_tag[tag_hash] = tag
         return torch.full((len(token_ids),), tag_hash, dtype=torch.int64)
     
     def _get_tag_hash(self, tag: str) -> int:
         hash_obj = hashlib.sha256(tag.encode('utf-8'))
         return int(hash_obj.hexdigest(), 16) & ((1 << 63) - 1)
 
 if __name__ == '__main__':
```

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/cache.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/cache.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/range.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/common/range.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/cuda_prefetcher.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/cuda_prefetcher.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/mbtable_iterable_dataset.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/mbtable_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/segment_dataset.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/megatron/segment_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/modelbest_dataloader.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/modelbest_dataloader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+from typing import List
+from more_itertools import distribute
 import torch
 from modelbest_sdk.dataset.batched_dataset import BatchedDataset
 from modelbest_sdk.dataset.megatron.segment_dataset import SegmentDataset
 from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import DatasetCheckpointList, DatasetInfoList
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 from modelbest_sdk.dataset.weighted_dataset import WeightedDataset
 
@@ -99,14 +101,60 @@
             for path in os.listdir(resume_dir):
                 abs_path = os.path.join(resume_dir, path)
                 if merged_ckpt is None:
                     merged_ckpt = DatasetCheckpointList.load_from_file(abs_path)
                 else:
                     merged_ckpt.merge(DatasetCheckpointList.load_from_file(abs_path))
             self.load_checkpoint(merged_ckpt)
+    
+    def progress(self, global_checkpoint: List[DatasetCheckpointList]):
+        # This is a approximate progress calculation
+        # This is used after:
+        #   global_ckpt_list = [_ for _ in range(world_size)]
+        #   dist.all_gather_object(global_ckpt_list, dataloader.checkpoint())
+        #   dataloader.progress(global_ckpt_list)
+        # or other all gather functions
+        if self.context.rank != 0:
+            return
+        merged_ckpt = None
+        for ckpt in global_checkpoint:
+            if merged_ckpt is None:
+                merged_ckpt = ckpt
+            else:
+                merged_ckpt.merge(ckpt)
+        
+        path_len_map = self.weighted_dataset.get_path_len_map()
+        progress_dict = {}
+
+        for checkpoint in merged_ckpt.checkpoint_list:
+            dataset_info = checkpoint.dataset_info
+            used = checkpoint.used
+            
+            total_samples_per_epoch = path_len_map[dataset_info.path]
+            consumed_samples = 0
+            
+            
+            for chunk, index_set in used.active.items():
+                consumed_samples += len(index_set)
+            min_epoch = 2048 if used.done else 0
+            for epoch, chunk_set in used.done.items():
+                min_epoch = min(min_epoch, epoch)
+                for chunk in chunk_set:
+                    consumed_samples += (chunk.stop - chunk.start)
+            if min_epoch > 0:
+                consumed_samples += total_samples_per_epoch * min_epoch
+
+            progress_percentage = consumed_samples / total_samples_per_epoch
+            
+            progress_dict[dataset_info.path] = {
+                "samples_per_epoch": total_samples_per_epoch,
+                "samples_consumed": consumed_samples,
+                "progress": progress_percentage
+            }
+        return progress_dict
             
 class MegatronExternalDataloader(ModelbestDataloader):
     def setup_dataset(self, context, batch_size, max_len):
         self.batched_dataset = SegmentDataset(
             context=context,
             weighted_dataset=self.weighted_dataset,
             max_len=max_len
```

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/base_doc.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/base_doc.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/utils.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/thrift_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/dataset/weighted_dataset.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/dataset/weighted_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         self.sampler = WeightedSampler(weights=self.dataset_weights, seed=self.context.world_size + self.context.rank)
         while True:
             if all(d.exhausted for d in self.datasets):
                 logger.warning(f"All dataset exhaust on rank {self.context.rank}")
                 break
             idx = self.sampler()
             if self.datasets[idx].exhausted:
-                print(f"Dataset {idx} exhaust on rank {self.context.rank}")
+                logger.warning(f"Dataset {idx} exhaust on rank {self.context.rank}")
+                self.sampler.remove_index(idx)
                 continue
             chosen_iter = self.datasets_iter[idx]
             try:
                 data = next(chosen_iter)
                 if data is None:
                     continue
                 data['dataset_idx'] = idx
@@ -85,14 +86,19 @@
         for i, checkpoint in enumerate(dataset_checkpoint_list.checkpoint_list):
             self.datasets[i].load_checkpoint(checkpoint)
             
     def update(self, dataset_entries: Dict[int, Dict]):
         for i, entries in dataset_entries.items():
             self.datasets[i].update(entries)
     
+    def __len__(self):
+        return sum(len(dataset) for dataset in self.datasets)
+    
+    def get_path_len_map(self):
+        return {dataset.path: len(dataset) for dataset in self.datasets}
 
 if __name__ == '__main__':
     context = DatasetContext(world_size=1, rank=0, num_workers=1)
 
     dataset_info_list = [
         DatasetInfo(
             path="/home/emr-user/modelbest_sdk/test/base_doc_simple",
```

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so` & `modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_builder.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable_builder.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_partition.py` & `modelbest_sdk-0.1.8.4/modelbest_sdk/file_format/mbtable_partition.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/chatdoc.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/chatdoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/const.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/const.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/context.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/context.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/data_base.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/data_base.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_checkpoint.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/dataset_checkpoint.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/general_doc.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/general_doc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/general_servlet_rpc.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/general_servlet_rpc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/linkinfo.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/linkinfo.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk/proto/mergeddoc.thrift` & `modelbest_sdk-0.1.8.4/modelbest_sdk/proto/mergeddoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk.egg-info/PKG-INFO` & `modelbest_sdk-0.1.8.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: modelbest-sdk
-Version: 0.1.6
+Name: modelbest_sdk
+Version: 0.1.8.4
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## 项目名称
 > 设计文档: https://www.kdocs.cn/l/cvKBY8SqJoCC  
 > Release Note: https://www.kdocs.cn/l/cvR7iKFqYQqY  
 > 快速上手: https://www.kdocs.cn/l/caTTLzF7yoWF  
 > 使用样例: example/*.py
```

### Comparing `modelbest_sdk-0.1.6/modelbest_sdk.egg-info/SOURCES.txt` & `modelbest_sdk-0.1.8.4/modelbest_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 modelbest_sdk/dataset/common/__init__.py
 modelbest_sdk/dataset/common/cache.py
 modelbest_sdk/dataset/common/range.py
 modelbest_sdk/dataset/megatron/__init__.py
 modelbest_sdk/dataset/megatron/segment_dataset.py
 modelbest_sdk/dataset/sampler/__init__.py
 modelbest_sdk/dataset/sampler/sampler.py
+modelbest_sdk/dataset/sampler/weighted_megatron_sampler.py
 modelbest_sdk/dataset/sampler/weighted_sampler.py
 modelbest_sdk/dataset/thrift_wrapper/__init__.py
 modelbest_sdk/dataset/thrift_wrapper/base_doc.py
 modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
 modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
 modelbest_sdk/dataset/thrift_wrapper/utils.py
 modelbest_sdk/file_format/__init__.py
```

### Comparing `modelbest_sdk-0.1.6/setup.py` & `modelbest_sdk-0.1.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modelbest_sdk',
-    version='0.1.6',
+    version='0.1.8.4',
     author='HankyZhao',
     author_email='zhq980115@gmail.com',
     description='Everything about modelbest data include data format mbtable, dataset, dataloader, and tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.8',
 )
```

### Comparing `modelbest_sdk-0.1.6/test/test_base.py` & `modelbest_sdk-0.1.8.4/test/test_base.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/test/test_batched_dataset.py` & `modelbest_sdk-0.1.8.4/test/test_batched_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/test/test_checkpoint.py` & `modelbest_sdk-0.1.8.4/test/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/test/test_dataset_context.py` & `modelbest_sdk-0.1.8.4/test/test_dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/test/test_mbtable.py` & `modelbest_sdk-0.1.8.4/test/test_mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.6/test/test_mbtable_partition.py` & `modelbest_sdk-0.1.8.4/test/test_mbtable_partition.py`

 * *Files identical despite different names*

