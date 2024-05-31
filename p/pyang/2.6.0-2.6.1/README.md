# Comparing `tmp/pyang-2.6.0.tar.gz` & `tmp/pyang-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyang-2.6.0.tar", last modified: Fri Nov  3 10:07:58 2023, max compression
+gzip compressed data, was "pyang-2.6.1.tar", last modified: Thu May 23 11:59:03 2024, max compression
```

## Comparing `pyang-2.6.0.tar` & `pyang-2.6.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.836672 pyang-2.6.0/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      756 2020-05-06 12:00:50.000000 pyang-2.6.0/LICENSE
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      204 2020-05-06 12:00:50.000000 pyang-2.6.0/MANIFEST.in
--rw-r--r--   0 mbj       (1000) mbj       (1000)      818 2023-11-03 10:07:58.836672 pyang-2.6.0/PKG-INFO
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5871 2023-11-03 09:53:35.000000 pyang-2.6.0/README.md
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.808675 pyang-2.6.0/bin/
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)      202 2023-11-03 09:53:35.000000 pyang-2.6.0/bin/json2xml
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)      202 2023-11-03 09:53:35.000000 pyang-2.6.0/bin/pyang
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)     9065 2023-01-13 07:54:15.000000 pyang-2.6.0/bin/yang2dsdl
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)      201 2023-11-03 09:53:35.000000 pyang-2.6.0/bin/yang2html
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      321 2023-11-03 08:44:08.000000 pyang-2.6.0/env.sh
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.804675 pyang-2.6.0/etc/
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.808675 pyang-2.6.0/etc/bash_completion.d/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6918 2022-03-30 08:12:45.000000 pyang-2.6.0/etc/bash_completion.d/pyang
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.804675 pyang-2.6.0/man/
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.808675 pyang-2.6.0/man/man1/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2507 2023-11-03 10:07:58.000000 pyang-2.6.0/man/man1/json2xml.1
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    41904 2023-11-03 10:07:58.000000 pyang-2.6.0/man/man1/pyang.1
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9055 2023-11-03 10:07:58.000000 pyang-2.6.0/man/man1/yang2dsdl.1
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.804675 pyang-2.6.0/modules/
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.808675 pyang-2.6.0/modules/iana/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4221 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/iana/iana-crypt-hash.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6140 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/iana/iana-hardware.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    38804 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/iana/iana-if-type.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10315 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/iana/iana-routing-types.yang
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.820674 pyang-2.6.0/modules/ietf/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    19816 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-access-control-list.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2065 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-acldns.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    18482 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-alarms-x733.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    53040 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-alarms.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2679 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-datastores.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10887 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-dslite.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    11242 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-ethertypes.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    25166 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-hardware-state.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    37326 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-hardware.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    56395 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-i2rs-rib.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    16829 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-inet-types.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    39363 2021-03-17 13:55:01.000000 pyang-2.6.0/modules/ietf/ietf-interfaces.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    27499 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-ip.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    11610 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-ipv4-unicast-routing.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17395 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-ipv6-router-advertisements.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    11886 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-ipv6-unicast-routing.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10302 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-key-chain.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)   102689 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-l2vpn-svc.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5073 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-l3-unicast-topology-state.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9867 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-l3-unicast-topology.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    86476 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-l3vpn-svc.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9113 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-lmap-common.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    29988 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-lmap-control.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6629 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-lmap-report.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5072 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-logical-network-element.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9171 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-mud.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    71354 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-nat.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    13282 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-netconf-acm.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17412 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-netconf-monitoring.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    12507 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-netconf-nmda.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10497 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-netconf-notifications.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     3926 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-netconf-with-defaults.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    26738 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-netconf.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     8951 2021-03-17 13:55:01.000000 pyang-2.6.0/modules/ietf/ietf-network-instance.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5522 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-network-state.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9641 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-network-topology-state.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10304 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-network-topology.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6073 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-network.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     3912 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-origin.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17468 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-packet-fields.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4397 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-restconf-monitoring.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     8743 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-restconf.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    24477 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-routing-types.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    20539 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-routing.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4944 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-common.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     7486 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-snmp-community.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4316 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-engine.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6383 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-notification.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4671 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-proxy.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4398 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-ssh.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6663 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-target.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6831 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-tls.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     3220 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-tsm.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6141 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-usm.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10289 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp-vacm.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2131 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-snmp.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    46634 2021-03-17 13:41:01.000000 pyang-2.6.0/modules/ietf/ietf-subscribed-notifications.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    24191 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-system.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9399 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-voucher.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    31146 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-vrrp.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    11033 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-x509-cert-to-name.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    16438 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-yang-library.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2953 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-yang-metadata.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    13133 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-yang-patch.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    27270 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-yang-push.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     7779 2020-05-06 12:00:50.000000 pyang-2.6.0/modules/ietf/ietf-yang-schema-mount.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5003 2019-03-15 15:08:34.000000 pyang-2.6.0/modules/ietf/ietf-yang-smiv2.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     7504 2020-07-01 07:57:34.000000 pyang-2.6.0/modules/ietf/ietf-yang-structure-ext.yang
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17933 2021-03-15 12:51:27.000000 pyang-2.6.0/modules/ietf/ietf-yang-types.yang
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.824673 pyang-2.6.0/pyang/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      124 2023-11-03 10:05:50.000000 pyang-2.6.0/pyang/__init__.py
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)      101 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/__main__.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    14056 2023-11-03 08:44:08.000000 pyang-2.6.0/pyang/context.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17316 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/error.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    25236 2023-11-03 08:03:52.000000 pyang-2.6.0/pyang/grammar.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4367 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/hello.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5962 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugin.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.828673 pyang-2.6.0/pyang/plugins/
--rw-r--r--   0 mbj       (1000) mbj       (1000)        0 2015-03-16 14:26:20.000000 pyang-2.6.0/pyang/plugins/__init__.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1116 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/bbf.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2089 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/capability.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    30946 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/check_update.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4850 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/depend.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17389 2022-03-30 08:42:54.000000 pyang-2.6.0/pyang/plugins/flatten.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     3294 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/identifiers.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1537 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/ieee.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     7093 2022-03-30 08:12:45.000000 pyang-2.6.0/pyang/plugins/ietf.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10230 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/jsonxsl.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    35804 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/jstree.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4332 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/jtox.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    12079 2023-11-03 09:56:35.000000 pyang-2.6.0/pyang/plugins/lint.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1010 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/mef.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1278 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/metadata.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1410 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/name.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    11901 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/omni.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     2381 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/restconf.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     9164 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/sample-xml-skeleton.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    35354 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/sid.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4114 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/plugins/smi.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     1913 2020-07-01 07:57:34.000000 pyang-2.6.0/pyang/plugins/structure.py
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)    11115 2022-03-30 08:12:45.000000 pyang-2.6.0/pyang/plugins/threegpp.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    23245 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/tree.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    61455 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/plugins/uml.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5740 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/repository.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.832672 pyang-2.6.0/pyang/scripts/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)        0 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/scripts/__init__.py
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)    16732 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/scripts/json2xml.py
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)    23151 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/scripts/pyang_tool.py
--rwxrwxr-x   0 mbj       (1000) mbj       (1000)     5388 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/scripts/yang2html.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)   136002 2023-11-03 10:05:03.000000 pyang-2.6.0/pyang/statements.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    14558 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/syntax.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.832672 pyang-2.6.0/pyang/transforms/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      108 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/transforms/__init__.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    12718 2022-03-30 08:12:45.000000 pyang-2.6.0/pyang/transforms/edit.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.832672 pyang-2.6.0/pyang/translators/
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      270 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/translators/__init__.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    51923 2023-11-03 08:44:08.000000 pyang-2.6.0/pyang/translators/dsdl.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    10505 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/translators/schemanode.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    17389 2022-03-30 08:12:45.000000 pyang-2.6.0/pyang/translators/yang.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6251 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/translators/yin.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    36775 2023-11-03 08:44:08.000000 pyang-2.6.0/pyang/types.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     4899 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/util.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    15435 2023-11-03 08:44:08.000000 pyang-2.6.0/pyang/xpath.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     6276 2020-05-06 12:00:50.000000 pyang-2.6.0/pyang/xpath_lexer.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     8996 2022-03-30 08:12:45.000000 pyang-2.6.0/pyang/xpath_parser.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)   137467 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/yacc.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    14677 2023-11-03 09:53:35.000000 pyang-2.6.0/pyang/yang_parser.py
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    14580 2023-11-02 10:31:12.000000 pyang-2.6.0/pyang/yin_parser.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.824673 pyang-2.6.0/pyang.egg-info/
--rw-r--r--   0 mbj       (1000) mbj       (1000)      818 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/PKG-INFO
--rw-r--r--   0 mbj       (1000) mbj       (1000)     4936 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/SOURCES.txt
--rw-r--r--   0 mbj       (1000) mbj       (1000)        1 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/dependency_links.txt
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      134 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/entry_points.txt
--rw-r--r--   0 mbj       (1000) mbj       (1000)        5 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/requires.txt
--rw-r--r--   0 mbj       (1000) mbj       (1000)        6 2023-11-03 10:07:58.000000 pyang-2.6.0/pyang.egg-info/top_level.txt
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.832672 pyang-2.6.0/schema/
--rw-r--r--   0 mbj       (1000) mbj       (1000)     1695 2015-03-16 14:26:20.000000 pyang-2.6.0/schema/edit-config-attributes.rng
--rw-r--r--   0 mbj       (1000) mbj       (1000)     1462 2015-03-16 14:26:20.000000 pyang-2.6.0/schema/hello-server.rng
--rw-r--r--   0 mbj       (1000) mbj       (1000)     2274 2015-05-16 13:29:21.000000 pyang-2.6.0/schema/relaxng-lib.rng
--rw-rw-r--   0 mbj       (1000) mbj       (1000)      170 2023-11-03 10:07:58.836672 pyang-2.6.0/setup.cfg
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     3709 2023-11-03 09:53:35.000000 pyang-2.6.0/setup.py
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.808675 pyang-2.6.0/tools/
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.832672 pyang-2.6.0/tools/images/
--rw-r--r--   0 mbj       (1000) mbj       (1000)      561 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/case.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)     1293 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/choice.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      774 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/container.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      152 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/file.gif
--rw-r--r--   0 mbj       (1000) mbj       (1000)      581 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/focus.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      220 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/folder-closed.gif
--rw-r--r--   0 mbj       (1000) mbj       (1000)      229 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/folder-open.gif
--rw-r--r--   0 mbj       (1000) mbj       (1000)      278 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/hammer.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      639 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/leaf-list.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      639 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/leaf-plus.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      573 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/leaf.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)     1222 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/leafref.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      514 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/list.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      807 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/module.png
--rw-r--r--   0 mbj       (1000) mbj       (1000)      536 2015-03-16 14:26:20.000000 pyang-2.6.0/tools/images/notification.png
-drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2023-11-03 10:07:58.836672 pyang-2.6.0/xslt/
--rw-r--r--   0 mbj       (1000) mbj       (1000)      544 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/basename.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)     3426 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/dsrl2xslt.xsl
--rw-rw-r--   0 mbj       (1000) mbj       (1000)     5058 2020-05-06 12:00:50.000000 pyang-2.6.0/xslt/gen-common.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)    18537 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/gen-dsrl.xsl
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    16569 2020-05-06 12:00:50.000000 pyang-2.6.0/xslt/gen-relaxng.xsl
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    25842 2020-05-06 12:00:50.000000 pyang-2.6.0/xslt/gen-schematron.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)    10923 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/iso_abstract_expand.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)    73713 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/iso_schematron_skeleton_for_xslt1.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)    21176 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/iso_svrl_for_xslt1.xsl
--rw-rw-r--   0 mbj       (1000) mbj       (1000)    21796 2020-05-06 12:00:50.000000 pyang-2.6.0/xslt/jsonxsl-templates.xsl
--rw-r--r--   0 mbj       (1000) mbj       (1000)     2374 2015-03-16 14:26:20.000000 pyang-2.6.0/xslt/svrl2text.xsl
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.239437 pyang-2.6.1/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      756 2020-05-06 12:00:50.000000 pyang-2.6.1/LICENSE
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      204 2020-05-06 12:00:50.000000 pyang-2.6.1/MANIFEST.in
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      821 2024-05-23 11:59:03.239437 pyang-2.6.1/PKG-INFO
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5871 2024-03-12 09:33:15.000000 pyang-2.6.1/README.md
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.213440 pyang-2.6.1/bin/
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)      202 2024-03-12 09:33:15.000000 pyang-2.6.1/bin/json2xml
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)      202 2024-03-12 09:33:15.000000 pyang-2.6.1/bin/pyang
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)     9065 2023-01-13 07:54:15.000000 pyang-2.6.1/bin/yang2dsdl
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)      201 2024-03-12 09:33:15.000000 pyang-2.6.1/bin/yang2html
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      351 2024-05-23 11:12:22.000000 pyang-2.6.1/env.sh
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.210440 pyang-2.6.1/etc/
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.213440 pyang-2.6.1/etc/bash_completion.d/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6918 2024-03-12 09:33:15.000000 pyang-2.6.1/etc/bash_completion.d/pyang
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.210440 pyang-2.6.1/man/
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.214440 pyang-2.6.1/man/man1/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2747 2024-05-23 11:59:02.000000 pyang-2.6.1/man/man1/json2xml.1
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    42114 2024-05-23 11:59:02.000000 pyang-2.6.1/man/man1/pyang.1
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9295 2024-05-23 11:59:02.000000 pyang-2.6.1/man/man1/yang2dsdl.1
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.211440 pyang-2.6.1/modules/
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.214440 pyang-2.6.1/modules/iana/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4221 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/iana/iana-crypt-hash.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6140 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/iana/iana-hardware.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    38804 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/iana/iana-if-type.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10315 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/iana/iana-routing-types.yang
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.225439 pyang-2.6.1/modules/ietf/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    19816 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-access-control-list.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2065 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-acldns.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    18482 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-alarms-x733.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    53040 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-alarms.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2679 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-datastores.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10887 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-dslite.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    11242 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-ethertypes.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    25166 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-hardware-state.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    37326 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-hardware.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    56395 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-i2rs-rib.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    16829 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-inet-types.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    39363 2021-03-17 13:55:01.000000 pyang-2.6.1/modules/ietf/ietf-interfaces.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    27499 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-ip.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    11610 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-ipv4-unicast-routing.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17395 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-ipv6-router-advertisements.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    11886 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-ipv6-unicast-routing.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10302 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-key-chain.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)   102689 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-l2vpn-svc.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5073 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-l3-unicast-topology-state.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9867 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-l3-unicast-topology.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    86476 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-l3vpn-svc.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9113 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-lmap-common.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    29988 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-lmap-control.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6629 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-lmap-report.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5072 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-logical-network-element.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9171 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-mud.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    71354 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-nat.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    13282 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-netconf-acm.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17412 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-netconf-monitoring.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    12507 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-netconf-nmda.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10497 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-netconf-notifications.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     3926 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-netconf-with-defaults.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    26738 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-netconf.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     8951 2021-03-17 13:55:01.000000 pyang-2.6.1/modules/ietf/ietf-network-instance.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5522 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-network-state.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9641 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-network-topology-state.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10304 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-network-topology.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6073 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-network.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     3912 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-origin.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17468 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-packet-fields.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4397 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-restconf-monitoring.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     8743 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-restconf.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    24477 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-routing-types.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    20539 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-routing.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4944 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-common.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     7486 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-snmp-community.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4316 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-engine.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6383 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-notification.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4671 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-proxy.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4398 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-ssh.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6663 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-target.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6831 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-tls.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     3220 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-tsm.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6141 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-usm.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10289 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp-vacm.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2131 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-snmp.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    46634 2021-03-17 13:41:01.000000 pyang-2.6.1/modules/ietf/ietf-subscribed-notifications.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    24191 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-system.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9399 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-voucher.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    31146 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-vrrp.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    11033 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-x509-cert-to-name.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    16438 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-yang-library.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2953 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-yang-metadata.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    13133 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-yang-patch.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    27270 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-yang-push.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     7779 2020-05-06 12:00:50.000000 pyang-2.6.1/modules/ietf/ietf-yang-schema-mount.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5003 2019-03-15 15:08:34.000000 pyang-2.6.1/modules/ietf/ietf-yang-smiv2.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     7504 2020-07-01 07:57:34.000000 pyang-2.6.1/modules/ietf/ietf-yang-structure-ext.yang
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17933 2021-03-15 12:51:27.000000 pyang-2.6.1/modules/ietf/ietf-yang-types.yang
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.228438 pyang-2.6.1/pyang/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      124 2024-05-23 11:56:10.000000 pyang-2.6.1/pyang/__init__.py
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)      101 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/__main__.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    14056 2024-05-23 11:09:42.000000 pyang-2.6.1/pyang/context.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17316 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/error.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    25236 2023-11-03 08:03:52.000000 pyang-2.6.1/pyang/grammar.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4367 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/hello.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5962 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugin.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.233438 pyang-2.6.1/pyang/plugins/
+-rw-r--r--   0 mbj       (1000) mbj       (1000)        0 2015-03-16 14:26:20.000000 pyang-2.6.1/pyang/plugins/__init__.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     1116 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/bbf.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2089 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/capability.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    31890 2024-05-23 11:25:41.000000 pyang-2.6.1/pyang/plugins/check_update.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4850 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/depend.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17389 2022-03-30 08:42:54.000000 pyang-2.6.1/pyang/plugins/flatten.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     3294 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/identifiers.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2013 2024-05-12 09:16:07.000000 pyang-2.6.1/pyang/plugins/ieee.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     7093 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/ietf.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10230 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/jsonxsl.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    35804 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/jstree.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4332 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/jtox.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    12079 2023-11-03 09:56:35.000000 pyang-2.6.1/pyang/plugins/lint.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     1010 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/mef.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     1278 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/metadata.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     1410 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/name.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    11901 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/omni.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     2381 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/restconf.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     9164 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/sample-xml-skeleton.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    35354 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/plugins/sid.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4114 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/plugins/smi.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     1913 2020-07-01 07:57:34.000000 pyang-2.6.1/pyang/plugins/structure.py
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)    11115 2022-03-30 08:12:45.000000 pyang-2.6.1/pyang/plugins/threegpp.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    23260 2024-03-12 09:57:25.000000 pyang-2.6.1/pyang/plugins/tree.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    61455 2024-03-12 09:57:25.000000 pyang-2.6.1/pyang/plugins/uml.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5740 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/repository.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.233438 pyang-2.6.1/pyang/scripts/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)        0 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/scripts/__init__.py
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)    16732 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/scripts/json2xml.py
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)    23151 2024-05-23 11:09:42.000000 pyang-2.6.1/pyang/scripts/pyang_tool.py
+-rwxrwxr-x   0 mbj       (1000) mbj       (1000)     5388 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/scripts/yang2html.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)   136238 2024-03-12 14:11:30.000000 pyang-2.6.1/pyang/statements.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    14558 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/syntax.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.234438 pyang-2.6.1/pyang/transforms/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      108 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/transforms/__init__.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    12718 2022-03-30 08:12:45.000000 pyang-2.6.1/pyang/transforms/edit.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.234438 pyang-2.6.1/pyang/translators/
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      270 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/translators/__init__.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    51923 2023-11-03 13:15:59.000000 pyang-2.6.1/pyang/translators/dsdl.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    10505 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/translators/schemanode.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    17389 2024-05-23 11:09:42.000000 pyang-2.6.1/pyang/translators/yang.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6251 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/translators/yin.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    36775 2023-11-03 13:15:59.000000 pyang-2.6.1/pyang/types.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     4899 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/util.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    15435 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/xpath.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     6276 2020-05-06 12:00:50.000000 pyang-2.6.1/pyang/xpath_lexer.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     8996 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/xpath_parser.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)   137467 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/yacc.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    14677 2024-03-12 09:33:15.000000 pyang-2.6.1/pyang/yang_parser.py
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    14580 2023-11-02 10:31:12.000000 pyang-2.6.1/pyang/yin_parser.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.239437 pyang-2.6.1/pyang.egg-info/
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      821 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/PKG-INFO
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     4936 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/SOURCES.txt
+-rw-r--r--   0 mbj       (1000) mbj       (1000)        1 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      134 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/entry_points.txt
+-rw-r--r--   0 mbj       (1000) mbj       (1000)        5 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/requires.txt
+-rw-r--r--   0 mbj       (1000) mbj       (1000)        6 2024-05-23 11:59:03.000000 pyang-2.6.1/pyang.egg-info/top_level.txt
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.235438 pyang-2.6.1/schema/
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     1695 2015-03-16 14:26:20.000000 pyang-2.6.1/schema/edit-config-attributes.rng
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     1462 2015-03-16 14:26:20.000000 pyang-2.6.1/schema/hello-server.rng
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     2274 2015-05-16 13:29:21.000000 pyang-2.6.1/schema/relaxng-lib.rng
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)      170 2024-05-23 11:59:03.240437 pyang-2.6.1/setup.cfg
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     3712 2024-05-23 11:09:42.000000 pyang-2.6.1/setup.py
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.212440 pyang-2.6.1/tools/
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.237438 pyang-2.6.1/tools/images/
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      561 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/case.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     1293 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/choice.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      774 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/container.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      152 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/file.gif
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      581 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/focus.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      220 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/folder-closed.gif
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      229 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/folder-open.gif
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      278 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/hammer.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      639 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/leaf-list.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      639 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/leaf-plus.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      573 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/leaf.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     1222 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/leafref.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      514 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/list.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      807 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/module.png
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      536 2015-03-16 14:26:20.000000 pyang-2.6.1/tools/images/notification.png
+drwxrwxr-x   0 mbj       (1000) mbj       (1000)        0 2024-05-23 11:59:03.239437 pyang-2.6.1/xslt/
+-rw-r--r--   0 mbj       (1000) mbj       (1000)      544 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/basename.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     3426 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/dsrl2xslt.xsl
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)     5058 2020-05-06 12:00:50.000000 pyang-2.6.1/xslt/gen-common.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)    18537 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/gen-dsrl.xsl
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    16569 2020-05-06 12:00:50.000000 pyang-2.6.1/xslt/gen-relaxng.xsl
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    25842 2020-05-06 12:00:50.000000 pyang-2.6.1/xslt/gen-schematron.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)    10923 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/iso_abstract_expand.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)    73713 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/iso_schematron_skeleton_for_xslt1.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)    21176 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/iso_svrl_for_xslt1.xsl
+-rw-rw-r--   0 mbj       (1000) mbj       (1000)    21796 2020-05-06 12:00:50.000000 pyang-2.6.1/xslt/jsonxsl-templates.xsl
+-rw-r--r--   0 mbj       (1000) mbj       (1000)     2374 2015-03-16 14:26:20.000000 pyang-2.6.1/xslt/svrl2text.xsl
```

### Comparing `pyang-2.6.0/LICENSE` & `pyang-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/PKG-INFO` & `pyang-2.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyang
-Version: 2.6.0
+Version: 2.6.1
 Summary: A YANG (RFC 6020/7950) validator and converter
 Home-page: https://github.com/mbj4668/pyang
 Author: Martin Bjorklund
