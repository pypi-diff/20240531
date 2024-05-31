# Comparing `tmp/cmflib-0.0.8.tar.gz` & `tmp/cmflib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmflib-0.0.8.tar", last modified: Fri Feb 16 17:51:44 2024, max compression
+gzip compressed data, was "cmflib-0.0.9.tar", last modified: Fri May 31 16:58:13 2024, max compression
```

## Comparing `cmflib-0.0.8.tar` & `cmflib-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/
--rw-r--r--   0 royann   (121683555) users      (100)    11356 2024-02-16 17:50:49.000000 cmflib-0.0.8/LICENSE
--rw-r--r--   0 royann   (121683555) users      (100)    10629 2024-02-16 17:51:44.000000 cmflib-0.0.8/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)    10154 2024-02-16 17:50:49.000000 cmflib-0.0.8/README.md
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/bin/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/bin/__init__.py
--rwxr-xr-x   0 royann   (121683555) users      (100)      214 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/bin/cmf
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/cli/
--rw-r--r--   0 royann   (121683555) users      (100)     1665 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cli/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)      910 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cli/command.py
--rw-r--r--   0 royann   (121683555) users      (100)     2912 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cli/parser.py
--rw-r--r--   0 royann   (121683555) users      (100)     2760 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cli/utils.py
--rw-r--r--   0 royann   (121683555) users      (100)    82694 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cmf.py
--rw-r--r--   0 royann   (121683555) users      (100)     5898 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cmf_commands_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)     6684 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cmf_merger.py
--rw-r--r--   0 royann   (121683555) users      (100)    36719 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/cmfquery.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/commands/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/commands/artifact/
--rw-r--r--   0 royann   (121683555) users      (100)     1450 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/artifact/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)    13517 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/artifact/pull.py
--rw-r--r--   0 royann   (121683555) users      (100)     1612 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/artifact/push.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/commands/init/
--rw-r--r--   0 royann   (121683555) users      (100)     1543 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     5468 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/amazonS3.py
--rw-r--r--   0 royann   (121683555) users      (100)     4669 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/local.py
--rw-r--r--   0 royann   (121683555) users      (100)     5547 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/minioS3.py
--rw-r--r--   0 royann   (121683555) users      (100)     2094 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/show.py
--rw-r--r--   0 royann   (121683555) users      (100)     5455 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/init/sshremote.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/commands/metadata/
--rw-r--r--   0 royann   (121683555) users      (100)     1509 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/metadata/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     3741 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/metadata/export.py
--rw-r--r--   0 royann   (121683555) users      (100)     4591 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/metadata/pull.py
--rw-r--r--   0 royann   (121683555) users      (100)     5249 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/commands/metadata/push.py
--rw-r--r--   0 royann   (121683555) users      (100)    15562 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/dvc_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    20186 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/graph_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    19461 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/metadata_helper.py
--rw-r--r--   0 royann   (121683555) users      (100)      807 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/mlmd_objects.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/server_interface/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/server_interface/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     1269 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/server_interface/server_interface.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/storage_backends/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/storage_backends/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     2219 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/storage_backends/amazonS3_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     1718 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/storage_backends/local_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     1779 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/storage_backends/minio_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     2229 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/storage_backends/sshremote_artifacts.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib/utils/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/utils/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     2089 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/utils/cmf_config.py
--rw-r--r--   0 royann   (121683555) users      (100)     1300 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/utils/dvc_config.py
--rw-r--r--   0 royann   (121683555) users      (100)      888 2024-02-16 17:50:49.000000 cmflib-0.0.8/cmflib/utils/helper_functions.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/
--rw-r--r--   0 royann   (121683555) users      (100)    10629 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)     1667 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/SOURCES.txt
--rw-r--r--   0 royann   (121683555) users      (100)        1 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/dependency_links.txt
--rw-r--r--   0 royann   (121683555) users      (100)      113 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/requires.txt
--rw-r--r--   0 royann   (121683555) users      (100)       14 2024-02-16 17:51:44.000000 cmflib-0.0.8/cmflib.egg-info/top_level.txt
--rw-r--r--   0 royann   (121683555) users      (100)      609 2024-02-16 17:50:49.000000 cmflib-0.0.8/pyproject.toml
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/server/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/server/app/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     8170 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/get_data.py
--rw-r--r--   0 royann   (121683555) users      (100)     8436 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/main.py
--rw-r--r--   0 royann   (121683555) users      (100)     2753 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/query_visualization.py
--rw-r--r--   0 royann   (121683555) users      (100)     1732 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/query_visualization_ArtifactExecution.py
--rw-r--r--   0 royann   (121683555) users      (100)     1443 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/query_visualization_execution.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2024-02-16 17:51:44.000000 cmflib-0.0.8/server/app/schemas/
--rw-r--r--   0 royann   (121683555) users      (100)        1 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/schemas/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)      188 2024-02-16 17:50:49.000000 cmflib-0.0.8/server/app/schemas/dataframe.py
--rw-r--r--   0 royann   (121683555) users      (100)      103 2024-02-16 17:51:44.000000 cmflib-0.0.8/setup.cfg
--rw-r--r--   0 royann   (121683555) users      (100)     1106 2024-02-16 17:50:49.000000 cmflib-0.0.8/setup.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.355485 cmflib-0.0.9/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    11356 2024-05-29 16:51:04.000000 cmflib-0.0.9/LICENSE
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    10877 2024-05-31 16:58:13.355485 cmflib-0.0.9/PKG-INFO
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    10154 2024-05-29 16:51:04.000000 cmflib-0.0.9/README.md
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.347485 cmflib-0.0.9/cmflib/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/__init__.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.347485 cmflib-0.0.9/cmflib/bin/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/bin/__init__.py
+-rwxr-xr-x   0 royann   (121683555) ldap      (6347)      214 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/bin/cmf
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     7022 2024-05-31 16:57:15.000000 cmflib-0.0.9/cmflib/bin/cmf_dvc_ingest.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.347485 cmflib-0.0.9/cmflib/cli/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1665 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/cli/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      910 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/cli/command.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2912 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/cli/parser.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2760 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/cli/utils.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    87048 2024-05-31 16:57:15.000000 cmflib-0.0.9/cmflib/cmf.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     5898 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/cmf_commands_wrapper.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     6684 2024-05-31 16:57:15.000000 cmflib-0.0.9/cmflib/cmf_merger.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    38657 2024-05-31 16:57:15.000000 cmflib-0.0.9/cmflib/cmfquery.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.347485 cmflib-0.0.9/cmflib/commands/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/__init__.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/commands/artifact/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1450 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/artifact/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    13517 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/artifact/pull.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1612 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/artifact/push.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/commands/init/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1543 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     5468 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/amazonS3.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     4669 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/local.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     5547 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/minioS3.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2094 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/show.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     5455 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/init/sshremote.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/commands/metadata/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1509 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/metadata/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     3741 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/metadata/export.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     4591 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/metadata/pull.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     7633 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/commands/metadata/push.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    15562 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/dvc_wrapper.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    20186 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/graph_wrapper.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    19673 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/metadata_helper.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      807 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/mlmd_objects.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/server_interface/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/server_interface/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1621 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/server_interface/server_interface.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/storage_backends/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/storage_backends/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2219 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/storage_backends/amazonS3_artifacts.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1718 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/storage_backends/local_artifacts.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1779 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/storage_backends/minio_artifacts.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2229 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/storage_backends/sshremote_artifacts.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/cmflib/utils/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/utils/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2089 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/utils/cmf_config.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1300 2024-05-29 16:51:04.000000 cmflib-0.0.9/cmflib/utils/dvc_config.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     2696 2024-05-31 16:57:15.000000 cmflib-0.0.9/cmflib/utils/helper_functions.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.355485 cmflib-0.0.9/cmflib.egg-info/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    10877 2024-05-31 16:58:13.000000 cmflib-0.0.9/cmflib.egg-info/PKG-INFO
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1729 2024-05-31 16:58:13.000000 cmflib-0.0.9/cmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        1 2024-05-31 16:58:13.000000 cmflib-0.0.9/cmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      113 2024-05-31 16:58:13.000000 cmflib-0.0.9/cmflib.egg-info/requires.txt
+-rw-r--r--   0 royann   (121683555) ldap      (6347)       14 2024-05-31 16:58:13.000000 cmflib-0.0.9/cmflib.egg-info/top_level.txt
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      610 2024-05-31 16:57:15.000000 cmflib-0.0.9/pyproject.toml
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.351485 cmflib-0.0.9/server/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/__init__.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.355485 cmflib-0.0.9/server/app/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        0 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     9663 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/get_data.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)    11593 2024-05-31 16:57:15.000000 cmflib-0.0.9/server/app/main.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1966 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/query_exec_lineage.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1943 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/query_visualization.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1732 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/query_visualization_ArtifactExecution.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      784 2024-05-31 16:57:15.000000 cmflib-0.0.9/server/app/query_visualization_execution.py
+drwxr-xr-x   0 royann   (121683555) ldap      (6347)        0 2024-05-31 16:58:13.355485 cmflib-0.0.9/server/app/schemas/
+-rw-r--r--   0 royann   (121683555) ldap      (6347)        1 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/schemas/__init__.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      188 2024-05-29 16:51:04.000000 cmflib-0.0.9/server/app/schemas/dataframe.py
+-rw-r--r--   0 royann   (121683555) ldap      (6347)      103 2024-05-31 16:58:13.355485 cmflib-0.0.9/setup.cfg
+-rw-r--r--   0 royann   (121683555) ldap      (6347)     1106 2024-05-31 16:57:15.000000 cmflib-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cmflib-0.0.8/LICENSE` & `cmflib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/PKG-INFO` & `cmflib-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
-Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <3.10,>=3.8
+Requires-Python: <=3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ml-metadata==1.15.0
+Requires-Dist: dvc[s3,ssh]==3.51.1
+Requires-Dist: pandas
+Requires-Dist: retrying
+Requires-Dist: pyarrow
+Requires-Dist: neo4j
+Requires-Dist: scikit-learn
+Requires-Dist: tabulate
+Requires-Dist: click
+Requires-Dist: minio
+Requires-Dist: paramiko
 
 # cmf
 ## Common Metadata Framework
 [Getting Started](https://hewlettpackard.github.io/cmf/)<br><br>
 [Detailed documentation of the API's](https://hewlettpackard.github.io/cmf/api/public/cmf) <br> 
 
 Interactions in data pipelines can be complex. The Different stages in the pipeline, (which may not be next to each other) may have to interact to produce or transform artifacts. As the artifacts navigates and undergo transformations through this pipeline, it can take a complicated path, which might also involve bidirectional movement across these stages.  Also there could be dependencies between the multiple stages, where the metrics produced by a stage could influence the metrics at a subsequent stage.  It is important to track the metadata across a pipeline to provide features like, lineage tracking, provenance and reproducibility.
```

### Comparing `cmflib-0.0.8/README.md` & `cmflib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cli/__init__.py` & `cmflib-0.0.9/cmflib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cli/command.py` & `cmflib-0.0.9/cmflib/cli/command.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cli/parser.py` & `cmflib-0.0.9/cmflib/cli/parser.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cli/utils.py` & `cmflib-0.0.9/cmflib/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cmf.py` & `cmflib-0.0.9/cmflib/cmf.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     link_execution_to_artifact,
     create_new_artifact_event_and_attribution,
     get_artifacts_by_id,
     put_artifact,
     link_execution_to_input_artifact,
 )
 from cmflib.utils.cmf_config import CmfConfig
+from cmflib.utils.helper_functions import get_python_env, change_dir
 from cmflib.cmf_commands_wrapper import (
     _metadata_push,
     _metadata_pull,
     _artifact_pull,
     _artifact_push,
     _artifact_pull_single,
     _cmf_cmd_init,
@@ -70,22 +71,22 @@
 class Cmf:
     """This class provides methods to log metadata for distributed AI pipelines.
     The class instance creates an ML metadata store to store the metadata.
     It creates a driver to store nodes and its relationships to neo4j.
     The user has to provide the name of the pipeline, that needs to be recorded with CMF.
     ```python
     cmflib.cmf.Cmf(
-        filename="mlmd",
+        filepath="mlmd",
         pipeline_name="test_pipeline",
         custom_properties={"owner": "user_a"},
         graph=False
     )
     ```
     Args:
-        filename: Path  to the sqlite file to store the metadata
+        filepath: Path  to the sqlite file to store the metadata
         pipeline_name: Name to uniquely identify the pipeline.
         Note that name is the unique identifier for a pipeline.
         If a pipeline already exist with the same name, the existing pipeline object is reused.
         custom_properties: Additional properties of the pipeline that needs to be stored.
         graph: If set to true, the libray also stores the relationships in the provided graph database.
         The following
         variables should be set: `neo4j_uri` (graph server URI), `neo4j_user` (user name) and
@@ -103,37 +104,48 @@
         attr_dict = CmfConfig.read_config(cmf_config)
         __neo4j_uri = attr_dict.get("neo4j-uri", "")
         __neo4j_password = attr_dict.get("neo4j-password", "")
         __neo4j_user = attr_dict.get("neo4j-user", "")
 
     def __init__(
         self,
-        filename: str = "mlmd",
+        filepath: str = "mlmd",
         pipeline_name: str = "",
         custom_properties: t.Optional[t.Dict] = None,
         graph: bool = False,
         is_server: bool = False,
     ):
+        #path to directory
+        self.cmf_init_path = filepath.rsplit("/",1)[0] \
+				 if len(filepath.rsplit("/",1)) > 1 \
+					else  os.getcwd()
+
+        logging_dir = change_dir(self.cmf_init_path)
         if is_server is False:
             Cmf.__prechecks()
         if custom_properties is None:
             custom_properties = {}
+        if not pipeline_name:
+            # assign folder name as pipeline name 
+            cur_folder = os.path.basename(os.getcwd())
+            pipeline_name = cur_folder
         config = mlpb.ConnectionConfig()
-        config.sqlite.filename_uri = filename
+        config.sqlite.filename_uri = filepath
         self.store = metadata_store.MetadataStore(config)
-        self.filename = filename
+        self.filepath = filepath
         self.child_context = None
         self.execution = None
         self.execution_name = ""
         self.execution_command = ""
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         self.graph = graph
-        self.branch_name = filename.rsplit("/", 1)[-1]
+        #last token in filepath
+        self.branch_name = filepath.rsplit("/", 1)[-1]
 
         if is_server is False:
             git_checkout_new_branch(self.branch_name)
         self.parent_context = get_or_create_parent_context(
             store=self.store,
             pipeline=pipeline_name,
             custom_properties=custom_properties,
@@ -144,14 +156,15 @@
             Cmf.__load_neo4j_params()
             self.driver = graph_wrapper.GraphDriver(
                 Cmf.__neo4j_uri, Cmf.__neo4j_user, Cmf.__neo4j_password
             )
             self.driver.create_pipeline_node(
                 pipeline_name, self.parent_context.id, custom_properties
             )
+        os.chdir(logging_dir)
 
     @staticmethod
     def __load_neo4j_params():
          cmf_config = os.environ.get("CONFIG_FILE", ".cmfconfig")
          if os.path.exists(cmf_config):
              attr_dict = CmfConfig.read_config(cmf_config)
              Cmf.__neo4j_uri = attr_dict.get("neo4j-uri", "")
@@ -222,15 +235,15 @@
         Example:
             ```python
             #Create context
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
             # Create CMF logger
-            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            cmf = Cmf(filepath="mlmd", pipeline_name="test_pipeline")
             # Create context
             context: mlmd.proto.Context = cmf.create_context(
                 pipeline_stage="prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             )
 
             ```
@@ -265,15 +278,15 @@
 
             ```python
             #Create context
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
             # Create CMF logger
-            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            cmf = Cmf(filepath="mlmd", pipeline_name="test_pipeline")
             # Create context
             context: mlmd.proto.Context = cmf.merge_created_context(
                 pipeline_stage="Test-env/prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             ```
             Args:
                 Pipeline_stage: Pipeline_Name/Stage_name.
@@ -308,15 +321,15 @@
         [create_context][cmflib.cmf.Cmf.create_context] must be called first.
         Example:
             ```python
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
             # Create CMF logger
-            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            cmf = Cmf(filepath="mlmd", pipeline_name="test_pipeline")
             # Create or reuse context for this stage
             context: mlmd.proto.Context = cmf.create_context(
                 pipeline_stage="prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             )
             # Create a new execution for this stage run
             execution: mlmd.proto.Execution = cmf.create_execution(
@@ -339,35 +352,48 @@
                 it will be reused.
                 Only executions created with  create_new_execution as False will have "name" as a property.
 
 
         Returns:
             Execution object from ML Metadata library associated with the new execution for this stage.
         """
+        # Assigning current file name as stage and execution name
+        current_script = sys.argv[0]
+        file_name = os.path.basename(current_script)
+        name_without_extension = os.path.splitext(file_name)[0]
+        # create context if not already created
+        if not self.child_context:
+            self.create_context(pipeline_stage=name_without_extension)
+            assert self.child_context is not None, f"Failed to create context for {self.pipeline_name}!!"
+
         # Initializing the execution related fields
+
+        logging_dir = change_dir(self.cmf_init_path)
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
         git_start_commit = git_get_commit()
         cmd = str(sys.argv) if cmd is None else cmd
+        python_env=get_python_env()
         self.execution = create_new_execution_in_existing_run_context(
             store=self.store,
             # Type field when re-using executions
             execution_type_name=self.child_context.name,
             execution_name=execution_type, 
             #Name field if we are re-using executions
             #Type field , if creating new executions always 
             context_id=self.child_context.id,
             execution=cmd,
             pipeline_id=self.parent_context.id,
             pipeline_type=self.parent_context.name,
             git_repo=git_repo,
             git_start_commit=git_start_commit,
+            python_env=python_env,
             custom_properties=custom_props,
             create_new_execution=create_new_execution,
         )
         uuids = self.execution.properties["Execution_uuid"].string_value
         if uuids:
             self.execution.properties["Execution_uuid"].string_value = uuids+","+str(uuid.uuid1())
         else:
@@ -377,39 +403,41 @@
         self.execution_command = cmd
         for k, v in custom_props.items():
             k = re.sub("-", "_", k)
             self.execution_label_props[k] = v
         self.execution_label_props["Execution_Name"] = (
             execution_type + ":" + str(self.execution.id)
         )
-        self.execution_label_props["execution_command"] = str(sys.argv)
+        
+        self.execution_label_props["execution_command"] = cmd
         if self.graph:
             self.driver.create_execution_node(
-                self.execution_name,
-                self.child_context.id,
-                self.parent_context,
-                str(sys.argv),
-                self.execution.id,
-                custom_props,
-            )
+            self.execution_name,
+            self.child_context.id,
+            self.parent_context,
+            cmd,
+            self.execution.id,
+            custom_props,
+        )
+        os.chdir(logging_dir)
         return self.execution
 
     def update_execution(
         self, execution_id: int, custom_properties: t.Optional[t.Dict] = None
     ):
         """Updates an existing execution.
         The custom properties can be updated after creation of the execution.
         The new custom properties is merged with earlier custom properties.
         Example
             ```python
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
             # Create CMF logger
-            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            cmf = Cmf(filepath="mlmd", pipeline_name="test_pipeline")
             # Update a execution
             execution: mlmd.proto.Execution = cmf.update_execution(
                 execution_id=8,
                 custom_properties = {"split": split, "seed": seed}
             )
             ```
             Args:
@@ -483,15 +511,15 @@
         to create new executions with additional data(Required on cmf-server).
         Example:
             ```python
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
             # Create CMF logger
-            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            cmf = Cmf(filepath="mlmd", pipeline_name="test_pipeline")
             # Create or reuse context for this stage
             context: mlmd.proto.Context = cmf.merge_created_context(
                 pipeline_stage="prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             )
             # Create a new execution for this stage run
             execution: mlmd.proto.Execution = cmf.merge_created_execution(
@@ -526,14 +554,15 @@
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         custom_props = {} if custom_properties is None else custom_properties
         # print(custom_props)
         git_repo = properties.get("Git_Repo", "")
         git_start_commit = properties.get("Git_Start_Commit", "")
+        python_env = properties.get("Python_Env", "")
         #name = properties.get("Name", "")
         create_new_execution = True
         execution_name = execution_type
         #exe.name property is passed as the orig_execution_name.
         #if name is not an empty string then we are re-using executions
         if orig_execution_name != "":
             create_new_execution = False
@@ -546,14 +575,15 @@
                                            #Type field , if creating new executions always
             context_id=self.child_context.id,
             execution=execution_cmd,
             pipeline_id=self.parent_context.id,
             pipeline_type=self.parent_context.name,
             git_repo=git_repo,
             git_start_commit=git_start_commit,
+            python_env=python_env,
             custom_properties=custom_props,
             create_new_execution=create_new_execution
         )
 
         uuids = ""
 
         uuids = self.execution.properties["Execution_uuid"].string_value
@@ -612,29 +642,49 @@
         Args:
              url: The path to the dataset.
              event: Takes arguments `INPUT` OR `OUTPUT`.
              custom_properties: Dataset properties (key/value pairs).
         Returns:
             Artifact object from ML Metadata library associated with the new dataset artifact.
         """
+
+        # Assigning current file name as stage and execution name
+        current_script = sys.argv[0]
+        file_name = os.path.basename(current_script)
+        name_without_extension = os.path.splitext(file_name)[0]
+        # create context if not already created
+        if not self.child_context:
+            self.create_context(pipeline_stage=name_without_extension)
+            assert self.child_context is not None, f"Failed to create context for {self.pipeline_name}!!"
+
+        # create execution if not already created
+        if not self.execution:
+            self.create_execution(execution_type=name_without_extension)
+            assert self.execution is not None, f"Failed to create execution for {self.pipeline_name}!!"
+
                 ### To Do : Technical Debt. 
         # If the dataset already exist , then we just link the existing dataset to the execution
         # We do not update the dataset properties . 
         # We need to append the new properties to the existing dataset properties
-
+        logging_dir = change_dir(self.cmf_init_path)
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
         name = re.split("/", url)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
 
         commit_output(url, self.execution.id)
         c_hash = dvc_get_hash(url)
+
+        if c_hash == "":
+            print("Error in getting the dvc hash,return without logging")
+            return null
+
         dataset_commit = c_hash
         dvc_url = dvc_get_url(url)
         dvc_url_with_pipeline = f"{self.parent_context.name}:{dvc_url}"
         url = url + ":" + c_hash
         if c_hash and c_hash.strip:
             existing_artifact.extend(self.store.get_artifacts_by_uri(c_hash))
 
@@ -723,14 +773,15 @@
                     "Execution_Command": self.execution_command,
                     "Pipeline_Id": self.parent_context.id,
                     "Pipeline_Name": self.parent_context.name,
                 }
                 self.driver.create_artifact_relationships(
                     self.input_artifacts, child_artifact, self.execution_label_props
                 )
