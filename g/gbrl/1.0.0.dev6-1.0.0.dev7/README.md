# Comparing `tmp/gbrl-1.0.0.dev6.tar.gz` & `tmp/gbrl-1.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbrl-1.0.0.dev6.tar", last modified: Sat May 18 07:21:02 2024, max compression
+gzip compressed data, was "gbrl-1.0.0.dev7.tar", last modified: Fri May 31 10:36:39 2024, max compression
```

## Comparing `gbrl-1.0.0.dev6.tar` & `gbrl-1.0.0.dev7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:46.051709 gbrl-1.0.0.dev6/
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     4044 2024-04-09 07:20:14.000000 gbrl-1.0.0.dev6/LICENSE
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      104 2024-04-01 11:37:53.000000 gbrl-1.0.0.dev6/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nobody   (65534)     4323 2024-05-18 07:20:46.049329 gbrl-1.0.0.dev6/PKG-INFO
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3562 2024-05-06 11:44:24.000000 gbrl-1.0.0.dev6/README.md
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:45.881607 gbrl-1.0.0.dev6/gbrl/
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      248 2024-05-02 14:08:30.000000 gbrl-1.0.0.dev6/gbrl/__init__.py
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    29081 2024-05-06 13:05:58.000000 gbrl-1.0.0.dev6/gbrl/ac_gbrl.py
--rw-r--r--   0 nobody   (65534) nobody   (65534)      173 2024-05-02 14:09:17.000000 gbrl-1.0.0.dev6/gbrl/config.py
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    21293 2024-05-02 14:44:24.000000 gbrl-1.0.0.dev6/gbrl/gbrl_wrapper.py
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     8903 2024-05-02 14:04:13.000000 gbrl-1.0.0.dev6/gbrl/gbt.py
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:45.850375 gbrl-1.0.0.dev6/gbrl/src/
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:45.987495 gbrl-1.0.0.dev6/gbrl/src/cpp/
--rw-r--r--   0 nobody   (65534) nobody   (65534)      170 2024-04-22 09:24:19.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/config.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    26703 2024-05-06 11:39:40.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/fitter.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1392 2024-04-18 15:24:37.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/fitter.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    42957 2024-05-06 11:39:25.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3027 2024-04-22 09:43:15.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    14516 2024-04-18 15:27:13.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl_binding.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2562 2024-05-06 11:29:30.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/loss.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      374 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/loss.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    14885 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/main.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    21067 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/math_ops.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3232 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/math_ops.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    22323 2024-04-04 16:30:35.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/node.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2196 2024-04-04 16:30:27.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/node.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     9950 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/optimizer.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2647 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/optimizer.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    11702 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/predictor.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1347 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/predictor.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3332 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/scheduler.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1717 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/scheduler.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    13138 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/split_candidate_generator.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1686 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/split_candidate_generator.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    21579 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/types.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     4165 2024-04-22 09:43:08.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/types.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1654 2024-04-22 09:39:52.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/utils.cpp
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1371 2024-04-22 09:40:24.000000 gbrl-1.0.0.dev6/gbrl/src/cpp/utils.h
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:46.034760 gbrl-1.0.0.dev6/gbrl/src/cuda/
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    67468 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_fitter.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     8351 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_fitter.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2399 2024-05-06 11:34:13.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_loss.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      884 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_loss.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    26320 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_predictor.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3847 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_predictor.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    17805 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_preprocess.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2926 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_preprocess.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    17660 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_types.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2294 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_types.h
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      760 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_utils.cu
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)      200 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_utils.h
--rw-r--r--   0 nobody   (65534) nobody   (65534)     2256 2024-05-06 12:32:09.000000 gbrl-1.0.0.dev6/gbrl/utils.py
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:46.044429 gbrl-1.0.0.dev6/gbrl.egg-info/
--rw-r--r--   0 nobody   (65534) nobody   (65534)     4323 2024-05-18 07:20:45.000000 gbrl-1.0.0.dev6/gbrl.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nobody   (65534)     1308 2024-05-18 07:20:45.000000 gbrl-1.0.0.dev6/gbrl.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nobody   (65534)        1 2024-05-18 07:20:45.000000 gbrl-1.0.0.dev6/gbrl.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nobody   (65534)       60 2024-05-18 07:20:45.000000 gbrl-1.0.0.dev6/gbrl.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nobody   (65534)        5 2024-05-18 07:20:45.000000 gbrl-1.0.0.dev6/gbrl.egg-info/top_level.txt
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1025 2024-05-18 07:14:10.000000 gbrl-1.0.0.dev6/pyproject.toml
--rw-r--r--   0 nobody   (65534) nobody   (65534)       38 2024-05-18 07:20:46.052498 gbrl-1.0.0.dev6/setup.cfg
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)     8925 2024-05-18 05:32:58.000000 gbrl-1.0.0.dev6/setup.py
-drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-18 07:20:46.040552 gbrl-1.0.0.dev6/tests/
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    22601 2024-05-02 14:16:12.000000 gbrl-1.0.0.dev6/tests/test_gbt_multi.py
--rwxrwxrwx   0 nobody   (65534) nobody   (65534)    18336 2024-05-02 14:11:56.000000 gbrl-1.0.0.dev6/tests/test_gbt_single.py
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.739119 gbrl-1.0.0.dev7/
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     4044 2024-04-09 07:20:14.000000 gbrl-1.0.0.dev7/LICENSE
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      104 2024-04-01 11:37:53.000000 gbrl-1.0.0.dev7/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nobody   (65534)     4330 2024-05-31 10:36:19.736143 gbrl-1.0.0.dev7/PKG-INFO
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3570 2024-05-18 07:23:09.000000 gbrl-1.0.0.dev7/README.md
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.489073 gbrl-1.0.0.dev7/gbrl/
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      248 2024-05-02 14:08:30.000000 gbrl-1.0.0.dev7/gbrl/__init__.py
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    29081 2024-05-06 13:05:58.000000 gbrl-1.0.0.dev7/gbrl/ac_gbrl.py
+-rw-r--r--   0 nobody   (65534) nobody   (65534)      173 2024-05-02 14:09:17.000000 gbrl-1.0.0.dev7/gbrl/config.py
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    21850 2024-05-30 11:15:46.000000 gbrl-1.0.0.dev7/gbrl/gbrl_wrapper.py
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     9311 2024-05-30 11:16:00.000000 gbrl-1.0.0.dev7/gbrl/gbt.py
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.447131 gbrl-1.0.0.dev7/gbrl/src/
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.674129 gbrl-1.0.0.dev7/gbrl/src/cpp/
+-rw-r--r--   0 nobody   (65534) nobody   (65534)      170 2024-04-22 09:24:19.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/config.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    26703 2024-05-06 11:39:40.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/fitter.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1392 2024-04-18 15:24:37.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/fitter.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    43825 2024-05-30 11:10:33.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3111 2024-05-30 11:10:27.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    14809 2024-05-30 11:14:25.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl_binding.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2562 2024-05-06 11:29:30.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/loss.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      374 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/loss.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    14885 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/main.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    21067 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/math_ops.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3232 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/math_ops.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    22323 2024-04-04 16:30:35.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/node.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2196 2024-04-04 16:30:27.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/node.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     9950 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/optimizer.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2647 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/optimizer.h
+-rwxr-xr-x   0 nobody   (65534) nobody   (65534)    11702 2024-05-31 10:23:32.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/predictor.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1347 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/predictor.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3332 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/scheduler.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1717 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/scheduler.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    13138 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/split_candidate_generator.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1686 2024-04-01 11:37:50.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/split_candidate_generator.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    28687 2024-05-31 10:21:43.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/types.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     4366 2024-05-30 11:09:48.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/types.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1654 2024-04-22 09:39:52.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/utils.cpp
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1371 2024-04-22 09:40:24.000000 gbrl-1.0.0.dev7/gbrl/src/cpp/utils.h
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.722070 gbrl-1.0.0.dev7/gbrl/src/cuda/
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    67468 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_fitter.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     8351 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_fitter.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2399 2024-05-06 11:34:13.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_loss.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      884 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_loss.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    26320 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_predictor.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     3847 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_predictor.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    17805 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_preprocess.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2926 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_preprocess.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    17660 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_types.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     2294 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_types.h
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      760 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_utils.cu
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)      200 2024-04-01 11:37:49.000000 gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_utils.h
+-rw-r--r--   0 nobody   (65534) nobody   (65534)     2256 2024-05-06 12:32:09.000000 gbrl-1.0.0.dev7/gbrl/utils.py
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.732114 gbrl-1.0.0.dev7/gbrl.egg-info/
+-rw-r--r--   0 nobody   (65534) nobody   (65534)     4330 2024-05-31 10:36:19.000000 gbrl-1.0.0.dev7/gbrl.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nobody   (65534)     1308 2024-05-31 10:36:19.000000 gbrl-1.0.0.dev7/gbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nobody   (65534)        1 2024-05-31 10:36:19.000000 gbrl-1.0.0.dev7/gbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nobody   (65534)       60 2024-05-31 10:36:19.000000 gbrl-1.0.0.dev7/gbrl.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nobody   (65534)        5 2024-05-31 10:36:19.000000 gbrl-1.0.0.dev7/gbrl.egg-info/top_level.txt
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     1025 2024-05-31 10:24:28.000000 gbrl-1.0.0.dev7/pyproject.toml
+-rw-r--r--   0 nobody   (65534) nobody   (65534)       38 2024-05-31 10:36:19.740076 gbrl-1.0.0.dev7/setup.cfg
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)     8925 2024-05-18 05:32:58.000000 gbrl-1.0.0.dev7/setup.py
+drwxr-xr-x   0 nobody   (65534) nobody   (65534)        0 2024-05-31 10:36:19.729073 gbrl-1.0.0.dev7/tests/
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    22601 2024-05-02 14:16:12.000000 gbrl-1.0.0.dev7/tests/test_gbt_multi.py
+-rwxrwxrwx   0 nobody   (65534) nobody   (65534)    18336 2024-05-02 14:11:56.000000 gbrl-1.0.0.dev7/tests/test_gbt_single.py
```

### Comparing `gbrl-1.0.0.dev6/LICENSE` & `gbrl-1.0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/PKG-INFO` & `gbrl-1.0.0.dev7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbrl
-Version: 1.0.0.dev6
+Version: 1.0.0.dev7
 Summary: Gradient Boosted Trees for RL
 Author-email: Benjamin Fuhrer <bfuhrer@nvidia.com>, Chen Tessler <ctessler@nvidia.com>, Gal Dalal <galal@nvidia.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