-Author-email: mbj@tail-f.com
+Author-email: mbj4668@gmail.com
 License: BSD
 Keywords: YANG validator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyang-2.6.0/README.md` & `pyang-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/bin/yang2dsdl` & `pyang-2.6.1/bin/yang2dsdl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/etc/bash_completion.d/pyang` & `pyang-2.6.1/etc/bash_completion.d/pyang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/man/man1/json2xml.1` & `pyang-2.6.1/man/man1/json2xml.1`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,24 @@
-.\" Automatically generated by Pandoc 2.9.2.1
+.\" Automatically generated by Pandoc 3.1.3
 .\"
-.TH "JSON2XML" "1" "2023-11-03" "json2xml-2.6.0" "User Manual"
+.\" Define V font for inline verbatim, using C font in formats
+.\" that render this, and otherwise B font.
+.ie "\f[CB]x\f[]"x" \{\
+. ftr V B
+. ftr VI BI
+. ftr VB B
+. ftr VBI BI
+.\}
+.el \{\
+. ftr V CR
+. ftr VI CI
+. ftr VB CB
+. ftr VBI CBI
+.\}
+.TH "JSON2XML" "1" "2024-05-23" "json2xml-2.6.1" "User Manual"
 .hy
 .SH NAME
 .PP
 json2xml - translates JSON documents conforming to a YANG data model
 into XML.
 .SH SYNOPSIS
 .PP
```

