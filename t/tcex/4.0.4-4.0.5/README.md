# Comparing `tmp/tcex-4.0.4.tar.gz` & `tmp/tcex-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcex-4.0.4.tar", last modified: Thu Mar 14 18:04:52 2024, max compression
+gzip compressed data, was "tcex-4.0.5.tar", last modified: Wed Apr 10 20:12:16 2024, max compression
```

## Comparing `tcex-4.0.4.tar` & `tcex-4.0.5.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.105247 tcex-4.0.4/
--rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2023-04-01 00:56:12.000000 tcex-4.0.4/LICENSE
--rw-r--r--   0 bsummers   (503) staff       (20)     4029 2024-03-14 18:04:52.104463 tcex-4.0.4/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)     2011 2023-07-26 23:39:14.000000 tcex-4.0.4/README.md
--rw-rw-r--   0 bsummers   (503) staff       (20)     6735 2024-03-14 17:51:53.000000 tcex-4.0.4/pyproject.toml
--rw-rw-r--   0 bsummers   (503) staff       (20)       38 2024-03-14 18:04:52.105435 tcex-4.0.4/setup.cfg
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.857624 tcex-4.0.4/tcex/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1189 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)       78 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/__metadata__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.862949 tcex-4.0.4/tcex/api/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      726 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/api.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.864264 tcex-4.0.4/tcex/api/tc/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2185 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/tc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.866612 tcex-4.0.4/tcex/api/tc/ti_transform/
--rw-rw-r--   0 bsummers   (503) staff       (20)      162 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/ti_transform/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      179 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/ti_transform/formatter.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.867648 tcex-4.0.4/tcex/api/tc/ti_transform/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      613 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/ti_transform/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7825 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/ti_transform/model/transform_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6246 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/ti_transform/ti_transform.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    26321 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/ti_transform/transform_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.868684 tcex-4.0.4/tcex/api/tc/util/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/util/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14771 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/util/threat_intel_util.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.870106 tcex-4.0.4/tcex/api/tc/v2/
--rw-rw-r--   0 bsummers   (503) staff       (20)       94 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.877090 tcex-4.0.4/tcex/api/tc/v2/batch/
--rw-rw-r--   0 bsummers   (503) staff       (20)      311 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2818 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    44913 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/batch.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18293 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/batch_submit.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    53186 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/batch_writer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    25062 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    30344 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1733 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1163 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/batch/tag.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.878663 tcex-4.0.4/tcex/api/tc/v2/datastore/
--rw-rw-r--   0 bsummers   (503) staff       (20)      121 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/datastore/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7207 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/datastore/cache.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10976 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/datastore/datastore.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.879825 tcex-4.0.4/tcex/api/tc/v2/metric/
--rw-rw-r--   0 bsummers   (503) staff       (20)       78 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/metric/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6524 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/metric/metric.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.880761 tcex-4.0.4/tcex/api/tc/v2/notification/
--rw-rw-r--   0 bsummers   (503) staff       (20)       96 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/notification/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3220 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/notification/notification.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.882898 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)      114 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.887760 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2371 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/filters.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.889168 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3727 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.900635 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8781 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/adversary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      949 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/attack_pattern.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1621 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/campaign.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      955 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/course_of_action.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4483 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/document.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1113 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/email.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2338 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/incident.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      944 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/intrusion_set.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      868 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/malware.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3701 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/report.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1561 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/signature.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      842 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tactic.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      843 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/threat.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      832 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      949 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/vulnerability.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.902191 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10391 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.906677 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2240 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2110 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/email_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7689 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/file.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3204 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/host.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2181 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/url.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22879 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/mapping.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2223 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2929 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2479 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1183 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/tags.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8641 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15104 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    57190 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    37126 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6862 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v2/v2.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.913222 tcex-4.0.4/tcex/api/tc/v3/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.917762 tcex-4.0.4/tcex/api/tc/v3/_gen/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9307 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    19858 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3566 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_args_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20614 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_filter_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17011 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    41985 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_object_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.919720 tcex-4.0.4/tcex/api/tc/v3/_gen/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      219 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4888 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/model/_filter_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15742 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/_gen/model/_property_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.920358 tcex-4.0.4/tcex/api/tc/v3/adversary_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/adversary_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1189 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/api_endpoints.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.922612 tcex-4.0.4/tcex/api/tc/v3/artifact_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifact_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3186 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4038 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2871 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.925387 tcex-4.0.4/tcex/api/tc/v3/artifacts/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifacts/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7075 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8443 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8582 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.928309 tcex-4.0.4/tcex/api/tc/v3/attribute_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/attribute_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3510 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5340 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3145 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.929809 tcex-4.0.4/tcex/api/tc/v3/attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2182 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/attributes/attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.931894 tcex-4.0.4/tcex/api/tc/v3/case_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/case_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5035 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10467 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5072 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.932886 tcex-4.0.4/tcex/api/tc/v3/case_management/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/case_management/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22002 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/case_management/case_management.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.935453 tcex-4.0.4/tcex/api/tc/v3/cases/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/cases/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13603 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/cases/case.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    23897 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/cases/case_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11956 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/cases/case_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.936878 tcex-4.0.4/tcex/api/tc/v3/file_actions/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/file_actions/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1690 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/file_actions/file_action_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.938022 tcex-4.0.4/tcex/api/tc/v3/file_occurrences/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/file_occurrences/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1582 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1713 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/filter_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.940056 tcex-4.0.4/tcex/api/tc/v3/group_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/group_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5062 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11262 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5510 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.942854 tcex-4.0.4/tcex/api/tc/v3/groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16272 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/groups/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    35827 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/groups/group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17637 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/groups/group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.945835 tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5170 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11362 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5630 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.949438 tcex-4.0.4/tcex/api/tc/v3/indicators/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/indicators/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16366 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicators/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    38608 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicators/indicator_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18677 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/indicators/indicator_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.951128 tcex-4.0.4/tcex/api/tc/v3/intel_requirement/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirement/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1988 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirement/ir.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.956230 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.958014 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/
--rw-rw-r--   0 bsummers   (503) staff       (20)     3292 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2161 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2216 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      256 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_req_type_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10326 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    35951 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8799 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      716 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/keyword_section_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.959746 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/
--rw-rw-r--   0 bsummers   (503) staff       (20)     3317 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8535 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4945 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.961332 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/
--rw-rw-r--   0 bsummers   (503) staff       (20)     3242 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2153 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2193 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.963438 tcex-4.0.4/tcex/api/tc/v3/notes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/notes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3500 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/notes/note.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7302 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/notes/note_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5948 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/notes/note_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13432 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/object_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7716 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/object_collection_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.967326 tcex-4.0.4/tcex/api/tc/v3/security/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1304 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/assignee_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/assignee_user_group_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      635 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/security/assignee_user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.969758 tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2910 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5143 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3422 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.972028 tcex-4.0.4/tcex/api/tc/v3/security/owners/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owners/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2797 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owners/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18119 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owners/owner_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7344 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/owners/owner_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2262 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/security.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.975069 tcex-4.0.4/tcex/api/tc/v3/security/system_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/system_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2936 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2551 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2599 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/task_assignee_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.977478 tcex-4.0.4/tcex/api/tc/v3/security/user_groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/user_groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2910 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2169 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2656 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.979637 tcex-4.0.4/tcex/api/tc/v3/security/users/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/users/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2771 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/users/user.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9703 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/security/users/user_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1937 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security/users/user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.982159 tcex-4.0.4/tcex/api/tc/v3/security_labels/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security_labels/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4352 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8930 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2902 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.984969 tcex-4.0.4/tcex/api/tc/v3/tags/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tags/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2320 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/tags/mitre_tags.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4141 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/tags/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10405 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/tags/tag_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5587 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/tags/tag_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.987410 tcex-4.0.4/tcex/api/tc/v3/tasks/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tasks/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6879 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tasks/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14303 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tasks/task_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7151 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/tasks/task_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.988598 tcex-4.0.4/tcex/api/tc/v3/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/threat_intelligence/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    19461 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.991181 tcex-4.0.4/tcex/api/tc/v3/tql/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tql/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/tql/tql.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      510 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/tql/tql_operator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      265 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/tql/tql_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1503 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/v3.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18576 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/v3_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1633 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/v3_types.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.993282 tcex-4.0.4/tcex/api/tc/v3/victim_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victim_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6065 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7768 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4860 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:51.997011 tcex-4.0.4/tcex/api/tc/v3/victim_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victim_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5095 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10917 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5113 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.001255 tcex-4.0.4/tcex/api/tc/v3/victims/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victims/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8302 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/victims/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14076 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/api/tc/v3/victims/victim_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6273 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/victims/victim_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.004779 tcex-4.0.4/tcex/api/tc/v3/workflow_events/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_events/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4668 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5713 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5335 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.007765 tcex-4.0.4/tcex/api/tc/v3/workflow_templates/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_templates/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3636 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5477 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4906 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.009383 tcex-4.0.4/tcex/app/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6535 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/app/app.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.016843 tcex-4.0.4/tcex/app/config/
--rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18720 2023-10-02 14:47:09.000000 tcex-4.0.4/tcex/app/config/app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9253 2023-07-26 23:40:09.000000 tcex-4.0.4/tcex/app/config/install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4215 2023-10-02 14:47:09.000000 tcex-4.0.4/tcex/app/config/install_json_update.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/install_json_validate.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1598 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4504 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/layout_json.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.020035 tcex-4.0.4/tcex/app/config/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      382 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13740 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/model/app_spec_yml_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    36068 2024-03-14 18:04:20.000000 tcex-4.0.4/tcex/app/config/model/install_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2942 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/model/job_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2921 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/model/layout_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1120 2023-08-31 19:21:29.000000 tcex-4.0.4/tcex/app/config/model/tcex_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    24583 2024-03-14 18:04:20.000000 tcex-4.0.4/tcex/app/config/permutation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2070 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/config/tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2469 2023-07-26 23:40:09.000000 tcex-4.0.4/tcex/app/config/tcex_json_update.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.024068 tcex-4.0.4/tcex/app/decorator/
--rw-rw-r--   0 bsummers   (503) staff       (20)      437 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/benchmark.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2039 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/debug.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4858 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/fail_on_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3901 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/on_exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/on_success.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3810 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/decorator/output.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.029187 tcex-4.0.4/tcex/app/key_value_store/
--rw-rw-r--   0 bsummers   (503) staff       (20)      279 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/key_value_store/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      932 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/key_value_store/key_value_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2008 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/key_value_store/key_value_api.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1675 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/key_value_store/key_value_mock.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2654 2023-07-26 23:39:48.000000 tcex-4.0.4/tcex/app/key_value_store/key_value_redis.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6437 2023-11-01 23:53:43.000000 tcex-4.0.4/tcex/app/key_value_store/key_value_store.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1298 2023-11-01 23:53:43.000000 tcex-4.0.4/tcex/app/key_value_store/redis_client.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2242 2023-11-01 23:53:43.000000 tcex-4.0.4/tcex/app/key_value_store/redis_client_ssl.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.033872 tcex-4.0.4/tcex/app/playbook/
--rw-rw-r--   0 bsummers   (503) staff       (20)       83 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/app/playbook/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5898 2023-10-02 14:47:35.000000 tcex-4.0.4/tcex/app/playbook/advanced_request.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3877 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/app/playbook/playbook.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21692 2023-07-26 23:40:41.000000 tcex-4.0.4/tcex/app/playbook/playbook_create.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      958 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/app/playbook/playbook_delete.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      638 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/app/playbook/playbook_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    25042 2023-10-02 14:47:35.000000 tcex-4.0.4/tcex/app/playbook/playbook_read.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.037560 tcex-4.0.4/tcex/app/service/
--rw-rw-r--   0 bsummers   (503) staff       (20)      406 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/service/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12084 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/service/api_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16005 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/app/service/common_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17206 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/service/common_service_trigger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10561 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/service/mqtt_message_broker.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15971 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/service/webhook_trigger_service.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.039224 tcex-4.0.4/tcex/app/token/
--rw-rw-r--   0 bsummers   (503) staff       (20)       75 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/token/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12649 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/app/token/token.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.040871 tcex-4.0.4/tcex/exit/
--rw-rw-r--   0 bsummers   (503) staff       (20)      179 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/exit/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5300 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/exit/error_code.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5587 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/exit/exit.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.042142 tcex-4.0.4/tcex/input/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.054206 tcex-4.0.4/tcex/input/field_type/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1930 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2812 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/input/field_type/binary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2334 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/case_management_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1616 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      805 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/datetime.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3707 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/edit_choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3228 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2435 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/group_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2094 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/indicator_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2847 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/integer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1666 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/ip_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1878 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/input/field_type/key_value.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5640 2023-10-02 14:46:58.000000 tcex-4.0.4/tcex/input/field_type/sensitive.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3315 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/string.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1115 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/tc_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8626 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/field_type/validator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15469 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/input.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.070519 tcex-4.0.4/tcex/input/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2644 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/advanced_request_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3019 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/api_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      327 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_api_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      163 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_external_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_feed_api_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      252 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      328 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      246 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/input/model/app_system_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_trigger_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      338 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/app_webhook_trigger_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1535 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/batch_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      894 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/cal_setting_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1257 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/cert_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      438 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/common_advanced_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      469 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1605 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/create_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1415 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/logging_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1922 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/model_map.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      777 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/module_app_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      439 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/module_requests_session_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      380 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1097 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/path_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1733 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/playbook_common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      833 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1279 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/proxy_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2020 2023-11-01 23:52:35.000000 tcex-4.0.4/tcex/input/model/service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1173 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/input/model/smtp_setting_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.074737 tcex-4.0.4/tcex/logger/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/logger/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3938 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/logger/api_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      893 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/logger/cache_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10370 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/logger/logger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1934 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/logger/rotating_file_handler_custom.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1094 2023-08-31 19:21:53.000000 tcex-4.0.4/tcex/logger/sensitive_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1043 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/logger/trace_logger.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.080389 tcex-4.0.4/tcex/pleb/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      936 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/cached_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/env_path.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      817 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      758 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/exception_thread.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      285 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/none_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1372 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/proxies.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2749 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/scoped_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      418 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/pleb/singleton.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7125 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/registry.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.082600 tcex-4.0.4/tcex/requests_external/
--rw-rw-r--   0 bsummers   (503) staff       (20)      231 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/requests_external/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13043 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/requests_external/external_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5002 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/requests_external/rate_limit_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1866 2023-07-26 23:39:14.000000 tcex-4.0.4/tcex/requests_external/requests_external.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.084100 tcex-4.0.4/tcex/requests_tc/
--rw-rw-r--   0 bsummers   (503) staff       (20)      137 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.086175 tcex-4.0.4/tcex/requests_tc/auth/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/auth/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1606 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/auth/hmac_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1449 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/auth/tc_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1414 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/auth/token_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3416 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/requests_tc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4417 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/requests_tc/tc_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6428 2024-03-14 17:51:53.000000 tcex-4.0.4/tcex/tcex.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.091882 tcex-4.0.4/tcex/util/
--rw-rw-r--   0 bsummers   (503) staff       (20)       71 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1827 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/aes_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4044 2023-07-26 23:41:04.000000 tcex-4.0.4/tcex/util/code_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10014 2023-07-26 23:41:04.000000 tcex-4.0.4/tcex/util/datetime_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7162 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/file_operation.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.093226 tcex-4.0.4/tcex/util/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/model/playbook_variable_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.099992 tcex-4.0.4/tcex/util/render/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/render/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      455 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/render/render.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4672 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/render/render_panel.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1243 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/render/render_prompt.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1855 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/render/render_table.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5807 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/requests_to_curl.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7034 2023-07-26 23:41:04.000000 tcex-4.0.4/tcex/util/string_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2856 2023-07-26 23:39:49.000000 tcex-4.0.4/tcex/util/util.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7992 2023-10-02 14:47:42.000000 tcex-4.0.4/tcex/util/variable.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-03-14 18:04:52.101021 tcex-4.0.4/tcex.egg-info/
--rw-r--r--   0 bsummers   (503) staff       (20)     4029 2024-03-14 18:04:51.000000 tcex-4.0.4/tcex.egg-info/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)    15272 2024-03-14 18:04:51.000000 tcex-4.0.4/tcex.egg-info/SOURCES.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2024-03-14 18:04:51.000000 tcex-4.0.4/tcex.egg-info/dependency_links.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)      302 2024-03-14 18:04:51.000000 tcex-4.0.4/tcex.egg-info/requires.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)       10 2024-03-14 18:04:51.000000 tcex-4.0.4/tcex.egg-info/top_level.txt
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.189207 tcex-4.0.5/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2023-04-01 00:56:12.000000 tcex-4.0.5/LICENSE
+-rw-r--r--   0 bsummers   (503) staff       (20)     4035 2024-04-10 20:12:16.188594 tcex-4.0.5/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2014 2024-04-10 20:10:53.000000 tcex-4.0.5/README.md
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6738 2024-04-10 20:10:53.000000 tcex-4.0.5/pyproject.toml
+-rw-rw-r--   0 bsummers   (503) staff       (20)       38 2024-04-10 20:12:16.189320 tcex-4.0.5/setup.cfg
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.873939 tcex-4.0.5/tcex/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1189 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)       78 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/__metadata__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.878242 tcex-4.0.5/tcex/api/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      726 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/api.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.879665 tcex-4.0.5/tcex/api/tc/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2185 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/tc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.882058 tcex-4.0.5/tcex/api/tc/ti_transform/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      162 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/ti_transform/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      179 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/ti_transform/formatter.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.883504 tcex-4.0.5/tcex/api/tc/ti_transform/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      613 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/ti_transform/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7825 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/ti_transform/model/transform_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6246 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/ti_transform/ti_transform.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    26321 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/ti_transform/transform_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.885040 tcex-4.0.5/tcex/api/tc/util/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/util/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14771 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/util/threat_intel_util.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.886532 tcex-4.0.5/tcex/api/tc/v2/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       94 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.892487 tcex-4.0.5/tcex/api/tc/v2/batch/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      311 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2818 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    44913 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/batch.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18293 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/batch_submit.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    53186 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/batch_writer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    25062 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    30344 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1733 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1163 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/batch/tag.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.894252 tcex-4.0.5/tcex/api/tc/v2/datastore/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      121 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/datastore/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7207 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/datastore/cache.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10976 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/datastore/datastore.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.895321 tcex-4.0.5/tcex/api/tc/v2/metric/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       78 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/metric/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6524 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/metric/metric.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.896357 tcex-4.0.5/tcex/api/tc/v2/notification/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       96 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/notification/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3220 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/notification/notification.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.899079 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      114 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.907565 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2371 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/filters.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.909617 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3727 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.924156 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8781 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/adversary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      949 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/attack_pattern.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1621 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/campaign.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      955 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/course_of_action.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4483 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/document.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1113 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/email.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2338 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/incident.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      944 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/intrusion_set.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      868 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/malware.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3701 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/report.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1561 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/signature.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      842 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tactic.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      843 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/threat.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      832 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      949 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/vulnerability.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.925814 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10391 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.931151 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2240 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2110 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/email_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7689 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/file.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3204 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/host.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2181 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/url.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22879 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/mapping.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2223 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2929 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2479 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1183 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/tags.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8641 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15104 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    57190 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    37126 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6862 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v2/v2.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.940282 tcex-4.0.5/tcex/api/tc/v3/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.946739 tcex-4.0.5/tcex/api/tc/v3/_gen/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9307 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    19858 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3566 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_args_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20614 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_filter_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17011 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    41985 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_object_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.950690 tcex-4.0.5/tcex/api/tc/v3/_gen/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      219 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4888 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/model/_filter_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16203 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/_gen/model/_property_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.951732 tcex-4.0.5/tcex/api/tc/v3/adversary_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/adversary_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1189 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/api_endpoints.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.957509 tcex-4.0.5/tcex/api/tc/v3/artifact_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifact_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3186 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4038 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2871 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.961946 tcex-4.0.5/tcex/api/tc/v3/artifacts/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifacts/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7075 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8443 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8582 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.966649 tcex-4.0.5/tcex/api/tc/v3/attribute_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/attribute_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3510 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5340 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3145 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.968733 tcex-4.0.5/tcex/api/tc/v3/attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2182 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/attributes/attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.974509 tcex-4.0.5/tcex/api/tc/v3/case_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/case_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4871 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10467 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4745 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.977246 tcex-4.0.5/tcex/api/tc/v3/case_management/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/case_management/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22002 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/case_management/case_management.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.982924 tcex-4.0.5/tcex/api/tc/v3/cases/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/cases/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13603 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/cases/case.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    23897 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/cases/case_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11956 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/cases/case_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.985307 tcex-4.0.5/tcex/api/tc/v3/file_actions/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/file_actions/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1690 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/file_actions/file_action_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.987304 tcex-4.0.5/tcex/api/tc/v3/file_occurrences/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/file_occurrences/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1582 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1713 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/filter_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.992455 tcex-4.0.5/tcex/api/tc/v3/group_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/group_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4898 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11262 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5183 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:15.996500 tcex-4.0.5/tcex/api/tc/v3/groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16272 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/groups/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    35827 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/groups/group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17638 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/groups/group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.000538 tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5006 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11362 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5303 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.004744 tcex-4.0.5/tcex/api/tc/v3/indicators/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/indicators/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16366 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicators/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    39224 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicators/indicator_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18677 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/indicators/indicator_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.007599 tcex-4.0.5/tcex/api/tc/v3/intel_requirement/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirement/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1988 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirement/ir.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.015181 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.017447 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3292 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2161 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2216 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      256 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_req_type_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10326 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    35951 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8799 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      716 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/keyword_section_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.020316 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3317 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8535 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4945 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.023390 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3242 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2153 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2193 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.027445 tcex-4.0.5/tcex/api/tc/v3/notes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/notes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3500 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/notes/note.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7302 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/notes/note_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5948 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/notes/note_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13432 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/object_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7716 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/object_collection_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.032523 tcex-4.0.5/tcex/api/tc/v3/security/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1304 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/assignee_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/assignee_user_group_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      635 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/security/assignee_user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.035705 tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2910 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5143 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3422 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.039979 tcex-4.0.5/tcex/api/tc/v3/security/owners/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owners/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2797 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owners/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18119 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owners/owner_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7344 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/owners/owner_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2262 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/security.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.043582 tcex-4.0.5/tcex/api/tc/v3/security/system_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/system_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2936 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2551 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2599 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/task_assignee_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.046624 tcex-4.0.5/tcex/api/tc/v3/security/user_groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/user_groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2910 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2169 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2656 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.049557 tcex-4.0.5/tcex/api/tc/v3/security/users/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/users/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2771 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/users/user.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9704 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/security/users/user_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1937 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security/users/user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.053341 tcex-4.0.5/tcex/api/tc/v3/security_labels/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security_labels/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4352 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8930 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2902 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.057582 tcex-4.0.5/tcex/api/tc/v3/tags/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tags/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2718 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/tags/mitre_tags.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4141 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/tags/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10405 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/tags/tag_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5587 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/tags/tag_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.060845 tcex-4.0.5/tcex/api/tc/v3/tasks/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tasks/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6879 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tasks/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14303 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tasks/task_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7151 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/tasks/task_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.062292 tcex-4.0.5/tcex/api/tc/v3/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/threat_intelligence/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    19364 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.065232 tcex-4.0.5/tcex/api/tc/v3/tql/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tql/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/tql/tql.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      510 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/tql/tql_operator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      265 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/tql/tql_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1585 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/v3.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18576 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/v3_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1633 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/v3_types.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.067459 tcex-4.0.5/tcex/api/tc/v3/victim_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victim_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6065 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7768 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4860 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.070388 tcex-4.0.5/tcex/api/tc/v3/victim_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victim_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4931 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10917 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4786 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.074314 tcex-4.0.5/tcex/api/tc/v3/victims/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victims/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8302 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/victims/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14076 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/api/tc/v3/victims/victim_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6273 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/victims/victim_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.077179 tcex-4.0.5/tcex/api/tc/v3/workflow_events/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_events/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4668 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5713 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5335 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.079350 tcex-4.0.5/tcex/api/tc/v3/workflow_templates/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_templates/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3636 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5477 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4906 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.080304 tcex-4.0.5/tcex/app/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6535 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/app/app.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.087586 tcex-4.0.5/tcex/app/config/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18720 2023-10-02 14:47:09.000000 tcex-4.0.5/tcex/app/config/app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9253 2023-07-26 23:40:09.000000 tcex-4.0.5/tcex/app/config/install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4215 2023-10-02 14:47:09.000000 tcex-4.0.5/tcex/app/config/install_json_update.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/install_json_validate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1598 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4504 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/layout_json.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.091297 tcex-4.0.5/tcex/app/config/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      382 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13740 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/model/app_spec_yml_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    36010 2024-04-10 20:11:04.000000 tcex-4.0.5/tcex/app/config/model/install_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2942 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/model/job_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2921 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/model/layout_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1120 2023-08-31 19:21:29.000000 tcex-4.0.5/tcex/app/config/model/tcex_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    24583 2024-03-14 18:04:20.000000 tcex-4.0.5/tcex/app/config/permutation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2070 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/config/tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2469 2023-07-26 23:40:09.000000 tcex-4.0.5/tcex/app/config/tcex_json_update.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.095285 tcex-4.0.5/tcex/app/decorator/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      437 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/benchmark.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2039 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/debug.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4858 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/fail_on_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3901 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/on_exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/on_success.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3810 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/decorator/output.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.101050 tcex-4.0.5/tcex/app/key_value_store/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      279 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/key_value_store/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      932 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/key_value_store/key_value_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2008 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/key_value_store/key_value_api.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1675 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/key_value_store/key_value_mock.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2654 2023-07-26 23:39:48.000000 tcex-4.0.5/tcex/app/key_value_store/key_value_redis.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6437 2023-11-01 23:53:43.000000 tcex-4.0.5/tcex/app/key_value_store/key_value_store.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1298 2023-11-01 23:53:43.000000 tcex-4.0.5/tcex/app/key_value_store/redis_client.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2242 2023-11-01 23:53:43.000000 tcex-4.0.5/tcex/app/key_value_store/redis_client_ssl.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.107887 tcex-4.0.5/tcex/app/playbook/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       83 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/app/playbook/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5898 2023-10-02 14:47:35.000000 tcex-4.0.5/tcex/app/playbook/advanced_request.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3877 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/app/playbook/playbook.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21692 2023-07-26 23:40:41.000000 tcex-4.0.5/tcex/app/playbook/playbook_create.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      958 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/app/playbook/playbook_delete.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      638 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/app/playbook/playbook_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    25042 2023-10-02 14:47:35.000000 tcex-4.0.5/tcex/app/playbook/playbook_read.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.114922 tcex-4.0.5/tcex/app/service/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      406 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/service/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12084 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/service/api_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16005 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/app/service/common_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17206 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/service/common_service_trigger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10561 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/service/mqtt_message_broker.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15971 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/service/webhook_trigger_service.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.117568 tcex-4.0.5/tcex/app/token/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       75 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/token/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12649 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/app/token/token.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.120503 tcex-4.0.5/tcex/exit/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      179 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/exit/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5300 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/exit/error_code.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5587 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/exit/exit.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.122099 tcex-4.0.5/tcex/input/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.133042 tcex-4.0.5/tcex/input/field_type/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1930 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2812 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/input/field_type/binary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2334 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/case_management_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1616 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      805 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/datetime.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3707 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/edit_choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3228 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2435 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/group_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2094 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/indicator_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2847 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/integer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1666 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/ip_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1878 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/input/field_type/key_value.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5640 2023-10-02 14:46:58.000000 tcex-4.0.5/tcex/input/field_type/sensitive.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3315 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/string.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1115 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/tc_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8626 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/field_type/validator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15469 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/input.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.153847 tcex-4.0.5/tcex/input/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2644 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/advanced_request_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3019 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/api_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      327 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_api_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      163 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_external_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_feed_api_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      252 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      328 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      246 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/input/model/app_system_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_trigger_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      338 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/app_webhook_trigger_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1535 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/batch_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      894 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/cal_setting_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1257 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/cert_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      438 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/common_advanced_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      469 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1605 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/create_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1415 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/logging_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1922 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/model_map.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      777 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/module_app_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      439 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/module_requests_session_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      380 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1097 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/path_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1733 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/playbook_common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      833 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1279 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/proxy_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2020 2023-11-01 23:52:35.000000 tcex-4.0.5/tcex/input/model/service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1173 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/input/model/smtp_setting_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.159671 tcex-4.0.5/tcex/logger/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/logger/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3938 2024-03-14 17:51:53.000000 tcex-4.0.5/tcex/logger/api_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      893 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/logger/cache_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10370 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/logger/logger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1934 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/logger/rotating_file_handler_custom.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1094 2023-08-31 19:21:53.000000 tcex-4.0.5/tcex/logger/sensitive_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1043 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/logger/trace_logger.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.167030 tcex-4.0.5/tcex/pleb/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      936 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/cached_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/env_path.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      817 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      758 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/exception_thread.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      285 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/none_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1372 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/proxies.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2749 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/scoped_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      418 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/pleb/singleton.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7125 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/registry.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.169973 tcex-4.0.5/tcex/requests_external/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      231 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/requests_external/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13043 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/requests_external/external_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5002 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/requests_external/rate_limit_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1866 2023-07-26 23:39:14.000000 tcex-4.0.5/tcex/requests_external/requests_external.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.172762 tcex-4.0.5/tcex/requests_tc/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      137 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.175524 tcex-4.0.5/tcex/requests_tc/auth/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/auth/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1606 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/auth/hmac_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1449 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/auth/tc_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1414 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/auth/token_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3416 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/requests_tc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4417 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/requests_tc/tc_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6435 2024-04-10 20:10:53.000000 tcex-4.0.5/tcex/tcex.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.181351 tcex-4.0.5/tcex/util/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       71 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1827 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/aes_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4044 2023-07-26 23:41:04.000000 tcex-4.0.5/tcex/util/code_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10014 2023-07-26 23:41:04.000000 tcex-4.0.5/tcex/util/datetime_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7162 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/file_operation.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.182499 tcex-4.0.5/tcex/util/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/model/playbook_variable_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.185124 tcex-4.0.5/tcex/util/render/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/render/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      455 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/render/render.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4672 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/render/render_panel.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1243 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/render/render_prompt.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1855 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/render/render_table.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5807 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/requests_to_curl.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6914 2024-04-10 20:11:22.000000 tcex-4.0.5/tcex/util/string_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2856 2023-07-26 23:39:49.000000 tcex-4.0.5/tcex/util/util.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7992 2023-10-02 14:47:42.000000 tcex-4.0.5/tcex/util/variable.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-10 20:12:16.186053 tcex-4.0.5/tcex.egg-info/
+-rw-r--r--   0 bsummers   (503) staff       (20)     4035 2024-04-10 20:12:15.000000 tcex-4.0.5/tcex.egg-info/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15272 2024-04-10 20:12:15.000000 tcex-4.0.5/tcex.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2024-04-10 20:12:15.000000 tcex-4.0.5/tcex.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)      305 2024-04-10 20:12:15.000000 tcex-4.0.5/tcex.egg-info/requires.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)       10 2024-04-10 20:12:15.000000 tcex-4.0.5/tcex.egg-info/top_level.txt
```

### Comparing `tcex-4.0.4/LICENSE` & `tcex-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/PKG-INFO` & `tcex-4.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 4.0.4
+Version: 4.0.5
 Summary: ThreatConnect Exchange App Framework
 Author-email: ThreatConnect <support@threatconnect.com>
 License: Apache-2.0
 Project-URL: Documentation, https://threatconnect.readme.io/docs/overview
 Project-URL: Release Notes, https://threatconnect.readme.io/docs/release-notes
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Keywords: exchange,tcex,threatconnect
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arrow
 Requires-Dist: black