@@ -29,18 +29,19 @@
 - Hardware Acceleration: GBRL leverages CUDA for hardware-accelerated computation, ensuring efficiency and speed.
 - Seamless Integration: GBRL is designed for easy integration with popular RL libraries, making it readily accessible for practitioners.
 
 
 ## Getting started
 
 ### Dependencies 
+#### MAC OS 
+```
 llvm
 openmp
-
-#### MAC OS 
+```
 
 Make sure to run:
 ```
 brew install libomp
 brew install llvm
  ```
```

### Comparing `gbrl-1.0.0.dev6/README.md` & `gbrl-1.0.0.dev7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 - Hardware Acceleration: GBRL leverages CUDA for hardware-accelerated computation, ensuring efficiency and speed.
 - Seamless Integration: GBRL is designed for easy integration with popular RL libraries, making it readily accessible for practitioners.
 
 
 ## Getting started
 
 ### Dependencies 
+#### MAC OS 
+```
 llvm
 openmp
-
-#### MAC OS 
+```
 
 Make sure to run:
 ```
 brew install libomp
 brew install llvm
  ```
```

### Comparing `gbrl-1.0.0.dev6/gbrl/ac_gbrl.py` & `gbrl-1.0.0.dev7/gbrl/ac_gbrl.py`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/gbrl_wrapper.py` & `gbrl-1.0.0.dev7/gbrl/gbrl_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,24 @@
     def save(self, filename: str) -> None:
         filename = filename.rstrip('.')
         filename += '.gbrl_model'
         assert self.model is not None, "Can't save non-existent model!"
         status = self.model.save(filename)
         assert status == 0, "Failed to save model"
 
+    def export(self, filename: str, modelname: str = None) -> None:
+        # exports model to C
+        filename = filename.rstrip('.')
+        filename += '.h'
+        assert self.model is not None, "Can't export non-existent model!"
+        if modelname is None:
+            modelname = ""
+        status = self.model.export(filename, modelname)
+        assert status == 0, "Failed to export model"
+
     @classmethod
     def load(cls, filename: str) -> "GBTWrapper":
         filename = filename.rstrip('.')
         if '.gbrl_model' not in filename:
             filename += '.gbrl_model'
         assert os.path.isfile(filename), "filename doesn't exist!"
         print("Loading model")
@@ -309,14 +319,18 @@
         self.policy_model.reset()
         self.value_model.reset()
 
     def save(self, filename: str) -> None:
         self.policy_model.save(filename + '_policy')
         self.value_model.save(filename + '_value')
 
+    def export(self, filename: str) -> None:
+        self.policy_model.export(filename + '_policy')
+        self.value_model.export(filename + '_value')
+
     @classmethod
     def load(cls, filename: str) -> "SeparateActorCriticWrapper":
         instance = cls.__new__(cls)
         instance.policy_model = GBTWrapper.load(filename + '_policy')
         instance.value_model = GBTWrapper.load(filename + '_value')
         instance.tree_struct = instance.policy_model.tree_struct
         instance.total_iterations = instance.policy_model.iteration + instance.value_model.iteration
```