### Comparing `pyang-2.6.0/man/man1/pyang.1` & `pyang-2.6.1/man/man1/pyang.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,24 @@
-.\" Automatically generated by Pandoc 2.9.2.1
+.\" Automatically generated by Pandoc 3.1.3
 .\"
-.TH "PYANG" "1" "2023-11-03" "pyang-2.6.0" "User Manual"
+.\" Define V font for inline verbatim, using C font in formats
+.\" that render this, and otherwise B font.
+.ie "\f[CB]x\f[]"x" \{\
+. ftr V B
+. ftr VI BI
+. ftr VB B
+. ftr VBI BI
+.\}
+.el \{\
+. ftr V CR
+. ftr VI CI
+. ftr VB CB
+. ftr VBI CBI
+.\}
+.TH "PYANG" "1" "2024-05-23" "pyang-2.6.1" "User Manual"
 .hy
 .SH NAME
 .PP
 pyang - validate and convert YANG modules to various formats
 .SH SYNOPSIS
 .PP
 \f[B]pyang\f[R] [--verbose] [--canonical] [--strict] [--lint] [--ietf]
@@ -344,15 +358,15 @@
 .IP "1." 3
 current directory
 .IP "2." 3
 \f[B]$YANG_MODPATH\f[R]
 .IP "3." 3
 \f[B]$HOME\f[R]/yang/modules
 .IP "4." 3
