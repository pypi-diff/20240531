# Comparing `tmp/graphene-federation-3.1.4.tar.gz` & `tmp/graphene-federation-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-federation-3.1.4.tar", last modified: Wed May 24 01:38:51 2023, max compression
+gzip compressed data, was "graphene-federation-3.1.5.tar", last modified: Fri May 31 19:18:33 2024, max compression
```

## Comparing `graphene-federation-3.1.4.tar` & `graphene-federation-3.1.5.tar`

### file list

```diff
@@ -1,48 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.943281 graphene-federation-3.1.4/graphene_federation/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/inaccessible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/provides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/shareable.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/graphene_federation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_custom_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_extend_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_inaccessible.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_key_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_provides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_provides_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_requires_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_shareable.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.943281 graphene-federation-3.1.4/graphene_federation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.772346 graphene-federation-3.1.5/graphene_federation/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.776346 graphene-federation-3.1.5/graphene_federation/apollo_versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/v2_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/apollo_versions/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/composable_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.776346 graphene-federation-3.1.5/graphene_federation/directives/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/authenticated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/extends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/inaccessible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/interface_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/provides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/requires_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/shareable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/directives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/graphene_federation/scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/federation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/federation_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/field_set_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/field_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/link_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/scalars/link_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/graphene_federation/schema_directives/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/schema_directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/schema_directives/compose_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/schema_directives/link_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/graphene_federation/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/transform/field_set_case_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/graphene_federation/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/validators/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/validators/provides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/validators/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/graphene_federation/validators/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:18:33.772346 graphene-federation-3.1.5/graphene_federation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-05-31 19:18:33.000000 graphene-federation-3.1.5/graphene_federation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-31 19:18:33.000000 graphene-federation-3.1.5/graphene_federation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:18:33.000000 graphene-federation-3.1.5/graphene_federation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 19:18:33.000000 graphene-federation-3.1.5/graphene_federation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 19:18:33.000000 graphene-federation-3.1.5/graphene_federation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 19:18:33.780346 graphene-federation-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-31 19:18:31.000000 graphene-federation-3.1.5/setup.py
```

### Comparing `graphene-federation-3.1.4/LICENSE.txt` & `graphene-federation-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.4/setup.py` & `graphene-federation-3.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import os
+
 from setuptools import find_packages, setup
 
 
 def read(*rnames):
-  return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
+    return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
+
 
-version = '3.1.4'
+version = "3.1.5"
 
 tests_require = [
     "pytest==7.1.2",
     "pytest-cov",
 ]
 
 dev_require = [
-    "black==22.3.0",
+    "black==23.12.1",
     "flake8==4.0.1",
     "mypy==0.961",
 ] + tests_require
 
 setup(
-  name='graphene-federation',
-  packages=find_packages(exclude=["tests"]),
-  version=version,
-  license='MIT',
-  description = 'Federation implementation for graphene',
-  long_description=(read('README.md')),
-  long_description_content_type='text/markdown',
-  author='Igor Kasianov',
-  author_email='super.hang.glider@gmail.com',
-  url='https://github.com/graphql-python/graphene-federation',
-  download_url=f'https://github.com/graphql-python/graphene-federation/archive/{version}.tar.gz',
-  keywords=["graphene", "graphql", "gql", "federation"],
-  install_requires=[
-    "graphene>=3.1",
-    "graphql-core>=3.1",
-  ],
-  classifiers=[
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Libraries",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-  ],
-  extras_require={
-    "test": tests_require,
-    "dev": dev_require,
-  },
+    name="graphene-federation",
+    packages=find_packages(exclude=["tests"]),
+    version=version,
+    license="MIT",
+    description="Federation implementation for graphene",
+    long_description=(read("README.md")),
+    long_description_content_type="text/markdown",
+    author="Igor Kasianov",
+    author_email="super.hang.glider@gmail.com",
+    url="https://github.com/graphql-python/graphene-federation",
+    download_url=f"https://github.com/graphql-python/graphene-federation/archive/{version}.tar.gz",
+    keywords=["graphene", "graphql", "gql", "federation"],
+    install_requires=[
+        "graphene>=3.1",
+        "graphql-core>=3.1",
+        "graphene-directives>=0.4.6",
+    ],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+    ],
+    extras_require={
+        "test": tests_require,
+        "dev": dev_require,
+    },
 )
```

