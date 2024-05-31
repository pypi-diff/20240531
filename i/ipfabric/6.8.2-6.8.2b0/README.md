# Comparing `tmp/ipfabric-6.8.2.tar.gz` & `tmp/ipfabric-6.8.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.8.2.tar", max compression
+gzip compressed data, was "ipfabric-6.8.2b0.tar", max compression
```

## Comparing `ipfabric-6.8.2.tar` & `ipfabric-6.8.2b0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.8.2/ipfabric/__init__.py
--rw-r--r--   0        0        0    11179 2024-05-31 13:51:35.960240 ipfabric-6.8.2/ipfabric/api.py
--rw-r--r--   0        0        0    10301 2024-05-14 16:42:35.403692 ipfabric-6.8.2/ipfabric/auth.py
--rw-r--r--   0        0        0    24100 2024-05-31 13:51:35.962237 ipfabric-6.8.2/ipfabric/client.py
--rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.8.2/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0    18233 2024-05-14 16:42:35.403692 ipfabric-6.8.2/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.8.2/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.8.2/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.8.2/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.8.2/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.8.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.8.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.8.2/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.8.2/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.8.2/ipfabric/diagrams/input_models/shared_view.py
--rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.8.2/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.8.2/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.8.2/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.8.2/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.8.2/ipfabric/exceptions.py
--rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.8.2/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    21346 2024-05-14 16:42:35.419308 ipfabric-6.8.2/ipfabric/models/device.py
--rw-r--r--   0        0        0     7694 2024-05-14 16:42:35.419308 ipfabric-6.8.2/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.8.2/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.8.2/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5827 2024-05-14 16:42:35.419308 ipfabric-6.8.2/ipfabric/models/jobs.py
--rw-r--r--   0        0        0     4469 2024-05-31 13:51:35.966239 ipfabric-6.8.2/ipfabric/models/oas.py
--rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.8.2/ipfabric/models/rbac.py
--rw-r--r--   0        0        0    27813 2024-05-14 16:42:35.419308 ipfabric-6.8.2/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0     5759 2024-05-14 16:42:35.419308 ipfabric-6.8.2/ipfabric/models/snapshots.py
--rw-r--r--   0        0        0    25314 2024-05-21 13:56:20.176258 ipfabric-6.8.2/ipfabric/models/table.py
--rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.8.2/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.8.2/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.8.2/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.8.2/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.8.2/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.8.2/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.8.2/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.8.2/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.8.2/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.8.2/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.8.2/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.8.2/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.8.2/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.8.2/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.8.2/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.8.2/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.8.2/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.8.2/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.8.2/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.8.2/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.8.2/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.8.2/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.8.2/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.8.2/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.8.2/ipfabric/models/users.py
--rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.8.2/ipfabric/oas/__init__.py
--rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.8.2/ipfabric/oas/v6.7.json
--rw-r--r--   0        0        0   390704 2024-05-14 16:42:35.426959 ipfabric-6.8.2/ipfabric/oas/v6.8.json
--rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.8.2/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3611 2024-05-14 16:42:35.426959 ipfabric-6.8.2/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     7607 2024-05-14 16:42:35.426959 ipfabric-6.8.2/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     9074 2024-05-14 16:42:35.433180 ipfabric-6.8.2/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1411 2024-05-14 16:42:35.435187 ipfabric-6.8.2/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     3232 2024-05-14 16:42:35.435876 ipfabric-6.8.2/ipfabric/settings/local_users.py
--rw-r--r--   0        0        0    14484 2024-05-14 16:42:35.435876 ipfabric-6.8.2/ipfabric/settings/rbac.py
--rw-r--r--   0        0        0     2255 2024-05-14 16:42:35.435876 ipfabric-6.8.2/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.8.2/ipfabric/settings/settings.py
--rw-r--r--   0        0        0     2111 2024-05-14 16:42:35.435876 ipfabric-6.8.2/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     4367 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     9192 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      687 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     8587 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5652 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.8.2/ipfabric/tools/managed_rbac/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/7/__init__.py
--rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/7/policies.json
--rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/7/roles.json
--rw-r--r--   0        0        0        0 2024-05-14 16:42:35.442401 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/8/__init__.py
--rw-r--r--   0        0        0    37983 2024-05-14 16:42:35.450957 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/8/policies.json
--rw-r--r--   0        0        0     3383 2024-05-14 16:42:35.450957 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/8/roles.json
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/__init__.py
--rw-r--r--   0        0        0     7166 2024-05-21 13:57:32.894570 ipfabric-6.8.2/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.8.2/ipfabric/tools/rbac.py
--rw-r--r--   0        0        0     4210 2024-05-14 16:42:35.452449 ipfabric-6.8.2/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0    24152 2024-05-14 16:42:35.452449 ipfabric-6.8.2/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.8.2/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.8.2/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.8.2/LICENSE
--rw-r--r--   0        0        0     3469 2024-05-14 16:42:35.403692 ipfabric-6.8.2/NOTICES.md
--rw-r--r--   0        0        0     3334 2024-05-31 13:51:35.970003 ipfabric-6.8.2/pyproject.toml
--rw-r--r--   0        0        0     6227 2024-05-14 16:42:35.403692 ipfabric-6.8.2/README.md
--rw-r--r--   0        0        0     8375 1970-01-01 00:00:00.000000 ipfabric-6.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.8.2b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0    11009 2024-05-14 16:42:35.403692 ipfabric-6.8.2b0/ipfabric/api.py
+-rw-r--r--   0        0        0    10301 2024-05-14 16:42:35.403692 ipfabric-6.8.2b0/ipfabric/auth.py
+-rw-r--r--   0        0        0    24100 2024-05-23 14:50:10.346521 ipfabric-6.8.2b0/ipfabric/client.py
+-rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.8.2b0/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0    18233 2024-05-14 16:42:35.403692 ipfabric-6.8.2b0/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.8.2b0/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.8.2b0/ipfabric/diagrams/input_models/shared_view.py
+-rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.8.2b0/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.8.2b0/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.8.2b0/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.8.2b0/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.8.2b0/ipfabric/exceptions.py
+-rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.8.2b0/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    21346 2024-05-14 16:42:35.419308 ipfabric-6.8.2b0/ipfabric/models/device.py
+-rw-r--r--   0        0        0     7694 2024-05-14 16:42:35.419308 ipfabric-6.8.2b0/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.8.2b0/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.8.2b0/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5827 2024-05-14 16:42:35.419308 ipfabric-6.8.2b0/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0     4207 2024-05-24 17:10:50.391576 ipfabric-6.8.2b0/ipfabric/models/oas.py
+-rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.8.2b0/ipfabric/models/rbac.py
+-rw-r--r--   0        0        0    27813 2024-05-14 16:42:35.419308 ipfabric-6.8.2b0/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0     5759 2024-05-14 16:42:35.419308 ipfabric-6.8.2b0/ipfabric/models/snapshots.py
+-rw-r--r--   0        0        0    25314 2024-05-21 13:56:20.176258 ipfabric-6.8.2b0/ipfabric/models/table.py
+-rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.8.2b0/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.8.2b0/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.8.2b0/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.8.2b0/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.8.2b0/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.8.2b0/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.8.2b0/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.8.2b0/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.8.2b0/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.8.2b0/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.8.2b0/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.8.2b0/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.8.2b0/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.8.2b0/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.8.2b0/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.8.2b0/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.8.2b0/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.8.2b0/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.8.2b0/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.8.2b0/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.8.2b0/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.8.2b0/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.8.2b0/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.8.2b0/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.8.2b0/ipfabric/models/users.py
+-rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.8.2b0/ipfabric/oas/__init__.py
+-rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.8.2b0/ipfabric/oas/v6.7.json
+-rw-r--r--   0        0        0   390704 2024-05-14 16:42:35.426959 ipfabric-6.8.2b0/ipfabric/oas/v6.8.json
+-rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.8.2b0/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3611 2024-05-14 16:42:35.426959 ipfabric-6.8.2b0/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     7607 2024-05-14 16:42:35.426959 ipfabric-6.8.2b0/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     9074 2024-05-14 16:42:35.433180 ipfabric-6.8.2b0/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1411 2024-05-14 16:42:35.435187 ipfabric-6.8.2b0/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     3232 2024-05-14 16:42:35.435876 ipfabric-6.8.2b0/ipfabric/settings/local_users.py
+-rw-r--r--   0        0        0    14484 2024-05-14 16:42:35.435876 ipfabric-6.8.2b0/ipfabric/settings/rbac.py
+-rw-r--r--   0        0        0     2255 2024-05-14 16:42:35.435876 ipfabric-6.8.2b0/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.8.2b0/ipfabric/settings/settings.py
+-rw-r--r--   0        0        0     2111 2024-05-14 16:42:35.435876 ipfabric-6.8.2b0/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     4367 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     9192 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      687 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     8587 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5652 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/7/__init__.py
+-rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/7/policies.json
+-rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/7/roles.json
+-rw-r--r--   0        0        0        0 2024-05-14 16:42:35.442401 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/8/__init__.py
+-rw-r--r--   0        0        0    37983 2024-05-14 16:42:35.450957 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/8/policies.json
+-rw-r--r--   0        0        0     3383 2024-05-14 16:42:35.450957 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/8/roles.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/__init__.py
+-rw-r--r--   0        0        0     7166 2024-05-21 13:57:32.894570 ipfabric-6.8.2b0/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.8.2b0/ipfabric/tools/rbac.py
+-rw-r--r--   0        0        0     4210 2024-05-14 16:42:35.452449 ipfabric-6.8.2b0/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0    24152 2024-05-14 16:42:35.452449 ipfabric-6.8.2b0/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.8.2b0/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.8.2b0/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.8.2b0/LICENSE
+-rw-r--r--   0        0        0     3469 2024-05-14 16:42:35.403692 ipfabric-6.8.2b0/NOTICES.md
+-rw-r--r--   0        0        0     3336 2024-05-24 17:13:20.735460 ipfabric-6.8.2b0/pyproject.toml
+-rw-r--r--   0        0        0     6227 2024-05-14 16:42:35.403692 ipfabric-6.8.2b0/README.md
+-rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 ipfabric-6.8.2b0/PKG-INFO
```

### Comparing `ipfabric-6.8.2/ipfabric/__init__.py` & `ipfabric-6.8.2b0/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/api.py` & `ipfabric-6.8.2b0/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Optional, Any, Union, Literal, List, Mapping, OrderedDict, Iterator
 
 from dotenv import find_dotenv
 from httpx import Client, BaseTransport, URL, Response
 from httpx._client import EventHook
 from httpx._types import CertTypes, VerifyTypes