-\f[B]\f[BI]Y\f[B]\f[BI]A\f[B]\f[BI]N\f[B]\f[BI]G\f[B]_\f[BI]I\f[B]\f[BI]N\f[B]\f[BI]S\f[B]\f[BI]T\f[B]\f[BI]A\f[B]\f[BI]L\f[B]\f[BI]L\f[B]\[u2005]*\[u2005]\[u2005]*\[u2005]/\f[BI]y\f[B]\f[BI]a\f[B]\f[BI]n\f[B]\f[BI]g\f[B]/\f[BI]m\f[B]\f[BI]o\f[B]\f[BI]d\f[B]\f[BI]u\f[B]\f[BI]l\f[B]\f[BI]e\f[B]\f[BI]s\f[B]\f[BI]O\f[B]\f[BI]R\f[B]\f[BI]i\f[B]\f[BI]f\f[B]\[u2005]*\[u2005]*YANG_INSTALL\f[R]
+\f[B]\f[BI]Y\f[B]\f[BI]A\f[B]\f[BI]N\f[B]\f[BI]G\f[B]_\f[BI]I\f[B]\f[BI]N\f[B]\f[BI]S\f[B]\f[BI]T\f[B]\f[BI]A\f[B]\f[BI]L\f[B]\f[BI]L\f[B] *  * /\f[BI]y\f[B]\f[BI]a\f[B]\f[BI]n\f[B]\f[BI]g\f[B]/\f[BI]m\f[B]\f[BI]o\f[B]\f[BI]d\f[B]\f[BI]u\f[B]\f[BI]l\f[B]\f[BI]e\f[B]\f[BI]s\f[B]\f[BI]O\f[B]\f[BI]R\f[B]\f[BI]i\f[B]\f[BI]f\f[B] * *YANG_INSTALL\f[R]
 is unset <the default installation directory>/yang/modules (on Unix
 systems: /usr/share/yang/modules)
 .RE
 .TP
 \f[B]--no-path-recurse\f[R]
 If this parameter is given, directories in the search path are not
 recursively scanned for modules.
