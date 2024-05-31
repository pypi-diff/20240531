# Comparing `tmp/illumio_pylo-0.3.6.tar.gz` & `tmp/illumio_pylo-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illumio_pylo-0.3.6.tar", last modified: Fri Apr 26 14:58:07 2024, max compression
+gzip compressed data, was "illumio_pylo-0.3.7.tar", last modified: Fri May 31 16:07:13 2024, max compression
```

## Comparing `illumio_pylo-0.3.6.tar` & `illumio_pylo-0.3.7.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.838063 illumio_pylo-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.818063 illumio_pylo-0.3.6/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.814063 illumio_pylo-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.818063 illumio_pylo-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.github/workflows/doxygen-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.github/workflows/make-binaries.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-26 14:58:07.838063 illumio_pylo-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.822063 illumio_pylo-0.3.6/dev_playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/check_unique_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/check_unique_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/delete_all_workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/delete_unused_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/explorer_report_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/export_rules_to_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/generate-random-workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/healthcheck_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/import-labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/import_workloads_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/iplists_stats_duplicates_unused_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/recalculate_explorer_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/recalculate_explorer_logs_multithreaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/rules_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/rules_exporter_special.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/test_change_workload_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/test_query2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/test_securityprincipals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/ven_idle_to_illumination.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/dev_playground/ven_reassign_pce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.822063 illumio_pylo-0.3.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/examples/explorer_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/examples/extend_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.826063 illumio_pylo-0.3.6/illumio_pylo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.830063 illumio_pylo-0.3.6/illumio_pylo/API/
--rw-r--r--   0 runner    (1001) docker     (127)    60725 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/APIConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/AuditLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/ClusterHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/CredentialsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/Explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/JsonPayloadTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/RuleSearchQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/AgentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.830063 illumio_pylo-0.3.6/illumio_pylo/Helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21890 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Helpers/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/IPList.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/IPMap.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/LabelCommon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/LabelGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/LabelStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/LabeledObject.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/ReferenceTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/RulesetStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/SecurityPrincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/SoftwareVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/VirtualService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/VirtualServiceStore.py
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/Workload.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/WorkloadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/WorkloadStoreSubClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.830063 illumio_pylo-0.3.6/illumio_pylo/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/NativeParsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/iplist_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/iplist_import_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/ruleset_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/update_pce_objects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/LabelCreation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_compatibility_report_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_duplicate_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_idle_to_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_reset_names_to_null.py
--rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/docs/Doxygen
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/credentials.example.json
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/health_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/iplists-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/iplists-import-example.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/workloads-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/illumio_pylo/utilities/resources/workloads-import-example.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:58:07.834063 illumio_pylo-0.3.6/illumio_pylo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-26 14:58:07.000000 illumio_pylo-0.3.6/illumio_pylo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-26 14:58:07.000000 illumio_pylo-0.3.6/illumio_pylo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:58:07.000000 illumio_pylo-0.3.6/illumio_pylo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 14:58:07.000000 illumio_pylo-0.3.6/illumio_pylo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 14:58:07.000000 illumio_pylo-0.3.6/illumio_pylo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:58:07.838063 illumio_pylo-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-26 14:57:59.000000 illumio_pylo-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.050203 illumio_pylo-0.3.7/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.046203 illumio_pylo-0.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.050203 illumio_pylo-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.github/workflows/doxygen-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.github/workflows/make-binaries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.054203 illumio_pylo-0.3.7/dev_playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/check_unique_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/check_unique_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/delete_all_workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/delete_unused_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/explorer_report_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/export_rules_to_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/generate-random-workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/healthcheck_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/import-labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/import_workloads_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/iplists_stats_duplicates_unused_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/recalculate_explorer_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/recalculate_explorer_logs_multithreaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/rules_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/rules_exporter_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/test_change_workload_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/test_query2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/test_securityprincipals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/ven_idle_to_illumination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/dev_playground/ven_reassign_pce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.054203 illumio_pylo-0.3.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/examples/explorer_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/examples/extend_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.058203 illumio_pylo-0.3.7/illumio_pylo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.062203 illumio_pylo-0.3.7/illumio_pylo/API/
+-rw-r--r--   0 runner    (1001) docker     (127)    60725 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/APIConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/AuditLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/ClusterHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/CredentialsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/Explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/JsonPayloadTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/RuleSearchQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/AgentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.062203 illumio_pylo-0.3.7/illumio_pylo/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21898 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Helpers/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/IPList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/IPMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/LabelCommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/LabelGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/LabelStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/LabeledObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/ReferenceTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/RulesetStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/SecurityPrincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/SoftwareVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/VirtualService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/VirtualServiceStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/Workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/WorkloadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/WorkloadStoreSubClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.062203 illumio_pylo-0.3.7/illumio_pylo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/NativeParsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.062203 illumio_pylo-0.3.7/illumio_pylo/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/iplist_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/iplist_import_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/ruleset_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/update_pce_objects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/LabelCreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_compatibility_report_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19580 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_duplicate_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_idle_to_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18923 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_reset_names_to_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28543 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/illumio_pylo/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/docs/Doxygen
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/illumio_pylo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/credentials.example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/health_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/iplists-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/iplists-import-example.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/workloads-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/illumio_pylo/utilities/resources/workloads-import-example.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/illumio_pylo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-05-31 16:07:13.000000 illumio_pylo-0.3.7/illumio_pylo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-31 16:07:13.000000 illumio_pylo-0.3.7/illumio_pylo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:07:13.000000 illumio_pylo-0.3.7/illumio_pylo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 16:07:13.000000 illumio_pylo-0.3.7/illumio_pylo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 16:07:13.000000 illumio_pylo-0.3.7/illumio_pylo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:07:13.066203 illumio_pylo-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-31 16:07:06.000000 illumio_pylo-0.3.7/setup.py
```

### Comparing `illumio_pylo-0.3.6/.devcontainer/devcontainer.json` & `illumio_pylo-0.3.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/.github/workflows/doxygen-publish.yml` & `illumio_pylo-0.3.7/.github/workflows/doxygen-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/.github/workflows/make-binaries.yml` & `illumio_pylo-0.3.7/.github/workflows/make-binaries.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/.github/workflows/python-publish.yml` & `illumio_pylo-0.3.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/LICENSE` & `illumio_pylo-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/PKG-INFO` & `illumio_pylo-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.6
+Version: 0.3.7
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.6/README.md` & `illumio_pylo-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/check_unique_hostnames.py` & `illumio_pylo-0.3.7/dev_playground/check_unique_hostnames.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/check_unique_services.py` & `illumio_pylo-0.3.7/dev_playground/check_unique_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/delete_all_workloads.py` & `illumio_pylo-0.3.7/dev_playground/delete_all_workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/delete_unused_services.py` & `illumio_pylo-0.3.7/dev_playground/delete_unused_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/explorer_report_exporter.py` & `illumio_pylo-0.3.7/dev_playground/explorer_report_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/export_rules_to_firewall.py` & `illumio_pylo-0.3.7/dev_playground/export_rules_to_firewall.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/generate-random-workloads.py` & `illumio_pylo-0.3.7/dev_playground/generate-random-workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/healthcheck_log.py` & `illumio_pylo-0.3.7/dev_playground/healthcheck_log.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/import-labels.py` & `illumio_pylo-0.3.7/dev_playground/import-labels.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/import_workloads_placeholders.py` & `illumio_pylo-0.3.7/dev_playground/import_workloads_placeholders.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/iplists_stats_duplicates_unused_finder.py` & `illumio_pylo-0.3.7/dev_playground/iplists_stats_duplicates_unused_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/recalculate_explorer_logs.py` & `illumio_pylo-0.3.7/dev_playground/recalculate_explorer_logs.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/recalculate_explorer_logs_multithreaded.py` & `illumio_pylo-0.3.7/dev_playground/recalculate_explorer_logs_multithreaded.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/rules_exporter.py` & `illumio_pylo-0.3.7/dev_playground/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/rules_exporter_special.py` & `illumio_pylo-0.3.7/dev_playground/rules_exporter_special.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/test.py` & `illumio_pylo-0.3.7/dev_playground/test.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/test_change_workload_desc.py` & `illumio_pylo-0.3.7/dev_playground/test_change_workload_desc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/test_query.py` & `illumio_pylo-0.3.7/dev_playground/test_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/test_query2.py` & `illumio_pylo-0.3.7/dev_playground/test_query2.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/test_securityprincipals.py` & `illumio_pylo-0.3.7/dev_playground/test_securityprincipals.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/ven_idle_to_illumination.py` & `illumio_pylo-0.3.7/dev_playground/ven_idle_to_illumination.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/dev_playground/ven_reassign_pce.py` & `illumio_pylo-0.3.7/dev_playground/ven_reassign_pce.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/examples/explorer_query.py` & `illumio_pylo-0.3.7/examples/explorer_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/examples/extend_cli.py` & `illumio_pylo-0.3.7/examples/extend_cli.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/APIConnector.py` & `illumio_pylo-0.3.7/illumio_pylo/API/APIConnector.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/AuditLog.py` & `illumio_pylo-0.3.7/illumio_pylo/API/AuditLog.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/ClusterHealth.py` & `illumio_pylo-0.3.7/illumio_pylo/API/ClusterHealth.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/CredentialsManager.py` & `illumio_pylo-0.3.7/illumio_pylo/API/CredentialsManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         self.api_key = api_key
         self.org_id = org_id
         self.verify_ssl = verify_ssl
         self.originating_file = originating_file
 
         self.raw_json: Optional[CredentialFileEntry] = None
 