-from pydantic import ConfigDict, Field, InstanceOf, FilePath
+from pydantic import ConfigDict, Field, InstanceOf
 from pydantic.dataclasses import dataclass
 
 from ipfabric.auth import Setup, ProxyTypes, TimeoutTypes, ProxiesTypes
 from ipfabric.exceptions import api_insuf_rights
 from ipfabric.models import Snapshot, OAS, Endpoint, Snapshots, Methods, User
 from ipfabric.tools import VALID_REFS, trigger_backup, raise_for_status
 
@@ -37,15 +37,14 @@
         timeout: httpx.Client - Default 5
         proxy: httpx.Client
         proxies: httpx.Client
         mounts: httpx.Client
         cert: httpx.Client
         event_hooks: httpx.Client
         local_oas: Default True, False mainly for development purposes
-        local_oas_file: Default True, False mainly for development purposes
         debug: Future use.
     """
 
     base_url: Optional[Union[str, InstanceOf[URL]]] = Field(
         None, description="Base URL of the IPF instance", examples=["https://demo.ipfabric.io"]
     )
     api_version: Optional[str] = Field(None, description="Defaults to SDK or API version.")
@@ -58,15 +57,14 @@
     timeout: InitVar[Optional[Union[TimeoutTypes, Literal["DEFAULT"]]]] = field(default="DEFAULT")
     proxy: InitVar[Optional[ProxyTypes]] = field(default=None)
     proxies: InitVar[Optional[ProxiesTypes]] = field(default=None)
     mounts: InitVar[Optional[Mapping[str, Optional[BaseTransport]]]] = field(default=None)
     cert: InitVar[Optional[CertTypes]] = field(default=None)
     event_hooks: InitVar[Optional[Mapping[str, List[EventHook]]]] = field(default=None)
     local_oas: bool = Field(True, description="Default True, use local minified OAS file instead of servers.")
-    local_oas_file: Optional[FilePath] = None
     debug: Optional[bool] = None
     http2: InitVar[Optional[bool]] = field(default=True)
     _os_version: Optional[str] = None
     _client: Client = None
     _prev_snapshot_id: Optional[str] = None
     _attribute_filters: Optional[dict] = None
     _no_loaded_snapshots: bool = False
@@ -101,15 +99,15 @@
             cert=cert,
             event_hooks=event_hooks,
             debug=self.debug,
             http2=http2,
         )
         [setattr(self, k, v) for k, v in setup.update_attrs.items()]
 
-        self._oas = OAS(client=self, local_oas=self.local_oas, local_oas_file=self.local_oas_file)
+        self._oas = OAS(client=self, local_oas=self.local_oas)
         self._user = self.get_user()
         self._snapshots = Snapshots(client=self)
         self.snapshot_id = setup.snapshot_id
         logger.debug(
             f"Successfully connected to '{self.base_url.host}' IPF version '{self.os_version}' "
             f"as user '{self.user.username}'"
         )
```

### Comparing `ipfabric-6.8.2/ipfabric/auth.py` & `ipfabric-6.8.2b0/ipfabric/auth.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/client.py` & `ipfabric-6.8.2b0/ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/__init__.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/graphs.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/icmp.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/__init__.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/constants.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/input_models/shared_view.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/input_models/shared_view.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/output_models/protocols.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/diagrams/output_models/trace.py` & `ipfabric-6.8.2b0/ipfabric/diagrams/output_models/trace.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/exceptions.py` & `ipfabric-6.8.2b0/ipfabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/__init__.py` & `ipfabric-6.8.2b0/ipfabric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/device.py` & `ipfabric-6.8.2b0/ipfabric/models/device.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/intent.py` & `ipfabric-6.8.2b0/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/intent_check.py` & `ipfabric-6.8.2b0/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/inventory.py` & `ipfabric-6.8.2b0/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/jobs.py` & `ipfabric-6.8.2b0/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/oas.py` & `ipfabric-6.8.2b0/ipfabric/models/oas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import json
 from typing import Optional, List, Any, Dict
 
-from pydantic import BaseModel, PrivateAttr, TypeAdapter, computed_field, Field, FilePath
+from pydantic import BaseModel, PrivateAttr, TypeAdapter, computed_field, Field
 
 from ipfabric.tools import raise_for_status
 
 try:
     from importlib.resources import files
 except ImportError:
     from importlib_resources import files
@@ -36,26 +35,25 @@
     post: Optional[Endpoint] = None
     delete: Optional[Endpoint] = None
 
 
 class OAS(BaseModel):
     client: Any = Field(exclude=True)
     local_oas: bool = True
-    local_oas_file: Optional[FilePath] = None
     _oas: Dict[str, Methods] = PrivateAttr(default_factory=dict)
 
     def model_post_init(self, __context) -> None:
         self._oas = self._get_oas()
 
     @property
     def oas(self) -> Dict[str, Methods]:
         return self._oas
 
     def _get_oas(self) -> Dict[str, Methods]:
-        if not self.local_oas or (self.local_oas_file and self.local_oas):
+        if not self.local_oas:
             return self._parse_oas()
         try:
             min_oas = OAS_DIR.joinpath(self.client.api_version + ".json").read_text()
             oas = TypeAdapter(Dict[str, Methods]).validate_json(min_oas)
             return oas
         except FileNotFoundError:
             return self._parse_oas()
@@ -99,24 +97,20 @@
             ]
             data.nested_columns = [k for k, v in columns.items() if "type" in v and v["type"] == "array"]
         except KeyError:
             pass
         return data
 
     def _parse_oas(self) -> Dict[str, Methods]:
-        if not self.local_oas:
-            oas = raise_for_status(
-                self.client.get(self.client.base_url.join("/api/oas/openapi-extended.json"), follow_redirects=True)
-            ).json()
-        else:
-            with open(self.local_oas_file, 'r') as f:
-                oas = json.load(f)
+        resp = raise_for_status(
+            self.client.get(self.client.base_url.join("/api/oas/openapi-extended.json"), follow_redirects=True)
+        )
 
         endpoints = dict()
-        for endpoint, methods in oas["paths"].items():
+        for endpoint, methods in resp.json()["paths"].items():
             methods_obj = Methods(api_endpoint=endpoint)
             for method, spec in methods.items():
                 data = Endpoint(
                     api_endpoint=endpoint[1:],
                     method=method,
                     api_scope_id=spec.get("x-apiScopeId", None),
                     summary=spec.get("summary", None),
```

### Comparing `ipfabric-6.8.2/ipfabric/models/rbac.py` & `ipfabric-6.8.2b0/ipfabric/models/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/snapshot.py` & `ipfabric-6.8.2b0/ipfabric/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/snapshots.py` & `ipfabric-6.8.2b0/ipfabric/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/table.py` & `ipfabric-6.8.2b0/ipfabric/models/table.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/__init__.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/addressing.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/cloud.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/cloud.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/dhcp.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/fhrp.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/interfaces.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/managed_networks.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/managed_networks.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/management.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/mpls.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/multicast.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/neighbors.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/oam.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/platforms.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/port_channels.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/qos.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/routing.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/sdn.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/sdwan.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/sdwan.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/security.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/stp.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/vlans.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/technology/wireless.py` & `ipfabric-6.8.2b0/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/models/users.py` & `ipfabric-6.8.2b0/ipfabric/models/users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/oas/v6.7.json` & `ipfabric-6.8.2b0/ipfabric/oas/v6.7.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/oas/v6.8.json` & `ipfabric-6.8.2b0/ipfabric/oas/v6.8.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/__init__.py` & `ipfabric-6.8.2b0/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/api_tokens.py` & `ipfabric-6.8.2b0/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/attributes.py` & `ipfabric-6.8.2b0/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/authentication.py` & `ipfabric-6.8.2b0/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/discovery.py` & `ipfabric-6.8.2b0/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/local_users.py` & `ipfabric-6.8.2b0/ipfabric/settings/local_users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/rbac.py` & `ipfabric-6.8.2b0/ipfabric/settings/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/seeds.py` & `ipfabric-6.8.2b0/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/settings.py` & `ipfabric-6.8.2b0/ipfabric/settings/settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/site_separation.py` & `ipfabric-6.8.2b0/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/vendor_api.py` & `ipfabric-6.8.2b0/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.8.2b0/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/__init__.py` & `ipfabric-6.8.2b0/ipfabric/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/configuration.py` & `ipfabric-6.8.2b0/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/discovery_history.py` & `ipfabric-6.8.2b0/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/7/policies.json` & `ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/7/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/7/roles.json` & `ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/7/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/8/policies.json` & `ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/8/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/managed_rbac/v6/8/roles.json` & `ipfabric-6.8.2b0/ipfabric/tools/managed_rbac/v6/8/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/nist.py` & `ipfabric-6.8.2b0/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/rbac.py` & `ipfabric-6.8.2b0/ipfabric/tools/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/restore_intents.py` & `ipfabric-6.8.2b0/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/shared.py` & `ipfabric-6.8.2b0/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.8.2b0/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.8.2b0/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/LICENSE` & `ipfabric-6.8.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/NOTICES.md` & `ipfabric-6.8.2b0/NOTICES.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/pyproject.toml` & `ipfabric-6.8.2b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.8.2"
+version = "v6.8.2b0"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.8.2/README.md` & `ipfabric-6.8.2b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.2/PKG-INFO` & `ipfabric-6.8.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.8.2
+Version: 6.8.2b0
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.8,<4.0
```