+        os.chdir(logging_dir)
         return artifact
 
     def update_dataset_url(self, artifact: mlpb.Artifact, updated_url: str):
         """Update dataset url
            Updates url of given artifact.
            Example
                ```python
@@ -943,30 +994,51 @@
             model_framework: Framework used to create the model.
             model_type: Type of model algorithm used.
             model_name: Name of the algorithm used.
             custom_properties: The model properties.
         Returns:
             Artifact object from ML Metadata library associated with the new model artifact.
         """
+
+        # Assigning current file name as stage and execution name
+        current_script = sys.argv[0]
+        file_name = os.path.basename(current_script)
+        name_without_extension = os.path.splitext(file_name)[0]
+        # create context if not already created
+        if not self.child_context:
+            self.create_context(pipeline_stage=name_without_extension)
+            assert self.child_context is not None, f"Failed to create context for {self.pipeline_name}!!"
+
+        # create execution if not already created
+        if not self.execution:
+            self.create_execution(execution_type=name_without_extension)
+            assert self.execution is not None, f"Failed to create execution for {self.pipeline_name}!!"
+
+
         # To Do : Technical Debt. 
         # If the model already exist , then we just link the existing model to the execution
         # We do not update the model properties . 
         # We need to append the new properties to the existing model properties
-
+        logging_dir = change_dir(self.cmf_init_path)
         if custom_properties is None:
             custom_properties = {}
         custom_props = {} if custom_properties is None else custom_properties
         # name = re.split('/', path)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
 
         commit_output(path, self.execution.id)
         c_hash = dvc_get_hash(path)