@@ -1070,15 +1084,16 @@
 .TP
 \f[B]--flatten-qualified-in-xpath\f[R]
 Output the qualified XPath i.e.,
 /module1:root/module1:node/module2:node/\&...
 .TP
 \f[B]--flatten-qualified-module-and-prefix-path\f[R]
 Output an XPath with both module and prefix i.e.,
-/module1:prefix1:root/\&... This is NOT a colloquial syntax of XPath.
+/module1:prefix1:root/\&...
+This is NOT a colloquial syntax of XPath.
 Emitted separately.
 .TP
 \f[B]--flatten-deviated\f[R]
 Flatten all data keywords instead of only data definition keywords.
 .TP
 \f[B]--flatten-filter-keyword\f[R] \f[I]keyword\f[R]
 Filter output to only desired keywords.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyang-2.6.0/man/man1/yang2dsdl.1` & `pyang-2.6.1/man/man1/yang2dsdl.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,24 @@
-.\" Automatically generated by Pandoc 2.9.2.1
+.\" Automatically generated by Pandoc 3.1.3
 .\"
-.TH "YANG2DSDL" "1" "2023-11-03" "yang2dsdl-2.6.0" "User Manual"
+.\" Define V font for inline verbatim, using C font in formats
+.\" that render this, and otherwise B font.
+.ie "\f[CB]x\f[]"x" \{\
+. ftr V B
+. ftr VI BI
+. ftr VB B
+. ftr VBI BI
+.\}
+.el \{\
+. ftr V CR
+. ftr VI CI
+. ftr VB CB
+. ftr VBI CBI
+.\}
+.TH "YANG2DSDL" "1" "2024-05-23" "yang2dsdl-2.6.1" "User Manual"
 .hy
 .SH NAME
 .PP
 yang2dsdl - translates YANG data models to DSDL schemas and validates
 instance documents.
 .SH SYNOPSIS
 .PP
@@ -137,15 +151,15 @@
 If necessary, the script could be easily modified for use with other
 RELAX NG validators and/or XSLT1 processors supporting EXSLT.
 .SH OPTIONS
 .TP
 \f[B]-b\f[R] \f[I]basename\f[R]
 Specifies the basename of files in which the output schemas are stored.
 The default is the concatenation of the names of all input YANG modules
-connected with the underscore character \[dq]_\[dq].
+connected with the underscore character \[lq]_\[lq].
 This option is mandatory if \f[B]-s\f[R] is used.
 .TP
 \f[B]-d\f[R] \f[I]dir\f[R]
 Specifies the directory for output files.
 By default they are stored in the current directory.
 .TP
 \f[B]-h\f[R]