-
     @staticmethod
     def from_credentials_file_entry(credential_file_entry: CredentialFileEntry, originating_file: Optional[str] = None):
         return CredentialProfile(credential_file_entry['name'],
                                  credential_file_entry['fqdn'],
                                  credential_file_entry['port'],
                                  credential_file_entry['api_user'],
                                  credential_file_entry['api_key'],
@@ -299,7 +298,29 @@
 
 def find_ssh_key_from_fingerprint(fingerprint: bytes) -> Optional[paramiko.AgentKey]:
     keys = paramiko.Agent().get_keys()
     for key in keys:
         if key.get_fingerprint() == fingerprint:
             return key
     return None
+
+
+def get_supported_keys_from_ssh_agent() -> list[paramiko.AgentKey]:
+    keys = paramiko.Agent().get_keys()
+    # filter out ECDSA NISTPXXX and sk-ssh-ed25519
+    # RSA and ED25519 keys are reported to be working
+    return [key for key in keys if not (key.get_name().startswith("ecdsa-sha2-nistp") or
+                                        key.get_name().startswith("sk-ssh-ed25519"))]
+
+
+def is_encryption_available() -> bool:
+    if paramiko is None:
+        return False
+
+    # does paramiko have an agent module and does it have any supported key?
+    if hasattr(paramiko, 'Agent'):
+        keys = get_supported_keys_from_ssh_agent()
+        return len(keys) > 0
+
+    return False
+
+
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/Explorer.py` & `illumio_pylo-0.3.7/illumio_pylo/API/Explorer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/JsonPayloadTypes.py` & `illumio_pylo-0.3.7/illumio_pylo/API/JsonPayloadTypes.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/API/RuleSearchQuery.py` & `illumio_pylo-0.3.7/illumio_pylo/API/RuleSearchQuery.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/AgentStore.py` & `illumio_pylo-0.3.7/illumio_pylo/AgentStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Exception.py` & `illumio_pylo-0.3.7/illumio_pylo/Exception.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Helpers/exports.py` & `illumio_pylo-0.3.7/illumio_pylo/Helpers/exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
 
             for row_count in range(1, source_worksheet.max_row+1):
                 # this is Headers
                 if row_count == 1:
                     for col_index in range(1, source_worksheet.max_column+1):
                         item = source_worksheet.cell(row_count, col_index).value
                         if item is None or len(item) < 1:
-                            raise pylo.PyloEx('Excel headers has blank fields, this is not supported')
+                            raise pylo.PyloEx('Excel headers has blank field at column #{}'.format(col_index))
                         self._detected_headers.append(item.lower())
                         if strict_headers and item.lower() not in mandatory_headers_dict:
                             raise pylo.PyloEx("CSV/Excel headers have an unexpected header named '{}'".format(item))
 
                     missing_headers = mandatory_headers_dict.copy()
                     for header_name in self._detected_headers:
                         self._header_index_to_name.append(header_name)
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Helpers/functions.py` & `illumio_pylo-0.3.7/illumio_pylo/Helpers/functions.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/IPList.py` & `illumio_pylo-0.3.7/illumio_pylo/IPList.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/IPMap.py` & `illumio_pylo-0.3.7/illumio_pylo/IPMap.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Label.py` & `illumio_pylo-0.3.7/illumio_pylo/Label.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/LabelCommon.py` & `illumio_pylo-0.3.7/illumio_pylo/LabelCommon.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/LabelGroup.py` & `illumio_pylo-0.3.7/illumio_pylo/LabelGroup.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/LabelStore.py` & `illumio_pylo-0.3.7/illumio_pylo/LabelStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/LabeledObject.py` & `illumio_pylo-0.3.7/illumio_pylo/LabeledObject.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Organization.py` & `illumio_pylo-0.3.7/illumio_pylo/Organization.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Query.py` & `illumio_pylo-0.3.7/illumio_pylo/Query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/ReferenceTracker.py` & `illumio_pylo-0.3.7/illumio_pylo/ReferenceTracker.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Rule.py` & `illumio_pylo-0.3.7/illumio_pylo/Rule.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Ruleset.py` & `illumio_pylo-0.3.7/illumio_pylo/Ruleset.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/RulesetStore.py` & `illumio_pylo-0.3.7/illumio_pylo/RulesetStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/SecurityPrincipal.py` & `illumio_pylo-0.3.7/illumio_pylo/SecurityPrincipal.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Service.py` & `illumio_pylo-0.3.7/illumio_pylo/Service.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/SoftwareVersion.py` & `illumio_pylo-0.3.7/illumio_pylo/SoftwareVersion.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/VirtualService.py` & `illumio_pylo-0.3.7/illumio_pylo/VirtualService.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/VirtualServiceStore.py` & `illumio_pylo-0.3.7/illumio_pylo/VirtualServiceStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/Workload.py` & `illumio_pylo-0.3.7/illumio_pylo/Workload.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/WorkloadStore.py` & `illumio_pylo-0.3.7/illumio_pylo/WorkloadStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/WorkloadStoreSubClasses.py` & `illumio_pylo-0.3.7/illumio_pylo/WorkloadStoreSubClasses.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/__init__.py` & `illumio_pylo-0.3.7/illumio_pylo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 from typing import Callable
 
 from .tmp import *
 from .Helpers import *
 
 from .Exception import PyloEx, PyloApiEx, PyloApiTooManyRequestsEx, PyloApiUnexpectedSyntax, PyloObjectNotFound, PyloApiRequestForbiddenEx
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/NativeParsers.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/NativeParsers.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/__init__.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,13 +147,13 @@
         commands.available_commands[selected_command.name].main(args, org=org, config_data=config_data, connector=connector, pce_cache_was_used=settings_use_cache)
 
     print()
     cli_end_time = datetime.datetime.now()
     print("**** END OF {} UTILITY ****".format(selected_command.name.upper()))
     print("Command Specific Execution time: {:.2f} seconds".format(time.perf_counter() - command_execution_time_start))
     print("CLI started at {} and finished at {}".format(cli_start_time, cli_end_time))
-    print("CLI Total Execution time: {}".format(cli_end_time - cli_start_time))
+    print("CLI Total Execution time: {}".format((cli_end_time - cli_start_time)))
     print()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/__init__.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/credential_manager.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/credential_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import os
 
 import paramiko
 
 import illumio_pylo as pylo
 import click
 from illumio_pylo.API.CredentialsManager import get_all_credentials, create_credential_in_file, CredentialFileEntry, \
-    create_credential_in_default_file,  \
+    create_credential_in_default_file, \
     get_credentials_from_file, encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305, \
-    decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305, decrypt_api_key_with_paramiko_ssh_key_fernet
+    decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305, get_supported_keys_from_ssh_agent, is_encryption_available
 
 from illumio_pylo import log
 from . import Command
 
 
 command_name = "cred-manager"
 objects_load_filter = None
@@ -113,40 +113,41 @@
             "port": wanted_port,
             "org_id": wanted_org,
             "api_user": wanted_api_user,
             "verify_ssl": wanted_verify_ssl,
             "api_key": api_key
         }
 