+
+        if c_hash == "":
+            print("Error in getting the dvc hash,return without logging")
+            return null
+
         model_commit = c_hash
 
         # If connecting to an existing artifact - The name of the artifact is
         # used as path/steps/key
         model_uri = path + ":" + c_hash
         dvc_url = dvc_get_url(path, False)
         url = dvc_url
@@ -1060,15 +1132,15 @@
                     "Pipeline_Id": self.parent_context.id,
                     "Pipeline_Name": self.parent_context.name,
                 }
 
                 self.driver.create_artifact_relationships(
                     self.input_artifacts, child_artifact, self.execution_label_props
                 )
-
+        os.chdir(logging_dir)
         return artifact
 
     # Add the model to dvc do a git commit and store the commit id in MLMD
     def log_model_with_version(
         self,
         path: str,
         event: str,
@@ -1224,14 +1296,15 @@
               ``` 
               Args: 
                  metrics_name: Name of the metrics in the format "name:uri:execution_id". 
                  custom_properties: Optional custom properties for the metrics. 
               Returns: 
                  Artifact object from the ML Protocol Buffers library associated with the metrics artifact.
         """
+
         metrics = None
         custom_props = {} if custom_properties is None else custom_properties
         existing_artifact = []
         name_tokens = metrics_name.split(":")
         if name_tokens and len(name_tokens) > 2:
             name = name_tokens[0]
             uri = name_tokens[1]
@@ -1302,14 +1375,30 @@
             ```
         Args:
             metrics_name: Name to identify the metrics.
             custom_properties: Dictionary with metric values.
         Returns:
               Artifact object from ML Metadata library associated with the new coarse-grained metrics artifact.
         """
+        # Assigning current file name as stage and execution name
+        current_script = sys.argv[0]
+        file_name = os.path.basename(current_script)
+        name_without_extension = os.path.splitext(file_name)[0]
+        # create context if not already created
+        if not self.child_context:
+            self.create_context(pipeline_stage=name_without_extension)
+            assert self.child_context is not None, f"Failed to create context for {self.pipeline_name}!!"
+
+        # create execution if not already created
+        if not self.execution:
+            self.create_execution(execution_type=name_without_extension)
+            assert self.execution is not None, f"Failed to create execution for {self.pipeline_name}!!"
+
+
+        logging_dir = change_dir(self.cmf_init_path)
         custom_props = {} if custom_properties is None else custom_properties
         uri = str(uuid.uuid1())
         metrics_name = metrics_name + ":" + uri + ":" + str(self.execution.id)
         metrics = create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
             context_id=self.child_context.id,
@@ -1341,14 +1430,15 @@
                 "Execution_Command": self.execution_command,
                 "Pipeline_Id": self.parent_context.id,
                 "Pipeline_Name": self.parent_context.name,
             }
             self.driver.create_artifact_relationships(
                 self.input_artifacts, child_artifact, self.execution_label_props
             )
+        os.chdir(logging_dir)
         return metrics
 
     def log_metric(
         self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None
     ) -> None:
         """Stores the fine-grained (per step or per epoch) metrics to memory.
         The metrics provided are stored in a parquet file. The `commit_metrics` call add the parquet file in the version
@@ -1384,20 +1474,25 @@
 
         Args:
            metrics_name: Name of the metrics.
 
         Returns:
            Artifact object from the ML Protocol Buffers library associated with the new metrics artifact.
         """
+        logging_dir = change_dir(self.cmf_init_path)
         metrics_df = pd.DataFrame.from_dict(
             self.metrics[metrics_name], orient="index")
         metrics_df.index.names = ["SequenceNumber"]
         metrics_df.to_parquet(metrics_name)
         commit_output(metrics_name, self.execution.id)
         uri = dvc_get_hash(metrics_name)
+
+        if uri == "":
+            print("Error in getting the dvc hash,return without logging")
+            return null
         metrics_commit = uri
         name = (
             metrics_name
             + ":"
             + uri
             + ":"
             + str(self.execution.id)
@@ -1434,14 +1529,16 @@
                 "Type": "Metrics",
                 "Execution_Command": self.execution_command,
                 "Pipeline_Id": self.parent_context.id,
             }
             self.driver.create_artifact_relationships(
                 self.input_artifacts, child_artifact, self.execution_label_props
             )
+
+        os.chdir(logging_dir)
         return metrics
 
     def commit_existing_metrics(self, metrics_name: str, uri: str, custom_properties: t.Optional[t.Dict] = None):
         """ 
         Commits existing metrics associated with the given URI to MLMD. 
         Example: 
         ```python 
@@ -1503,15 +1600,15 @@
                 self.input_artifacts, child_artifact, self.execution_label_props
             )
         return metrics
 
 
     def log_validation_output(
         self, version: str, custom_properties: t.Optional[t.Dict] = None
-    ) -> object:
+    ) -> object: 
         uri = str(uuid.uuid1())
         return create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
             context_id=self.child_context.id,
             uri=uri,
             name=uri,
@@ -1519,14 +1616,15 @@
             event_type=mlpb.Event.Type.INTERNAL_OUTPUT,
             properties={"version": version},
             artifact_type_properties={"version": mlpb.STRING},
             custom_properties=custom_properties,
             milliseconds_since_epoch=int(time.time() * 1000),
         )
 
+
     def update_existing_artifact(
         self, artifact: mlpb.Artifact, custom_properties: t.Dict
     ):
         """ Updates an existing artifact with the provided custom properties and stores it back to MLMD. 
           Example: 
           ```python
                 update_artifact=cmf.update_existing_artifact(existing_artifact, {"key1": "updated_value"}) 
@@ -1672,14 +1770,18 @@
             dataslice_df = pd.DataFrame.from_dict(self.props, orient="index")
             dataslice_df.index.names = ["Path"]
             dataslice_df.to_parquet(self.name)
             existing_artifact = []
 
             commit_output(self.name, self.writer.execution.id)
             c_hash = dvc_get_hash(self.name)
+            if c_hash == "":
+                print("Error in getting the dvc hash,return without logging")
+                return null
+
             dataslice_commit = c_hash
             remote = dvc_get_url(self.name)
             if c_hash and c_hash.strip():
                 existing_artifact.extend(
                     self.writer.store.get_artifacts_by_uri(c_hash))
             if existing_artifact and len(existing_artifact) != 0:
                 print("Adding to existing data slice")
@@ -1756,89 +1858,89 @@
 #            df = pd.read_parquet(name)
 #            for index, row in df.iterrows():
 #                print(index)
 #                first, middle, last = str(index).split("/")
 #                print(last)
 #                os.symlink(str(index), slicedir + "/ " + last)
 
-def metadata_push(pipeline_name,filename,execution_id: str = ""):
+def metadata_push(pipeline_name,filepath,execution_id: str = ""):
     """ Pushes MLMD file to CMF-server.
     Example:
     ```python
          result = metadata_push("example_pipeline", "mlmd_file", "3")
     ```
     Args:
         pipeline_name: Name of the pipeline.
-        filename: Path to the MLMD file.
+        filepath: Path to the MLMD file.
         execution_id: Optional execution ID.
 
     Returns:
         Response output from the _metadata_push function.
     """
-    # Required arguments:  pipeline_name, filename (mlmd file path) 
+    # Required arguments:  pipeline_name, filepath (mlmd file path) 
     #Optional arguments: Execution_ID
-    output = _metadata_push(pipeline_name,filename, execution_id)
+    output = _metadata_push(pipeline_name,filepath, execution_id)
     return output
 
-def metadata_pull(pipeline_name,filename ="./mlmd", execution_id: str = ""):
+def metadata_pull(pipeline_name,filepath ="./mlmd", execution_id: str = ""):
     """ Pulls MLMD file from CMF-server. 
      Example: 
      ```python 
           result = metadata_pull("example_pipeline", "./mlmd_directory", "execution_123") 
      ``` 
      Args: 
         pipeline_name: Name of the pipeline. 
-        filename: File path to store the MLMD file. 
+        filepath: File path to store the MLMD file. 
         execution_id: Optional execution ID. 
      Returns: 
         Message from the _metadata_pull function. 
      """
-    # Required arguments:  pipeline_name, filename(file path to store mlmd file) 
+    # Required arguments:  pipeline_name, filepath(file path to store mlmd file) 
     #Optional arguments: Execution_ID
-    output = _metadata_pull(pipeline_name,filename, execution_id)
+    output = _metadata_pull(pipeline_name,filepath, execution_id)
     return output
 
-def artifact_pull(pipeline_name,filename="./mlmd"):
+def artifact_pull(pipeline_name,filepath="./mlmd"):
     """ Pulls artifacts from the initialized repository.
 
     Example:
     ```python
          result = artifact_pull("example_pipeline", "./mlmd_directory")
     ```
 
     Args:
         pipeline_name: Name of the pipeline.
-        filename: Path to store artifacts.
+        filepath: Path to store artifacts.
 
     Returns:
         Output from the _artifact_pull function.
     """
 
     # Required arguments: Pipeline_name
-    # Optional arguments: filename( path to store artifacts)
-    output = _artifact_pull(pipeline_name,filename)
+    # Optional arguments: filepath( path to store artifacts)
+    output = _artifact_pull(pipeline_name,filepath)
     return output
 
-def artifact_pull_single(pipeline_name,filename,artifact_name):
+def artifact_pull_single(pipeline_name,filepath,artifact_name):
     """ Pulls a single artifact from the initialized repository. 
     Example: 
     ```python 
         result = artifact_pull_single("example_pipeline", "./mlmd_directory", "example_artifact") 
     ```
     Args: 
        pipeline_name: Name of the pipeline. 
-       filename: Path to store the artifact. 
+       filepath: Path to store the artifact. 
        artifact_name: Name of the artifact. 
     Returns:
        Output from the _artifact_pull_single function. 
     """
 
     # Required arguments: Pipeline_name
-    # Optional arguments: filename( path to store artifacts)
-    output = _artifact_pull_single(pipeline_name,filename,artifact_name)
+    # Optional arguments: filepath( path to store artifacts)
+    output = _artifact_pull_single(pipeline_name,filepath,artifact_name)
     return output
 
 def artifact_push():
     """ Pushes artifacts to the initialized repository.
 
     Example:
     ```python
@@ -2009,9 +2111,8 @@
 
     dict_repository_args={"local":local,"minioS3":minioS3,"amazonS3":amazonS3,"sshremote":sshremote}
     
     for repo,arg in dict_repository_args.items():
         if repo ==type:
             non_related_args=list(set(available_args)-set(dict_repository_args[repo]))
     return non_related_args
- 
-    
+
```

### Comparing `cmflib-0.0.8/cmflib/cmf_commands_wrapper.py` & `cmflib-0.0.9/cmflib/cmf_commands_wrapper.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/cmf_merger.py` & `cmflib-0.0.9/cmflib/cmf_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     if cmd == "push":
         data = create_original_time_since_epoch(mlmd_data)
     else:
         data = mlmd_data
     graph = False
     if os.getenv('NEO4J_URI', "") != "":
         graph = True
-    cmf_class = cmf.Cmf(filename=path_to_store, pipeline_name=pipeline_name,
+    cmf_class = cmf.Cmf(filepath=path_to_store, pipeline_name=pipeline_name,
                         graph=graph, is_server=True)
     for stage in data["Pipeline"][0]["stages"]:  # Iterates over all the stages
         if exec_id is None:
             list_executions = [execution for execution in stage["executions"]]
         elif exec_id is not None:
             list_executions = [
                 execution
```

### Comparing `cmflib-0.0.8/cmflib/cmfquery.py` & `cmflib-0.0.9/cmflib/cmfquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             list_exec=self.store.get_executions_by_id(execution_ids)
             execution_ids=[]
             for exe in list_exec:
                 if (self._transform_to_dataframe(exe).Pipeline_id.to_string(index=False)) == str(pipeline_id):
                     execution_ids.append(exe.id)
         return execution_ids
 
-    def _get_executions_by_output_artifact_id(self, artifact_id: int) -> t.List[int]:
+    def _get_executions_by_output_artifact_id(self, artifact_id: int, pipeline_id: str = None) -> t.List[int]:
         """Return stage execution that produced given output artifact.
 
         Args:
             artifact_id: Identifier of the output artifact.
         Return:
             List of stage executions, should probably be size of 1 or zero.
         """
@@ -288,16 +288,21 @@
             event.execution_id
             for event in self.store.get_events_by_artifact_ids([artifact_id])
             if event.type == mlpb.Event.OUTPUT
         ]
         # According to CMF, it's OK to have multiple executions that produce the same exact artifact.
         # if len(execution_ids) >= 2:
         #     logger.warning("%d executions claim artifact (id=%d) as output.", len(execution_ids), artifact_id)
-
-        return list(set(execution_ids))
+        if pipeline_id != None:
+            list_exec = self.store.get_executions_by_id(execution_ids)
+            execution_ids = []
+            for exe in list_exec:
+                if (self._transform_to_dataframe(exe).Pipeline_id.to_string(index=False)) == str(pipeline_id):
+                    execution_ids.append(exe.id)
+        return execution_ids
 
     def _get_artifact(self, name: str) -> t.Optional[mlpb.Artifact]:
         """Return artifact with the given name or None.
         Args:
             name: Fully-qualified name (e.g., artifact hash is added to the name), so name collisions across different
                   artifact types are not issues here.
         Returns:
@@ -589,30 +594,32 @@
 
         # Get output artifacts of executions consumed the above artifact.
         artifacts_ids = self._get_output_artifacts(self._get_executions_by_input_artifact_id(artifact.id,pipeline_id))
         return self._as_pandas_df(
             self.store.get_artifacts_by_id(artifacts_ids), lambda _artifact: self.get_artifact_df(_artifact)
         )
 
-    def get_one_hop_parent_executions(self, execution_id: t.List[int]) -> t.List[int]:
+    def get_one_hop_parent_executions(self, execution_id: t.List[int], pipeline_id: str = None) -> t.List[int]:
         """Get artifacts produced by executions that consume given artifact.
 
         Args:
             artifact name: Name of an artifact.
         Return:
             Output artifacts of all executions that consumed given artifact.
         """
         artifacts_input=self._get_input_artifacts(execution_id)
-        arti=self.store.get_artifacts_by_id(artifacts_input)
-         
+        arti = self.store.get_artifacts_by_id(artifacts_input)
+        list_exec = []
+        exec_ids_added = []
         for i in artifacts_input:
-            exec=self._get_executions_by_output_artifact_id(i)
-            list_exec=self.store.get_executions_by_id(exec)
-#            for id in list_exec:
-                #print(self._transform_to_dataframe(id).Execution_type_name,"@@@@@@@@@")
+            exec = self._get_executions_by_output_artifact_id(i, pipeline_id)
+            if exec not in exec_ids_added:
+                exec_ids_added.append(exec)
+                list_exec.append(self.store.get_executions_by_id(exec))
+        return list_exec
 
     def get_one_hop_child_executions(self, execution_id: t.List[int]) -> t.List[int]:
         """Get artifacts produced by executions that consume given artifact.
 
         Args:
             artifact name: Name of an artifact.
         Return:
@@ -676,14 +683,40 @@
         for row in d1.itertuples():
             d1 = self.get_all_parent_artifacts(row.name)
             # df = df.append(d1, sort=True, ignore_index=True)
             df = pd.concat([df, d1], sort=True, ignore_index=True)
         df = df.drop_duplicates(subset=None, keep="first", inplace=False)
         return df
 
+    def get_all_parent_executions_by_id(self, execution_id: t.List[int], pipeline_id: str = None) -> t.List[int]:
+        parent_executions = [[],[]]
+        current_execution_id = execution_id
+        list_of_parent_execution_id = []
+        link_src_trgt_list = []
+        while current_execution_id:
+            parent_execution_ids = self.get_one_hop_parent_executions(current_execution_id, pipeline_id)
+            list_of_parent_execution_id = []
+            for data in parent_execution_ids:
+                for j in data:
+                    temp=[j.id, j.properties["Execution_type_name"].string_value, j.properties["Execution_uuid"].string_value]
+                    if temp not in parent_executions[0]:
+                        link_src_trgt_list.append({"source":j.id, "target":current_execution_id[0]})
+                        list_of_parent_execution_id.append(temp)
+            if list_of_parent_execution_id:
+                parent_executions[0].extend(list_of_parent_execution_id)
+                parent_executions[1].extend(link_src_trgt_list)
+                for id_name_uuid in list_of_parent_execution_id:
+                    current_execution_id = [id_name_uuid[0]]
+                    recursive_parents = self.get_all_parent_executions_by_id(current_execution_id, pipeline_id)
+                    parent_executions[0].extend(recursive_parents[0])
+                    parent_executions[1].extend(recursive_parents[1])
+            else:
+                break
+        return parent_executions
+
     def get_all_parent_executions(self, artifact_name: str) -> pd.DataFrame:
         """Return all executions that produced upstream artifacts for the given artifact.
         Args:
             artifact_name: Artifact name.
         Returns:
             Data frame containing all parent executions.
         """
```

### Comparing `cmflib-0.0.8/cmflib/commands/artifact/__init__.py` & `cmflib-0.0.9/cmflib/commands/artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/artifact/pull.py` & `cmflib-0.0.9/cmflib/commands/artifact/pull.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/artifact/push.py` & `cmflib-0.0.9/cmflib/commands/artifact/push.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/__init__.py` & `cmflib-0.0.9/cmflib/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/amazonS3.py` & `cmflib-0.0.9/cmflib/commands/init/amazonS3.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/local.py` & `cmflib-0.0.9/cmflib/commands/init/local.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/minioS3.py` & `cmflib-0.0.9/cmflib/commands/init/minioS3.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/show.py` & `cmflib-0.0.9/cmflib/commands/init/show.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/init/sshremote.py` & `cmflib-0.0.9/cmflib/commands/init/sshremote.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/metadata/__init__.py` & `cmflib-0.0.9/cmflib/commands/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/metadata/export.py` & `cmflib-0.0.9/cmflib/commands/metadata/export.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/commands/metadata/pull.py` & `cmflib-0.0.9/cmflib/commands/metadata/pull.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/dvc_wrapper.py` & `cmflib-0.0.9/cmflib/dvc_wrapper.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/graph_wrapper.py` & `cmflib-0.0.9/cmflib/graph_wrapper.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/metadata_helper.py` & `cmflib-0.0.9/cmflib/metadata_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,15 @@
 EXECUTION_CONTEXT_NAME_PROPERTY_NAME = "Context_Type"
 EXECUTION_CONTEXT_ID = "Context_ID"
 EXECUTION_EXECUTION = "Execution"
 EXECUTION_EXECUTION_TYPE_NAME="Execution_type_name"
 EXECUTION_REPO = "Git_Repo"
 EXECUTION_START_COMMIT = "Git_Start_Commit"
 EXECUTION_END_COMMIT = "Git_End_Commit"
+EXECUTION_PYTHON_ENV= "Python_Env"
 EXECUTION_PIPELINE_TYPE = "Pipeline_Type"
 
 EXECUTION_PIPELINE_ID = "Pipeline_id"
 EXECUTION_UNIQUE_ID = "Execution_uuid"
 
 def get_or_create_parent_context(
         store,
@@ -381,14 +382,15 @@
         context_id: int = 0,  # TRAINING CONTEXT ASSOCIATED WITH THIS EXECUTION
         execution: str = None,
         pipeline_id: int = 0,  # THE PARENT CONTEXT
         pipeline_type: str = None,
         git_repo: str = None,
         git_start_commit: str = None,
         git_end_commit: str = "",
+        python_env: str = "",
         custom_properties: {} = None,
         create_new_execution:bool = True
 ) -> metadata_store_pb2.Execution:
     mlmd_custom_properties = {}
     for property_name, property_value in (custom_properties or {}).items():
         mlmd_custom_properties[property_name] = value_to_mlmd_value(
             property_value)
@@ -405,28 +407,30 @@
             EXECUTION_EXECUTION: metadata_store_pb2.STRING,
             EXECUTION_EXECUTION_TYPE_NAME: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_TYPE: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_ID: metadata_store_pb2.INT,
             EXECUTION_REPO: metadata_store_pb2.STRING,
             EXECUTION_START_COMMIT: metadata_store_pb2.STRING,
             EXECUTION_END_COMMIT: metadata_store_pb2.STRING,
+            EXECUTION_PYTHON_ENV: metadata_store_pb2.STRING,
         },
 
         properties={
 
             EXECUTION_CONTEXT_NAME_PROPERTY_NAME: metadata_store_pb2.Value(string_value=execution_type_name),
             # Mistakenly used for grouping in the UX
             EXECUTION_CONTEXT_ID: metadata_store_pb2.Value(int_value=context_id),
             EXECUTION_EXECUTION: metadata_store_pb2.Value(string_value=execution),
             EXECUTION_EXECUTION_TYPE_NAME: metadata_store_pb2.Value(string_value=execution_type_name),
             EXECUTION_PIPELINE_TYPE: metadata_store_pb2.Value(string_value=pipeline_type),
             EXECUTION_PIPELINE_ID: metadata_store_pb2.Value(int_value=pipeline_id),
             EXECUTION_REPO: metadata_store_pb2.Value(string_value=git_repo),
             EXECUTION_START_COMMIT: metadata_store_pb2.Value(string_value=git_start_commit),
-            EXECUTION_END_COMMIT: metadata_store_pb2.Value(string_value=git_end_commit)
+            EXECUTION_END_COMMIT: metadata_store_pb2.Value(string_value=git_end_commit),
+            EXECUTION_PYTHON_ENV: metadata_store_pb2.Value(string_value=python_env),
             # should set to task ID, not component ID
         },
         custom_properties=mlmd_custom_properties,
         create_new_execution=create_new_execution
     )
```

### Comparing `cmflib-0.0.8/cmflib/mlmd_objects.py` & `cmflib-0.0.9/cmflib/mlmd_objects.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/server_interface/server_interface.py` & `cmflib-0.0.9/cmflib/server_interface/server_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,16 @@
 
 
 # This function gets mlmd data from mlmd_pull api from cmf-server
 def call_mlmd_pull(url, pipeline_name, exec_id):
     url_to_pass = f"{url}/mlmd_pull/{pipeline_name}"
     response = requests.get(url_to_pass, json={"exec_id": exec_id})  # Get request
     return response
+
+
+# This function posts tensorboard files to cmf-server
+def call_tensorboard(url, pipeline_name, file_name, file_path):
+    url_to_pass = f"{url}/tensorboard"
+    files = {'file': (file_name, open(file_path, 'rb'))}
+    params = {'pipeline_name': pipeline_name}
+    response = requests.post(url_to_pass, files=files, params=params)
+    return response
```

### Comparing `cmflib-0.0.8/cmflib/storage_backends/amazonS3_artifacts.py` & `cmflib-0.0.9/cmflib/storage_backends/amazonS3_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/storage_backends/local_artifacts.py` & `cmflib-0.0.9/cmflib/storage_backends/local_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/storage_backends/minio_artifacts.py` & `cmflib-0.0.9/cmflib/storage_backends/minio_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/storage_backends/sshremote_artifacts.py` & `cmflib-0.0.9/cmflib/storage_backends/sshremote_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/utils/cmf_config.py` & `cmflib-0.0.9/cmflib/utils/cmf_config.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib/utils/dvc_config.py` & `cmflib-0.0.9/cmflib/utils/dvc_config.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/cmflib.egg-info/PKG-INFO` & `cmflib-0.0.9/cmflib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
-Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <3.10,>=3.8
+Requires-Python: <=3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ml-metadata==1.15.0
+Requires-Dist: dvc[s3,ssh]==3.51.1
+Requires-Dist: pandas
+Requires-Dist: retrying
+Requires-Dist: pyarrow
+Requires-Dist: neo4j
+Requires-Dist: scikit-learn
+Requires-Dist: tabulate
+Requires-Dist: click
+Requires-Dist: minio
+Requires-Dist: paramiko
 
 # cmf
 ## Common Metadata Framework
 [Getting Started](https://hewlettpackard.github.io/cmf/)<br><br>
 [Detailed documentation of the API's](https://hewlettpackard.github.io/cmf/api/public/cmf) <br> 
 
 Interactions in data pipelines can be complex. The Different stages in the pipeline, (which may not be next to each other) may have to interact to produce or transform artifacts. As the artifacts navigates and undergo transformations through this pipeline, it can take a complicated path, which might also involve bidirectional movement across these stages.  Also there could be dependencies between the multiple stages, where the metrics produced by a stage could influence the metrics at a subsequent stage.  It is important to track the metadata across a pipeline to provide features like, lineage tracking, provenance and reproducibility.
```

### Comparing `cmflib-0.0.8/cmflib.egg-info/SOURCES.txt` & `cmflib-0.0.9/cmflib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 cmflib.egg-info/PKG-INFO
 cmflib.egg-info/SOURCES.txt
 cmflib.egg-info/dependency_links.txt
 cmflib.egg-info/requires.txt
 cmflib.egg-info/top_level.txt
 cmflib/bin/__init__.py
 cmflib/bin/cmf
+cmflib/bin/cmf_dvc_ingest.py
 cmflib/cli/__init__.py
 cmflib/cli/command.py
 cmflib/cli/parser.py
 cmflib/cli/utils.py
 cmflib/commands/__init__.py
 cmflib/commands/artifact/__init__.py
 cmflib/commands/artifact/pull.py
@@ -48,12 +49,13 @@
 cmflib/utils/cmf_config.py
 cmflib/utils/dvc_config.py
 cmflib/utils/helper_functions.py
 server/__init__.py
 server/app/__init__.py
 server/app/get_data.py
 server/app/main.py
+server/app/query_exec_lineage.py
 server/app/query_visualization.py
 server/app/query_visualization_ArtifactExecution.py
 server/app/query_visualization_execution.py
 server/app/schemas/__init__.py
 server/app/schemas/dataframe.py
```

### Comparing `cmflib-0.0.8/pyproject.toml` & `cmflib-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "cmflib"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
-	"ml-metadata==1.11.0",
-	"dvc[ssh,s3]==2.27.0",
+	"ml-metadata==1.15.0",
+	"dvc[ssh,s3]==3.51.1",
 	"pandas",
 	"retrying",
 	"pyarrow",
 	"neo4j",
 	"scikit-learn",
 	"tabulate",
 	"click",
@@ -15,15 +15,15 @@
 	"paramiko",
 ]
 authors = [
   { name="Hewlett Packard Enterprise"},
 ]
 description = "Track metadata for AI pipeline"
 readme = "README.md"
-requires-python = ">=3.8,<3.10"
+requires-python = ">=3.9,<=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/HewlettPackard/cmf"
```

### Comparing `cmflib-0.0.8/server/app/get_data.py` & `cmflib-0.0.9/server/app/get_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,68 +2,88 @@
 import pandas as pd
 import json,glob
 import os
 from server.app.query_visualization import query_visualization
 from server.app.query_visualization_execution import query_visualization_execution
 from fastapi.responses import FileResponse
 
-def get_executions_by_ids(mlmdfilepath, pipeline_name, exe_ids):
+async def get_executions_by_ids(mlmdfilepath, pipeline_name, exe_ids):
+    '''
+    Args:
+     mlmdfilepath: mlmd file path.
+     pipeline_name: name of the pipeline.
+     exe_ids: list of execution ids.
+   
+    Returns:
+     returns dataframe of executions using execution_ids.
+    '''
     query = cmfquery.CmfQuery(mlmdfilepath)
     df = pd.DataFrame()
     executions = query.get_all_executions_by_ids_list(exe_ids)
     df = pd.concat([df, executions], sort=True, ignore_index=True)
     #df=df.drop('name',axis=1)
     return df
 
-def get_all_exe_ids(mlmdfilepath):
+async def get_all_exe_ids(mlmdfilepath):
+    '''
+    Returns:
+        returns a dictionary which has pipeline_name as key and dataframe which includes {id,Execution_uuid,Context_Type,Context_id} as value.
+    '''
     query = cmfquery.CmfQuery(mlmdfilepath)
-    df = pd.DataFrame()
     execution_ids = {}
     names = query.get_pipeline_names()
     for name in names:
+        df = pd.DataFrame()    # df is emptied to store execution ids for next pipeline.
         stages = query.get_pipeline_stages(name)
         for stage in stages:
             executions = query.get_all_executions_in_stage(stage)
             df = pd.concat([df, executions], sort=True, ignore_index=True)
-    if df.empty:
-        return
-    for name in names:
-        execution_ids[name] = df.loc[df['Pipeline_Type'] == name, ['id', 'Context_Type']]
+        # check if df is empty return just pipeline_name: {}
+        # if df is not empty return dictionary with pipeline_name as key 
+        # and df with id, context_type, uuid, context_ID as value.
+        if not df.empty:
+            execution_ids[name] = df[['id', 'Context_Type', 'Execution_uuid', 'Context_ID']]
+        else:
+            execution_ids[name] = pd.DataFrame()
     return execution_ids
 
-def get_all_artifact_ids(mlmdfilepath):
+async def get_all_artifact_ids(mlmdfilepath):
     # following is a dictionary of dictionary
     # First level dictionary key is pipeline_name
     # First level dicitonary value is nested dictionary
     # Nested dictionary key is type i.e. Dataset, Model, etc.
     # Nested dictionary value is ids i.e. set of integers
     artifact_ids = {}
     query = cmfquery.CmfQuery(mlmdfilepath)
     names = query.get_pipeline_names()
-    execution_ids = get_all_exe_ids(mlmdfilepath)
+    execution_ids = await get_all_exe_ids(mlmdfilepath)
     for name in names:
         df = pd.DataFrame()
-        exe_ids = execution_ids[name]['id'].tolist()
-        for id in exe_ids:
-            artifacts = query.get_all_artifacts_for_execution(id)
-            df = pd.concat([df, artifacts], sort=True, ignore_index=True)
-        df.sort_values("id", inplace=True) 
-        df.drop_duplicates(subset="id",keep='first', inplace=True)
-        if df.empty:
-            return 
+        if not execution_ids.get(name).empty:
+            exe_ids = execution_ids[name]['id'].tolist()
+            for id in exe_ids:
+                artifacts = query.get_all_artifacts_for_execution(id)
+                df = pd.concat([df, artifacts], sort=True, ignore_index=True)
+            #acknowledging pipeline exist even if df is empty. 
+            if df.empty:
+                artifact_ids[name] = pd.DataFrame()   # { pipeline_name: {empty df} }
+            else:
+                df.sort_values("id", inplace=True)
+                df.drop_duplicates(subset="id", keep='first', inplace=True)
+                artifact_ids[name] = {}
+                for art_type in df['type']:
+                    filtered_values = df.loc[df['type'] == art_type, ['id', 'name']]
+                    artifact_ids[name][art_type] = filtered_values
+        # if execution_ids is empty create dictionary with key as pipeline name
+        # and value as empty df
         else:
-            artifact_ids[name] = {}
-            for art_type in df['type']:
-                filtered_values = df.loc[df['type'] == art_type, ['id', 'name']]
-                artifact_ids[name][art_type] = filtered_values
-    #print("artifact_ids")
-    #print(artifact_ids)
+            artifact_ids[name] = pd.DataFrame()
     return artifact_ids
 
-def get_artifacts(mlmdfilepath, pipeline_name, art_type, artifact_ids):
+async def get_artifacts(mlmdfilepath, pipeline_name, art_type, artifact_ids):
     query = cmfquery.CmfQuery(mlmdfilepath)
     names = query.get_pipeline_names()  # getting all pipeline names in mlmd
     df = pd.DataFrame()
     for name in names:
         if name == pipeline_name:
             df = query.get_all_artifacts_by_ids_list(artifact_ids)
             if len(df) == 0:
@@ -72,15 +92,15 @@
             art_names = df['name'].tolist()
             name_dict = {}
             name_list = []
             exec_type_name_list = []
             exe_type_name = pd.DataFrame()
             for name in art_names:
                 executions = query.get_all_executions_for_artifact(name)
-                exe_type_name = pd.concat([exe_type_name,executions],ignore_index=True)
+                exe_type_name = pd.concat([exe_type_name, executions], ignore_index=True)
                 execution_type_name = exe_type_name["execution_type_name"].drop_duplicates().tolist()
                 execution_type_name = [str(element).split('"')[1] for element in execution_type_name]
                 execution_type_name_str = ',\n '.join(map(str, execution_type_name))
                 name_list.append(name)
                 exec_type_name_list.append(execution_type_name_str)
             name_dict['name'] = name_list
             name_dict['execution_type_name'] = exec_type_name_list
@@ -93,40 +113,41 @@
             return tempout
 
 def get_artifact_types(mlmdfilepath):
     query = cmfquery.CmfQuery(mlmdfilepath)
     artifact_types = query.get_all_artifact_types()
     return artifact_types
 
-def create_unique_executions(server_store_path, req_info):
+async def create_unique_executions(server_store_path, req_info):
     mlmd_data = json.loads(req_info["json_payload"])
     pipelines = mlmd_data["Pipeline"]
     pipeline = pipelines[0]
     pipeline_name = pipeline["name"]
     executions_server = []
     list_executions_exists = []
     if os.path.exists(server_store_path):
         query = cmfquery.CmfQuery(server_store_path)
         stages = query.get_pipeline_stages(pipeline_name)
         for stage in stages:
             executions = []
             executions = query.get_all_executions_in_stage(stage)
-            for i in executions.index:                
+            for i in executions.index:
                 for uuid in executions['Execution_uuid'][i].split(","):
                     executions_server.append(uuid)
         executions_client = []
         for i in mlmd_data['Pipeline'][0]["stages"]:  # checks if given execution_id present in mlmd
             for j in i["executions"]:
                 if j['name'] != "": #If executions have name , they are reusable executions
-                    continue       #which needs to be merged in irrespective of whether already 
+                    continue       #which needs to be merged in irrespective of whether already
                                    #present or not so that new artifacts associated with it gets in.
                 if 'Execution_uuid' in j['properties']:
                     for uuid in j['properties']['Execution_uuid'].split(","):
                         executions_client.append(uuid)
                 else:
+                    # mlmd push is failed here
                     status="version_update"
                     return status
         if executions_server != []:
             list_executions_exists = list(set(executions_client).intersection(set(executions_server)))
         for i in mlmd_data["Pipeline"]:
             for stage in i['stages']:
                 for cmf_exec in stage['executions'][:]:
@@ -144,15 +165,15 @@
             cmf_merger.parse_json_to_mlmd(
                 json.dumps(mlmd_data), "/cmf-server/data/mlmd", "push", req_info["id"]
             )
             status='success'
     return status
 
 
-def get_mlmd_from_server(server_store_path, pipeline_name, exec_id):
+async def get_mlmd_from_server(server_store_path, pipeline_name, exec_id):
     query = cmfquery.CmfQuery(server_store_path)
     execution_flag = 0
     # checks if given execution_id present in mlmd
     if (
         pipeline_name in query.get_pipeline_names()
     ):  # checks if pipeline name is available in mlmd
         json_payload = query.dumptojson(pipeline_name, None)
@@ -170,17 +191,27 @@
             else:
                 json_payload = "no_exec_id"
                 return json_payload
     else:
         json_payload = "NULL"
     return json_payload
 
-def get_lineage_img_path(server_store_path,pipeline_name,type):
+async def get_lineage_data(server_store_path,pipeline_name,type,dict_of_art_ids,dict_of_exe_ids):
     query = cmfquery.CmfQuery(server_store_path)
     if type=="Artifacts":
-        lineage_data = query_visualization(server_store_path, pipeline_name)
+        lineage_data = query_visualization(server_store_path, pipeline_name, dict_of_art_ids)
+        '''
+        returns dictionary of nodes and links for artifact lineage.
+        lineage_data= {
+                       nodes:[],
+                       links:[]
+                      }
+        '''
     elif type=="Execution":
-        lineage_data = query_visualization_execution(server_store_path, pipeline_name)
+        lineage_data = query_visualization_execution(server_store_path, pipeline_name, dict_of_art_ids, dict_of_exe_ids)
+        '''
+        returns list of execution types for specific pipeline.
+        '''
     else:
-        lineage_data = query_visualization_ArtifactExecution(server_store_path, pipeline_name)  
+        lineage_data = query_visualization_ArtifactExecution(server_store_path, pipeline_name)
     return lineage_data
```

### Comparing `cmflib-0.0.8/server/app/main.py` & `cmflib-0.0.9/server/app/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # cmf-server api's
-from fastapi import FastAPI, Request, status, HTTPException, Query
+from fastapi import FastAPI, Request, status, HTTPException, Query, UploadFile, File
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse, StreamingResponse
 from fastapi.staticfiles import StaticFiles
-
 from contextlib import asynccontextmanager
 import pandas as pd
 
 from cmflib import cmfquery, cmf_merger
 from server.app.get_data import (
     get_artifacts,
-    get_lineage_img_path,
+    get_lineage_data,
     create_unique_executions,
     get_mlmd_from_server,
     get_artifact_types,
     get_all_artifact_ids,
     get_all_exe_ids,
     get_executions_by_ids
 )
 from server.app.query_visualization import query_visualization
-
+from server.app.query_exec_lineage import query_exec_lineage
 from pathlib import Path
 import os
 import json
 
 server_store_path = "/cmf-server/data/mlmd"
 
 dict_of_art_ids = {}
 dict_of_exe_ids = {}
 
+#lifespan used to prevent multiple loading and save time for visualization.
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     global dict_of_art_ids
     global dict_of_exe_ids
     if os.path.exists(server_store_path):
         # loaded artifact ids into memory
-        dict_of_art_ids = get_all_artifact_ids(server_store_path)
+        dict_of_art_ids = await get_all_artifact_ids(server_store_path)
         # loaded execution ids with names into memory
-        dict_of_exe_ids = get_all_exe_ids(server_store_path)
+        dict_of_exe_ids = await get_all_exe_ids(server_store_path)
     yield
     dict_of_art_ids.clear()
     dict_of_exe_ids.clear()
 
 app = FastAPI(title="cmf-server", lifespan=lifespan)
 
 BASE_PATH = Path(__file__).resolve().parent
 app.mount("/cmf-server/data/static", StaticFiles(directory="/cmf-server/data/static"), name="static")
 server_store_path = "/cmf-server/data/mlmd"
 
 my_ip = os.environ.get("MYIP", "127.0.0.1")
 hostname = os.environ.get('HOSTNAME', "localhost")
 
+#checking if IP or Hostname is provided,initializing url accordingly.
 if my_ip != "127.0.0.1":
     url="http://"+my_ip+":3000"
 else:
     url="http://"+hostname+":3000"
 
 origins = [
     "http://localhost:3000",
@@ -68,38 +69,42 @@
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
 @app.get("/")
-def read_root(request: Request):
+async def read_root(request: Request):
     return {"cmf-server"}
 
 
 # api to post mlmd file to cmf-server
 @app.post("/mlmd_push")
 async def mlmd_push(info: Request):
     print("mlmd push started")
     print("......................")
     req_info = await info.json()
-    status= create_unique_executions(server_store_path,req_info)
+    status = await create_unique_executions(server_store_path, req_info)
+    if status == "version_update":
+        # Raise an HTTPException with status code 422
+        raise HTTPException(status_code=422, detail="version_update")
     # async function
     await update_global_art_dict()
     await update_global_exe_dict()
     return {"status": status, "data": req_info}
 
 
 # api to get mlmd file from cmf-server
-@app.get("/mlmd_pull/{pipeline_name}",response_class=HTMLResponse)
+@app.get("/mlmd_pull/{pipeline_name}", response_class=HTMLResponse)
 async def mlmd_pull(info: Request, pipeline_name: str):
     # checks if mlmd file exists on server
     req_info = await info.json()
     if os.path.exists(server_store_path):
-        json_payload= get_mlmd_from_server(server_store_path,pipeline_name,req_info['exec_id'])
+        #json_payload values can be json data, NULL or no_exec_id.
+        json_payload= await get_mlmd_from_server(server_store_path, pipeline_name, req_info['exec_id'])
     else:
         print("No mlmd file submitted.")
         json_payload = ""
     return json_payload
 
 # api to display executions available in mlmd
 @app.get("/display_executions/{pipeline_name}")
@@ -124,45 +129,84 @@
         exe_ids = exe_ids_sorted['id'].tolist()
         total_items = len(exe_ids)
         start_idx = (page - 1) * per_page
         end_idx = start_idx + per_page
         if total_items < end_idx:
             end_idx = total_items
         exe_ids_list = exe_ids[start_idx:end_idx]
-        executions_df = get_executions_by_ids(server_store_path, pipeline_name, exe_ids_list)
+        executions_df = await get_executions_by_ids(server_store_path, pipeline_name, exe_ids_list)
         temp = executions_df.to_json(orient="records")
         executions_parsed = json.loads(temp)
         return {
             "total_items": total_items,
             "items": executions_parsed
         }
     else:
         return
 
+@app.get("/display_artifact_lineage/{pipeline_name}")
+async def display_artifact_lineage(request: Request, pipeline_name: str):
+    '''
+      This api's returns dictionary of nodes and links for given 
+      pipeline.
+      response = {
+                   nodes: [{id:"",name:""}],
+                   links: [{source:1,target:4},{}],
+                 }
 
-@app.get("/display_lineage/{lineage_type}/{pipeline_name}")
-async def display_lineage(request: Request,lineage_type: str, pipeline_name: str):
+    '''
     # checks if mlmd file exists on server
-    img_path=""
+ 
     if os.path.exists(server_store_path):
         query = cmfquery.CmfQuery(server_store_path)
         if (pipeline_name in query.get_pipeline_names()):
-            if lineage_type=="Artifacts":
-                response=get_lineage_img_path(server_store_path,pipeline_name,"Artifacts")
-            elif lineage_type=="Execution":
-                response=get_lineage_img_path(server_store_path,pipeline_name,"Execution")
-            else:
-                response=get_lineage_img_path(server_store_path,pipeline_name,"ArtifactExecution")
+            response=await get_lineage_data(server_store_path,pipeline_name,"Artifacts",dict_of_art_ids,dict_of_exe_ids)
             return response
         else:
             return f"Pipeline name {pipeline_name} doesn't exist."
 
     else:
-        return 'mlmd does not exist!!'
+        return None
+
+@app.get("/get_execution_types/{pipeline_name}")
+async def get_execution_types(request: Request, pipeline_name: str):
+    '''
+      This api's returns
+      list of execution types.
+
+    '''
+    # checks if mlmd file exists on server
+    if os.path.exists(server_store_path):
+        query = cmfquery.CmfQuery(server_store_path)
+        if (pipeline_name in query.get_pipeline_names()):
+            response = await get_lineage_data(server_store_path,pipeline_name,"Execution",dict_of_art_ids,dict_of_exe_ids)
+            return response
+        else:
+            return f"Pipeline name {pipeline_name} doesn't exist."
 
+    else:
+        return None
+
+@app.get("/display_exec_lineage/{exec_type}/{pipeline_name}/{uuid}")
+async def display_exec_lineage(request: Request, exec_type: str, pipeline_name: str, uuid: str):
+    '''
+      returns dictionary of nodes and links for given execution_type.
+      response = {
+                   nodes: [{id:"",name:"",execution_uuid:""}],
+                   links: [{source:1,target:4},{}],
+                 } 
+    '''
+    # checks if mlmd file exists on server
+    if os.path.exists(server_store_path):
+        query = cmfquery.CmfQuery(server_store_path)
+        if (pipeline_name in query.get_pipeline_names()):
+            response = await query_exec_lineage(server_store_path, pipeline_name, dict_of_exe_ids, exec_type, uuid)
+    else:
+        response = None
+    return response
 
 # api to display artifacts available in mlmd
 @app.get("/display_artifacts/{pipeline_name}/{type}")
 async def display_artifact(
     request: Request,
     pipeline_name: str,
     type: str,   # type = artifact type
@@ -176,43 +220,58 @@
     empty_df = pd.DataFrame()
     art_ids_dict = {}
     art_type = type
     # checks if mlmd file exists on server
     if os.path.exists(server_store_path):
         art_ids_dict = dict_of_art_ids[pipeline_name]
         if not art_ids_dict:
-            return
+            return {               #return {items: None} so that GUI loads 
+            "total_items": 0,      #empty page when art_ids_dict is {}
+            "items": None
+            }
         art_ids_initial = []
         if art_type in art_ids_dict:
             art_ids_initial = art_ids_dict[art_type]
         else:
-            return
+            return {
+            "total_items": 0,
+            "items": None
+        }
         # Apply filtering if provided
         if filter_by and filter_value:
             art_ids_initial = art_ids_initial[art_ids_initial[filter_by].str.contains(filter_value, case=False)]
         # Apply sorting if provided
         art_ids_sorted = art_ids_initial.sort_values(by=sort_field, ascending=(sort_order == "asc"))
         art_ids = art_ids_sorted['id'].tolist()
         total_items = len(art_ids)
         start_idx = (page - 1) * per_page
         end_idx = start_idx + per_page
         if total_items < end_idx:
             end_idx = total_items
         artifact_id_list = list(art_ids)[start_idx:end_idx]
-        artifact_df = get_artifacts(server_store_path, pipeline_name, art_type, artifact_id_list)
+        artifact_df = await get_artifacts(server_store_path, pipeline_name, art_type, artifact_id_list)
         data_paginated = artifact_df
+        #data_paginated is returned None if artifact df is None or {}
+        #it will load empty page, without this condition it will load 
+        #data of whichever artifact_type is loaded before this. 
+        if artifact_df == None or artifact_df == {}:   
+            data_paginated = None      
+            total_items = 0
         return {
             "total_items": total_items,
             "items": data_paginated
         }
     else:
-        return f"{server_store_path} file doesn't exist."
-
-
+        print(f"{server_store_path} file doesn't exist.")
+        return {
+            "total_items": 0,
+            "items": None
+        }
 
+#This api's returns list of artifact types.
 @app.get("/display_artifact_types")
 async def display_artifact_types(request: Request):
     # checks if mlmd file exists on server
     if os.path.exists(server_store_path):
         artifact_types = get_artifact_types(server_store_path)
         return artifact_types
     else:
@@ -229,20 +288,31 @@
         return pipeline_names
     else:
         print("No mlmd file submitted.")
         pipeline_names = []
         return pipeline_names
 
 
+@app.post("/tensorboard")
+async def upload_file(request:Request, pipeline_name: str = Query(..., description="Pipeline name"),
+    file: UploadFile = File(..., description="The file to upload")):
+    try:
+        file_path = os.path.join("/cmf-server/data/tensorboard-logs", pipeline_name, file.filename)
+        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        with open(file_path, "wb") as buffer:
+            buffer.write(await file.read())
+        return {"message": f"File '{file.filename}' uploaded successfully"}
+    except Exception as e:
+        return {"error": f"Failed to up load file: {e}"}
 
 async def update_global_art_dict():
     global dict_of_art_ids
-    output_dict = get_all_artifact_ids(server_store_path)
+    output_dict = await get_all_artifact_ids(server_store_path)
     dict_of_art_ids = output_dict
     return
 
 
 async def update_global_exe_dict():
     global dict_of_exe_ids
-    output_dict = get_all_exe_ids(server_store_path)
+    output_dict = await get_all_exe_ids(server_store_path)
     dict_of_exe_ids = output_dict
     return
```

### Comparing `cmflib-0.0.8/server/app/query_visualization_ArtifactExecution.py` & `cmflib-0.0.9/server/app/query_visualization_ArtifactExecution.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.8/setup.py` & `cmflib-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Metadata Python Package'
 LONG_DESCRIPTION = 'Metadata framework storing AI metadata into MLMD'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="cmflib",
         version=VERSION,
         author="Hewlett Packard Enterprise",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=["ml-metadata==1.11.0",
-                          "dvc[ssh,s3]==2.27.0", "pandas", "retrying", "pyarrow", "neo4j", \
+        install_requires=["ml-metadata==1.15.0",
+                          "dvc[ssh,s3]==3.51.1", "pandas", "retrying", "pyarrow", "neo4j", \
                             "scikit-learn", "tabulate", "click", "minio", "paramiko"],  # add any additional packages that
         # needs to be installed along with your package. Eg: 'caer'
 
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
```