```

### Comparing `pyang-2.6.0/modules/iana/iana-crypt-hash.yang` & `pyang-2.6.1/modules/iana/iana-crypt-hash.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/iana/iana-hardware.yang` & `pyang-2.6.1/modules/iana/iana-hardware.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/iana/iana-if-type.yang` & `pyang-2.6.1/modules/iana/iana-if-type.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/iana/iana-routing-types.yang` & `pyang-2.6.1/modules/iana/iana-routing-types.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-access-control-list.yang` & `pyang-2.6.1/modules/ietf/ietf-access-control-list.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-acldns.yang` & `pyang-2.6.1/modules/ietf/ietf-acldns.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-alarms-x733.yang` & `pyang-2.6.1/modules/ietf/ietf-alarms-x733.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-alarms.yang` & `pyang-2.6.1/modules/ietf/ietf-alarms.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-datastores.yang` & `pyang-2.6.1/modules/ietf/ietf-datastores.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-dslite.yang` & `pyang-2.6.1/modules/ietf/ietf-dslite.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-ethertypes.yang` & `pyang-2.6.1/modules/ietf/ietf-ethertypes.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-hardware-state.yang` & `pyang-2.6.1/modules/ietf/ietf-hardware-state.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-hardware.yang` & `pyang-2.6.1/modules/ietf/ietf-hardware.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-i2rs-rib.yang` & `pyang-2.6.1/modules/ietf/ietf-i2rs-rib.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-inet-types.yang` & `pyang-2.6.1/modules/ietf/ietf-inet-types.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-interfaces.yang` & `pyang-2.6.1/modules/ietf/ietf-interfaces.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-ip.yang` & `pyang-2.6.1/modules/ietf/ietf-ip.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-ipv4-unicast-routing.yang` & `pyang-2.6.1/modules/ietf/ietf-ipv4-unicast-routing.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-ipv6-router-advertisements.yang` & `pyang-2.6.1/modules/ietf/ietf-ipv6-router-advertisements.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-ipv6-unicast-routing.yang` & `pyang-2.6.1/modules/ietf/ietf-ipv6-unicast-routing.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-key-chain.yang` & `pyang-2.6.1/modules/ietf/ietf-key-chain.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-l2vpn-svc.yang` & `pyang-2.6.1/modules/ietf/ietf-l2vpn-svc.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-l3-unicast-topology-state.yang` & `pyang-2.6.1/modules/ietf/ietf-l3-unicast-topology-state.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-l3-unicast-topology.yang` & `pyang-2.6.1/modules/ietf/ietf-l3-unicast-topology.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-l3vpn-svc.yang` & `pyang-2.6.1/modules/ietf/ietf-l3vpn-svc.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-lmap-common.yang` & `pyang-2.6.1/modules/ietf/ietf-lmap-common.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-lmap-control.yang` & `pyang-2.6.1/modules/ietf/ietf-lmap-control.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-lmap-report.yang` & `pyang-2.6.1/modules/ietf/ietf-lmap-report.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-logical-network-element.yang` & `pyang-2.6.1/modules/ietf/ietf-logical-network-element.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-mud.yang` & `pyang-2.6.1/modules/ietf/ietf-mud.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-nat.yang` & `pyang-2.6.1/modules/ietf/ietf-nat.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf-acm.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf-acm.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf-monitoring.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf-monitoring.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf-nmda.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf-nmda.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf-notifications.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf-notifications.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf-with-defaults.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf-with-defaults.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-netconf.yang` & `pyang-2.6.1/modules/ietf/ietf-netconf.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-network-instance.yang` & `pyang-2.6.1/modules/ietf/ietf-network-instance.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-network-state.yang` & `pyang-2.6.1/modules/ietf/ietf-network-state.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-network-topology-state.yang` & `pyang-2.6.1/modules/ietf/ietf-network-topology-state.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-network-topology.yang` & `pyang-2.6.1/modules/ietf/ietf-network-topology.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-network.yang` & `pyang-2.6.1/modules/ietf/ietf-network.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-origin.yang` & `pyang-2.6.1/modules/ietf/ietf-origin.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-packet-fields.yang` & `pyang-2.6.1/modules/ietf/ietf-packet-fields.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-restconf-monitoring.yang` & `pyang-2.6.1/modules/ietf/ietf-restconf-monitoring.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-restconf.yang` & `pyang-2.6.1/modules/ietf/ietf-restconf.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-routing-types.yang` & `pyang-2.6.1/modules/ietf/ietf-routing-types.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-routing.yang` & `pyang-2.6.1/modules/ietf/ietf-routing.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-common.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-common.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-community.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-community.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-engine.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-engine.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-notification.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-notification.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-proxy.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-proxy.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-ssh.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-ssh.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-target.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-target.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-tls.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-tls.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-tsm.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-tsm.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-usm.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-usm.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp-vacm.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp-vacm.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-snmp.yang` & `pyang-2.6.1/modules/ietf/ietf-snmp.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-subscribed-notifications.yang` & `pyang-2.6.1/modules/ietf/ietf-subscribed-notifications.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-system.yang` & `pyang-2.6.1/modules/ietf/ietf-system.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-voucher.yang` & `pyang-2.6.1/modules/ietf/ietf-voucher.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-vrrp.yang` & `pyang-2.6.1/modules/ietf/ietf-vrrp.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-x509-cert-to-name.yang` & `pyang-2.6.1/modules/ietf/ietf-x509-cert-to-name.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-library.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-library.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-metadata.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-metadata.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-patch.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-patch.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-push.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-push.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-schema-mount.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-schema-mount.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-smiv2.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-smiv2.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-structure-ext.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-structure-ext.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/modules/ietf/ietf-yang-types.yang` & `pyang-2.6.1/modules/ietf/ietf-yang-types.yang`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/context.py` & `pyang-2.6.1/pyang/context.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/error.py` & `pyang-2.6.1/pyang/error.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/grammar.py` & `pyang-2.6.1/pyang/grammar.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/hello.py` & `pyang-2.6.1/pyang/hello.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugin.py` & `pyang-2.6.1/pyang/plugin.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/bbf.py` & `pyang-2.6.1/pyang/plugins/bbf.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/capability.py` & `pyang-2.6.1/pyang/plugins/capability.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/check_update.py` & `pyang-2.6.1/pyang/plugins/check_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -157,14 +157,17 @@
         error.add_error_code(
             'CHK_RESTRICTION_CHANGED_v1.1', 3,
             "the %s has been illegally restricted"
             + " (RFC 7950: sec. 11, p5, bullet 3)")
         error.add_error_code(
             'CHK_UNION_TYPES', 3,
             "the member types in the union have changed")
+        error.add_error_code(
+            'CHK_IO_ERROR', 1,
+            "error %s: %s")
 
     def post_validate_ctx(self, ctx, modules):
         if not ctx.opts.check_update_from:
             return
 
         check_update(ctx, modules[0])
 
@@ -190,16 +193,17 @@
         p.setup_ctx(oldctx)
 
     for oldfilename in [ctx.opts.check_update_from] + ctx.opts.old_deviation:
         try:
             fd = io.open(oldfilename, "r", encoding="utf-8")
             text = fd.read()
         except IOError as ex:
-            sys.stderr.write("error %s: %s\n" % (oldfilename, ex))
-            sys.exit(1)
+            pos = error.Position(oldfilename)
+            err_add(ctx.errors, pos, "CHK_IO_ERROR", (oldfilename, ex))
+            return
         if oldfilename in ctx.opts.old_deviation:
             oldctx.add_module(oldfilename, text)
         else:
             oldmod = oldctx.add_module(oldfilename, text)
     oldctx.validate()
 
     ctx.errors.extend(oldctx.errors)
@@ -641,34 +645,52 @@
         # check if this unique was present before
         o = util.keysearch([s.arg for s in l], 1, oldunique)
         if o is not None:
             oldunique.remove(o)
         else:
             err_def_added(u, ctx)
 
+def chk_ordered_by(old, new, ctx):
+    oldorderedby = old.search_one('ordered-by')
+    neworderedby = new.search_one('ordered-by')
+    if oldorderedby is None and neworderedby is None:
+        pass
+    elif oldorderedby is None and neworderedby is not None and \
+         neworderedby.arg == 'user':
+        err_def_added(neworderedby, ctx)
+    elif oldorderedby is not None and neworderedby is None and \
+         oldorderedby.arg == 'user':
+        err_def_removed(oldorderedby, new, ctx)
+    elif oldorderedby is not None and neworderedby is not None and \
+         oldorderedby.arg != neworderedby.arg:
+        err_add(ctx.errors, neworderedby.pos, 'CHK_DEF_CHANGED',
+                ('ordered-by', neworderedby.arg, oldorderedby.arg))
+
 def chk_leaf(old, new, ctx):
     chk_type(old.search_one('type'), new.search_one('type'), ctx)
     chk_units(old, new, ctx)
     chk_default(old, new, ctx)
     chk_mandatory(old, new, ctx)
 
 def chk_leaf_list(old, new, ctx):
     chk_type(old.search_one('type'), new.search_one('type'), ctx)
     chk_units(old, new, ctx)
     chk_min_max(old, new, ctx)
+    chk_ordered_by(old, new, ctx)
 
 def chk_container(old, new, ctx):
     chk_presence(old, new, ctx)
     chk_i_children(old, new, ctx)
 
 def chk_list(old, new, ctx):
     chk_min_max(old, new, ctx)
     chk_key(old, new, ctx)
     chk_unique(old, new, ctx)
     chk_i_children(old, new, ctx)
+    chk_ordered_by(old, new, ctx)
 
 def chk_choice(old, new, ctx):
     chk_mandatory(old, new, ctx)
     chk_i_children(old, new, ctx)
 
 def chk_case(old, new, ctx):
     chk_i_children(old, new, ctx)
```