-        encrypt_api_key = click.prompt('> Encrypt API (requires an SSH agent running and an RSA or Ed25519 key) ? Y/N', type=bool)
-        if encrypt_api_key:
-            print("Available keys (ECDSA NISTPXXX keys and a few others are not supported and will be filtered out):")
-            ssh_keys = paramiko.Agent().get_keys()
-            # filter out ECDSA NISTPXXX and sk-ssh-ed25519@openssh.com
-            ssh_keys = get_supported_keys_from_ssh_agent()
-
-            # display a table of keys
-            print_keys(keys=ssh_keys, display_index=True)
-            print()
-
-            index_of_selected_key = click.prompt('> Select key by ID#', type=click.IntRange(0, len(ssh_keys)-1))
-            selected_ssh_key = ssh_keys[index_of_selected_key]
-            print("Selected key: {} | {} | {}".format(selected_ssh_key.get_name(),
-                                                      selected_ssh_key.get_fingerprint().hex(),
-                                                      selected_ssh_key.comment))
-            print(" * encrypting API key with selected key (you may be prompted by your SSH agent for confirmation or PIN code) ...", flush=True, end="")
-            # encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_fernet(ssh_key=selected_ssh_key, api_key=api_key)
-            encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(ssh_key=selected_ssh_key, api_key=api_key)
-            print("OK!")
-            print(" * trying to decrypt the encrypted API key...", flush=True, end="")
-            decrypted_api_key = decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(encrypted_api_key_payload=encrypted_api_key)
-            if decrypted_api_key != api_key:
-                raise pylo.PyloEx("Decrypted API key does not match original API key")
-            print("OK!")
-            credentials_data["api_key"] = encrypted_api_key
+        if is_encryption_available():
+            encrypt_api_key = click.prompt('> Encrypt API (requires an SSH agent running and an RSA or Ed25519 key added to them) ? Y/N', type=bool)
+            if encrypt_api_key:
+                print("Available keys (ECDSA NISTPXXX keys and a few others are not supported and will be filtered out):")
+                ssh_keys = get_supported_keys_from_ssh_agent()
+
+                # display a table of keys
+                print_keys(keys=ssh_keys, display_index=True)
+                print()
+
+                index_of_selected_key = click.prompt('> Select key by ID#', type=click.IntRange(0, len(ssh_keys)-1))
+                selected_ssh_key = ssh_keys[index_of_selected_key]
+                print("Selected key: {} | {} | {}".format(selected_ssh_key.get_name(),
+                                                          selected_ssh_key.get_fingerprint().hex(),
+                                                          selected_ssh_key.comment))
+                print(" * encrypting API key with selected key (you may be prompted by your SSH agent for confirmation or PIN code) ...", flush=True, end="")
+                # encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_fernet(ssh_key=selected_ssh_key, api_key=api_key)
+                encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(ssh_key=selected_ssh_key, api_key=api_key)
+                print("OK!")
+                print(" * trying to decrypt the encrypted API key...", flush=True, end="")
+                decrypted_api_key = decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(encrypted_api_key_payload=encrypted_api_key)
+                if decrypted_api_key != api_key:
+                    raise pylo.PyloEx("Decrypted API key does not match original API key")
+                print("OK!")
+                credentials_data["api_key"] = encrypted_api_key
+        else:
+            print(" * encryption is not available (no SSH agent or compatible key found), storing API key in plain text...")
 
 
         cwd = os.getcwd()
         create_in_current_workdir = click.prompt('> Create in current workdir ({})? If not then user homedir will be used.   Y/N '.format(cwd), type=bool)
 
 
         print("* Creating credential...", flush=True, end="")
