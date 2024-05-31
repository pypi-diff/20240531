# Comparing `tmp/resc_backend-3.3.2.tar.gz` & `tmp/resc_backend-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.3.2.tar", last modified: Tue May 28 14:31:53 2024, max compression
+gzip compressed data, was "resc_backend-3.3.3.tar", last modified: Fri May 31 11:43:36 2024, max compression
```

## Comparing `resc_backend-3.3.2.tar` & `resc_backend-3.3.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.777187 resc_backend-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 14:31:49.000000 resc_backend-3.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-28 14:31:53.777187 resc_backend-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-28 14:31:49.000000 resc_backend-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-28 14:31:49.000000 resc_backend-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 14:31:49.000000 resc_backend-3.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-28 14:31:53.777187 resc_backend-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 14:31:49.000000 resc_backend-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.757187 resc_backend-3.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.761187 resc_backend-3.3.2/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.761187 resc_backend-3.3.2/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.761187 resc_backend-3.3.2/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.765187 resc_backend-3.3.2/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.765187 resc_backend-3.3.2/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/list_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.765187 resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.765187 resc_backend-3.3.2/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.769187 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    37721 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.769187 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.773187 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/toml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.777187 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.777187 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-28 14:31:49.000000 resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:31:53.777187 resc_backend-3.3.2/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:31:53.000000 resc_backend-3.3.2/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.819855 resc_backend-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 11:43:32.000000 resc_backend-3.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-31 11:43:36.819855 resc_backend-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-31 11:43:32.000000 resc_backend-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-31 11:43:32.000000 resc_backend-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-31 11:43:32.000000 resc_backend-3.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 11:43:36.819855 resc_backend-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 11:43:32.000000 resc_backend-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.799855 resc_backend-3.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.803855 resc_backend-3.3.3/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.803855 resc_backend-3.3.3/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.803855 resc_backend-3.3.3/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.807855 resc_backend-3.3.3/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.807855 resc_backend-3.3.3/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/list_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.807855 resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.807855 resc_backend-3.3.3/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.811855 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38433 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.811855 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.811855 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/toml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.815855 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.819855 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 11:43:32.000000 resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:43:36.819855 resc_backend-3.3.3/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 11:43:36.000000 resc_backend-3.3.3/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.3.2/LICENSE.md` & `resc_backend-3.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/PKG-INFO` & `resc_backend-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.3.2
+Version: 3.3.3
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.3.2/README.md` & `resc_backend-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/pyproject.toml` & `resc_backend-3.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-3.3.3/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/common.py` & `resc_backend-3.3.3/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/constants.py` & `resc_backend-3.3.3/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/connection.py` & `resc_backend-3.3.3/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/engine_azure.py` & `resc_backend-3.3.3/src/resc_backend/db/engine_azure.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/__init__.py` & `resc_backend-3.3.3/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/audit.py` & `resc_backend-3.3.3/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/finding.py` & `resc_backend-3.3.3/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/repository.py` & `resc_backend-3.3.3/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/rule.py` & `resc_backend-3.3.3/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-3.3.3/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/rule_pack.py` & `resc_backend-3.3.3/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/scan.py` & `resc_backend-3.3.3/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-3.3.3/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-3.3.3/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-3.3.3/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-3.3.3/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/api.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/api.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Standard Library
 import logging
 from datetime import datetime, timedelta, UTC
 
 # Third Party
