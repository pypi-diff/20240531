# Comparing `tmp/nopecha-1.0.9.tar.gz` & `tmp/nopecha-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopecha-1.0.9.tar", last modified: Wed May  8 13:16:41 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nopecha-1.0.9.tar` & `nopecha-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.132273 nopecha-1.0.9/
--rw-r--r--   0 jae       (1000) jae       (1000)     1064 2023-10-25 05:59:14.000000 nopecha-1.0.9/LICENSE
--rw-r--r--   0 jae       (1000) jae       (1000)     2465 2024-05-08 13:16:41.132273 nopecha-1.0.9/PKG-INFO
--rw-r--r--   0 jae       (1000) jae       (1000)     1921 2023-10-25 05:59:14.000000 nopecha-1.0.9/README.md
--rw-r--r--   0 jae       (1000) jae       (1000)      610 2024-05-08 12:19:04.000000 nopecha-1.0.9/pyproject.toml
--rw-r--r--   0 jae       (1000) jae       (1000)       38 2024-05-08 13:16:41.135606 nopecha-1.0.9/setup.cfg
-drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.115606 nopecha-1.0.9/src/
-drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.125606 nopecha-1.0.9/src/nopecha/
--rw-r--r--   0 jae       (1000) jae       (1000)      814 2024-05-08 11:19:46.000000 nopecha-1.0.9/src/nopecha/__init__.py
--rw-r--r--   0 jae       (1000) jae       (1000)     6128 2024-05-08 11:19:15.000000 nopecha-1.0.9/src/nopecha/api_requestor.py
--rw-r--r--   0 jae       (1000) jae       (1000)      962 2024-05-08 11:19:59.000000 nopecha-1.0.9/src/nopecha/error.py
--rw-r--r--   0 jae       (1000) jae       (1000)     1857 2024-05-08 12:19:35.000000 nopecha-1.0.9/src/nopecha/nopecha.py
--rw-r--r--   0 jae       (1000) jae       (1000)     3210 2023-10-25 05:59:14.000000 nopecha-1.0.9/src/nopecha/nopecha_object.py
-drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.132273 nopecha-1.0.9/src/nopecha.egg-info/
--rw-r--r--   0 jae       (1000) jae       (1000)     2465 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/PKG-INFO
--rw-r--r--   0 jae       (1000) jae       (1000)      299 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/SOURCES.txt
--rw-r--r--   0 jae       (1000) jae       (1000)        1 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/dependency_links.txt
--rw-r--r--   0 jae       (1000) jae       (1000)        8 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/top_level.txt
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/__init__.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/_v1_compat.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/__init__.py
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/_base.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/_key.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/_throttle.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/_validate.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/aiohttp.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/httpx.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/requests.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/types.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/api/urllib.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/extension/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/extension/_adapter.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 nopecha-2.0.0/src/nopecha/extension/extension.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 nopecha-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 nopecha-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 nopecha-2.0.0/README.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 nopecha-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 nopecha-2.0.0/PKG-INFO
```

### Comparing `nopecha-1.0.9/LICENSE` & `nopecha-2.0.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 NopeCHA
+Copyright (c) 2022-present NopeCHA
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