@@ -183,23 +184,17 @@
         connector = pylo.APIConnector.create_from_credentials_object(found_profile)
         connector.objects_label_dimension_get()
         print("OK!")
 
     else:
         raise pylo.PyloEx("Unknown sub-command '{}'".format(args['sub_command']))
 
-command_object = Command(command_name, __main, fill_parser, credentials_manager_mode=True)
 
+command_object = Command(command_name, __main, fill_parser, credentials_manager_mode=True)
 
-def get_supported_keys_from_ssh_agent() -> list[paramiko.AgentKey]:
-    keys = paramiko.Agent().get_keys()
-    # filter out ECDSA NISTPXXX and sk-ssh-ed25519
-    # RSA and ED25519 keys are reported to be working
-    return [key for key in keys if not (key.get_name().startswith("ecdsa-sha2-nistp") or
-                                        key.get_name().startswith("sk-ssh-ed25519"))]
 
 def print_keys(keys: list[paramiko.AgentKey], display_index = True) -> None:
 
     args_for_print = []
 
     column_properties = [  # (name, width)
         ("ID#", 4),
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/iplist_analyzer.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/iplist_analyzer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/iplist_import_from_file.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/iplist_import_from_file.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/ruleset_export.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/ruleset_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,29 +21,26 @@
                         "R-WEB" + os.linesep +
                         "A-FUSION" + os.linesep +
                         "IPLISTS: " + os.linesep +
                         "Private_Networks" + os.linesep +
                         "Public_NATed")
 
 