### Comparing `pyang-2.6.0/pyang/plugins/depend.py` & `pyang-2.6.1/pyang/plugins/depend.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/flatten.py` & `pyang-2.6.1/pyang/plugins/flatten.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/identifiers.py` & `pyang-2.6.1/pyang/plugins/identifiers.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/ietf.py` & `pyang-2.6.1/pyang/plugins/ietf.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/jsonxsl.py` & `pyang-2.6.1/pyang/plugins/jsonxsl.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/jstree.py` & `pyang-2.6.1/pyang/plugins/jstree.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/jtox.py` & `pyang-2.6.1/pyang/plugins/jtox.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/lint.py` & `pyang-2.6.1/pyang/plugins/lint.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/mef.py` & `pyang-2.6.1/pyang/plugins/mef.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/metadata.py` & `pyang-2.6.1/pyang/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/name.py` & `pyang-2.6.1/pyang/plugins/name.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/omni.py` & `pyang-2.6.1/pyang/plugins/omni.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/restconf.py` & `pyang-2.6.1/pyang/plugins/restconf.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/sample-xml-skeleton.py` & `pyang-2.6.1/pyang/plugins/sample-xml-skeleton.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/sid.py` & `pyang-2.6.1/pyang/plugins/sid.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/smi.py` & `pyang-2.6.1/pyang/plugins/smi.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/structure.py` & `pyang-2.6.1/pyang/plugins/structure.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/threegpp.py` & `pyang-2.6.1/pyang/plugins/threegpp.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/plugins/tree.py` & `pyang-2.6.1/pyang/plugins/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,29 +132,31 @@
     TARGET is the leafref path, with prefixes removed if possible.
 
   <if-features> is the list of features this node depends on, printed
     within curly brackets and a question mark "{...}?"
 """)
 
 def emit_tree(ctx, modules, fd, depth, llen, path):
-    printed_header = False
-
     def print_header(module):
-        nonlocal printed_header
         if not printed_header:
             bstr = ""
             b = module.search_one('belongs-to')
             if b is not None:
                 bstr = " (belongs-to %s)" % b.arg
             fd.write("%s: %s%s\n" % (module.keyword, module.arg, bstr))
-            printed_header = True
+            printed_header.append(None)
+
+    printed_header = []
 
     for module in modules:
         if printed_header:
             fd.write("\n")
+        del printed_header[:]
+            
+
         chs = [ch for ch in module.i_children
                if ch.keyword in statements.data_definition_keywords]
         if path is not None and len(path) > 0:
             chs = [ch for ch in chs if ch.arg == path[0]]
             chpath = path[1:]
         else:
             chpath = path
```

### Comparing `pyang-2.6.0/pyang/plugins/uml.py` & `pyang-2.6.1/pyang/plugins/uml.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,26 +282,26 @@
                     self.case_relation_symbol = "<|.."
             else:
                 sys.stderr.write("\"%s\" no valid argument to --uml-case=...,  valid arguments (one only): %s \n" %(ctx.opts.uml_case, relationship_strings))
         uses_strings = ("aggregation", "association", "composition", "dependency", "generalization", "realization")
         if ctx.opts.uml_uses != "":
             if ctx.opts.uml_uses in uses_strings:
                 if ctx.opts.uml_uses == 'generalization':
-                    self.uses_relation_symbol = "<|--"
+                    self.uses_relation_symbol = "--|>"
                 elif ctx.opts.uml_uses == 'aggregation':
                     self.uses_relation_symbol = "o--"
                 elif ctx.opts.uml_uses == 'association':
                     self.uses_relation_symbol = "--"
                 elif ctx.opts.uml_uses == 'composition':
                     self.uses_relation_symbol = "*--"
                 elif ctx.opts.uml_uses == 'dependency':
                     self.uses_relation_symbol = "..>"
                     self.uses_relation_label = "<<uses>>"
                 elif ctx.opts.uml_uses == 'realization':
-                    self.uses_relation_symbol = "<|.."
+                    self.uses_relation_symbol = "..|>"
             else:
                 sys.stderr.write("\"%s\" no valid argument to --uml-uses=...,  valid arguments (one only): %s \n" %(ctx.opts.uml_uses, uses_strings))
 
         self.ctx_filterfile = ctx.opts.uml_gen_filter_file
 
         self.ctx_truncate_augments = "augment" in ctx.opts.uml_truncate.split(",")
         self.ctx_truncate_leafrefs = "leafref" in ctx.opts.uml_truncate.split(",")
```

### Comparing `pyang-2.6.0/pyang/repository.py` & `pyang-2.6.1/pyang/repository.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/scripts/json2xml.py` & `pyang-2.6.1/pyang/scripts/json2xml.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/scripts/pyang_tool.py` & `pyang-2.6.1/pyang/scripts/pyang_tool.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/scripts/yang2html.py` & `pyang-2.6.1/pyang/scripts/yang2html.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/statements.py` & `pyang-2.6.1/pyang/statements.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,16 @@
         mod = stmt
     else:
         belongs_to = stmt.search_one('belongs-to')
         if belongs_to is not None and belongs_to.arg is not None:
             prefix = belongs_to.search_one('prefix')
             stmt.i_modulename = belongs_to.arg
             mod = ctx.get_module(stmt.i_modulename)
-            if mod is None:
+            if mod is None or not mod.i_is_validated:
+                # this happens if a submodule is validated standalone
                 mod = stmt
         else:
             stmt.i_modulename = ""
             mod = None
 
     if prefix is not None and prefix.arg is not None:
         stmt.i_prefixes[prefix.arg] = (stmt.arg, None)
@@ -2050,16 +2051,20 @@
                         err_add(ctx.errors, s.pos, 'KEY_BAD_SUBSTMT', substmt)
                 mandatory = ptr.search_one('mandatory')
                 if mandatory is not None and mandatory.arg == 'false':
                     err_add(ctx.errors, mandatory.pos,
                             'KEY_HAS_MANDATORY_FALSE', ())
 
                 if ptr.i_config != stmt.i_config:
-                    err_add(ctx.errors, ptr.search_one('config').pos,
-                            'KEY_BAD_CONFIG', name)
+                    cfg = ptr.search_one('config')
+                    if cfg is not None:
+                        pos = cfg.pos
+                    else:
+                        pos = ptr.pos
+                    err_add(ctx.errors, pos, 'KEY_BAD_CONFIG', name)
 
                 stmt.i_key.append(ptr)
                 ptr.i_is_key = True
                 found.append(x)
 
     def v_unique():
         # i_unique is a list of entries, one entry per 'unique' stmt.
```

### Comparing `pyang-2.6.0/pyang/syntax.py` & `pyang-2.6.1/pyang/syntax.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/transforms/edit.py` & `pyang-2.6.1/pyang/transforms/edit.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/translators/dsdl.py` & `pyang-2.6.1/pyang/translators/dsdl.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/translators/schemanode.py` & `pyang-2.6.1/pyang/translators/schemanode.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/translators/yang.py` & `pyang-2.6.1/pyang/translators/yang.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/translators/yin.py` & `pyang-2.6.1/pyang/translators/yin.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/types.py` & `pyang-2.6.1/pyang/types.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/util.py` & `pyang-2.6.1/pyang/util.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/xpath.py` & `pyang-2.6.1/pyang/xpath.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/xpath_lexer.py` & `pyang-2.6.1/pyang/xpath_lexer.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/xpath_parser.py` & `pyang-2.6.1/pyang/xpath_parser.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/yacc.py` & `pyang-2.6.1/pyang/yacc.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/yang_parser.py` & `pyang-2.6.1/pyang/yang_parser.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang/yin_parser.py` & `pyang-2.6.1/pyang/yin_parser.py`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/pyang.egg-info/PKG-INFO` & `pyang-2.6.1/pyang.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyang
-Version: 2.6.0
+Version: 2.6.1
 Summary: A YANG (RFC 6020/7950) validator and converter
 Home-page: https://github.com/mbj4668/pyang
 Author: Martin Bjorklund
-Author-email: mbj@tail-f.com
+Author-email: mbj4668@gmail.com
 License: BSD
 Keywords: YANG validator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyang-2.6.0/pyang.egg-info/SOURCES.txt` & `pyang-2.6.1/pyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/schema/edit-config-attributes.rng` & `pyang-2.6.1/schema/edit-config-attributes.rng`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/schema/hello-server.rng` & `pyang-2.6.1/schema/hello-server.rng`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/schema/relaxng-lib.rng` & `pyang-2.6.1/schema/relaxng-lib.rng`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/setup.py` & `pyang-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                   self.preprocess_files(opts["install"].get("prefix",
                                                             ("", None))[1])
             Distribution.run_commands(self)
 
 setup(name='pyang',
       version=pyang.__version__,
       author='Martin Bjorklund',
-      author_email='mbj@tail-f.com',
+      author_email='mbj4668@gmail.com',
       description="A YANG (RFC 6020/7950) validator and converter",
       long_description="An extensible  YANG (RFC 6020/7950) validator." + \
       " Provides a framework for plugins that can convert YANG modules" + \
       "to other formats.",
       url='https://github.com/mbj4668/pyang',
       install_requires = ["lxml"],
       license='BSD',
```

### Comparing `pyang-2.6.0/tools/images/case.png` & `pyang-2.6.1/tools/images/case.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/choice.png` & `pyang-2.6.1/tools/images/choice.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/container.png` & `pyang-2.6.1/tools/images/container.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/focus.png` & `pyang-2.6.1/tools/images/focus.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/leaf-list.png` & `pyang-2.6.1/tools/images/leaf-list.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/leaf-plus.png` & `pyang-2.6.1/tools/images/leaf-plus.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/leaf.png` & `pyang-2.6.1/tools/images/leaf.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/leafref.png` & `pyang-2.6.1/tools/images/leafref.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/list.png` & `pyang-2.6.1/tools/images/list.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/module.png` & `pyang-2.6.1/tools/images/module.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/tools/images/notification.png` & `pyang-2.6.1/tools/images/notification.png`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/basename.xsl` & `pyang-2.6.1/xslt/basename.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/dsrl2xslt.xsl` & `pyang-2.6.1/xslt/dsrl2xslt.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/gen-common.xsl` & `pyang-2.6.1/xslt/gen-common.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/gen-dsrl.xsl` & `pyang-2.6.1/xslt/gen-dsrl.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/gen-relaxng.xsl` & `pyang-2.6.1/xslt/gen-relaxng.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/gen-schematron.xsl` & `pyang-2.6.1/xslt/gen-schematron.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/iso_abstract_expand.xsl` & `pyang-2.6.1/xslt/iso_abstract_expand.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/iso_schematron_skeleton_for_xslt1.xsl` & `pyang-2.6.1/xslt/iso_schematron_skeleton_for_xslt1.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/iso_svrl_for_xslt1.xsl` & `pyang-2.6.1/xslt/iso_svrl_for_xslt1.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/jsonxsl-templates.xsl` & `pyang-2.6.1/xslt/jsonxsl-templates.xsl`

 * *Files identical despite different names*

### Comparing `pyang-2.6.0/xslt/svrl2text.xsl` & `pyang-2.6.1/xslt/svrl2text.xsl`

 * *Files identical despite different names*

