# Comparing `tmp/pycti-6.1.6.tar.gz` & `tmp/pycti-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.6.tar", last modified: Wed May 29 17:55:53 2024, max compression
+gzip compressed data, was "pycti-6.1.7.tar", last modified: Fri May 31 11:14:13 2024, max compression
```

## Comparing `pycti-6.1.6.tar` & `pycti-6.1.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.429020 pycti-6.1.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-29 17:55:37.000000 pycti-6.1.6/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-29 17:55:53.429020 pycti-6.1.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-29 17:55:37.000000 pycti-6.1.6/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.417020 pycti-6.1.6/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.417020 pycti-6.1.6/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29701 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.417020 pycti-6.1.6/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61944 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.425020 pycti-6.1.6/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43249 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.425020 pycti-6.1.6/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   117232 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4907 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-29 17:55:37.000000 pycti-6.1.6/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 17:55:53.425020 pycti-6.1.6/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-29 17:55:53.000000 pycti-6.1.6/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-29 17:55:53.000000 pycti-6.1.6/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-29 17:55:53.000000 pycti-6.1.6/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      662 2024-05-29 17:55:53.000000 pycti-6.1.6/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-29 17:55:53.000000 pycti-6.1.6/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-29 17:55:37.000000 pycti-6.1.6/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2024-05-29 17:55:53.429020 pycti-6.1.6/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.161487 pycti-6.1.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-31 11:13:59.000000 pycti-6.1.7/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-31 11:14:13.161487 pycti-6.1.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-31 11:13:59.000000 pycti-6.1.7/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.149487 pycti-6.1.7/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.149487 pycti-6.1.7/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29701 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.149487 pycti-6.1.7/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61944 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.157487 pycti-6.1.7/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43524 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12605 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17935 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27823 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.157487 pycti-6.1.7/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   117232 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4907 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-31 11:13:59.000000 pycti-6.1.7/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 11:14:13.157487 pycti-6.1.7/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-31 11:14:13.000000 pycti-6.1.7/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-31 11:14:13.000000 pycti-6.1.7/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-31 11:14:13.000000 pycti-6.1.7/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      662 2024-05-31 11:14:13.000000 pycti-6.1.7/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-31 11:14:13.000000 pycti-6.1.7/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-31 11:13:59.000000 pycti-6.1.7/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2024-05-31 11:14:13.161487 pycti-6.1.7/setup.cfg
```

### Comparing `pycti-6.1.6/LICENSE` & `pycti-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/PKG-INFO` & `pycti-6.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.6
+Version: 6.1.7
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.6/README.md` & `pycti-6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/__init__.py` & `pycti-6.1.7/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.6"
+__version__ = "6.1.7"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.6/pycti/api/opencti_api_client.py` & `pycti-6.1.7/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/api/opencti_api_connector.py` & `pycti-6.1.7/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/api/opencti_api_playbook.py` & `pycti-6.1.7/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/api/opencti_api_work.py` & `pycti-6.1.7/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/connector/opencti_connector.py` & `pycti-6.1.7/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.7/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.7/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.7/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_campaign.py` & `pycti-6.1.7/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_case_incident.py` & `pycti-6.1.7/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.7/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_case_rft.py` & `pycti-6.1.7/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_channel.py` & `pycti-6.1.7/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.7/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_data_component.py` & `pycti-6.1.7/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_data_source.py` & `pycti-6.1.7/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_event.py` & `pycti-6.1.7/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_external_reference.py` & `pycti-6.1.7/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_feedback.py` & `pycti-6.1.7/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_grouping.py` & `pycti-6.1.7/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_identity.py` & `pycti-6.1.7/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_incident.py` & `pycti-6.1.7/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_indicator.py` & `pycti-6.1.7/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.7/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.7/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.7/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_label.py` & `pycti-6.1.7/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_language.py` & `pycti-6.1.7/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_location.py` & `pycti-6.1.7/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_malware.py` & `pycti-6.1.7/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.7/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.7/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_narrative.py` & `pycti-6.1.7/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_note.py` & `pycti-6.1.7/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_observed_data.py` & `pycti-6.1.7/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_opinion.py` & `pycti-6.1.7/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_report.py` & `pycti-6.1.7/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix.py` & `pycti-6.1.7/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.7/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.7/pycti/entities/opencti_stix_core_relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,14 +517,15 @@
         from_id = kwargs.get("fromId", None)
         to_id = kwargs.get("toId", None)
         relationship_type = kwargs.get("relationship_type", None)
         start_time_start = kwargs.get("startTimeStart", None)
         start_time_stop = kwargs.get("startTimeStop", None)
         stop_time_start = kwargs.get("stopTimeStart", None)
         stop_time_stop = kwargs.get("stopTimeStop", None)
