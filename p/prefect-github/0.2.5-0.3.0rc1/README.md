# Comparing `tmp/prefect_github-0.2.5.tar.gz` & `tmp/prefect_github-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_github-0.2.5.tar", last modified: Thu May 16 20:58:38 2024, max compression
+gzip compressed data, was "prefect_github-0.3.0rc1.tar", last modified: Fri May 31 20:49:42 2024, max compression
```

## Comparing `prefect_github-0.2.5.tar` & `prefect_github-0.3.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:26.000000 prefect_github-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:26.000000 prefect_github-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 20:58:38.732838 prefect_github-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-16 20:58:26.000000 prefect_github-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.720838 prefect_github-0.2.5/prefect_github/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.716838 prefect_github-0.2.5/prefect_github/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.720838 prefect_github-0.2.5/prefect_github/configs/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_comment.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_pull_request_review.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/add_star.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/close_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/close_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/create_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/create_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/remove_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/remove_star.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/mutation/request_reviews.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.724838 prefect_github-0.2.5/prefect_github/configs/query/
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/organization.json
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/repository_owner.json
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/user.json
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/configs/query/viewer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)    64980 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)   108596 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/repository_owner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.728838 prefect_github-0.2.5/prefect_github/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  4561834 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/graphql_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)  1066892 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/schemas/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    77111 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    73099 2024-05-16 20:58:26.000000 prefect_github-0.2.5/prefect_github/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/prefect_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:38.000000 prefect_github-0.2.5/prefect_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 20:58:26.000000 prefect_github-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:38.732838 prefect_github-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:38.732838 prefect_github-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:26.000000 prefect_github-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.507476 prefect_github-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 20:49:42.507476 prefect_github-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.491476 prefect_github-0.3.0rc1/prefect_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.487476 prefect_github-0.3.0rc1/prefect_github/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.495476 prefect_github-0.3.0rc1/prefect_github/configs/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/add_comment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/add_pull_request_review.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/add_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/add_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/close_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/close_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/create_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/create_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/remove_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/remove_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/mutation/request_reviews.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.495476 prefect_github-0.3.0rc1/prefect_github/configs/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/query/organization.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/query/repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/query/repository_owner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/query/user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/configs/query/viewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64980 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107600 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/repository_owner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.503476 prefect_github-0.3.0rc1/prefect_github/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4561834 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/schemas/graphql_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1066892 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/schemas/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77111 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73099 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/prefect_github/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.507476 prefect_github-0.3.0rc1/prefect_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 20:49:42.000000 prefect_github-0.3.0rc1/prefect_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:42.507476 prefect_github-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.503476 prefect_github-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 20:49:30.000000 prefect_github-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_github-0.2.5/LICENSE` & `prefect_github-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/PKG-INFO` & `prefect_github-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations interacting with GitHub
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-github
- 
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
@@ -52,15 +50,15 @@
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_github-0.2.5/README.md` & `prefect_github-0.3.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # prefect-github
- 
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
@@ -13,15 +13,15 @@
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/add_pull_request_review.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/add_pull_request_review.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/close_issue.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/close_issue.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/close_pull_request.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/close_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/create_issue.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/create_issue.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/create_pull_request.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/create_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/mutation/request_reviews.json` & `prefect_github-0.3.0rc1/prefect_github/configs/mutation/request_reviews.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/query/organization.json` & `prefect_github-0.3.0rc1/prefect_github/configs/query/organization.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/query/repository.json` & `prefect_github-0.3.0rc1/prefect_github/configs/query/repository.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/query/repository_owner.json` & `prefect_github-0.3.0rc1/prefect_github/configs/query/repository_owner.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/query/user.json` & `prefect_github-0.3.0rc1/prefect_github/configs/query/user.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/configs/query/viewer.json` & `prefect_github-0.3.0rc1/prefect_github/configs/query/viewer.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/credentials.py` & `prefect_github-0.3.0rc1/prefect_github/credentials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 """Credential classes used to perform authenticated interactions with GitHub"""
 
-import warnings
 
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.blocks.abstract import CredentialsBlock
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr
-else:
-    from pydantic import Field, SecretStr
+from typing import Optional
 
+from pydantic import Field, SecretStr
 from sgqlc.endpoint.http import HTTPEndpoint
 
+from prefect.blocks.abstract import CredentialsBlock
+
 
 class GitHubCredentials(CredentialsBlock):
     """
     Block used to manage GitHub authentication.
 
     Attributes:
         token: the token to authenticate into GitHub.
@@ -29,15 +24,15 @@
         ```
     """
 
     _block_type_name = "GitHub Credentials"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/41971cfecfea5f79ff334164f06ecb34d1038dd4-250x250.png"  # noqa
     _documentation_url = "https://prefecthq.github.io/prefect-github/credentials/#prefect_github.credentials.GitHubCredentials"  # noqa
 