### Comparing `gbrl-1.0.0.dev6/gbrl/gbt.py` & `gbrl-1.0.0.dev7/gbrl/gbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,17 +168,32 @@
 
         Returns:
             int: number of trees in the ensemble
         """
         return self._model.get_num_trees()
         
 
-    def save_model(self, save_path: str=None) -> None:
+    def save_model(self, save_path: str) -> None:
+        """
+        Saves model to file
+
+        Args:
+            filename (str): Absolute path and name of save filename.
+        """
         self._model.save(save_path) 
 
+    def export_model(self, filename: str, modelname: str = None) -> None:
+        """
+        Exports model as a C-header file
+
+        Args:
+            filename (str): Absolute path and name of exported filename.
+        """
+        self._model.export(filename, modelname) 
+
     @classmethod
     def load_model(cls, load_name: str):
         instance = cls.__new__(cls)
         instance._model = GBTWrapper.load(load_name)
         instance.optimizer =  instance._model.optimizer
         instance.output_dim = instance._model.output_dim
         instance.verbose = instance._model.verbose
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/fitter.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/fitter.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/fitter.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/fitter.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -678,14 +678,36 @@
         delete[] training_cat_obs;
         delete[] training_targets;
     }
 
     return full_loss;   
 }
 
+int GBRL::exportModel(const std::string& filename, const std::string& modelname){
+    std::ofstream header_file(filename, std::ios::binary);
+    if (!header_file.is_open() || header_file.fail()) {
+        std::cerr << "Error opening file: " << filename << std::endl;
+        throw std::runtime_error("File opening error");
+        return -1;
+    }
+    if (this->metadata->grow_policy != OBLIVIOUS) {
+        std::cerr << "Export is supported only for Oblivious trees." << std::endl;
+        header_file.close();
+        return -1;
+    }
+    export_ensemble_data(header_file, modelname, this->edata, this->metadata, this->device, this->opts);
+    if (!header_file.good()) {
+        std::cerr << "Error occurred at writing time." << std::endl;
+        throw std::runtime_error("Writing to file error");
+        return -1;
+    }
+
+    header_file.close();
+    return 0;
+}
 
 int GBRL::saveToFile(const std::string& filename){
     std::ofstream file(filename, std::ios::binary);
     if (!file.is_open() || file.fail()) {
         std::cerr << "Error opening file: " << filename << std::endl;
         throw std::runtime_error("File opening error");
         return -1;
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl.h`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         GBRL(const std::string& filename);
         GBRL(GBRL& other);
         ~GBRL();
         static bool cuda_available();
         void to_device(deviceType device);
         std::string get_device();
         int saveToFile(const std::string& filename);
+        int exportModel(const std::string& filename, const std::string& modelname);
         int loadFromFile(const std::string& filename);
 
         void step(const float *obs, const char *categorical_obs, float *grads, const int n_samples, const int n_num_features, const int n_cat_features);
 #ifdef USE_CUDA
         void _step_gpu(dataSet *dataset);
         float _fit_gpu(dataSet *datasett, float *targets, const int n_iterations);
 #endif
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/gbrl_binding.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/gbrl_binding.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,18 @@
         self.predict(obs_ptr, cat_obs_ptr, preds_ptr, n_samples, n_num_features, n_cat_features, start_tree_idx, stop_tree_idx);  
     }, py::arg("obs"), py::arg("categorical_obs"), py::arg("start_preds"), py::arg("start_tree_idx")=0, py::arg("stop_tree_idx")=0, "Predict using the model");
         // saveToFile method
     gbrl.def("save", [](GBRL &self, const std::string& filename) -> int {
         py::gil_scoped_release release; 
         return self.saveToFile(filename); 
     }, "Save the model to a file");
+    gbrl.def("export", [](GBRL &self, const std::string& filename, const std::string& modelname) -> int {
+        py::gil_scoped_release release; 
+        return self.exportModel(filename, modelname); 
+    }, py::arg("filename"), py::arg("modelname") = "", "Export model as a C-header file");
     gbrl.def("get_scheduler_lrs", [](GBRL &self) ->  std::tuple<float, float> {
         py::gil_scoped_release release; 
         return self.get_scheduler_lrs(); 
     }, "Return current scheduler lrs");  
     gbrl.def("get_num_trees", [](GBRL &self) ->  int {
         py::gil_scoped_release release; 
         return self.get_num_trees();
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/loss.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/loss.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/main.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/math_ops.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/math_ops.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/math_ops.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/math_ops.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/node.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/node.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/node.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/node.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/optimizer.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/optimizer.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/optimizer.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/optimizer.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/predictor.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/predictor.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/predictor.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/predictor.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/scheduler.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/scheduler.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/scheduler.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/scheduler.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/split_candidate_generator.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/split_candidate_generator.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/split_candidate_generator.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/split_candidate_generator.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/types.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/types.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <string>
 #include <cstring>
 #include <iostream>
 #include <fstream>
 #include <stdexcept>
 
 #include "types.h"
+#include "optimizer.h"
 #ifdef USE_CUDA
 #include "cuda_types.h"
 #endif
 
 
 scoreFunc stringToScoreFunc(std::string str) {
     if (str == "L2" || str == "l2") return scoreFunc::L2;
@@ -278,14 +279,169 @@
     delete[] edata->feature_values;
     delete[] edata->is_numerics;
     delete[] edata->categorical_values;
     delete[] edata->inequality_directions; 
     delete edata;
 }
 
+void export_ensemble_data(std::ofstream& header_file, const std::string& model_name, ensembleData *edata, ensembleMetaData *metadata, deviceType device, std::vector<Optimizer*> opts)
+{
+    if (!header_file.is_open() || header_file.fail()) {
+        std::cerr << "Error file is not open for writing: " << std::endl;
+        throw std::runtime_error("Error opening header_file");
+    }
+    ensembleData *edata_cpu = nullptr;
+#ifdef USE_CUDA
+    if (device == gpu){
+        edata_cpu = ensemble_data_copy_gpu_cpu(metadata, edata);
+    }
+#endif 
+    if (device == cpu)
+        edata_cpu = edata;
+    
+    int binary_splits = 0;
+    for (int i  = 0; i < metadata->n_trees; ++i){
+        binary_splits += edata_cpu->depths[i];
+    }
+
+    for (size_t opt_idx = 0; opt_idx < opts.size(); ++opt_idx){
+        optimizerAlgo algo = opts[opt_idx]->getAlgo();
+        if (algo != SGD){
+            std::cerr << "Error. Can only export SGD optimizers" << std::endl;
+            return;
+        }
+    }
+
+    header_file << "#ifndef GBRL_MODEL_H\n";
+    header_file << "#define GBRL_MODEL_H\n\n";
+
+    
+    header_file << "/*\n";
+
+    if (!model_name.empty()) {
+           header_file << "###########################\n";
+        header_file << "model_name: " << model_name << "\n";
+    }
+    header_file << "###########################\n";
+    header_file << "n_leaves: " << metadata->n_leaves << ", ";
+    header_file << "n_trees: " << metadata->n_trees << ", ";
+    header_file << "max_trees: " << metadata->max_trees << ", ";
+    header_file << "max_leaves: " << metadata->max_leaves << ", ";
+    header_file << "max_trees_batch: " << metadata->max_trees_batch << ", ";
+    header_file << "max_leaves_batch: " << metadata->max_leaves_batch << ", ";
+    header_file << "output_dim: " << metadata->output_dim << ", ";
+    header_file << "policy_dim: " << metadata->policy_dim;
+    header_file << "\nmax_depth: " << metadata->max_depth << ", ";
+    header_file << "min_data_in_leaf: " << metadata->min_data_in_leaf << ", ";
+    header_file << "n_bins: " << metadata->n_bins << ", ";
+    header_file << "par_th: " << metadata->par_th << ", ";
+    header_file << "cv_beta: " << metadata->cv_beta << ", ";
+    header_file << "verbose: " << metadata->verbose << ", ";
+    header_file << "batch_size: " << metadata->batch_size << ", ";
+    header_file << "use_cv: " << metadata->use_cv;
+    header_file << "\nsplit_score_func: " << scoreFuncToString(metadata->split_score_func) << ", ";
+    header_file << "generator_type: " << generatorTypeToString(metadata->generator_type) << ", ";
+    header_file << "grow_policy: " << growPolicyToString(metadata->grow_policy) << ", ";
+    header_file << "n_num_features: " << metadata->n_num_features << ", ";
+    header_file << "n_cat_features: " << metadata->n_cat_features << ", ";
+    header_file << "iteration: " << metadata->iteration;
+    header_file << "\n*/\n";
+
+    header_file << "#define N_TREES " << metadata->n_trees << "\n";
+    header_file << "#define N_LEAVES " << metadata->n_leaves << "\n";
+    header_file << "#define BINARY_FEATURES " << binary_splits << "\n";
+    header_file << "#define N_OUTPUTS " << metadata->output_dim << "\n";
+    header_file << "#define N_FEATURES " << metadata->n_num_features  << "\n\n";
+
+    header_file << "static inline void gbrl_predict(float *results, const float *features){\n\n";
+    header_file << "\tunsigned int j, tree_idx, depth, current_depth, idx, leaf_ptr, cond_ptr;\n";
+    header_file << "\t/* Model data */\n";
+    header_file << "\tconst unsigned int depths[N_TREES] = {";
+    for (int i  = 0; i < metadata->n_trees; ++i){
+        header_file << edata_cpu->depths[i];
+        if (i < metadata->n_trees - 1)
+            header_file << ", ";
+    }
+    header_file << "};\n";
+    header_file << "\tconst float bias[N_OUTPUTS] = {";
+    for (int i  = 0; i < metadata->output_dim; ++i){
+        header_file << edata_cpu->bias[i];
+        if (i < metadata->output_dim - 1)
+            header_file << ", ";
+    }
+    header_file << "};\n";
+    header_file << "\tconst unsigned int feature_indices[BINARY_FEATURES] = {";
+    for (int i  = 0; i < binary_splits; ++i){
+        header_file << edata_cpu->feature_indices[i];
+        if (i < binary_splits - 1)
+            header_file << ", ";
+    }
+    header_file << "};\n";
+    header_file << "\tconst float feature_values[BINARY_FEATURES] = {";
+    for (int i  = 0; i < binary_splits; ++i){
+        header_file << edata_cpu->feature_values[i];
+        if (i < binary_splits - 1)
+            header_file << ", ";
+    }
+    header_file << "};\n";
+    header_file << "\tconst float leaf_values[N_LEAVES*N_OUTPUTS] = {";
+    int tree_idx = 0;
+    int limit_leaf_idx = edata_cpu->tree_indices[tree_idx];
+    float value;
+    for (int i  = 0; i < metadata->n_leaves; ++i){
+        if (i > limit_leaf_idx){
+            tree_idx += 1;
+            limit_leaf_idx = edata_cpu->tree_indices[tree_idx];
+        }
+        int value_idx = i*metadata->output_dim;
+        for (size_t opt_idx = 0; opt_idx < opts.size(); ++opt_idx){
+            for (int j=opts[opt_idx]->start_idx; j < opts[opt_idx]->end_idx; ++j){
+                value = -edata_cpu->values[value_idx + j] * opts[opt_idx]->scheduler->get_lr(tree_idx);
+                header_file << value;
+                if ((i < metadata->n_leaves - 1) || (j < metadata->output_dim - 1  && i == metadata->n_leaves - 1))
+                    header_file << ", ";
+            }
+        }
+    }
+    header_file << "};\n";
+    // header_file << "\tconst unsigned int tree_indices[N_TREES] = {";
+    // for (int i  = 0; i < metadata->n_trees; ++i){
+    //     header_file << edata_cpu->tree_indices[i];
+    //     if (i < metadata->n_trees - 1)
+    //         header_file << ", ";
+    // }
+    // header_file << "};\n";
+    header_file << "\tleaf_ptr = 0;\n";
+    header_file << "\tcond_ptr = 0;\n";
+    header_file << "\tunsigned char pass;\n";
+    header_file << "\tfor (tree_idx = 0; tree_idx < N_TREES; ++tree_idx)\n";
+    header_file << "\t{\n";
+    header_file << "\t\tcurrent_depth = depths[tree_idx];\n";
+    header_file << "\t\tidx = 0;\n";
+    header_file << "\t\tfor (depth = 0; depth < current_depth; ++depth){\n";
+    header_file << "\t\t\tpass = (unsigned char)(features[feature_indices[cond_ptr + depth]] > feature_values[cond_ptr + depth]);\n";
+    header_file << "\t\t\tidx |= (pass <<  (current_depth - 1 - depth));\n";
+    header_file << "\t\t}\n";
+    header_file << "\t\tfor (j = 0 ; j < N_OUTPUTS; j++)\n";
+    header_file << "\t\t\tresults[j] += leaf_values[(leaf_ptr + idx)*N_OUTPUTS + j];\n";
+    header_file << "\t\tleaf_ptr += (1 << current_depth);\n";
+    header_file << "\t\tcond_ptr += current_depth;\n";
+    header_file << "\t}\n";
+    header_file << "\tfor (j = 0 ; j < N_OUTPUTS; j++)\n";
+    header_file << "\t\tresults[j] += bias[j];\n";
+    header_file << "}\n";
+    header_file << "#endif\n";
+
+#ifdef USE_CUDA
+    if (device == gpu){
+        ensemble_data_dealloc(edata_cpu);
+    }
+#endif 
+}
+
 void save_ensemble_data(std::ofstream& file, ensembleData *edata, ensembleMetaData *metadata, deviceType device){
     if (!file.is_open() || file.fail()) {
         std::cerr << "Error file is not open for writing: " << std::endl;
         throw std::runtime_error("Error opening file");
     }
     ensembleData *edata_cpu = nullptr;
 #ifdef USE_CUDA
@@ -334,14 +490,20 @@
     file.write(reinterpret_cast<char*>(&check), sizeof(NULL_CHECK));
     if (edata_cpu->inequality_directions != nullptr)
         file.write(reinterpret_cast<char*>(edata_cpu->inequality_directions), metadata->max_depth * metadata->n_leaves * sizeof(bool));
     check = edata_cpu->categorical_values != nullptr ? VALID : NULL_OPT;
     file.write(reinterpret_cast<char*>(&check), sizeof(NULL_CHECK));
     if (edata_cpu->categorical_values != nullptr)
         file.write(reinterpret_cast<char*>(edata_cpu->categorical_values), metadata->max_depth * sizes * sizeof(char) * MAX_CHAR_SIZE);
+
+#ifdef USE_CUDA
+    if (device == gpu){
+        ensemble_data_dealloc(edata_cpu);
+    }
+#endif 
 }
 
 ensembleData* load_ensemble_data(std::ifstream& file, ensembleMetaData *metadata){
     if (!file.is_open() || file.fail()) {
         std::cerr << "Error file is not open for writing: " << std::endl;
         throw std::runtime_error("Error opening file");
     }
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/types.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/types.h`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #include <string>
 #include <cstdint>
 
 #define INITAL_MAX_TREES 50000 //50k
 #define TREES_BATCH  25000 // 100 K
 #define MAX_CHAR_SIZE 128
 
+class Optimizer;
 struct splitCondition {
     int feature_idx;
     float feature_value;
     bool inequality_direction;
     char *categorical_value;
 };
 
@@ -161,10 +162,11 @@
 
 ensembleMetaData* ensemble_metadata_alloc(int max_trees, int max_leaves, int max_trees_batch, int max_leaves_batch, int output_dim, int policy_dim, int max_depth, int min_data_in_leaf, int n_bins, int par_th, float cv_beta, int verbose, int batch_size, bool use_cv, scoreFunc split_score_func, generatorType generator_type, growPolicy grow_policy);
 ensembleData* ensemble_data_alloc(ensembleMetaData *metadata);
 ensembleData* ensemble_copy_data_alloc(ensembleMetaData *metadata);
 ensembleData* copy_ensemble_data(ensembleData *other_edata, ensembleMetaData *metadata);
 void ensemble_data_dealloc(ensembleData *edata);
 void save_ensemble_data(std::ofstream& file, ensembleData *edata, ensembleMetaData *metadata, deviceType device);
+void export_ensemble_data(std::ofstream& header_file, const std::string& model_name, ensembleData *edata, ensembleMetaData *metadata, deviceType device, std::vector<Optimizer*> opts);
 ensembleData* load_ensemble_data(std::ifstream& file, ensembleMetaData *metadata);
 void allocate_ensemble_memory(ensembleMetaData *metadata, ensembleData *edata);
 #endif
```

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/utils.cpp` & `gbrl-1.0.0.dev7/gbrl/src/cpp/utils.cpp`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cpp/utils.h` & `gbrl-1.0.0.dev7/gbrl/src/cpp/utils.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_fitter.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_fitter.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_fitter.h` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_fitter.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_loss.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_loss.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_loss.h` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_loss.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_predictor.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_predictor.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_predictor.h` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_predictor.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_preprocess.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_preprocess.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_preprocess.h` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_preprocess.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_types.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_types.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_types.h` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_types.h`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/src/cuda/cuda_utils.cu` & `gbrl-1.0.0.dev7/gbrl/src/cuda/cuda_utils.cu`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl/utils.py` & `gbrl-1.0.0.dev7/gbrl/utils.py`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/gbrl.egg-info/PKG-INFO` & `gbrl-1.0.0.dev7/gbrl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbrl
-Version: 1.0.0.dev6
+Version: 1.0.0.dev7
 Summary: Gradient Boosted Trees for RL
 Author-email: Benjamin Fuhrer <bfuhrer@nvidia.com>, Chen Tessler <ctessler@nvidia.com>, Gal Dalal <galal@nvidia.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
@@ -29,18 +29,19 @@
 - Hardware Acceleration: GBRL leverages CUDA for hardware-accelerated computation, ensuring efficiency and speed.
 - Seamless Integration: GBRL is designed for easy integration with popular RL libraries, making it readily accessible for practitioners.
 
 
 ## Getting started
 
 ### Dependencies 
+#### MAC OS 
+```
 llvm
 openmp
-
-#### MAC OS 
+```
 
 Make sure to run:
 ```
 brew install libomp
 brew install llvm
  ```
```

### Comparing `gbrl-1.0.0.dev6/gbrl.egg-info/SOURCES.txt` & `gbrl-1.0.0.dev7/gbrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/pyproject.toml` & `gbrl-1.0.0.dev7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "pybind11==2.11.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gbrl"
-version = "1.0.0.dev6"
+version = "1.0.0.dev7"
 description = "Gradient Boosted Trees for RL"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     {name = "Benjamin Fuhrer", email = "bfuhrer@nvidia.com"},
     {name = "Chen Tessler", email = "ctessler@nvidia.com"},
     {name = "Gal Dalal", email = "galal@nvidia.com"}
 ]
```

### Comparing `gbrl-1.0.0.dev6/setup.py` & `gbrl-1.0.0.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/tests/test_gbt_multi.py` & `gbrl-1.0.0.dev7/tests/test_gbt_multi.py`

 * *Files identical despite different names*

### Comparing `gbrl-1.0.0.dev6/tests/test_gbt_single.py` & `gbrl-1.0.0.dev7/tests/test_gbt_single.py`

 * *Files identical despite different names*