+        filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
             self.opencti.app_logger.info("Reading stix_core_relationship", {"id": id})
             query = (
                 """
                     query StixCoreRelationship($id: String!) {
                         stixCoreRelationship(id: $id) {
@@ -539,14 +540,20 @@
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
                 result["data"]["stixCoreRelationship"]
             )
+        elif filters is not None:
+            result = self.list(filters=filters, customAttributes=custom_attributes)
+            if len(result) > 0:
+                return result[0]
+            else:
+                return None
         elif from_id is not None and to_id is not None:
             result = self.list(
                 fromOrToId=from_or_to_id,
                 fromId=from_id,
                 toId=to_id,
                 relationship_type=relationship_type,
                 startTimeStart=start_time_start,
```

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.7/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.7/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.7/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         to_id = kwargs.get("toId", None)
         relationship_type = kwargs.get("relationship_type", None)
         start_time_start = kwargs.get("startTimeStart", None)
         start_time_stop = kwargs.get("startTimeStop", None)
         stop_time_start = kwargs.get("stopTimeStart", None)
         stop_time_stop = kwargs.get("stopTimeStop", None)
         custom_attributes = kwargs.get("customAttributes", None)
+        filters = kwargs.get("filters", None)
         if id is not None:
             self.opencti.app_logger.info(
                 "Reading stix_observable_relationship", {"id": id}
             )
             query = (
                 """
                 query StixRefRelationship($id: String!) {
@@ -197,14 +198,20 @@
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
                 result["data"]["stixRefRelationship"]
             )
+        elif filters is not None:
+            result = self.list(filters=filters, customAttributes=custom_attributes)
+            if len(result) > 0:
+                return result[0]
+            else:
+                return None
         else:
             result = self.list(
                 fromOrToId=from_or_to_id,
                 fromId=from_id,
                 toId=to_id,
                 relationship_type=relationship_type,
                 startTimeStart=start_time_start,
```

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.7/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,14 +477,15 @@
         :param id: the id of the StixObjectOrStixRelationship
         :return StixObjectOrStixRelationship object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         custom_attributes = kwargs.get("customAttributes", None)
+        filters = kwargs.get("filters", None)
         if id is not None:
             self.opencti.app_logger.info(
                 "Reading StixObjectOrStixRelationship", {"id": id}
             )
             query = (
                 """
                     query StixObjectOrStixRelationship($id: String!) {
@@ -500,14 +501,20 @@
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
                 result["data"]["stixObjectOrStixRelationship"]
             )
+        elif filters is not None:
+            result = self.list(filters=filters)
+            if len(result) > 0:
+                return result[0]
+            else:
+                return None
         else:
             self.opencti.app_logger.error("Missing parameters: id")
             return None
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
```

### Comparing `pycti-6.1.6/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.7/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,15 @@
         from_id = kwargs.get("fromId", None)
         to_id = kwargs.get("toId", None)
         first_seen_start = kwargs.get("firstSeenStart", None)
         first_seen_stop = kwargs.get("firstSeenStop", None)
         last_seen_start = kwargs.get("lastSeenStart", None)
         last_seen_stop = kwargs.get("lastSeenStop", None)
         custom_attributes = kwargs.get("customAttributes", None)
+        filters = kwargs.get("filters", None)
         if id is not None:
             self.opencti.app_logger.info("Reading stix_sighting", {"id": id})
             query = (
                 """
                     query StixSightingRelationship($id: String!) {
                         stixSightingRelationship(id: $id) {
                             """
@@ -448,14 +449,20 @@
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
                 result["data"]["stixSightingRelationship"]
             )
+        elif filters is not None:
+            result = self.list(filters=filters)
+            if len(result) > 0:
+                return result[0]
+            else:
+                return None
         elif from_id is not None and to_id is not None:
             result = self.list(
                 fromOrToId=from_or_to_id,
                 fromId=from_id,
                 toId=to_id,
                 firstSeenStart=first_seen_start,
                 firstSeenStop=first_seen_stop,
```

### Comparing `pycti-6.1.6/pycti/entities/opencti_task.py` & `pycti-6.1.7/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.7/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.7/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.7/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_tool.py` & `pycti-6.1.7/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.7/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.7/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/constants.py` & `pycti-6.1.7/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/opencti_logger.py` & `pycti-6.1.7/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/opencti_stix2.py` & `pycti-6.1.7/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.7/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.7/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.7/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti.egg-info/PKG-INFO` & `pycti-6.1.7/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.6
+Version: 6.1.7
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.6/pycti.egg-info/SOURCES.txt` & `pycti-6.1.7/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pycti.egg-info/requires.txt` & `pycti-6.1.7/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/pyproject.toml` & `pycti-6.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.6/setup.cfg` & `pycti-6.1.7/setup.cfg`

 * *Files identical despite different names*