-
 def __main(args: Dict, org: pylo.Organization, **kwargs):
 
     setting_prefix_objects_with_type: bool|str = args['prefix_objects_with_type']
     setting_object_types_as_section: bool = args['prefix_objects_with_type']
     settings_output_file_format = args['format']
     settings_output_dir = args['output_dir']
 
-
     if setting_prefix_objects_with_type is False:
         print(" * Prefix for object types are disabled")
     else:
         print(" * Prefix for object types are enabled")
 
-
     if setting_object_types_as_section is False:
         print(" * Object types as section are disabled")
     else:
         print(" * Object types as section are enabled")
 
     csv_report, output_file_name, sheet = prepare_csv_report_object(settings_output_file_format, settings_output_dir)
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/update_pce_objects_cache.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/update_pce_objects_cache.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/LabelCreation.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/LabelCreation.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/utils/misc.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/utils/misc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_compatibility_report_export.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_compatibility_report_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_duplicate_remover.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_duplicate_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,14 +284,15 @@
     else:
         print("\n** WARNING: no entry matched your filters so reports were not generated !\n")
 
 
 # make this command available to the CLI system
 command_object = Command(command_name, __main, fill_parser, objects_load_filter)
 
+
 class DuplicateRecordManager:
     class DuplicatedRecord:
         def __init__(self, pce_offline_timer_override: Optional[int] = None):
             self.offline = []
             self.online = []
             self.unmanaged= []
             self.all: List[pylo.Workload] = []
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_idle_to_visibility.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_idle_to_visibility.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/ven_upgrader.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/ven_upgrader.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_export.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_import.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,16 +279,16 @@
                         print(
                             "  - WARNING: CSV has an entry for workload name '{}' at line #{} but it exists already in the PCE. It will be ignored.".format(
                             lower_name, csv_object['*line*']))
 
         if csv_object['hostname'] is not None and len(csv_object['hostname']) > 0:
             lower_hostname = csv_object['hostname'].lower()
             if lower_name != lower_hostname:
-                if csv_object['hostname'] not in name_cache:
-                    name_cache[csv_object['hostname']] = WorkloadCollisionItem(from_pce=False, csv_object=csv_object,
+                if lower_hostname not in name_cache:
+                    name_cache[lower_hostname] = WorkloadCollisionItem(from_pce=False, csv_object=csv_object,
                                                                                managed=False)
                 else:
                     if not name_cache[lower_hostname].from_pce:
                         raise pylo.PyloEx('CSV contains workloads with duplicates name/hostname: {}'.format(lower_name))
                     else:
                         if not ignore_all_sorts_collisions and not ignore_hostname_collision:
                             csv_object['**not_created_reason**'] = 'Found duplicated name/hostname in PCE'
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_reset_names_to_null.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_reset_names_to_null.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_update.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     csv_input_object = pylo.CsvExcelToObject(settings_input_file, expected_headers=csv_expected_fields, csv_delimiter=settings_input_file_delimiter)
     for label_type in org.LabelStore.label_types:
         if f'{context.settings_label_type_header_prefix}{label_type}' not in csv_input_object.headers():
             context.csv_input_missing_label_types.append(label_type)
 
     print('OK')
     print("   - CSV has {} columns and {} lines (headers don't count)".format(csv_input_object.count_columns(), csv_input_object.count_lines()))
+    context.csv_data = csv_input_object.objects()
     # </editor-fold desc="CSV input file data extraction">
 
 
     if not input_match_on_ip and not input_match_on_hostname and not input_match_on_href:
         pylo.log.error('You must specify at least one (or several) property to match on for workloads vs input: href, ip or hostname')
         sys.exit(1)
 
@@ -303,15 +304,15 @@
                       flush=True)
 
             if len(csv_data['**ip_array**']) < 1:
                 print("   - ERROR: CSV line #{} has no valid IP address defined".format(csv_data['*line*']), flush=True)
     if input_match_on_hostname:
         for csv_data in context.csv_data:
             name = csv_data['hostname']