-    token: SecretStr = Field(
+    token: Optional[SecretStr] = Field(
         default=None, description="A GitHub personal access token (PAT)."
     )
 
     def get_client(self) -> HTTPEndpoint:
         """
         Gets an authenticated GitHub GraphQL HTTPEndpoint client.
 
@@ -59,37 +54,7 @@
         else:
             base_headers = None
 
         endpoint = HTTPEndpoint(
             "https://api.github.com/graphql", base_headers=base_headers
         )
         return endpoint
-
-    def get_endpoint(self) -> HTTPEndpoint:
-        """
-        Gets an authenticated GitHub GraphQL HTTPEndpoint.
-
-        Returns:
-            An authenticated GitHub GraphQL HTTPEndpoint
-
-        Example:
-            Gets an authenticated GitHub GraphQL HTTPEndpoint.
-            ```python
-            from prefect import flow
-            from prefect_github import GitHubCredentials
-
-            @flow
-            def example_get_endpoint_flow():
-                token = "token_xxxxxxx"
-                github_credentials = GitHubCredentials(token=token)
-                endpoint = github_credentials.get_endpoint()
-                return endpoint
-
-            example_get_endpoint_flow()
-            ```
-        """
-        warnings.warn(
-            "`get_endpoint` is deprecated and will be removed March 31st, 2023, "
-            "use `get_client` instead.",
-            DeprecationWarning,
-        )
-        return self.get_client()
```

### Comparing `prefect_github-0.2.5/prefect_github/graphql.py` & `prefect_github-0.3.0rc1/prefect_github/graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pprint import pformat
 from typing import Any, Dict, Iterable, List, Tuple, Union
 
 from anyio import to_thread
 from sgqlc.operation import Operation, Selection
 
 from prefect import task
+from prefect.utilities.asyncutils import sync_compatible
 from prefect_github import GitHubCredentials
 from prefect_github.utils import camel_to_snake_case
 
 
 async def _execute_graphql_op(
     op: Union[Operation, str],
     github_credentials: GitHubCredentials,
@@ -57,14 +58,15 @@
         op_selection.__fields__(*return_fields)
     except KeyError:  # nested under node
         op_selection.nodes().__fields__(*return_fields)
     return op_selection
 
 
 @task
+@sync_compatible
 async def execute_graphql(
     op: Union[Operation, str],
     github_credentials: GitHubCredentials,
     error_key: str = "errors",
     **vars,
 ) -> Dict[str, Any]:
     # NOTE: Maintainers can update these examples to match their collection!
```

### Comparing `prefect_github-0.2.5/prefect_github/mutations.py` & `prefect_github-0.3.0rc1/prefect_github/mutations.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/organization.py` & `prefect_github-0.3.0rc1/prefect_github/organization.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/repository.py` & `prefect_github-0.3.0rc1/prefect_github/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,37 +5,29 @@
 
 # This module was auto-generated using prefect-collection-generator so
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 import io
 import shlex
+import shutil
 from datetime import datetime
-from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 from urllib.parse import urlparse, urlunparse
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
+from sgqlc.operation import Operation
 
 from prefect import task
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
-from sgqlc.operation import Operation
-
 from prefect_github import GitHubCredentials
-from prefect_github.exceptions import InvalidRepositoryURLError
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_path = Path(__file__).parent.resolve() / "configs" / "query" / "repository.json"
 return_fields_defaults = initialize_return_fields_defaults(config_path)
 
@@ -62,31 +54,14 @@
         description="An optional reference to pin to; can be a branch name or tag.",
     )
     credentials: Optional[GitHubCredentials] = Field(
         default=None,
         description="An optional GitHubCredentials block for using private GitHub repos.",  # noqa: E501
     )
 
-    @validator("credentials")
-    def _ensure_credentials_go_with_https(cls, v: str, values: dict):
-        """Ensure that credentials are not provided with 'SSH' formatted GitHub URLs."""
-        if v is not None:
-            if urlparse(values["repository_url"]).scheme != "https":
-                raise InvalidRepositoryURLError(
-                    (
-                        "Crendentials can only be used with GitHub repositories "
-                        "using the 'HTTPS' format. You must either remove the "
-                        "credential if you wish to use the 'SSH' format and are not "
-                        "using a private repository, or you must change the repository "
-                        "url to the 'HTTPS' format. "
-                    )
-                )
-
-        return v
-
     def _create_repo_url(self) -> str:
         """Format the URL provided to the `git clone` command.
 
         For private repos: https://<oauth-key>@github.com/<username>/<repo>.git
         All other repos should be the same as `self.repository`.
         """
         url_components = urlparse(self.repository_url)
@@ -156,15 +131,17 @@
                 err_stream.seek(0)
                 raise RuntimeError(f"Failed to pull from remote:\n {err_stream.read()}")
 
             content_source, content_destination = self._get_paths(
                 dst_dir=local_path, src_dir=tmp_path_str, sub_directory=from_path
             )
 
-            copy_tree(src=content_source, dst=content_destination)
+            shutil.copytree(
+                src=content_source, dst=content_destination, dirs_exist_ok=True
+            )
 
 
 @task
 async def query_repository(  # noqa
     owner: str,
     name: str,
     github_credentials: GitHubCredentials,
```

### Comparing `prefect_github-0.2.5/prefect_github/repository_owner.py` & `prefect_github-0.3.0rc1/prefect_github/repository_owner.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/schemas/graphql_schema.json` & `prefect_github-0.3.0rc1/prefect_github/schemas/graphql_schema.json`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/schemas/graphql_schema.py` & `prefect_github-0.3.0rc1/prefect_github/schemas/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/user.py` & `prefect_github-0.3.0rc1/prefect_github/user.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/utils.py` & `prefect_github-0.3.0rc1/prefect_github/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github/viewer.py` & `prefect_github-0.3.0rc1/prefect_github/viewer.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/prefect_github.egg-info/PKG-INFO` & `prefect_github-0.3.0rc1/prefect_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations interacting with GitHub
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-github
- 
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
@@ -52,15 +50,15 @@
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_github-0.2.5/prefect_github.egg-info/SOURCES.txt` & `prefect_github-0.3.0rc1/prefect_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/pyproject.toml` & `prefect_github-0.3.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-github"
-dependencies = ["sgqlc>=15.0", "prefect>=2.13.5, < 3.0.0"]
+dependencies = [
+  "sgqlc>=15.0",
+  "prefect>=3.0.0rc1",
+]
 dynamic = ["version"]
 description = "Prefect integrations interacting with GitHub"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
 
@@ -30,15 +32,14 @@
 dev = [
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pillow",
   "pre-commit",
   "pytest-asyncio",
   "pytest",
   "pytest-xdist",
 ]
@@ -48,15 +49,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_github = "prefect_github"
 
 [tool.setuptools_scm]
 version_file = "prefect_github/_version.py"
 root = "../../.."
-tag_regex = "^prefect-github-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-github-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-github-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_github/_version.py", "tests"]
```

### Comparing `prefect_github-0.2.5/tests/test_graphql.py` & `prefect_github-0.3.0rc1/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `prefect_github-0.2.5/tests/test_repository.py` & `prefect_github-0.3.0rc1/tests/test_repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Tuple
 
-import pytest
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.testing.utilities import AsyncMock
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1.error_wrappers import ValidationError
-else:
-    from pydantic.error_wrappers import ValidationError
-
 import prefect_github
+import pytest
 from prefect_github import GitHubCredentials
 from prefect_github.repository import GitHubRepository
 
+from prefect.testing.utilities import AsyncMock
+
 
 class TestGitHubRepository:
     async def test_subprocess_errors_are_surfaced(self):
         """Ensure that errors from GitHub are being surfaced to users."""
         g = GitHubRepository(repository_url="incorrect-url-scheme")
         with pytest.raises(
             RuntimeError,
@@ -76,36 +69,14 @@
         await g.get_directory()
         assert mock.await_count == 1
         assert (
             "git clone https://XYZ@github.com/PrefectHQ/prefect.git --depth 1"
             in " ".join(mock.await_args[0][0])
         )
 
-    async def test_ssh_fails_with_credential(self, monkeypatch):
-        """Ensure that credentials cannot be passed in if the URL is not in the HTTPS
-        format.
-        """
-
-        class p:
-            returncode = 0
-
-        mock = AsyncMock(return_value=p())
-        monkeypatch.setattr(prefect_github.repository, "run_process", mock)
-        credential = GitHubCredentials(token="XYZ")
-        error_msg = (
-            "Crendentials can only be used with GitHub repositories using the 'HTTPS' format"  # noqa
-            ".*"
-            "(type=value_error.invalidrepositoryurl)"
-        )
-        with pytest.raises(ValidationError, match=error_msg):
-            GitHubRepository(
-                repository_url="git@github.com:PrefectHQ/prefect.git",
-                credentials=credential,
-            )
-
     def setup_test_directory(
         self, tmp_src: str, sub_dir: str = "puppy"
     ) -> Tuple[str, str]:
         """Add files and directories to a temporary directory. Returns a tuple with the
         expected parent-level contents and the expected child-level contents.
         """
         # add file to tmp_src
```

### Comparing `prefect_github-0.2.5/tests/test_utils.py` & `prefect_github-0.3.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