-from sqlalchemy import extract, func, select, union
+from sqlalchemy import Column, extract, func, select, union
 from sqlalchemy.engine import Row
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.query import Query
 from sqlalchemy.sql.expression import literal_column
 
 # First Party
 from resc_backend.constants import (
@@ -277,15 +277,15 @@
     sub_query = sub_query.where(DBscanFinding.scan_id == scan.id_)
     sub_query = sub_query.subquery()
     query = query.where(DBfinding.id_.not_in(sub_query))
 
     return db_connection.execute(query).scalars().all()
 
 
-def get_untriaged_finding_outdated_for_current_rule_pack(db_connection: Session, scan: DBscan) -> list[int]:
+def get_untriaged_finding_outdated_for_current_scan(db_connection: Session, scan: DBscan) -> list[int]:
     """
     Retrieve all the findings which are:
      - tied to the repository of the scan
      - where the rule is not in the rule pack of the scan
      - which are not analyzed
 
     Args:
@@ -914,15 +914,15 @@
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
     return count_over_time
 
 
-def get_un_triaged_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_untriaged_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
     """
         Retrieve count of un triaged findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
@@ -963,7 +963,22 @@
         query = query.group_by(DBVcsInstance.provider_type)
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
     return count_over_time
+
+
+def query_untriaged_findings_for_rule_pack(query: Query, version: str | Column[str]) -> Query:
+    query = query.join(DBfinding, DBfinding.id_ == DBscanFinding.finding_id)
+    query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+    query = query.join(DBrule, DBrule.rule_name == DBfinding.rule_name)
+    query = query.join(
+        DBaudit,
+        (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
+        isouter=True,
+    )
+    query = query.where(DBrule.rule_pack == version)
+    query = query.where(DBscan.rule_pack == version)
+    query = query.where((DBaudit.status == FindingStatus.NOT_ANALYZED) | (DBaudit.status == None))  # noqa: E711
+    return query
```

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Standard Library
 import logging
 
 # Third Party
 from packaging.version import Version
-from sqlalchemy import func, update
+from sqlalchemy import func, update, case, literal_column
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.query import Query
-from sqlalchemy.sql.expression import true
 
 # First Party
 from resc_backend.constants import (
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     MAX_RECORDS_PER_PAGE_LIMIT,
 )
-from resc_backend.db.model import DBrule, DBrulePack, DBruleTag, DBtag
+from resc_backend.db.model import DBscanFinding, DBrule, DBrulePack, DBruleTag, DBtag
 from resc_backend.resc_web_service.schema import rule_pack as rule_pack_schema
+from resc_backend.resc_web_service.crud.finding import query_untriaged_findings_for_rule_pack
 
 logger = logging.getLogger(__name__)
 
 
 def get_rule_pack(db_connection: Session, version: str | None) -> rule_pack_schema.RulePackRead:
     """
         Get active rule pack from database
@@ -30,15 +30,15 @@
         The output returns RulePackRead type object
     """
     query = db_connection.query(DBrulePack)
     if version:
         query = query.where(DBrulePack.version == version)
     else:
         logger.debug("rule pack version not specified, fetching currently active one")
-        query = query.where(DBrulePack.active == true())
+        query = query.where(DBrulePack.active == True)  # noqa: E712
     rule_pack = query.first()
     return rule_pack
 
 
 def create_rule_pack_version(db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate):
     """
         Create rule pack version in database
@@ -96,16 +96,24 @@
     :param limit:
         integer amount of records to return, to support pagination
     :return: [RulePackRead]
         The output will contain a PaginationModel containing the list of RulePackRead type objects,
         or an empty list if no rule pack was found
     """
     limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    query = db_connection.query(DBrulePack)
 
+    outdated_stmt = db_connection.query(
+        case((func.count(DBscanFinding.finding_id) == 0, literal_column("'1'")), else_=literal_column("'0'"))
+    )
+    outdated_stmt = query_untriaged_findings_for_rule_pack(outdated_stmt, DBrulePack.version)
+    outdated_stmt = outdated_stmt.label("outdated")
+
+    query: Query = db_connection.query(
+        DBrulePack.version, DBrulePack.active, DBrulePack.created, DBrulePack.global_allow_list, outdated_stmt
+    )
     if version:
         query = query.where(DBrulePack.version == version)
     if active is not None:
         query = query.where(DBrulePack.active == active)
     rule_packs = query.order_by(DBrulePack.version.desc()).offset(skip).limit(limit_val).all()
     return rule_packs
```

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         Retrieve count of UnTriaged findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
-    audit_counts = finding_crud.get_un_triaged_finding_count_by_vcs_provider_over_time(
+    audit_counts = finding_crud.get_untriaged_finding_count_by_vcs_provider_over_time(
         db_connection=db_connection, weeks=weeks
     )
     output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
     return output
 
 
 def convert_rows_to_finding_count_over_time(count_over_time: dict, weeks: int) -> list[FindingCountOverTime]:
```

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         db_connection=db_connection, scan=db_scan
     )
     audit_crud.create_automated_audit(
         db_connection=db_connection, findings_ids=findings_to_audit, status=FindingStatus.OUTDATED
     )
 
     # 8. Mark findings which are no longer in rule pack (i.e. rule name not in current rule pack) as outdated
-    old_findings_to_audit: list[int] = finding_crud.get_untriaged_finding_outdated_for_current_rule_pack(
+    old_findings_to_audit: list[int] = finding_crud.get_untriaged_finding_outdated_for_current_scan(
         db_connection=db_connection, scan=db_scan
     )
     audit_crud.create_automated_audit(
         db_connection=db_connection, findings_ids=old_findings_to_audit, status=FindingStatus.OUTDATED
     )
 
     # Clear cache related to findings
```

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/filters.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/helpers/toml.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/helpers/toml.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/finding_status.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/finding_status.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 RULE_PACK_VERSION_REGEX = r"^\d+(?:\.\d+){2}$"
 
 
 class RulePackBase(BaseModel):
     version: constr(regex=RULE_PACK_VERSION_REGEX)
     active: bool = False
     global_allow_list: conint(gt=0) | None
+    outdated: bool = False
 
 
 class RulePackCreate(RulePackBase):
     version: constr(regex=RULE_PACK_VERSION_REGEX)
     global_allow_list: conint(gt=0) | None
 
     @classmethod
```

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-3.3.3/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.2/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-3.3.3/src/resc_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.3.2
+Version: 3.3.3
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.3.2/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-3.3.3/src/resc_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