-Requires-Dist: inflect
+Requires-Dist: inflection
 Requires-Dist: isort
 Requires-Dist: jmespath
 Requires-Dist: paho-mqtt<2.0.0
 Requires-Dist: pyaes
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
@@ -57,15 +57,15 @@
 
 The ThreatConnect&trade; TcEx App Framework provides functionality for writing ThreatConnect Exchange Apps.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.org/project/inflection/)
  * isort (https://pypi.org/project/isort/)
  * jmespath (https://pypi.org/project/jmespath/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * pyyaml (https://pypi.python.org/pypi/pyyaml)
```

### Comparing `tcex-4.0.4/README.md` & `tcex-4.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The ThreatConnect&trade; TcEx App Framework provides functionality for writing ThreatConnect Exchange Apps.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.org/project/inflection/)
  * isort (https://pypi.org/project/isort/)
  * jmespath (https://pypi.org/project/jmespath/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * pyyaml (https://pypi.python.org/pypi/pyyaml)
```

### Comparing `tcex-4.0.4/pyproject.toml` & `tcex-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Security",
 ]
 dependencies = [
   "arrow",
   "black",
-  "inflect",
+  "inflection",
   "isort",
   "jmespath",
   "paho-mqtt<2.0.0",
   "pyaes",
   "pydantic<2.0.0",
   "python-dateutil",
   "PyYAML",
```

### Comparing `tcex-4.0.4/tcex/__init__.py` & `tcex-4.0.5/tcex/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/api.py` & `tcex-4.0.5/tcex/api/api.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/tc.py` & `tcex-4.0.5/tcex/api/tc/tc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/ti_transform/model/__init__.py` & `tcex-4.0.5/tcex/api/tc/ti_transform/model/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/ti_transform/model/transform_model.py` & `tcex-4.0.5/tcex/api/tc/ti_transform/model/transform_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/ti_transform/ti_transform.py` & `tcex-4.0.5/tcex/api/tc/ti_transform/ti_transform.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/ti_transform/transform_abc.py` & `tcex-4.0.5/tcex/api/tc/ti_transform/transform_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/util/threat_intel_util.py` & `tcex-4.0.5/tcex/api/tc/util/threat_intel_util.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/attribute.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/batch.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/batch.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/batch_submit.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/batch_submit.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/batch_writer.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/batch_writer.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/group.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/group.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/indicator.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/security_label.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/batch/tag.py` & `tcex-4.0.5/tcex/api/tc/v2/batch/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/datastore/cache.py` & `tcex-4.0.5/tcex/api/tc/v2/datastore/cache.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/datastore/datastore.py` & `tcex-4.0.5/tcex/api/tc/v2/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/metric/metric.py` & `tcex-4.0.5/tcex/api/tc/v2/metric/metric.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/notification/notification.py` & `tcex-4.0.5/tcex/api/tc/v2/notification/notification.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/filters.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/filters.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/adversary.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/adversary.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/attack_pattern.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/campaign.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/campaign.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/course_of_action.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/course_of_action.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/document.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/document.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/email.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/email.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/event.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/event.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/incident.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/incident.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/intrusion_set.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/intrusion_set.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/malware.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/malware.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/report.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/report.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/signature.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/signature.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tactic.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tactic.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/threat.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/threat.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tool.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/tool.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/vulnerability.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/group/group_type/vulnerability.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/address.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/address.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/email_address.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/email_address.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/file.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/file.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/host.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/host.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/url.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/indicator/indicator_type/url.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/mapping.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/owner.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/security_label.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/tag.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/tags.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/tags.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/task.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/task.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/mapping/victim.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/mapping/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py` & `tcex-4.0.5/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v2/v2.py` & `tcex-4.0.5/tcex/api/tc/v2/v2.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_args_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_args_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_filter_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_model_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_model_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/_gen_object_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/_gen_object_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/model/_filter_model.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/model/_filter_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/_gen/model/_property_model.py` & `tcex-4.0.5/tcex/api/tc/v3/_gen/model/_property_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """TcEx Framework Module"""
+
 # third-party
 from pydantic import BaseModel, Extra, Field, validator
 
 # first-party
 from tcex.pleb.cached_property import cached_property
 from tcex.util import Util
+from tcex.util.render.render import Render
 from tcex.util.string_operation import CamelString
 
 
 # pylint: disable=no-self-argument
 class ExtraModel(
     BaseModel,
     extra=Extra.forbid,
@@ -128,16 +130,20 @@
         # process tc types
         self.__process_tc_types(self, extra)
 
         # process special types
         self.__process_special_types(self, extra)
 
         if extra.get('typing_type') is None:
-            raise RuntimeError(
-                f'Unable to determine typing_type for name={self.name}, type={self.type}.'
+            Render.panel.failure(
+                f'New type found for object name="{self.name}"\n'
+                f'Type: "{self.type}" should be added to PropertyModel '
+                f'in one of the following methods:\n'
+                f'_process_dict, _process_tc_type, _process_special_types\n'
+                f'\nextra: {extra}'
             )
 
         return extra
 
     def __calculate_methods(self):
         """Calculate the field methods."""
 
@@ -159,14 +165,15 @@
         if pm.type.lower() in types:
             extra.update({'typing_type': 'bool'})
 
     @classmethod
     def __process_dict_types(cls, pm: 'PropertyModel', extra: dict[str, str]):
         """Process standard type."""
         types = [
+            'AiInsights',
             'AttackSecurityCoverage',
             'AttributeSource',
             'DNSResolutions',
             'Enrichments',
             'GeoLocation',
             'InvestigationLinks',
             'IntelReqType',
@@ -310,14 +317,20 @@
                 }
             )
         elif pm.name == 'customAssociationNames':
             extra.update(
                 {
                     'typing_type': 'list[str]',
                 }
+            )
+        elif pm.name == 'customAssociationNames':
+            extra.update(
+                {
+                    'typing_type': 'list[str]',
+                }
             )
         elif pm.type == 'TaskAssignees':
             extra.update(
                 {
                     'import_data': (f'{bi}security.task_assignee_model import TaskAssigneesModel'),
                     'import_source': 'first-party-forward-reference',
                     'model': f'{pm.type}Model',
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/api_endpoints.py` & `tcex-4.0.5/tcex/api/tc/v3/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type.py` & `tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifact_types/artifact_type_model.py` & `tcex-4.0.5/tcex/api/tc/v3/artifact_types/artifact_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact.py` & `tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/artifacts/artifact_model.py` & `tcex-4.0.5/tcex/api/tc/v3/artifacts/artifact_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type.py` & `tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/attribute_types/attribute_type_model.py` & `tcex-4.0.5/tcex/api/tc/v3/attribute_types/attribute_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/attributes/attribute_model.py` & `tcex-4.0.5/tcex/api/tc/v3/attributes/attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute.py` & `tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,14 @@
             within the object. Only applies to certain attribute and data types.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
-        update_last_modified_date (bool, kwargs): A flag giving the client the ability to choose if
-            the attribute last modified date should be changed.
         value (str, kwargs): The attribute value.
     """
 
     def __init__(self, **kwargs):
         """Initialize instance properties."""
         super().__init__(kwargs.pop('session', None))
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/case_attributes/case_attribute_model.py` & `tcex-4.0.5/tcex/api/tc/v3/case_attributes/case_attribute_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,24 +96,14 @@
     type: str | None = Field(
         None,
         description='The attribute type.',
         methods=['POST'],
         read_only=False,
         title='type',
     )
-    update_last_modified_date: bool = Field(
-        None,
-        description=(
-            'A flag giving the client the ability to choose if the attribute last modified date '
-            'should be changed.'
-        ),
-        methods=['POST', 'PUT'],
-        read_only=False,
-        title='updateLastModifiedDate',
-    )
     value: str | None = Field(
         None,
         description='The attribute value.',
         methods=['POST', 'PUT'],
         read_only=False,
         title='value',
     )
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/case_management/case_management.py` & `tcex-4.0.5/tcex/api/tc/v3/case_management/case_management.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/cases/case.py` & `tcex-4.0.5/tcex/api/tc/v3/cases/case.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/cases/case_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/cases/case_model.py` & `tcex-4.0.5/tcex/api/tc/v3/cases/case_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/file_actions/file_action_model.py` & `tcex-4.0.5/tcex/api/tc/v3/file_actions/file_action_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py` & `tcex-4.0.5/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/filter_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute.py` & `tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
         group_id (int, kwargs): Group associated with attribute.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
-        update_last_modified_date (bool, kwargs): A flag giving the client the ability to choose if
-            the attribute last modified date should be changed.
         value (str, kwargs): The attribute value.
     """
 
     def __init__(self, **kwargs):
         """Initialize instance properties."""
         super().__init__(kwargs.pop('session', None))
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/group_attributes/group_attribute_model.py` & `tcex-4.0.5/tcex/api/tc/v3/group_attributes/group_attribute_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,24 +103,14 @@
     type: str | None = Field(
         None,
         description='The attribute type.',
         methods=['POST'],
         read_only=False,
         title='type',
     )
-    update_last_modified_date: bool = Field(
-        None,
-        description=(
-            'A flag giving the client the ability to choose if the attribute last modified date '
-            'should be changed.'
-        ),
-        methods=['POST', 'PUT'],
-        read_only=False,
-        title='updateLastModifiedDate',
-    )
     value: str | None = Field(
         None,
         description='The attribute value.',
         methods=['POST', 'PUT'],
         read_only=False,
         title='value',
     )
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/groups/group.py` & `tcex-4.0.5/tcex/api/tc/v3/groups/group.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/groups/group_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/groups/group_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/groups/group_model.py` & `tcex-4.0.5/tcex/api/tc/v3/groups/group_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     )
     id: int | None = Field(
         None,
         description='The ID of the item.',
         read_only=True,
         title='id',
     )
-    insights: str | None = Field(
+    insights: dict | None = Field(
         None,
         allow_mutation=False,
         applies_to=['Document', 'Report'],
         description='An AI generated synopsis of the document.',
         read_only=True,
         title='insights',
     )
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py` & `tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,14 @@
         indicator_id (int, kwargs): Indicator associated with attribute.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
-        update_last_modified_date (bool, kwargs): A flag giving the client the ability to choose if
-            the attribute last modified date should be changed.
         value (str, kwargs): The attribute value.
     """
 
     def __init__(self, **kwargs):
         """Initialize instance properties."""
         super().__init__(kwargs.pop('session', None))
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py` & `tcex-4.0.5/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,24 +103,14 @@
     type: str | None = Field(
         None,
         description='The attribute type.',
         methods=['POST'],
         read_only=False,
         title='type',
     )
-    update_last_modified_date: bool = Field(
-        None,
-        description=(
-            'A flag giving the client the ability to choose if the attribute last modified date '
-            'should be changed.'
-        ),
-        methods=['POST', 'PUT'],
-        read_only=False,
-        title='updateLastModifiedDate',
-    )
     value: str | None = Field(
         None,
         description='The attribute value.',
         methods=['POST', 'PUT'],
         read_only=False,
         title='value',
     )
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicators/indicator.py` & `tcex-4.0.5/tcex/api/tc/v3/indicators/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicators/indicator_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/indicators/indicator_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,29 @@
             raise RuntimeError(
                 'Operator must be CONTAINS, NOT_CONTAINS, IN'
                 'or NOT_IN when filtering on a list of values.'
             )
 
         self._tql.add_filter('attribute', operator, attribute, TqlType.STRING)
 
+    def common_id(self, operator: Enum, common_id: int | list):
+        """Filter Common Id based on **commonId** keyword.
+
+        Args:
+            operator: The operator enum for the filter.
+            common_id: The common ID of the indicator linking it between owners.
+        """
+        if isinstance(common_id, list) and operator not in self.list_types:
+            raise RuntimeError(
+                'Operator must be CONTAINS, NOT_CONTAINS, IN'
+                'or NOT_IN when filtering on a list of values.'
+            )
+
+        self._tql.add_filter('commonId', operator, common_id, TqlType.INTEGER)
+
     def confidence(self, operator: Enum, confidence: int | list):
         """Filter Confidence Rating based on **confidence** keyword.
 
         Args:
             operator: The operator enum for the filter.
             confidence: The confidence in the indicator's rating.
         """
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/indicators/indicator_model.py` & `tcex-4.0.5/tcex/api/tc/v3/indicators/indicator_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirement/ir.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirement/ir.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/categories/category_model.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/categories/category_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/intel_requirement_model.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/intel_requirement_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/keyword_section_model.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/keyword_section_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/results/result_model.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/results/result_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/intel_requirements/subtypes/subtype_model.py` & `tcex-4.0.5/tcex/api/tc/v3/intel_requirements/subtypes/subtype_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/notes/note.py` & `tcex-4.0.5/tcex/api/tc/v3/notes/note.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/notes/note_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/notes/note_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/notes/note_model.py` & `tcex-4.0.5/tcex/api/tc/v3/notes/note_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/object_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/object_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/object_collection_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/object_collection_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/assignee_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/assignee_user_group_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/assignee_user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/assignee_user_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/assignee_user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owner_roles/owner_role_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owner_roles/owner_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owners/owner.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owners/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owners/owner_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owners/owner_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/owners/owner_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/owners/owner_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/security.py` & `tcex-4.0.5/tcex/api/tc/v3/security/security.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role.py` & `tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/system_roles/system_role_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/system_roles/system_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/task_assignee_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/task_assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group.py` & `tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/user_groups/user_group_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/user_groups/user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/users/user.py` & `tcex-4.0.5/tcex/api/tc/v3/security/users/user.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/users/user_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security/users/user_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 from datetime import datetime
 from enum import Enum
 
 # third-party
 from arrow import Arrow
 
@@ -153,16 +154,16 @@
         self._tql.add_filter('locked', operator, locked, TqlType.BOOLEAN)
 
     def password_reset_required(self, operator: Enum, password_reset_required: bool):
         """Filter Password Reset Required based on **passwordResetRequired** keyword.
 
         Args:
             operator: The operator enum for the filter.
-            password_reset_required: A flag indicating whether or not
-                the user's password needs to be reset upon next login.
+            password_reset_required: A flag indicating whether or not the user's password needs to
+                be reset upon next login.
         """
         self._tql.add_filter(
             'passwordResetRequired', operator, password_reset_required, TqlType.BOOLEAN
         )
 
     def pseudonym(self, operator: Enum, pseudonym: list | str):
         """Filter Pseudonym based on **pseudonym** keyword.
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security/users/user_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security/users/user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label.py` & `tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/security_labels/security_label_model.py` & `tcex-4.0.5/tcex/api/tc/v3/security_labels/security_label_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tags/mitre_tags.py` & `tcex-4.0.5/tcex/api/tc/v3/tags/mitre_tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,50 +25,55 @@
         """Return the formatted tag."""
         return f'{self.id} - {self.name}'
 
 
 class MitreTags:
     """MitreTags Class"""
 
-    def __init__(self, mitre_tags: dict[str, str]):
+    def __init__(self, mitre_tags: dict[str, str], verbose: bool = False):
         """Initialize instance properties."""
         self._mitre_tags = {id_: MitreTag(id=id_, name=name) for id_, name in mitre_tags.items()}
+        self.verbose = verbose
         self.log = _logger
 
     @cached_property
-    def mitre_tags_name_id(self):
+    def mitre_tags_name_id(self) -> dict[str, MitreTag]:
         """Return a dict of MitreTags keyed by name."""
         mitre_tags = {}
         for tag in self._mitre_tags.values():
             titles = tag.name.split(': ')
 
             key = titles[1].strip() if len(titles) > 1 else tag.name
             mitre_tags[key.lower()] = MitreTag(id=tag.id, name=tag.name)
 
         return mitre_tags
 
-    def get_by_name(self, name: str) -> str | None:
+    def get_by_name(self, name: str, default: str | None = None) -> str | None:
         """Return the tag id for the provided name."""
         mitre_tag = self.mitre_tags_name_id.get(name.lower())
         if mitre_tag is None:
-            self.log.warning(f'No Mitre match found for {name}.')
-            return None
+            if self.verbose is True:
+                self.log.warning(f'No Mitre match found for {name}.')
+            return default
         return mitre_tag.formatted
 
-    def get_by_id(self, id_: str) -> str:
-        """Return the tag name for the provided id."""
-        mitre_tag = self._mitre_tags.get(id_)
+    def get_by_id(self, id_: str, default: str | None = None) -> str | None:
+        """Return the tag name for the provided id (e.g., T1000)."""
+        mitre_tag = self._mitre_tags.get(str(id_).upper())
         if mitre_tag is None:
-            self.log.warning(f'No Mitre match found for {id_}, returning id unformatted.')
-            return id_
+            if self.verbose is True:
+                self.log.warning(f'No Mitre match found for {id_}, returning id unformatted.')
+            return default
         return mitre_tag.formatted
 
-    def get_by_id_regex(self, value: str):
+    def get_by_id_regex(self, value: str, default: str | None = None) -> str | None:
         r"""Get the appropriate MitreTag using the (T\d+(?:\.\d+)?) regex."""
-        matches = re.findall(r'(T\d+(?:\.\d+)?)', value)
+        matches = re.findall(r'([Tt]\d+(?:\.\d+)?)', value)
         if not matches:
-            self.log.warning(f'No Mitre matches found for {value}')
-            return None
+            if self.verbose is True:
+                self.log.warning(f'No Mitre matches found for {value}')
+            return default
         if len(matches) > 1:
-            self.log.warning(f'Multiple Mitre matches found for {value}: {matches}')
-            return None
-        return self.get_by_id(matches[0])
+            if self.verbose is True:
+                self.log.warning(f'Multiple Mitre matches found for {value}: {matches}')
+            return default
+        return self.get_by_id(matches[0], default)
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tags/tag.py` & `tcex-4.0.5/tcex/api/tc/v3/tags/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tags/tag_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/tags/tag_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tags/tag_model.py` & `tcex-4.0.5/tcex/api/tc/v3/tags/tag_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tasks/task.py` & `tcex-4.0.5/tcex/api/tc/v3/tasks/task.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tasks/task_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/tasks/task_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tasks/task_model.py` & `tcex-4.0.5/tcex/api/tc/v3/tasks/task_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py` & `tcex-4.0.5/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 import logging
 
 # third-party
 from requests import Session
 
 # first-party
@@ -33,23 +34,20 @@
     Args:
         session: An configured instance of request.Session with TC API Auth.
     """
 
     def __init__(self, session: Session):
         """Initialize instance properties."""
         self.session = session
-        self._ti_utils = None
         self.log = _logger
 
-    @property
+    @cached_property
     def ti_utils(self):
         """Return instance of Threat Intel Utils."""
-        if not self._ti_utils:
-            self._ti_utils = ThreatIntelUtil(session_tc=self.session)
-        return self._ti_utils
+        return ThreatIntelUtil(session_tc=self.session)
 
     def create_entity(self, entity: dict, owner: str) -> dict | None:
         """Create a CM object provided a dict and owner."""
         entity_type = entity['type'].lower()
         entity_type = entity_type.replace(' ', '_')
         try:
             if entity_type in (type_.lower() for type_ in self.ti_utils.group_types):
@@ -188,28 +186,14 @@
         Keyword Args:
             initial_response (dict, optional): Initial data in Case Object for Group.
             tql_filters (list, optional): A list of TQL filters.
             params (dict, optional): A dict of query params for the request.
         """
         return Groups(session=self.session, **kwargs)
 
-    @cached_property
-    def mitre_tags(self) -> MitreTags:
-        """Mitre Tags"""
-        mitre_tags = {}
-        try:
-            tags = Tags(session=self.session, params={'resultLimit': 1_000})
-            tags.filter.technique_id(TqlOperator.NE, None)  # type: ignore
-            for tag in tags:
-                mitre_tags[str(tag.model.technique_id)] = tag.model.name
-        except Exception as e:
-            self.log.exception('Error downloading Mitre Tags')
-            raise e
-        return MitreTags(mitre_tags)
-
     def indicator(self, **kwargs) -> Indicator:
         """Return a instance of Group object.
 
         Args:
             **kwargs: Additional keyword arguments.
 
         Keyword Args:
@@ -311,14 +295,28 @@
         Keyword Args:
             initial_response (dict, optional): Initial data in Case Object for Indicator.
             tql_filters (list, optional): A list of TQL filters.
             params (dict, optional): A dict of query params for the request.
         """
         return Indicators(session=self.session, **kwargs)
 
+    @cached_property
+    def mitre_tags(self) -> MitreTags:
+        """Mitre Tags"""
+        mitre_tags = {}
+        try:
+            tags = Tags(session=self.session, params={'resultLimit': 1_000})
+            tags.filter.technique_id(TqlOperator.NE, None)  # type: ignore
+            for tag in tags:
+                mitre_tags[str(tag.model.technique_id)] = tag.model.name
+        except Exception as e:
+            self.log.exception('Error downloading Mitre Tags')
+            raise e
+        return MitreTags(mitre_tags)
+
     def security_label(self, **kwargs) -> SecurityLabel:
         """Return a instance of Case Attributes object.
 
         Args:
             **kwargs: Additional keyword arguments.
 
         Keyword Args:
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/tql/tql.py` & `tcex-4.0.5/tcex/api/tc/v3/tql/tql.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/v3.py` & `tcex-4.0.5/tcex/api/tc/v3/v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # first-party
 from tcex.api.tc.v3.attribute_types.attribute_type import AttributeType, AttributeTypes
 from tcex.api.tc.v3.case_management.case_management import CaseManagement
 from tcex.api.tc.v3.intel_requirement.ir import IR
 from tcex.api.tc.v3.security.security import Security
 from tcex.api.tc.v3.threat_intelligence.threat_intelligence import ThreatIntelligence
+from tcex.pleb.cached_property import cached_property
 
 
 class V3(CaseManagement, Security, ThreatIntelligence):
     """V3 API Collection
 
     Args:
         session: An configured instance of request.Session with TC API Auth.
@@ -19,26 +20,26 @@
         """Return a instance of Attribute Types object."""
         return AttributeType(session=self.session, **kwargs)
 
     def attribute_types(self, **kwargs) -> AttributeTypes:
         """Return a instance of Attribute Types object."""
         return AttributeTypes(session=self.session, **kwargs)
 
-    @property
+    @cached_property
     def cm(self) -> CaseManagement:
         """Return Case Management API collection."""
         return CaseManagement(self.session)
 
-    @property
+    @cached_property
     def ir(self) -> IR:
         """Return Intel Requirement API collection."""
         return IR(self.session)
 
-    @property
+    @cached_property
     def security(self) -> Security:
         """Return Security API collection."""
         return Security(self.session)
 
-    @property
+    @cached_property
     def ti(self) -> ThreatIntelligence:
         """Return Threat Intelligence API collection."""
         return ThreatIntelligence(self.session)
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/v3_model_abc.py` & `tcex-4.0.5/tcex/api/tc/v3/v3_model_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/v3_types.py` & `tcex-4.0.5/tcex/api/tc/v3/v3_types.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_assets/victim_asset_model.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_assets/victim_asset_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,14 @@
             within the object. Only applies to certain attribute and data types.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
-        update_last_modified_date (bool, kwargs): A flag giving the client the ability to choose if
-            the attribute last modified date should be changed.
         value (str, kwargs): The attribute value.
         victim_id (int, kwargs): Victim associated with attribute.
     """
 
     def __init__(self, **kwargs):
         """Initialize instance properties."""
         super().__init__(kwargs.pop('session', None))
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py` & `tcex-4.0.5/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,24 +89,14 @@
     type: str | None = Field(
         None,
         description='The attribute type.',
         methods=['POST'],
         read_only=False,
         title='type',
     )
-    update_last_modified_date: bool = Field(
-        None,
-        description=(
-            'A flag giving the client the ability to choose if the attribute last modified date '
-            'should be changed.'
-        ),
-        methods=['POST', 'PUT'],
-        read_only=False,
-        title='updateLastModifiedDate',
-    )
     value: str | None = Field(
         None,
         description='The attribute value.',
         methods=['POST', 'PUT'],
         read_only=False,
         title='value',
     )
```

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victims/victim.py` & `tcex-4.0.5/tcex/api/tc/v3/victims/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victims/victim_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/victims/victim_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/victims/victim_model.py` & `tcex-4.0.5/tcex/api/tc/v3/victims/victim_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_events/workflow_event_model.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_events/workflow_event_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/api/tc/v3/workflow_templates/workflow_template_model.py` & `tcex-4.0.5/tcex/api/tc/v3/workflow_templates/workflow_template_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/app.py` & `tcex-4.0.5/tcex/app/app.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/app_spec_yml.py` & `tcex-4.0.5/tcex/app/config/app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/install_json.py` & `tcex-4.0.5/tcex/app/config/install_json.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/install_json_update.py` & `tcex-4.0.5/tcex/app/config/install_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/install_json_validate.py` & `tcex-4.0.5/tcex/app/config/install_json_validate.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/job_json.py` & `tcex-4.0.5/tcex/app/config/job_json.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/layout_json.py` & `tcex-4.0.5/tcex/app/config/layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/model/app_spec_yml_model.py` & `tcex-4.0.5/tcex/app/config/model/app_spec_yml_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/model/install_json_model.py` & `tcex-4.0.5/tcex/app/config/model/install_json_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
         commit_hash = os.getenv('CI_COMMIT_SHA') or os.getenv('GITHUB_SHA')
 
     return commit_hash
 
 
 def gen_app_id() -> UUID5:
     """Return a generate id for the current App."""
-    return uuid.uuid5(uuid.NAMESPACE_X500, os.path.basename(os.getcwd()).lower())
+    return uuid.uuid4()
 
 
 class InstallJsonCommonModel(BaseModel):
     """Model definition for install.json common configuration
 
     This model contains the common fields for the install.json file and
     the app_spec.yaml file.
```

### Comparing `tcex-4.0.4/tcex/app/config/model/job_json_model.py` & `tcex-4.0.5/tcex/app/config/model/job_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/model/layout_json_model.py` & `tcex-4.0.5/tcex/app/config/model/layout_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/model/tcex_json_model.py` & `tcex-4.0.5/tcex/app/config/model/tcex_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/permutation.py` & `tcex-4.0.5/tcex/app/config/permutation.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/tcex_json.py` & `tcex-4.0.5/tcex/app/config/tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/config/tcex_json_update.py` & `tcex-4.0.5/tcex/app/config/tcex_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/benchmark.py` & `tcex-4.0.5/tcex/app/decorator/benchmark.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/debug.py` & `tcex-4.0.5/tcex/app/decorator/debug.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/fail_on_output.py` & `tcex-4.0.5/tcex/app/decorator/fail_on_output.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/on_exception.py` & `tcex-4.0.5/tcex/app/decorator/on_exception.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/on_success.py` & `tcex-4.0.5/tcex/app/decorator/on_success.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/decorator/output.py` & `tcex-4.0.5/tcex/app/decorator/output.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/key_value_abc.py` & `tcex-4.0.5/tcex/app/key_value_store/key_value_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/key_value_api.py` & `tcex-4.0.5/tcex/app/key_value_store/key_value_api.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/key_value_mock.py` & `tcex-4.0.5/tcex/app/key_value_store/key_value_mock.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/key_value_redis.py` & `tcex-4.0.5/tcex/app/key_value_store/key_value_redis.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/key_value_store.py` & `tcex-4.0.5/tcex/app/key_value_store/key_value_store.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/redis_client.py` & `tcex-4.0.5/tcex/app/key_value_store/redis_client.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/key_value_store/redis_client_ssl.py` & `tcex-4.0.5/tcex/app/key_value_store/redis_client_ssl.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/advanced_request.py` & `tcex-4.0.5/tcex/app/playbook/advanced_request.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/playbook.py` & `tcex-4.0.5/tcex/app/playbook/playbook.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/playbook_create.py` & `tcex-4.0.5/tcex/app/playbook/playbook_create.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/playbook_delete.py` & `tcex-4.0.5/tcex/app/playbook/playbook_delete.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/playbook_output.py` & `tcex-4.0.5/tcex/app/playbook/playbook_output.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/playbook/playbook_read.py` & `tcex-4.0.5/tcex/app/playbook/playbook_read.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/service/api_service.py` & `tcex-4.0.5/tcex/app/service/api_service.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/service/common_service.py` & `tcex-4.0.5/tcex/app/service/common_service.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/service/common_service_trigger.py` & `tcex-4.0.5/tcex/app/service/common_service_trigger.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/service/mqtt_message_broker.py` & `tcex-4.0.5/tcex/app/service/mqtt_message_broker.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/service/webhook_trigger_service.py` & `tcex-4.0.5/tcex/app/service/webhook_trigger_service.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/app/token/token.py` & `tcex-4.0.5/tcex/app/token/token.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/exit/error_code.py` & `tcex-4.0.5/tcex/exit/error_code.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/exit/exit.py` & `tcex-4.0.5/tcex/exit/exit.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/__init__.py` & `tcex-4.0.5/tcex/input/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/binary.py` & `tcex-4.0.5/tcex/input/field_type/binary.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/case_management_entity.py` & `tcex-4.0.5/tcex/input/field_type/case_management_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/choice.py` & `tcex-4.0.5/tcex/input/field_type/choice.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/datetime.py` & `tcex-4.0.5/tcex/input/field_type/datetime.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/edit_choice.py` & `tcex-4.0.5/tcex/input/field_type/edit_choice.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/exception.py` & `tcex-4.0.5/tcex/input/field_type/exception.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/group_entity.py` & `tcex-4.0.5/tcex/input/field_type/group_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/indicator_entity.py` & `tcex-4.0.5/tcex/input/field_type/indicator_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/integer.py` & `tcex-4.0.5/tcex/input/field_type/integer.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/ip_address.py` & `tcex-4.0.5/tcex/input/field_type/ip_address.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/key_value.py` & `tcex-4.0.5/tcex/input/field_type/key_value.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/sensitive.py` & `tcex-4.0.5/tcex/input/field_type/sensitive.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/string.py` & `tcex-4.0.5/tcex/input/field_type/string.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/tc_entity.py` & `tcex-4.0.5/tcex/input/field_type/tc_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/field_type/validator.py` & `tcex-4.0.5/tcex/input/field_type/validator.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/input.py` & `tcex-4.0.5/tcex/input/input.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/advanced_request_model.py` & `tcex-4.0.5/tcex/input/model/advanced_request_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/api_model.py` & `tcex-4.0.5/tcex/input/model/api_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/batch_model.py` & `tcex-4.0.5/tcex/input/model/batch_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/cal_setting_model.py` & `tcex-4.0.5/tcex/input/model/cal_setting_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/cert_model.py` & `tcex-4.0.5/tcex/input/model/cert_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/create_config_model.py` & `tcex-4.0.5/tcex/input/model/create_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/logging_model.py` & `tcex-4.0.5/tcex/input/model/logging_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/model_map.py` & `tcex-4.0.5/tcex/input/model/model_map.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/module_app_model.py` & `tcex-4.0.5/tcex/input/model/module_app_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/path_model.py` & `tcex-4.0.5/tcex/input/model/path_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/playbook_common_model.py` & `tcex-4.0.5/tcex/input/model/playbook_common_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/playbook_model.py` & `tcex-4.0.5/tcex/input/model/playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/proxy_model.py` & `tcex-4.0.5/tcex/input/model/proxy_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/service_model.py` & `tcex-4.0.5/tcex/input/model/service_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/input/model/smtp_setting_model.py` & `tcex-4.0.5/tcex/input/model/smtp_setting_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/api_handler.py` & `tcex-4.0.5/tcex/logger/api_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/cache_handler.py` & `tcex-4.0.5/tcex/logger/cache_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/logger.py` & `tcex-4.0.5/tcex/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/rotating_file_handler_custom.py` & `tcex-4.0.5/tcex/logger/rotating_file_handler_custom.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/sensitive_filter.py` & `tcex-4.0.5/tcex/logger/sensitive_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/logger/trace_logger.py` & `tcex-4.0.5/tcex/logger/trace_logger.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/cached_property.py` & `tcex-4.0.5/tcex/pleb/cached_property.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/env_path.py` & `tcex-4.0.5/tcex/pleb/env_path.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/event.py` & `tcex-4.0.5/tcex/pleb/event.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/exception_thread.py` & `tcex-4.0.5/tcex/pleb/exception_thread.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/proxies.py` & `tcex-4.0.5/tcex/pleb/proxies.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/pleb/scoped_property.py` & `tcex-4.0.5/tcex/pleb/scoped_property.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/registry.py` & `tcex-4.0.5/tcex/registry.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_external/external_session.py` & `tcex-4.0.5/tcex/requests_external/external_session.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_external/rate_limit_handler.py` & `tcex-4.0.5/tcex/requests_external/rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_external/requests_external.py` & `tcex-4.0.5/tcex/requests_external/requests_external.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_tc/auth/hmac_auth.py` & `tcex-4.0.5/tcex/requests_tc/auth/hmac_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_tc/auth/tc_auth.py` & `tcex-4.0.5/tcex/requests_tc/auth/tc_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_tc/auth/token_auth.py` & `tcex-4.0.5/tcex/requests_tc/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_tc/requests_tc.py` & `tcex-4.0.5/tcex/requests_tc/requests_tc.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/requests_tc/tc_session.py` & `tcex-4.0.5/tcex/requests_tc/tc_session.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/tcex.py` & `tcex-4.0.5/tcex/tcex.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         exit_code = ExitCode.SUCCESS
         if threading.current_thread().name == 'MainThread' and signal_interrupt in (2, 15):
             exit_code = ExitCode.FAILURE
 
         # pylint: disable=no-member
         self.exit.exit(exit_code, 'The App received an interrupt signal and will now exit.')
 
-    @property
+    @cached_property
     def api(self) -> API:
         """Return instance of API."""
         # pylint: disable=no-member
         return API(self.inputs, self.session.tc)
 
     @cached_property
     def app(self) -> App:
```

### Comparing `tcex-4.0.4/tcex/util/aes_operation.py` & `tcex-4.0.5/tcex/util/aes_operation.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/code_operation.py` & `tcex-4.0.5/tcex/util/code_operation.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/datetime_operation.py` & `tcex-4.0.5/tcex/util/datetime_operation.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/file_operation.py` & `tcex-4.0.5/tcex/util/file_operation.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/model/playbook_variable_model.py` & `tcex-4.0.5/tcex/util/model/playbook_variable_model.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/render/render_panel.py` & `tcex-4.0.5/tcex/util/render/render_panel.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/render/render_prompt.py` & `tcex-4.0.5/tcex/util/render/render_prompt.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/render/render_table.py` & `tcex-4.0.5/tcex/util/render/render_table.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/requests_to_curl.py` & `tcex-4.0.5/tcex/util/requests_to_curl.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/string_operation.py` & `tcex-4.0.5/tcex/util/string_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 """TcEx Framework Module"""
+
 # standard library
 import random
-import re
 from functools import cached_property, reduce
 from string import ascii_letters
 
 # third-party
-import inflect
+import inflection
 
 
 class StringOperation:
     """TcEx Utilities String Operations Class"""
 
     @staticmethod
     def camel_string(string: str) -> 'CamelString':
         """Return str with custom properties/methods."""
         return CamelString(string)
 
     def camel_to_snake(self, string: str) -> str:
         """Return snake_case string from a camelCase string."""
-        return self._camel_pattern.sub('_', string).lower()
+        return inflection.underscore(string)
 
     def camel_to_space(self, string: str) -> str:
         """Return space case string from a camelCase string."""
-        return self._camel_pattern.sub(' ', string).lower()
+        return inflection.underscore(string).replace('_', ' ')
 
     @cached_property
-    def inflect(self) -> inflect.engine:
+    def inflect(self):
         """Return instance of inflect."""
-        return inflect.engine()
+        return inflection
+
+    @cached_property
+    def inflection(self):
+        """Return instance of inflect."""
+        return inflection
 
     @staticmethod
     def random_string(string_length: int = 10) -> str:
         """Generate a random string of fixed length."""
         return ''.join(random.choice(ascii_letters) for _ in range(string_length))  # nosec
 
     @staticmethod
     def snake_string(string: str) -> 'SnakeString':
         """Return custom str with custom properties/methods."""
         return SnakeString(string)
 
     @staticmethod
     def snake_to_pascal(string: str) -> str:
         """Convert snake_case to PascalCase."""
-        return string.replace('_', ' ').title().replace(' ', '')
+        return inflection.camelize(string, uppercase_first_letter=True)
 
     @staticmethod
     def snake_to_camel(string: str) -> str:
         """Convert snake_case to camelCase."""
-        components = string.split('_')
-        return components[0] + ''.join(x.title() for x in components[1:])
+        return inflection.camelize(string, uppercase_first_letter=False)
 
     @staticmethod
     def to_bool(value: bool | int | str) -> bool:
         """Convert value to bool."""
         return str(value).lower() in ['1', 't', 'true', 'y', 'yes']
 
     @staticmethod
@@ -93,19 +97,14 @@
         if spaces is True:
             if not output.endswith(' '):
                 # split output on spaces and drop last item to terminate string on word
                 output = ' '.join(output.split(' ')[:-1])
 
         return f'{output.rstrip()}{append_chars}'
 
-    @property
-    def _camel_pattern(self) -> re.Pattern:
-        """Return compiled re pattern for converting to camelCase."""
-        return re.compile(r'(?<!^)(?=[A-Z])')
-
     @staticmethod
     def wrap_string(
         line: str,
         wrap_chars: list[str] | None = None,
         length: int = 100,
         force_wrap: bool = True,
     ) -> str:
@@ -159,19 +158,19 @@
 
     def pascal_case(self):
         """Return a PascalCase version of a camelCase string."""
         return CamelString(self.so.camel_to_space(self).title().replace(' ', ''))
 
     def plural(self):
         """Return the plural spelling of a camelCase string."""
-        return CamelString(self.so.inflect.plural(self.singular()))
+        return CamelString(self.so.inflection.pluralize(self.singular()))
 
     def singular(self):
         """Return the singular spelling of a camelCase string."""
-        _singular = self.so.inflect.singular_noun(self)
+        _singular = self.so.inflection.singularize(self)
 
         if not _singular:
             _singular = self
         return CamelString(_singular)
 
     def snake_case(self):
         """Return a snake_case version of a camelCase string."""
@@ -194,19 +193,19 @@
 
     def pascal_case(self):
         """Return a PascalCase version of a snake_case string."""
         return SnakeString(self.so.snake_to_pascal(self))
 
     def plural(self):
         """Return the plural spelling of a snake_case string."""
-        return SnakeString(self.so.inflect.plural(self.singular()))
+        return SnakeString(self.so.inflection.pluralize(self.singular()))
 
     def singular(self):
         """Return the singular spelling of a snake_case string."""
-        _singular = self.so.inflect.singular_noun(self)
+        _singular = self.so.inflection.singularize(self)
 
         if not _singular:
             _singular = self
         return SnakeString(_singular)
 
     def space_case(self, title: bool = True):
         """Return a "space case" version of a snake_case string."""
```

### Comparing `tcex-4.0.4/tcex/util/util.py` & `tcex-4.0.5/tcex/util/util.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex/util/variable.py` & `tcex-4.0.5/tcex/util/variable.py`

 * *Files identical despite different names*

### Comparing `tcex-4.0.4/tcex.egg-info/PKG-INFO` & `tcex-4.0.5/tcex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 4.0.4
+Version: 4.0.5
 Summary: ThreatConnect Exchange App Framework
 Author-email: ThreatConnect <support@threatconnect.com>
 License: Apache-2.0
 Project-URL: Documentation, https://threatconnect.readme.io/docs/overview
 Project-URL: Release Notes, https://threatconnect.readme.io/docs/release-notes
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Keywords: exchange,tcex,threatconnect
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arrow
 Requires-Dist: black
-Requires-Dist: inflect
+Requires-Dist: inflection
 Requires-Dist: isort
 Requires-Dist: jmespath
 Requires-Dist: paho-mqtt<2.0.0
 Requires-Dist: pyaes
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
@@ -57,15 +57,15 @@
 
 The ThreatConnect&trade; TcEx App Framework provides functionality for writing ThreatConnect Exchange Apps.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.org/project/inflection/)
  * isort (https://pypi.org/project/isort/)
  * jmespath (https://pypi.org/project/jmespath/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * pyyaml (https://pypi.python.org/pypi/pyyaml)
```

### Comparing `tcex-4.0.4/tcex.egg-info/SOURCES.txt` & `tcex-4.0.5/tcex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