-            name = pylo.Workload.static_name_stripped_fqdn(name)
+            name = pylo.Workload.static_name_stripped_fqdn(name).lower()
             if name is None or len(name) < 1:
                 print("   - ERROR: CSV line #{} has invalid hostname defined: '{}'".format(csv_data['*line*'],
                                                                                            csv_data['hostname']),
                       flush=True)
                 csv_check_failed_count += 1
                 continue
 
@@ -328,25 +329,26 @@
             if href is None or len(href) < 1:
                 print("   - ERROR: CSV line #{} has invalid href defined: '{}'".format(csv_data['*line*'],
                                                                                        csv_data['href']), flush=True)
                 csv_check_failed_count += 1
                 continue
 
             if href not in context.csv_href_index:
-                context.csv_name_index[href] = csv_data
+                context.csv_href_index[href] = csv_data
                 continue
 
             print("   - ERROR: CSV line #{} has duplicate href defined from a previous line: '{}'".format(
                 csv_data['*line*'], csv_data['href']), flush=True)
             csv_check_failed_count += 1
     if csv_check_failed_count > 0:
         pylo.log.error(
             "ERROR! Several ({}) inconsistencies were found in the CSV, please fix them before you continue!".format(
                 csv_check_failed_count))
         sys.exit(1)
+
     print("   * Done")
 
 
 def match_pce_workloads_vs_csv(context: ContextSingleton,
                                match_on_hostname, match_on_href, match_on_ip,
                                workloads_to_relabel) -> Dict[pylo.Workload, Dict]:
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo/cli/commands/workload_used_in_rule_finder.py` & `illumio_pylo-0.3.7/illumio_pylo/cli/commands/workload_used_in_rule_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/docs/Doxygen` & `illumio_pylo-0.3.7/illumio_pylo/docs/Doxygen`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/tmp.py` & `illumio_pylo-0.3.7/illumio_pylo/tmp.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/utilities/health_monitoring.py` & `illumio_pylo-0.3.7/illumio_pylo/utilities/health_monitoring.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/utilities/resources/iplists-import-example.xlsx` & `illumio_pylo-0.3.7/illumio_pylo/utilities/resources/iplists-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo/utilities/resources/workloads-import-example.xlsx` & `illumio_pylo-0.3.7/illumio_pylo/utilities/resources/workloads-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/illumio_pylo.egg-info/PKG-INFO` & `illumio_pylo-0.3.7/illumio_pylo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.6
+Version: 0.3.7
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.6/illumio_pylo.egg-info/SOURCES.txt` & `illumio_pylo-0.3.7/illumio_pylo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/pyproject.toml` & `illumio_pylo-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.6/setup.py` & `illumio_pylo-0.3.7/setup.py`

 * *Files identical despite different names*

